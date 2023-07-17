# Comparing `tmp/sigtech-0.0.38.tar.gz` & `tmp/sigtech-0.0.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigtech-0.0.38.tar", last modified: Mon Jul 17 12:37:47 2023, max compression
+gzip compressed data, was "sigtech-0.0.39.tar", last modified: Mon Jul 17 15:03:03 2023, max compression
```

## Comparing `sigtech-0.0.38.tar` & `sigtech-0.0.39.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:37:47.039963 sigtech-0.0.38/
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-17 12:37:16.000000 sigtech-0.0.38/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8232 2023-07-17 12:37:47.039963 sigtech-0.0.38/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-07-17 12:37:16.000000 sigtech-0.0.38/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-17 12:37:16.000000 sigtech-0.0.38/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 12:37:47.039963 sigtech-0.0.38/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:37:47.035963 sigtech-0.0.38/sigtech/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-17 12:37:16.000000 sigtech-0.0.38/sigtech/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:37:47.035963 sigtech-0.0.38/sigtech/api/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-17 12:37:16.000000 sigtech-0.0.38/sigtech/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:37:47.039963 sigtech-0.0.38/sigtech/api/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 12:37:16.000000 sigtech-0.0.38/sigtech/api/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-07-17 12:37:16.000000 sigtech-0.0.38/sigtech/api/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-07-17 12:37:16.000000 sigtech-0.0.38/sigtech/api/client/response.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-17 12:37:16.000000 sigtech-0.0.38/sigtech/api/client/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:37:47.039963 sigtech-0.0.38/sigtech/api/framework/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 12:37:16.000000 sigtech-0.0.38/sigtech/api/framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-07-17 12:37:16.000000 sigtech-0.0.38/sigtech/api/framework/basket_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-07-17 12:37:16.000000 sigtech-0.0.38/sigtech/api/framework/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-17 12:37:16.000000 sigtech-0.0.38/sigtech/api/framework/framework_api_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-17 12:37:16.000000 sigtech-0.0.38/sigtech/api/framework/instrument_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-07-17 12:37:16.000000 sigtech-0.0.38/sigtech/api/framework/rolling_future_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-07-17 12:37:16.000000 sigtech-0.0.38/sigtech/api/framework/signal_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-17 12:37:16.000000 sigtech-0.0.38/sigtech/api/framework/strategy_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:37:47.035963 sigtech-0.0.38/sigtech.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8232 2023-07-17 12:37:47.000000 sigtech-0.0.38/sigtech.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-17 12:37:47.000000 sigtech-0.0.38/sigtech.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 12:37:47.000000 sigtech-0.0.38/sigtech.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-17 12:37:47.000000 sigtech-0.0.38/sigtech.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-17 12:37:47.000000 sigtech-0.0.38/sigtech.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:37:47.039963 sigtech-0.0.38/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-17 12:37:16.000000 sigtech-0.0.38/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-17 12:37:16.000000 sigtech-0.0.38/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-17 12:37:16.000000 sigtech-0.0.38/tests/test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-17 12:37:16.000000 sigtech-0.0.38/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:03:03.673523 sigtech-0.0.39/
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-17 15:02:39.000000 sigtech-0.0.39/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8232 2023-07-17 15:03:03.669523 sigtech-0.0.39/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-07-17 15:02:39.000000 sigtech-0.0.39/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-17 15:02:39.000000 sigtech-0.0.39/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 15:03:03.673523 sigtech-0.0.39/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:03:03.665523 sigtech-0.0.39/sigtech/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-17 15:02:39.000000 sigtech-0.0.39/sigtech/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:03:03.669523 sigtech-0.0.39/sigtech/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-17 15:02:39.000000 sigtech-0.0.39/sigtech/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:03:03.669523 sigtech-0.0.39/sigtech/api/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:02:39.000000 sigtech-0.0.39/sigtech/api/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-07-17 15:02:39.000000 sigtech-0.0.39/sigtech/api/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-07-17 15:02:39.000000 sigtech-0.0.39/sigtech/api/client/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-17 15:02:39.000000 sigtech-0.0.39/sigtech/api/client/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:03:03.669523 sigtech-0.0.39/sigtech/api/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:02:39.000000 sigtech-0.0.39/sigtech/api/framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-07-17 15:02:39.000000 sigtech-0.0.39/sigtech/api/framework/basket_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-07-17 15:02:39.000000 sigtech-0.0.39/sigtech/api/framework/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-17 15:02:39.000000 sigtech-0.0.39/sigtech/api/framework/framework_api_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-17 15:02:39.000000 sigtech-0.0.39/sigtech/api/framework/instrument_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-07-17 15:02:39.000000 sigtech-0.0.39/sigtech/api/framework/rolling_future_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-07-17 15:02:39.000000 sigtech-0.0.39/sigtech/api/framework/signal_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-17 15:02:39.000000 sigtech-0.0.39/sigtech/api/framework/strategy_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:03:03.665523 sigtech-0.0.39/sigtech.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8232 2023-07-17 15:03:03.000000 sigtech-0.0.39/sigtech.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-17 15:03:03.000000 sigtech-0.0.39/sigtech.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 15:03:03.000000 sigtech-0.0.39/sigtech.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-17 15:03:03.000000 sigtech-0.0.39/sigtech.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-17 15:03:03.000000 sigtech-0.0.39/sigtech.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:03:03.669523 sigtech-0.0.39/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-17 15:02:39.000000 sigtech-0.0.39/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-17 15:02:39.000000 sigtech-0.0.39/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-17 15:02:39.000000 sigtech-0.0.39/tests/test_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-17 15:02:39.000000 sigtech-0.0.39/tests/test_utils.py
```

### Comparing `sigtech-0.0.38/LICENSE.txt` & `sigtech-0.0.39/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sigtech-0.0.38/PKG-INFO` & `sigtech-0.0.39/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigtech
-Version: 0.0.38
+Version: 0.0.39
 Summary: SigTech Python SDK
 Author-email: SigTech <support@sigtech.com>
 License: MIT
 Project-URL: Homepage, https://github.com/SIGTechnologies/sigtech-python
 Keywords: SIGTECH,FINANCE,TRADING,BACKTEST,QUANT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sigtech Version: 0.0.38 Summary: SigTech Python SDK
+Metadata-Version: 2.1 Name: sigtech Version: 0.0.39 Summary: SigTech Python SDK
 Author-email: SigTech
 sigtech.com> License: MIT Project-URL: Homepage, https://github.com/
 SIGTechnologies/sigtech-python Keywords: SIGTECH,FINANCE,TRADING,BACKTEST,QUANT
 Classifier: Development Status :: 5 - Production/Stable Classifier: Operating
 System :: OS Independent Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Financial and Insurance Industry Classifier: Programming Language :: Python
```

### Comparing `sigtech-0.0.38/README.md` & `sigtech-0.0.39/README.md`

 * *Files identical despite different names*

### Comparing `sigtech-0.0.38/pyproject.toml` & `sigtech-0.0.39/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sigtech"
-version = "0.0.38"
+version = "0.0.39"
 authors = [
   { name="SigTech", email="support@sigtech.com" },
 ]
 description = "SigTech Python SDK"
 readme = {file = "README.md", content-type = "text/markdown"}
 keywords = ["SIGTECH", "FINANCE", "TRADING", "BACKTEST", "QUANT"]
 license = {text= "MIT"}
```

### Comparing `sigtech-0.0.38/sigtech/api/client/client.py` & `sigtech-0.0.39/sigtech/api/client/client.py`

 * *Files identical despite different names*

### Comparing `sigtech-0.0.38/sigtech/api/client/response.py` & `sigtech-0.0.39/sigtech/api/client/response.py`

 * *Files identical despite different names*

### Comparing `sigtech-0.0.38/sigtech/api/client/utils.py` & `sigtech-0.0.39/sigtech/api/client/utils.py`

 * *Files identical despite different names*

### Comparing `sigtech-0.0.38/sigtech/api/framework/basket_strategy.py` & `sigtech-0.0.39/sigtech/api/framework/basket_strategy.py`

 * *Files identical despite different names*

### Comparing `sigtech-0.0.38/sigtech/api/framework/environment.py` & `sigtech-0.0.39/sigtech/api/framework/environment.py`

 * *Files identical despite different names*

### Comparing `sigtech-0.0.38/sigtech/api/framework/framework_api_object.py` & `sigtech-0.0.39/sigtech/api/framework/framework_api_object.py`

 * *Files identical despite different names*

### Comparing `sigtech-0.0.38/sigtech/api/framework/instrument_base.py` & `sigtech-0.0.39/sigtech/api/framework/instrument_base.py`

 * *Files identical despite different names*

### Comparing `sigtech-0.0.38/sigtech/api/framework/rolling_future_strategy.py` & `sigtech-0.0.39/sigtech/api/framework/rolling_future_strategy.py`

 * *Files identical despite different names*

### Comparing `sigtech-0.0.38/sigtech/api/framework/signal_strategy.py` & `sigtech-0.0.39/sigtech/api/framework/signal_strategy.py`

 * *Files identical despite different names*

### Comparing `sigtech-0.0.38/sigtech/api/framework/strategy_base.py` & `sigtech-0.0.39/sigtech/api/framework/strategy_base.py`

 * *Files identical despite different names*

### Comparing `sigtech-0.0.38/sigtech.egg-info/PKG-INFO` & `sigtech-0.0.39/sigtech.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigtech
-Version: 0.0.38
+Version: 0.0.39
 Summary: SigTech Python SDK
 Author-email: SigTech <support@sigtech.com>
 License: MIT
 Project-URL: Homepage, https://github.com/SIGTechnologies/sigtech-python
 Keywords: SIGTECH,FINANCE,TRADING,BACKTEST,QUANT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sigtech Version: 0.0.38 Summary: SigTech Python SDK
+Metadata-Version: 2.1 Name: sigtech Version: 0.0.39 Summary: SigTech Python SDK
 Author-email: SigTech
 sigtech.com> License: MIT Project-URL: Homepage, https://github.com/
 SIGTechnologies/sigtech-python Keywords: SIGTECH,FINANCE,TRADING,BACKTEST,QUANT
 Classifier: Development Status :: 5 - Production/Stable Classifier: Operating
 System :: OS Independent Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Financial and Insurance Industry Classifier: Programming Language :: Python
```

### Comparing `sigtech-0.0.38/sigtech.egg-info/SOURCES.txt` & `sigtech-0.0.39/sigtech.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sigtech-0.0.38/tests/test_client.py` & `sigtech-0.0.39/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `sigtech-0.0.38/tests/test_examples.py` & `sigtech-0.0.39/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `sigtech-0.0.38/tests/test_response.py` & `sigtech-0.0.39/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `sigtech-0.0.38/tests/test_utils.py` & `sigtech-0.0.39/tests/test_utils.py`

 * *Files identical despite different names*

