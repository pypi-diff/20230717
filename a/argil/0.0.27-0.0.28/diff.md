# Comparing `tmp/argil-0.0.27.tar.gz` & `tmp/argil-0.0.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argil-0.0.27.tar", last modified: Mon Jul 17 05:25:34 2023, max compression
+gzip compressed data, was "argil-0.0.28.tar", last modified: Mon Jul 17 05:28:30 2023, max compression
```

## Comparing `argil-0.0.27.tar` & `argil-0.0.28.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2023-07-17 05:25:34.905725 argil-0.0.27/
--rw-rw-r--   0 charles   (1000) charles   (1000)    34600 2023-07-05 16:58:03.000000 argil-0.0.27/LICENCE.md
--rw-rw-r--   0 charles   (1000) charles   (1000)       26 2023-07-17 05:18:04.000000 argil-0.0.27/MANIFEST.in
--rw-rw-r--   0 charles   (1000) charles   (1000)     1255 2023-07-17 05:25:34.905725 argil-0.0.27/PKG-INFO
--rw-rw-r--   0 charles   (1000) charles   (1000)      655 2023-07-05 16:40:12.000000 argil-0.0.27/README.md
-drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2023-07-17 05:25:34.905725 argil-0.0.27/argil/
--rw-rw-r--   0 charles   (1000) charles   (1000)      251 2023-07-05 16:40:12.000000 argil-0.0.27/argil/__init__.py
--rw-rw-r--   0 charles   (1000) charles   (1000)       38 2023-07-05 17:08:31.000000 argil-0.0.27/argil/config.json
--rw-rw-r--   0 charles   (1000) charles   (1000)      197 2023-07-17 05:06:16.000000 argil-0.0.27/argil/types.py
--rw-rw-r--   0 charles   (1000) charles   (1000)      910 2023-07-17 05:24:53.000000 argil-0.0.27/argil/workflowRuns.py
--rw-rw-r--   0 charles   (1000) charles   (1000)      646 2023-07-17 05:24:43.000000 argil-0.0.27/argil/workflows.py
-drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2023-07-17 05:25:34.905725 argil-0.0.27/argil.egg-info/
--rw-rw-r--   0 charles   (1000) charles   (1000)     1255 2023-07-17 05:25:34.000000 argil-0.0.27/argil.egg-info/PKG-INFO
--rw-rw-r--   0 charles   (1000) charles   (1000)      277 2023-07-17 05:25:34.000000 argil-0.0.27/argil.egg-info/SOURCES.txt
--rw-rw-r--   0 charles   (1000) charles   (1000)        1 2023-07-17 05:25:34.000000 argil-0.0.27/argil.egg-info/dependency_links.txt
--rw-rw-r--   0 charles   (1000) charles   (1000)        9 2023-07-17 05:25:34.000000 argil-0.0.27/argil.egg-info/requires.txt
--rw-rw-r--   0 charles   (1000) charles   (1000)        6 2023-07-17 05:25:34.000000 argil-0.0.27/argil.egg-info/top_level.txt
--rw-rw-r--   0 charles   (1000) charles   (1000)       38 2023-07-17 05:25:34.905725 argil-0.0.27/setup.cfg
--rw-rw-r--   0 charles   (1000) charles   (1000)     1197 2023-07-17 05:25:24.000000 argil-0.0.27/setup.py
+drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2023-07-17 05:28:30.144377 argil-0.0.28/
+-rw-rw-r--   0 charles   (1000) charles   (1000)    34600 2023-07-05 16:58:03.000000 argil-0.0.28/LICENCE.md
+-rw-rw-r--   0 charles   (1000) charles   (1000)       26 2023-07-17 05:18:04.000000 argil-0.0.28/MANIFEST.in
+-rw-rw-r--   0 charles   (1000) charles   (1000)     1255 2023-07-17 05:28:30.144377 argil-0.0.28/PKG-INFO
+-rw-rw-r--   0 charles   (1000) charles   (1000)      655 2023-07-05 16:40:12.000000 argil-0.0.28/README.md
+drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2023-07-17 05:28:30.144377 argil-0.0.28/argil/
+-rw-rw-r--   0 charles   (1000) charles   (1000)      251 2023-07-05 16:40:12.000000 argil-0.0.28/argil/__init__.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)       38 2023-07-05 17:08:31.000000 argil-0.0.28/argil/config.json
+-rw-rw-r--   0 charles   (1000) charles   (1000)      197 2023-07-17 05:06:16.000000 argil-0.0.28/argil/types.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)      792 2023-07-17 05:28:04.000000 argil-0.0.28/argil/workflowRuns.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)      646 2023-07-17 05:28:00.000000 argil-0.0.28/argil/workflows.py
+drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2023-07-17 05:28:30.144377 argil-0.0.28/argil.egg-info/
+-rw-rw-r--   0 charles   (1000) charles   (1000)     1255 2023-07-17 05:28:30.000000 argil-0.0.28/argil.egg-info/PKG-INFO
+-rw-rw-r--   0 charles   (1000) charles   (1000)      277 2023-07-17 05:28:30.000000 argil-0.0.28/argil.egg-info/SOURCES.txt
+-rw-rw-r--   0 charles   (1000) charles   (1000)        1 2023-07-17 05:28:30.000000 argil-0.0.28/argil.egg-info/dependency_links.txt
+-rw-rw-r--   0 charles   (1000) charles   (1000)        9 2023-07-17 05:28:30.000000 argil-0.0.28/argil.egg-info/requires.txt
+-rw-rw-r--   0 charles   (1000) charles   (1000)        6 2023-07-17 05:28:30.000000 argil-0.0.28/argil.egg-info/top_level.txt
+-rw-rw-r--   0 charles   (1000) charles   (1000)       38 2023-07-17 05:28:30.144377 argil-0.0.28/setup.cfg
+-rw-rw-r--   0 charles   (1000) charles   (1000)     1197 2023-07-17 05:28:13.000000 argil-0.0.28/setup.py
```

### Comparing `argil-0.0.27/LICENCE.md` & `argil-0.0.28/LICENCE.md`

 * *Files identical despite different names*

### Comparing `argil-0.0.27/PKG-INFO` & `argil-0.0.28/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argil
-Version: 0.0.27
+Version: 0.0.28
 Summary: SDK for the Argil API
 Home-page: https://github.com/argildotai/argil-sdk-python
 Author: Brivael Le Pogam
 Author-email: briva@argil.ai
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `argil-0.0.27/README.md` & `argil-0.0.28/README.md`

 * *Files identical despite different names*

### Comparing `argil-0.0.27/argil/workflows.py` & `argil-0.0.28/argil/workflows.py`

 * *Files identical despite different names*

### Comparing `argil-0.0.27/argil.egg-info/PKG-INFO` & `argil-0.0.28/argil.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argil
-Version: 0.0.27
+Version: 0.0.28
 Summary: SDK for the Argil API
 Home-page: https://github.com/argildotai/argil-sdk-python
 Author: Brivael Le Pogam
 Author-email: briva@argil.ai
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `argil-0.0.27/setup.py` & `argil-0.0.28/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\\n" + fh.read()
 
 setup(
     name='argil',
-    version='0.0.27',#'{{VERSION_PLACEHOLDER}}',
+    version='0.0.28',#'{{VERSION_PLACEHOLDER}}',
     author="Brivael Le Pogam",
     author_email="briva@argil.ai",
     description='SDK for the Argil API',
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url='https://github.com/argildotai/argil-sdk-python',
     packages=find_packages(),
```

