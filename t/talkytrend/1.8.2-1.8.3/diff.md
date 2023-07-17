# Comparing `tmp/talkytrend-1.8.2.tar.gz` & `tmp/talkytrend-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talkytrend-1.8.2.tar", max compression
+gzip compressed data, was "talkytrend-1.8.3.tar", max compression
```

## Comparing `talkytrend-1.8.2.tar` & `talkytrend-1.8.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-07-17 05:55:37.496523 talkytrend-1.8.2/LICENSE
--rw-r--r--   0        0        0     3446 2023-07-17 05:55:37.496523 talkytrend-1.8.2/README.md
--rw-r--r--   0        0        0     2476 2023-07-17 05:55:38.264550 talkytrend-1.8.2/pyproject.toml
--rw-r--r--   0        0        0      101 2023-07-17 05:55:38.264550 talkytrend-1.8.2/talkytrend/__init__.py
--rw-r--r--   0        0        0      706 2023-07-17 05:55:37.496523 talkytrend-1.8.2/talkytrend/config.py
--rw-r--r--   0        0        0     2285 2023-07-17 05:55:37.496523 talkytrend-1.8.2/talkytrend/default_settings.toml
--rw-r--r--   0        0        0     7377 2023-07-17 05:55:37.496523 talkytrend-1.8.2/talkytrend/main.py
--rw-r--r--   0        0        0     4470 1970-01-01 00:00:00.000000 talkytrend-1.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-17 06:28:58.370004 talkytrend-1.8.3/LICENSE
+-rw-r--r--   0        0        0     3446 2023-07-17 06:28:58.370004 talkytrend-1.8.3/README.md
+-rw-r--r--   0        0        0     2475 2023-07-17 06:28:59.142008 talkytrend-1.8.3/pyproject.toml
+-rw-r--r--   0        0        0      101 2023-07-17 06:28:59.142008 talkytrend-1.8.3/talkytrend/__init__.py
+-rw-r--r--   0        0        0      706 2023-07-17 06:28:58.370004 talkytrend-1.8.3/talkytrend/config.py
+-rw-r--r--   0        0        0     2285 2023-07-17 06:28:58.370004 talkytrend-1.8.3/talkytrend/default_settings.toml
+-rw-r--r--   0        0        0     7377 2023-07-17 06:28:58.370004 talkytrend-1.8.3/talkytrend/main.py
+-rw-r--r--   0        0        0     4470 1970-01-01 00:00:00.000000 talkytrend-1.8.3/PKG-INFO
```

### Comparing `talkytrend-1.8.2/LICENSE` & `talkytrend-1.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `talkytrend-1.8.2/README.md` & `talkytrend-1.8.3/README.md`

 * *Files identical despite different names*

### Comparing `talkytrend-1.8.2/pyproject.toml` & `talkytrend-1.8.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "talkytrend"
-version = "1.8.2"
+version = "1.8.3"
 description = "A python package to retrieve  economic data such as Trend for any financial symbol."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["finance", "crypto", "bot","trend","economic"]
 packages = [
     {include = "talkytrend"}
@@ -28,15 +28,15 @@
 aiohttp = "^3.8.4"
 tradingview_ta = "^3.3.0"
 prettytable = "^3.8.0"
 alphavantage_api_client = "^2.2.2"
 xmltodict = "*"
 
 [tool.poetry.dev-dependencies]
-python-semantic-release = "^7.34.3"
+python-semantic-release = "^8.0.0"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.0"
 pytest-cov = "^4.1"
 pytest-asyncio = "^0.21.0"
 pytest-mock = "^3.11.1"
```

### Comparing `talkytrend-1.8.2/talkytrend/config.py` & `talkytrend-1.8.3/talkytrend/config.py`

 * *Files identical despite different names*

### Comparing `talkytrend-1.8.2/talkytrend/default_settings.toml` & `talkytrend-1.8.3/talkytrend/default_settings.toml`

 * *Files identical despite different names*

### Comparing `talkytrend-1.8.2/talkytrend/main.py` & `talkytrend-1.8.3/talkytrend/main.py`

 * *Files identical despite different names*

### Comparing `talkytrend-1.8.2/PKG-INFO` & `talkytrend-1.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talkytrend
-Version: 1.8.2
+Version: 1.8.3
 Summary: A python package to retrieve  economic data such as Trend for any financial symbol.
 License: MIT
 Keywords: finance,crypto,bot,trend,economic
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: talkytrend Version: 1.8.2 Summary: A python package
+Metadata-Version: 2.1 Name: talkytrend Version: 1.8.3 Summary: A python package
 to retrieve economic data such as Trend for any financial symbol. License: MIT
 Keywords: finance,crypto,bot,trend,economic Author: mraniki Author-email:
 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: aiohttp
 (>=3.8.4,<4.0.0) Requires-Dist: alphavantage_api_client (>=2.2.2,<3.0.0)
```

