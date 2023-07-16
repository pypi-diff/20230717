# Comparing `tmp/scale_llm_engine-0.0.0b0.tar.gz` & `tmp/scale_llm_engine-0.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scale_llm_engine-0.0.0b0.tar", max compression
+gzip compressed data, was "scale_llm_engine-0.0.0b1.tar", max compression
```

## Comparing `scale_llm_engine-0.0.0b0.tar` & `scale_llm_engine-0.0.0b1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1006 2023-07-15 16:31:10.656012 scale_llm_engine-0.0.0b0/README.md
--rw-r--r--   0        0        0     1059 2023-07-15 17:24:52.423107 scale_llm_engine-0.0.0b0/llmengine/__init__.py
--rw-r--r--   0        0        0     5746 2023-07-15 17:24:30.933268 scale_llm_engine-0.0.0b0/llmengine/api_engine.py
--rw-r--r--   0        0        0    17835 2023-07-15 16:31:10.659325 scale_llm_engine-0.0.0b0/llmengine/client.py
--rw-r--r--   0        0        0     7962 2023-07-15 16:31:10.659701 scale_llm_engine-0.0.0b0/llmengine/completion.py
--rw-r--r--   0        0        0     8154 2023-07-15 17:24:30.934470 scale_llm_engine-0.0.0b0/llmengine/data_types.py
--rw-r--r--   0        0        0     1639 2023-07-15 17:24:30.935531 scale_llm_engine-0.0.0b0/llmengine/errors.py
--rw-r--r--   0        0        0     4254 2023-07-15 16:31:10.660754 scale_llm_engine-0.0.0b0/llmengine/fine_tuning.py
--rw-r--r--   0        0        0     2069 2023-07-15 16:31:10.661087 scale_llm_engine-0.0.0b0/llmengine/model.py
--rw-r--r--   0        0        0      807 2023-07-15 17:24:52.427224 scale_llm_engine-0.0.0b0/pyproject.toml
--rw-r--r--   0        0        0     1903 1970-01-01 00:00:00.000000 scale_llm_engine-0.0.0b0/PKG-INFO
+-rw-r--r--   0        0        0     1006 2023-07-16 19:49:15.428915 scale_llm_engine-0.0.0b1/README.md
+-rw-r--r--   0        0        0     1434 2023-07-16 22:32:20.465394 scale_llm_engine-0.0.0b1/llmengine/__init__.py
+-rw-r--r--   0        0        0     5716 2023-07-16 21:02:55.721851 scale_llm_engine-0.0.0b1/llmengine/api_engine.py
+-rw-r--r--   0        0        0    17749 2023-07-16 21:37:09.852272 scale_llm_engine-0.0.0b1/llmengine/client.py
+-rw-r--r--   0        0        0     9561 2023-07-16 21:37:09.852593 scale_llm_engine-0.0.0b1/llmengine/completion.py
+-rw-r--r--   0        0        0     8506 2023-07-16 21:37:09.852948 scale_llm_engine-0.0.0b1/llmengine/data_types.py
+-rw-r--r--   0        0        0     2745 2023-07-16 19:49:15.429730 scale_llm_engine-0.0.0b1/llmengine/errors.py
+-rw-r--r--   0        0        0     4179 2023-07-16 21:37:09.853211 scale_llm_engine-0.0.0b1/llmengine/fine_tuning.py
+-rw-r--r--   0        0        0     2083 2023-07-16 19:49:15.429911 scale_llm_engine-0.0.0b1/llmengine/model.py
+-rw-r--r--   0        0        0      807 2023-07-16 22:32:20.462460 scale_llm_engine-0.0.0b1/pyproject.toml
+-rw-r--r--   0        0        0     1903 1970-01-01 00:00:00.000000 scale_llm_engine-0.0.0b1/PKG-INFO
```

### Comparing `scale_llm_engine-0.0.0b0/README.md` & `scale_llm_engine-0.0.0b1/README.md`

 * *Files identical despite different names*

### Comparing `scale_llm_engine-0.0.0b0/llmengine/api_engine.py` & `scale_llm_engine-0.0.0b1/llmengine/api_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,17 +19,15 @@
     return SCALE_API_KEY or "root"
 
 
 def assert_self_hosted(func):
     @wraps(func)
     def inner(*args, **kwargs):
         if SPELLBOOK_API_URL == LLM_ENGINE_BASE_PATH:
-            raise ValueError(
-                "This feature is only available for self-hosted users."
-            )
+            raise ValueError("This feature is only available for self-hosted users.")
         return func(*args, **kwargs)
 
     return inner
 
 
 class APIEngine:
     @classmethod
```

### Comparing `scale_llm_engine-0.0.0b0/llmengine/client.py` & `scale_llm_engine-0.0.0b1/llmengine/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import json
 import os
 from typing import AsyncIterator, Dict, Iterator, Optional
 
 import requests
 from aiohttp import BasicAuth, ClientSession, ClientTimeout
-from pydantic import ValidationError
 from llmengine.errors import parse_error
 from llmengine.types import (
-    CancelFineTuneJobResponse,
+    CancelFineTuneResponse,
     CompletionStreamV1Request,
     CompletionStreamV1Response,
     CompletionSyncV1Request,
     CompletionSyncV1Response,
-    CreateFineTuneJobRequest,
-    CreateFineTuneJobResponse,
-    GetFineTuneJobResponse,
-    ListFineTuneJobResponse,
+    CreateFineTuneRequest,
+    CreateFineTuneResponse,
+    GetFineTuneResponse,
+    ListFineTunesResponse,
 )
+from pydantic import ValidationError
 
 SPELLBOOK_API_URL = "https://api.spellbook.scale.com"
 
 
 def get_sync_inference_url(base_url, model_name):
     return os.path.join(base_url, f"v1/llm/completions-sync?model_endpoint_name={model_name}")
 
@@ -180,15 +180,15 @@
         self,
         training_file: str,
         validation_file: str,
         model_name: str,
         base_model: str,
         fine_tuning_method: str,
         hyperparameters: Dict[str, str],
-    ) -> CreateFineTuneJobResponse:
+    ) -> CreateFineTuneResponse:
         """
         Create a fine-tuning job
 
         Args:
             training_file (`str`):
                 Path to file of training dataset
             validation_file (`str`):
@@ -199,18 +199,18 @@
                 Base model to train from
             fine_tuning_method (`str`):
                 Fine-tuning method
             hyperparameters (`str`):
                 Hyperparameters
 
         Returns:
-            CreateFineTuneJobResponse: ID of the created fine-tuning job
+            CreateFineTuneResponse: ID of the created fine-tuning job
         """
         # Validate parameters
-        request = CreateFineTuneJobRequest(
+        request = CreateFineTuneRequest(
             training_file=training_file,
             validation_file=validation_file,
             model_name=model_name,
             base_model=base_model,
             fine_tuning_method=fine_tuning_method,
             hyperparameters=hyperparameters,
         )
@@ -220,82 +220,82 @@
             json=request.dict(),
             auth=(self.api_key, ""),
             timeout=self.timeout,
         )
         payload = resp.json()
         if resp.status_code != 200:
             raise parse_error(resp.status_code, payload)
-        return CreateFineTuneJobResponse.parse_obj(payload)
+        return CreateFineTuneResponse.parse_obj(payload)
 
     def get_fine_tune_job(
         self,
         fine_tune_id: str,
-    ) -> GetFineTuneJobResponse:
+    ) -> GetFineTuneResponse:
         """
         Get status of a fine-tuning job
 
         Args:
             fine_tune_id (`str`):
                 ID of the fine-tuning job
 
         Returns:
-            GetFineTuneJobResponse: ID and status of the requested job
+            GetFineTuneResponse: ID and status of the requested job
         """
         resp = requests.get(
             f"{get_fine_tune_url(self.base_url)}/{fine_tune_id}",
             auth=(self.api_key, ""),
             timeout=self.timeout,
         )
         payload = resp.json()
         if resp.status_code != 200:
             raise parse_error(resp.status_code, payload)
-        return GetFineTuneJobResponse.parse_obj(payload)
+        return GetFineTuneResponse.parse_obj(payload)
 
     def list_fine_tune_jobs(
         self,
-    ) -> ListFineTuneJobResponse:
+    ) -> ListFineTunesResponse:
         """
         List fine-tuning jobs
 
         Returns:
-            ListFineTuneJobResponse: list of all fine-tuning jobs and their statuses
+            ListFineTunesResponse: list of all fine-tuning jobs and their statuses
         """
         resp = requests.get(
             get_fine_tune_url(self.base_url),
             auth=(self.api_key, ""),
             timeout=self.timeout,
         )
         payload = resp.json()
         if resp.status_code != 200:
             raise parse_error(resp.status_code, payload)
-        return ListFineTuneJobResponse.parse_obj(payload)
+        return ListFineTunesResponse.parse_obj(payload)
 
     def cancel_fine_tune_job(
         self,
         fine_tune_id: str,
-    ) -> CancelFineTuneJobResponse:
+    ) -> CancelFineTuneResponse:
         """
         Cancel a fine-tuning job
 
         Args:
             fine_tune_id (`str`):
                 ID of the fine-tuning job
 
         Returns:
-            CancelFineTuneJobResponse: whether the cancellation was successful
+            CancelFineTuneResponse: whether the cancellation was successful
         """
         resp = requests.put(
             f"{get_fine_tune_url(self.base_url)}/{fine_tune_id}/cancel",
             auth=(self.api_key, ""),
             timeout=self.timeout,
         )
         payload = resp.json()
         if resp.status_code != 200:
             raise parse_error(resp.status_code, payload)
-        return CancelFineTuneJobResponse.parse_obj(payload)
+        return CancelFineTuneResponse.parse_obj(payload)
 
 
 class AsyncClient:
     """Asynchronous Client to make calls to a llmengine instance
 
      Example:
 
@@ -442,15 +442,15 @@
         self,
         training_file: str,
         validation_file: str,
         model_name: str,
         base_model: str,
         fine_tuning_method: str,
         hyperparameters: Dict[str, str],
-    ) -> CreateFineTuneJobResponse:
+    ) -> CreateFineTuneResponse:
         """
         Create a fine-tuning job
 
         Args:
             training_file (`str`):
                 Path to file of training dataset
             validation_file (`str`):
@@ -461,18 +461,18 @@
                 Base model to train from
             fine_tuning_method (`str`):
                 Fine-tuning method
             hyperparameters (`str`):
                 Hyperparameters
 
         Returns:
-            CreateFineTuneJobResponse: ID of the created fine-tuning job
+            CreateFineTuneResponse: ID of the created fine-tuning job
         """
         # Validate parameters
-        request = CreateFineTuneJobRequest(
+        request = CreateFineTuneRequest(
             training_file=training_file,
             validation_file=validation_file,
             model_name=model_name,
             base_model=base_model,
             fine_tuning_method=fine_tuning_method,
             hyperparameters=hyperparameters,
         )
@@ -481,77 +481,77 @@
             timeout=self.timeout, auth=BasicAuth(login=self.api_key)
         ) as session:
             async with session.post(get_fine_tune_url(self.base_url), json=request.dict()) as resp:
                 payload = await resp.json()
 
                 if resp.status != 200:
                     raise parse_error(resp.status, payload)
-                return CreateFineTuneJobResponse.parse_obj(payload)
+                return CreateFineTuneResponse.parse_obj(payload)
 
     async def get_fine_tune_job(
         self,
         fine_tune_id: str,
-    ) -> GetFineTuneJobResponse:
+    ) -> GetFineTuneResponse:
         """
         Get status of a fine-tuning job
 
         Args:
             fine_tune_id (`str`):
                 ID of the fine-tuning job
 
         Returns:
-            GetFineTuneJobResponse: ID and status of the requested job
+            GetFineTuneResponse: ID and status of the requested job
         """
         async with ClientSession(
             timeout=self.timeout, auth=BasicAuth(login=self.api_key)
         ) as session:
             async with session.get(f"{get_fine_tune_url(self.base_url)}/{fine_tune_id}") as resp:
                 payload = await resp.json()
 
                 if resp.status != 200:
                     raise parse_error(resp.status, payload)
-                return GetFineTuneJobResponse.parse_obj(payload)
+                return GetFineTuneResponse.parse_obj(payload)
 
     async def list_fine_tune_jobs(
         self,
-    ) -> ListFineTuneJobResponse:
+    ) -> ListFineTunesResponse:
         """
         List fine-tuning jobs
 
         Returns:
-            ListFineTuneJobResponse: list of all fine-tuning jobs and their statuses
+            ListFineTunesResponse: list of all fine-tuning jobs and their statuses
         """
         async with ClientSession(
             timeout=self.timeout, auth=BasicAuth(login=self.api_key)
         ) as session:
             async with session.get(get_fine_tune_url(self.base_url)) as resp:
                 payload = await resp.json()
 
                 if resp.status != 200:
                     raise parse_error(resp.status, payload)
-                return ListFineTuneJobResponse.parse_obj(payload)
+                return ListFineTunesResponse.parse_obj(payload)
 
     async def cancel_fine_tune_job(
         self,
         fine_tune_id: str,
-    ) -> CancelFineTuneJobResponse:
+    ) -> CancelFineTuneResponse:
         """
         Cancel a fine-tuning job
 
         Args:
             fine_tune_id (`str`):
                 ID of the fine-tuning job
 
         Returns:
-            CancelFineTuneJobResponse: whether the cancellation was successful
+            CancelFineTuneResponse: whether the cancellation was successful
         """
         async with ClientSession(
             timeout=self.timeout, auth=BasicAuth(login=self.api_key)
         ) as session:
             async with session.put(
                 f"{get_fine_tune_url(self.base_url)}/{fine_tune_id}/cancel"
             ) as resp:
                 payload = await resp.json()
 
                 if resp.status != 200:
                     raise parse_error(resp.status, payload)
-                return CancelFineTuneJobResponse.parse_obj(payload)
+                return CancelFineTuneResponse.parse_obj(payload)
```

### Comparing `scale_llm_engine-0.0.0b0/llmengine/completion.py` & `scale_llm_engine-0.0.0b1/llmengine/completion.py`

 * *Files 16% similar despite different names*

```diff
@@ -27,30 +27,73 @@
         stream: bool = False,
     ) -> Union[CompletionSyncV1Response, AsyncIterable[CompletionStreamV1Response]]:
         """
         Create a completion task asynchronously.
 
         Example without token streaming:
             ```python
+            import asyncio
             from llmengine import Completion
 
             async def main():
-                response_stream = await Completion.acreate(
+                response = await Completion.acreate(
                     model_name="llama-7b",
                     prompt="Hello, my name is",
                     max_new_tokens=10,
                     temperature=0.2,
                 )
-                async for response in response_stream:
-                    print(response.output.text)
+                print(response.json())
+
+            asyncio.run(main())
             ```
 
-        JSON Response:
-        ```json
-        ```
+        JSON response:
+            ```json
+            {
+                "outputs": [
+                    {
+                        "text": "_______ and I am a _______",
+                        "num_prompt_tokens": null,
+                        "num_completion_tokens": 10
+                    }
+                ]
+            }
+            ```
+
+        Example with token streaming:
+            ```python
+            import asyncio
+            from llmengine import Completion
+
+            async def main():
+                stream = await Completion.acreate(
+                    model_name="llama-7b",
+                    prompt="why is the sky blue?",
+                    max_new_tokens=5,
+                    temperature=0.2,
+                    stream=True,
+                )
+
+                async for response in stream:
+                    if response.output:
+                        print(response.json())
+
+            asyncio.run(main())
+            ```
+
+        JSON responses:
+            ```json
+            [
+                {"output": {"text": "\\n", "finished": false, "num_prompt_tokens": null, "num_completion_tokens": 1}},
+                {"output": {"text": "The", "finished": false, "num_prompt_tokens": null, "num_completion_tokens": 2}},
+                {"output": {"text": " sky", "finished": false, "num_prompt_tokens": null, "num_completion_tokens": 3}},
+                {"output": {"text": " is", "finished": false, "num_prompt_tokens": null, "num_completion_tokens": 4}},
+                {"output": {"text": " blue", "finished": true, "num_prompt_tokens": null, "num_completion_tokens": 5}}
+            ]
+            ```
 
 
         Args:
             model_name (str):
                 Model name to use for inference
             prompt (str):
                 Input text
@@ -65,15 +108,17 @@
                 `Iterator[CompletionStreamV1Response]`.
 
         Returns:
             response (Union[CompletionSyncV1Response, AsyncIterable[CompletionStreamV1Response]]): generated response or iterator of response chunks
         """
         if stream:
 
-            async def _acreate_stream(**kwargs) -> AsyncIterable[CompletionStreamV1Response]:
+            async def _acreate_stream(
+                **kwargs,
+            ) -> AsyncIterable[CompletionStreamV1Response]:
                 data = CompletionStreamV1Request(**kwargs).dict()
                 response = cls.apost_stream(
                     resource_name=f"v1/llm/completions-stream?model_endpoint_name={model_name}",
                     data=data,
                     timeout=timeout,
                 )
                 async for chunk in response:
@@ -121,57 +166,55 @@
 
             response = Completion.create(
                 model_name="llama-7b",
                 prompt="Hello, my name is",
                 max_new_tokens=10,
                 temperature=0.2,
             )
-            print(response)
+            print(response.json())
             ```
 
         JSON Response:
             ```json
             {
-                "status": "SUCCESS",
                 "outputs": [
                     {
                         "text": "\\nThe sky is blue because of the way the light is reflected off the molecules in the air.\\nWhat is the sky blue?\\nThe sky is blue because of the way the light is reflected off the molecules in the air.\\nWhat is the sky blue?\\nThe sky is blue because of the way the light is reflected off the molecules in the air. The sky is blue because of the way the light is reflected off the molecules in the air.\\nWhat is",
                         "num_prompt_tokens": null,
                         "num_completion_tokens": 100
                     }
-                ],
-                "traceback": null
+                ]
             }
             ```
 
         Example request with token streaming:
             ```python
             from llmengine import Completion
 
             stream = Completion.create(
                 model_name="llama-7b",
                 prompt="why is the sky blue?",
                 max_new_tokens=5,
                 temperature=0.2,
                 stream=True,
             )
-    
+
             for response in stream:
                 if response.output:
-                    print(response.output)
+                    print(response.json())
             ```
 
-        Stream response JSONs:
+        JSON responses:
             ```json
             [
-                {"text": "\\n", "finished": false, "num_prompt_tokens": null, "num_completion_tokens": 1},
-                {"text": "I", "finished": false, "num_prompt_tokens": null, "num_completion_tokens": 2},
-                {"text": "'", "finished": false, "num_prompt_tokens": null, "num_completion_tokens": 3},
-                {"text": "m", "finished": false, "num_prompt_tokens": null, "num_completion_tokens": 4},
-                {"text": " not", "finished": true, "num_prompt_tokens": null, "num_completion_tokens": 5}
+                {"output": {"text": "\\n", "finished": false, "num_prompt_tokens": null, "num_completion_tokens": 1}},
+                {"output": {"text": "I", "finished": false, "num_prompt_tokens": null, "num_completion_tokens": 2}},
+                {"output": {"text": "'", "finished": false, "num_prompt_tokens": null, "num_completion_tokens": 3}},
+                {"output": {"text": "m", "finished": false, "num_prompt_tokens": null, "num_completion_tokens": 4}},
+                {"output": {"text": " not", "finished": true, "num_prompt_tokens": null, "num_completion_tokens": 5}}
             ]
             ```
 
         Args:
             model_name (str):
                 Model name to use for inference
             prompt (str):
```

### Comparing `scale_llm_engine-0.0.0b0/llmengine/data_types.py` & `scale_llm_engine-0.0.0b1/llmengine/data_types.py`

 * *Files 14% similar despite different names*

```diff
@@ -247,55 +247,43 @@
     output: Optional[CompletionStreamOutput] = None
     """Completion output."""
 
     traceback: Optional[str] = None
     """Traceback if the task failed."""
 
 
-# everything below copied from hosted_model_inference/hosted_model_inference/common/dtos/llms.py
+# everything below copied from scaleapi/packages/spellbook-backend/server/spellbook_server/dtos.py
 
 
-class CreateFineTuneJobRequest(BaseModel):
-    training_file: str
-    """Path to file of training dataset"""
-    validation_file: str
-    """Path to file of validation dataset"""
-    model_name: str
-    """Name of the fine-tuned model"""
-    base_model: str  # TODO enum
-    """Base model to train from"""
-    fine_tuning_method: str  # TODO enum
-    """Fine-tuning method"""
-    hyperparameters: Dict[str, str]  # TODO validated somewhere else
-    """Hyperparameters"""
-
-
-class CreateFineTuneJobResponse(BaseModel):
-    fine_tune_id: str
-    """ID of the created fine-tuning job"""
+class CreateFineTuneRequest(BaseModel):
+    model: str = Field(..., description="Identifier of base model to train from.")
+    training_file: str = Field(..., description="Path to file of training dataset. Dataset must be a csv with columns 'prompt' and 'response'.")
+    validation_file: Optional[str] = Field(default=None, description="Path to file of validation dataset. Has the same format as training_file. If not provided, we will generate a split from the training dataset.")
+    hyperparameters: Optional[Dict[str, Any]] = Field(default=None, description="Hyperparameters to pass in to training job.")
+    suffix: Optional[str] = Field(default=None, description="Optional user-provided identifier suffix for the fine-tuned model.")
+
+
+class CreateFineTuneResponse(BaseModel):
+    fine_tune_id: str = Field(..., description="ID of the created fine-tuning job.")
 
 
 class BatchJobStatus(str, Enum):
     PENDING = "PENDING"
     RUNNING = "RUNNING"
     SUCCESS = "SUCCESS"
     FAILURE = "FAILURE"
     CANCELLED = "CANCELLED"
     UNDEFINED = "UNDEFINED"
     TIMEOUT = "TIMEOUT"
 
 
-class GetFineTuneJobResponse(BaseModel):
-    fine_tune_id: str
-    """ID of the requested job"""
-    status: BatchJobStatus
-    """Status of the requested job"""
+class GetFineTuneResponse(BaseModel):
+    fine_tune_id: str = Field(..., description="ID of the requested job.")
+    status: BatchJobStatus = Field(..., description="Status of the requested job.")
 
 
-class ListFineTuneJobResponse(BaseModel):
-    jobs: List[GetFineTuneJobResponse]
-    """List of fine-tuning jobs and their statuses"""
+class ListFineTunesResponse(BaseModel):
+    jobs: List[GetFineTuneResponse] = Field(..., description="List of fine-tuning jobs and their statuses.")
 
 
-class CancelFineTuneJobResponse(BaseModel):
-    success: bool
-    """Whether cancellation was successful"""
+class CancelFineTuneResponse(BaseModel):
+    success: bool = Field(..., description="Whether cancellation was successful.")
```

### Comparing `scale_llm_engine-0.0.0b0/llmengine/fine_tuning.py` & `scale_llm_engine-0.0.0b1/llmengine/fine_tuning.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,33 @@
-from typing import Dict
+from typing import Dict, Optional
 
-from llmengine.api_engine import APIEngine, DEFAULT_TIMEOUT
+from llmengine.api_engine import DEFAULT_TIMEOUT, APIEngine
 from llmengine.data_types import (
-    CancelFineTuneJobResponse,
-    CreateFineTuneJobRequest,
-    CreateFineTuneJobResponse,
-    GetFineTuneJobResponse,
-    ListFineTuneJobResponse,
+    CancelFineTuneResponse,
+    CreateFineTuneRequest,
+    CreateFineTuneResponse,
+    GetFineTuneResponse,
+    ListFineTunesResponse,
 )
 
 
 class FineTune(APIEngine):
     """
     FineTune API. This API is used to fine-tune models.
     """
 
     @classmethod
     def create(
         cls,
+        model: str,
         training_file: str,
-        validation_file: str,
-        model_name: str,
-        base_model: str,
-        fine_tuning_method: str,
-        hyperparameters: Dict[str, str],
-    ) -> CreateFineTuneJobResponse:
+        validation_file: Optional[str] = None,
+        hyperparameters: Optional[Dict[str, str]] = None,
+        suffix: Optional[str] = None,
+    ) -> CreateFineTuneResponse:
         """
         Create a fine-tuning job.
 
         Example:
             ```python
             from llmengine import FineTune
 
@@ -59,36 +58,35 @@
                 Base model to train from
             fine_tuning_method (`str`):
                 Fine-tuning method
             hyperparameters (`str`):
                 Hyperparameters
 
         Returns:
-            CreateFineTuneJobResponse: ID of the created fine-tuning job
+            CreateFineTuneResponse: ID of the created fine-tuning job
         """
-        request = CreateFineTuneJobRequest(
+        request = CreateFineTuneRequest(
+            model=model,
             training_file=training_file,
             validation_file=validation_file,
-            model_name=model_name,
-            base_model=base_model,
-            fine_tuning_method=fine_tuning_method,
             hyperparameters=hyperparameters,
+            suffix=suffix,
         )
         response = cls.post_sync(
             resource_name="v1/llm/fine-tunes",
             data=request.dict(),
             timeout=DEFAULT_TIMEOUT,
         )
-        return CreateFineTuneJobResponse.parse_obj(response)
+        return CreateFineTuneResponse.parse_obj(response)
 
     @classmethod
     def retrieve(
         cls,
         fine_tune_id: str,
-    ) -> GetFineTuneJobResponse:
+    ) -> GetFineTuneResponse:
         """
         Get status of a fine-tuning job
 
         Example:
             ```python
             from llmengine import FineTune
 
@@ -105,21 +103,21 @@
 
 
         Args:
             fine_tune_id (`str`):
                 ID of the fine-tuning job
 
         Returns:
-            GetFineTuneJobResponse: ID and status of the requested job
+            GetFineTuneResponse: ID and status of the requested job
         """
         response = cls.get(f"v1/llm/fine-tunes/{fine_tune_id}", timeout=DEFAULT_TIMEOUT)
-        return GetFineTuneJobResponse.parse_obj(response)
+        return GetFineTuneResponse.parse_obj(response)
 
     @classmethod
-    def list(cls) -> ListFineTuneJobResponse:
+    def list(cls) -> ListFineTunesResponse:
         """
         List fine-tuning jobs
 
         Example:
             ```python
             from llmengine import FineTune
 
@@ -128,29 +126,31 @@
             ```
 
         JSON Response:
             ```json
             ```
 
         Returns:
-            ListFineTuneJobResponse: list of all fine-tuning jobs and their statuses
+            ListFineTunesResponse: list of all fine-tuning jobs and their statuses
         """
         response = cls.get("v1/llm/fine-tunes", timeout=DEFAULT_TIMEOUT)
-        return ListFineTuneJobResponse.parse_obj(response)
+        return ListFineTunesResponse.parse_obj(response)
 
     @classmethod
-    def cancel(cls, fine_tune_id: str) -> CancelFineTuneJobResponse:
+    def cancel(cls, fine_tune_id: str) -> CancelFineTuneResponse:
         """
         Cancel a fine-tuning job
 
 
         Args:
             fine_tune_id (`str`):
                 ID of the fine-tuning job
 
         Returns:
-            CancelFineTuneJobResponse: whether the cancellation was successful
+            CancelFineTuneResponse: whether the cancellation was successful
         """
         response = cls.put(
-            f"v1/llm/fine-tunes/{fine_tune_id}/cancel", data=None, timeout=DEFAULT_TIMEOUT
+            f"v1/llm/fine-tunes/{fine_tune_id}/cancel",
+            data=None,
+            timeout=DEFAULT_TIMEOUT,
         )
-        return CancelFineTuneJobResponse.parse_obj(response)
+        return CancelFineTuneResponse.parse_obj(response)
```

### Comparing `scale_llm_engine-0.0.0b0/llmengine/model.py` & `scale_llm_engine-0.0.0b1/llmengine/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,13 @@
-from llmengine.api_engine import APIEngine, DEFAULT_TIMEOUT, assert_self_hosted
+from llmengine.api_engine import DEFAULT_TIMEOUT, APIEngine, assert_self_hosted
 from llmengine.data_types import (
-    ListLLMModelEndpointsV1Response, GetLLMModelEndpointV1Response, CreateLLMModelEndpointV1Response, CreateLLMModelEndpointV1Request
+    CreateLLMModelEndpointV1Request,
+    CreateLLMModelEndpointV1Response,
+    GetLLMModelEndpointV1Response,
+    ListLLMModelEndpointsV1Response,
 )
 
 
 class Model(APIEngine):
     """
     Model API. This API is used to retrieve, list, and create models.
 
@@ -13,14 +16,15 @@
         ```python
         from llmengine import Model
 
         response = Model.list()
         print(response)
         ```
     """
+
     @classmethod
     @assert_self_hosted
     def create(
         cls,
         model_name: str,
     ) -> CreateLLMModelEndpointV1Response:
         """
```

### Comparing `scale_llm_engine-0.0.0b0/pyproject.toml` & `scale_llm_engine-0.0.0b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scale-llm-engine"
-version = "0.0.0.beta0"
+version = "0.0.0.beta1"
 description = "Scale LLM Engine Python client"
 license = "Apache-2.0"
 authors = ["Phil Chen <phil.chen@scale.com>"]
 maintainers = ["Phil Chen <phil.chen@scale.com>"]
 readme = "README.md"
 homepage = "https://scaleapi.github.io/llm-engine/"
 repository = "https://github.com/scaleapi/llm-engine"
```

### Comparing `scale_llm_engine-0.0.0b0/PKG-INFO` & `scale_llm_engine-0.0.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scale-llm-engine
-Version: 0.0.0b0
+Version: 0.0.0b1
 Summary: Scale LLM Engine Python client
 Home-page: https://scaleapi.github.io/llm-engine/
 License: Apache-2.0
 Author: Phil Chen
 Author-email: phil.chen@scale.com
 Maintainer: Phil Chen
 Maintainer-email: phil.chen@scale.com
```

