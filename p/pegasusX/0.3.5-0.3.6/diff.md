# Comparing `tmp/pegasusX-0.3.5.tar.gz` & `tmp/pegasusX-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pegasusX-0.3.5.tar", last modified: Mon Jul 17 16:35:25 2023, max compression
+gzip compressed data, was "pegasusX-0.3.6.tar", last modified: Mon Jul 17 16:55:50 2023, max compression
```

## Comparing `pegasusX-0.3.5.tar` & `pegasusX-0.3.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:35:25.491962 pegasusX-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 16:35:11.000000 pegasusX-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 16:35:25.491962 pegasusX-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9587 2023-07-17 16:35:11.000000 pegasusX-0.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:35:25.487962 pegasusX-0.3.5/pegasus/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:35:25.487962 pegasusX-0.3.5/pegasus/ImageBind/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-17 16:35:11.000000 pegasusX-0.3.5/pegasus/ImageBind/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11863 2023-07-17 16:35:11.000000 pegasusX-0.3.5/pegasus/ImageBind/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:35:25.491962 pegasusX-0.3.5/pegasus/ImageBind/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 16:35:11.000000 pegasusX-0.3.5/pegasus/ImageBind/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-07-17 16:35:11.000000 pegasusX-0.3.5/pegasus/ImageBind/models/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16431 2023-07-17 16:35:11.000000 pegasusX-0.3.5/pegasus/ImageBind/models/imagebind_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    23088 2023-07-17 16:35:11.000000 pegasusX-0.3.5/pegasus/ImageBind/models/multimodal_preprocessors.py
--rw-r--r--   0 runner    (1001) docker     (123)     9748 2023-07-17 16:35:11.000000 pegasusX-0.3.5/pegasus/ImageBind/models/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-17 16:35:11.000000 pegasusX-0.3.5/pegasus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-17 16:35:11.000000 pegasusX-0.3.5/pegasus/embedding_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-17 16:35:11.000000 pegasusX-0.3.5/pegasus/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-17 16:35:11.000000 pegasusX-0.3.5/pegasus/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-07-17 16:35:11.000000 pegasusX-0.3.5/pegasus/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:35:25.491962 pegasusX-0.3.5/pegasusX.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 16:35:25.000000 pegasusX-0.3.5/pegasusX.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-17 16:35:25.000000 pegasusX-0.3.5/pegasusX.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 16:35:25.000000 pegasusX-0.3.5/pegasusX.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-17 16:35:25.000000 pegasusX-0.3.5/pegasusX.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 16:35:25.000000 pegasusX-0.3.5/pegasusX.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 16:35:25.491962 pegasusX-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-17 16:35:11.000000 pegasusX-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:55:50.442108 pegasusX-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 16:55:32.000000 pegasusX-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 16:55:50.442108 pegasusX-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9587 2023-07-17 16:55:32.000000 pegasusX-0.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:55:50.438108 pegasusX-0.3.6/pegasus/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:55:50.438108 pegasusX-0.3.6/pegasus/ImageBind/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-17 16:55:32.000000 pegasusX-0.3.6/pegasus/ImageBind/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-07-17 16:55:32.000000 pegasusX-0.3.6/pegasus/ImageBind/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:55:50.442108 pegasusX-0.3.6/pegasus/ImageBind/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 16:55:32.000000 pegasusX-0.3.6/pegasus/ImageBind/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-07-17 16:55:32.000000 pegasusX-0.3.6/pegasus/ImageBind/models/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16431 2023-07-17 16:55:32.000000 pegasusX-0.3.6/pegasus/ImageBind/models/imagebind_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23088 2023-07-17 16:55:32.000000 pegasusX-0.3.6/pegasus/ImageBind/models/multimodal_preprocessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9748 2023-07-17 16:55:32.000000 pegasusX-0.3.6/pegasus/ImageBind/models/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-17 16:55:32.000000 pegasusX-0.3.6/pegasus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-07-17 16:55:32.000000 pegasusX-0.3.6/pegasus/embedding_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-17 16:55:32.000000 pegasusX-0.3.6/pegasus/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-17 16:55:32.000000 pegasusX-0.3.6/pegasus/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-07-17 16:55:32.000000 pegasusX-0.3.6/pegasus/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:55:50.442108 pegasusX-0.3.6/pegasusX.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 16:55:50.000000 pegasusX-0.3.6/pegasusX.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-17 16:55:50.000000 pegasusX-0.3.6/pegasusX.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 16:55:50.000000 pegasusX-0.3.6/pegasusX.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-17 16:55:50.000000 pegasusX-0.3.6/pegasusX.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 16:55:50.000000 pegasusX-0.3.6/pegasusX.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 16:55:50.442108 pegasusX-0.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-17 16:55:32.000000 pegasusX-0.3.6/setup.py
```

### Comparing `pegasusX-0.3.5/LICENSE` & `pegasusX-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pegasusX-0.3.5/PKG-INFO` & `pegasusX-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pegasusX
-Version: 0.3.5
+Version: 0.3.6
 Summary: pegasus - Pytorch
 Home-page: https://github.com/kyegomez/pegasus
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pegasusX-0.3.5/README.md` & `pegasusX-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `pegasusX-0.3.5/pegasus/ImageBind/data.py` & `pegasusX-0.3.6/pegasus/ImageBind/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from pytorchvideo.data.encoded_video import EncodedVideo
 
 from torchvision import transforms
 from torchvision.transforms._transforms_video import NormalizeVideo
 
 DEFAULT_AUDIO_FRAME_SHIFT_MS = 10  # in milliseconds
 
-BPE_PATH = "./ImageBind/bpe_simple_vocab_16e6.txt.gz"
+BPE_PATH = "./bpe_simple_vocab_16e6.txt.gz"
 
 
 def waveform2melspec(waveform, sample_rate, num_mel_bins, target_length):
     # Based on https://github.com/YuanGongND/ast/blob/d7d8b4b8e06cdaeb6c843cdb38794c1c7692234c/src/dataloader.py#L102
     waveform -= waveform.mean()
     fbank = torchaudio.compliance.kaldi.fbank(
         waveform,
```

### Comparing `pegasusX-0.3.5/pegasus/ImageBind/models/helpers.py` & `pegasusX-0.3.6/pegasus/ImageBind/models/helpers.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.3.5/pegasus/ImageBind/models/imagebind_model.py` & `pegasusX-0.3.6/pegasus/ImageBind/models/imagebind_model.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.3.5/pegasus/ImageBind/models/multimodal_preprocessors.py` & `pegasusX-0.3.6/pegasus/ImageBind/models/multimodal_preprocessors.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.3.5/pegasus/ImageBind/models/transformer.py` & `pegasusX-0.3.6/pegasus/ImageBind/models/transformer.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.3.5/pegasus/errors.py` & `pegasusX-0.3.6/pegasus/errors.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.3.5/pegasus/main.py` & `pegasusX-0.3.6/pegasus/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,8 +28,10 @@
             data = np.array(data)
         
         if not self.multi_process:
             return self._embed_data(data)
         
         with ProcessPoolExecutor(max_workers=self.n_processes) as executor:
             future_to_data = {executor.submit(self._embed_data, d): d for d in data}
-            return {future_to_data[future]: future.result() for future in as_completed(future_to_data)}
+            return {future_to_data[future]: future.result() for future in as_completed(future_to_data)}
+        
+
```

### Comparing `pegasusX-0.3.5/pegasus/types.py` & `pegasusX-0.3.6/pegasus/types.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.3.5/pegasusX.egg-info/PKG-INFO` & `pegasusX-0.3.6/pegasusX.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pegasusX
-Version: 0.3.5
+Version: 0.3.6
 Summary: pegasus - Pytorch
 Home-page: https://github.com/kyegomez/pegasus
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pegasusX-0.3.5/pegasusX.egg-info/SOURCES.txt` & `pegasusX-0.3.6/pegasusX.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pegasusX-0.3.5/setup.py` & `pegasusX-0.3.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'pegasusX',
   packages = find_packages(exclude=[]),
-  version = '0.3.5',
+  version = '0.3.6',
   license='MIT',
   description = 'pegasus - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/pegasus',
   keywords = [
```

