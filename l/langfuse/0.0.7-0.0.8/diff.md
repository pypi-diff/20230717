# Comparing `tmp/langfuse-0.0.7.tar.gz` & `tmp/langfuse-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langfuse-0.0.7.tar", max compression
+gzip compressed data, was "langfuse-0.0.8.tar", max compression
```

## Comparing `langfuse-0.0.7.tar` & `langfuse-0.0.8.tar`

### file list

```diff
@@ -1,46 +1,5 @@
--rw-r--r--   0        0        0     3693 2023-07-12 11:28:38.262604 langfuse-0.0.7/README.md
--rw-r--r--   0        0        0        0 2023-07-12 12:12:18.033577 langfuse-0.0.7/langfuse/__init__.py
--rw-r--r--   0        0        0       47 2023-07-12 11:28:38.302195 langfuse-0.0.7/langfuse/api/__init__.py
--rw-r--r--   0        0        0        0 2023-07-12 11:28:38.307846 langfuse-0.0.7/langfuse/api/event/__init__.py
--rw-r--r--   0        0        0     4794 2023-07-12 11:28:38.860217 langfuse-0.0.7/langfuse/api/event/event_create.py
--rw-r--r--   0        0        0        0 2023-07-12 11:28:38.319025 langfuse-0.0.7/langfuse/api/generations/__init__.py
--rw-r--r--   0        0        0     4557 2023-07-12 11:28:38.871136 langfuse-0.0.7/langfuse/api/generations/generations_log.py
--rw-r--r--   0        0        0     4713 2023-07-12 11:28:38.863639 langfuse-0.0.7/langfuse/api/generations/generations_update.py
--rw-r--r--   0        0        0        0 2023-07-12 11:28:38.320137 langfuse-0.0.7/langfuse/api/score/__init__.py
--rw-r--r--   0        0        0     4790 2023-07-12 11:28:38.867895 langfuse-0.0.7/langfuse/api/score/score_create.py
--rw-r--r--   0        0        0        0 2023-07-12 11:28:38.320737 langfuse-0.0.7/langfuse/api/span/__init__.py
--rw-r--r--   0        0        0     4761 2023-07-12 11:28:38.866173 langfuse-0.0.7/langfuse/api/span/span_create.py
--rw-r--r--   0        0        0     4774 2023-07-12 11:28:38.871407 langfuse-0.0.7/langfuse/api/span/span_update.py
--rw-r--r--   0        0        0        0 2023-07-12 11:28:38.321803 langfuse-0.0.7/langfuse/api/trace/__init__.py
--rw-r--r--   0        0        0     4790 2023-07-12 11:28:38.881219 langfuse-0.0.7/langfuse/api/trace/trace_create.py
--rw-r--r--   0        0        0     2817 2023-07-12 11:28:38.860072 langfuse-0.0.7/langfuse/client.py
--rw-r--r--   0        0        0      470 2023-07-12 11:28:38.866826 langfuse-0.0.7/langfuse/errors.py
--rw-r--r--   0        0        0     1728 2023-07-12 11:28:38.301226 langfuse-0.0.7/langfuse/models/__init__.py
--rw-r--r--   0        0        0     5412 2023-07-12 11:28:38.897239 langfuse-0.0.7/langfuse/models/create_event_request.py
--rw-r--r--   0        0        0     9118 2023-07-12 11:28:38.937787 langfuse-0.0.7/langfuse/models/create_log.py
--rw-r--r--   0        0        0     1725 2023-07-12 11:28:38.883101 langfuse-0.0.7/langfuse/models/create_log_model_parameters.py
--rw-r--r--   0        0        0     3071 2023-07-12 11:28:38.902369 langfuse-0.0.7/langfuse/models/create_score_request.py
--rw-r--r--   0        0        0     6087 2023-07-12 11:28:38.916905 langfuse-0.0.7/langfuse/models/create_span_request.py
--rw-r--r--   0        0        0     2334 2023-07-12 11:28:38.891619 langfuse-0.0.7/langfuse/models/create_trace_request.py
--rw-r--r--   0        0        0     4004 2023-07-12 11:28:38.902333 langfuse-0.0.7/langfuse/models/event.py
--rw-r--r--   0        0        0     2232 2023-07-12 11:28:38.886603 langfuse-0.0.7/langfuse/models/llm_usage.py
--rw-r--r--   0        0        0     7657 2023-07-12 11:28:38.920966 langfuse-0.0.7/langfuse/models/log.py
--rw-r--r--   0        0        0     1692 2023-07-12 11:28:38.895920 langfuse-0.0.7/langfuse/models/log_model_parameters.py
--rw-r--r--   0        0        0      214 2023-07-12 11:28:38.605234 langfuse-0.0.7/langfuse/models/observation_level_event.py
--rw-r--r--   0        0        0      219 2023-07-12 11:28:38.604669 langfuse-0.0.7/langfuse/models/observation_level_generation.py
--rw-r--r--   0        0        0      213 2023-07-12 11:28:38.597789 langfuse-0.0.7/langfuse/models/observation_level_span.py
--rw-r--r--   0        0        0     2723 2023-07-12 11:28:38.903995 langfuse-0.0.7/langfuse/models/score.py
--rw-r--r--   0        0        0     4686 2023-07-12 11:28:38.928970 langfuse-0.0.7/langfuse/models/span.py
--rw-r--r--   0        0        0     2716 2023-07-12 11:28:38.918702 langfuse-0.0.7/langfuse/models/trace.py
--rw-r--r--   0        0        0      168 2023-07-12 11:28:38.594692 langfuse-0.0.7/langfuse/models/trace_id_type.py
--rw-r--r--   0        0        0      173 2023-07-12 11:28:38.597198 langfuse-0.0.7/langfuse/models/trace_id_type_event.py
--rw-r--r--   0        0        0      179 2023-07-12 11:28:38.590702 langfuse-0.0.7/langfuse/models/trace_id_type_generations.py
--rw-r--r--   0        0        0      172 2023-07-12 11:28:38.599195 langfuse-0.0.7/langfuse/models/trace_id_type_span.py
--rw-r--r--   0        0        0     7379 2023-07-12 11:28:38.939815 langfuse-0.0.7/langfuse/models/update_generation_request.py
--rw-r--r--   0        0        0     1798 2023-07-12 11:28:38.911989 langfuse-0.0.7/langfuse/models/update_generation_request_model_parameters.py
--rw-r--r--   0        0        0     3908 2023-07-12 11:28:38.930144 langfuse-0.0.7/langfuse/models/update_span_request.py
--rw-r--r--   0        0        0       25 2023-07-12 11:28:38.260242 langfuse-0.0.7/langfuse/py.typed
--rw-r--r--   0        0        0      993 2023-07-12 11:28:38.912136 langfuse-0.0.7/langfuse/types.py
--rw-r--r--   0        0        0     1410 2023-07-12 12:08:54.234365 langfuse-0.0.7/langfuse/wrapper.py
--rw-r--r--   0        0        0      652 2023-07-12 12:12:27.639569 langfuse-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     4234 1970-01-01 00:00:00.000000 langfuse-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-17 11:30:32.660307 langfuse-0.0.8/README.md
+-rw-r--r--   0        0        0        0 2023-07-17 11:29:03.775228 langfuse-0.0.8/langfuse/__init__.py
+-rw-r--r--   0        0        0     1458 2023-07-17 12:54:43.388678 langfuse-0.0.8/langfuse/wrapper.py
+-rw-r--r--   0        0        0      623 2023-07-17 12:59:17.572191 langfuse-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      699 1970-01-01 00:00:00.000000 langfuse-0.0.8/PKG-INFO
```

### Comparing `langfuse-0.0.7/langfuse/wrapper.py` & `langfuse-0.0.8/langfuse/wrapper.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,45 @@
-from asyncio import coroutines
+import asyncio
 import base64
 from typing import Coroutine, Optional
-import attr
+from api.api.trace import trace_create
+
+from api.client import Client
+from api.models.create_trace_request import CreateTraceRequest
 
-from langfuse.client import Client
-from langfuse.models.create_trace_request import CreateTraceRequest
-from langfuse.api.trace import trace_create
 
-@attr.s(auto_attribs=True)
 class ApiClient:
     """A Client which has been authenticated for use on secured endpoints"""
 
-    client: Client
-    promises: list[Coroutine] = attr.ib(factory=list)
-
+    
     def __init__(self, public_key: str, secret_key: str, base_url: Optional[str]):
-        self.base_url = base_url if base_url else 'https://cloud.langfuse.com'
         
+        self.promises: list[Coroutine] = []#attr.ib(factory=list)
 
+        self.base_url = base_url if base_url else 'https://cloud.langfuse.com'
+
+        print("__init__", self.promises)
         auth = base64.b64encode(f"{public_key}:{secret_key}".encode()).decode()
         headers = {
             'Authorization': 'Basic ' + auth,
-            'X-Langfuse-Sdk-Name': 'langfuse-js',
+            'X-Langfuse-Sdk-Name': 'langfuse-python',
             'X-Langfuse-Sdk-Version': 'version',
             'X-Langfuse-Sdk-Variant': 'Server',
         }
         self.client = Client(
             base_url=self.base_url,
             headers=headers,
             verify_ssl=True,
             raise_on_unexpected_status=False,
             follow_redirects=False,
         )
+        
+        print("self.promises")
     
     def trace(self, body: CreateTraceRequest):
-        trace_promise = trace_create.asyncio(self.client, body)
+        trace_promise = trace_create.asyncio(client=self.client, json_body=body)
+        print("trace_promise", self.promises)
         self.promises.append(trace_promise)
 
-    def flush(self):
-        coroutines.all_tasks()
-        coroutines.run(coroutines.wait(self.promises))
+    async def flush(self):
+        return await asyncio.gather(*self.promises)
         
-
```

### Comparing `langfuse-0.0.7/pyproject.toml` & `langfuse-0.0.8/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 [tool.poetry]
 name = "langfuse"
-version = "0.0.7"
+version = "0.0.8"
 description = "A client library for accessing langfuse"
-
-authors = []
-
+authors = ["langfuse <developers@langfuse.com>"]
+license = "MIT"
 readme = "README.md"
-packages = [
-    {include = "langfuse"},
-]
-include = ["CHANGELOG.md", "langfuse/py.typed"]
 
 [tool.poetry.dependencies]
+pytest = "^7.4.0"
 python = "^3.8"
 httpx = ">=0.15.4,<0.25.0"
 attrs = ">=21.3.0"
 python-dateutil = "^2.8.0"
 
+
 [build-system]
-requires = ["poetry-core>=1.0.0"]
+requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
 target_version = ['py38', 'py39', 'py310', 'py311']
 exclude = '''
 (
```

