# Comparing `tmp/langfuse-0.0.8.tar.gz` & `tmp/langfuse-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langfuse-0.0.8.tar", max compression
+gzip compressed data, was "langfuse-0.0.9.tar", max compression
```

## Comparing `langfuse-0.0.8.tar` & `langfuse-0.0.9.tar`

### file list

```diff
@@ -1,5 +1,46 @@
--rw-r--r--   0        0        0        0 2023-07-17 11:30:32.660307 langfuse-0.0.8/README.md
--rw-r--r--   0        0        0        0 2023-07-17 11:29:03.775228 langfuse-0.0.8/langfuse/__init__.py
--rw-r--r--   0        0        0     1458 2023-07-17 12:54:43.388678 langfuse-0.0.8/langfuse/wrapper.py
--rw-r--r--   0        0        0      623 2023-07-17 12:59:17.572191 langfuse-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      699 1970-01-01 00:00:00.000000 langfuse-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-17 11:30:32.660307 langfuse-0.0.9/README.md
+-rw-r--r--   0        0        0        0 2023-07-17 11:29:03.775228 langfuse-0.0.9/langfuse/__init__.py
+-rw-r--r--   0        0        0     1473 2023-07-17 13:59:45.677668 langfuse-0.0.9/langfuse/langfuse.py
+-rw-r--r--   0        0        0      152 2023-07-17 13:59:40.438625 langfuse-0.0.9/langfuse/openapi/__init__.py
+-rw-r--r--   0        0        0       47 2023-07-17 13:59:39.776134 langfuse-0.0.9/langfuse/openapi/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-17 13:59:39.782050 langfuse-0.0.9/langfuse/openapi/api/event/__init__.py
+-rw-r--r--   0        0        0     4794 2023-07-17 13:59:40.459218 langfuse-0.0.9/langfuse/openapi/api/event/event_create.py
+-rw-r--r--   0        0        0        0 2023-07-17 13:59:39.794205 langfuse-0.0.9/langfuse/openapi/api/generations/__init__.py
+-rw-r--r--   0        0        0     4557 2023-07-17 13:59:40.455503 langfuse-0.0.9/langfuse/openapi/api/generations/generations_log.py
+-rw-r--r--   0        0        0     4713 2023-07-17 13:59:40.475145 langfuse-0.0.9/langfuse/openapi/api/generations/generations_update.py
+-rw-r--r--   0        0        0        0 2023-07-17 13:59:39.795364 langfuse-0.0.9/langfuse/openapi/api/score/__init__.py
+-rw-r--r--   0        0        0     4790 2023-07-17 13:59:40.477165 langfuse-0.0.9/langfuse/openapi/api/score/score_create.py
+-rw-r--r--   0        0        0        0 2023-07-17 13:59:39.796019 langfuse-0.0.9/langfuse/openapi/api/span/__init__.py
+-rw-r--r--   0        0        0     4761 2023-07-17 13:59:40.459936 langfuse-0.0.9/langfuse/openapi/api/span/span_create.py
+-rw-r--r--   0        0        0     4774 2023-07-17 13:59:40.468462 langfuse-0.0.9/langfuse/openapi/api/span/span_update.py
+-rw-r--r--   0        0        0        0 2023-07-17 13:59:39.797188 langfuse-0.0.9/langfuse/openapi/api/trace/__init__.py
+-rw-r--r--   0        0        0     4790 2023-07-17 13:59:40.463881 langfuse-0.0.9/langfuse/openapi/api/trace/trace_create.py
+-rw-r--r--   0        0        0     2817 2023-07-17 13:59:40.480520 langfuse-0.0.9/langfuse/openapi/client.py
+-rw-r--r--   0        0        0      470 2023-07-17 13:59:40.467748 langfuse-0.0.9/langfuse/openapi/errors.py
+-rw-r--r--   0        0        0     1728 2023-07-17 13:59:39.775136 langfuse-0.0.9/langfuse/openapi/models/__init__.py
+-rw-r--r--   0        0        0     5412 2023-07-17 13:59:40.511569 langfuse-0.0.9/langfuse/openapi/models/create_event_request.py
+-rw-r--r--   0        0        0     9118 2023-07-17 13:59:40.519167 langfuse-0.0.9/langfuse/openapi/models/create_log.py
+-rw-r--r--   0        0        0     1725 2023-07-17 13:59:40.470268 langfuse-0.0.9/langfuse/openapi/models/create_log_model_parameters.py
+-rw-r--r--   0        0        0     3071 2023-07-17 13:59:40.480378 langfuse-0.0.9/langfuse/openapi/models/create_score_request.py
+-rw-r--r--   0        0        0     6087 2023-07-17 13:59:40.499034 langfuse-0.0.9/langfuse/openapi/models/create_span_request.py
+-rw-r--r--   0        0        0     2334 2023-07-17 13:59:40.486537 langfuse-0.0.9/langfuse/openapi/models/create_trace_request.py
+-rw-r--r--   0        0        0     4004 2023-07-17 13:59:40.501876 langfuse-0.0.9/langfuse/openapi/models/event.py
+-rw-r--r--   0        0        0     2232 2023-07-17 13:59:40.487223 langfuse-0.0.9/langfuse/openapi/models/llm_usage.py
+-rw-r--r--   0        0        0     7657 2023-07-17 13:59:40.522709 langfuse-0.0.9/langfuse/openapi/models/log.py
+-rw-r--r--   0        0        0     1692 2023-07-17 13:59:40.489991 langfuse-0.0.9/langfuse/openapi/models/log_model_parameters.py
+-rw-r--r--   0        0        0      214 2023-07-17 13:59:40.127911 langfuse-0.0.9/langfuse/openapi/models/observation_level_event.py
+-rw-r--r--   0        0        0      219 2023-07-17 13:59:40.127354 langfuse-0.0.9/langfuse/openapi/models/observation_level_generation.py
+-rw-r--r--   0        0        0      213 2023-07-17 13:59:40.120236 langfuse-0.0.9/langfuse/openapi/models/observation_level_span.py
+-rw-r--r--   0        0        0     2723 2023-07-17 13:59:40.507884 langfuse-0.0.9/langfuse/openapi/models/score.py
+-rw-r--r--   0        0        0     4686 2023-07-17 13:59:40.520376 langfuse-0.0.9/langfuse/openapi/models/span.py
+-rw-r--r--   0        0        0     2716 2023-07-17 13:59:40.505288 langfuse-0.0.9/langfuse/openapi/models/trace.py
+-rw-r--r--   0        0        0      168 2023-07-17 13:59:40.117128 langfuse-0.0.9/langfuse/openapi/models/trace_id_type.py
+-rw-r--r--   0        0        0      173 2023-07-17 13:59:40.119647 langfuse-0.0.9/langfuse/openapi/models/trace_id_type_event.py
+-rw-r--r--   0        0        0      179 2023-07-17 13:59:40.112409 langfuse-0.0.9/langfuse/openapi/models/trace_id_type_generations.py
+-rw-r--r--   0        0        0      172 2023-07-17 13:59:40.121897 langfuse-0.0.9/langfuse/openapi/models/trace_id_type_span.py
+-rw-r--r--   0        0        0     7379 2023-07-17 13:59:40.538461 langfuse-0.0.9/langfuse/openapi/models/update_generation_request.py
+-rw-r--r--   0        0        0     1798 2023-07-17 13:59:40.499828 langfuse-0.0.9/langfuse/openapi/models/update_generation_request_model_parameters.py
+-rw-r--r--   0        0        0     3908 2023-07-17 13:59:40.527528 langfuse-0.0.9/langfuse/openapi/models/update_span_request.py
+-rw-r--r--   0        0        0      993 2023-07-17 13:59:40.506157 langfuse-0.0.9/langfuse/openapi/types.py
+-rw-r--r--   0        0        0      623 2023-07-17 14:06:01.802578 langfuse-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      699 1970-01-01 00:00:00.000000 langfuse-0.0.9/PKG-INFO
```

### Comparing `langfuse-0.0.8/langfuse/wrapper.py` & `langfuse-0.0.9/langfuse/langfuse.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import asyncio
 import base64
 from typing import Coroutine, Optional
-from api.api.trace import trace_create
 
-from api.client import Client
-from api.models.create_trace_request import CreateTraceRequest
+from langfuse.openapi.client import Client
+from langfuse.openapi.models.create_trace_request import CreateTraceRequest
+from langfuse.openapi.api.trace import trace_create
 
-
-class ApiClient:
+class Langfuse:
     """A Client which has been authenticated for use on secured endpoints"""
 
     
     def __init__(self, public_key: str, secret_key: str, base_url: Optional[str]):
         
-        self.promises: list[Coroutine] = []#attr.ib(factory=list)
+        self.promises: list[Coroutine] = []
 
         self.base_url = base_url if base_url else 'https://cloud.langfuse.com'
 
         print("__init__", self.promises)
         auth = base64.b64encode(f"{public_key}:{secret_key}".encode()).decode()
         headers = {
             'Authorization': 'Basic ' + auth,
```

### Comparing `langfuse-0.0.8/pyproject.toml` & `langfuse-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langfuse"
-version = "0.0.8"
+version = "0.0.9"
 description = "A client library for accessing langfuse"
 authors = ["langfuse <developers@langfuse.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 pytest = "^7.4.0"
```

### Comparing `langfuse-0.0.8/PKG-INFO` & `langfuse-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langfuse
-Version: 0.0.8
+Version: 0.0.9
 Summary: A client library for accessing langfuse
 License: MIT
 Author: langfuse
 Author-email: developers@langfuse.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

