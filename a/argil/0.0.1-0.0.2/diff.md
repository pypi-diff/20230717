# Comparing `tmp/argil-0.0.1.tar.gz` & `tmp/argil-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argil-0.0.1.tar", last modified: Mon Jul 17 04:12:20 2023, max compression
+gzip compressed data, was "argil-0.0.2.tar", last modified: Mon Jul 17 04:36:02 2023, max compression
```

## Comparing `argil-0.0.1.tar` & `argil-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2023-07-17 04:12:20.329727 argil-0.0.1/
--rw-rw-r--   0 charles   (1000) charles   (1000)    34600 2023-07-05 16:58:03.000000 argil-0.0.1/LICENCE.md
--rw-rw-r--   0 charles   (1000) charles   (1000)     1231 2023-07-17 04:12:20.329727 argil-0.0.1/PKG-INFO
--rw-rw-r--   0 charles   (1000) charles   (1000)      655 2023-07-05 16:40:12.000000 argil-0.0.1/README.md
-drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2023-07-17 04:12:20.329727 argil-0.0.1/argil/
--rw-rw-r--   0 charles   (1000) charles   (1000)      251 2023-07-05 16:40:12.000000 argil-0.0.1/argil/__init__.py
--rw-rw-r--   0 charles   (1000) charles   (1000)      167 2023-07-05 16:40:12.000000 argil-0.0.1/argil/types.py
--rw-rw-r--   0 charles   (1000) charles   (1000)      883 2023-07-05 17:08:17.000000 argil-0.0.1/argil/workflowRuns.py
--rw-rw-r--   0 charles   (1000) charles   (1000)      608 2023-07-05 16:40:12.000000 argil-0.0.1/argil/workflows.py
-drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2023-07-17 04:12:20.329727 argil-0.0.1/argil.egg-info/
--rw-rw-r--   0 charles   (1000) charles   (1000)     1231 2023-07-17 04:12:20.000000 argil-0.0.1/argil.egg-info/PKG-INFO
--rw-rw-r--   0 charles   (1000) charles   (1000)      247 2023-07-17 04:12:20.000000 argil-0.0.1/argil.egg-info/SOURCES.txt
--rw-rw-r--   0 charles   (1000) charles   (1000)        1 2023-07-17 04:12:20.000000 argil-0.0.1/argil.egg-info/dependency_links.txt
--rw-rw-r--   0 charles   (1000) charles   (1000)       16 2023-07-17 04:12:20.000000 argil-0.0.1/argil.egg-info/requires.txt
--rw-rw-r--   0 charles   (1000) charles   (1000)        6 2023-07-17 04:12:20.000000 argil-0.0.1/argil.egg-info/top_level.txt
--rw-rw-r--   0 charles   (1000) charles   (1000)       38 2023-07-17 04:12:20.329727 argil-0.0.1/setup.cfg
--rw-rw-r--   0 charles   (1000) charles   (1000)     1125 2023-07-17 04:12:16.000000 argil-0.0.1/setup.py
+drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2023-07-17 04:36:02.407368 argil-0.0.2/
+-rw-rw-r--   0 charles   (1000) charles   (1000)    34600 2023-07-05 16:58:03.000000 argil-0.0.2/LICENCE.md
+-rw-rw-r--   0 charles   (1000) charles   (1000)     1255 2023-07-17 04:36:02.407368 argil-0.0.2/PKG-INFO
+-rw-rw-r--   0 charles   (1000) charles   (1000)      655 2023-07-05 16:40:12.000000 argil-0.0.2/README.md
+drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2023-07-17 04:36:02.407368 argil-0.0.2/argil/
+-rw-rw-r--   0 charles   (1000) charles   (1000)      251 2023-07-05 16:40:12.000000 argil-0.0.2/argil/__init__.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)      167 2023-07-17 04:28:54.000000 argil-0.0.2/argil/types.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)      883 2023-07-17 04:26:25.000000 argil-0.0.2/argil/workflowRuns.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)      608 2023-07-05 16:40:12.000000 argil-0.0.2/argil/workflows.py
+drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2023-07-17 04:36:02.407368 argil-0.0.2/argil.egg-info/
+-rw-rw-r--   0 charles   (1000) charles   (1000)     1255 2023-07-17 04:36:02.000000 argil-0.0.2/argil.egg-info/PKG-INFO
+-rw-rw-r--   0 charles   (1000) charles   (1000)      247 2023-07-17 04:36:02.000000 argil-0.0.2/argil.egg-info/SOURCES.txt
+-rw-rw-r--   0 charles   (1000) charles   (1000)        1 2023-07-17 04:36:02.000000 argil-0.0.2/argil.egg-info/dependency_links.txt
+-rw-rw-r--   0 charles   (1000) charles   (1000)       16 2023-07-17 04:36:02.000000 argil-0.0.2/argil.egg-info/requires.txt
+-rw-rw-r--   0 charles   (1000) charles   (1000)        6 2023-07-17 04:36:02.000000 argil-0.0.2/argil.egg-info/top_level.txt
+-rw-rw-r--   0 charles   (1000) charles   (1000)       38 2023-07-17 04:36:02.407368 argil-0.0.2/setup.cfg
+-rw-rw-r--   0 charles   (1000) charles   (1000)     1124 2023-07-17 04:35:29.000000 argil-0.0.2/setup.py
```

### Comparing `argil-0.0.1/LICENCE.md` & `argil-0.0.2/LICENCE.md`

 * *Files identical despite different names*

### Comparing `argil-0.0.1/PKG-INFO` & `argil-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: argil
-Version: 0.0.1
+Version: 0.0.2
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
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENCE.md
 
 \n# Argil SDK for Python
 
 This is the Python SDK for the Argil API. It provides a convenient way to interact with the API from Python applications.
```

### Comparing `argil-0.0.1/README.md` & `argil-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `argil-0.0.1/argil/workflowRuns.py` & `argil-0.0.2/argil/workflowRuns.py`

 * *Files identical despite different names*

### Comparing `argil-0.0.1/argil/workflows.py` & `argil-0.0.2/argil/workflows.py`

 * *Files identical despite different names*

### Comparing `argil-0.0.1/argil.egg-info/PKG-INFO` & `argil-0.0.2/argil.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: argil
-Version: 0.0.1
+Version: 0.0.2
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
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENCE.md
 
 \n# Argil SDK for Python
 
 This is the Python SDK for the Argil API. It provides a convenient way to interact with the API from Python applications.
```

### Comparing `argil-0.0.1/setup.py` & `argil-0.0.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\\n" + fh.read()
 
 setup(
     name='argil',
-    version='0.0.1',#'{{VERSION_PLACEHOLDER}}',
+    version='0.0.2',#'{{VERSION_PLACEHOLDER}}',
     author="Brivael Le Pogam",
     author_email="briva@argil.ai",
     description='SDK for the Argil API',
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url='https://github.com/argildotai/argil-sdk-python',
     packages=find_packages(),
@@ -27,9 +27,9 @@
     ],
     install_requires=[
         'requests',
         'typing',
     ],
     # package_dir = {"": "src"},
     # packages = setuptools.find_packages(where="src"),
-    # python_requires = ">=3.6"
+    python_requires = ">=3.10"
 )
```

