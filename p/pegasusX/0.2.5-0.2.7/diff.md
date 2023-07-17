# Comparing `tmp/pegasusX-0.2.5.tar.gz` & `tmp/pegasusX-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pegasusX-0.2.5.tar", last modified: Mon Jul 17 14:47:14 2023, max compression
+gzip compressed data, was "pegasusX-0.2.7.tar", last modified: Mon Jul 17 15:08:07 2023, max compression
```

## Comparing `pegasusX-0.2.5.tar` & `pegasusX-0.2.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:47:14.573933 pegasusX-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 14:47:01.000000 pegasusX-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 14:47:14.573933 pegasusX-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-07-17 14:47:01.000000 pegasusX-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:47:14.573933 pegasusX-0.2.5/pegasus/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:47:14.573933 pegasusX-0.2.5/pegasus/ImageBind/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-17 14:47:01.000000 pegasusX-0.2.5/pegasus/ImageBind/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11875 2023-07-17 14:47:01.000000 pegasusX-0.2.5/pegasus/ImageBind/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:47:14.573933 pegasusX-0.2.5/pegasus/ImageBind/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:47:01.000000 pegasusX-0.2.5/pegasus/ImageBind/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-07-17 14:47:01.000000 pegasusX-0.2.5/pegasus/ImageBind/models/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16431 2023-07-17 14:47:01.000000 pegasusX-0.2.5/pegasus/ImageBind/models/imagebind_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    23088 2023-07-17 14:47:01.000000 pegasusX-0.2.5/pegasus/ImageBind/models/multimodal_preprocessors.py
--rw-r--r--   0 runner    (1001) docker     (123)     9748 2023-07-17 14:47:01.000000 pegasusX-0.2.5/pegasus/ImageBind/models/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-17 14:47:01.000000 pegasusX-0.2.5/pegasus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-07-17 14:47:01.000000 pegasusX-0.2.5/pegasus/embedding_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-17 14:47:01.000000 pegasusX-0.2.5/pegasus/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-17 14:47:01.000000 pegasusX-0.2.5/pegasus/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-07-17 14:47:01.000000 pegasusX-0.2.5/pegasus/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:47:14.573933 pegasusX-0.2.5/pegasusX.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 14:47:14.000000 pegasusX-0.2.5/pegasusX.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-17 14:47:14.000000 pegasusX-0.2.5/pegasusX.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 14:47:14.000000 pegasusX-0.2.5/pegasusX.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-17 14:47:14.000000 pegasusX-0.2.5/pegasusX.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 14:47:14.000000 pegasusX-0.2.5/pegasusX.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 14:47:14.573933 pegasusX-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-17 14:47:01.000000 pegasusX-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:08:07.420718 pegasusX-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 15:07:53.000000 pegasusX-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 15:08:07.420718 pegasusX-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-07-17 15:07:53.000000 pegasusX-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:08:07.416718 pegasusX-0.2.7/pegasus/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:08:07.420718 pegasusX-0.2.7/pegasus/ImageBind/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-17 15:07:53.000000 pegasusX-0.2.7/pegasus/ImageBind/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11875 2023-07-17 15:07:53.000000 pegasusX-0.2.7/pegasus/ImageBind/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:08:07.420718 pegasusX-0.2.7/pegasus/ImageBind/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:07:53.000000 pegasusX-0.2.7/pegasus/ImageBind/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-07-17 15:07:53.000000 pegasusX-0.2.7/pegasus/ImageBind/models/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16431 2023-07-17 15:07:53.000000 pegasusX-0.2.7/pegasus/ImageBind/models/imagebind_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23088 2023-07-17 15:07:53.000000 pegasusX-0.2.7/pegasus/ImageBind/models/multimodal_preprocessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9748 2023-07-17 15:07:53.000000 pegasusX-0.2.7/pegasus/ImageBind/models/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-17 15:07:53.000000 pegasusX-0.2.7/pegasus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-07-17 15:07:53.000000 pegasusX-0.2.7/pegasus/embedding_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-17 15:07:53.000000 pegasusX-0.2.7/pegasus/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-17 15:07:53.000000 pegasusX-0.2.7/pegasus/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-07-17 15:07:53.000000 pegasusX-0.2.7/pegasus/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:08:07.420718 pegasusX-0.2.7/pegasusX.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 15:08:07.000000 pegasusX-0.2.7/pegasusX.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-17 15:08:07.000000 pegasusX-0.2.7/pegasusX.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 15:08:07.000000 pegasusX-0.2.7/pegasusX.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-17 15:08:07.000000 pegasusX-0.2.7/pegasusX.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 15:08:07.000000 pegasusX-0.2.7/pegasusX.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 15:08:07.420718 pegasusX-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-17 15:07:53.000000 pegasusX-0.2.7/setup.py
```

### Comparing `pegasusX-0.2.5/LICENSE` & `pegasusX-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pegasusX-0.2.5/PKG-INFO` & `pegasusX-0.2.7/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pegasusX
-Version: 0.2.5
+Version: 0.2.7
 Summary: pegasus - Pytorch
 Home-page: https://github.com/kyegomez/pegasus
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pegasusX-0.2.5/README.md` & `pegasusX-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `pegasusX-0.2.5/pegasus/ImageBind/data.py` & `pegasusX-0.2.7/pegasus/ImageBind/data.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.2.5/pegasus/ImageBind/models/helpers.py` & `pegasusX-0.2.7/pegasus/ImageBind/models/helpers.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.2.5/pegasus/ImageBind/models/imagebind_model.py` & `pegasusX-0.2.7/pegasus/ImageBind/models/imagebind_model.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.2.5/pegasus/ImageBind/models/multimodal_preprocessors.py` & `pegasusX-0.2.7/pegasus/ImageBind/models/multimodal_preprocessors.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.2.5/pegasus/ImageBind/models/transformer.py` & `pegasusX-0.2.7/pegasus/ImageBind/models/transformer.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.2.5/pegasus/embedding_functions.py` & `pegasusX-0.2.7/pegasus/embedding_functions.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.2.5/pegasus/errors.py` & `pegasusX-0.2.7/pegasus/errors.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.2.5/pegasus/main.py` & `pegasusX-0.2.7/pegasus/main.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.2.5/pegasus/types.py` & `pegasusX-0.2.7/pegasus/types.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.2.5/pegasusX.egg-info/PKG-INFO` & `pegasusX-0.2.7/pegasusX.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pegasusX
-Version: 0.2.5
+Version: 0.2.7
 Summary: pegasus - Pytorch
 Home-page: https://github.com/kyegomez/pegasus
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pegasusX-0.2.5/pegasusX.egg-info/SOURCES.txt` & `pegasusX-0.2.7/pegasusX.egg-info/SOURCES.txt`

 * *Files identical despite different names*

