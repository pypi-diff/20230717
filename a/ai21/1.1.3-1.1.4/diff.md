# Comparing `tmp/ai21-1.1.3.tar.gz` & `tmp/ai21-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai21-1.1.3.tar", last modified: Thu Jun  8 14:35:03 2023, max compression
+gzip compressed data, was "ai21-1.1.4.tar", last modified: Sun Jun 11 11:53:46 2023, max compression
```

## Comparing `ai21-1.1.3.tar` & `ai21-1.1.4.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 amirkoblyansky   (501) staff       (20)        0 2023-06-08 14:35:03.828075 ai21-1.1.3/
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     1065 2023-03-25 06:53:34.000000 ai21-1.1.3/LICENSE
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     4095 2023-06-08 14:35:03.828182 ai21-1.1.3/PKG-INFO
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     3161 2023-06-08 14:21:53.000000 ai21-1.1.3/README.md
-drwxr-xr-x   0 amirkoblyansky   (501) staff       (20)        0 2023-06-08 14:35:03.823254 ai21-1.1.3/ai21/
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     2209 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/AWS_utils.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      885 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/__init__.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      971 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/ai21_object.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     2055 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/ai21_studio_client.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      473 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/api_resources.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     1923 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/bedrock_client.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      246 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/constants.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     3084 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/errors.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     4034 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/http_client.py
-drwxr-xr-x   0 amirkoblyansky   (501) staff       (20)        0 2023-06-08 14:35:03.826472 ai21-1.1.3/ai21/modules/
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)        0 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/modules/__init__.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     2009 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/modules/completion.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      856 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/modules/custom_model.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      646 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/modules/dataset.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      445 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/modules/destination.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     1801 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/modules/experimental.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      986 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/modules/gec.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      925 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/modules/improvements.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     1000 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/modules/paraphrase.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     1104 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/modules/question_answering.py
-drwxr-xr-x   0 amirkoblyansky   (501) staff       (20)        0 2023-06-08 14:35:03.827901 ai21-1.1.3/ai21/modules/resources/
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)        0 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/modules/resources/__init__.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      585 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/modules/resources/ai21_module.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      371 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/modules/resources/creatable_resource.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     1605 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/modules/resources/execution_utils.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      352 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/modules/resources/listable_resource.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     2059 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/modules/resources/nlp_task.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      387 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/modules/resources/retrievable_resource.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      476 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/modules/resources/upload_resource.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      915 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/modules/segmentation.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     1164 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/modules/summarize.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      693 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/modules/tokenization.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     3038 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/utils.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)       22 2023-06-08 14:34:42.000000 ai21-1.1.3/ai21/version.py
-drwxr-xr-x   0 amirkoblyansky   (501) staff       (20)        0 2023-06-08 14:35:03.824090 ai21-1.1.3/ai21.egg-info/
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     4095 2023-06-08 14:35:03.000000 ai21-1.1.3/ai21.egg-info/PKG-INFO
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     1070 2023-06-08 14:35:03.000000 ai21-1.1.3/ai21.egg-info/SOURCES.txt
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)        1 2023-06-08 14:35:03.000000 ai21-1.1.3/ai21.egg-info/dependency_links.txt
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)       40 2023-06-08 14:35:03.000000 ai21-1.1.3/ai21.egg-info/requires.txt
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)        5 2023-06-08 14:35:03.000000 ai21-1.1.3/ai21.egg-info/top_level.txt
--rwxr-xr-x   0 amirkoblyansky   (501) staff       (20)      155 2023-06-08 14:35:03.828492 ai21-1.1.3/setup.cfg
--rwxr-xr-x   0 amirkoblyansky   (501) staff       (20)      600 2023-06-08 14:21:53.000000 ai21-1.1.3/setup.py
+drwxr-xr-x   0 etang      (501) staff       (20)        0 2023-06-11 11:53:46.891493 ai21-1.1.4/
+-rw-r--r--   0 etang      (501) staff       (20)     1065 2023-05-22 10:53:48.000000 ai21-1.1.4/LICENSE
+-rw-r--r--   0 etang      (501) staff       (20)     4577 2023-06-11 11:53:46.891597 ai21-1.1.4/PKG-INFO
+-rw-r--r--   0 etang      (501) staff       (20)     3595 2023-06-11 11:49:53.000000 ai21-1.1.4/README.md
+drwxr-xr-x   0 etang      (501) staff       (20)        0 2023-06-11 11:53:46.885805 ai21-1.1.4/ai21/
+-rw-r--r--   0 etang      (501) staff       (20)     2164 2023-06-11 11:49:53.000000 ai21-1.1.4/ai21/AWS_utils.py
+-rw-r--r--   0 etang      (501) staff       (20)      878 2023-06-11 11:49:53.000000 ai21-1.1.4/ai21/__init__.py
+-rw-r--r--   0 etang      (501) staff       (20)      971 2023-05-22 10:53:48.000000 ai21-1.1.4/ai21/ai21_object.py
+-rw-r--r--   0 etang      (501) staff       (20)     2055 2023-06-07 10:54:53.000000 ai21-1.1.4/ai21/ai21_studio_client.py
+-rw-r--r--   0 etang      (501) staff       (20)      473 2023-05-22 10:53:48.000000 ai21-1.1.4/ai21/api_resources.py
+-rw-r--r--   0 etang      (501) staff       (20)     2195 2023-06-11 11:49:53.000000 ai21-1.1.4/ai21/bedrock_client.py
+-rw-r--r--   0 etang      (501) staff       (20)      250 2023-06-11 11:49:53.000000 ai21-1.1.4/ai21/constants.py
+-rw-r--r--   0 etang      (501) staff       (20)     3273 2023-06-11 11:49:53.000000 ai21-1.1.4/ai21/errors.py
+-rw-r--r--   0 etang      (501) staff       (20)     4034 2023-06-09 06:49:33.000000 ai21-1.1.4/ai21/http_client.py
+drwxr-xr-x   0 etang      (501) staff       (20)        0 2023-06-11 11:53:46.889648 ai21-1.1.4/ai21/modules/
+-rw-r--r--   0 etang      (501) staff       (20)        0 2023-05-22 10:53:48.000000 ai21-1.1.4/ai21/modules/__init__.py
+-rw-r--r--   0 etang      (501) staff       (20)     2009 2023-06-07 10:54:53.000000 ai21-1.1.4/ai21/modules/completion.py
+-rw-r--r--   0 etang      (501) staff       (20)      856 2023-05-22 10:53:48.000000 ai21-1.1.4/ai21/modules/custom_model.py
+-rw-r--r--   0 etang      (501) staff       (20)      646 2023-05-22 10:53:48.000000 ai21-1.1.4/ai21/modules/dataset.py
+-rw-r--r--   0 etang      (501) staff       (20)      445 2023-06-07 10:54:53.000000 ai21-1.1.4/ai21/modules/destination.py
+-rw-r--r--   0 etang      (501) staff       (20)     1801 2023-06-07 10:54:53.000000 ai21-1.1.4/ai21/modules/experimental.py
+-rw-r--r--   0 etang      (501) staff       (20)      986 2023-06-07 10:54:53.000000 ai21-1.1.4/ai21/modules/gec.py
+-rw-r--r--   0 etang      (501) staff       (20)      925 2023-06-07 10:54:53.000000 ai21-1.1.4/ai21/modules/improvements.py
+-rw-r--r--   0 etang      (501) staff       (20)     1000 2023-06-07 10:54:53.000000 ai21-1.1.4/ai21/modules/paraphrase.py
+-rw-r--r--   0 etang      (501) staff       (20)     1104 2023-06-07 10:54:53.000000 ai21-1.1.4/ai21/modules/question_answering.py
+drwxr-xr-x   0 etang      (501) staff       (20)        0 2023-06-11 11:53:46.891336 ai21-1.1.4/ai21/modules/resources/
+-rw-r--r--   0 etang      (501) staff       (20)        0 2023-05-22 10:53:48.000000 ai21-1.1.4/ai21/modules/resources/__init__.py
+-rw-r--r--   0 etang      (501) staff       (20)      585 2023-05-22 10:53:48.000000 ai21-1.1.4/ai21/modules/resources/ai21_module.py
+-rw-r--r--   0 etang      (501) staff       (20)      371 2023-05-22 10:53:48.000000 ai21-1.1.4/ai21/modules/resources/creatable_resource.py
+-rw-r--r--   0 etang      (501) staff       (20)     1605 2023-06-07 10:54:53.000000 ai21-1.1.4/ai21/modules/resources/execution_utils.py
+-rw-r--r--   0 etang      (501) staff       (20)      352 2023-05-22 10:53:48.000000 ai21-1.1.4/ai21/modules/resources/listable_resource.py
+-rw-r--r--   0 etang      (501) staff       (20)     2059 2023-06-07 10:54:53.000000 ai21-1.1.4/ai21/modules/resources/nlp_task.py
+-rw-r--r--   0 etang      (501) staff       (20)      387 2023-05-22 10:53:48.000000 ai21-1.1.4/ai21/modules/resources/retrievable_resource.py
+-rw-r--r--   0 etang      (501) staff       (20)      476 2023-05-22 10:53:48.000000 ai21-1.1.4/ai21/modules/resources/upload_resource.py
+-rw-r--r--   0 etang      (501) staff       (20)      915 2023-06-07 10:54:53.000000 ai21-1.1.4/ai21/modules/segmentation.py
+-rw-r--r--   0 etang      (501) staff       (20)     1164 2023-06-08 08:05:25.000000 ai21-1.1.4/ai21/modules/summarize.py
+-rw-r--r--   0 etang      (501) staff       (20)      693 2023-06-07 10:54:53.000000 ai21-1.1.4/ai21/modules/tokenization.py
+-rw-r--r--   0 etang      (501) staff       (20)     3038 2023-06-09 06:54:03.000000 ai21-1.1.4/ai21/utils.py
+-rw-r--r--   0 etang      (501) staff       (20)       22 2023-06-11 11:53:44.000000 ai21-1.1.4/ai21/version.py
+drwxr-xr-x   0 etang      (501) staff       (20)        0 2023-06-11 11:53:46.886745 ai21-1.1.4/ai21.egg-info/
+-rw-r--r--   0 etang      (501) staff       (20)     4577 2023-06-11 11:53:46.000000 ai21-1.1.4/ai21.egg-info/PKG-INFO
+-rw-r--r--   0 etang      (501) staff       (20)     1070 2023-06-11 11:53:46.000000 ai21-1.1.4/ai21.egg-info/SOURCES.txt
+-rw-r--r--   0 etang      (501) staff       (20)        1 2023-06-11 11:53:46.000000 ai21-1.1.4/ai21.egg-info/dependency_links.txt
+-rw-r--r--   0 etang      (501) staff       (20)       40 2023-06-11 11:53:46.000000 ai21-1.1.4/ai21.egg-info/requires.txt
+-rw-r--r--   0 etang      (501) staff       (20)        5 2023-06-11 11:53:46.000000 ai21-1.1.4/ai21.egg-info/top_level.txt
+-rwxr-xr-x   0 etang      (501) staff       (20)      155 2023-06-11 11:53:46.891881 ai21-1.1.4/setup.cfg
+-rwxr-xr-x   0 etang      (501) staff       (20)      600 2023-06-07 10:54:53.000000 ai21-1.1.4/setup.py
```

### Comparing `ai21-1.1.3/LICENSE` & `ai21-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ai21-1.1.3/PKG-INFO` & `ai21-1.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai21
-Version: 1.1.3
+Version: 1.1.4
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: ai21 labs
 Author-email: support@ai21.com
 License: MIT
 Description: # AI21 Studio Client
         Python client for the AI21 Studio API
@@ -48,51 +48,57 @@
         This example uses a simple completion call with only prompt and maxTokens arguments supplied
         (all other completion settings are set to their defaults):
         ```python
         import ai21
         
         ai21.api_key = 'my_api_key'
         ai21.timeout_sec = 20
-        response = ai21.Completion.execute(model="j2-ultra", prompt="Write a news release in the voice of a global banking conglomerate announcing an unprecedented building campaign to expand and rebuild their corporate headquarters in Alpha Centauri.", maxTokens=200)
+        response = ai21.Completion.execute(
+            model="j2-ultra",
+            prompt="Write a news release in the voice of a global banking conglomerate announcing an unprecedented building campaign to expand and rebuild their corporate headquarters in Alpha Centauri.",
+            maxTokens=200,
+        )
         print(response)
         ```
         
         ### AWS Client
         This python SDK can also be used to invoke Jurassic models as a SageMaker (SM) endpoint or as an AWS Bedrock API.
         To activate this option, make sure to install with the extra AWS dependencies:
         
         `pip install -U "ai21[AWS]"`
         
         #### Sagemaker endpoint request
         You can then generate a completion by running:
         ```python
         import ai21
-        ai21.aws_region = 'us-east-1'
+        
         response = ai21.Completion.execute(
             destination=ai21.SageMakerDestination("<your_endpoint_name>"),
-            prompt="hello world",
-            maxTokens=20,
+            prompt="Write a news release in the voice of a global banking conglomerate announcing an unprecedented building campaign to expand and rebuild their corporate headquarters in Alpha Centauri.",
+            maxTokens=200,
         )
         
         print(response)
         ```
         
         #### Bedrock API request
-        
         You can use one of the models offered in the following list as model_id:
         - ai21.j2-grande-instruct
         - ai21.j2-jumbo-instruct
         
         ```python
         import ai21
         
+        # The bedrock API is available only to us-east-1 scoped clients right now
+        ai21.aws_region = 'us-east-1'
+        
         response = ai21.Completion.execute(
             destination=ai21.BedrockDestination(model_id=ai21.BedrockModelID.J2_JUMBO_INSTRUCT),
-            prompt="hello world",
-            maxTokens=20,
+            prompt="Write a news release in the voice of a global banking conglomerate announcing an unprecedented building campaign to expand and rebuild their corporate headquarters in Alpha Centauri.",
+            maxTokens=200,
         )
         
         print(response)
         ```
         
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `ai21-1.1.3/README.md` & `ai21-1.1.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -40,48 +40,54 @@
 This example uses a simple completion call with only prompt and maxTokens arguments supplied
 (all other completion settings are set to their defaults):
 ```python
 import ai21
 
 ai21.api_key = 'my_api_key'
 ai21.timeout_sec = 20
-response = ai21.Completion.execute(model="j2-ultra", prompt="Write a news release in the voice of a global banking conglomerate announcing an unprecedented building campaign to expand and rebuild their corporate headquarters in Alpha Centauri.", maxTokens=200)
+response = ai21.Completion.execute(
+    model="j2-ultra",
+    prompt="Write a news release in the voice of a global banking conglomerate announcing an unprecedented building campaign to expand and rebuild their corporate headquarters in Alpha Centauri.",
+    maxTokens=200,
+)
 print(response)
 ```
 
 ### AWS Client
 This python SDK can also be used to invoke Jurassic models as a SageMaker (SM) endpoint or as an AWS Bedrock API.
 To activate this option, make sure to install with the extra AWS dependencies:
 
 `pip install -U "ai21[AWS]"`
 
 #### Sagemaker endpoint request
 You can then generate a completion by running:
 ```python
 import ai21
-ai21.aws_region = 'us-east-1'
+
 response = ai21.Completion.execute(
     destination=ai21.SageMakerDestination("<your_endpoint_name>"),
-    prompt="hello world",
-    maxTokens=20,
+    prompt="Write a news release in the voice of a global banking conglomerate announcing an unprecedented building campaign to expand and rebuild their corporate headquarters in Alpha Centauri.",
+    maxTokens=200,
 )
 
 print(response)
 ```
 
 #### Bedrock API request
-
 You can use one of the models offered in the following list as model_id:
 - ai21.j2-grande-instruct
 - ai21.j2-jumbo-instruct
 
 ```python
 import ai21
 
+# The bedrock API is available only to us-east-1 scoped clients right now
+ai21.aws_region = 'us-east-1'
+
 response = ai21.Completion.execute(
     destination=ai21.BedrockDestination(model_id=ai21.BedrockModelID.J2_JUMBO_INSTRUCT),
-    prompt="hello world",
-    maxTokens=20,
+    prompt="Write a news release in the voice of a global banking conglomerate announcing an unprecedented building campaign to expand and rebuild their corporate headquarters in Alpha Centauri.",
+    maxTokens=200,
 )
 
 print(response)
 ```
```

### Comparing `ai21-1.1.3/ai21/AWS_utils.py` & `ai21-1.1.4/ai21/AWS_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import json
 import re
 
 import boto3
-from botocore.credentials import Credentials
 from botocore.exceptions import ClientError
 
 import ai21
 from ai21.errors import ServerError, ServiceUnavailable, BadRequest, APIError
 from ai21.http_client import handle_non_success_response
 from ai21.utils import convert_to_ai21_object, log_error
```

### Comparing `ai21-1.1.3/ai21/__init__.py` & `ai21-1.1.4/ai21/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,9 +16,9 @@
 api_key = None
 organization = None
 application = None
 api_version = DEFAULT_API_VERSION
 api_host = STUDIO_HOST
 timeout_sec = None
 num_retries = None
-aws_region = 'us-east-1'
+aws_region = None
 log_level = 'error'
```

### Comparing `ai21-1.1.3/ai21/ai21_object.py` & `ai21-1.1.4/ai21/ai21_object.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.3/ai21/ai21_studio_client.py` & `ai21-1.1.4/ai21/ai21_studio_client.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.3/ai21/bedrock_client.py` & `ai21-1.1.4/ai21/bedrock_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,25 @@
 from typing import Optional, Dict, Any
 
+import boto3
 from aws_requests_auth.boto_utils import BotoAWSRequestsAuth
 
 from ai21.constants import BEDROCK_HOST_FORMAT, BEDROCK_URL_FORMAT
-from ai21.errors import WrongInputTypeException
+from ai21.errors import WrongInputTypeException, NoSpecifiedRegionException
 from ai21.http_client import HttpClient
 from ai21.utils import get_global_configs, convert_to_ai21_object, get_value
 
-_global_configs = get_global_configs()
-_aws_region = _global_configs.get('aws_region')
-_auth_token = BotoAWSRequestsAuth(
-    aws_host=BEDROCK_HOST_FORMAT.format(aws_region=_aws_region),
-    aws_region=_aws_region,
-    aws_service='bedrock',
-)
-
 
 class BedrockClient:
     def __init__(self, **params):
-        self._aws_region = _aws_region or _global_configs.get('aws_region')
-        self._http_client = self._build_http_client(_global_configs, params)
+        self._aws_region = self._get_aws_region()
+        self._http_client = self._build_http_client(params)
 
-    def _build_http_client(self, global_configs, params):
+    def _build_http_client(self, params):
+        global_configs = get_global_configs()
         headers = self._build_default_headers()
         passed_headers = params.get('headers', None)
 
         if passed_headers is not None:
             if not isinstance(passed_headers, Dict):
                 raise WrongInputTypeException('headers', Dict, type(passed_headers))
             headers.update(passed_headers)
@@ -37,17 +31,30 @@
 
     def _build_default_headers(self):
         headers = {'Content-Type': 'application/json'}
 
         return headers
 
     def execute_http_request(self, params: Optional[Dict[str, Any]], model_id: str):
-        bedrock_url = f'{BEDROCK_URL_FORMAT}/model/{model_id}/invoke'
+        if not self._aws_region:
+            raise NoSpecifiedRegionException()
+
+        auth_token = BotoAWSRequestsAuth(
+            aws_host=BEDROCK_HOST_FORMAT.format(region_name=self._aws_region),
+            aws_region=self._aws_region,
+            aws_service='bedrock',
+        )
+
+        bedrock_url = f'{BEDROCK_URL_FORMAT.format(region_name=self._aws_region)}/model/{model_id}/invoke'
 
         response = self._http_client.execute_http_request(
             method='POST',
             url=bedrock_url,
             params=params,
-            auth=_auth_token,
+            auth=auth_token,
         )
 
         return convert_to_ai21_object(response)
+
+    def _get_aws_region(self) -> str:
+        global_configs = get_global_configs()
+        return global_configs.get('aws_region') or boto3.Session().region_name
```

### Comparing `ai21-1.1.3/ai21/errors.py` & `ai21-1.1.4/ai21/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,7 +87,14 @@
 
 
 class MissingApiKeyException(AI21ClientException):
     def __init__(self):
         message = 'API key must be supplied either globally in the ai21 namespace, or to be provided in the call args'
         super().__init__(message)
         self.message = message
+
+
+class NoSpecifiedRegionException(AI21ClientException):
+    def __init__(self):
+        message = 'No AWS region provided'
+        super().__init__(message)
+        self.message = message
```

### Comparing `ai21-1.1.3/ai21/http_client.py` & `ai21-1.1.4/ai21/http_client.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.3/ai21/modules/completion.py` & `ai21-1.1.4/ai21/modules/completion.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.3/ai21/modules/custom_model.py` & `ai21-1.1.4/ai21/modules/custom_model.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.3/ai21/modules/dataset.py` & `ai21-1.1.4/ai21/modules/dataset.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.3/ai21/modules/experimental.py` & `ai21-1.1.4/ai21/modules/experimental.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.3/ai21/modules/gec.py` & `ai21-1.1.4/ai21/modules/gec.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.3/ai21/modules/improvements.py` & `ai21-1.1.4/ai21/modules/improvements.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.3/ai21/modules/paraphrase.py` & `ai21-1.1.4/ai21/modules/paraphrase.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.3/ai21/modules/question_answering.py` & `ai21-1.1.4/ai21/modules/question_answering.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.3/ai21/modules/resources/ai21_module.py` & `ai21-1.1.4/ai21/modules/resources/ai21_module.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.3/ai21/modules/resources/execution_utils.py` & `ai21-1.1.4/ai21/modules/resources/execution_utils.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.3/ai21/modules/resources/nlp_task.py` & `ai21-1.1.4/ai21/modules/resources/nlp_task.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.3/ai21/modules/segmentation.py` & `ai21-1.1.4/ai21/modules/segmentation.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.3/ai21/modules/summarize.py` & `ai21-1.1.4/ai21/modules/summarize.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.3/ai21/modules/tokenization.py` & `ai21-1.1.4/ai21/modules/tokenization.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.3/ai21/utils.py` & `ai21-1.1.4/ai21/utils.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.3/ai21.egg-info/PKG-INFO` & `ai21-1.1.4/ai21.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai21
-Version: 1.1.3
+Version: 1.1.4
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: ai21 labs
 Author-email: support@ai21.com
 License: MIT
 Description: # AI21 Studio Client
         Python client for the AI21 Studio API
@@ -48,51 +48,57 @@
         This example uses a simple completion call with only prompt and maxTokens arguments supplied
         (all other completion settings are set to their defaults):
         ```python
         import ai21
         
         ai21.api_key = 'my_api_key'
         ai21.timeout_sec = 20
-        response = ai21.Completion.execute(model="j2-ultra", prompt="Write a news release in the voice of a global banking conglomerate announcing an unprecedented building campaign to expand and rebuild their corporate headquarters in Alpha Centauri.", maxTokens=200)
+        response = ai21.Completion.execute(
+            model="j2-ultra",
+            prompt="Write a news release in the voice of a global banking conglomerate announcing an unprecedented building campaign to expand and rebuild their corporate headquarters in Alpha Centauri.",
+            maxTokens=200,
+        )
         print(response)
         ```
         
         ### AWS Client
         This python SDK can also be used to invoke Jurassic models as a SageMaker (SM) endpoint or as an AWS Bedrock API.
         To activate this option, make sure to install with the extra AWS dependencies:
         
         `pip install -U "ai21[AWS]"`
         
         #### Sagemaker endpoint request
         You can then generate a completion by running:
         ```python
         import ai21
-        ai21.aws_region = 'us-east-1'
+        
         response = ai21.Completion.execute(
             destination=ai21.SageMakerDestination("<your_endpoint_name>"),
-            prompt="hello world",
-            maxTokens=20,
+            prompt="Write a news release in the voice of a global banking conglomerate announcing an unprecedented building campaign to expand and rebuild their corporate headquarters in Alpha Centauri.",
+            maxTokens=200,
         )
         
         print(response)
         ```
         
         #### Bedrock API request
-        
         You can use one of the models offered in the following list as model_id:
         - ai21.j2-grande-instruct
         - ai21.j2-jumbo-instruct
         
         ```python
         import ai21
         
+        # The bedrock API is available only to us-east-1 scoped clients right now
+        ai21.aws_region = 'us-east-1'
+        
         response = ai21.Completion.execute(
             destination=ai21.BedrockDestination(model_id=ai21.BedrockModelID.J2_JUMBO_INSTRUCT),
-            prompt="hello world",
-            maxTokens=20,
+            prompt="Write a news release in the voice of a global banking conglomerate announcing an unprecedented building campaign to expand and rebuild their corporate headquarters in Alpha Centauri.",
+            maxTokens=200,
         )
         
         print(response)
         ```
         
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `ai21-1.1.3/ai21.egg-info/SOURCES.txt` & `ai21-1.1.4/ai21.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ai21-1.1.3/setup.py` & `ai21-1.1.4/setup.py`

 * *Files identical despite different names*

