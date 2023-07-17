# Comparing `tmp/pegasusX-0.1.3.tar.gz` & `tmp/pegasusX-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pegasusX-0.1.3.tar", last modified: Mon Jul 17 03:53:01 2023, max compression
+gzip compressed data, was "pegasusX-0.1.4.tar", last modified: Mon Jul 17 04:08:06 2023, max compression
```

## Comparing `pegasusX-0.1.3.tar` & `pegasusX-0.1.4.tar`

### file list

```diff
@@ -1,46 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:53:01.564407 pegasusX-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 03:52:48.000000 pegasusX-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 03:53:01.564407 pegasusX-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-07-17 03:52:48.000000 pegasusX-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:53:01.560407 pegasusX-0.1.3/pegasus/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:53:01.560407 pegasusX-0.1.3/pegasus/Ocean/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-17 03:52:48.000000 pegasusX-0.1.3/pegasus/Ocean/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:53:01.560407 pegasusX-0.1.3/pegasus/Ocean/oceandb/
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-07-17 03:52:48.000000 pegasusX-0.1.3/pegasus/Ocean/oceandb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:53:01.560407 pegasusX-0.1.3/pegasus/Ocean/oceandb/api/
--rw-r--r--   0 runner    (1001) docker     (123)    10235 2023-07-17 03:52:48.000000 pegasusX-0.1.3/pegasus/Ocean/oceandb/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11533 2023-07-17 03:52:48.000000 pegasusX-0.1.3/pegasus/Ocean/oceandb/api/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)    16334 2023-07-17 03:52:48.000000 pegasusX-0.1.3/pegasus/Ocean/oceandb/api/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    12827 2023-07-17 03:52:48.000000 pegasusX-0.1.3/pegasus/Ocean/oceandb/api/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-17 03:52:48.000000 pegasusX-0.1.3/pegasus/Ocean/oceandb/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-17 03:52:48.000000 pegasusX-0.1.3/pegasus/Ocean/oceandb/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:53:01.564407 pegasusX-0.1.3/pegasus/Ocean/oceandb/db/
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-07-17 03:52:48.000000 pegasusX-0.1.3/pegasus/Ocean/oceandb/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21244 2023-07-17 03:52:48.000000 pegasusX-0.1.3/pegasus/Ocean/oceandb/db/clickhouse.py
--rw-r--r--   0 runner    (1001) docker     (123)    17598 2023-07-17 03:52:48.000000 pegasusX-0.1.3/pegasus/Ocean/oceandb/db/duckdb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:53:01.564407 pegasusX-0.1.3/pegasus/Ocean/oceandb/db/index/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-17 03:52:48.000000 pegasusX-0.1.3/pegasus/Ocean/oceandb/db/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9126 2023-07-17 03:52:48.000000 pegasusX-0.1.3/pegasus/Ocean/oceandb/db/index/hnswlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-17 03:52:48.000000 pegasusX-0.1.3/pegasus/Ocean/oceandb/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:53:01.564407 pegasusX-0.1.3/pegasus/Ocean/oceandb/server/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-17 03:52:48.000000 pegasusX-0.1.3/pegasus/Ocean/oceandb/server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:53:01.564407 pegasusX-0.1.3/pegasus/Ocean/oceandb/server/fastapi/
--rw-r--r--   0 runner    (1001) docker     (123)     8456 2023-07-17 03:52:48.000000 pegasusX-0.1.3/pegasus/Ocean/oceandb/server/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-07-17 03:52:48.000000 pegasusX-0.1.3/pegasus/Ocean/oceandb/server/fastapi/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:53:01.564407 pegasusX-0.1.3/pegasus/Ocean/oceandb/telemetry/
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-17 03:52:48.000000 pegasusX-0.1.3/pegasus/Ocean/oceandb/telemetry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-17 03:52:48.000000 pegasusX-0.1.3/pegasus/Ocean/oceandb/telemetry/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-17 03:52:48.000000 pegasusX-0.1.3/pegasus/Ocean/oceandb/telemetry/posthog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:53:01.564407 pegasusX-0.1.3/pegasus/Ocean/oceandb/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 03:52:48.000000 pegasusX-0.1.3/pegasus/Ocean/oceandb/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8028 2023-07-17 03:52:48.000000 pegasusX-0.1.3/pegasus/Ocean/oceandb/utils/embedding_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-17 03:52:48.000000 pegasusX-0.1.3/pegasus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-17 03:52:48.000000 pegasusX-0.1.3/pegasus/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:53:01.564407 pegasusX-0.1.3/pegasusX.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 03:53:01.000000 pegasusX-0.1.3/pegasusX.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-17 03:53:01.000000 pegasusX-0.1.3/pegasusX.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 03:53:01.000000 pegasusX-0.1.3/pegasusX.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-17 03:53:01.000000 pegasusX-0.1.3/pegasusX.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 03:53:01.000000 pegasusX-0.1.3/pegasusX.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 03:53:01.564407 pegasusX-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-17 03:52:48.000000 pegasusX-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:08:06.035761 pegasusX-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 04:07:49.000000 pegasusX-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 04:08:06.035761 pegasusX-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-07-17 04:07:49.000000 pegasusX-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:08:06.031761 pegasusX-0.1.4/pegasus/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-17 04:07:49.000000 pegasusX-0.1.4/pegasus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-17 04:07:49.000000 pegasusX-0.1.4/pegasus/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:08:06.031761 pegasusX-0.1.4/pegasus/oceandb/
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-07-17 04:07:49.000000 pegasusX-0.1.4/pegasus/oceandb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:08:06.035761 pegasusX-0.1.4/pegasus/oceandb/api/
+-rw-r--r--   0 runner    (1001) docker     (123)    10235 2023-07-17 04:07:49.000000 pegasusX-0.1.4/pegasus/oceandb/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11533 2023-07-17 04:07:49.000000 pegasusX-0.1.4/pegasus/oceandb/api/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16334 2023-07-17 04:07:49.000000 pegasusX-0.1.4/pegasus/oceandb/api/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12827 2023-07-17 04:07:49.000000 pegasusX-0.1.4/pegasus/oceandb/api/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-17 04:07:49.000000 pegasusX-0.1.4/pegasus/oceandb/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-17 04:07:49.000000 pegasusX-0.1.4/pegasus/oceandb/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:08:06.035761 pegasusX-0.1.4/pegasus/oceandb/db/
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-07-17 04:07:49.000000 pegasusX-0.1.4/pegasus/oceandb/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21244 2023-07-17 04:07:49.000000 pegasusX-0.1.4/pegasus/oceandb/db/clickhouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17598 2023-07-17 04:07:49.000000 pegasusX-0.1.4/pegasus/oceandb/db/duckdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:08:06.035761 pegasusX-0.1.4/pegasus/oceandb/db/index/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-17 04:07:49.000000 pegasusX-0.1.4/pegasus/oceandb/db/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9126 2023-07-17 04:07:49.000000 pegasusX-0.1.4/pegasus/oceandb/db/index/hnswlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-17 04:07:49.000000 pegasusX-0.1.4/pegasus/oceandb/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:08:06.035761 pegasusX-0.1.4/pegasus/oceandb/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-17 04:07:49.000000 pegasusX-0.1.4/pegasus/oceandb/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:08:06.035761 pegasusX-0.1.4/pegasus/oceandb/server/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)     8456 2023-07-17 04:07:49.000000 pegasusX-0.1.4/pegasus/oceandb/server/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-07-17 04:07:49.000000 pegasusX-0.1.4/pegasus/oceandb/server/fastapi/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:08:06.035761 pegasusX-0.1.4/pegasus/oceandb/telemetry/
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-17 04:07:49.000000 pegasusX-0.1.4/pegasus/oceandb/telemetry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-17 04:07:49.000000 pegasusX-0.1.4/pegasus/oceandb/telemetry/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-17 04:07:49.000000 pegasusX-0.1.4/pegasus/oceandb/telemetry/posthog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:08:06.035761 pegasusX-0.1.4/pegasus/oceandb/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 04:07:49.000000 pegasusX-0.1.4/pegasus/oceandb/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8028 2023-07-17 04:07:49.000000 pegasusX-0.1.4/pegasus/oceandb/utils/embedding_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:08:06.035761 pegasusX-0.1.4/pegasusX.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 04:08:06.000000 pegasusX-0.1.4/pegasusX.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-17 04:08:06.000000 pegasusX-0.1.4/pegasusX.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 04:08:06.000000 pegasusX-0.1.4/pegasusX.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-17 04:08:06.000000 pegasusX-0.1.4/pegasusX.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 04:08:06.000000 pegasusX-0.1.4/pegasusX.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 04:08:06.035761 pegasusX-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-17 04:07:49.000000 pegasusX-0.1.4/setup.py
```

### Comparing `pegasusX-0.1.3/LICENSE` & `pegasusX-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pegasusX-0.1.3/PKG-INFO` & `pegasusX-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pegasusX
-Version: 0.1.3
+Version: 0.1.4
 Summary: pegasus - Pytorch
 Home-page: https://github.com/kyegomez/pegasus
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pegasusX-0.1.3/README.md` & `pegasusX-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pegasusX-0.1.3/pegasus/Ocean/oceandb/__init__.py` & `pegasusX-0.1.4/pegasus/oceandb/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import oceandb.config
 import logging
 from oceandb.telemetry.events import ClientStartEvent
 from oceandb.telemetry.posthog import Posthog
 
+from oceandb.utils.embedding_functions import ImageBindEmbeddingFunction
+
 logger = logging.getLogger(__name__)
 
 __settings = oceandb.config.Settings()
 
 __version__ = "0.3.22"
```

### Comparing `pegasusX-0.1.3/pegasus/Ocean/oceandb/api/__init__.py` & `pegasusX-0.1.4/pegasus/oceandb/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.1.3/pegasus/Ocean/oceandb/api/fastapi.py` & `pegasusX-0.1.4/pegasus/oceandb/api/fastapi.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.1.3/pegasus/Ocean/oceandb/api/local.py` & `pegasusX-0.1.4/pegasus/oceandb/api/local.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.1.3/pegasus/Ocean/oceandb/api/types.py` & `pegasusX-0.1.4/pegasus/oceandb/api/types.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.1.3/pegasus/Ocean/oceandb/config.py` & `pegasusX-0.1.4/pegasus/oceandb/config.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.1.3/pegasus/Ocean/oceandb/db/__init__.py` & `pegasusX-0.1.4/pegasus/oceandb/db/__init__.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.1.3/pegasus/Ocean/oceandb/db/clickhouse.py` & `pegasusX-0.1.4/pegasus/oceandb/db/clickhouse.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.1.3/pegasus/Ocean/oceandb/db/duckdb.py` & `pegasusX-0.1.4/pegasus/oceandb/db/duckdb.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.1.3/pegasus/Ocean/oceandb/db/index/hnswlib.py` & `pegasusX-0.1.4/pegasus/oceandb/db/index/hnswlib.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.1.3/pegasus/Ocean/oceandb/errors.py` & `pegasusX-0.1.4/pegasus/oceandb/errors.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.1.3/pegasus/Ocean/oceandb/server/fastapi/__init__.py` & `pegasusX-0.1.4/pegasus/oceandb/server/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.1.3/pegasus/Ocean/oceandb/server/fastapi/types.py` & `pegasusX-0.1.4/pegasus/oceandb/server/fastapi/types.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.1.3/pegasus/Ocean/oceandb/telemetry/__init__.py` & `pegasusX-0.1.4/pegasus/oceandb/telemetry/__init__.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.1.3/pegasus/Ocean/oceandb/telemetry/events.py` & `pegasusX-0.1.4/pegasus/oceandb/telemetry/events.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.1.3/pegasus/Ocean/oceandb/telemetry/posthog.py` & `pegasusX-0.1.4/pegasus/oceandb/telemetry/posthog.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.1.3/pegasus/Ocean/oceandb/utils/embedding_functions.py` & `pegasusX-0.1.4/pegasus/oceandb/utils/embedding_functions.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.1.3/pegasus/main.py` & `pegasusX-0.1.4/pegasus/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from concurrent.futures import ProcessPoolExecutor, as_completed
 from numba import njit
 from joblib import Memory
 import numpy as np
 
-from pegasus.Ocean import ImageBindEmbeddingFunction
+# from pegasus.Ocean import ImageBindEmbeddingFunctio
+from pegasus.oceandb import ImageBindEmbeddingFunction
 
 memory = Memory("PegasusStore", verbose=0)
 
 @memory.cache
 @njit
 def optimized_embedding_function(modality, data):
     return ImageBindEmbeddingFunction(modality)(data)
```

### Comparing `pegasusX-0.1.3/pegasusX.egg-info/PKG-INFO` & `pegasusX-0.1.4/pegasusX.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pegasusX
-Version: 0.1.3
+Version: 0.1.4
 Summary: pegasus - Pytorch
 Home-page: https://github.com/kyegomez/pegasus
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pegasusX-0.1.3/setup.py` & `pegasusX-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 # 
 
 setup(
   name = 'pegasusX',
   packages = find_packages(exclude=[]),
-  version = '0.1.3',
+  version = '0.1.4',
   license='MIT',
   description = 'pegasus - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/pegasus',
   keywords = [
```

