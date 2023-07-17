# Comparing `tmp/pegasusX-0.2.4.tar.gz` & `tmp/pegasusX-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pegasusX-0.2.4.tar", last modified: Mon Jul 17 14:42:19 2023, max compression
+gzip compressed data, was "pegasusX-0.2.5.tar", last modified: Mon Jul 17 14:47:14 2023, max compression
```

## Comparing `pegasusX-0.2.4.tar` & `pegasusX-0.2.5.tar`

### file list

```diff
@@ -1,18 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:42:19.428125 pegasusX-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 14:42:08.000000 pegasusX-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 14:42:19.428125 pegasusX-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-07-17 14:42:08.000000 pegasusX-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:42:19.428125 pegasusX-0.2.4/pegasus/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-17 14:42:08.000000 pegasusX-0.2.4/pegasus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-07-17 14:42:08.000000 pegasusX-0.2.4/pegasus/embedding_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-17 14:42:08.000000 pegasusX-0.2.4/pegasus/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-17 14:42:08.000000 pegasusX-0.2.4/pegasus/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-07-17 14:42:08.000000 pegasusX-0.2.4/pegasus/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:42:19.428125 pegasusX-0.2.4/pegasusX.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 14:42:19.000000 pegasusX-0.2.4/pegasusX.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-17 14:42:19.000000 pegasusX-0.2.4/pegasusX.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 14:42:19.000000 pegasusX-0.2.4/pegasusX.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-17 14:42:19.000000 pegasusX-0.2.4/pegasusX.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 14:42:19.000000 pegasusX-0.2.4/pegasusX.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 14:42:19.428125 pegasusX-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-17 14:42:08.000000 pegasusX-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:47:14.573933 pegasusX-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 14:47:01.000000 pegasusX-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 14:47:14.573933 pegasusX-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-07-17 14:47:01.000000 pegasusX-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:47:14.573933 pegasusX-0.2.5/pegasus/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:47:14.573933 pegasusX-0.2.5/pegasus/ImageBind/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-17 14:47:01.000000 pegasusX-0.2.5/pegasus/ImageBind/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11875 2023-07-17 14:47:01.000000 pegasusX-0.2.5/pegasus/ImageBind/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:47:14.573933 pegasusX-0.2.5/pegasus/ImageBind/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:47:01.000000 pegasusX-0.2.5/pegasus/ImageBind/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-07-17 14:47:01.000000 pegasusX-0.2.5/pegasus/ImageBind/models/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16431 2023-07-17 14:47:01.000000 pegasusX-0.2.5/pegasus/ImageBind/models/imagebind_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23088 2023-07-17 14:47:01.000000 pegasusX-0.2.5/pegasus/ImageBind/models/multimodal_preprocessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9748 2023-07-17 14:47:01.000000 pegasusX-0.2.5/pegasus/ImageBind/models/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-17 14:47:01.000000 pegasusX-0.2.5/pegasus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-07-17 14:47:01.000000 pegasusX-0.2.5/pegasus/embedding_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-17 14:47:01.000000 pegasusX-0.2.5/pegasus/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-17 14:47:01.000000 pegasusX-0.2.5/pegasus/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-07-17 14:47:01.000000 pegasusX-0.2.5/pegasus/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:47:14.573933 pegasusX-0.2.5/pegasusX.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 14:47:14.000000 pegasusX-0.2.5/pegasusX.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-17 14:47:14.000000 pegasusX-0.2.5/pegasusX.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 14:47:14.000000 pegasusX-0.2.5/pegasusX.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-17 14:47:14.000000 pegasusX-0.2.5/pegasusX.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 14:47:14.000000 pegasusX-0.2.5/pegasusX.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 14:47:14.573933 pegasusX-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-17 14:47:01.000000 pegasusX-0.2.5/setup.py
```

### Comparing `pegasusX-0.2.4/LICENSE` & `pegasusX-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pegasusX-0.2.4/PKG-INFO` & `pegasusX-0.2.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pegasusX
-Version: 0.2.4
+Version: 0.2.5
 Summary: pegasus - Pytorch
 Home-page: https://github.com/kyegomez/pegasus
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pegasusX-0.2.4/README.md` & `pegasusX-0.2.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -101,8 +101,11 @@
 
 * **Production-Level API Deployment:** PegasusX will enter Agora's paid API line up so you can effortlessly make API requests and receive your embeddings no complicated setup necessary
 
 * **Making it Extremely Fast Through Quantization:** By utilizing quantization techniques, we aim to significantly increase the speed and efficiency of the PegasusX model.
 
 * **Parallelization, Asynchrony, and Other Optimizations:** To ensure seamless operation even with large amounts of data, we're planning to implement parallelization, asynchronous operations, and other optimizations in the model.
 
-Thank you for considering contributing to PegasusX. Your expertise and commitment to this project are what make it thrive. Let's build the future of multimodal embeddings together.
+* Remake in Jax using dynamic sparse flash attention
+
+Thank you for considering contributing to PegasusX. Your expertise and commitment to this project are what make it thrive. Let's build the future of multimodal embeddings together.
+
```

### Comparing `pegasusX-0.2.4/pegasus/embedding_functions.py` & `pegasusX-0.2.5/pegasus/embedding_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pegasus.types import Documents, EmbeddingFunction, Embeddings
 from typing import Optional
 import torch
 
-from pegasus.ImageBind.models import imagebind_model
-from pegasus.ImageBind.models.imagebind_model import ModalityType
-from pegasus.ImageBind.data import load_and_transform_text, load_and_transform_vision_data, load_and_transform_audio_data
+from pegasus.ImageBind import imagebind_model
+from pegasus.ImageBind import ModalityType
+from pegasus.ImageBind import load_and_transform_text, load_and_transform_vision_data, load_and_transform_audio_data
 
 
 class MultiModalEmbeddingFunction(EmbeddingFunction):
     def __init__(
         self,
         modality: str = ModalityType,  # type: ignore
         model_path: str = "https://dl.fbaipublicfiles.com/imagebind/imagebind_huge.pth",
```

### Comparing `pegasusX-0.2.4/pegasus/errors.py` & `pegasusX-0.2.5/pegasus/errors.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.2.4/pegasus/main.py` & `pegasusX-0.2.5/pegasus/main.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.2.4/pegasus/types.py` & `pegasusX-0.2.5/pegasus/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Optional, Union, Dict, Sequence, TypeVar, List
 from typing_extensions import Literal, TypedDict, Protocol
 import pegasus.errors as errors
 from abc import ABC, abstractmethod
 import torch.nn as nn
 
 # from ..utils.ImageBind.imagebind_model import ModalityType
-from pegasus.ImageBind.models.imagebind_model import ModalityType
+from pegasus.ImageBind import ModalityType
 
 import numpy as np
 
 # use better cosine
 from sklearn.metrics.pairwise import cosine_similarity
```

### Comparing `pegasusX-0.2.4/pegasusX.egg-info/PKG-INFO` & `pegasusX-0.2.5/pegasusX.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pegasusX
-Version: 0.2.4
+Version: 0.2.5
 Summary: pegasus - Pytorch
 Home-page: https://github.com/kyegomez/pegasus
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pegasusX-0.2.4/setup.py` & `pegasusX-0.2.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 # 
 
 setup(
   name = 'pegasusX',
   packages = find_packages(exclude=[]),
-  version = '0.2.4',
+  version = '0.2.5',
   license='MIT',
   description = 'pegasus - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/pegasus',
   keywords = [
```

