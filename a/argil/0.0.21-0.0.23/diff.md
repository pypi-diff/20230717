# Comparing `tmp/argil-0.0.21.tar.gz` & `tmp/argil-0.0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argil-0.0.21.tar", last modified: Mon Jul 17 04:59:43 2023, max compression
+gzip compressed data, was "argil-0.0.23.tar", last modified: Mon Jul 17 05:06:41 2023, max compression
```

## Comparing `argil-0.0.21.tar` & `argil-0.0.23.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2023-07-17 04:59:43.656138 argil-0.0.21/
--rw-rw-r--   0 charles   (1000) charles   (1000)    34600 2023-07-05 16:58:03.000000 argil-0.0.21/LICENCE.md
--rw-rw-r--   0 charles   (1000) charles   (1000)     1256 2023-07-17 04:59:43.656138 argil-0.0.21/PKG-INFO
--rw-rw-r--   0 charles   (1000) charles   (1000)      655 2023-07-05 16:40:12.000000 argil-0.0.21/README.md
-drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2023-07-17 04:59:43.656138 argil-0.0.21/argil/
--rw-rw-r--   0 charles   (1000) charles   (1000)      251 2023-07-05 16:40:12.000000 argil-0.0.21/argil/__init__.py
--rw-rw-r--   0 charles   (1000) charles   (1000)      167 2023-07-17 04:28:54.000000 argil-0.0.21/argil/types.py
--rw-rw-r--   0 charles   (1000) charles   (1000)      883 2023-07-17 04:26:25.000000 argil-0.0.21/argil/workflowRuns.py
--rw-rw-r--   0 charles   (1000) charles   (1000)      619 2023-07-17 04:58:15.000000 argil-0.0.21/argil/workflows.py
-drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2023-07-17 04:59:43.656138 argil-0.0.21/argil.egg-info/
--rw-rw-r--   0 charles   (1000) charles   (1000)     1256 2023-07-17 04:59:43.000000 argil-0.0.21/argil.egg-info/PKG-INFO
--rw-rw-r--   0 charles   (1000) charles   (1000)      247 2023-07-17 04:59:43.000000 argil-0.0.21/argil.egg-info/SOURCES.txt
--rw-rw-r--   0 charles   (1000) charles   (1000)        1 2023-07-17 04:59:43.000000 argil-0.0.21/argil.egg-info/dependency_links.txt
--rw-rw-r--   0 charles   (1000) charles   (1000)       16 2023-07-17 04:59:43.000000 argil-0.0.21/argil.egg-info/requires.txt
--rw-rw-r--   0 charles   (1000) charles   (1000)        6 2023-07-17 04:59:43.000000 argil-0.0.21/argil.egg-info/top_level.txt
--rw-rw-r--   0 charles   (1000) charles   (1000)       38 2023-07-17 04:59:43.656138 argil-0.0.21/setup.cfg
--rw-rw-r--   0 charles   (1000) charles   (1000)     1125 2023-07-17 04:59:35.000000 argil-0.0.21/setup.py
+drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2023-07-17 05:06:41.992457 argil-0.0.23/
+-rw-rw-r--   0 charles   (1000) charles   (1000)    34600 2023-07-05 16:58:03.000000 argil-0.0.23/LICENCE.md
+-rw-rw-r--   0 charles   (1000) charles   (1000)     1255 2023-07-17 05:06:41.992457 argil-0.0.23/PKG-INFO
+-rw-rw-r--   0 charles   (1000) charles   (1000)      655 2023-07-05 16:40:12.000000 argil-0.0.23/README.md
+drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2023-07-17 05:06:41.992457 argil-0.0.23/argil/
+-rw-rw-r--   0 charles   (1000) charles   (1000)      251 2023-07-05 16:40:12.000000 argil-0.0.23/argil/__init__.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)      197 2023-07-17 05:06:16.000000 argil-0.0.23/argil/types.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)      883 2023-07-17 04:26:25.000000 argil-0.0.23/argil/workflowRuns.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)      619 2023-07-17 04:58:15.000000 argil-0.0.23/argil/workflows.py
+drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2023-07-17 05:06:41.992457 argil-0.0.23/argil.egg-info/
+-rw-rw-r--   0 charles   (1000) charles   (1000)     1255 2023-07-17 05:06:41.000000 argil-0.0.23/argil.egg-info/PKG-INFO
+-rw-rw-r--   0 charles   (1000) charles   (1000)      247 2023-07-17 05:06:41.000000 argil-0.0.23/argil.egg-info/SOURCES.txt
+-rw-rw-r--   0 charles   (1000) charles   (1000)        1 2023-07-17 05:06:41.000000 argil-0.0.23/argil.egg-info/dependency_links.txt
+-rw-rw-r--   0 charles   (1000) charles   (1000)        9 2023-07-17 05:06:41.000000 argil-0.0.23/argil.egg-info/requires.txt
+-rw-rw-r--   0 charles   (1000) charles   (1000)        6 2023-07-17 05:06:41.000000 argil-0.0.23/argil.egg-info/top_level.txt
+-rw-rw-r--   0 charles   (1000) charles   (1000)       38 2023-07-17 05:06:41.992457 argil-0.0.23/setup.cfg
+-rw-rw-r--   0 charles   (1000) charles   (1000)     1106 2023-07-17 05:06:28.000000 argil-0.0.23/setup.py
```

### Comparing `argil-0.0.21/LICENCE.md` & `argil-0.0.23/LICENCE.md`

 * *Files identical despite different names*

### Comparing `argil-0.0.21/PKG-INFO` & `argil-0.0.23/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: argil
-Version: 0.0.21
+Version: 0.0.23
 Summary: SDK for the Argil API
 Home-page: https://github.com/argildotai/argil-sdk-python
 Author: Brivael Le Pogam
 Author-email: briva@argil.ai
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENCE.md
 
 \n# Argil SDK for Python
 
 This is the Python SDK for the Argil API. It provides a convenient way to interact with the API from Python applications.
```

### Comparing `argil-0.0.21/README.md` & `argil-0.0.23/README.md`

 * *Files identical despite different names*

### Comparing `argil-0.0.21/argil/workflowRuns.py` & `argil-0.0.23/argil/workflowRuns.py`

 * *Files identical despite different names*

### Comparing `argil-0.0.21/argil/workflows.py` & `argil-0.0.23/argil/workflows.py`

 * *Files identical despite different names*

### Comparing `argil-0.0.21/argil.egg-info/PKG-INFO` & `argil-0.0.23/argil.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: argil
-Version: 0.0.21
+Version: 0.0.23
 Summary: SDK for the Argil API
 Home-page: https://github.com/argildotai/argil-sdk-python
 Author: Brivael Le Pogam
 Author-email: briva@argil.ai
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENCE.md
 
 \n# Argil SDK for Python
 
 This is the Python SDK for the Argil API. It provides a convenient way to interact with the API from Python applications.
```

### Comparing `argil-0.0.21/setup.py` & `argil-0.0.23/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\\n" + fh.read()
 
 setup(
     name='argil',
-    version='0.0.21',#'{{VERSION_PLACEHOLDER}}',
+    version='0.0.23',#'{{VERSION_PLACEHOLDER}}',
     author="Brivael Le Pogam",
     author_email="briva@argil.ai",
     description='SDK for the Argil API',
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url='https://github.com/argildotai/argil-sdk-python',
     packages=find_packages(),
@@ -23,13 +23,12 @@
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
         "Operating System :: OS Independent",
     ],
     install_requires=[
         'requests',
-        'typing',
     ],
     # package_dir = {"": "src"},
     # packages = setuptools.find_packages(where="src"),
-    python_requires = ">=3.10"
+    python_requires = ">=3.8"
 )
```

