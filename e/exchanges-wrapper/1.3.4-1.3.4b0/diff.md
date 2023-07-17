# Comparing `tmp/exchanges_wrapper-1.3.4.tar.gz` & `tmp/exchanges-wrapper-1.3.4b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exchanges_wrapper-1.3.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "exchanges-wrapper-1.3.4b0.tar", last modified: Sun Jul 16 16:11:52 2023, max compression
```

## Comparing `exchanges_wrapper-1.3.4.tar` & `exchanges-wrapper-1.3.4b0.tar`

### file list

```diff
@@ -1,20 +1,31 @@
--rw-r--r--   0        0        0     1114 2023-07-17 07:08:35.651978 exchanges_wrapper-1.3.4/LICENSE.md
--rw-r--r--   0        0        0     7068 2023-07-17 07:08:35.651978 exchanges_wrapper-1.3.4/README.md
--rw-r--r--   0        0        0     1317 2023-07-17 07:08:35.655978 exchanges_wrapper-1.3.4/exchanges_wrapper/__init__.py
--rw-r--r--   0        0        0    25161 2023-07-17 07:08:35.655978 exchanges_wrapper-1.3.4/exchanges_wrapper/api_pb2.py
--rw-r--r--   0        0        0    44445 2023-07-17 07:08:35.655978 exchanges_wrapper-1.3.4/exchanges_wrapper/api_pb2_grpc.py
--rw-r--r--   0        0        0    19609 2023-07-17 07:08:35.655978 exchanges_wrapper-1.3.4/exchanges_wrapper/bitfinex_parser.py
--rw-r--r--   0        0        0     6184 2023-07-17 07:08:35.655978 exchanges_wrapper-1.3.4/exchanges_wrapper/c_structures.py
--rw-r--r--   0        0        0    61849 2023-07-17 07:08:35.655978 exchanges_wrapper-1.3.4/exchanges_wrapper/client.py
--rw-r--r--   0        0        0     2768 2023-07-17 07:08:35.655978 exchanges_wrapper-1.3.4/exchanges_wrapper/definitions.py
--rw-r--r--   0        0        0      796 2023-07-17 07:08:35.655978 exchanges_wrapper-1.3.4/exchanges_wrapper/errors.py
--rw-r--r--   0        0        0    12485 2023-07-17 07:08:35.655978 exchanges_wrapper-1.3.4/exchanges_wrapper/events.py
--rwxr-xr-x   0        0        0    47721 2023-07-17 07:08:35.655978 exchanges_wrapper-1.3.4/exchanges_wrapper/exch_srv.py
--rw-r--r--   0        0        0     4429 2023-07-17 07:08:35.655978 exchanges_wrapper-1.3.4/exchanges_wrapper/exch_srv_cfg.toml.template
--rw-r--r--   0        0        0    10260 2023-07-17 07:08:35.655978 exchanges_wrapper-1.3.4/exchanges_wrapper/http_client.py
--rw-r--r--   0        0        0    15714 2023-07-17 07:08:35.655978 exchanges_wrapper-1.3.4/exchanges_wrapper/huobi_parser.py
--rw-r--r--   0        0        0    16089 2023-07-17 07:08:35.655978 exchanges_wrapper-1.3.4/exchanges_wrapper/okx_parser.py
--rw-r--r--   0        0        0    12097 2023-07-17 07:08:35.655978 exchanges_wrapper-1.3.4/exchanges_wrapper/proto/exchanges_wrapper/api.proto
--rw-r--r--   0        0        0    22397 2023-07-17 07:08:35.655978 exchanges_wrapper-1.3.4/exchanges_wrapper/web_sockets.py
--rw-r--r--   0        0        0     1147 2023-07-17 07:08:35.655978 exchanges_wrapper-1.3.4/pyproject.toml
--rw-r--r--   0        0        0     7980 1970-01-01 00:00:00.000000 exchanges_wrapper-1.3.4/PKG-INFO
+-rw-r--r--   0        0        0      165 2022-06-06 16:51:29.613842 exchanges-wrapper-1.3.4b0/.deepsource.toml
+-rw-r--r--   0        0        0       78 2022-09-23 15:45:46.921324 exchanges-wrapper-1.3.4b0/.dockerignore
+-rw-r--r--   0        0        0       71 2022-06-07 10:33:14.780369 exchanges-wrapper-1.3.4b0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      502 2022-09-23 19:36:49.587213 exchanges-wrapper-1.3.4b0/.github/dependabot.yml
+-rw-r--r--   0        0        0      950 2023-06-21 13:50:12.422384 exchanges-wrapper-1.3.4b0/.github/workflows/docker-image.yml
+-rw-r--r--   0        0        0     1105 2023-06-21 11:56:25.815510 exchanges-wrapper-1.3.4b0/.github/workflows/python-publish.yml
+-rwxr-xr-x   0        0        0     6960 2023-07-11 17:04:46.392454 exchanges-wrapper-1.3.4b0/CHANGELOG.md
+-rw-r--r--   0        0        0      641 2022-09-23 17:33:34.192514 exchanges-wrapper-1.3.4b0/Dockerfile
+-rw-r--r--   0        0        0     1114 2022-05-29 08:10:10.422624 exchanges-wrapper-1.3.4b0/LICENSE.md
+-rw-r--r--   0        0        0     7068 2023-07-06 10:11:57.993253 exchanges-wrapper-1.3.4b0/README.md
+-rw-r--r--   0        0        0    15398 2023-06-19 18:46:17.287114 exchanges-wrapper-1.3.4b0/example/exch_client.py
+-rwxr-xr-x   0        0        0      216 2023-06-20 16:57:56.566218 exchanges-wrapper-1.3.4b0/example/ms_cfg.toml
+-rw-r--r--   0        0        0     1319 2023-07-16 16:05:47.206493 exchanges-wrapper-1.3.4b0/exchanges_wrapper/__init__.py
+-rw-r--r--   0        0        0    25161 2023-07-16 16:08:14.630475 exchanges-wrapper-1.3.4b0/exchanges_wrapper/api_pb2.py
+-rw-r--r--   0        0        0    44445 2023-07-16 16:08:14.634480 exchanges-wrapper-1.3.4b0/exchanges_wrapper/api_pb2_grpc.py
+-rw-r--r--   0        0        0    19609 2023-07-04 16:39:16.922863 exchanges-wrapper-1.3.4b0/exchanges_wrapper/bitfinex_parser.py
+-rw-r--r--   0        0        0     6184 2023-06-29 16:06:47.201826 exchanges-wrapper-1.3.4b0/exchanges_wrapper/c_structures.py
+-rw-r--r--   0        0        0    61849 2023-07-12 07:21:31.626804 exchanges-wrapper-1.3.4b0/exchanges_wrapper/client.py
+-rw-r--r--   0        0        0     2768 2023-06-29 16:06:47.201826 exchanges-wrapper-1.3.4b0/exchanges_wrapper/definitions.py
+-rw-r--r--   0        0        0      796 2023-06-14 12:41:55.572680 exchanges-wrapper-1.3.4b0/exchanges_wrapper/errors.py
+-rw-r--r--   0        0        0    12485 2023-07-04 16:39:16.922863 exchanges-wrapper-1.3.4b0/exchanges_wrapper/events.py
+-rwxr-xr-x   0        0        0    47721 2023-07-04 16:39:16.922863 exchanges-wrapper-1.3.4b0/exchanges_wrapper/exch_srv.py
+-rw-r--r--   0        0        0     4429 2023-06-29 16:06:47.201826 exchanges-wrapper-1.3.4b0/exchanges_wrapper/exch_srv_cfg.toml.template
+-rw-r--r--   0        0        0    10260 2023-07-08 19:35:27.596549 exchanges-wrapper-1.3.4b0/exchanges_wrapper/http_client.py
+-rw-r--r--   0        0        0    15714 2023-07-04 16:39:16.922863 exchanges-wrapper-1.3.4b0/exchanges_wrapper/huobi_parser.py
+-rw-r--r--   0        0        0    16089 2023-07-04 16:39:16.922863 exchanges-wrapper-1.3.4b0/exchanges_wrapper/okx_parser.py
+-rw-r--r--   0        0        0    12097 2023-06-19 18:46:17.287114 exchanges-wrapper-1.3.4b0/exchanges_wrapper/proto/exchanges_wrapper/api.proto
+-rw-r--r--   0        0        0    22397 2023-06-29 16:57:42.989839 exchanges-wrapper-1.3.4b0/exchanges_wrapper/web_sockets.py
+-rw-r--r--   0        0        0     1147 2023-07-16 16:05:47.190524 exchanges-wrapper-1.3.4b0/pyproject.toml
+-rw-r--r--   0        0        0      123 2023-07-16 16:05:47.198509 exchanges-wrapper-1.3.4b0/requirements.txt
+-rw-r--r--   0        0        0     7982 1970-01-01 00:00:00.000000 exchanges-wrapper-1.3.4b0/PKG-INFO
```

### Comparing `exchanges_wrapper-1.3.4/LICENSE.md` & `exchanges-wrapper-1.3.4b0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.4/README.md` & `exchanges-wrapper-1.3.4b0/README.md`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.4/exchanges_wrapper/__init__.py` & `exchanges-wrapper-1.3.4b0/exchanges_wrapper/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 __authors__ = ["Th0rgal", "Jerry Fedorenko"]
 __license__ = "MIT"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 __email__ = "jerry.fedorenko@yahoo.com"
 __credits__ = ["https://github.com/DanyaSWorlD"]
-__version__ = "1.3.4"
+__version__ = "1.3.4b0"
 
 from pathlib import Path
 import shutil
 
 WORK_PATH = Path(Path.home(), ".MartinBinance")
 CONFIG_PATH = Path(WORK_PATH, "config")
 CONFIG_FILE = Path(CONFIG_PATH, "exch_srv_cfg.toml")
```

### Comparing `exchanges_wrapper-1.3.4/exchanges_wrapper/api_pb2.py` & `exchanges-wrapper-1.3.4b0/exchanges_wrapper/api_pb2.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.4/exchanges_wrapper/api_pb2_grpc.py` & `exchanges-wrapper-1.3.4b0/exchanges_wrapper/api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.4/exchanges_wrapper/bitfinex_parser.py` & `exchanges-wrapper-1.3.4b0/exchanges_wrapper/bitfinex_parser.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.4/exchanges_wrapper/c_structures.py` & `exchanges-wrapper-1.3.4b0/exchanges_wrapper/c_structures.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.4/exchanges_wrapper/client.py` & `exchanges-wrapper-1.3.4b0/exchanges_wrapper/client.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.4/exchanges_wrapper/definitions.py` & `exchanges-wrapper-1.3.4b0/exchanges_wrapper/definitions.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.4/exchanges_wrapper/errors.py` & `exchanges-wrapper-1.3.4b0/exchanges_wrapper/errors.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.4/exchanges_wrapper/events.py` & `exchanges-wrapper-1.3.4b0/exchanges_wrapper/events.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.4/exchanges_wrapper/exch_srv.py` & `exchanges-wrapper-1.3.4b0/exchanges_wrapper/exch_srv.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.4/exchanges_wrapper/exch_srv_cfg.toml.template` & `exchanges-wrapper-1.3.4b0/exchanges_wrapper/exch_srv_cfg.toml.template`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.4/exchanges_wrapper/http_client.py` & `exchanges-wrapper-1.3.4b0/exchanges_wrapper/http_client.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.4/exchanges_wrapper/huobi_parser.py` & `exchanges-wrapper-1.3.4b0/exchanges_wrapper/huobi_parser.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.4/exchanges_wrapper/okx_parser.py` & `exchanges-wrapper-1.3.4b0/exchanges_wrapper/okx_parser.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.4/exchanges_wrapper/proto/exchanges_wrapper/api.proto` & `exchanges-wrapper-1.3.4b0/exchanges_wrapper/proto/exchanges_wrapper/api.proto`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.4/exchanges_wrapper/web_sockets.py` & `exchanges-wrapper-1.3.4b0/exchanges_wrapper/web_sockets.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.4/pyproject.toml` & `exchanges-wrapper-1.3.4b0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.4/PKG-INFO` & `exchanges-wrapper-1.3.4b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exchanges-wrapper
-Version: 1.3.4
+Version: 1.3.4b0
 Summary: REST API and WebSocket asyncio wrapper with grpc powered multiplexer server
 Author-email: Thomas Marchand <thomas.marchand@tuta.io>, Jerry Fedorenko <jerry.fedorenko@yahoo.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: exchanges-wrapper Version: 1.3.4 Summary: REST API
-and WebSocket asyncio wrapper with grpc powered multiplexer server Author-
+Metadata-Version: 2.1 Name: exchanges-wrapper Version: 1.3.4b0 Summary: REST
+API and WebSocket asyncio wrapper with grpc powered multiplexer server Author-
 email: Thomas Marchand
 marchand@tuta.io>, Jerry Fedorenko
 fedorenko@yahoo.com> Requires-Python: >=3.8 Description-Content-Type: text/
 markdown Classifier: Programming Language :: Python :: 3 Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: Unix Classifier: Operating
 System :: Microsoft :: Windows Classifier: Operating System :: MacOS Requires-
```

