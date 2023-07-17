# Comparing `tmp/simple-swag-0.1.0.tar.gz` & `tmp/simple-swag-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple-swag-0.1.0.tar", last modified: Mon Jul 17 08:50:49 2023, max compression
+gzip compressed data, was "simple-swag-0.1.1.tar", last modified: Mon Jul 17 08:57:46 2023, max compression
```

## Comparing `simple-swag-0.1.0.tar` & `simple-swag-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 peterprescott  (1000) peterprescott  (1000)        0 2023-07-17 08:50:49.670648 simple-swag-0.1.0/
--rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)      845 2023-07-17 08:50:49.670648 simple-swag-0.1.0/PKG-INFO
--rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)      489 2023-07-14 08:55:13.000000 simple-swag-0.1.0/README.md
--rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)      104 2023-07-11 17:11:37.000000 simple-swag-0.1.0/pyproject.toml
--rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)      666 2023-07-17 08:50:49.670648 simple-swag-0.1.0/setup.cfg
-drwxr-xr-x   0 peterprescott  (1000) peterprescott  (1000)        0 2023-07-17 08:50:49.666648 simple-swag-0.1.0/src/
-drwxr-xr-x   0 peterprescott  (1000) peterprescott  (1000)        0 2023-07-17 08:50:49.666648 simple-swag-0.1.0/src/simple_swag.egg-info/
--rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)      845 2023-07-17 08:50:49.000000 simple-swag-0.1.0/src/simple_swag.egg-info/PKG-INFO
--rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)      406 2023-07-17 08:50:49.000000 simple-swag-0.1.0/src/simple_swag.egg-info/SOURCES.txt
--rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)        1 2023-07-17 08:50:49.000000 simple-swag-0.1.0/src/simple_swag.egg-info/dependency_links.txt
--rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)       39 2023-07-17 08:50:49.000000 simple-swag-0.1.0/src/simple_swag.egg-info/entry_points.txt
--rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)       55 2023-07-17 08:50:49.000000 simple-swag-0.1.0/src/simple_swag.egg-info/requires.txt
--rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)        5 2023-07-17 08:50:49.000000 simple-swag-0.1.0/src/simple_swag.egg-info/top_level.txt
-drwxr-xr-x   0 peterprescott  (1000) peterprescott  (1000)        0 2023-07-17 08:50:49.666648 simple-swag-0.1.0/src/swag/
--rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)        0 2023-07-15 16:44:08.000000 simple-swag-0.1.0/src/swag/__init__.py
--rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)     2380 2023-07-15 18:50:02.000000 simple-swag-0.1.0/src/swag/autoblog.py
--rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)     5650 2023-07-17 08:31:43.000000 simple-swag-0.1.0/src/swag/builder.py
--rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)     2288 2023-07-15 17:14:52.000000 simple-swag-0.1.0/src/swag/cli.py
--rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)     1093 2023-07-15 17:02:53.000000 simple-swag-0.1.0/src/swag/lorem.py
--rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)     4689 2023-07-15 17:01:11.000000 simple-swag-0.1.0/src/swag/resources.py
-drwxr-xr-x   0 peterprescott  (1000) peterprescott  (1000)        0 2023-07-17 08:50:49.670648 simple-swag-0.1.0/tests/
--rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)      198 2023-07-14 09:25:30.000000 simple-swag-0.1.0/tests/test_cli.py
+drwxr-xr-x   0 peterprescott  (1000) peterprescott  (1000)        0 2023-07-17 08:57:46.192302 simple-swag-0.1.1/
+-rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)      845 2023-07-17 08:57:46.192302 simple-swag-0.1.1/PKG-INFO
+-rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)      489 2023-07-14 08:55:13.000000 simple-swag-0.1.1/README.md
+-rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)      104 2023-07-11 17:11:37.000000 simple-swag-0.1.1/pyproject.toml
+-rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)      686 2023-07-17 08:57:46.192302 simple-swag-0.1.1/setup.cfg
+drwxr-xr-x   0 peterprescott  (1000) peterprescott  (1000)        0 2023-07-17 08:57:46.188301 simple-swag-0.1.1/src/
+drwxr-xr-x   0 peterprescott  (1000) peterprescott  (1000)        0 2023-07-17 08:57:46.192302 simple-swag-0.1.1/src/simple_swag.egg-info/
+-rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)      845 2023-07-17 08:57:46.000000 simple-swag-0.1.1/src/simple_swag.egg-info/PKG-INFO
+-rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)      406 2023-07-17 08:57:46.000000 simple-swag-0.1.1/src/simple_swag.egg-info/SOURCES.txt
+-rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)        1 2023-07-17 08:57:46.000000 simple-swag-0.1.1/src/simple_swag.egg-info/dependency_links.txt
+-rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)       39 2023-07-17 08:57:46.000000 simple-swag-0.1.1/src/simple_swag.egg-info/entry_points.txt
+-rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)       74 2023-07-17 08:57:46.000000 simple-swag-0.1.1/src/simple_swag.egg-info/requires.txt
+-rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)        5 2023-07-17 08:57:46.000000 simple-swag-0.1.1/src/simple_swag.egg-info/top_level.txt
+drwxr-xr-x   0 peterprescott  (1000) peterprescott  (1000)        0 2023-07-17 08:57:46.192302 simple-swag-0.1.1/src/swag/
+-rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)        0 2023-07-15 16:44:08.000000 simple-swag-0.1.1/src/swag/__init__.py
+-rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)     2380 2023-07-15 18:50:02.000000 simple-swag-0.1.1/src/swag/autoblog.py
+-rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)     5650 2023-07-17 08:31:43.000000 simple-swag-0.1.1/src/swag/builder.py
+-rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)     2288 2023-07-15 17:14:52.000000 simple-swag-0.1.1/src/swag/cli.py
+-rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)     1093 2023-07-15 17:02:53.000000 simple-swag-0.1.1/src/swag/lorem.py
+-rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)     4689 2023-07-15 17:01:11.000000 simple-swag-0.1.1/src/swag/resources.py
+drwxr-xr-x   0 peterprescott  (1000) peterprescott  (1000)        0 2023-07-17 08:57:46.192302 simple-swag-0.1.1/tests/
+-rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)      198 2023-07-14 09:25:30.000000 simple-swag-0.1.1/tests/test_cli.py
```

### Comparing `simple-swag-0.1.0/PKG-INFO` & `simple-swag-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-swag
-Version: 0.1.0
+Version: 0.1.1
 Summary: "Simple Website Auto Generator"
 Home-page: https://github.com/peterprescott/simple-swag
 Author: Peter Prescott
 Author-email: prescott.peter@gmail.com
 Project-URL: Bug Tracker, https://github.com/peterprescott/simple-swag/issues
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `simple-swag-0.1.0/setup.cfg` & `simple-swag-0.1.1/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = simple-swag
-version = 0.1.0
+version = 0.1.1
 author = Peter Prescott
 author_email = prescott.peter@gmail.com
 description = "Simple Website Auto Generator"
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/peterprescott/simple-swag
 project_urls = 
@@ -16,14 +16,15 @@
 packages = find:
 python_requires = >=3.6
 install_requires = 
 	fire
 	lorem
 	markdown
 	markdown-full-yaml-metadata
+	multiavatar-python
 	pandas
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts =
```

### Comparing `simple-swag-0.1.0/src/simple_swag.egg-info/PKG-INFO` & `simple-swag-0.1.1/src/simple_swag.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-swag
-Version: 0.1.0
+Version: 0.1.1
 Summary: "Simple Website Auto Generator"
 Home-page: https://github.com/peterprescott/simple-swag
 Author: Peter Prescott
 Author-email: prescott.peter@gmail.com
 Project-URL: Bug Tracker, https://github.com/peterprescott/simple-swag/issues
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `simple-swag-0.1.0/src/swag/autoblog.py` & `simple-swag-0.1.1/src/swag/autoblog.py`

 * *Files identical despite different names*

### Comparing `simple-swag-0.1.0/src/swag/builder.py` & `simple-swag-0.1.1/src/swag/builder.py`

 * *Files identical despite different names*

### Comparing `simple-swag-0.1.0/src/swag/cli.py` & `simple-swag-0.1.1/src/swag/cli.py`

 * *Files identical despite different names*

### Comparing `simple-swag-0.1.0/src/swag/lorem.py` & `simple-swag-0.1.1/src/swag/lorem.py`

 * *Files identical despite different names*

### Comparing `simple-swag-0.1.0/src/swag/resources.py` & `simple-swag-0.1.1/src/swag/resources.py`

 * *Files identical despite different names*

