# Comparing `tmp/pegasusX-0.3.0.tar.gz` & `tmp/pegasusX-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pegasusX-0.3.0.tar", last modified: Mon Jul 17 15:52:03 2023, max compression
+gzip compressed data, was "pegasusX-0.3.1.tar", last modified: Mon Jul 17 16:05:27 2023, max compression
```

## Comparing `pegasusX-0.3.0.tar` & `pegasusX-0.3.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:52:03.520499 pegasusX-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 15:51:49.000000 pegasusX-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 15:52:03.520499 pegasusX-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9510 2023-07-17 15:51:49.000000 pegasusX-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:52:03.520499 pegasusX-0.3.0/pegasus/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:52:03.520499 pegasusX-0.3.0/pegasus/ImageBind/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-17 15:51:49.000000 pegasusX-0.3.0/pegasus/ImageBind/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11875 2023-07-17 15:51:49.000000 pegasusX-0.3.0/pegasus/ImageBind/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:52:03.520499 pegasusX-0.3.0/pegasus/ImageBind/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:51:49.000000 pegasusX-0.3.0/pegasus/ImageBind/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-07-17 15:51:49.000000 pegasusX-0.3.0/pegasus/ImageBind/models/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16431 2023-07-17 15:51:49.000000 pegasusX-0.3.0/pegasus/ImageBind/models/imagebind_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    23088 2023-07-17 15:51:49.000000 pegasusX-0.3.0/pegasus/ImageBind/models/multimodal_preprocessors.py
--rw-r--r--   0 runner    (1001) docker     (123)     9748 2023-07-17 15:51:49.000000 pegasusX-0.3.0/pegasus/ImageBind/models/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-17 15:51:49.000000 pegasusX-0.3.0/pegasus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-07-17 15:51:49.000000 pegasusX-0.3.0/pegasus/embedding_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-17 15:51:49.000000 pegasusX-0.3.0/pegasus/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-17 15:51:49.000000 pegasusX-0.3.0/pegasus/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-07-17 15:51:49.000000 pegasusX-0.3.0/pegasus/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:52:03.520499 pegasusX-0.3.0/pegasusX.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 15:52:03.000000 pegasusX-0.3.0/pegasusX.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-17 15:52:03.000000 pegasusX-0.3.0/pegasusX.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 15:52:03.000000 pegasusX-0.3.0/pegasusX.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-17 15:52:03.000000 pegasusX-0.3.0/pegasusX.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 15:52:03.000000 pegasusX-0.3.0/pegasusX.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 15:52:03.520499 pegasusX-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-17 15:51:49.000000 pegasusX-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:05:27.171683 pegasusX-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 16:05:12.000000 pegasusX-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 16:05:27.171683 pegasusX-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9510 2023-07-17 16:05:12.000000 pegasusX-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:05:27.167683 pegasusX-0.3.1/pegasus/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:05:27.167683 pegasusX-0.3.1/pegasus/ImageBind/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-17 16:05:12.000000 pegasusX-0.3.1/pegasus/ImageBind/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11869 2023-07-17 16:05:12.000000 pegasusX-0.3.1/pegasus/ImageBind/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:05:27.171683 pegasusX-0.3.1/pegasus/ImageBind/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 16:05:12.000000 pegasusX-0.3.1/pegasus/ImageBind/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-07-17 16:05:12.000000 pegasusX-0.3.1/pegasus/ImageBind/models/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16431 2023-07-17 16:05:12.000000 pegasusX-0.3.1/pegasus/ImageBind/models/imagebind_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23088 2023-07-17 16:05:12.000000 pegasusX-0.3.1/pegasus/ImageBind/models/multimodal_preprocessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9748 2023-07-17 16:05:12.000000 pegasusX-0.3.1/pegasus/ImageBind/models/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-17 16:05:12.000000 pegasusX-0.3.1/pegasus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-17 16:05:12.000000 pegasusX-0.3.1/pegasus/embedding_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-17 16:05:12.000000 pegasusX-0.3.1/pegasus/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-17 16:05:12.000000 pegasusX-0.3.1/pegasus/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-07-17 16:05:12.000000 pegasusX-0.3.1/pegasus/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:05:27.171683 pegasusX-0.3.1/pegasusX.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 16:05:27.000000 pegasusX-0.3.1/pegasusX.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-17 16:05:27.000000 pegasusX-0.3.1/pegasusX.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 16:05:27.000000 pegasusX-0.3.1/pegasusX.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-17 16:05:27.000000 pegasusX-0.3.1/pegasusX.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 16:05:27.000000 pegasusX-0.3.1/pegasusX.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 16:05:27.171683 pegasusX-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-17 16:05:12.000000 pegasusX-0.3.1/setup.py
```

### Comparing `pegasusX-0.3.0/LICENSE` & `pegasusX-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pegasusX-0.3.0/PKG-INFO` & `pegasusX-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pegasusX
-Version: 0.3.0
+Version: 0.3.1
 Summary: pegasus - Pytorch
 Home-page: https://github.com/kyegomez/pegasus
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pegasusX-0.3.0/README.md` & `pegasusX-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pegasusX-0.3.0/pegasus/ImageBind/data.py` & `pegasusX-0.3.1/pegasus/ImageBind/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from pytorchvideo.data.encoded_video import EncodedVideo
 
 from torchvision import transforms
 from torchvision.transforms._transforms_video import NormalizeVideo
 
 DEFAULT_AUDIO_FRAME_SHIFT_MS = 10  # in milliseconds
 
-BPE_PATH = "oceandb/utils/ImageBind/bpe_simple_vocab_16e6.txt.gz"
+BPE_PATH = "pegasus/ImageBind/bpe_simple_vocab_16e6.txt.gz"
 
 
 def waveform2melspec(waveform, sample_rate, num_mel_bins, target_length):
     # Based on https://github.com/YuanGongND/ast/blob/d7d8b4b8e06cdaeb6c843cdb38794c1c7692234c/src/dataloader.py#L102
     waveform -= waveform.mean()
     fbank = torchaudio.compliance.kaldi.fbank(
         waveform,
```

### Comparing `pegasusX-0.3.0/pegasus/ImageBind/models/helpers.py` & `pegasusX-0.3.1/pegasus/ImageBind/models/helpers.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.3.0/pegasus/ImageBind/models/imagebind_model.py` & `pegasusX-0.3.1/pegasus/ImageBind/models/imagebind_model.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.3.0/pegasus/ImageBind/models/multimodal_preprocessors.py` & `pegasusX-0.3.1/pegasus/ImageBind/models/multimodal_preprocessors.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.3.0/pegasus/ImageBind/models/transformer.py` & `pegasusX-0.3.1/pegasus/ImageBind/models/transformer.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.3.0/pegasus/errors.py` & `pegasusX-0.3.1/pegasus/errors.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.3.0/pegasus/main.py` & `pegasusX-0.3.1/pegasus/main.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.3.0/pegasus/types.py` & `pegasusX-0.3.1/pegasus/types.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.3.0/pegasusX.egg-info/PKG-INFO` & `pegasusX-0.3.1/pegasusX.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pegasusX
-Version: 0.3.0
+Version: 0.3.1
 Summary: pegasus - Pytorch
 Home-page: https://github.com/kyegomez/pegasus
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pegasusX-0.3.0/pegasusX.egg-info/SOURCES.txt` & `pegasusX-0.3.1/pegasusX.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pegasusX-0.3.0/setup.py` & `pegasusX-0.3.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'pegasusX',
   packages = find_packages(exclude=[]),
-  version = '0.3.0',
+  version = '0.3.1',
   license='MIT',
   description = 'pegasus - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/pegasus',
   keywords = [
```

