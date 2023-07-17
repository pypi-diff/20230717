# Comparing `tmp/pegasusX-0.1.0.tar.gz` & `tmp/pegasusX-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pegasusX-0.1.0.tar", last modified: Mon Jul 17 03:42:10 2023, max compression
+gzip compressed data, was "pegasusX-0.1.1.tar", last modified: Mon Jul 17 03:46:16 2023, max compression
```

## Comparing `pegasusX-0.1.0.tar` & `pegasusX-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:42:10.549841 pegasusX-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 03:41:59.000000 pegasusX-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 03:42:10.549841 pegasusX-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-07-17 03:41:59.000000 pegasusX-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:42:10.549841 pegasusX-0.1.0/pegasusX.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 03:42:10.000000 pegasusX-0.1.0/pegasusX.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-17 03:42:10.000000 pegasusX-0.1.0/pegasusX.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 03:42:10.000000 pegasusX-0.1.0/pegasusX.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-17 03:42:10.000000 pegasusX-0.1.0/pegasusX.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 03:42:10.000000 pegasusX-0.1.0/pegasusX.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 03:42:10.549841 pegasusX-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-17 03:41:59.000000 pegasusX-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:46:16.546973 pegasusX-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 03:46:03.000000 pegasusX-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 03:46:16.546973 pegasusX-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-07-17 03:46:03.000000 pegasusX-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:46:16.546973 pegasusX-0.1.1/pegasus/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-17 03:46:03.000000 pegasusX-0.1.1/pegasus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-17 03:46:03.000000 pegasusX-0.1.1/pegasus/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:46:16.546973 pegasusX-0.1.1/pegasusX.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 03:46:16.000000 pegasusX-0.1.1/pegasusX.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-17 03:46:16.000000 pegasusX-0.1.1/pegasusX.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 03:46:16.000000 pegasusX-0.1.1/pegasusX.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-17 03:46:16.000000 pegasusX-0.1.1/pegasusX.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 03:46:16.000000 pegasusX-0.1.1/pegasusX.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 03:46:16.546973 pegasusX-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-17 03:46:03.000000 pegasusX-0.1.1/setup.py
```

### Comparing `pegasusX-0.1.0/LICENSE` & `pegasusX-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pegasusX-0.1.0/PKG-INFO` & `pegasusX-0.1.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pegasusX
-Version: 0.1.0
+Version: 0.1.1
 Summary: pegasus - Pytorch
 Home-page: https://github.com/kyegomez/pegasus
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pegasusX-0.1.0/README.md` & `pegasusX-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pegasusX-0.1.0/pegasusX.egg-info/PKG-INFO` & `pegasusX-0.1.1/pegasusX.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pegasusX
-Version: 0.1.0
+Version: 0.1.1
 Summary: pegasus - Pytorch
 Home-page: https://github.com/kyegomez/pegasus
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pegasusX-0.1.0/setup.py` & `pegasusX-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 # 
 
 setup(
   name = 'pegasusX',
   packages = find_packages(exclude=[]),
-  version = '0.1.0',
+  version = '0.1.1',
   license='MIT',
   description = 'pegasus - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/pegasus',
   keywords = [
```

