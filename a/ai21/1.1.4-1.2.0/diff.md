# Comparing `tmp/ai21-1.1.4.tar.gz` & `tmp/ai21-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai21-1.1.4.tar", last modified: Sun Jun 11 11:53:46 2023, max compression
+gzip compressed data, was "ai21-1.2.0.tar", last modified: Mon Jul 17 16:00:06 2023, max compression
```

## Comparing `ai21-1.1.4.tar` & `ai21-1.2.0.tar`

### file list

```diff
@@ -1,47 +1,49 @@
-drwxr-xr-x   0 etang      (501) staff       (20)        0 2023-06-11 11:53:46.891493 ai21-1.1.4/
--rw-r--r--   0 etang      (501) staff       (20)     1065 2023-05-22 10:53:48.000000 ai21-1.1.4/LICENSE
--rw-r--r--   0 etang      (501) staff       (20)     4577 2023-06-11 11:53:46.891597 ai21-1.1.4/PKG-INFO
--rw-r--r--   0 etang      (501) staff       (20)     3595 2023-06-11 11:49:53.000000 ai21-1.1.4/README.md
-drwxr-xr-x   0 etang      (501) staff       (20)        0 2023-06-11 11:53:46.885805 ai21-1.1.4/ai21/
--rw-r--r--   0 etang      (501) staff       (20)     2164 2023-06-11 11:49:53.000000 ai21-1.1.4/ai21/AWS_utils.py
--rw-r--r--   0 etang      (501) staff       (20)      878 2023-06-11 11:49:53.000000 ai21-1.1.4/ai21/__init__.py
--rw-r--r--   0 etang      (501) staff       (20)      971 2023-05-22 10:53:48.000000 ai21-1.1.4/ai21/ai21_object.py
--rw-r--r--   0 etang      (501) staff       (20)     2055 2023-06-07 10:54:53.000000 ai21-1.1.4/ai21/ai21_studio_client.py
--rw-r--r--   0 etang      (501) staff       (20)      473 2023-05-22 10:53:48.000000 ai21-1.1.4/ai21/api_resources.py
--rw-r--r--   0 etang      (501) staff       (20)     2195 2023-06-11 11:49:53.000000 ai21-1.1.4/ai21/bedrock_client.py
--rw-r--r--   0 etang      (501) staff       (20)      250 2023-06-11 11:49:53.000000 ai21-1.1.4/ai21/constants.py
--rw-r--r--   0 etang      (501) staff       (20)     3273 2023-06-11 11:49:53.000000 ai21-1.1.4/ai21/errors.py
--rw-r--r--   0 etang      (501) staff       (20)     4034 2023-06-09 06:49:33.000000 ai21-1.1.4/ai21/http_client.py
-drwxr-xr-x   0 etang      (501) staff       (20)        0 2023-06-11 11:53:46.889648 ai21-1.1.4/ai21/modules/
--rw-r--r--   0 etang      (501) staff       (20)        0 2023-05-22 10:53:48.000000 ai21-1.1.4/ai21/modules/__init__.py
--rw-r--r--   0 etang      (501) staff       (20)     2009 2023-06-07 10:54:53.000000 ai21-1.1.4/ai21/modules/completion.py
--rw-r--r--   0 etang      (501) staff       (20)      856 2023-05-22 10:53:48.000000 ai21-1.1.4/ai21/modules/custom_model.py
--rw-r--r--   0 etang      (501) staff       (20)      646 2023-05-22 10:53:48.000000 ai21-1.1.4/ai21/modules/dataset.py
--rw-r--r--   0 etang      (501) staff       (20)      445 2023-06-07 10:54:53.000000 ai21-1.1.4/ai21/modules/destination.py
--rw-r--r--   0 etang      (501) staff       (20)     1801 2023-06-07 10:54:53.000000 ai21-1.1.4/ai21/modules/experimental.py
--rw-r--r--   0 etang      (501) staff       (20)      986 2023-06-07 10:54:53.000000 ai21-1.1.4/ai21/modules/gec.py
--rw-r--r--   0 etang      (501) staff       (20)      925 2023-06-07 10:54:53.000000 ai21-1.1.4/ai21/modules/improvements.py
--rw-r--r--   0 etang      (501) staff       (20)     1000 2023-06-07 10:54:53.000000 ai21-1.1.4/ai21/modules/paraphrase.py
--rw-r--r--   0 etang      (501) staff       (20)     1104 2023-06-07 10:54:53.000000 ai21-1.1.4/ai21/modules/question_answering.py
-drwxr-xr-x   0 etang      (501) staff       (20)        0 2023-06-11 11:53:46.891336 ai21-1.1.4/ai21/modules/resources/
--rw-r--r--   0 etang      (501) staff       (20)        0 2023-05-22 10:53:48.000000 ai21-1.1.4/ai21/modules/resources/__init__.py
--rw-r--r--   0 etang      (501) staff       (20)      585 2023-05-22 10:53:48.000000 ai21-1.1.4/ai21/modules/resources/ai21_module.py
--rw-r--r--   0 etang      (501) staff       (20)      371 2023-05-22 10:53:48.000000 ai21-1.1.4/ai21/modules/resources/creatable_resource.py
--rw-r--r--   0 etang      (501) staff       (20)     1605 2023-06-07 10:54:53.000000 ai21-1.1.4/ai21/modules/resources/execution_utils.py
--rw-r--r--   0 etang      (501) staff       (20)      352 2023-05-22 10:53:48.000000 ai21-1.1.4/ai21/modules/resources/listable_resource.py
--rw-r--r--   0 etang      (501) staff       (20)     2059 2023-06-07 10:54:53.000000 ai21-1.1.4/ai21/modules/resources/nlp_task.py
--rw-r--r--   0 etang      (501) staff       (20)      387 2023-05-22 10:53:48.000000 ai21-1.1.4/ai21/modules/resources/retrievable_resource.py
--rw-r--r--   0 etang      (501) staff       (20)      476 2023-05-22 10:53:48.000000 ai21-1.1.4/ai21/modules/resources/upload_resource.py
--rw-r--r--   0 etang      (501) staff       (20)      915 2023-06-07 10:54:53.000000 ai21-1.1.4/ai21/modules/segmentation.py
--rw-r--r--   0 etang      (501) staff       (20)     1164 2023-06-08 08:05:25.000000 ai21-1.1.4/ai21/modules/summarize.py
--rw-r--r--   0 etang      (501) staff       (20)      693 2023-06-07 10:54:53.000000 ai21-1.1.4/ai21/modules/tokenization.py
--rw-r--r--   0 etang      (501) staff       (20)     3038 2023-06-09 06:54:03.000000 ai21-1.1.4/ai21/utils.py
--rw-r--r--   0 etang      (501) staff       (20)       22 2023-06-11 11:53:44.000000 ai21-1.1.4/ai21/version.py
-drwxr-xr-x   0 etang      (501) staff       (20)        0 2023-06-11 11:53:46.886745 ai21-1.1.4/ai21.egg-info/
--rw-r--r--   0 etang      (501) staff       (20)     4577 2023-06-11 11:53:46.000000 ai21-1.1.4/ai21.egg-info/PKG-INFO
--rw-r--r--   0 etang      (501) staff       (20)     1070 2023-06-11 11:53:46.000000 ai21-1.1.4/ai21.egg-info/SOURCES.txt
--rw-r--r--   0 etang      (501) staff       (20)        1 2023-06-11 11:53:46.000000 ai21-1.1.4/ai21.egg-info/dependency_links.txt
--rw-r--r--   0 etang      (501) staff       (20)       40 2023-06-11 11:53:46.000000 ai21-1.1.4/ai21.egg-info/requires.txt
--rw-r--r--   0 etang      (501) staff       (20)        5 2023-06-11 11:53:46.000000 ai21-1.1.4/ai21.egg-info/top_level.txt
--rwxr-xr-x   0 etang      (501) staff       (20)      155 2023-06-11 11:53:46.891881 ai21-1.1.4/setup.cfg
--rwxr-xr-x   0 etang      (501) staff       (20)      600 2023-06-07 10:54:53.000000 ai21-1.1.4/setup.py
+drwxr-xr-x   0 amirkoblyansky   (501) staff       (20)        0 2023-07-17 16:00:06.225975 ai21-1.2.0/
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)     1065 2023-03-25 06:53:34.000000 ai21-1.2.0/LICENSE
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)     4577 2023-07-17 16:00:06.226103 ai21-1.2.0/PKG-INFO
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)     3595 2023-07-15 13:04:46.000000 ai21-1.2.0/README.md
+drwxr-xr-x   0 amirkoblyansky   (501) staff       (20)        0 2023-07-17 16:00:06.218183 ai21-1.2.0/ai21/
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)     2317 2023-07-17 14:08:40.000000 ai21-1.2.0/ai21/AWS_utils.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      919 2023-07-17 13:50:26.000000 ai21-1.2.0/ai21/__init__.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      971 2023-06-08 14:30:41.000000 ai21-1.2.0/ai21/ai21_object.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)     2055 2023-06-08 14:30:41.000000 ai21-1.2.0/ai21/ai21_studio_client.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      473 2023-06-08 14:30:41.000000 ai21-1.2.0/ai21/api_resources.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)     2195 2023-07-15 13:04:46.000000 ai21-1.2.0/ai21/bedrock_client.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      250 2023-07-15 13:04:46.000000 ai21-1.2.0/ai21/constants.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)     3273 2023-07-15 13:04:46.000000 ai21-1.2.0/ai21/errors.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)     4034 2023-06-08 14:30:41.000000 ai21-1.2.0/ai21/http_client.py
+drwxr-xr-x   0 amirkoblyansky   (501) staff       (20)        0 2023-07-17 16:00:06.222946 ai21-1.2.0/ai21/modules/
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)        0 2023-06-08 14:30:41.000000 ai21-1.2.0/ai21/modules/__init__.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)     1993 2023-07-17 14:08:40.000000 ai21-1.2.0/ai21/modules/completion.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      856 2023-07-17 10:29:52.000000 ai21-1.2.0/ai21/modules/custom_model.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      654 2023-07-17 13:48:31.000000 ai21-1.2.0/ai21/modules/dataset.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      534 2023-07-17 14:08:40.000000 ai21-1.2.0/ai21/modules/destination.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)     1740 2023-07-17 14:08:40.000000 ai21-1.2.0/ai21/modules/experimental.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      970 2023-07-17 14:08:40.000000 ai21-1.2.0/ai21/modules/gec.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      925 2023-06-08 14:30:41.000000 ai21-1.2.0/ai21/modules/improvements.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)     1368 2023-07-17 13:48:31.000000 ai21-1.2.0/ai21/modules/library.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      984 2023-07-17 14:08:40.000000 ai21-1.2.0/ai21/modules/paraphrase.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)     1088 2023-07-17 14:08:40.000000 ai21-1.2.0/ai21/modules/question_answering.py
+drwxr-xr-x   0 amirkoblyansky   (501) staff       (20)        0 2023-07-17 16:00:06.225731 ai21-1.2.0/ai21/modules/resources/
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)        0 2023-06-08 14:30:41.000000 ai21-1.2.0/ai21/modules/resources/__init__.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      585 2023-07-17 10:29:12.000000 ai21-1.2.0/ai21/modules/resources/ai21_module.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      371 2023-06-08 14:30:41.000000 ai21-1.2.0/ai21/modules/resources/creatable_resource.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)     1793 2023-07-17 14:08:40.000000 ai21-1.2.0/ai21/modules/resources/execution_utils.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      352 2023-06-08 14:30:41.000000 ai21-1.2.0/ai21/modules/resources/listable_resource.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)     2059 2023-07-17 10:29:07.000000 ai21-1.2.0/ai21/modules/resources/nlp_task.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      391 2023-07-17 13:52:59.000000 ai21-1.2.0/ai21/modules/resources/retrievable_resource.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      404 2023-07-17 13:52:59.000000 ai21-1.2.0/ai21/modules/resources/updatable_resource.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      480 2023-07-17 13:48:31.000000 ai21-1.2.0/ai21/modules/resources/upload_resource.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      915 2023-06-08 14:30:41.000000 ai21-1.2.0/ai21/modules/segmentation.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)     1148 2023-07-17 14:08:40.000000 ai21-1.2.0/ai21/modules/summarize.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      693 2023-06-08 14:30:41.000000 ai21-1.2.0/ai21/modules/tokenization.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)     3038 2023-06-08 14:30:41.000000 ai21-1.2.0/ai21/utils.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)       22 2023-07-17 14:09:39.000000 ai21-1.2.0/ai21/version.py
+drwxr-xr-x   0 amirkoblyansky   (501) staff       (20)        0 2023-07-17 16:00:06.219067 ai21-1.2.0/ai21.egg-info/
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)     4577 2023-07-17 16:00:06.000000 ai21-1.2.0/ai21.egg-info/PKG-INFO
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)     1139 2023-07-17 16:00:06.000000 ai21-1.2.0/ai21.egg-info/SOURCES.txt
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)        1 2023-07-17 16:00:06.000000 ai21-1.2.0/ai21.egg-info/dependency_links.txt
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)       40 2023-07-17 16:00:06.000000 ai21-1.2.0/ai21.egg-info/requires.txt
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)        5 2023-07-17 16:00:06.000000 ai21-1.2.0/ai21.egg-info/top_level.txt
+-rwxr-xr-x   0 amirkoblyansky   (501) staff       (20)      155 2023-07-17 16:00:06.226533 ai21-1.2.0/setup.cfg
+-rwxr-xr-x   0 amirkoblyansky   (501) staff       (20)      600 2023-06-08 14:21:53.000000 ai21-1.2.0/setup.py
```

### Comparing `ai21-1.1.4/LICENSE` & `ai21-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ai21-1.1.4/PKG-INFO` & `ai21-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai21
-Version: 1.1.4
+Version: 1.2.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: ai21 labs
 Author-email: support@ai21.com
 License: MIT
 Description: # AI21 Studio Client
         Python client for the AI21 Studio API
```

### Comparing `ai21-1.1.4/README.md` & `ai21-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ai21-1.1.4/ai21/AWS_utils.py` & `ai21-1.2.0/ai21/AWS_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 import json
 import re
+from typing import Optional
 
 import boto3
+import sagemaker
 from botocore.exceptions import ClientError
 
 import ai21
 from ai21.errors import ServerError, ServiceUnavailable, BadRequest, APIError
 from ai21.http_client import handle_non_success_response
 from ai21.utils import convert_to_ai21_object, log_error
 
 sm_runtime = boto3.client("sagemaker-runtime", region_name=ai21.aws_region)
 
 
-def invoke_sm_endpoint(endpoint_name: str, input_json: str):
+def invoke_sm_endpoint(endpoint_name: str, input_json: str, sm_session: Optional[sagemaker.session.Session]):
+    sm_session = sm_session if sm_session else sm_runtime
+
     try:
-        response = sm_runtime.invoke_endpoint(
+        response = sm_session.invoke_endpoint(
             EndpointName=endpoint_name,
             ContentType="application/json",
             Accept="application/json",
             Body=input_json,
         )
 
         response_body = json.load(response["Body"])
```

### Comparing `ai21-1.1.4/ai21/__init__.py` & `ai21-1.2.0/ai21/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from ai21.modules.custom_model import CustomModel
 from ai21.modules.experimental import Experimental
 from ai21.modules.paraphrase import Paraphrase
 from ai21.modules.summarize import Summarize
 from ai21.modules.segmentation import Segmentation
 from ai21.modules.improvements import Improvements
 from ai21.modules.question_answering import Answer
+from ai21.modules.library import Library
 from ai21.modules.gec import GEC
 from ai21.modules.destination import BedrockDestination, AI21Destination, BedrockModelID, SageMakerDestination
 
 
 api_key = None
 organization = None
 application = None
```

### Comparing `ai21-1.1.4/ai21/ai21_object.py` & `ai21-1.2.0/ai21/ai21_object.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.4/ai21/ai21_studio_client.py` & `ai21-1.2.0/ai21/ai21_studio_client.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.4/ai21/bedrock_client.py` & `ai21-1.2.0/ai21/bedrock_client.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.4/ai21/errors.py` & `ai21-1.2.0/ai21/errors.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.4/ai21/http_client.py` & `ai21-1.2.0/ai21/http_client.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.4/ai21/modules/completion.py` & `ai21-1.2.0/ai21/modules/completion.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
             unsupported_fields=['model', 'custom_model'],
             params=params,
         )
 
     @classmethod
     def _execute_sm(cls, destination: SageMakerDestination, params):
         return execute_sm_request(
-            endpoint_name=destination.endpoint_name,
+            destination=destination,
             unsupported_fields=['model', 'custom_model'],
             params=params,
         )
 
     @classmethod
     def _execute_studio_api(cls, params):
         validate_mandatory_field(
```

### Comparing `ai21-1.1.4/ai21/modules/custom_model.py` & `ai21-1.2.0/ai21/modules/custom_model.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.4/ai21/modules/experimental.py` & `ai21-1.2.0/ai21/modules/experimental.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,31 @@
-from ai21.modules.completion import Completion
 from ai21.modules.destination import SageMakerDestination
 from ai21.modules.resources.ai21_module import AI21Module
 from ai21.modules.resources.execution_utils import execute_studio_request, execute_sm_request
 from ai21.modules.resources.nlp_task import NLPTask
 from ai21.utils import validate_mandatory_field
 
 
 class Experimental(AI21Module):
+
     @classmethod
     def embed(cls, **params):
         validate_mandatory_field(key='texts', call_name="embed_experimental", params=params, validate_type=True,
                                  expected_type=list)
         url = cls.get_base_url(**params)
         url = f'{url}/experimental/embed'
         return execute_studio_request(task_url=url, params=params)
 
     @classmethod
     def answer(cls, **params):
         return _AnswerExperimental.execute(**params)
 
 
 class _AnswerExperimental(NLPTask):
+
     MODULE_NAME = 'answer_experimental'
 
     @classmethod
     def _get_call_name(cls) -> str:
         return cls.MODULE_NAME
 
     @classmethod
@@ -32,14 +33,14 @@
         validate_mandatory_field(key='context', call_name="answer_experimental", params=params, validate_type=True,
                                  expected_type=str)
         validate_mandatory_field(key='question', call_name="answer_experimental", params=params, validate_type=True,
                                  expected_type=str)
 
     @classmethod
     def _execute_sm(cls, destination: SageMakerDestination, params):
-        return execute_sm_request(endpoint_name=destination.endpoint_name, params=params)
+        return execute_sm_request(destination=destination, params=params)
 
     @classmethod
     def _execute_studio_api(cls, params):
         url = cls.get_base_url(**params)
         url = f'{url}/experimental/answer'
         return execute_studio_request(task_url=url, params=params)
```

### Comparing `ai21-1.1.4/ai21/modules/gec.py` & `ai21-1.2.0/ai21/modules/paraphrase.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from ai21.modules.destination import SageMakerDestination
 from ai21.modules.resources.execution_utils import execute_sm_request, execute_studio_request
 
 from ai21.modules.resources.nlp_task import NLPTask
 from ai21.utils import validate_mandatory_field
 
 
-class GEC(NLPTask):
-    MODULE_NAME = 'gec'
+class Paraphrase(NLPTask):
+    MODULE_NAME = 'paraphrase'
 
     @classmethod
     def _get_call_name(cls) -> str:
         return cls.MODULE_NAME
 
     @classmethod
     def _validate_params(cls, params):
         validate_mandatory_field(key='text', call_name=cls.MODULE_NAME, params=params, validate_type=True,
                                  expected_type=str)
 
     @classmethod
     def _execute_sm(cls, destination: SageMakerDestination, params):
-        return execute_sm_request(endpoint_name=destination.endpoint_name, params=params)
+        return execute_sm_request(destination=destination, params=params)
 
     @classmethod
     def _execute_studio_api(cls, params):
         url = cls.get_base_url(**params)
         url = f'{url}/{cls.MODULE_NAME}'
         return execute_studio_request(task_url=url, params=params)
```

### Comparing `ai21-1.1.4/ai21/modules/improvements.py` & `ai21-1.2.0/ai21/modules/improvements.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.4/ai21/modules/paraphrase.py` & `ai21-1.2.0/ai21/modules/gec.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from ai21.modules.destination import SageMakerDestination
 from ai21.modules.resources.execution_utils import execute_sm_request, execute_studio_request
 
 from ai21.modules.resources.nlp_task import NLPTask
 from ai21.utils import validate_mandatory_field
 
 
-class Paraphrase(NLPTask):
-    MODULE_NAME = 'paraphrase'
+class GEC(NLPTask):
+    MODULE_NAME = 'gec'
 
     @classmethod
     def _get_call_name(cls) -> str:
         return cls.MODULE_NAME
 
     @classmethod
     def _validate_params(cls, params):
         validate_mandatory_field(key='text', call_name=cls.MODULE_NAME, params=params, validate_type=True,
                                  expected_type=str)
 
     @classmethod
     def _execute_sm(cls, destination: SageMakerDestination, params):
-        return execute_sm_request(endpoint_name=destination.endpoint_name, params=params)
+        return execute_sm_request(destination=destination, params=params)
 
     @classmethod
     def _execute_studio_api(cls, params):
         url = cls.get_base_url(**params)
         url = f'{url}/{cls.MODULE_NAME}'
         return execute_studio_request(task_url=url, params=params)
```

### Comparing `ai21-1.1.4/ai21/modules/question_answering.py` & `ai21-1.2.0/ai21/modules/question_answering.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,12 +16,12 @@
         validate_mandatory_field(key='context', call_name=cls.MODULE_NAME, params=params, validate_type=True,
                                  expected_type=str)
         validate_mandatory_field(key='question', call_name=cls.MODULE_NAME, params=params, validate_type=True,
                                  expected_type=str)
 
     @classmethod
     def _execute_sm(cls, destination: SageMakerDestination, params):
-        return execute_sm_request(endpoint_name=destination.endpoint_name, params=params)
+        return execute_sm_request(destination=destination, params=params)
 
     @classmethod
     def _execute_studio_api(cls, params):
         raise NotImplementedError(f'The module {cls.MODULE_NAME} is not implemented for the non experimental endpoint')
```

### Comparing `ai21-1.1.4/ai21/modules/resources/ai21_module.py` & `ai21-1.2.0/ai21/modules/resources/ai21_module.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.4/ai21/modules/resources/execution_utils.py` & `ai21-1.2.0/ai21/modules/resources/execution_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 import json
 from typing import Optional, List
 
+from ai21.modules.destination import SageMakerDestination
 from ai21.ai21_studio_client import AI21StudioClient
 from ai21.utils import validate_mandatory_field, validate_unsupported_field
 
 
 def execute_studio_request(task_url: str, params, method: str = 'POST'):
     client = AI21StudioClient(**params)
     return client.execute_http_request(method=method, url=task_url, params=params)
 
 
-def execute_sm_request(endpoint_name: str, params, mandatory_fields=None, unsupported_fields=None):
-    call_name = f'Sagemaker {endpoint_name}'
+def execute_sm_request(destination: SageMakerDestination, params, mandatory_fields=None, unsupported_fields=None):
+    call_name = f'Sagemaker {destination.endpoint_name}'
 
     if mandatory_fields is not None:
         for mandatory_field in mandatory_fields:
             validate_mandatory_field(mandatory_field, call_name, params)
 
     if unsupported_fields is not None:
         for unsupported_field in unsupported_fields:
             validate_unsupported_field(key=unsupported_field, call_name=call_name, params=params)
 
     input_json = json.dumps(params)
 
     from ai21.AWS_utils import invoke_sm_endpoint  # import here because boto3 exists only in AWS mode
 
-    return invoke_sm_endpoint(endpoint_name, input_json)
+    return invoke_sm_endpoint(
+        endpoint_name=destination.endpoint_name,
+        input_json=input_json,
+        sm_session=destination.sm_session,
+    )
 
 
 def execute_bedrock_request(model_id: str, params, unsupported_fields: Optional[List[str]] = None):
     call_name = 'Bedrock'
 
     if unsupported_fields is not None:
         for unsupported_field in unsupported_fields:
```

### Comparing `ai21-1.1.4/ai21/modules/resources/nlp_task.py` & `ai21-1.2.0/ai21/modules/resources/nlp_task.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.4/ai21/modules/segmentation.py` & `ai21-1.2.0/ai21/modules/segmentation.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.4/ai21/modules/summarize.py` & `ai21-1.2.0/ai21/modules/summarize.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,8 +22,8 @@
     def _execute_studio_api(cls, params):
         url = cls.get_base_url(**params)
         url = f'{url}/{cls.MODULE_NAME}'
         return execute_studio_request(task_url=url, params=params)
 
     @classmethod
     def _execute_sm(cls, destination: SageMakerDestination, params):
-        return execute_sm_request(endpoint_name=destination.endpoint_name, params=params)
+        return execute_sm_request(destination=destination, params=params)
```

### Comparing `ai21-1.1.4/ai21/modules/tokenization.py` & `ai21-1.2.0/ai21/modules/tokenization.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.4/ai21/utils.py` & `ai21-1.2.0/ai21/utils.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.4/ai21.egg-info/PKG-INFO` & `ai21-1.2.0/ai21.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai21
-Version: 1.1.4
+Version: 1.2.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: ai21 labs
 Author-email: support@ai21.com
 License: MIT
 Description: # AI21 Studio Client
         Python client for the AI21 Studio API
```

### Comparing `ai21-1.1.4/ai21.egg-info/SOURCES.txt` & `ai21-1.2.0/ai21.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -22,20 +22,22 @@
 ai21/modules/completion.py
 ai21/modules/custom_model.py
 ai21/modules/dataset.py
 ai21/modules/destination.py
 ai21/modules/experimental.py
 ai21/modules/gec.py
 ai21/modules/improvements.py
+ai21/modules/library.py
 ai21/modules/paraphrase.py
 ai21/modules/question_answering.py
 ai21/modules/segmentation.py
 ai21/modules/summarize.py
 ai21/modules/tokenization.py
 ai21/modules/resources/__init__.py
 ai21/modules/resources/ai21_module.py
 ai21/modules/resources/creatable_resource.py
 ai21/modules/resources/execution_utils.py
 ai21/modules/resources/listable_resource.py
 ai21/modules/resources/nlp_task.py
 ai21/modules/resources/retrievable_resource.py
+ai21/modules/resources/updatable_resource.py
 ai21/modules/resources/upload_resource.py
```

### Comparing `ai21-1.1.4/setup.py` & `ai21-1.2.0/setup.py`

 * *Files identical despite different names*

