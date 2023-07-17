# Comparing `tmp/amnis-0.1.0.tar.gz` & `tmp/amnis-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amnis-0.1.0.tar", last modified: Mon Jul 17 14:20:50 2023, max compression
+gzip compressed data, was "amnis-0.1.1.tar", last modified: Mon Jul 17 14:37:30 2023, max compression
```

## Comparing `amnis-0.1.0.tar` & `amnis-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 zahash    (1000) zahash    (1000)        0 2023-07-17 14:20:50.269289 amnis-0.1.0/
--rw-rw-r--   0 zahash    (1000) zahash    (1000)     1063 2021-09-26 12:41:19.000000 amnis-0.1.0/LICENSE
--rw-rw-r--   0 zahash    (1000) zahash    (1000)       15 2021-09-26 12:44:27.000000 amnis-0.1.0/MANIFEST.in
--rw-rw-r--   0 zahash    (1000) zahash    (1000)     7912 2023-07-17 14:20:50.269289 amnis-0.1.0/PKG-INFO
--rw-rw-r--   0 zahash    (1000) zahash    (1000)     7513 2023-07-17 11:49:07.000000 amnis-0.1.0/README.md
-drwxrwxr-x   0 zahash    (1000) zahash    (1000)        0 2023-07-17 14:20:50.269289 amnis-0.1.0/amnis/
--rw-rw-r--   0 zahash    (1000) zahash    (1000)       36 2022-09-11 14:43:08.000000 amnis-0.1.0/amnis/__init__.py
--rw-rw-r--   0 zahash    (1000) zahash    (1000)     5502 2022-09-11 15:38:51.000000 amnis-0.1.0/amnis/stream.py
-drwxrwxr-x   0 zahash    (1000) zahash    (1000)        0 2023-07-17 14:20:50.269289 amnis-0.1.0/amnis.egg-info/
--rw-rw-r--   0 zahash    (1000) zahash    (1000)     7912 2023-07-17 14:20:50.000000 amnis-0.1.0/amnis.egg-info/PKG-INFO
--rw-rw-r--   0 zahash    (1000) zahash    (1000)      188 2023-07-17 14:20:50.000000 amnis-0.1.0/amnis.egg-info/SOURCES.txt
--rw-rw-r--   0 zahash    (1000) zahash    (1000)        1 2023-07-17 14:20:50.000000 amnis-0.1.0/amnis.egg-info/dependency_links.txt
--rw-rw-r--   0 zahash    (1000) zahash    (1000)        6 2023-07-17 14:20:50.000000 amnis-0.1.0/amnis.egg-info/top_level.txt
--rw-rw-r--   0 zahash    (1000) zahash    (1000)       38 2023-07-17 14:20:50.269289 amnis-0.1.0/setup.cfg
--rw-rw-r--   0 zahash    (1000) zahash    (1000)      793 2023-07-17 14:19:12.000000 amnis-0.1.0/setup.py
+drwxrwxr-x   0 zahash    (1000) zahash    (1000)        0 2023-07-17 14:37:30.298782 amnis-0.1.1/
+-rw-rw-r--   0 zahash    (1000) zahash    (1000)     1063 2021-09-26 12:41:19.000000 amnis-0.1.1/LICENSE
+-rw-rw-r--   0 zahash    (1000) zahash    (1000)       15 2021-09-26 12:44:27.000000 amnis-0.1.1/MANIFEST.in
+-rw-rw-r--   0 zahash    (1000) zahash    (1000)     7844 2023-07-17 14:37:30.298782 amnis-0.1.1/PKG-INFO
+-rw-rw-r--   0 zahash    (1000) zahash    (1000)     7445 2023-07-17 14:32:48.000000 amnis-0.1.1/README.md
+drwxrwxr-x   0 zahash    (1000) zahash    (1000)        0 2023-07-17 14:37:30.298782 amnis-0.1.1/amnis/
+-rw-rw-r--   0 zahash    (1000) zahash    (1000)       36 2022-09-11 14:43:08.000000 amnis-0.1.1/amnis/__init__.py
+-rw-rw-r--   0 zahash    (1000) zahash    (1000)     5502 2022-09-11 15:38:51.000000 amnis-0.1.1/amnis/stream.py
+drwxrwxr-x   0 zahash    (1000) zahash    (1000)        0 2023-07-17 14:37:30.298782 amnis-0.1.1/amnis.egg-info/
+-rw-rw-r--   0 zahash    (1000) zahash    (1000)     7844 2023-07-17 14:37:30.000000 amnis-0.1.1/amnis.egg-info/PKG-INFO
+-rw-rw-r--   0 zahash    (1000) zahash    (1000)      188 2023-07-17 14:37:30.000000 amnis-0.1.1/amnis.egg-info/SOURCES.txt
+-rw-rw-r--   0 zahash    (1000) zahash    (1000)        1 2023-07-17 14:37:30.000000 amnis-0.1.1/amnis.egg-info/dependency_links.txt
+-rw-rw-r--   0 zahash    (1000) zahash    (1000)        6 2023-07-17 14:37:30.000000 amnis-0.1.1/amnis.egg-info/top_level.txt
+-rw-rw-r--   0 zahash    (1000) zahash    (1000)       38 2023-07-17 14:37:30.298782 amnis-0.1.1/setup.cfg
+-rw-rw-r--   0 zahash    (1000) zahash    (1000)      885 2023-07-17 14:33:03.000000 amnis-0.1.1/setup.py
```

### Comparing `amnis-0.1.0/LICENSE` & `amnis-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `amnis-0.1.0/PKG-INFO` & `amnis-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amnis
-Version: 0.1.0
+Version: 0.1.1
 Summary: Java like Stream Api for Python
 Home-page: https://github.com/zahash/amnis
 Author: zahash
 Author-email: zahash.z@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -24,21 +24,21 @@
 
 ## Installation
 
 pip install this repo.
 (Note: Incompatible with Python 2.x)
 
 ```sh
-pip3 install git+https://github.com/zahash/amnis.git
+pip3 install amnis
 ```
 
 (or)
 
 ```sh
-pip install git+https://github.com/zahash/amnis.git
+pip install amnis
 ```
 
 ## Usage examples
 
 ### map
 
 ```Python
```

### Comparing `amnis-0.1.0/README.md` & `amnis-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 
 ## Installation
 
 pip install this repo.
 (Note: Incompatible with Python 2.x)
 
 ```sh
-pip3 install git+https://github.com/zahash/amnis.git
+pip3 install amnis
 ```
 
 (or)
 
 ```sh
-pip install git+https://github.com/zahash/amnis.git
+pip install amnis
 ```
 
 ## Usage examples
 
 ### map
 
 ```Python
```

### Comparing `amnis-0.1.0/amnis/stream.py` & `amnis-0.1.1/amnis/stream.py`

 * *Files identical despite different names*

### Comparing `amnis-0.1.0/amnis.egg-info/PKG-INFO` & `amnis-0.1.1/amnis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amnis
-Version: 0.1.0
+Version: 0.1.1
 Summary: Java like Stream Api for Python
 Home-page: https://github.com/zahash/amnis
 Author: zahash
 Author-email: zahash.z@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -24,21 +24,21 @@
 
 ## Installation
 
 pip install this repo.
 (Note: Incompatible with Python 2.x)
 
 ```sh
-pip3 install git+https://github.com/zahash/amnis.git
+pip3 install amnis
 ```
 
 (or)
 
 ```sh
-pip install git+https://github.com/zahash/amnis.git
+pip install amnis
 ```
 
 ## Usage examples
 
 ### map
 
 ```Python
```

