# Comparing `tmp/pegasusX-0.2.7.tar.gz` & `tmp/pegasusX-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pegasusX-0.2.7.tar", last modified: Mon Jul 17 15:08:07 2023, max compression
+gzip compressed data, was "pegasusX-0.2.9.tar", last modified: Mon Jul 17 15:47:15 2023, max compression
```

## Comparing `pegasusX-0.2.7.tar` & `pegasusX-0.2.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:08:07.420718 pegasusX-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 15:07:53.000000 pegasusX-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 15:08:07.420718 pegasusX-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-07-17 15:07:53.000000 pegasusX-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:08:07.416718 pegasusX-0.2.7/pegasus/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:08:07.420718 pegasusX-0.2.7/pegasus/ImageBind/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-17 15:07:53.000000 pegasusX-0.2.7/pegasus/ImageBind/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11875 2023-07-17 15:07:53.000000 pegasusX-0.2.7/pegasus/ImageBind/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:08:07.420718 pegasusX-0.2.7/pegasus/ImageBind/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:07:53.000000 pegasusX-0.2.7/pegasus/ImageBind/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-07-17 15:07:53.000000 pegasusX-0.2.7/pegasus/ImageBind/models/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16431 2023-07-17 15:07:53.000000 pegasusX-0.2.7/pegasus/ImageBind/models/imagebind_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    23088 2023-07-17 15:07:53.000000 pegasusX-0.2.7/pegasus/ImageBind/models/multimodal_preprocessors.py
--rw-r--r--   0 runner    (1001) docker     (123)     9748 2023-07-17 15:07:53.000000 pegasusX-0.2.7/pegasus/ImageBind/models/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-17 15:07:53.000000 pegasusX-0.2.7/pegasus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-07-17 15:07:53.000000 pegasusX-0.2.7/pegasus/embedding_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-17 15:07:53.000000 pegasusX-0.2.7/pegasus/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-17 15:07:53.000000 pegasusX-0.2.7/pegasus/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-07-17 15:07:53.000000 pegasusX-0.2.7/pegasus/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:08:07.420718 pegasusX-0.2.7/pegasusX.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 15:08:07.000000 pegasusX-0.2.7/pegasusX.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-17 15:08:07.000000 pegasusX-0.2.7/pegasusX.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 15:08:07.000000 pegasusX-0.2.7/pegasusX.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-17 15:08:07.000000 pegasusX-0.2.7/pegasusX.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 15:08:07.000000 pegasusX-0.2.7/pegasusX.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 15:08:07.420718 pegasusX-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-17 15:07:53.000000 pegasusX-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:47:15.791410 pegasusX-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 15:47:00.000000 pegasusX-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 15:47:15.791410 pegasusX-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9510 2023-07-17 15:47:00.000000 pegasusX-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:47:15.787410 pegasusX-0.2.9/pegasus/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:47:15.791410 pegasusX-0.2.9/pegasus/ImageBind/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-17 15:47:00.000000 pegasusX-0.2.9/pegasus/ImageBind/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11875 2023-07-17 15:47:00.000000 pegasusX-0.2.9/pegasus/ImageBind/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:47:15.791410 pegasusX-0.2.9/pegasus/ImageBind/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:47:00.000000 pegasusX-0.2.9/pegasus/ImageBind/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-07-17 15:47:00.000000 pegasusX-0.2.9/pegasus/ImageBind/models/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16431 2023-07-17 15:47:00.000000 pegasusX-0.2.9/pegasus/ImageBind/models/imagebind_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23088 2023-07-17 15:47:00.000000 pegasusX-0.2.9/pegasus/ImageBind/models/multimodal_preprocessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9748 2023-07-17 15:47:00.000000 pegasusX-0.2.9/pegasus/ImageBind/models/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-17 15:47:00.000000 pegasusX-0.2.9/pegasus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-07-17 15:47:00.000000 pegasusX-0.2.9/pegasus/embedding_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-17 15:47:00.000000 pegasusX-0.2.9/pegasus/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-17 15:47:00.000000 pegasusX-0.2.9/pegasus/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-07-17 15:47:00.000000 pegasusX-0.2.9/pegasus/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:47:15.791410 pegasusX-0.2.9/pegasusX.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 15:47:15.000000 pegasusX-0.2.9/pegasusX.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-17 15:47:15.000000 pegasusX-0.2.9/pegasusX.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 15:47:15.000000 pegasusX-0.2.9/pegasusX.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-17 15:47:15.000000 pegasusX-0.2.9/pegasusX.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 15:47:15.000000 pegasusX-0.2.9/pegasusX.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 15:47:15.791410 pegasusX-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-17 15:47:00.000000 pegasusX-0.2.9/setup.py
```

### Comparing `pegasusX-0.2.7/LICENSE` & `pegasusX-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pegasusX-0.2.7/PKG-INFO` & `pegasusX-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pegasusX
-Version: 0.2.7
+Version: 0.2.9
 Summary: pegasus - Pytorch
 Home-page: https://github.com/kyegomez/pegasus
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pegasusX-0.2.7/README.md` & `pegasusX-0.2.9/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,36 @@
 # PegasusX: The Future of Multimodal Embeddings 🦄 🦄 
 
-![Pegasus Banner](./assets/banner.png)
+<div align="center">
+
+[![GitHub issues](https://img.shields.io/github/issues/kyegomez/Pegasus)](https://github.com/kyegomez/Pegasus/issues)
+[![GitHub forks](https://img.shields.io/github/forks/kyegomez/Pegasus)](https://github.com/kyegomez/Pegasus/network)
+[![GitHub stars](https://img.shields.io/github/stars/kyegomez/Pegasus)](https://github.com/kyegomez/Pegasus/stargazers)
+[![GitHub license](https://img.shields.io/github/license/kyegomez/Pegasus)](https://github.com/kyegomez/Pegasus/blob/main/LICENSE)
+[![GitHub star chart](https://img.shields.io/github/stars/kyegomez/Pegasus?style=social)](https://star-history.com/#kyegomez/Pegasus)
+[![Dependency Status](https://img.shields.io/librariesio/github/kyegomez/Pegasus)](https://libraries.io/github/kyegomez/Pegasus)
+[![Downloads](https://static.pepy.tech/badge/pegasusx/month)](https://pepy.tech/project/pegasusx)
+
+### Share on Social Media
+
+[![Twitter](https://img.shields.io/twitter/url?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2FPegasus)](https://twitter.com/intent/tweet?text=Check%20out%20this%20amazing%20project%20on%20GitHub%3A%20&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2FPegasus)
+[![Facebook](https://img.shields.io/badge/Share-Facebook-blue)](https://www.facebook.com/sharer/sharer.php?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2FPegasus)
+[![LinkedIn](https://img.shields.io/badge/Share-LinkedIn-blue)](https://www.linkedin.com/shareArticle?mini=true&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2FPegasus&title=&summary=&source=)
+[![Reddit](https://img.shields.io/badge/-Share%20on%20Reddit-orange)](https://www.reddit.com/submit?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2FPegasus&title=PegasusX%20-%20The%20Future%20of%20Multimodal%20Embeddings)
+[![Hacker News](https://img.shields.io/badge/-Share%20on%20Hacker%20News-orange)](https://news.ycombinator.com/submitlink?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2FPegasus&t=PegasusX%20-%20The%20Future%20of%20Multimodal%20Embeddings)
+[![Pinterest](https://img.shields.io/badge/-Share%20on%20Pinterest-red)](https://pinterest.com/pin/create/button/?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2FPegasus&media=https%3A%2F%2Fexample.com%2Fimage.jpg&description=PegasusX%20-%20The%20Future%20of%20Multimodal%20Embeddings)
+[![WhatsApp](https://img.shields.io/badge/-Share%20on%20WhatsApp-green)](https://api.whatsapp.com/send?text=Check%20out%20PegasusX%20-%20The%20Future%20of%20Multimodal%20Embeddings%20%23Pegasus%20%23AI%0A%0Ahttps%3A%2F%2Fgithub.com%2Fkyegomez%2FPegasus)
+
+</div>
+
 
 Welcome to PegasusX, the latest and most advanced package for creating high-quality embeddings from multimodal data. We're pushing the boundaries of what's possible with machine learning, enabling tasks and applications that were once mere visions of the future.
 
-In essence, PegasusX is designed to transform the way we look at data. Our aim is to make it easier for anyone, regardless of their domain or discipline, to generate task-specific, high-quality embeddings from any type of data, be it text, image, video, audio, or even more complex data types.
+In essence, PegasusX is designed to transform the way we look at data. Our aim is to make it easier for anyone, regardless of their domain or discipline, to generate task-specific, high-quality embeddings from any type of data, be it text, image, video, audio, or even more complex data types..
+
 
 ## Installation
 ```bash
 pip install pegasusx
 ```
 
 ## Usage
```

### Comparing `pegasusX-0.2.7/pegasus/ImageBind/data.py` & `pegasusX-0.2.9/pegasus/ImageBind/data.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.2.7/pegasus/ImageBind/models/helpers.py` & `pegasusX-0.2.9/pegasus/ImageBind/models/helpers.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.2.7/pegasus/ImageBind/models/imagebind_model.py` & `pegasusX-0.2.9/pegasus/ImageBind/models/imagebind_model.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.2.7/pegasus/ImageBind/models/multimodal_preprocessors.py` & `pegasusX-0.2.9/pegasus/ImageBind/models/multimodal_preprocessors.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.2.7/pegasus/ImageBind/models/transformer.py` & `pegasusX-0.2.9/pegasus/ImageBind/models/transformer.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.2.7/pegasus/embedding_functions.py` & `pegasusX-0.2.9/pegasus/embedding_functions.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.2.7/pegasus/errors.py` & `pegasusX-0.2.9/pegasus/errors.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.2.7/pegasus/main.py` & `pegasusX-0.2.9/pegasus/main.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.2.7/pegasus/types.py` & `pegasusX-0.2.9/pegasus/types.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.2.7/pegasusX.egg-info/PKG-INFO` & `pegasusX-0.2.9/pegasusX.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pegasusX
-Version: 0.2.7
+Version: 0.2.9
 Summary: pegasus - Pytorch
 Home-page: https://github.com/kyegomez/pegasus
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pegasusX-0.2.7/pegasusX.egg-info/SOURCES.txt` & `pegasusX-0.2.9/pegasusX.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pegasusX-0.2.7/setup.py` & `pegasusX-0.2.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'pegasusX',
   packages = find_packages(exclude=[]),
-  version = '0.2.7',
+  version = '0.2.9',
   license='MIT',
   description = 'pegasus - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/pegasus',
   keywords = [
@@ -23,14 +23,15 @@
     'requests==2.28.1',
     'typing_extensions==4.5.0',
     'uvicorn[standard]==0.18.3',
     'torch',
     'torchvision',
     'torchaudio',
     'timm==0.6.7',
+    'pytorchvideo',
     'ftfy',
     'regex',
     'einops',
     'fvcore',
     'decord==0.6.0',
     'numba',
     'joblib',
```

