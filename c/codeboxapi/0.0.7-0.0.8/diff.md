# Comparing `tmp/codeboxapi-0.0.7.tar.gz` & `tmp/codeboxapi-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codeboxapi-0.0.7.tar", max compression
+gzip compressed data, was "codeboxapi-0.0.8.tar", max compression
```

## Comparing `codeboxapi-0.0.7.tar` & `codeboxapi-0.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1074 2023-07-09 12:26:51.625346 codeboxapi-0.0.7/LICENSE
--rw-r--r--   0        0        0     1124 2023-07-14 23:30:25.010671 codeboxapi-0.0.7/README.md
--rw-r--r--   0        0        0      447 2023-07-11 16:58:07.407377 codeboxapi-0.0.7/codeboxapi/__init__.py
--rw-r--r--   0        0        0       89 2023-07-11 17:29:00.964544 codeboxapi-0.0.7/codeboxapi/box/__init__.py
--rw-r--r--   0        0        0     2351 2023-07-13 21:08:10.583088 codeboxapi-0.0.7/codeboxapi/box/basebox.py
--rw-r--r--   0        0        0     5632 2023-07-14 12:27:21.432883 codeboxapi-0.0.7/codeboxapi/box/codebox.py
--rw-r--r--   0        0        0    16723 2023-07-15 09:59:55.579865 codeboxapi-0.0.7/codeboxapi/box/localbox.py
--rw-r--r--   0        0        0      386 2023-07-14 23:28:15.423391 codeboxapi-0.0.7/codeboxapi/config.py
--rw-r--r--   0        0        0     1822 2023-07-09 12:26:51.659184 codeboxapi-0.0.7/codeboxapi/errors.py
--rw-r--r--   0        0        0      590 2023-07-12 14:35:14.261440 codeboxapi-0.0.7/codeboxapi/schema.py
--rw-r--r--   0        0        0     2883 2023-07-14 23:29:29.893039 codeboxapi-0.0.7/codeboxapi/utils.py
--rw-r--r--   0        0        0      595 2023-07-15 11:58:53.949942 codeboxapi-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1918 1970-01-01 00:00:00.000000 codeboxapi-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-07-09 12:26:51.625346 codeboxapi-0.0.8/LICENSE
+-rw-r--r--   0        0        0     1124 2023-07-14 23:30:25.010671 codeboxapi-0.0.8/README.md
+-rw-r--r--   0        0        0      447 2023-07-17 13:07:06.595127 codeboxapi-0.0.8/codeboxapi/__init__.py
+-rw-r--r--   0        0        0       89 2023-07-17 13:07:06.595368 codeboxapi-0.0.8/codeboxapi/box/__init__.py
+-rw-r--r--   0        0        0     2351 2023-07-17 13:07:06.595639 codeboxapi-0.0.8/codeboxapi/box/basebox.py
+-rw-r--r--   0        0        0     5645 2023-07-17 13:22:59.484993 codeboxapi-0.0.8/codeboxapi/box/codebox.py
+-rw-r--r--   0        0        0    16777 2023-07-17 13:22:59.488023 codeboxapi-0.0.8/codeboxapi/box/localbox.py
+-rw-r--r--   0        0        0      396 2023-07-17 13:22:59.488093 codeboxapi-0.0.8/codeboxapi/config.py
+-rw-r--r--   0        0        0     1822 2023-07-09 12:26:51.659184 codeboxapi-0.0.8/codeboxapi/errors.py
+-rw-r--r--   0        0        0      628 2023-07-17 13:22:59.488147 codeboxapi-0.0.8/codeboxapi/schema.py
+-rw-r--r--   0        0        0     2925 2023-07-17 13:22:59.488185 codeboxapi-0.0.8/codeboxapi/utils.py
+-rw-r--r--   0        0        0      595 2023-07-17 13:23:59.278123 codeboxapi-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1918 1970-01-01 00:00:00.000000 codeboxapi-0.0.8/PKG-INFO
```

### Comparing `codeboxapi-0.0.7/LICENSE` & `codeboxapi-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `codeboxapi-0.0.7/README.md` & `codeboxapi-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `codeboxapi-0.0.7/codeboxapi/box/basebox.py` & `codeboxapi-0.0.8/codeboxapi/box/basebox.py`

 * *Files identical despite different names*

### Comparing `codeboxapi-0.0.7/codeboxapi/box/codebox.py` & `codeboxapi-0.0.8/codeboxapi/box/codebox.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any
+from typing import Any, Optional
 from codeboxapi import settings
 from codeboxapi.box import BaseBox
 from ..utils import base_request, abase_request
 from ..schema import (
     CodeBoxStatus, 
     CodeBoxOutput,
     CodeBoxFile
@@ -20,15 +20,15 @@
             from .localbox import LocalBox
             return LocalBox(*args, **kwargs)
         else:
             return super().__new__(cls, *args, **kwargs)
     
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
-        self.session: ClientSession | None = None
+        self.session: Optional[ClientSession] = None
     
     def start(self) -> CodeBoxStatus:
         return self.status()
     
     async def astart(self) -> CodeBoxStatus:
         self.session = ClientSession()
         return await self.astatus()
```

### Comparing `codeboxapi-0.0.7/codeboxapi/box/localbox.py` & `codeboxapi-0.0.8/codeboxapi/box/localbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import json
 import time
 import requests  # type: ignore
 import asyncio
 import aiohttp
 import subprocess
 from uuid import uuid4
+from typing import Optional, Union
 from typing_extensions import Self
 from websockets.exceptions import ConnectionClosedError
 from websockets.client import WebSocketClientProtocol, connect as ws_connect
 from websockets.sync.client import connect as ws_connect_sync, ClientConnection
 from codeboxapi.box import BaseBox
 from codeboxapi.schema import (
     CodeBoxStatus, 
@@ -22,15 +23,15 @@
 class LocalBox(BaseBox):
     """
     LocalBox is a CodeBox implementation that runs code locally.
     This is useful for testing and development.c
     In case you don't put an api_key, 
     this is the default CodeBox.
     """
-    _instance: Self | None = None
+    _instance: Optional[Self] = None
     
     def __new__(cls, *args, **kwargs):
         if not cls._instance:
             cls._instance = super().__new__(cls, *args, **kwargs)
         else:
             print(
                 "INFO: Using a LocalBox which is not isolated.\n"
@@ -38,18 +39,18 @@
                 "      Make sure to put an API-Key in production.\n"
             )
         return cls._instance
         
     def __init__(self, port: int = 8888) -> None:
         super().__init__()
         self.port = port
-        self.kernel: dict | None = None
-        self.ws: WebSocketClientProtocol | ClientConnection | None = None
-        self.subprocess: asyncio.subprocess.Process | subprocess.Popen | None = None
-        self.session: aiohttp.ClientSession | None = None
+        self.kernel: Optional[dict] = None
+        self.ws: Union[WebSocketClientProtocol, ClientConnection, None] = None
+        self.subprocess: Union[asyncio.subprocess.Process, subprocess.Popen, None] = None
+        self.session: Optional[aiohttp.ClientSession] = None
     
     def start(self) -> CodeBoxStatus:
         os.makedirs(".codebox", exist_ok=True)
         self._check_port()
         if settings.VERBOSE:
             print("Starting kernel...")
             out = None
```

### Comparing `codeboxapi-0.0.7/codeboxapi/errors.py` & `codeboxapi-0.0.8/codeboxapi/errors.py`

 * *Files identical despite different names*

### Comparing `codeboxapi-0.0.7/codeboxapi/schema.py` & `codeboxapi-0.0.8/codeboxapi/schema.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Optional
 from pydantic import BaseModel
 
 
 class CodeBoxStatus(BaseModel):
     status: str
     
     def __str__(self):
@@ -20,14 +21,14 @@
     
     def __repr__(self):
         return f"{self.type}({self.content})"
 
 
 class CodeBoxFile(BaseModel):
     name: str
-    content: bytes | None
+    content: Optional[bytes] = None
     
     def __str__(self):
         return self.name
     
     def __repr__(self):
         return f"File({self.name})"
```

### Comparing `codeboxapi-0.0.7/codeboxapi/utils.py` & `codeboxapi-0.0.8/codeboxapi/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import json
 import requests  # type: ignore
+from typing import Optional
 from aiohttp import ClientSession, ClientResponse, FormData
 from codeboxapi.config import settings
 
 
 def build_request_data(
     method: str, 
     endpoint: str, 
-    body: dict | None = None, 
-    files: dict | None = None, 
+    body: Optional[dict] = None,
+    files: Optional[dict] = None, 
     content_type: str = "application/json"
 ) -> dict:
     return {
         "method": method,
         "url": settings.CODEBOX_BASE_URL + endpoint,
         "headers": {
             "Content-Type": content_type,
@@ -50,29 +51,29 @@
         raise Exception(f"Error: {response.status} {await response.text()}")
     return await handler(response)
 
 
 def base_request(
     method: str, 
     endpoint: str, 
-    body: dict | None = None, 
-    files: dict | None = None, 
+    body: Optional[dict] = None,
+    files: Optional[dict] = None, 
     content_type: str = "application/json"
 ) -> dict:
     request_data = build_request_data(method, endpoint, body, files, content_type)
     response = requests.request(**request_data)
     return handle_response(response)
 
 
 async def abase_request(
     session: ClientSession, 
     method: str, 
     endpoint: str, 
-    body: dict | None = None, 
-    files: dict | None = None, 
+    body: Optional[dict] = None,
+    files: Optional[dict] = None,
     content_type: str = "application/json"
 ) -> dict:
     request_data = build_request_data(method, endpoint, body, files, content_type)
     if files is not None:
         data = FormData()
         for key, file in files.items():
             data.add_field(key, file)
```

### Comparing `codeboxapi-0.0.7/pyproject.toml` & `codeboxapi-0.0.8/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "codeboxapi"
-version = "0.0.7"
+version = "0.0.8"
 description = "CodeBox is the simplest cloud infrastructure for your LLM Apps and Services."
 authors = ["Shroominic <pleurae-berets.0u@icloud.com>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `codeboxapi-0.0.7/PKG-INFO` & `codeboxapi-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codeboxapi
-Version: 0.0.7
+Version: 0.0.8
 Summary: CodeBox is the simplest cloud infrastructure for your LLM Apps and Services.
 License: MIT
 Author: Shroominic
 Author-email: pleurae-berets.0u@icloud.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

