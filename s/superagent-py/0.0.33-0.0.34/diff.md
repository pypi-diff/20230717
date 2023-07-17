# Comparing `tmp/superagent_py-0.0.33.tar.gz` & `tmp/superagent_py-0.0.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superagent_py-0.0.33.tar", max compression
+gzip compressed data, was "superagent_py-0.0.34.tar", max compression
```

## Comparing `superagent_py-0.0.33.tar` & `superagent_py-0.0.34.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1073 2023-07-12 22:10:52.048381 superagent_py-0.0.33/LICENSE
--rw-r--r--   0        0        0     3169 2023-07-12 22:10:52.048381 superagent_py-0.0.33/README.md
--rw-r--r--   0        0        0      380 2023-07-12 22:10:52.048381 superagent_py-0.0.33/pyproject.toml
--rw-r--r--   0        0        0      589 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/__init__.py
--rw-r--r--   0        0        0     2956 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/client.py
--rw-r--r--   0        0        0      348 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/core/__init__.py
--rw-r--r--   0        0        0      426 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      170 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/errors/__init__.py
--rw-r--r--   0        0        0      313 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0        0 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/py.typed
--rw-r--r--   0        0        0      343 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/resources/agent/__init__.py
--rw-r--r--   0        0        0    14309 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/resources/agent/client.py
--rw-r--r--   0        0        0       65 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/resources/agent_documents/__init__.py
--rw-r--r--   0        0        0     9260 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/resources/agent_documents/client.py
--rw-r--r--   0        0        0       65 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/resources/agent_tools/__init__.py
--rw-r--r--   0        0        0     9132 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/resources/agent_tools/client.py
--rw-r--r--   0        0        0       65 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/resources/api_token/__init__.py
--rw-r--r--   0        0        0     8538 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/resources/api_token/client.py
--rw-r--r--   0        0        0       65 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/resources/auth/__init__.py
--rw-r--r--   0        0        0     5901 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/resources/auth/client.py
--rw-r--r--   0        0        0       65 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/resources/documents/__init__.py
--rw-r--r--   0        0        0    10039 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/resources/documents/client.py
--rw-r--r--   0        0        0       65 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/resources/prompts/__init__.py
--rw-r--r--   0        0        0    10865 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/resources/prompts/client.py
--rw-r--r--   0        0        0       65 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/resources/tools/__init__.py
--rw-r--r--   0        0        0     9383 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/resources/tools/client.py
--rw-r--r--   0        0        0       65 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/resources/traces/__init__.py
--rw-r--r--   0        0        0     2236 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/resources/traces/client.py
--rw-r--r--   0        0        0       65 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/resources/user/__init__.py
--rw-r--r--   0        0        0     4328 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/resources/user/client.py
--rw-r--r--   0        0        0      308 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/types/__init__.py
--rw-r--r--   0        0        0      843 2023-07-12 22:10:52.052381 superagent_py-0.0.33/src/superagent/types/http_validation_error.py
--rw-r--r--   0        0        0      869 2023-07-12 22:10:52.052381 superagent_py-0.0.33/src/superagent/types/validation_error.py
--rw-r--r--   0        0        0      128 2023-07-12 22:10:52.052381 superagent_py-0.0.33/src/superagent/types/validation_error_loc_item.py
--rw-r--r--   0        0        0     3680 1970-01-01 00:00:00.000000 superagent_py-0.0.33/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-17 11:38:46.217009 superagent_py-0.0.34/LICENSE
+-rw-r--r--   0        0        0     3251 2023-07-17 11:38:46.217009 superagent_py-0.0.34/README.md
+-rw-r--r--   0        0        0      380 2023-07-17 11:38:46.217009 superagent_py-0.0.34/pyproject.toml
+-rw-r--r--   0        0        0      589 2023-07-17 11:38:46.217009 superagent_py-0.0.34/src/superagent/__init__.py
+-rw-r--r--   0        0        0     2956 2023-07-17 11:38:46.217009 superagent_py-0.0.34/src/superagent/client.py
+-rw-r--r--   0        0        0      348 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      170 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/errors/__init__.py
+-rw-r--r--   0        0        0      313 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0        0 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/py.typed
+-rw-r--r--   0        0        0      343 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/resources/agent/__init__.py
+-rw-r--r--   0        0        0    14309 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/resources/agent/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/resources/agent_documents/__init__.py
+-rw-r--r--   0        0        0     9260 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/resources/agent_documents/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/resources/agent_tools/__init__.py
+-rw-r--r--   0        0        0     9132 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/resources/agent_tools/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/resources/api_token/__init__.py
+-rw-r--r--   0        0        0     8538 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/resources/api_token/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/resources/auth/__init__.py
+-rw-r--r--   0        0        0     5901 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/resources/auth/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/resources/documents/__init__.py
+-rw-r--r--   0        0        0    10039 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/resources/documents/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/resources/prompts/__init__.py
+-rw-r--r--   0        0        0    10865 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/resources/prompts/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/resources/tools/__init__.py
+-rw-r--r--   0        0        0     9383 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/resources/tools/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/resources/traces/__init__.py
+-rw-r--r--   0        0        0     2236 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/resources/traces/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/resources/user/__init__.py
+-rw-r--r--   0        0        0     4328 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/resources/user/client.py
+-rw-r--r--   0        0        0      308 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/types/__init__.py
+-rw-r--r--   0        0        0      843 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/types/http_validation_error.py
+-rw-r--r--   0        0        0      869 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/types/validation_error.py
+-rw-r--r--   0        0        0      128 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0     3762 1970-01-01 00:00:00.000000 superagent_py-0.0.34/PKG-INFO
```

### Comparing `superagent_py-0.0.33/LICENSE` & `superagent_py-0.0.34/LICENSE`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.33/README.md` & `superagent_py-0.0.34/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -30,29 +30,29 @@
 ```
 
 ## Usage
 
 ```python
 from superagent.client import Superagent
 
-client = Superagent(token="API_TOKEN")
+client = Superagent(token="API_TOKEN", environment="https://api.superagent.sh")
 
 agent = client.agents.get_agent("<AGENT_ID>")
 
 print("Received response from superagent", agent)
 ```
 
 ## Async Client
 
 ```python
 from superagent.client import AsyncSuperagent
 
 import asyncio
 
-client = AsyncSuperagent(token="API_TOKEN")
+client = AsyncSuperagent(token="API_TOKEN", environment="https://api.superagent.sh")
 
 async def get_agent() -> None:
     agent = client.agents.get_agent("<AGENT_ID>")
     print(token_response)
 
 asyncio.run(get_agent())
 ```
```

### Comparing `superagent_py-0.0.33/src/superagent/__init__.py` & `superagent_py-0.0.34/src/superagent/__init__.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.33/src/superagent/client.py` & `superagent_py-0.0.34/src/superagent/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.33/src/superagent/core/datetime_utils.py` & `superagent_py-0.0.34/src/superagent/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.33/src/superagent/core/jsonable_encoder.py` & `superagent_py-0.0.34/src/superagent/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.33/src/superagent/resources/agent/client.py` & `superagent_py-0.0.34/src/superagent/resources/agent/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.33/src/superagent/resources/agent_documents/client.py` & `superagent_py-0.0.34/src/superagent/resources/agent_documents/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.33/src/superagent/resources/agent_tools/client.py` & `superagent_py-0.0.34/src/superagent/resources/agent_tools/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.33/src/superagent/resources/api_token/client.py` & `superagent_py-0.0.34/src/superagent/resources/api_token/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.33/src/superagent/resources/auth/client.py` & `superagent_py-0.0.34/src/superagent/resources/auth/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.33/src/superagent/resources/documents/client.py` & `superagent_py-0.0.34/src/superagent/resources/documents/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.33/src/superagent/resources/prompts/client.py` & `superagent_py-0.0.34/src/superagent/resources/prompts/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.33/src/superagent/resources/tools/client.py` & `superagent_py-0.0.34/src/superagent/resources/tools/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.33/src/superagent/resources/traces/client.py` & `superagent_py-0.0.34/src/superagent/resources/traces/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.33/src/superagent/resources/user/client.py` & `superagent_py-0.0.34/src/superagent/resources/user/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.33/src/superagent/types/http_validation_error.py` & `superagent_py-0.0.34/src/superagent/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.33/src/superagent/types/validation_error.py` & `superagent_py-0.0.34/src/superagent/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.33/PKG-INFO` & `superagent_py-0.0.34/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superagent-py
-Version: 0.0.33
+Version: 0.0.34
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -45,29 +45,29 @@
 ```
 
 ## Usage
 
 ```python
 from superagent.client import Superagent
 
-client = Superagent(token="API_TOKEN")
+client = Superagent(token="API_TOKEN", environment="https://api.superagent.sh")
 
 agent = client.agents.get_agent("<AGENT_ID>")
 
 print("Received response from superagent", agent)
 ```
 
 ## Async Client
 
 ```python
 from superagent.client import AsyncSuperagent
 
 import asyncio
 
-client = AsyncSuperagent(token="API_TOKEN")
+client = AsyncSuperagent(token="API_TOKEN", environment="https://api.superagent.sh")
 
 async def get_agent() -> None:
     agent = client.agents.get_agent("<AGENT_ID>")
     print(token_response)
 
 asyncio.run(get_agent())
 ```
```

