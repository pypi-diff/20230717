# Comparing `tmp/crypto-ws-api-1.0.1.tar.gz` & `tmp/crypto-ws-api-1.0.1.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-ws-api-1.0.1.tar", last modified: Tue Jul  4 16:29:38 2023, max compression
+gzip compressed data, was "crypto-ws-api-1.0.1.post3.tar", last modified: Mon Jul 17 18:53:55 2023, max compression
```

## Comparing `crypto-ws-api-1.0.1.tar` & `crypto-ws-api-1.0.1.post3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      165 2022-06-06 16:51:29.613842 crypto-ws-api-1.0.1/.deepsource.toml
--rwxr-xr-x   0        0        0      180 2023-07-04 16:26:13.069466 crypto-ws-api-1.0.1/CHANGELOG.md
--rw-r--r--   0        0        0     1078 2023-06-30 17:01:10.037954 crypto-ws-api-1.0.1/LICENSE.md
--rw-r--r--   0        0        0     5781 2023-07-04 12:03:35.360477 crypto-ws-api-1.0.1/README.md
--rw-r--r--   0        0        0     1301 2023-07-04 16:26:13.073459 crypto-ws-api-1.0.1/crypto_ws_api/__init__.py
--rw-r--r--   0        0        0     3511 2023-07-04 15:47:08.409027 crypto-ws-api-1.0.1/crypto_ws_api/demo.py
--rw-r--r--   0        0        0      551 2023-07-01 18:52:39.110102 crypto-ws-api-1.0.1/crypto_ws_api/ws_api.toml.template
--rw-r--r--   0        0        0    10363 2023-07-04 16:26:13.065474 crypto-ws-api-1.0.1/crypto_ws_api/ws_session.py
--rw-r--r--   0        0        0     1000 2023-07-03 19:17:40.031531 crypto-ws-api-1.0.1/pyproject.toml
--rw-r--r--   0        0        0       90 2023-07-03 18:01:56.150626 crypto-ws-api-1.0.1/requirements.txt
--rw-r--r--   0        0        0     6531 1970-01-01 00:00:00.000000 crypto-ws-api-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      165 2022-06-06 16:51:29.613842 crypto-ws-api-1.0.1.post3/.deepsource.toml
+-rwxr-xr-x   0        0        0      373 2023-07-17 18:01:30.262695 crypto-ws-api-1.0.1.post3/CHANGELOG.md
+-rw-r--r--   0        0        0     1078 2023-06-30 17:01:10.037954 crypto-ws-api-1.0.1.post3/LICENSE.md
+-rw-r--r--   0        0        0     5768 2023-07-05 15:44:42.509478 crypto-ws-api-1.0.1.post3/README.md
+-rw-r--r--   0        0        0     1303 2023-07-17 18:34:11.883696 crypto-ws-api-1.0.1.post3/crypto_ws_api/__init__.py
+-rw-r--r--   0        0        0     3511 2023-07-17 18:01:30.262695 crypto-ws-api-1.0.1.post3/crypto_ws_api/demo.py
+-rw-r--r--   0        0        0      551 2023-07-01 18:52:39.110102 crypto-ws-api-1.0.1.post3/crypto_ws_api/ws_api.toml.template
+-rw-r--r--   0        0        0    10528 2023-07-17 18:01:30.262695 crypto-ws-api-1.0.1.post3/crypto_ws_api/ws_session.py
+-rw-r--r--   0        0        0      993 2023-07-17 18:34:11.879713 crypto-ws-api-1.0.1.post3/pyproject.toml
+-rw-r--r--   0        0        0       83 2023-07-17 18:34:11.891662 crypto-ws-api-1.0.1.post3/requirements.txt
+-rw-r--r--   0        0        0     6517 1970-01-01 00:00:00.000000 crypto-ws-api-1.0.1.post3/PKG-INFO
```

### Comparing `crypto-ws-api-1.0.1/LICENSE.md` & `crypto-ws-api-1.0.1.post3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `crypto-ws-api-1.0.1/README.md` & `crypto-ws-api-1.0.1.post3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,15 @@
-
-<p align="center"><img src="https://user-images.githubusercontent.com/77513676/250364389-cbedc171-a930-4467-a0cd-21627a6a41ed.svg" width="250"></p>
-
-***
-<h1 align="center">Crypto WS API connector for ASYNC requests</h1>
+<h1 align="center"><img align="center" src="https://user-images.githubusercontent.com/77513676/250364389-cbedc171-a930-4467-a0cd-21627a6a41ed.svg" width="75">Crypto WS API connector for ASYNC requests</h1>
 
 <h2 align="center">Full coverage of all methods provided by the interface</h2>
 
 <h3 align="center">Provides of connection management, keepalive and rate limits control</h3>
 
 ***
-<a href="https://badge.fury.io/py/crypto-ws-api"><img src="https://badge.fury.io/py/crypto-ws-api.svg" alt="PyPI version"></a>
+<a href="https://pypi.org/project/crypto-ws-api/"><img src="https://img.shields.io/pypi/v/crypto-ws-api" alt="PyPI version"></a>
 <a href="https://codeclimate.com/github/DogsTailFarmer/crypto-ws-api/maintainability"><img src="https://api.codeclimate.com/v1/badges/2d2a654ba393eb88d911/maintainability" /></a>
 <a href="https://app.deepsource.com/gh/DogsTailFarmer/crypto-ws-api/?ref=repository-badge}" target="_blank"><img alt="DeepSource" title="DeepSource" src="https://app.deepsource.com/gh/DogsTailFarmer/crypto-ws-api.svg/?label=resolved+issues&token=TXghPzbi0YWhkCLU8Q1tmDyQ"/></a>
 <a href="https://app.deepsource.com/gh/DogsTailFarmer/crypto-ws-api/?ref=repository-badge}" target="_blank"><img alt="DeepSource" title="DeepSource" src="https://app.deepsource.com/gh/DogsTailFarmer/crypto-ws-api.svg/?label=active+issues&token=TXghPzbi0YWhkCLU8Q1tmDyQ"/></a>
 <a href="https://sonarcloud.io/summary/new_code?id=DogsTailFarmer_crypto-ws-api" target="_blank"><img alt="sonarcloud" title="sonarcloud" src="https://sonarcloud.io/api/project_badges/measure?project=DogsTailFarmer_crypto-ws-api&metric=alert_status"/></a>
 <a href="https://pepy.tech/project/crypto-ws-api" target="_blank"><img alt="Downloads" title="Downloads" src="https://static.pepy.tech/badge/crypto-ws-api"/></a>
 ***
 For :heavy_check_mark:Binance,
```

#### html2text {}

```diff
@@ -1,11 +1,10 @@
- [https://user-images.githubusercontent.com/77513676/250364389-cbedc171-a930-
-                          4467-a0cd-21627a6a41ed.svg]
-***
-           ****** Crypto WS API connector for ASYNC requests ******
+****** [https://user-images.githubusercontent.com/77513676/250364389-cbedc171-
+  a930-4467-a0cd-21627a6a41ed.svg]Crypto WS API connector for ASYNC requests
+                                    ******
       ***** Full coverage of all methods provided by the interface *****
 **** Provides of connection management, keepalive and rate limits control ****
 *** [PyPI_version] [https://api.codeclimate.com/v1/badges/2d2a654ba393eb88d911/
 maintainability] [DeepSource] [DeepSource] [sonarcloud] [Downloads] *** For :
 heavy_check_mark:Binance, *** ## Features Lightweight and efficient solution to
 utilize of all available methods provided through the: * [Binance Websocket API
 v3](https://developers.binance.com/docs/binance-trading-api/websocket_api) ###
```

### Comparing `crypto-ws-api-1.0.1/crypto_ws_api/__init__.py` & `crypto-ws-api-1.0.1.post3/crypto_ws_api/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 """
 __authors__ = ["Jerry Fedorenko"]
 __license__ = "MIT"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 __email__ = "jerry.fedorenko@yahoo.com"
 __credits__ = ["https://github.com/DanyaSWorlD"]
-__version__ = "1.0.1"
+__version__ = "1.0.1-3"
 
 from pathlib import Path
 import shutil
 from platformdirs import user_config_path
 
 
 TIMEOUT = 10  # sec timeout for WSS receive
```

### Comparing `crypto-ws-api-1.0.1/crypto_ws_api/demo.py` & `crypto-ws-api-1.0.1.post3/crypto_ws_api/demo.py`

 * *Files identical despite different names*

### Comparing `crypto-ws-api-1.0.1/crypto_ws_api/ws_api.toml.template` & `crypto-ws-api-1.0.1.post3/crypto_ws_api/ws_api.toml.template`

 * *Files identical despite different names*

### Comparing `crypto-ws-api-1.0.1/crypto_ws_api/ws_session.py` & `crypto-ws-api-1.0.1.post3/crypto_ws_api/ws_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,19 +33,22 @@
         "trade_id",
         "operational_status",
         "order_handling",
     )
 
     def __init__(
             self,
-            api_key: str,
-            api_secret: str,
-            session: aiohttp.ClientSession,
-            endpoint: str
+            api_key: str = None,
+            api_secret: str = None,
+            session: aiohttp.ClientSession = None,
+            endpoint: str = None
     ):
+        if None in {api_key, api_secret, session, endpoint}:
+            raise UserWarning("UserWSSession: all parameters must be set")
+
         self._api_key = api_key
         self._api_secret = api_secret
         self._session = session
         self._endpoint = endpoint
         self._web_socket = None
         self._listen_key = None
         self._try_count = 0
```

### Comparing `crypto-ws-api-1.0.1/pyproject.toml` & `crypto-ws-api-1.0.1.post3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
              "Operating System :: Unix",
              "Operating System :: Microsoft :: Windows",
              "Operating System :: MacOS"]
 dynamic = ["version", "description"]
 requires-python = ">=3.8"
 
 dependencies = [
-    "exchanges-wrapper~=1.3.2",
+    "exchanges-wrapper",
     "aiohttp==3.8.4",
     "shortuuid~=1.0.11",
     "platformdirs~=3.8.0",
     "toml~=0.10.2",
 ]
 
 [tool.flit.module]
```

### Comparing `crypto-ws-api-1.0.1/PKG-INFO` & `crypto-ws-api-1.0.1.post3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,35 @@
 Metadata-Version: 2.1
 Name: crypto-ws-api
-Version: 1.0.1
+Version: 1.0.1.post3
 Summary: Crypto WS API connector for ASYNC requests
 Author-email: Jerry Fedorenko <jerry.fedorenko@yahoo.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
-Requires-Dist: exchanges-wrapper~=1.3.2
+Requires-Dist: exchanges-wrapper
 Requires-Dist: aiohttp==3.8.4
 Requires-Dist: shortuuid~=1.0.11
 Requires-Dist: platformdirs~=3.8.0
 Requires-Dist: toml~=0.10.2
 Project-URL: Source, https://github.com/DogsTailFarmer/crypto-ws-api
 
-
-<p align="center"><img src="https://user-images.githubusercontent.com/77513676/250364389-cbedc171-a930-4467-a0cd-21627a6a41ed.svg" width="250"></p>
-
-***
-<h1 align="center">Crypto WS API connector for ASYNC requests</h1>
+<h1 align="center"><img align="center" src="https://user-images.githubusercontent.com/77513676/250364389-cbedc171-a930-4467-a0cd-21627a6a41ed.svg" width="75">Crypto WS API connector for ASYNC requests</h1>
 
 <h2 align="center">Full coverage of all methods provided by the interface</h2>
 
 <h3 align="center">Provides of connection management, keepalive and rate limits control</h3>
 
 ***
-<a href="https://badge.fury.io/py/crypto-ws-api"><img src="https://badge.fury.io/py/crypto-ws-api.svg" alt="PyPI version"></a>
+<a href="https://pypi.org/project/crypto-ws-api/"><img src="https://img.shields.io/pypi/v/crypto-ws-api" alt="PyPI version"></a>
 <a href="https://codeclimate.com/github/DogsTailFarmer/crypto-ws-api/maintainability"><img src="https://api.codeclimate.com/v1/badges/2d2a654ba393eb88d911/maintainability" /></a>
 <a href="https://app.deepsource.com/gh/DogsTailFarmer/crypto-ws-api/?ref=repository-badge}" target="_blank"><img alt="DeepSource" title="DeepSource" src="https://app.deepsource.com/gh/DogsTailFarmer/crypto-ws-api.svg/?label=resolved+issues&token=TXghPzbi0YWhkCLU8Q1tmDyQ"/></a>
 <a href="https://app.deepsource.com/gh/DogsTailFarmer/crypto-ws-api/?ref=repository-badge}" target="_blank"><img alt="DeepSource" title="DeepSource" src="https://app.deepsource.com/gh/DogsTailFarmer/crypto-ws-api.svg/?label=active+issues&token=TXghPzbi0YWhkCLU8Q1tmDyQ"/></a>
 <a href="https://sonarcloud.io/summary/new_code?id=DogsTailFarmer_crypto-ws-api" target="_blank"><img alt="sonarcloud" title="sonarcloud" src="https://sonarcloud.io/api/project_badges/measure?project=DogsTailFarmer_crypto-ws-api&metric=alert_status"/></a>
 <a href="https://pepy.tech/project/crypto-ws-api" target="_blank"><img alt="Downloads" title="Downloads" src="https://static.pepy.tech/badge/crypto-ws-api"/></a>
 ***
 For :heavy_check_mark:Binance,
```

#### html2text {}

```diff
@@ -1,22 +1,21 @@
-Metadata-Version: 2.1 Name: crypto-ws-api Version: 1.0.1 Summary: Crypto WS API
-connector for ASYNC requests Author-email: Jerry Fedorenko
+Metadata-Version: 2.1 Name: crypto-ws-api Version: 1.0.1.post3 Summary: Crypto
+WS API connector for ASYNC requests Author-email: Jerry Fedorenko
 fedorenko@yahoo.com> Requires-Python: >=3.8 Description-Content-Type: text/
 markdown Classifier: Programming Language :: Python :: 3 Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: Unix Classifier: Operating
 System :: Microsoft :: Windows Classifier: Operating System :: MacOS Requires-
-Dist: exchanges-wrapper~=1.3.2 Requires-Dist: aiohttp==3.8.4 Requires-Dist:
+Dist: exchanges-wrapper Requires-Dist: aiohttp==3.8.4 Requires-Dist:
 shortuuid~=1.0.11 Requires-Dist: platformdirs~=3.8.0 Requires-Dist:
 toml~=0.10.2 Project-URL: Source, https://github.com/DogsTailFarmer/crypto-ws-
 api
- [https://user-images.githubusercontent.com/77513676/250364389-cbedc171-a930-
-                          4467-a0cd-21627a6a41ed.svg]
-***
-           ****** Crypto WS API connector for ASYNC requests ******
+****** [https://user-images.githubusercontent.com/77513676/250364389-cbedc171-
+  a930-4467-a0cd-21627a6a41ed.svg]Crypto WS API connector for ASYNC requests
+                                    ******
       ***** Full coverage of all methods provided by the interface *****
 **** Provides of connection management, keepalive and rate limits control ****
 *** [PyPI_version] [https://api.codeclimate.com/v1/badges/2d2a654ba393eb88d911/
 maintainability] [DeepSource] [DeepSource] [sonarcloud] [Downloads] *** For :
 heavy_check_mark:Binance, *** ## Features Lightweight and efficient solution to
 utilize of all available methods provided through the: * [Binance Websocket API
 v3](https://developers.binance.com/docs/binance-trading-api/websocket_api) ###
```

