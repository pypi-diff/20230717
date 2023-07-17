# Comparing `tmp/alphatools_jv-3.0.0.tar.gz` & `tmp/alphatools_jv-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphatools_jv-3.0.0.tar", last modified: Mon Jul 17 01:44:17 2023, max compression
+gzip compressed data, was "alphatools_jv-3.1.0.tar", last modified: Mon Jul 17 03:04:10 2023, max compression
```

## Comparing `alphatools_jv-3.0.0.tar` & `alphatools_jv-3.1.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 jaskiratsingh   (501) staff       (20)        0 2023-07-17 01:44:17.198527 alphatools_jv-3.0.0/
--rw-r--r--   0 jaskiratsingh   (501) staff       (20)     2055 2023-07-17 01:44:17.197622 alphatools_jv-3.0.0/PKG-INFO
--rw-r--r--   0 jaskiratsingh   (501) staff       (20)     1651 2023-07-13 23:58:33.000000 alphatools_jv-3.0.0/README.md
-drwxr-xr-x   0 jaskiratsingh   (501) staff       (20)        0 2023-07-17 01:44:17.093088 alphatools_jv-3.0.0/alphatools/
--rw-r--r--   0 jaskiratsingh   (501) staff       (20)        0 2023-07-13 23:58:33.000000 alphatools_jv-3.0.0/alphatools/__init__.py
--rw-r--r--   0 jaskiratsingh   (501) staff       (20)     7134 2023-07-17 01:01:41.000000 alphatools_jv-3.0.0/alphatools/backtesting_app.py
-drwxr-xr-x   0 jaskiratsingh   (501) staff       (20)        0 2023-07-17 01:44:17.097609 alphatools_jv-3.0.0/alphatools/utils/
--rw-r--r--   0 jaskiratsingh   (501) staff       (20)        0 2023-07-13 23:58:33.000000 alphatools_jv-3.0.0/alphatools/utils/__init__.py
--rw-r--r--   0 jaskiratsingh   (501) staff       (20)      335 2023-07-17 01:01:41.000000 alphatools_jv-3.0.0/alphatools/utils/alphatools_prompt.py
--rw-r--r--   0 jaskiratsingh   (501) staff       (20)     1376 2023-07-17 01:01:41.000000 alphatools_jv-3.0.0/alphatools/utils/cache.py
--rw-r--r--   0 jaskiratsingh   (501) staff       (20)     1170 2023-07-13 23:58:33.000000 alphatools_jv-3.0.0/alphatools/utils/instrument_pnl_calculator.py
--rw-r--r--   0 jaskiratsingh   (501) staff       (20)     3397 2023-07-17 01:01:41.000000 alphatools_jv-3.0.0/alphatools/utils/instruments.py
--rw-r--r--   0 jaskiratsingh   (501) staff       (20)     1012 2023-07-13 23:58:33.000000 alphatools_jv-3.0.0/alphatools/utils/pnl_calculator.py
--rw-r--r--   0 jaskiratsingh   (501) staff       (20)     2603 2023-07-17 01:01:41.000000 alphatools_jv-3.0.0/alphatools/utils/smartapi_helper.py
--rw-r--r--   0 jaskiratsingh   (501) staff       (20)     2969 2023-07-16 04:53:16.000000 alphatools_jv-3.0.0/alphatools/utils/token_manager.py
-drwxr-xr-x   0 jaskiratsingh   (501) staff       (20)        0 2023-07-17 01:44:17.193507 alphatools_jv-3.0.0/alphatools_jv.egg-info/
--rw-r--r--   0 jaskiratsingh   (501) staff       (20)     2055 2023-07-17 01:44:17.000000 alphatools_jv-3.0.0/alphatools_jv.egg-info/PKG-INFO
--rw-r--r--   0 jaskiratsingh   (501) staff       (20)      620 2023-07-17 01:44:17.000000 alphatools_jv-3.0.0/alphatools_jv.egg-info/SOURCES.txt
--rw-r--r--   0 jaskiratsingh   (501) staff       (20)        1 2023-07-17 01:44:17.000000 alphatools_jv-3.0.0/alphatools_jv.egg-info/dependency_links.txt
--rw-r--r--   0 jaskiratsingh   (501) staff       (20)      134 2023-07-17 01:44:17.000000 alphatools_jv-3.0.0/alphatools_jv.egg-info/requires.txt
--rw-r--r--   0 jaskiratsingh   (501) staff       (20)       16 2023-07-17 01:44:17.000000 alphatools_jv-3.0.0/alphatools_jv.egg-info/top_level.txt
--rw-r--r--   0 jaskiratsingh   (501) staff       (20)       91 2023-07-17 01:29:34.000000 alphatools_jv-3.0.0/pyproject.toml
--rw-r--r--   0 jaskiratsingh   (501) staff       (20)       38 2023-07-17 01:44:17.198595 alphatools_jv-3.0.0/setup.cfg
--rw-r--r--   0 jaskiratsingh   (501) staff       (20)      868 2023-07-17 01:18:54.000000 alphatools_jv-3.0.0/setup.py
-drwxr-xr-x   0 jaskiratsingh   (501) staff       (20)        0 2023-07-17 01:44:17.196955 alphatools_jv-3.0.0/test/
--rw-r--r--   0 jaskiratsingh   (501) staff       (20)        0 2023-07-13 23:58:33.000000 alphatools_jv-3.0.0/test/__init__.py
--rw-r--r--   0 jaskiratsingh   (501) staff       (20)     3009 2023-07-17 01:01:41.000000 alphatools_jv-3.0.0/test/test_backtesting_app.py
--rw-r--r--   0 jaskiratsingh   (501) staff       (20)        0 2023-07-17 01:01:41.000000 alphatools_jv-3.0.0/test/test_pnl_calculator.py
+drwxr-xr-x   0 jaskiratsingh   (501) staff       (20)        0 2023-07-17 03:04:10.581209 alphatools_jv-3.1.0/
+-rw-r--r--   0 jaskiratsingh   (501) staff       (20)     2055 2023-07-17 03:04:10.580933 alphatools_jv-3.1.0/PKG-INFO
+-rw-r--r--   0 jaskiratsingh   (501) staff       (20)     1651 2023-07-13 23:58:33.000000 alphatools_jv-3.1.0/README.md
+drwxr-xr-x   0 jaskiratsingh   (501) staff       (20)        0 2023-07-17 03:04:10.534805 alphatools_jv-3.1.0/alphatools/
+-rw-r--r--   0 jaskiratsingh   (501) staff       (20)        0 2023-07-13 23:58:33.000000 alphatools_jv-3.1.0/alphatools/__init__.py
+-rw-r--r--   0 jaskiratsingh   (501) staff       (20)     7134 2023-07-17 01:01:41.000000 alphatools_jv-3.1.0/alphatools/backtesting_app.py
+drwxr-xr-x   0 jaskiratsingh   (501) staff       (20)        0 2023-07-17 03:04:10.540596 alphatools_jv-3.1.0/alphatools/utils/
+-rw-r--r--   0 jaskiratsingh   (501) staff       (20)        0 2023-07-13 23:58:33.000000 alphatools_jv-3.1.0/alphatools/utils/__init__.py
+-rw-r--r--   0 jaskiratsingh   (501) staff       (20)      335 2023-07-17 01:01:41.000000 alphatools_jv-3.1.0/alphatools/utils/alphatools_prompt.py
+-rw-r--r--   0 jaskiratsingh   (501) staff       (20)     1376 2023-07-17 01:01:41.000000 alphatools_jv-3.1.0/alphatools/utils/cache.py
+-rw-r--r--   0 jaskiratsingh   (501) staff       (20)     1170 2023-07-13 23:58:33.000000 alphatools_jv-3.1.0/alphatools/utils/instrument_pnl_calculator.py
+-rw-r--r--   0 jaskiratsingh   (501) staff       (20)     3397 2023-07-17 01:01:41.000000 alphatools_jv-3.1.0/alphatools/utils/instruments.py
+-rw-r--r--   0 jaskiratsingh   (501) staff       (20)     1012 2023-07-13 23:58:33.000000 alphatools_jv-3.1.0/alphatools/utils/pnl_calculator.py
+-rw-r--r--   0 jaskiratsingh   (501) staff       (20)     2603 2023-07-17 01:01:41.000000 alphatools_jv-3.1.0/alphatools/utils/smartapi_helper.py
+-rw-r--r--   0 jaskiratsingh   (501) staff       (20)     2969 2023-07-16 04:53:16.000000 alphatools_jv-3.1.0/alphatools/utils/token_manager.py
+drwxr-xr-x   0 jaskiratsingh   (501) staff       (20)        0 2023-07-17 03:04:10.578492 alphatools_jv-3.1.0/alphatools_jv.egg-info/
+-rw-r--r--   0 jaskiratsingh   (501) staff       (20)     2055 2023-07-17 03:04:10.000000 alphatools_jv-3.1.0/alphatools_jv.egg-info/PKG-INFO
+-rw-r--r--   0 jaskiratsingh   (501) staff       (20)      620 2023-07-17 03:04:10.000000 alphatools_jv-3.1.0/alphatools_jv.egg-info/SOURCES.txt
+-rw-r--r--   0 jaskiratsingh   (501) staff       (20)        1 2023-07-17 03:04:10.000000 alphatools_jv-3.1.0/alphatools_jv.egg-info/dependency_links.txt
+-rw-r--r--   0 jaskiratsingh   (501) staff       (20)      134 2023-07-17 03:04:10.000000 alphatools_jv-3.1.0/alphatools_jv.egg-info/requires.txt
+-rw-r--r--   0 jaskiratsingh   (501) staff       (20)       16 2023-07-17 03:04:10.000000 alphatools_jv-3.1.0/alphatools_jv.egg-info/top_level.txt
+-rw-r--r--   0 jaskiratsingh   (501) staff       (20)       91 2023-07-17 01:29:34.000000 alphatools_jv-3.1.0/pyproject.toml
+-rw-r--r--   0 jaskiratsingh   (501) staff       (20)       38 2023-07-17 03:04:10.581263 alphatools_jv-3.1.0/setup.cfg
+-rw-r--r--   0 jaskiratsingh   (501) staff       (20)      867 2023-07-17 01:46:20.000000 alphatools_jv-3.1.0/setup.py
+drwxr-xr-x   0 jaskiratsingh   (501) staff       (20)        0 2023-07-17 03:04:10.580440 alphatools_jv-3.1.0/test/
+-rw-r--r--   0 jaskiratsingh   (501) staff       (20)        0 2023-07-13 23:58:33.000000 alphatools_jv-3.1.0/test/__init__.py
+-rw-r--r--   0 jaskiratsingh   (501) staff       (20)     3009 2023-07-17 01:01:41.000000 alphatools_jv-3.1.0/test/test_backtesting_app.py
+-rw-r--r--   0 jaskiratsingh   (501) staff       (20)        0 2023-07-17 01:01:41.000000 alphatools_jv-3.1.0/test/test_pnl_calculator.py
```

### Comparing `alphatools_jv-3.0.0/PKG-INFO` & `alphatools_jv-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphatools_jv
-Version: 3.0.0
+Version: 3.1.0
 Summary: Wrapper over angel broking smartapi to read cached options market data
 Home-page: https://github.com/jaskirat1208/backtest-platform
 Author: Jaskirat Singh
 Author-email: jaskiratsingh1208@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `alphatools_jv-3.0.0/README.md` & `alphatools_jv-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `alphatools_jv-3.0.0/alphatools/backtesting_app.py` & `alphatools_jv-3.1.0/alphatools/backtesting_app.py`

 * *Files identical despite different names*

### Comparing `alphatools_jv-3.0.0/alphatools/utils/cache.py` & `alphatools_jv-3.1.0/alphatools/utils/cache.py`

 * *Files identical despite different names*

### Comparing `alphatools_jv-3.0.0/alphatools/utils/instrument_pnl_calculator.py` & `alphatools_jv-3.1.0/alphatools/utils/instrument_pnl_calculator.py`

 * *Files identical despite different names*

### Comparing `alphatools_jv-3.0.0/alphatools/utils/instruments.py` & `alphatools_jv-3.1.0/alphatools/utils/instruments.py`

 * *Files identical despite different names*

### Comparing `alphatools_jv-3.0.0/alphatools/utils/pnl_calculator.py` & `alphatools_jv-3.1.0/alphatools/utils/pnl_calculator.py`

 * *Files identical despite different names*

### Comparing `alphatools_jv-3.0.0/alphatools/utils/smartapi_helper.py` & `alphatools_jv-3.1.0/alphatools/utils/smartapi_helper.py`

 * *Files identical despite different names*

### Comparing `alphatools_jv-3.0.0/alphatools/utils/token_manager.py` & `alphatools_jv-3.1.0/alphatools/utils/token_manager.py`

 * *Files identical despite different names*

### Comparing `alphatools_jv-3.0.0/alphatools_jv.egg-info/PKG-INFO` & `alphatools_jv-3.1.0/alphatools_jv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphatools-jv
-Version: 3.0.0
+Version: 3.1.0
 Summary: Wrapper over angel broking smartapi to read cached options market data
 Home-page: https://github.com/jaskirat1208/backtest-platform
 Author: Jaskirat Singh
 Author-email: jaskiratsingh1208@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `alphatools_jv-3.0.0/alphatools_jv.egg-info/SOURCES.txt` & `alphatools_jv-3.1.0/alphatools_jv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alphatools_jv-3.0.0/setup.py` & `alphatools_jv-3.1.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open("requirements.txt", "r") as fh:
     install_requires = fh.read()
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-__version__ = "v3.0.0"
+__version__ = "3.1.0"
 
 setuptools.setup(
     name="alphatools_jv",
     version=__version__,
     author="Jaskirat Singh",
     author_email="jaskiratsingh1208@gmail.com",
     description="Wrapper over angel broking smartapi to read cached options market data",
```

### Comparing `alphatools_jv-3.0.0/test/test_backtesting_app.py` & `alphatools_jv-3.1.0/test/test_backtesting_app.py`

 * *Files identical despite different names*

