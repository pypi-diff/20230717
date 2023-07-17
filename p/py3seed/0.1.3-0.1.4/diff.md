# Comparing `tmp/py3seed-0.1.3.tar.gz` & `tmp/py3seed-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3seed-0.1.3.tar", last modified: Mon Jul 17 08:13:19 2023, max compression
+gzip compressed data, was "py3seed-0.1.4.tar", last modified: Mon Jul 17 08:24:11 2023, max compression
```

## Comparing `py3seed-0.1.3.tar` & `py3seed-0.1.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-17 08:13:19.858812 py3seed-0.1.3/
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1072 2021-08-08 16:29:42.000000 py3seed-0.1.3/LICENSE
--rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-07-17 08:13:19.858969 py3seed-0.1.3/PKG-INFO
--rw-r--r--   0 weiminfeng   (501) staff       (20)      288 2021-08-11 03:57:41.000000 py3seed-0.1.3/README.md
--rw-r--r--   0 weiminfeng   (501) staff       (20)      104 2021-09-18 08:01:25.000000 py3seed-0.1.3/pyproject.toml
--rw-r--r--   0 weiminfeng   (501) staff       (20)      911 2023-07-17 08:13:19.859792 py3seed-0.1.3/setup.cfg
--rw-r--r--   0 weiminfeng   (501) staff       (20)      214 2023-07-06 08:35:28.000000 py3seed-0.1.3/setup.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-17 08:13:19.834321 py3seed-0.1.3/src/
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-17 08:13:19.847240 py3seed-0.1.3/src/py3seed/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      743 2023-07-10 07:31:29.000000 py3seed-0.1.3/src/py3seed/__init__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1624 2023-07-10 03:47:01.000000 py3seed-0.1.3/src/py3seed/__main__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)      992 2021-09-02 08:44:38.000000 py3seed-0.1.3/src/py3seed/admin.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     6458 2023-07-10 03:55:28.000000 py3seed-0.1.3/src/py3seed/cachesupport.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-17 08:13:19.853145 py3seed-0.1.3/src/py3seed/commands/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      151 2021-09-01 02:10:05.000000 py3seed-0.1.3/src/py3seed/commands/__init__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    20437 2023-07-17 08:12:35.000000 py3seed-0.1.3/src/py3seed/commands/gen.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)      732 2023-06-27 01:48:25.000000 py3seed-0.1.3/src/py3seed/error.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    11554 2023-07-10 03:49:24.000000 py3seed-0.1.3/src/py3seed/inflection.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1166 2022-05-06 11:35:05.000000 py3seed-0.1.3/src/py3seed/log.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    17725 2023-07-11 02:10:39.000000 py3seed-0.1.3/src/py3seed/merge3.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    57699 2023-07-13 02:24:43.000000 py3seed-0.1.3/src/py3seed/model.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    14489 2023-07-10 03:55:58.000000 py3seed-0.1.3/src/py3seed/mongosupport.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    14313 2023-07-17 08:10:25.000000 py3seed-0.1.3/src/py3seed/utils.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     7471 2023-07-10 03:54:22.000000 py3seed-0.1.3/src/py3seed/websupport.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-17 08:13:19.852018 py3seed-0.1.3/src/py3seed.egg-info/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-07-17 08:13:19.000000 py3seed-0.1.3/src/py3seed.egg-info/PKG-INFO
--rw-r--r--   0 weiminfeng   (501) staff       (20)      718 2023-07-17 08:13:19.000000 py3seed-0.1.3/src/py3seed.egg-info/SOURCES.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)        1 2023-07-17 08:13:19.000000 py3seed-0.1.3/src/py3seed.egg-info/dependency_links.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)      111 2023-07-17 08:13:19.000000 py3seed-0.1.3/src/py3seed.egg-info/entry_points.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)       48 2023-07-17 08:13:19.000000 py3seed-0.1.3/src/py3seed.egg-info/requires.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)        8 2023-07-17 08:13:19.000000 py3seed-0.1.3/src/py3seed.egg-info/top_level.txt
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-17 08:13:19.857980 py3seed-0.1.3/tests/
--rw-r--r--   0 weiminfeng   (501) staff       (20)     3216 2022-12-09 02:58:18.000000 py3seed-0.1.3/tests/test_cachesupport.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     6333 2023-07-13 03:38:58.000000 py3seed-0.1.3/tests/test_gen.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    14977 2023-07-10 03:39:53.000000 py3seed-0.1.3/tests/test_merge3.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     5116 2023-07-05 06:36:00.000000 py3seed-0.1.3/tests/test_model.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     2083 2023-07-05 06:36:25.000000 py3seed-0.1.3/tests/test_mongosupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-17 08:24:11.309841 py3seed-0.1.4/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1072 2021-08-08 16:29:42.000000 py3seed-0.1.4/LICENSE
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-07-17 08:24:11.309965 py3seed-0.1.4/PKG-INFO
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      288 2021-08-11 03:57:41.000000 py3seed-0.1.4/README.md
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      104 2021-09-18 08:01:25.000000 py3seed-0.1.4/pyproject.toml
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      911 2023-07-17 08:24:11.310570 py3seed-0.1.4/setup.cfg
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      214 2023-07-06 08:35:28.000000 py3seed-0.1.4/setup.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-17 08:24:11.287514 py3seed-0.1.4/src/
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-17 08:24:11.301378 py3seed-0.1.4/src/py3seed/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      743 2023-07-10 07:31:29.000000 py3seed-0.1.4/src/py3seed/__init__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1624 2023-07-10 03:47:01.000000 py3seed-0.1.4/src/py3seed/__main__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      992 2021-09-02 08:44:38.000000 py3seed-0.1.4/src/py3seed/admin.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     6458 2023-07-10 03:55:28.000000 py3seed-0.1.4/src/py3seed/cachesupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-17 08:24:11.305923 py3seed-0.1.4/src/py3seed/commands/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      151 2021-09-01 02:10:05.000000 py3seed-0.1.4/src/py3seed/commands/__init__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    20437 2023-07-17 08:12:35.000000 py3seed-0.1.4/src/py3seed/commands/gen.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      732 2023-06-27 01:48:25.000000 py3seed-0.1.4/src/py3seed/error.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    11554 2023-07-10 03:49:24.000000 py3seed-0.1.4/src/py3seed/inflection.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1166 2022-05-06 11:35:05.000000 py3seed-0.1.4/src/py3seed/log.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    17725 2023-07-11 02:10:39.000000 py3seed-0.1.4/src/py3seed/merge3.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    57699 2023-07-13 02:24:43.000000 py3seed-0.1.4/src/py3seed/model.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14489 2023-07-10 03:55:58.000000 py3seed-0.1.4/src/py3seed/mongosupport.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14318 2023-07-17 08:23:47.000000 py3seed-0.1.4/src/py3seed/utils.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     7471 2023-07-10 03:54:22.000000 py3seed-0.1.4/src/py3seed/websupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-17 08:24:11.304924 py3seed-0.1.4/src/py3seed.egg-info/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-07-17 08:24:11.000000 py3seed-0.1.4/src/py3seed.egg-info/PKG-INFO
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      718 2023-07-17 08:24:11.000000 py3seed-0.1.4/src/py3seed.egg-info/SOURCES.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)        1 2023-07-17 08:24:11.000000 py3seed-0.1.4/src/py3seed.egg-info/dependency_links.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      111 2023-07-17 08:24:11.000000 py3seed-0.1.4/src/py3seed.egg-info/entry_points.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)       48 2023-07-17 08:24:11.000000 py3seed-0.1.4/src/py3seed.egg-info/requires.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)        8 2023-07-17 08:24:11.000000 py3seed-0.1.4/src/py3seed.egg-info/top_level.txt
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-17 08:24:11.309329 py3seed-0.1.4/tests/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     3216 2022-12-09 02:58:18.000000 py3seed-0.1.4/tests/test_cachesupport.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     6333 2023-07-13 03:38:58.000000 py3seed-0.1.4/tests/test_gen.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14977 2023-07-10 03:39:53.000000 py3seed-0.1.4/tests/test_merge3.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     5116 2023-07-05 06:36:00.000000 py3seed-0.1.4/tests/test_model.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     2083 2023-07-05 06:36:25.000000 py3seed-0.1.4/tests/test_mongosupport.py
```

### Comparing `py3seed-0.1.3/LICENSE` & `py3seed-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.3/PKG-INFO` & `py3seed-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3seed
-Version: 0.1.3
+Version: 0.1.4
 Summary: A package that bootstraps your project by simple data models definition and auto api and user interface generation
 Home-page: https://github.com/okosioc/pyseed
 Author: Samuel Feng
 Author-email: okosioc@gmail.com
 Project-URL: Bug Tracker, https://github.com/okosioc/pyseed/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py3seed-0.1.3/setup.cfg` & `py3seed-0.1.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = py3seed
-version = 0.1.3
+version = 0.1.4
 author = Samuel Feng
 author_email = okosioc@gmail.com
 description = A package that bootstraps your project by simple data models definition and auto api and user interface generation
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/okosioc/pyseed
 project_urls =
```

### Comparing `py3seed-0.1.3/src/py3seed/__init__.py` & `py3seed-0.1.4/src/py3seed/__init__.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.3/src/py3seed/__main__.py` & `py3seed-0.1.4/src/py3seed/__main__.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.3/src/py3seed/admin.py` & `py3seed-0.1.4/src/py3seed/admin.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.3/src/py3seed/cachesupport.py` & `py3seed-0.1.4/src/py3seed/cachesupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.3/src/py3seed/commands/gen.py` & `py3seed-0.1.4/src/py3seed/commands/gen.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.3/src/py3seed/error.py` & `py3seed-0.1.4/src/py3seed/error.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.3/src/py3seed/inflection.py` & `py3seed-0.1.4/src/py3seed/inflection.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.3/src/py3seed/log.py` & `py3seed-0.1.4/src/py3seed/log.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.3/src/py3seed/merge3.py` & `py3seed-0.1.4/src/py3seed/merge3.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.3/src/py3seed/model.py` & `py3seed-0.1.4/src/py3seed/model.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.3/src/py3seed/mongosupport.py` & `py3seed-0.1.4/src/py3seed/mongosupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.3/src/py3seed/utils.py` & `py3seed-0.1.4/src/py3seed/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -322,15 +322,15 @@
             col_name = col['name']
             if not col_name:
                 pass
             elif col_name == '-':
                 pass
             elif col_name.replace('.', '').isdigit():
                 # Need to get fields under a group
-                yield get_layout_fields(col['rows'])
+                yield from get_layout_fields(col['rows'])
             else:
                 # Return current level field names, do not recursively parse inner object/array
                 yield col_name
 
 
 class Pagination(object):
     """ Pagination support. """
```

### Comparing `py3seed-0.1.3/src/py3seed/websupport.py` & `py3seed-0.1.4/src/py3seed/websupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.3/src/py3seed.egg-info/PKG-INFO` & `py3seed-0.1.4/src/py3seed.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3seed
-Version: 0.1.3
+Version: 0.1.4
 Summary: A package that bootstraps your project by simple data models definition and auto api and user interface generation
 Home-page: https://github.com/okosioc/pyseed
 Author: Samuel Feng
 Author-email: okosioc@gmail.com
 Project-URL: Bug Tracker, https://github.com/okosioc/pyseed/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py3seed-0.1.3/src/py3seed.egg-info/SOURCES.txt` & `py3seed-0.1.4/src/py3seed.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.3/tests/test_cachesupport.py` & `py3seed-0.1.4/tests/test_cachesupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.3/tests/test_gen.py` & `py3seed-0.1.4/tests/test_gen.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.3/tests/test_merge3.py` & `py3seed-0.1.4/tests/test_merge3.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.3/tests/test_model.py` & `py3seed-0.1.4/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.3/tests/test_mongosupport.py` & `py3seed-0.1.4/tests/test_mongosupport.py`

 * *Files identical despite different names*

