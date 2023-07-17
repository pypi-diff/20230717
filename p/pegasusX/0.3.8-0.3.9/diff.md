# Comparing `tmp/pegasusX-0.3.8.tar.gz` & `tmp/pegasusX-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pegasusX-0.3.8.tar", last modified: Mon Jul 17 17:53:55 2023, max compression
+gzip compressed data, was "pegasusX-0.3.9.tar", last modified: Mon Jul 17 18:44:01 2023, max compression
```

## Comparing `pegasusX-0.3.8.tar` & `pegasusX-0.3.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:53:55.181384 pegasusX-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 17:53:43.000000 pegasusX-0.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 17:53:55.181384 pegasusX-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9587 2023-07-17 17:53:43.000000 pegasusX-0.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:53:55.181384 pegasusX-0.3.8/pegasus/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:53:55.181384 pegasusX-0.3.8/pegasus/ImageBind/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-17 17:53:43.000000 pegasusX-0.3.8/pegasus/ImageBind/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11871 2023-07-17 17:53:43.000000 pegasusX-0.3.8/pegasus/ImageBind/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:53:55.181384 pegasusX-0.3.8/pegasus/ImageBind/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 17:53:43.000000 pegasusX-0.3.8/pegasus/ImageBind/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-07-17 17:53:43.000000 pegasusX-0.3.8/pegasus/ImageBind/models/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16431 2023-07-17 17:53:43.000000 pegasusX-0.3.8/pegasus/ImageBind/models/imagebind_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    23088 2023-07-17 17:53:43.000000 pegasusX-0.3.8/pegasus/ImageBind/models/multimodal_preprocessors.py
--rw-r--r--   0 runner    (1001) docker     (123)     9748 2023-07-17 17:53:43.000000 pegasusX-0.3.8/pegasus/ImageBind/models/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-17 17:53:43.000000 pegasusX-0.3.8/pegasus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-07-17 17:53:43.000000 pegasusX-0.3.8/pegasus/embedding_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-17 17:53:43.000000 pegasusX-0.3.8/pegasus/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-07-17 17:53:43.000000 pegasusX-0.3.8/pegasus/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-07-17 17:53:43.000000 pegasusX-0.3.8/pegasus/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:53:55.181384 pegasusX-0.3.8/pegasusX.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 17:53:55.000000 pegasusX-0.3.8/pegasusX.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-17 17:53:55.000000 pegasusX-0.3.8/pegasusX.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 17:53:55.000000 pegasusX-0.3.8/pegasusX.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-17 17:53:55.000000 pegasusX-0.3.8/pegasusX.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 17:53:55.000000 pegasusX-0.3.8/pegasusX.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 17:53:55.181384 pegasusX-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-17 17:53:43.000000 pegasusX-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:44:01.284704 pegasusX-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 18:43:50.000000 pegasusX-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 18:44:01.284704 pegasusX-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10816 2023-07-17 18:43:50.000000 pegasusX-0.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:44:01.280704 pegasusX-0.3.9/pegasus/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:44:01.280704 pegasusX-0.3.9/pegasus/ImageBind/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-17 18:43:50.000000 pegasusX-0.3.9/pegasus/ImageBind/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11871 2023-07-17 18:43:50.000000 pegasusX-0.3.9/pegasus/ImageBind/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:44:01.284704 pegasusX-0.3.9/pegasus/ImageBind/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:50.000000 pegasusX-0.3.9/pegasus/ImageBind/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-07-17 18:43:50.000000 pegasusX-0.3.9/pegasus/ImageBind/models/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16431 2023-07-17 18:43:50.000000 pegasusX-0.3.9/pegasus/ImageBind/models/imagebind_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23088 2023-07-17 18:43:50.000000 pegasusX-0.3.9/pegasus/ImageBind/models/multimodal_preprocessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9748 2023-07-17 18:43:50.000000 pegasusX-0.3.9/pegasus/ImageBind/models/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-17 18:43:50.000000 pegasusX-0.3.9/pegasus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-07-17 18:43:50.000000 pegasusX-0.3.9/pegasus/embedding_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-17 18:43:50.000000 pegasusX-0.3.9/pegasus/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-07-17 18:43:50.000000 pegasusX-0.3.9/pegasus/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-07-17 18:43:50.000000 pegasusX-0.3.9/pegasus/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:44:01.284704 pegasusX-0.3.9/pegasusX.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 18:44:01.000000 pegasusX-0.3.9/pegasusX.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-17 18:44:01.000000 pegasusX-0.3.9/pegasusX.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 18:44:01.000000 pegasusX-0.3.9/pegasusX.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-17 18:44:01.000000 pegasusX-0.3.9/pegasusX.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 18:44:01.000000 pegasusX-0.3.9/pegasusX.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 18:44:01.284704 pegasusX-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-17 18:43:50.000000 pegasusX-0.3.9/setup.py
```

### Comparing `pegasusX-0.3.8/LICENSE` & `pegasusX-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pegasusX-0.3.8/PKG-INFO` & `pegasusX-0.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pegasusX
-Version: 0.3.8
+Version: 0.3.9
 Summary: pegasus - Pytorch
 Home-page: https://github.com/kyegomez/pegasus
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pegasusX-0.3.8/README.md` & `pegasusX-0.3.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -31,25 +31,69 @@
 </div>
 
 
 Welcome to PegasusX, the latest and most advanced package for creating high-quality embeddings from multimodal data. We're pushing the boundaries of what's possible with machine learning, enabling tasks and applications that were once mere visions of the future.
 
 In essence, PegasusX is designed to transform the way we look at data. Our aim is to make it easier for anyone, regardless of their domain or discipline, to generate task-specific, high-quality embeddings from any type of data, be it text, image, video, audio, or even more complex data types..
 
+# Documentation
+* [Click here for documentation](DOCs/DOCUMENTATION.md)
 
 ## Installation
+
+Sure, here is the modified section including installation instructions using `git clone`:
+
+# Git Clone Installation
+
+There are 2 methods of installation. Currently, we're experiencing some path errors with pip installation. For a smooth installation, we recommend using git clone:
+
 ```bash
-pip install pegasusx
+git clone https://github.com/kyegomez/Pegasus.git
+cd Pegasus
+pip install -r requirements.txt
+```
+
+To validate your installation, you can run the provided example:
+
+```bash
+python3 example.py
 ```
 
 ## Usage
 
 ```python
 from pegasus import Pegasus
 
+# For video and audio modalities, you can initialize the Pegasus class with "Pegasus('vision')" or "Pegasus('audio')" respectively, then pass in the file path of the vision or audio data
+pegasus = Pegasus("text", multi_process=False, n_processes=4)
+
+text_data = [
+    'This is a query about artificial intelligence',
+    'Another query about machine learning',
+    'Yet another query about deep learning',
+    'And one more about natural language processing'
+]
+
+embeddings = pegasus.embed_data(text_data)
+
+print(embeddings)
+```
+
+## Pip Installation
+Please help us with this file path errors, they are very annoying.
+
+```bash
+pip install pegasusx
+```
+
+## Pip Usage
+
+```python
+from pegasus import Pegasus
+
 # for video, audio do "Pegasus('vision'), Pegasus("audio") respectively then pass in the file path of the vision or audio data
 pegasus = Pegasus("text", multi_process=False, n_processes=4)
 
 text_data = ['This is a query about artificial intelligence',
              'Another query about machine learning',
              'Yet another query about deep learning',
              'And one more about natural language processing']
```

### Comparing `pegasusX-0.3.8/pegasus/ImageBind/data.py` & `pegasusX-0.3.9/pegasus/ImageBind/data.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.3.8/pegasus/ImageBind/models/helpers.py` & `pegasusX-0.3.9/pegasus/ImageBind/models/helpers.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.3.8/pegasus/ImageBind/models/imagebind_model.py` & `pegasusX-0.3.9/pegasus/ImageBind/models/imagebind_model.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.3.8/pegasus/ImageBind/models/multimodal_preprocessors.py` & `pegasusX-0.3.9/pegasus/ImageBind/models/multimodal_preprocessors.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.3.8/pegasus/ImageBind/models/transformer.py` & `pegasusX-0.3.9/pegasus/ImageBind/models/transformer.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.3.8/pegasus/embedding_functions.py` & `pegasusX-0.3.9/pegasus/embedding_functions.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.3.8/pegasus/errors.py` & `pegasusX-0.3.9/pegasus/errors.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.3.8/pegasus/types.py` & `pegasusX-0.3.9/pegasus/types.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.3.8/pegasusX.egg-info/PKG-INFO` & `pegasusX-0.3.9/pegasusX.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pegasusX
-Version: 0.3.8
+Version: 0.3.9
 Summary: pegasus - Pytorch
 Home-page: https://github.com/kyegomez/pegasus
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pegasusX-0.3.8/pegasusX.egg-info/SOURCES.txt` & `pegasusX-0.3.9/pegasusX.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pegasusX-0.3.8/setup.py` & `pegasusX-0.3.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'pegasusX',
   packages = find_packages(exclude=[]),
-  version = '0.3.8',
+  version = '0.3.9',
   license='MIT',
   description = 'pegasus - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/pegasus',
   keywords = [
```

