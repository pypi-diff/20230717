# Comparing `tmp/typedhttp-0.1.0.tar.gz` & `tmp/typedhttp-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typedhttp-0.1.0.tar", max compression
+gzip compressed data, was "typedhttp-0.2.0.tar", max compression
```

## Comparing `typedhttp-0.1.0.tar` & `typedhttp-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-06-23 01:57:27.662939 typedhttp-0.1.0/README.md
--rw-r--r--   0        0        0      324 2023-06-23 01:57:27.662939 typedhttp-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-23 02:02:04.252873 typedhttp-0.1.0/src/typedhttp/__init__.py
--rw-r--r--   0        0        0     1504 2023-06-23 02:01:16.852885 typedhttp-0.1.0/src/typedhttp/main.py
--rw-r--r--   0        0        0        0 2023-06-23 02:02:09.292872 typedhttp-0.1.0/src/typedhttp/py.typed
--rw-r--r--   0        0        0     2329 2023-06-23 02:05:04.722832 typedhttp-0.1.0/src/typedhttp/requests_hook.py
--rw-r--r--   0        0        0      443 1970-01-01 00:00:00.000000 typedhttp-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-10 18:18:06.546066 typedhttp-0.2.0/README.md
+-rw-r--r--   0        0        0      380 2023-07-17 13:50:38.051074 typedhttp-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      134 2023-07-17 13:49:00.751120 typedhttp-0.2.0/src/typedhttp/__init__.py
+-rw-r--r--   0        0        0     1504 2023-07-10 18:18:06.546066 typedhttp-0.2.0/src/typedhttp/main.py
+-rw-r--r--   0        0        0        0 2023-07-10 18:18:06.546066 typedhttp-0.2.0/src/typedhttp/py.typed
+-rw-r--r--   0        0        0     2336 2023-07-17 13:50:21.251086 typedhttp-0.2.0/src/typedhttp/requests_hook.py
+-rw-r--r--   0        0        0      495 1970-01-01 00:00:00.000000 typedhttp-0.2.0/PKG-INFO
```

### Comparing `typedhttp-0.1.0/src/typedhttp/main.py` & `typedhttp-0.2.0/src/typedhttp/main.py`

 * *Files identical despite different names*

### Comparing `typedhttp-0.1.0/src/typedhttp/requests_hook.py` & `typedhttp-0.2.0/src/typedhttp/requests_hook.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-from typing import (
-    Iterator,
-    List,
-    Tuple,
-)
+from typing import Iterator, List, Tuple, TypeVar
 
 import requests
 
-from typedhttp import HTTPHandler, HTTPRequestObject, ResponseProvider, T
+from typedhttp import HTTPHandler, HTTPRequestObject, ResponseProvider
+
+T = TypeVar("T")
 
 class RequestsResponseProvider(ResponseProvider):
     def __init__(self, response: requests.Response) -> None:
         self.response = response
 
     def get_raw_response(self) -> bytes:
         return self.response.content
```

