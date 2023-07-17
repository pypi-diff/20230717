# Comparing `tmp/openai_wrapper-0.5.9.tar.gz` & `tmp/openai_wrapper-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_wrapper-0.5.9.tar", max compression
+gzip compressed data, was "openai_wrapper-0.6.0.tar", max compression
```

## Comparing `openai_wrapper-0.5.9.tar` & `openai_wrapper-0.6.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0      134 2022-11-29 21:49:50.056076 openai_wrapper-0.5.9/openai_wrapper/__init__.py
--rw-r--r--   0        0        0    13150 2022-11-29 21:49:50.056076 openai_wrapper-0.5.9/openai_wrapper/completion.py
--rw-r--r--   0        0        0     2053 2022-11-29 21:49:50.056076 openai_wrapper-0.5.9/openai_wrapper/config.py
--rw-r--r--   0        0        0      729 2022-11-29 21:49:50.060076 openai_wrapper-0.5.9/pyproject.toml
--rw-r--r--   0        0        0      978 1970-01-01 00:00:00.000000 openai_wrapper-0.5.9/setup.py
--rw-r--r--   0        0        0      961 1970-01-01 00:00:00.000000 openai_wrapper-0.5.9/PKG-INFO
+-rw-r--r--   0        0        0      134 2023-07-17 09:00:29.816401 openai_wrapper-0.6.0/openai_wrapper/__init__.py
+-rw-r--r--   0        0        0     5605 2023-07-17 09:00:29.816401 openai_wrapper-0.6.0/openai_wrapper/chat_completion.py
+-rw-r--r--   0        0        0    18790 2023-07-17 09:00:29.816401 openai_wrapper-0.6.0/openai_wrapper/completion.py
+-rw-r--r--   0        0        0     2053 2023-07-17 09:00:29.816401 openai_wrapper-0.6.0/openai_wrapper/config.py
+-rw-r--r--   0        0        0     4367 2023-07-17 09:00:29.816401 openai_wrapper-0.6.0/openai_wrapper/embeddings.py
+-rw-r--r--   0        0        0      729 2023-07-17 09:00:29.820401 openai_wrapper-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      961 1970-01-01 00:00:00.000000 openai_wrapper-0.6.0/PKG-INFO
```

### Comparing `openai_wrapper-0.5.9/openai_wrapper/completion.py` & `openai_wrapper-0.6.0/openai_wrapper/completion.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-import json
 from datetime import datetime
-from typing import Callable, Dict, Any, List
+from typing import Callable, Dict, Any, List, Generator, Union
 
 import aiohttp
 from typeguard import typechecked
 
 from openai_wrapper.config import Config
 import logging
 
@@ -135,14 +134,89 @@
             return 0.0120
         elif model_name.startswith("davinci:"):
             return 0.1200
         else:
             logging.warning(f"No cost per 1000 tokens found for model {model_name}, using default value of 0.0")
             return 0.0
 
+    def stream_create(self,
+               prompt: str,
+               prompt_version: str,
+               prompt_version_description: str,
+               preprocess_prompt: Callable = _preprocess_prompt,
+               process_response: Callable = _process_response,
+               preprocess_prompt_args: Dict[Any, Any] = None,
+               process_response_args: Dict[Any, Any] = None) -> Union[Dict[Any, Any], Generator[Any, Any, Any]]:
+        """
+        Create a completion request and store it in MongoDB
+
+        Args:
+            prompt: The prompt to use for the completion
+            prompt_version: The version of the prompt (e.g. "1.0")
+            prompt_version_description: A description of the prompt version (e.g. "Added more diverse examples")
+            preprocess_prompt: A function that preprocesses the prompt
+            process_response: A function that processes the response
+            preprocess_prompt_args: A dictionary of arguments to pass to the preprocess_prompt function
+            process_response_args: A dictionary of arguments to pass to the process_response function
+
+        Returns:
+            A generator containing the completion responses, token by token
+        """
+        self.model_params['stream'] = True
+
+        if preprocess_prompt_args is None:
+            preprocess_prompt_args = {}
+        if process_response_args is None:
+            process_response_args = {}
+
+        preprocessed_prompt = preprocess_prompt(prompt, **preprocess_prompt_args)
+        response = self.openai_client.Completion.create(**self.model_params, prompt=preprocessed_prompt)
+
+        all_logprobs = {'tokens': [], 'token_logprobs': [], 'top_logprobs': [], 'text_offset': []}
+        completion_text = ""
+        token_number = 0
+
+        for resp in response:                
+            logprobs = resp['choices'][0]['logprobs']                
+            all_logprobs['tokens'].extend(logprobs['tokens'])
+            all_logprobs['token_logprobs'].extend(logprobs['token_logprobs'])
+            all_logprobs['top_logprobs'].extend(logprobs['top_logprobs'])
+            all_logprobs['text_offset'].extend(logprobs['text_offset'])
+            
+            completion_text += resp['choices'][0]['text']  
+            token_number += 1
+            yield resp
+        
+        openai_response = resp.__dict__['_previous']
+        openai_response['choices'][0]['logprobs'] = all_logprobs
+        openai_response['choices'][0]['text'] = completion_text
+
+        request_costs = self._calculate_request_costs(token_number)
+
+        document = {
+            "prompt": preprocessed_prompt,
+            "prompt_version": prompt_version,
+            "prompt_version_description": prompt_version_description,
+            "completion_text":  completion_text,
+            "openai_response": openai_response,
+            "model_params": self.model_params,
+            "created_at": str(datetime.utcnow()),
+            "experiment_metadata": self.experiment_metadata,
+            "project_metadata": self.project_metadata,
+            "request_cost_in_usd": request_costs
+        }
+
+        if self.extra_params is not None:
+            document.update(self.extra_params)
+
+        mongo_db = self.mongo_client[self.config.mongo_db_name]
+        mongo_collection = mongo_db[self.use_case_name]
+        mongo_collection.insert_one(document)
+
+    
     def create(self,
                prompt: str,
                prompt_version: str,
                prompt_version_description: str,
                preprocess_prompt: Callable = _preprocess_prompt,
                process_response: Callable = _process_response,
                preprocess_prompt_args: Dict[Any, Any] = None,
@@ -194,14 +268,15 @@
 
         mongo_db = self.mongo_client[self.config.mongo_db_name]
         mongo_collection = mongo_db[self.use_case_name]
         mongo_collection.insert_one(document)
 
         return document
 
+
     async def async_create(self,
                            prompt: str,
                            prompt_version: str,
                            prompt_version_description: str,
                            preprocess_prompt: Callable = _preprocess_prompt,
                            process_response: Callable = _process_response,
                            preprocess_prompt_args: Dict[Any, Any] = None,
@@ -225,15 +300,15 @@
             preprocess_prompt_args = {}
         if process_response_args is None:
             process_response_args = {}
 
         logging.info(f"Sending async request to OpenAI with params: {self.model_params}")
         preprocessed_prompt = preprocess_prompt(prompt, **preprocess_prompt_args)
         self.model_params["prompt"] = preprocessed_prompt
-        request_headers = {"Authorization": f"Bearer {self.openai_client.api_key}",
+        request_headers = {"Authorization": f"Bearer {self.config.openai_api_key}",
                            "Content-Type": "application/json"}
         try:
             async with aiohttp.ClientSession() as session:
                 async with session.post("https://api.openai.com/v1/completions",
                                         headers=request_headers,
                                         json=self.model_params) as resp:
                     response = await resp.json()
@@ -263,15 +338,15 @@
                     mongo_db = self.async_mongo_client[self.config.mongo_db_name]
                     mongo_collection = mongo_db[self.use_case_name]
                     await mongo_collection.insert_one(document)
 
                     return document
         except Exception as e:
             logging.error(f"Error in async request: {e}")
-            return {}
+            raise e
 
     def get_completions_for_prompt(self, prompt: str, prompt_version: str = None) -> List[Dict[Any, Any]]:
         """
         Get all completions for a given prompt
 
         Args:
             prompt: The prompt to get completions for
@@ -324,7 +399,58 @@
         Get all existing use cases (e.g. MongoDB collections)
 
         Returns:
             A list of use-cases/collections
         """
         mongo_db = config.mongo_client[config.mongo_db_name]
         return list(mongo_db.list_collection_names())
+    
+    def save_to_mongo(self,
+               prompt: str,
+               response: dict,
+               prompt_version: str,
+               prompt_version_description: str,
+               process_response: Callable = _process_response,
+               process_response_args: Dict[Any, Any] = None) -> Dict[Any, Any]:
+        """
+        Save the given prompt and OpenAI response to MongoDB. This functions is for use cases where you want to save the prompt and response without calling the OpenAI API.
+
+        Args:
+            prompt: The prompt submitted to OpenAI
+            response: The response object OpenAI API returned as completion
+            prompt_version: The version of the prompt (e.g. "1.0")
+            prompt_version_description: A description of the prompt version (e.g. "Added more diverse examples")
+            process_response: A function that processes the response
+            preprocess_prompt_args: A dictionary of arguments to pass to the preprocess_prompt function
+            process_response_args: A dictionary of arguments to pass to the process_response function
+
+        Returns:
+            A dictionary containing the completion request and response
+        """
+
+     
+        if process_response is not None:
+            response = process_response(response, **process_response_args)
+
+        request_costs = self._calculate_request_costs(response["usage"]["total_tokens"])
+
+        document = {
+            "prompt": prompt,
+            "prompt_version": prompt_version,
+            "prompt_version_description": prompt_version_description,
+            "completion_text": response["choices"][0]["text"],
+            "openai_response": response.__dict__['_previous'],
+            "model_params": self.model_params,
+            "created_at": str(datetime.utcnow()),
+            "experiment_metadata": self.experiment_metadata,
+            "project_metadata": self.project_metadata,
+            "request_cost_in_usd": request_costs
+        }
+
+        if self.extra_params is not None:
+            document.update(self.extra_params)
+
+        mongo_db = self.mongo_client[self.config.mongo_db_name]
+        mongo_collection = mongo_db[self.use_case_name]
+        mongo_collection.insert_one(document)
+
+        return document
```

### Comparing `openai_wrapper-0.5.9/openai_wrapper/config.py` & `openai_wrapper-0.6.0/openai_wrapper/config.py`

 * *Files identical despite different names*

### Comparing `openai_wrapper-0.5.9/pyproject.toml` & `openai_wrapper-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "openai-wrapper"
-version = "0.5.9"
+version = "0.6.0"
 description = "A wrapper for OpenAI's python API which wraps around the openAI functions and stores the request, response and metadata to MongoDB. The stored data can be used to fine tune GPT-3 models or HuggingFace models."
 authors = ["AI Team <datascience@prosus.com>"]
 license = "MIT License"
 
 [tool.poetry.dependencies]
 python = "^3.7.1"
-openai = "^0.25.0"
+openai = "^0.27.2"
 pymongo = "^4.2.0"
 dnspython = "^2.2.1"
 typeguard = "^2.13.3"
 configobj = "^5.0.6"
 aiohttp = "^3.8.3"
 motor = "^3.1.1"
```

### Comparing `openai_wrapper-0.5.9/PKG-INFO` & `openai_wrapper-0.6.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-wrapper
-Version: 0.5.9
+Version: 0.6.0
 Summary: A wrapper for OpenAI's python API which wraps around the openAI functions and stores the request, response and metadata to MongoDB. The stored data can be used to fine tune GPT-3 models or HuggingFace models.
 License: MIT
 Author: AI Team
 Author-email: datascience@prosus.com
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,10 +12,10 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
 Requires-Dist: configobj (>=5.0.6,<6.0.0)
 Requires-Dist: dnspython (>=2.2.1,<3.0.0)
 Requires-Dist: motor (>=3.1.1,<4.0.0)
-Requires-Dist: openai (>=0.25.0,<0.26.0)
+Requires-Dist: openai (>=0.27.2,<0.28.0)
 Requires-Dist: pymongo (>=4.2.0,<5.0.0)
 Requires-Dist: typeguard (>=2.13.3,<3.0.0)
```

