# Comparing `tmp/pegasusX-0.1.7.tar.gz` & `tmp/pegasusX-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pegasusX-0.1.7.tar", last modified: Mon Jul 17 04:24:34 2023, max compression
+gzip compressed data, was "pegasusX-0.2.0.tar", last modified: Mon Jul 17 04:45:38 2023, max compression
```

## Comparing `pegasusX-0.1.7.tar` & `pegasusX-0.2.0.tar`

### file list

```diff
@@ -1,44 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:24:34.897679 pegasusX-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 04:24:20.000000 pegasusX-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 04:24:34.893679 pegasusX-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-07-17 04:24:20.000000 pegasusX-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:24:34.885679 pegasusX-0.1.7/pegasus/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-17 04:24:20.000000 pegasusX-0.1.7/pegasus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-17 04:24:20.000000 pegasusX-0.1.7/pegasus/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:24:34.889679 pegasusX-0.1.7/pegasus/oceandb/
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-07-17 04:24:20.000000 pegasusX-0.1.7/pegasus/oceandb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:24:34.889679 pegasusX-0.1.7/pegasus/oceandb/api/
--rw-r--r--   0 runner    (1001) docker     (123)    10265 2023-07-17 04:24:20.000000 pegasusX-0.1.7/pegasus/oceandb/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11581 2023-07-17 04:24:20.000000 pegasusX-0.1.7/pegasus/oceandb/api/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)    16412 2023-07-17 04:24:20.000000 pegasusX-0.1.7/pegasus/oceandb/api/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    12835 2023-07-17 04:24:20.000000 pegasusX-0.1.7/pegasus/oceandb/api/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-17 04:24:20.000000 pegasusX-0.1.7/pegasus/oceandb/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-17 04:24:20.000000 pegasusX-0.1.7/pegasus/oceandb/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:24:34.889679 pegasusX-0.1.7/pegasus/oceandb/db/
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-17 04:24:20.000000 pegasusX-0.1.7/pegasus/oceandb/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21284 2023-07-17 04:24:20.000000 pegasusX-0.1.7/pegasus/oceandb/db/clickhouse.py
--rw-r--r--   0 runner    (1001) docker     (123)    17618 2023-07-17 04:24:20.000000 pegasusX-0.1.7/pegasus/oceandb/db/duckdb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:24:34.889679 pegasusX-0.1.7/pegasus/oceandb/db/index/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-17 04:24:20.000000 pegasusX-0.1.7/pegasus/oceandb/db/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-07-17 04:24:20.000000 pegasusX-0.1.7/pegasus/oceandb/db/index/hnswlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-17 04:24:20.000000 pegasusX-0.1.7/pegasus/oceandb/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:24:34.893679 pegasusX-0.1.7/pegasus/oceandb/server/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-17 04:24:20.000000 pegasusX-0.1.7/pegasus/oceandb/server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:24:34.893679 pegasusX-0.1.7/pegasus/oceandb/server/fastapi/
--rw-r--r--   0 runner    (1001) docker     (123)     8510 2023-07-17 04:24:20.000000 pegasusX-0.1.7/pegasus/oceandb/server/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-17 04:24:20.000000 pegasusX-0.1.7/pegasus/oceandb/server/fastapi/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:24:34.893679 pegasusX-0.1.7/pegasus/oceandb/telemetry/
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-07-17 04:24:20.000000 pegasusX-0.1.7/pegasus/oceandb/telemetry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-17 04:24:20.000000 pegasusX-0.1.7/pegasus/oceandb/telemetry/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-17 04:24:20.000000 pegasusX-0.1.7/pegasus/oceandb/telemetry/posthog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:24:34.893679 pegasusX-0.1.7/pegasus/oceandb/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 04:24:20.000000 pegasusX-0.1.7/pegasus/oceandb/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-07-17 04:24:20.000000 pegasusX-0.1.7/pegasus/oceandb/utils/embedding_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:24:34.893679 pegasusX-0.1.7/pegasusX.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 04:24:34.000000 pegasusX-0.1.7/pegasusX.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-17 04:24:34.000000 pegasusX-0.1.7/pegasusX.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 04:24:34.000000 pegasusX-0.1.7/pegasusX.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-17 04:24:34.000000 pegasusX-0.1.7/pegasusX.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 04:24:34.000000 pegasusX-0.1.7/pegasusX.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 04:24:34.897679 pegasusX-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-17 04:24:20.000000 pegasusX-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:45:38.000773 pegasusX-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 04:45:23.000000 pegasusX-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 04:45:38.000773 pegasusX-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-07-17 04:45:23.000000 pegasusX-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:45:38.000773 pegasusX-0.2.0/pegasus/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-17 04:45:23.000000 pegasusX-0.2.0/pegasus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-17 04:45:23.000000 pegasusX-0.2.0/pegasus/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:45:38.000773 pegasusX-0.2.0/pegasus/oceandb/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-17 04:45:23.000000 pegasusX-0.2.0/pegasus/oceandb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-17 04:45:23.000000 pegasusX-0.2.0/pegasus/oceandb/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-17 04:45:23.000000 pegasusX-0.2.0/pegasus/oceandb/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:45:38.000773 pegasusX-0.2.0/pegasus/oceandb/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 04:45:23.000000 pegasusX-0.2.0/pegasus/oceandb/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8036 2023-07-17 04:45:23.000000 pegasusX-0.2.0/pegasus/oceandb/utils/embedding_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:45:38.000773 pegasusX-0.2.0/pegasusX.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 04:45:37.000000 pegasusX-0.2.0/pegasusX.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-17 04:45:37.000000 pegasusX-0.2.0/pegasusX.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 04:45:37.000000 pegasusX-0.2.0/pegasusX.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-17 04:45:37.000000 pegasusX-0.2.0/pegasusX.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 04:45:37.000000 pegasusX-0.2.0/pegasusX.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 04:45:38.000773 pegasusX-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-17 04:45:23.000000 pegasusX-0.2.0/setup.py
```

### Comparing `pegasusX-0.1.7/LICENSE` & `pegasusX-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pegasusX-0.1.7/PKG-INFO` & `pegasusX-0.2.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pegasusX
-Version: 0.1.7
+Version: 0.2.0
 Summary: pegasus - Pytorch
 Home-page: https://github.com/kyegomez/pegasus
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pegasusX-0.1.7/README.md` & `pegasusX-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pegasusX-0.1.7/pegasus/main.py` & `pegasusX-0.2.0/pegasus/main.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.1.7/pegasus/oceandb/config.py` & `pegasusX-0.2.0/pegasus/oceandb/config.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.1.7/pegasus/oceandb/errors.py` & `pegasusX-0.2.0/pegasus/oceandb/errors.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.1.7/pegasus/oceandb/utils/embedding_functions.py` & `pegasusX-0.2.0/pegasus/oceandb/utils/embedding_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import pegasus.oceandb.api.types import Documents, EmbeddingFunction, Embeddings
+from pegasus.oceandb.api.types import Documents, EmbeddingFunction, Embeddings
 from typing import Optional
 import torch
 from .ImageBind.models import imagebind_model
 from .ImageBind.models.imagebind_model import ModalityType
 from .ImageBind.data import load_and_transform_text, load_and_transform_vision_data, load_and_transform_audio_data
 
 class SentenceTransformerEmbeddingFunction(EmbeddingFunction):
```

### Comparing `pegasusX-0.1.7/pegasusX.egg-info/PKG-INFO` & `pegasusX-0.2.0/pegasusX.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pegasusX
-Version: 0.1.7
+Version: 0.2.0
 Summary: pegasus - Pytorch
 Home-page: https://github.com/kyegomez/pegasus
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pegasusX-0.1.7/setup.py` & `pegasusX-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 # 
 
 setup(
   name = 'pegasusX',
   packages = find_packages(exclude=[]),
-  version = '0.1.7',
+  version = '0.2.0',
   license='MIT',
   description = 'pegasus - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/pegasus',
   keywords = [
```

