# Comparing `tmp/fastapi-serve-0.0.3.dev5.tar.gz` & `tmp/fastapi-serve-0.0.3.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-serve-0.0.3.dev5.tar", last modified: Mon Jul 17 17:13:14 2023, max compression
+gzip compressed data, was "fastapi-serve-0.0.3.dev6.tar", last modified: Mon Jul 17 17:17:04 2023, max compression
```

## Comparing `fastapi-serve-0.0.3.dev5.tar` & `fastapi-serve-0.0.3.dev6.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:13:14.664826 fastapi-serve-0.0.3.dev5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 17:13:08.000000 fastapi-serve-0.0.3.dev5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-17 17:13:08.000000 fastapi-serve-0.0.3.dev5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-07-17 17:13:14.664826 fastapi-serve-0.0.3.dev5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-07-17 17:13:08.000000 fastapi-serve-0.0.3.dev5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:13:14.656826 fastapi-serve-0.0.3.dev5/fastapi_serve/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-17 17:13:14.000000 fastapi-serve-0.0.3.dev5/fastapi_serve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-17 17:13:08.000000 fastapi-serve-0.0.3.dev5/fastapi_serve/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:13:14.660826 fastapi-serve-0.0.3.dev5/fastapi_serve/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-17 17:13:08.000000 fastapi-serve-0.0.3.dev5/fastapi_serve/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-07-17 17:13:08.000000 fastapi-serve-0.0.3.dev5/fastapi_serve/cloud/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     8001 2023-07-17 17:13:08.000000 fastapi-serve-0.0.3.dev5/fastapi_serve/cloud/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-07-17 17:13:08.000000 fastapi-serve-0.0.3.dev5/fastapi_serve/cloud/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-17 17:13:08.000000 fastapi-serve-0.0.3.dev5/fastapi_serve/cloud/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-17 17:13:08.000000 fastapi-serve-0.0.3.dev5/fastapi_serve/cloud/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-07-17 17:13:08.000000 fastapi-serve-0.0.3.dev5/fastapi_serve/cloud/options.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-17 17:13:08.000000 fastapi-serve-0.0.3.dev5/fastapi_serve/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:13:14.660826 fastapi-serve-0.0.3.dev5/fastapi_serve/gateway/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-17 17:13:08.000000 fastapi-serve-0.0.3.dev5/fastapi_serve/gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-07-17 17:13:08.000000 fastapi-serve-0.0.3.dev5/fastapi_serve/gateway/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-07-17 17:13:08.000000 fastapi-serve-0.0.3.dev5/fastapi_serve/gateway/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-07-17 17:13:08.000000 fastapi-serve-0.0.3.dev5/fastapi_serve/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:13:14.660826 fastapi-serve-0.0.3.dev5/fastapi_serve/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-17 17:13:08.000000 fastapi-serve-0.0.3.dev5/fastapi_serve/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-17 17:13:08.000000 fastapi-serve-0.0.3.dev5/fastapi_serve/utils/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:13:14.664826 fastapi-serve-0.0.3.dev5/fastapi_serve/utils/blob/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-17 17:13:08.000000 fastapi-serve-0.0.3.dev5/fastapi_serve/utils/blob/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-07-17 17:13:08.000000 fastapi-serve-0.0.3.dev5/fastapi_serve/utils/blob/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-17 17:13:08.000000 fastapi-serve-0.0.3.dev5/fastapi_serve/utils/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:13:14.660826 fastapi-serve-0.0.3.dev5/fastapi_serve.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-07-17 17:13:14.000000 fastapi-serve-0.0.3.dev5/fastapi_serve.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-17 17:13:14.000000 fastapi-serve-0.0.3.dev5/fastapi_serve.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 17:13:14.000000 fastapi-serve-0.0.3.dev5/fastapi_serve.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-17 17:13:14.000000 fastapi-serve-0.0.3.dev5/fastapi_serve.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 17:13:14.000000 fastapi-serve-0.0.3.dev5/fastapi_serve.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-17 17:13:14.000000 fastapi-serve-0.0.3.dev5/fastapi_serve.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-17 17:13:14.000000 fastapi-serve-0.0.3.dev5/fastapi_serve.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-17 17:13:08.000000 fastapi-serve-0.0.3.dev5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 17:13:14.664826 fastapi-serve-0.0.3.dev5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-17 17:13:08.000000 fastapi-serve-0.0.3.dev5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:17:04.678874 fastapi-serve-0.0.3.dev6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 17:16:59.000000 fastapi-serve-0.0.3.dev6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-17 17:16:59.000000 fastapi-serve-0.0.3.dev6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-07-17 17:17:04.678874 fastapi-serve-0.0.3.dev6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-07-17 17:16:59.000000 fastapi-serve-0.0.3.dev6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:17:04.678874 fastapi-serve-0.0.3.dev6/fastapi_serve/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-17 17:17:04.000000 fastapi-serve-0.0.3.dev6/fastapi_serve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-17 17:16:59.000000 fastapi-serve-0.0.3.dev6/fastapi_serve/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:17:04.678874 fastapi-serve-0.0.3.dev6/fastapi_serve/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-17 17:16:59.000000 fastapi-serve-0.0.3.dev6/fastapi_serve/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-07-17 17:16:59.000000 fastapi-serve-0.0.3.dev6/fastapi_serve/cloud/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8001 2023-07-17 17:16:59.000000 fastapi-serve-0.0.3.dev6/fastapi_serve/cloud/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-07-17 17:16:59.000000 fastapi-serve-0.0.3.dev6/fastapi_serve/cloud/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-17 17:16:59.000000 fastapi-serve-0.0.3.dev6/fastapi_serve/cloud/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-17 17:16:59.000000 fastapi-serve-0.0.3.dev6/fastapi_serve/cloud/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-07-17 17:16:59.000000 fastapi-serve-0.0.3.dev6/fastapi_serve/cloud/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-17 17:16:59.000000 fastapi-serve-0.0.3.dev6/fastapi_serve/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:17:04.678874 fastapi-serve-0.0.3.dev6/fastapi_serve/gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-17 17:16:59.000000 fastapi-serve-0.0.3.dev6/fastapi_serve/gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-07-17 17:16:59.000000 fastapi-serve-0.0.3.dev6/fastapi_serve/gateway/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-07-17 17:16:59.000000 fastapi-serve-0.0.3.dev6/fastapi_serve/gateway/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-07-17 17:16:59.000000 fastapi-serve-0.0.3.dev6/fastapi_serve/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:17:04.678874 fastapi-serve-0.0.3.dev6/fastapi_serve/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-17 17:16:59.000000 fastapi-serve-0.0.3.dev6/fastapi_serve/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-17 17:16:59.000000 fastapi-serve-0.0.3.dev6/fastapi_serve/utils/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:17:04.678874 fastapi-serve-0.0.3.dev6/fastapi_serve/utils/blob/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-17 17:16:59.000000 fastapi-serve-0.0.3.dev6/fastapi_serve/utils/blob/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-07-17 17:16:59.000000 fastapi-serve-0.0.3.dev6/fastapi_serve/utils/blob/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-17 17:16:59.000000 fastapi-serve-0.0.3.dev6/fastapi_serve/utils/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:17:04.678874 fastapi-serve-0.0.3.dev6/fastapi_serve.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-07-17 17:17:04.000000 fastapi-serve-0.0.3.dev6/fastapi_serve.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-17 17:17:04.000000 fastapi-serve-0.0.3.dev6/fastapi_serve.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 17:17:04.000000 fastapi-serve-0.0.3.dev6/fastapi_serve.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-17 17:17:04.000000 fastapi-serve-0.0.3.dev6/fastapi_serve.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 17:17:04.000000 fastapi-serve-0.0.3.dev6/fastapi_serve.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-17 17:17:04.000000 fastapi-serve-0.0.3.dev6/fastapi_serve.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-17 17:17:04.000000 fastapi-serve-0.0.3.dev6/fastapi_serve.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-17 17:16:59.000000 fastapi-serve-0.0.3.dev6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 17:17:04.678874 fastapi-serve-0.0.3.dev6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-17 17:16:59.000000 fastapi-serve-0.0.3.dev6/setup.py
```

### Comparing `fastapi-serve-0.0.3.dev5/LICENSE` & `fastapi-serve-0.0.3.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.3.dev5/PKG-INFO` & `fastapi-serve-0.0.3.dev6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-serve
-Version: 0.0.3.dev5
+Version: 0.0.3.dev6
 Summary: FastAPI Serve - FastAPI to the Cloud, Batteries Included!
 Home-page: https://github.com/jina-ai/fastapi-serve/
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/fastapi-serve/tags
 Project-URL: Documentation, https://docs.jina.ai
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi-serve Version: 0.0.3.dev5 Summary: FastAPI
+Metadata-Version: 2.1 Name: fastapi-serve Version: 0.0.3.dev6 Summary: FastAPI
 Serve - FastAPI to the Cloud, Batteries Included! Home-page: https://
 github.com/jina-ai/fastapi-serve/ Author: Jina AI Author-email: hello@jina.ai
 License: Apache 2.0 Download-URL: https://github.com/jina-ai/fastapi-serve/tags
 Project-URL: Documentation, https://docs.jina.ai Project-URL: Source, https://
 github.com/jina-ai/fastapi-serve/ Project-URL: Tracker, https://github.com/
 jina-ai/fastapi-serve/issues Keywords: jina fastapi restapi cloud docker
 kubernetes Platform: UNKNOWN Classifier: Development Status :: 5 - Production/
```

### Comparing `fastapi-serve-0.0.3.dev5/README.md` & `fastapi-serve-0.0.3.dev6/README.md`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.3.dev5/fastapi_serve/__main__.py` & `fastapi-serve-0.0.3.dev6/fastapi_serve/__main__.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.3.dev5/fastapi_serve/cloud/build.py` & `fastapi-serve-0.0.3.dev6/fastapi_serve/cloud/build.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.3.dev5/fastapi_serve/cloud/config.py` & `fastapi-serve-0.0.3.dev6/fastapi_serve/cloud/config.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.3.dev5/fastapi_serve/cloud/deploy.py` & `fastapi-serve-0.0.3.dev6/fastapi_serve/cloud/deploy.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.3.dev5/fastapi_serve/cloud/errors.py` & `fastapi-serve-0.0.3.dev6/fastapi_serve/cloud/errors.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.3.dev5/fastapi_serve/cloud/helper.py` & `fastapi-serve-0.0.3.dev6/fastapi_serve/cloud/helper.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.3.dev5/fastapi_serve/cloud/options.py` & `fastapi-serve-0.0.3.dev6/fastapi_serve/cloud/options.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.3.dev5/fastapi_serve/gateway/gateway.py` & `fastapi-serve-0.0.3.dev6/fastapi_serve/gateway/gateway.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.3.dev5/fastapi_serve/gateway/helper.py` & `fastapi-serve-0.0.3.dev6/fastapi_serve/gateway/helper.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.3.dev5/fastapi_serve/helper.py` & `fastapi-serve-0.0.3.dev6/fastapi_serve/helper.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.3.dev5/fastapi_serve/utils/auth.py` & `fastapi-serve-0.0.3.dev6/fastapi_serve/utils/auth.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.3.dev5/fastapi_serve/utils/blob/storage.py` & `fastapi-serve-0.0.3.dev6/fastapi_serve/utils/blob/storage.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.3.dev5/fastapi_serve/utils/helper.py` & `fastapi-serve-0.0.3.dev6/fastapi_serve/utils/helper.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.3.dev5/fastapi_serve.egg-info/PKG-INFO` & `fastapi-serve-0.0.3.dev6/fastapi_serve.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-serve
-Version: 0.0.3.dev5
+Version: 0.0.3.dev6
 Summary: FastAPI Serve - FastAPI to the Cloud, Batteries Included!
 Home-page: https://github.com/jina-ai/fastapi-serve/
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/fastapi-serve/tags
 Project-URL: Documentation, https://docs.jina.ai
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi-serve Version: 0.0.3.dev5 Summary: FastAPI
+Metadata-Version: 2.1 Name: fastapi-serve Version: 0.0.3.dev6 Summary: FastAPI
 Serve - FastAPI to the Cloud, Batteries Included! Home-page: https://
 github.com/jina-ai/fastapi-serve/ Author: Jina AI Author-email: hello@jina.ai
 License: Apache 2.0 Download-URL: https://github.com/jina-ai/fastapi-serve/tags
 Project-URL: Documentation, https://docs.jina.ai Project-URL: Source, https://
 github.com/jina-ai/fastapi-serve/ Project-URL: Tracker, https://github.com/
 jina-ai/fastapi-serve/issues Keywords: jina fastapi restapi cloud docker
 kubernetes Platform: UNKNOWN Classifier: Development Status :: 5 - Production/
```

### Comparing `fastapi-serve-0.0.3.dev5/fastapi_serve.egg-info/SOURCES.txt` & `fastapi-serve-0.0.3.dev6/fastapi_serve.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.3.dev5/setup.py` & `fastapi-serve-0.0.3.dev6/setup.py`

 * *Files identical despite different names*

