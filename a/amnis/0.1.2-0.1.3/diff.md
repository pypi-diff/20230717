# Comparing `tmp/amnis-0.1.2.tar.gz` & `tmp/amnis-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amnis-0.1.2.tar", last modified: Mon Jul 17 16:34:52 2023, max compression
+gzip compressed data, was "amnis-0.1.3.tar", last modified: Mon Jul 17 18:16:33 2023, max compression
```

## Comparing `amnis-0.1.2.tar` & `amnis-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 zahash    (1000) zahash    (1000)        0 2023-07-17 16:34:52.864887 amnis-0.1.2/
--rw-rw-r--   0 zahash    (1000) zahash    (1000)     1063 2021-09-26 12:41:19.000000 amnis-0.1.2/LICENSE
--rw-rw-r--   0 zahash    (1000) zahash    (1000)       15 2021-09-26 12:44:27.000000 amnis-0.1.2/MANIFEST.in
--rw-rw-r--   0 zahash    (1000) zahash    (1000)     7844 2023-07-17 16:34:52.864887 amnis-0.1.2/PKG-INFO
--rw-rw-r--   0 zahash    (1000) zahash    (1000)     7445 2023-07-17 14:32:48.000000 amnis-0.1.2/README.md
-drwxrwxr-x   0 zahash    (1000) zahash    (1000)        0 2023-07-17 16:34:52.864887 amnis-0.1.2/amnis/
--rw-rw-r--   0 zahash    (1000) zahash    (1000)       36 2022-09-11 14:43:08.000000 amnis-0.1.2/amnis/__init__.py
--rw-rw-r--   0 zahash    (1000) zahash    (1000)     5639 2023-07-17 16:31:23.000000 amnis-0.1.2/amnis/stream.py
-drwxrwxr-x   0 zahash    (1000) zahash    (1000)        0 2023-07-17 16:34:52.864887 amnis-0.1.2/amnis.egg-info/
--rw-rw-r--   0 zahash    (1000) zahash    (1000)     7844 2023-07-17 16:34:52.000000 amnis-0.1.2/amnis.egg-info/PKG-INFO
--rw-rw-r--   0 zahash    (1000) zahash    (1000)      188 2023-07-17 16:34:52.000000 amnis-0.1.2/amnis.egg-info/SOURCES.txt
--rw-rw-r--   0 zahash    (1000) zahash    (1000)        1 2023-07-17 16:34:52.000000 amnis-0.1.2/amnis.egg-info/dependency_links.txt
--rw-rw-r--   0 zahash    (1000) zahash    (1000)        6 2023-07-17 16:34:52.000000 amnis-0.1.2/amnis.egg-info/top_level.txt
--rw-rw-r--   0 zahash    (1000) zahash    (1000)       38 2023-07-17 16:34:52.864887 amnis-0.1.2/setup.cfg
--rw-rw-r--   0 zahash    (1000) zahash    (1000)      885 2023-07-17 16:33:19.000000 amnis-0.1.2/setup.py
+drwxrwxr-x   0 zahash    (1000) zahash    (1000)        0 2023-07-17 18:16:33.264148 amnis-0.1.3/
+-rw-rw-r--   0 zahash    (1000) zahash    (1000)     1063 2021-09-26 12:41:19.000000 amnis-0.1.3/LICENSE
+-rw-rw-r--   0 zahash    (1000) zahash    (1000)       15 2021-09-26 12:44:27.000000 amnis-0.1.3/MANIFEST.in
+-rw-rw-r--   0 zahash    (1000) zahash    (1000)     7844 2023-07-17 18:16:33.264148 amnis-0.1.3/PKG-INFO
+-rw-rw-r--   0 zahash    (1000) zahash    (1000)     7445 2023-07-17 18:14:05.000000 amnis-0.1.3/README.md
+drwxrwxr-x   0 zahash    (1000) zahash    (1000)        0 2023-07-17 18:16:33.264148 amnis-0.1.3/amnis/
+-rw-rw-r--   0 zahash    (1000) zahash    (1000)       36 2022-09-11 14:43:08.000000 amnis-0.1.3/amnis/__init__.py
+-rw-rw-r--   0 zahash    (1000) zahash    (1000)     5639 2023-07-17 16:31:23.000000 amnis-0.1.3/amnis/stream.py
+drwxrwxr-x   0 zahash    (1000) zahash    (1000)        0 2023-07-17 18:16:33.264148 amnis-0.1.3/amnis.egg-info/
+-rw-rw-r--   0 zahash    (1000) zahash    (1000)     7844 2023-07-17 18:16:33.000000 amnis-0.1.3/amnis.egg-info/PKG-INFO
+-rw-rw-r--   0 zahash    (1000) zahash    (1000)      188 2023-07-17 18:16:33.000000 amnis-0.1.3/amnis.egg-info/SOURCES.txt
+-rw-rw-r--   0 zahash    (1000) zahash    (1000)        1 2023-07-17 18:16:33.000000 amnis-0.1.3/amnis.egg-info/dependency_links.txt
+-rw-rw-r--   0 zahash    (1000) zahash    (1000)        6 2023-07-17 18:16:33.000000 amnis-0.1.3/amnis.egg-info/top_level.txt
+-rw-rw-r--   0 zahash    (1000) zahash    (1000)       38 2023-07-17 18:16:33.264148 amnis-0.1.3/setup.cfg
+-rw-rw-r--   0 zahash    (1000) zahash    (1000)      885 2023-07-17 18:16:14.000000 amnis-0.1.3/setup.py
```

### Comparing `amnis-0.1.2/LICENSE` & `amnis-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `amnis-0.1.2/PKG-INFO` & `amnis-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amnis
-Version: 0.1.2
+Version: 0.1.3
 Summary: Java like Stream Api for Python
 Home-page: https://github.com/zahash/amnis
 Author: zahash
 Author-email: zahash.z@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -15,16 +15,15 @@
 
 # amnis
 
 > Java like Streams Api for Python
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
-Python package for Java like Streams. Streams are lazy evaluated -- That is, evaluation starts only when a terminal
-operation is applied
+Python package for Java like Streams. Streams are lazy evaluated -- That is, evaluation starts only when a terminal operation is applied
 
 ## Installation
 
 pip install this repo.
 (Note: Incompatible with Python 2.x)
 
 ```sh
```

### Comparing `amnis-0.1.2/README.md` & `amnis-0.1.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # amnis
 
 > Java like Streams Api for Python
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
-Python package for Java like Streams. Streams are lazy evaluated -- That is, evaluation starts only when a terminal
-operation is applied
+Python package for Java like Streams. Streams are lazy evaluated -- That is, evaluation starts only when a terminal operation is applied
 
 ## Installation
 
 pip install this repo.
 (Note: Incompatible with Python 2.x)
 
 ```sh
```

### Comparing `amnis-0.1.2/amnis/stream.py` & `amnis-0.1.3/amnis/stream.py`

 * *Files identical despite different names*

### Comparing `amnis-0.1.2/amnis.egg-info/PKG-INFO` & `amnis-0.1.3/amnis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amnis
-Version: 0.1.2
+Version: 0.1.3
 Summary: Java like Stream Api for Python
 Home-page: https://github.com/zahash/amnis
 Author: zahash
 Author-email: zahash.z@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -15,16 +15,15 @@
 
 # amnis
 
 > Java like Streams Api for Python
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
-Python package for Java like Streams. Streams are lazy evaluated -- That is, evaluation starts only when a terminal
-operation is applied
+Python package for Java like Streams. Streams are lazy evaluated -- That is, evaluation starts only when a terminal operation is applied
 
 ## Installation
 
 pip install this repo.
 (Note: Incompatible with Python 2.x)
 
 ```sh
```

### Comparing `amnis-0.1.2/setup.py` & `amnis-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 README = (HERE / "README.md").read_text()
 
 with (HERE / "requirements.txt").open() as f:
     requirements = f.read().splitlines()
 
 setup(
     name="amnis",
-    version="0.1.2",
+    version="0.1.3",
     description="Java like Stream Api for Python",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/zahash/amnis",
     author="zahash",
     author_email="zahash.z@gmail.com",
     license="MIT",
```

