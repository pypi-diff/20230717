# Comparing `tmp/pegasusX-0.1.5.tar.gz` & `tmp/pegasusX-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pegasusX-0.1.5.tar", last modified: Mon Jul 17 04:12:03 2023, max compression
+gzip compressed data, was "pegasusX-0.1.6.tar", last modified: Mon Jul 17 04:15:31 2023, max compression
```

## Comparing `pegasusX-0.1.5.tar` & `pegasusX-0.1.6.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:12:03.117573 pegasusX-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 04:11:52.000000 pegasusX-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 04:12:03.117573 pegasusX-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-07-17 04:11:52.000000 pegasusX-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:12:03.117573 pegasusX-0.1.5/pegasus/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-17 04:11:52.000000 pegasusX-0.1.5/pegasus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-17 04:11:52.000000 pegasusX-0.1.5/pegasus/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:12:03.117573 pegasusX-0.1.5/pegasus/oceandb/
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-17 04:11:52.000000 pegasusX-0.1.5/pegasus/oceandb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:12:03.117573 pegasusX-0.1.5/pegasus/oceandb/api/
--rw-r--r--   0 runner    (1001) docker     (123)    10235 2023-07-17 04:11:52.000000 pegasusX-0.1.5/pegasus/oceandb/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11533 2023-07-17 04:11:52.000000 pegasusX-0.1.5/pegasus/oceandb/api/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)    16334 2023-07-17 04:11:52.000000 pegasusX-0.1.5/pegasus/oceandb/api/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    12827 2023-07-17 04:11:52.000000 pegasusX-0.1.5/pegasus/oceandb/api/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-17 04:11:52.000000 pegasusX-0.1.5/pegasus/oceandb/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-17 04:11:52.000000 pegasusX-0.1.5/pegasus/oceandb/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:12:03.117573 pegasusX-0.1.5/pegasus/oceandb/db/
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-07-17 04:11:52.000000 pegasusX-0.1.5/pegasus/oceandb/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21244 2023-07-17 04:11:52.000000 pegasusX-0.1.5/pegasus/oceandb/db/clickhouse.py
--rw-r--r--   0 runner    (1001) docker     (123)    17598 2023-07-17 04:11:52.000000 pegasusX-0.1.5/pegasus/oceandb/db/duckdb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:12:03.117573 pegasusX-0.1.5/pegasus/oceandb/db/index/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-17 04:11:52.000000 pegasusX-0.1.5/pegasus/oceandb/db/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9126 2023-07-17 04:11:52.000000 pegasusX-0.1.5/pegasus/oceandb/db/index/hnswlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-17 04:11:52.000000 pegasusX-0.1.5/pegasus/oceandb/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:12:03.117573 pegasusX-0.1.5/pegasus/oceandb/server/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-17 04:11:52.000000 pegasusX-0.1.5/pegasus/oceandb/server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:12:03.117573 pegasusX-0.1.5/pegasus/oceandb/server/fastapi/
--rw-r--r--   0 runner    (1001) docker     (123)     8456 2023-07-17 04:11:52.000000 pegasusX-0.1.5/pegasus/oceandb/server/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-07-17 04:11:52.000000 pegasusX-0.1.5/pegasus/oceandb/server/fastapi/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:12:03.117573 pegasusX-0.1.5/pegasus/oceandb/telemetry/
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-17 04:11:52.000000 pegasusX-0.1.5/pegasus/oceandb/telemetry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-17 04:11:52.000000 pegasusX-0.1.5/pegasus/oceandb/telemetry/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-17 04:11:52.000000 pegasusX-0.1.5/pegasus/oceandb/telemetry/posthog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:12:03.117573 pegasusX-0.1.5/pegasus/oceandb/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 04:11:52.000000 pegasusX-0.1.5/pegasus/oceandb/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8028 2023-07-17 04:11:52.000000 pegasusX-0.1.5/pegasus/oceandb/utils/embedding_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:12:03.117573 pegasusX-0.1.5/pegasusX.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 04:12:03.000000 pegasusX-0.1.5/pegasusX.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-17 04:12:03.000000 pegasusX-0.1.5/pegasusX.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 04:12:03.000000 pegasusX-0.1.5/pegasusX.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-17 04:12:03.000000 pegasusX-0.1.5/pegasusX.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 04:12:03.000000 pegasusX-0.1.5/pegasusX.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 04:12:03.117573 pegasusX-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-17 04:11:52.000000 pegasusX-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:15:31.721065 pegasusX-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 04:15:18.000000 pegasusX-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 04:15:31.721065 pegasusX-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-07-17 04:15:18.000000 pegasusX-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:15:31.717065 pegasusX-0.1.6/pegasus/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-17 04:15:18.000000 pegasusX-0.1.6/pegasus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-17 04:15:18.000000 pegasusX-0.1.6/pegasus/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:15:31.717065 pegasusX-0.1.6/pegasus/oceandb/
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-17 04:15:18.000000 pegasusX-0.1.6/pegasus/oceandb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:15:31.717065 pegasusX-0.1.6/pegasus/oceandb/api/
+-rw-r--r--   0 runner    (1001) docker     (123)    10235 2023-07-17 04:15:18.000000 pegasusX-0.1.6/pegasus/oceandb/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11533 2023-07-17 04:15:18.000000 pegasusX-0.1.6/pegasus/oceandb/api/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16334 2023-07-17 04:15:18.000000 pegasusX-0.1.6/pegasus/oceandb/api/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12827 2023-07-17 04:15:18.000000 pegasusX-0.1.6/pegasus/oceandb/api/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-17 04:15:18.000000 pegasusX-0.1.6/pegasus/oceandb/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-17 04:15:18.000000 pegasusX-0.1.6/pegasus/oceandb/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:15:31.717065 pegasusX-0.1.6/pegasus/oceandb/db/
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-07-17 04:15:18.000000 pegasusX-0.1.6/pegasus/oceandb/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21244 2023-07-17 04:15:18.000000 pegasusX-0.1.6/pegasus/oceandb/db/clickhouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17598 2023-07-17 04:15:18.000000 pegasusX-0.1.6/pegasus/oceandb/db/duckdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:15:31.717065 pegasusX-0.1.6/pegasus/oceandb/db/index/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-17 04:15:18.000000 pegasusX-0.1.6/pegasus/oceandb/db/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9126 2023-07-17 04:15:18.000000 pegasusX-0.1.6/pegasus/oceandb/db/index/hnswlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-17 04:15:18.000000 pegasusX-0.1.6/pegasus/oceandb/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:15:31.717065 pegasusX-0.1.6/pegasus/oceandb/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-17 04:15:18.000000 pegasusX-0.1.6/pegasus/oceandb/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:15:31.717065 pegasusX-0.1.6/pegasus/oceandb/server/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)     8456 2023-07-17 04:15:18.000000 pegasusX-0.1.6/pegasus/oceandb/server/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-07-17 04:15:18.000000 pegasusX-0.1.6/pegasus/oceandb/server/fastapi/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:15:31.717065 pegasusX-0.1.6/pegasus/oceandb/telemetry/
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-17 04:15:18.000000 pegasusX-0.1.6/pegasus/oceandb/telemetry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-17 04:15:18.000000 pegasusX-0.1.6/pegasus/oceandb/telemetry/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-17 04:15:18.000000 pegasusX-0.1.6/pegasus/oceandb/telemetry/posthog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:15:31.721065 pegasusX-0.1.6/pegasus/oceandb/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 04:15:18.000000 pegasusX-0.1.6/pegasus/oceandb/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8028 2023-07-17 04:15:18.000000 pegasusX-0.1.6/pegasus/oceandb/utils/embedding_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:15:31.721065 pegasusX-0.1.6/pegasusX.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 04:15:31.000000 pegasusX-0.1.6/pegasusX.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-17 04:15:31.000000 pegasusX-0.1.6/pegasusX.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 04:15:31.000000 pegasusX-0.1.6/pegasusX.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-17 04:15:31.000000 pegasusX-0.1.6/pegasusX.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 04:15:31.000000 pegasusX-0.1.6/pegasusX.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 04:15:31.721065 pegasusX-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-17 04:15:18.000000 pegasusX-0.1.6/setup.py
```

### Comparing `pegasusX-0.1.5/LICENSE` & `pegasusX-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pegasusX-0.1.5/PKG-INFO` & `pegasusX-0.1.6/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pegasusX
-Version: 0.1.5
+Version: 0.1.6
 Summary: pegasus - Pytorch
 Home-page: https://github.com/kyegomez/pegasus
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pegasusX-0.1.5/README.md` & `pegasusX-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `pegasusX-0.1.5/pegasus/main.py` & `pegasusX-0.1.6/pegasus/main.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.1.5/pegasus/oceandb/__init__.py` & `pegasusX-0.1.6/pegasus/oceandb/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from . import config
 import logging
-from oceandb.telemetry.events import ClientStartEvent
-from oceandb.telemetry.posthog import Posthog
+from pegasus.oceandb.telemetry.events import ClientStartEvent
+from pegasus.oceandb.telemetry.posthog import Posthog
 
-from oceandb.utils.embedding_functions import ImageBindEmbeddingFunction
+from pegasus.oceandb.utils.embedding_functions import ImageBindEmbeddingFunction
 
 logger = logging.getLogger(__name__)
 
 __settings = config.Settings()
 
 __version__ = "0.3.22"
```

### Comparing `pegasusX-0.1.5/pegasus/oceandb/api/__init__.py` & `pegasusX-0.1.6/pegasus/oceandb/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.1.5/pegasus/oceandb/api/fastapi.py` & `pegasusX-0.1.6/pegasus/oceandb/api/fastapi.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.1.5/pegasus/oceandb/api/local.py` & `pegasusX-0.1.6/pegasus/oceandb/api/local.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.1.5/pegasus/oceandb/api/types.py` & `pegasusX-0.1.6/pegasus/oceandb/api/types.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.1.5/pegasus/oceandb/config.py` & `pegasusX-0.1.6/pegasus/oceandb/config.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.1.5/pegasus/oceandb/db/__init__.py` & `pegasusX-0.1.6/pegasus/oceandb/db/__init__.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.1.5/pegasus/oceandb/db/clickhouse.py` & `pegasusX-0.1.6/pegasus/oceandb/db/clickhouse.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.1.5/pegasus/oceandb/db/duckdb.py` & `pegasusX-0.1.6/pegasus/oceandb/db/duckdb.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.1.5/pegasus/oceandb/db/index/hnswlib.py` & `pegasusX-0.1.6/pegasus/oceandb/db/index/hnswlib.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.1.5/pegasus/oceandb/errors.py` & `pegasusX-0.1.6/pegasus/oceandb/errors.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.1.5/pegasus/oceandb/server/fastapi/__init__.py` & `pegasusX-0.1.6/pegasus/oceandb/server/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.1.5/pegasus/oceandb/server/fastapi/types.py` & `pegasusX-0.1.6/pegasus/oceandb/server/fastapi/types.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.1.5/pegasus/oceandb/telemetry/__init__.py` & `pegasusX-0.1.6/pegasus/oceandb/telemetry/__init__.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.1.5/pegasus/oceandb/telemetry/events.py` & `pegasusX-0.1.6/pegasus/oceandb/telemetry/events.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.1.5/pegasus/oceandb/telemetry/posthog.py` & `pegasusX-0.1.6/pegasus/oceandb/telemetry/posthog.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.1.5/pegasus/oceandb/utils/embedding_functions.py` & `pegasusX-0.1.6/pegasus/oceandb/utils/embedding_functions.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.1.5/pegasusX.egg-info/PKG-INFO` & `pegasusX-0.1.6/pegasusX.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pegasusX
-Version: 0.1.5
+Version: 0.1.6
 Summary: pegasus - Pytorch
 Home-page: https://github.com/kyegomez/pegasus
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pegasusX-0.1.5/pegasusX.egg-info/SOURCES.txt` & `pegasusX-0.1.6/pegasusX.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pegasusX-0.1.5/setup.py` & `pegasusX-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 # 
 
 setup(
   name = 'pegasusX',
   packages = find_packages(exclude=[]),
-  version = '0.1.5',
+  version = '0.1.6',
   license='MIT',
   description = 'pegasus - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/pegasus',
   keywords = [
```

