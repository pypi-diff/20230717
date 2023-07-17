# Comparing `tmp/pegasusX-0.2.9.tar.gz` & `tmp/pegasusX-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pegasusX-0.2.9.tar", last modified: Mon Jul 17 15:47:15 2023, max compression
+gzip compressed data, was "pegasusX-0.3.0.tar", last modified: Mon Jul 17 15:52:03 2023, max compression
```

## Comparing `pegasusX-0.2.9.tar` & `pegasusX-0.3.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:47:15.791410 pegasusX-0.2.9/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 15:47:00.000000 pegasusX-0.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 15:47:15.791410 pegasusX-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9510 2023-07-17 15:47:00.000000 pegasusX-0.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:47:15.787410 pegasusX-0.2.9/pegasus/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:47:15.791410 pegasusX-0.2.9/pegasus/ImageBind/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-17 15:47:00.000000 pegasusX-0.2.9/pegasus/ImageBind/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11875 2023-07-17 15:47:00.000000 pegasusX-0.2.9/pegasus/ImageBind/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:47:15.791410 pegasusX-0.2.9/pegasus/ImageBind/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:47:00.000000 pegasusX-0.2.9/pegasus/ImageBind/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-07-17 15:47:00.000000 pegasusX-0.2.9/pegasus/ImageBind/models/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16431 2023-07-17 15:47:00.000000 pegasusX-0.2.9/pegasus/ImageBind/models/imagebind_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    23088 2023-07-17 15:47:00.000000 pegasusX-0.2.9/pegasus/ImageBind/models/multimodal_preprocessors.py
--rw-r--r--   0 runner    (1001) docker     (123)     9748 2023-07-17 15:47:00.000000 pegasusX-0.2.9/pegasus/ImageBind/models/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-17 15:47:00.000000 pegasusX-0.2.9/pegasus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-07-17 15:47:00.000000 pegasusX-0.2.9/pegasus/embedding_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-17 15:47:00.000000 pegasusX-0.2.9/pegasus/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-17 15:47:00.000000 pegasusX-0.2.9/pegasus/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-07-17 15:47:00.000000 pegasusX-0.2.9/pegasus/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:47:15.791410 pegasusX-0.2.9/pegasusX.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 15:47:15.000000 pegasusX-0.2.9/pegasusX.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-17 15:47:15.000000 pegasusX-0.2.9/pegasusX.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 15:47:15.000000 pegasusX-0.2.9/pegasusX.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-17 15:47:15.000000 pegasusX-0.2.9/pegasusX.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 15:47:15.000000 pegasusX-0.2.9/pegasusX.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 15:47:15.791410 pegasusX-0.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-17 15:47:00.000000 pegasusX-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:52:03.520499 pegasusX-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 15:51:49.000000 pegasusX-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 15:52:03.520499 pegasusX-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9510 2023-07-17 15:51:49.000000 pegasusX-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:52:03.520499 pegasusX-0.3.0/pegasus/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:52:03.520499 pegasusX-0.3.0/pegasus/ImageBind/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-17 15:51:49.000000 pegasusX-0.3.0/pegasus/ImageBind/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11875 2023-07-17 15:51:49.000000 pegasusX-0.3.0/pegasus/ImageBind/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:52:03.520499 pegasusX-0.3.0/pegasus/ImageBind/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:51:49.000000 pegasusX-0.3.0/pegasus/ImageBind/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-07-17 15:51:49.000000 pegasusX-0.3.0/pegasus/ImageBind/models/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16431 2023-07-17 15:51:49.000000 pegasusX-0.3.0/pegasus/ImageBind/models/imagebind_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23088 2023-07-17 15:51:49.000000 pegasusX-0.3.0/pegasus/ImageBind/models/multimodal_preprocessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9748 2023-07-17 15:51:49.000000 pegasusX-0.3.0/pegasus/ImageBind/models/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-17 15:51:49.000000 pegasusX-0.3.0/pegasus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-07-17 15:51:49.000000 pegasusX-0.3.0/pegasus/embedding_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-17 15:51:49.000000 pegasusX-0.3.0/pegasus/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-17 15:51:49.000000 pegasusX-0.3.0/pegasus/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-07-17 15:51:49.000000 pegasusX-0.3.0/pegasus/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:52:03.520499 pegasusX-0.3.0/pegasusX.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 15:52:03.000000 pegasusX-0.3.0/pegasusX.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-17 15:52:03.000000 pegasusX-0.3.0/pegasusX.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 15:52:03.000000 pegasusX-0.3.0/pegasusX.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-17 15:52:03.000000 pegasusX-0.3.0/pegasusX.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 15:52:03.000000 pegasusX-0.3.0/pegasusX.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 15:52:03.520499 pegasusX-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-17 15:51:49.000000 pegasusX-0.3.0/setup.py
```

### Comparing `pegasusX-0.2.9/LICENSE` & `pegasusX-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pegasusX-0.2.9/PKG-INFO` & `pegasusX-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pegasusX
-Version: 0.2.9
+Version: 0.3.0
 Summary: pegasus - Pytorch
 Home-page: https://github.com/kyegomez/pegasus
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pegasusX-0.2.9/README.md` & `pegasusX-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pegasusX-0.2.9/pegasus/ImageBind/data.py` & `pegasusX-0.3.0/pegasus/ImageBind/data.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.2.9/pegasus/ImageBind/models/helpers.py` & `pegasusX-0.3.0/pegasus/ImageBind/models/helpers.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.2.9/pegasus/ImageBind/models/imagebind_model.py` & `pegasusX-0.3.0/pegasus/ImageBind/models/imagebind_model.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.2.9/pegasus/ImageBind/models/multimodal_preprocessors.py` & `pegasusX-0.3.0/pegasus/ImageBind/models/multimodal_preprocessors.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.2.9/pegasus/ImageBind/models/transformer.py` & `pegasusX-0.3.0/pegasus/ImageBind/models/transformer.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.2.9/pegasus/embedding_functions.py` & `pegasusX-0.3.0/pegasus/embedding_functions.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.2.9/pegasus/errors.py` & `pegasusX-0.3.0/pegasus/errors.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.2.9/pegasus/main.py` & `pegasusX-0.3.0/pegasus/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from concurrent.futures import ProcessPoolExecutor, as_completed
-from numba import njit
-from joblib import Memory
+# from numba import njit
+# from joblib import Memory
 import numpy as np
 
 from pegasus.embedding_functions import MultiModalEmbeddingFunction
 
-memory = Memory("PegasusStore", verbose=0)
+# memory = Memory("PegasusStore", verbose=0)
 
-@memory.cache
-@njit
+# @memory.cache
+# # @njit
 def optimized_embedding_function(modality, data):
     return MultiModalEmbeddingFunction(modality)(data)
 
 class Pegasus:
     def __init__(self, modality, multi_process=False, n_processes=4):
         self.modality = modality
         self.multi_process = multi_process
```

### Comparing `pegasusX-0.2.9/pegasus/types.py` & `pegasusX-0.3.0/pegasus/types.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.2.9/pegasusX.egg-info/PKG-INFO` & `pegasusX-0.3.0/pegasusX.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pegasusX
-Version: 0.2.9
+Version: 0.3.0
 Summary: pegasus - Pytorch
 Home-page: https://github.com/kyegomez/pegasus
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pegasusX-0.2.9/pegasusX.egg-info/SOURCES.txt` & `pegasusX-0.3.0/pegasusX.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pegasusX-0.2.9/setup.py` & `pegasusX-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'pegasusX',
   packages = find_packages(exclude=[]),
-  version = '0.2.9',
+  version = '0.3.0',
   license='MIT',
   description = 'pegasus - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/pegasus',
   keywords = [
```

