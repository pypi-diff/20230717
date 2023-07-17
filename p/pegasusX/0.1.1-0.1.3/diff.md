# Comparing `tmp/pegasusX-0.1.1.tar.gz` & `tmp/pegasusX-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pegasusX-0.1.1.tar", last modified: Mon Jul 17 03:46:16 2023, max compression
+gzip compressed data, was "pegasusX-0.1.3.tar", last modified: Mon Jul 17 03:53:01 2023, max compression
```

## Comparing `pegasusX-0.1.1.tar` & `pegasusX-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:46:16.546973 pegasusX-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 03:46:03.000000 pegasusX-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 03:46:16.546973 pegasusX-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-07-17 03:46:03.000000 pegasusX-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:46:16.546973 pegasusX-0.1.1/pegasus/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-17 03:46:03.000000 pegasusX-0.1.1/pegasus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-17 03:46:03.000000 pegasusX-0.1.1/pegasus/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:46:16.546973 pegasusX-0.1.1/pegasusX.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 03:46:16.000000 pegasusX-0.1.1/pegasusX.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-17 03:46:16.000000 pegasusX-0.1.1/pegasusX.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 03:46:16.000000 pegasusX-0.1.1/pegasusX.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-17 03:46:16.000000 pegasusX-0.1.1/pegasusX.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 03:46:16.000000 pegasusX-0.1.1/pegasusX.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 03:46:16.546973 pegasusX-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-17 03:46:03.000000 pegasusX-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:53:01.564407 pegasusX-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 03:52:48.000000 pegasusX-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 03:53:01.564407 pegasusX-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-07-17 03:52:48.000000 pegasusX-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:53:01.560407 pegasusX-0.1.3/pegasus/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:53:01.560407 pegasusX-0.1.3/pegasus/Ocean/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-17 03:52:48.000000 pegasusX-0.1.3/pegasus/Ocean/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:53:01.560407 pegasusX-0.1.3/pegasus/Ocean/oceandb/
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-07-17 03:52:48.000000 pegasusX-0.1.3/pegasus/Ocean/oceandb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:53:01.560407 pegasusX-0.1.3/pegasus/Ocean/oceandb/api/
+-rw-r--r--   0 runner    (1001) docker     (123)    10235 2023-07-17 03:52:48.000000 pegasusX-0.1.3/pegasus/Ocean/oceandb/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11533 2023-07-17 03:52:48.000000 pegasusX-0.1.3/pegasus/Ocean/oceandb/api/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16334 2023-07-17 03:52:48.000000 pegasusX-0.1.3/pegasus/Ocean/oceandb/api/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12827 2023-07-17 03:52:48.000000 pegasusX-0.1.3/pegasus/Ocean/oceandb/api/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-17 03:52:48.000000 pegasusX-0.1.3/pegasus/Ocean/oceandb/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-17 03:52:48.000000 pegasusX-0.1.3/pegasus/Ocean/oceandb/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:53:01.564407 pegasusX-0.1.3/pegasus/Ocean/oceandb/db/
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-07-17 03:52:48.000000 pegasusX-0.1.3/pegasus/Ocean/oceandb/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21244 2023-07-17 03:52:48.000000 pegasusX-0.1.3/pegasus/Ocean/oceandb/db/clickhouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17598 2023-07-17 03:52:48.000000 pegasusX-0.1.3/pegasus/Ocean/oceandb/db/duckdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:53:01.564407 pegasusX-0.1.3/pegasus/Ocean/oceandb/db/index/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-17 03:52:48.000000 pegasusX-0.1.3/pegasus/Ocean/oceandb/db/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9126 2023-07-17 03:52:48.000000 pegasusX-0.1.3/pegasus/Ocean/oceandb/db/index/hnswlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-17 03:52:48.000000 pegasusX-0.1.3/pegasus/Ocean/oceandb/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:53:01.564407 pegasusX-0.1.3/pegasus/Ocean/oceandb/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-17 03:52:48.000000 pegasusX-0.1.3/pegasus/Ocean/oceandb/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:53:01.564407 pegasusX-0.1.3/pegasus/Ocean/oceandb/server/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)     8456 2023-07-17 03:52:48.000000 pegasusX-0.1.3/pegasus/Ocean/oceandb/server/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-07-17 03:52:48.000000 pegasusX-0.1.3/pegasus/Ocean/oceandb/server/fastapi/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:53:01.564407 pegasusX-0.1.3/pegasus/Ocean/oceandb/telemetry/
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-17 03:52:48.000000 pegasusX-0.1.3/pegasus/Ocean/oceandb/telemetry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-17 03:52:48.000000 pegasusX-0.1.3/pegasus/Ocean/oceandb/telemetry/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-17 03:52:48.000000 pegasusX-0.1.3/pegasus/Ocean/oceandb/telemetry/posthog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:53:01.564407 pegasusX-0.1.3/pegasus/Ocean/oceandb/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 03:52:48.000000 pegasusX-0.1.3/pegasus/Ocean/oceandb/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8028 2023-07-17 03:52:48.000000 pegasusX-0.1.3/pegasus/Ocean/oceandb/utils/embedding_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-17 03:52:48.000000 pegasusX-0.1.3/pegasus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-17 03:52:48.000000 pegasusX-0.1.3/pegasus/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:53:01.564407 pegasusX-0.1.3/pegasusX.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 03:53:01.000000 pegasusX-0.1.3/pegasusX.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-17 03:53:01.000000 pegasusX-0.1.3/pegasusX.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 03:53:01.000000 pegasusX-0.1.3/pegasusX.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-17 03:53:01.000000 pegasusX-0.1.3/pegasusX.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 03:53:01.000000 pegasusX-0.1.3/pegasusX.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 03:53:01.564407 pegasusX-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-17 03:52:48.000000 pegasusX-0.1.3/setup.py
```

### Comparing `pegasusX-0.1.1/LICENSE` & `pegasusX-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pegasusX-0.1.1/PKG-INFO` & `pegasusX-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pegasusX
-Version: 0.1.1
+Version: 0.1.3
 Summary: pegasus - Pytorch
 Home-page: https://github.com/kyegomez/pegasus
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pegasusX-0.1.1/README.md` & `pegasusX-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pegasusX-0.1.1/pegasus/main.py` & `pegasusX-0.1.3/pegasus/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from concurrent.futures import ProcessPoolExecutor, as_completed
 from numba import njit
 from joblib import Memory
 import numpy as np
 
-from oceandb.utils.embedding_functions import ImageBindEmbeddingFunction
-
+from pegasus.Ocean import ImageBindEmbeddingFunction
 
 memory = Memory("PegasusStore", verbose=0)
 
 @memory.cache
 @njit
 def optimized_embedding_function(modality, data):
     return ImageBindEmbeddingFunction(modality)(data)
```

### Comparing `pegasusX-0.1.1/pegasusX.egg-info/PKG-INFO` & `pegasusX-0.1.3/pegasusX.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pegasusX
-Version: 0.1.1
+Version: 0.1.3
 Summary: pegasus - Pytorch
 Home-page: https://github.com/kyegomez/pegasus
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pegasusX-0.1.1/setup.py` & `pegasusX-0.1.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 from setuptools import setup, find_packages
 # 
 
 setup(
   name = 'pegasusX',
   packages = find_packages(exclude=[]),
-  version = '0.1.1',
+  version = '0.1.3',
   license='MIT',
   description = 'pegasus - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/pegasus',
   keywords = [
     'artificial intelligence',
     'deep learning',
     'optimizers',
     "Prompt Engineering"
   ],
     install_requires=[
-        'oceandb',
         'numba',
         'joblib',
     ],
   classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'Topic :: Scientific/Engineering :: Artificial Intelligence',
```

