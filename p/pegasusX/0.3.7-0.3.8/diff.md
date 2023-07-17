# Comparing `tmp/pegasusX-0.3.7.tar.gz` & `tmp/pegasusX-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pegasusX-0.3.7.tar", last modified: Mon Jul 17 17:07:37 2023, max compression
+gzip compressed data, was "pegasusX-0.3.8.tar", last modified: Mon Jul 17 17:53:55 2023, max compression
```

## Comparing `pegasusX-0.3.7.tar` & `pegasusX-0.3.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:07:37.487515 pegasusX-0.3.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 17:07:26.000000 pegasusX-0.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 17:07:37.487515 pegasusX-0.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9587 2023-07-17 17:07:26.000000 pegasusX-0.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:07:37.483515 pegasusX-0.3.7/pegasus/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:07:37.487515 pegasusX-0.3.7/pegasus/ImageBind/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-17 17:07:26.000000 pegasusX-0.3.7/pegasus/ImageBind/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11871 2023-07-17 17:07:26.000000 pegasusX-0.3.7/pegasus/ImageBind/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:07:37.487515 pegasusX-0.3.7/pegasus/ImageBind/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 17:07:26.000000 pegasusX-0.3.7/pegasus/ImageBind/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-07-17 17:07:26.000000 pegasusX-0.3.7/pegasus/ImageBind/models/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16431 2023-07-17 17:07:26.000000 pegasusX-0.3.7/pegasus/ImageBind/models/imagebind_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    23088 2023-07-17 17:07:26.000000 pegasusX-0.3.7/pegasus/ImageBind/models/multimodal_preprocessors.py
--rw-r--r--   0 runner    (1001) docker     (123)     9748 2023-07-17 17:07:26.000000 pegasusX-0.3.7/pegasus/ImageBind/models/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-17 17:07:26.000000 pegasusX-0.3.7/pegasus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-07-17 17:07:26.000000 pegasusX-0.3.7/pegasus/embedding_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-17 17:07:26.000000 pegasusX-0.3.7/pegasus/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-17 17:07:26.000000 pegasusX-0.3.7/pegasus/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-07-17 17:07:26.000000 pegasusX-0.3.7/pegasus/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:07:37.487515 pegasusX-0.3.7/pegasusX.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 17:07:37.000000 pegasusX-0.3.7/pegasusX.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-17 17:07:37.000000 pegasusX-0.3.7/pegasusX.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 17:07:37.000000 pegasusX-0.3.7/pegasusX.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-17 17:07:37.000000 pegasusX-0.3.7/pegasusX.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 17:07:37.000000 pegasusX-0.3.7/pegasusX.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 17:07:37.487515 pegasusX-0.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-17 17:07:26.000000 pegasusX-0.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:53:55.181384 pegasusX-0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 17:53:43.000000 pegasusX-0.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 17:53:55.181384 pegasusX-0.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9587 2023-07-17 17:53:43.000000 pegasusX-0.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:53:55.181384 pegasusX-0.3.8/pegasus/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:53:55.181384 pegasusX-0.3.8/pegasus/ImageBind/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-17 17:53:43.000000 pegasusX-0.3.8/pegasus/ImageBind/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11871 2023-07-17 17:53:43.000000 pegasusX-0.3.8/pegasus/ImageBind/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:53:55.181384 pegasusX-0.3.8/pegasus/ImageBind/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 17:53:43.000000 pegasusX-0.3.8/pegasus/ImageBind/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-07-17 17:53:43.000000 pegasusX-0.3.8/pegasus/ImageBind/models/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16431 2023-07-17 17:53:43.000000 pegasusX-0.3.8/pegasus/ImageBind/models/imagebind_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23088 2023-07-17 17:53:43.000000 pegasusX-0.3.8/pegasus/ImageBind/models/multimodal_preprocessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9748 2023-07-17 17:53:43.000000 pegasusX-0.3.8/pegasus/ImageBind/models/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-17 17:53:43.000000 pegasusX-0.3.8/pegasus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-07-17 17:53:43.000000 pegasusX-0.3.8/pegasus/embedding_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-17 17:53:43.000000 pegasusX-0.3.8/pegasus/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-07-17 17:53:43.000000 pegasusX-0.3.8/pegasus/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-07-17 17:53:43.000000 pegasusX-0.3.8/pegasus/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:53:55.181384 pegasusX-0.3.8/pegasusX.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 17:53:55.000000 pegasusX-0.3.8/pegasusX.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-17 17:53:55.000000 pegasusX-0.3.8/pegasusX.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 17:53:55.000000 pegasusX-0.3.8/pegasusX.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-17 17:53:55.000000 pegasusX-0.3.8/pegasusX.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 17:53:55.000000 pegasusX-0.3.8/pegasusX.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 17:53:55.181384 pegasusX-0.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-17 17:53:43.000000 pegasusX-0.3.8/setup.py
```

### Comparing `pegasusX-0.3.7/LICENSE` & `pegasusX-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pegasusX-0.3.7/PKG-INFO` & `pegasusX-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pegasusX
-Version: 0.3.7
+Version: 0.3.8
 Summary: pegasus - Pytorch
 Home-page: https://github.com/kyegomez/pegasus
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pegasusX-0.3.7/README.md` & `pegasusX-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `pegasusX-0.3.7/pegasus/ImageBind/data.py` & `pegasusX-0.3.8/pegasus/ImageBind/data.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.3.7/pegasus/ImageBind/models/helpers.py` & `pegasusX-0.3.8/pegasus/ImageBind/models/helpers.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.3.7/pegasus/ImageBind/models/imagebind_model.py` & `pegasusX-0.3.8/pegasus/ImageBind/models/imagebind_model.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.3.7/pegasus/ImageBind/models/multimodal_preprocessors.py` & `pegasusX-0.3.8/pegasus/ImageBind/models/multimodal_preprocessors.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.3.7/pegasus/ImageBind/models/transformer.py` & `pegasusX-0.3.8/pegasus/ImageBind/models/transformer.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.3.7/pegasus/embedding_functions.py` & `pegasusX-0.3.8/pegasus/embedding_functions.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.3.7/pegasus/errors.py` & `pegasusX-0.3.8/pegasus/errors.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.3.7/pegasus/types.py` & `pegasusX-0.3.8/pegasus/types.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.3.7/pegasusX.egg-info/PKG-INFO` & `pegasusX-0.3.8/pegasusX.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pegasusX
-Version: 0.3.7
+Version: 0.3.8
 Summary: pegasus - Pytorch
 Home-page: https://github.com/kyegomez/pegasus
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pegasusX-0.3.7/pegasusX.egg-info/SOURCES.txt` & `pegasusX-0.3.8/pegasusX.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pegasusX-0.3.7/setup.py` & `pegasusX-0.3.8/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'pegasusX',
   packages = find_packages(exclude=[]),
-  version = '0.3.7',
+  version = '0.3.8',
   license='MIT',
   description = 'pegasus - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/pegasus',
   keywords = [
```

