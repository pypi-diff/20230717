# Comparing `tmp/pegasusX-0.2.2.tar.gz` & `tmp/pegasusX-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pegasusX-0.2.2.tar", last modified: Mon Jul 17 14:21:44 2023, max compression
+gzip compressed data, was "pegasusX-0.2.4.tar", last modified: Mon Jul 17 14:42:19 2023, max compression
```

## Comparing `pegasusX-0.2.2.tar` & `pegasusX-0.2.4.tar`

### file list

```diff
@@ -1,25 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:21:44.259887 pegasusX-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 14:21:33.000000 pegasusX-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 14:21:44.259887 pegasusX-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-07-17 14:21:33.000000 pegasusX-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:21:44.259887 pegasusX-0.2.2/pegasus/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-17 14:21:33.000000 pegasusX-0.2.2/pegasus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-17 14:21:33.000000 pegasusX-0.2.2/pegasus/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:21:44.259887 pegasusX-0.2.2/pegasus/oceandb/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-17 14:21:33.000000 pegasusX-0.2.2/pegasus/oceandb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:21:44.259887 pegasusX-0.2.2/pegasus/oceandb/api/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-17 14:21:33.000000 pegasusX-0.2.2/pegasus/oceandb/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12835 2023-07-17 14:21:33.000000 pegasusX-0.2.2/pegasus/oceandb/api/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-17 14:21:33.000000 pegasusX-0.2.2/pegasus/oceandb/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-17 14:21:33.000000 pegasusX-0.2.2/pegasus/oceandb/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:21:44.259887 pegasusX-0.2.2/pegasus/oceandb/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:21:33.000000 pegasusX-0.2.2/pegasus/oceandb/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-07-17 14:21:33.000000 pegasusX-0.2.2/pegasus/oceandb/utils/embedding_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:21:44.259887 pegasusX-0.2.2/pegasusX.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 14:21:44.000000 pegasusX-0.2.2/pegasusX.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-17 14:21:44.000000 pegasusX-0.2.2/pegasusX.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 14:21:44.000000 pegasusX-0.2.2/pegasusX.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-17 14:21:44.000000 pegasusX-0.2.2/pegasusX.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 14:21:44.000000 pegasusX-0.2.2/pegasusX.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 14:21:44.259887 pegasusX-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-17 14:21:33.000000 pegasusX-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:42:19.428125 pegasusX-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 14:42:08.000000 pegasusX-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 14:42:19.428125 pegasusX-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-07-17 14:42:08.000000 pegasusX-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:42:19.428125 pegasusX-0.2.4/pegasus/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-17 14:42:08.000000 pegasusX-0.2.4/pegasus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-07-17 14:42:08.000000 pegasusX-0.2.4/pegasus/embedding_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-17 14:42:08.000000 pegasusX-0.2.4/pegasus/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-17 14:42:08.000000 pegasusX-0.2.4/pegasus/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-07-17 14:42:08.000000 pegasusX-0.2.4/pegasus/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:42:19.428125 pegasusX-0.2.4/pegasusX.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 14:42:19.000000 pegasusX-0.2.4/pegasusX.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-17 14:42:19.000000 pegasusX-0.2.4/pegasusX.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 14:42:19.000000 pegasusX-0.2.4/pegasusX.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-17 14:42:19.000000 pegasusX-0.2.4/pegasusX.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 14:42:19.000000 pegasusX-0.2.4/pegasusX.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 14:42:19.428125 pegasusX-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-17 14:42:08.000000 pegasusX-0.2.4/setup.py
```

### Comparing `pegasusX-0.2.2/LICENSE` & `pegasusX-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pegasusX-0.2.2/PKG-INFO` & `pegasusX-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pegasusX
-Version: 0.2.2
+Version: 0.2.4
 Summary: pegasus - Pytorch
 Home-page: https://github.com/kyegomez/pegasus
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pegasusX-0.2.2/README.md` & `pegasusX-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `pegasusX-0.2.2/pegasus/main.py` & `pegasusX-0.2.4/pegasus/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from concurrent.futures import ProcessPoolExecutor, as_completed
 from numba import njit
 from joblib import Memory
 import numpy as np
 
-# from pegasus.Ocean import ImageBindEmbeddingFunctio
-from pegasus.oceandb import ImageBindEmbeddingFunction
+from pegasus.embedding_functions import MultiModalEmbeddingFunction
 
 memory = Memory("PegasusStore", verbose=0)
 
 @memory.cache
 @njit
 def optimized_embedding_function(modality, data):
-    return ImageBindEmbeddingFunction(modality)(data)
+    return MultiModalEmbeddingFunction(modality)(data)
 
 class Pegasus:
     def __init__(self, modality, multi_process=False, n_processes=4):
         self.modality = modality
         self.multi_process = multi_process
         self.n_processes = n_processes if multi_process else 1
```

### Comparing `pegasusX-0.2.2/pegasus/oceandb/api/types.py` & `pegasusX-0.2.4/pegasus/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from typing import Optional, Union, Dict, Sequence, TypeVar, List
 from typing_extensions import Literal, TypedDict, Protocol
-import pegasus.oceandb.errors as errors
+import pegasus.errors as errors
 from abc import ABC, abstractmethod
 import torch.nn as nn
 
 # from ..utils.ImageBind.imagebind_model import ModalityType
-from ..utils.ImageBind.models.imagebind_model import ModalityType
+from pegasus.ImageBind.models.imagebind_model import ModalityType
+
 import numpy as np
 
 # use better cosine
 from sklearn.metrics.pairwise import cosine_similarity
 
 
 ID = str
@@ -249,15 +250,15 @@
     ) -> List[List[ID]]:
         pass
 
 
 class CrossModalRetrieval(SearchFunction):
 
     """
-    Use the provided ImageBindEmbeddingFunction to compute embeddings for the query.
+    Use the provided MultiModalEmbeddingFunction to compute embeddings for the query.
     Select the corresponding embeddings of the other modality.
     Perform similarity search using the computed embeddings.
     Return the results.
 
     """
 
     def __init__(self, modality: str):
```

### Comparing `pegasusX-0.2.2/pegasus/oceandb/errors.py` & `pegasusX-0.2.4/pegasus/errors.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.2.2/pegasus/oceandb/utils/embedding_functions.py` & `pegasusX-0.2.4/pegasus/embedding_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from oceandb.api.types import Documents, EmbeddingFunction, Embeddings
+from pegasus.types import Documents, EmbeddingFunction, Embeddings
 from typing import Optional
 import torch
 
-from .ImageBind.models import imagebind_model
-from .ImageBind.models.imagebind_model import ModalityType
-from .ImageBind.data import load_and_transform_text, load_and_transform_vision_data, load_and_transform_audio_data
+from pegasus.ImageBind.models import imagebind_model
+from pegasus.ImageBind.models.imagebind_model import ModalityType
+from pegasus.ImageBind.data import load_and_transform_text, load_and_transform_vision_data, load_and_transform_audio_data
 
 
-class ImageBindEmbeddingFunction(EmbeddingFunction):
+class MultiModalEmbeddingFunction(EmbeddingFunction):
     def __init__(
         self,
         modality: str = ModalityType,  # type: ignore
         model_path: str = "https://dl.fbaipublicfiles.com/imagebind/imagebind_huge.pth",
         device: str = "cuda:0"
     ):
         self._modality = modality
@@ -56,17 +56,17 @@
 
         # return embeddings_list
 
         return [embedding.tolist() for embedding in embeddings_array]
 
 
 """
-text_embedding_function = ImageBindEmbeddingFunction(modality=ModalityType.TEXT)
-vision_embedding_function = ImageBindEmbeddingFunction(modality=ModalityType.VISION)
-audio_embedding_function = ImageBindEmbeddingFunction(modality=ModalityType.AUDIO)
+text_embedding_function = MultiModalEmbeddingFunction(modality=ModalityType.TEXT)
+vision_embedding_function = MultiModalEmbeddingFunction(modality=ModalityType.VISION)
+audio_embedding_function = MultiModalEmbeddingFunction(modality=ModalityType.AUDIO)
 
 
 """
 
 
 class OpenAIEmbeddingFunction(EmbeddingFunction):
     def __init__(
```

### Comparing `pegasusX-0.2.2/pegasusX.egg-info/PKG-INFO` & `pegasusX-0.2.4/pegasusX.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pegasusX
-Version: 0.2.2
+Version: 0.2.4
 Summary: pegasus - Pytorch
 Home-page: https://github.com/kyegomez/pegasus
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pegasusX-0.2.2/setup.py` & `pegasusX-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 # 
 
 setup(
   name = 'pegasusX',
   packages = find_packages(exclude=[]),
-  version = '0.2.2',
+  version = '0.2.4',
   license='MIT',
   description = 'pegasus - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/pegasus',
   keywords = [
```

