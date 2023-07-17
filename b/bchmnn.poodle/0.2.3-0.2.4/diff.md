# Comparing `tmp/bchmnn.poodle-0.2.3.tar.gz` & `tmp/bchmnn.poodle-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bchmnn.poodle-0.2.3.tar", last modified: Mon Jul 17 15:26:34 2023, max compression
+gzip compressed data, was "bchmnn.poodle-0.2.4.tar", last modified: Mon Jul 17 15:52:58 2023, max compression
```

## Comparing `bchmnn.poodle-0.2.3.tar` & `bchmnn.poodle-0.2.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:26:34.099934 bchmnn.poodle-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-17 15:25:50.000000 bchmnn.poodle-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    44286 2023-07-17 15:26:34.099934 bchmnn.poodle-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-07-17 15:25:50.000000 bchmnn.poodle-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:26:34.095934 bchmnn.poodle-0.2.3/bchmnn.poodle.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    44286 2023-07-17 15:26:34.000000 bchmnn.poodle-0.2.3/bchmnn.poodle.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-17 15:26:34.000000 bchmnn.poodle-0.2.3/bchmnn.poodle.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 15:26:34.000000 bchmnn.poodle-0.2.3/bchmnn.poodle.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-17 15:26:34.000000 bchmnn.poodle-0.2.3/bchmnn.poodle.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-17 15:26:34.000000 bchmnn.poodle-0.2.3/bchmnn.poodle.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:26:34.095934 bchmnn.poodle-0.2.3/poodle/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-17 15:25:50.000000 bchmnn.poodle-0.2.3/poodle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-07-17 15:25:50.000000 bchmnn.poodle-0.2.3/poodle/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-17 15:25:50.000000 bchmnn.poodle-0.2.3/poodle/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-07-17 15:25:50.000000 bchmnn.poodle-0.2.3/poodle/corews.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-17 15:25:50.000000 bchmnn.poodle-0.2.3/poodle/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     7828 2023-07-17 15:25:50.000000 bchmnn.poodle-0.2.3/poodle/poodle.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:25:50.000000 bchmnn.poodle-0.2.3/poodle/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:26:34.095934 bchmnn.poodle-0.2.3/poodle/types/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-17 15:25:50.000000 bchmnn.poodle-0.2.3/poodle/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26959 2023-07-17 15:25:50.000000 bchmnn.poodle-0.2.3/poodle/types/assign.py
--rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-07-17 15:25:50.000000 bchmnn.poodle-0.2.3/poodle/types/course.py
--rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-07-17 15:25:50.000000 bchmnn.poodle-0.2.3/poodle/types/courses.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-17 15:25:50.000000 bchmnn.poodle-0.2.3/poodle/types/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-17 15:25:50.000000 bchmnn.poodle-0.2.3/poodle/types/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-17 15:25:50.000000 bchmnn.poodle-0.2.3/poodle/types/jsonable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-17 15:25:50.000000 bchmnn.poodle-0.2.3/poodle/types/methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     7680 2023-07-17 15:25:50.000000 bchmnn.poodle-0.2.3/poodle/types/site.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-17 15:25:50.000000 bchmnn.poodle-0.2.3/poodle/types/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-17 15:25:50.000000 bchmnn.poodle-0.2.3/poodle/types/ws.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:26:34.099934 bchmnn.poodle-0.2.3/poodle/util/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-17 15:25:50.000000 bchmnn.poodle-0.2.3/poodle/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-17 15:25:50.000000 bchmnn.poodle-0.2.3/poodle/util/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-17 15:25:50.000000 bchmnn.poodle-0.2.3/poodle/util/loggable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-17 15:25:50.000000 bchmnn.poodle-0.2.3/poodle/util/parse_form.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-17 15:25:50.000000 bchmnn.poodle-0.2.3/poodle/util/tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-17 15:25:50.000000 bchmnn.poodle-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 15:26:34.099934 bchmnn.poodle-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:52:58.595575 bchmnn.poodle-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-17 15:52:20.000000 bchmnn.poodle-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    44286 2023-07-17 15:52:58.595575 bchmnn.poodle-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-07-17 15:52:20.000000 bchmnn.poodle-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:52:58.595575 bchmnn.poodle-0.2.4/bchmnn.poodle.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    44286 2023-07-17 15:52:58.000000 bchmnn.poodle-0.2.4/bchmnn.poodle.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-17 15:52:58.000000 bchmnn.poodle-0.2.4/bchmnn.poodle.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 15:52:58.000000 bchmnn.poodle-0.2.4/bchmnn.poodle.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-17 15:52:58.000000 bchmnn.poodle-0.2.4/bchmnn.poodle.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-17 15:52:58.000000 bchmnn.poodle-0.2.4/bchmnn.poodle.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:52:58.595575 bchmnn.poodle-0.2.4/poodle/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-17 15:52:20.000000 bchmnn.poodle-0.2.4/poodle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-07-17 15:52:20.000000 bchmnn.poodle-0.2.4/poodle/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-17 15:52:20.000000 bchmnn.poodle-0.2.4/poodle/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-07-17 15:52:20.000000 bchmnn.poodle-0.2.4/poodle/corews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-17 15:52:20.000000 bchmnn.poodle-0.2.4/poodle/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7828 2023-07-17 15:52:20.000000 bchmnn.poodle-0.2.4/poodle/poodle.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:52:20.000000 bchmnn.poodle-0.2.4/poodle/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:52:58.595575 bchmnn.poodle-0.2.4/poodle/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-17 15:52:20.000000 bchmnn.poodle-0.2.4/poodle/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26959 2023-07-17 15:52:20.000000 bchmnn.poodle-0.2.4/poodle/types/assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-07-17 15:52:20.000000 bchmnn.poodle-0.2.4/poodle/types/course.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-07-17 15:52:20.000000 bchmnn.poodle-0.2.4/poodle/types/courses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-17 15:52:20.000000 bchmnn.poodle-0.2.4/poodle/types/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-17 15:52:20.000000 bchmnn.poodle-0.2.4/poodle/types/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-17 15:52:20.000000 bchmnn.poodle-0.2.4/poodle/types/jsonable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-17 15:52:20.000000 bchmnn.poodle-0.2.4/poodle/types/methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7680 2023-07-17 15:52:20.000000 bchmnn.poodle-0.2.4/poodle/types/site.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-17 15:52:20.000000 bchmnn.poodle-0.2.4/poodle/types/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-17 15:52:20.000000 bchmnn.poodle-0.2.4/poodle/types/ws.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:52:58.595575 bchmnn.poodle-0.2.4/poodle/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-17 15:52:20.000000 bchmnn.poodle-0.2.4/poodle/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-17 15:52:20.000000 bchmnn.poodle-0.2.4/poodle/util/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-17 15:52:20.000000 bchmnn.poodle-0.2.4/poodle/util/loggable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-17 15:52:20.000000 bchmnn.poodle-0.2.4/poodle/util/parse_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-17 15:52:20.000000 bchmnn.poodle-0.2.4/poodle/util/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-17 15:52:20.000000 bchmnn.poodle-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 15:52:58.595575 bchmnn.poodle-0.2.4/setup.cfg
```

### Comparing `bchmnn.poodle-0.2.3/LICENSE` & `bchmnn.poodle-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bchmnn.poodle-0.2.3/PKG-INFO` & `bchmnn.poodle-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bchmnn.poodle
-Version: 0.2.3
+Version: 0.2.4
 Summary: Python Moodle SDK
 Author-email: Jacob Bachmann <jacob.bachmann@posteo.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `bchmnn.poodle-0.2.3/README.md` & `bchmnn.poodle-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `bchmnn.poodle-0.2.3/bchmnn.poodle.egg-info/PKG-INFO` & `bchmnn.poodle-0.2.4/bchmnn.poodle.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bchmnn.poodle
-Version: 0.2.3
+Version: 0.2.4
 Summary: Python Moodle SDK
 Author-email: Jacob Bachmann <jacob.bachmann@posteo.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `bchmnn.poodle-0.2.3/bchmnn.poodle.egg-info/SOURCES.txt` & `bchmnn.poodle-0.2.4/bchmnn.poodle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bchmnn.poodle-0.2.3/poodle/auth.py` & `bchmnn.poodle-0.2.4/poodle/auth.py`

 * *Files identical despite different names*

### Comparing `bchmnn.poodle-0.2.3/poodle/corews.py` & `bchmnn.poodle-0.2.4/poodle/corews.py`

 * *Files identical despite different names*

### Comparing `bchmnn.poodle-0.2.3/poodle/credentials.py` & `bchmnn.poodle-0.2.4/poodle/credentials.py`

 * *Files identical despite different names*

### Comparing `bchmnn.poodle-0.2.3/poodle/poodle.py` & `bchmnn.poodle-0.2.4/poodle/poodle.py`

 * *Files identical despite different names*

### Comparing `bchmnn.poodle-0.2.3/poodle/types/assign.py` & `bchmnn.poodle-0.2.4/poodle/types/assign.py`

 * *Files identical despite different names*

### Comparing `bchmnn.poodle-0.2.3/poodle/types/course.py` & `bchmnn.poodle-0.2.4/poodle/types/course.py`

 * *Files identical despite different names*

### Comparing `bchmnn.poodle-0.2.3/poodle/types/courses.py` & `bchmnn.poodle-0.2.4/poodle/types/courses.py`

 * *Files identical despite different names*

### Comparing `bchmnn.poodle-0.2.3/poodle/types/exception.py` & `bchmnn.poodle-0.2.4/poodle/types/exception.py`

 * *Files identical despite different names*

### Comparing `bchmnn.poodle-0.2.3/poodle/types/methods.py` & `bchmnn.poodle-0.2.4/poodle/types/methods.py`

 * *Files identical despite different names*

### Comparing `bchmnn.poodle-0.2.3/poodle/types/site.py` & `bchmnn.poodle-0.2.4/poodle/types/site.py`

 * *Files identical despite different names*

### Comparing `bchmnn.poodle-0.2.3/poodle/types/tag.py` & `bchmnn.poodle-0.2.4/poodle/types/tag.py`

 * *Files identical despite different names*

### Comparing `bchmnn.poodle-0.2.3/poodle/types/ws.py` & `bchmnn.poodle-0.2.4/poodle/types/ws.py`

 * *Files identical despite different names*

### Comparing `bchmnn.poodle-0.2.3/poodle/util/cache.py` & `bchmnn.poodle-0.2.4/poodle/util/cache.py`

 * *Files identical despite different names*

### Comparing `bchmnn.poodle-0.2.3/poodle/util/loggable.py` & `bchmnn.poodle-0.2.4/poodle/util/loggable.py`

 * *Files identical despite different names*

### Comparing `bchmnn.poodle-0.2.3/poodle/util/parse_form.py` & `bchmnn.poodle-0.2.4/poodle/util/parse_form.py`

 * *Files identical despite different names*

### Comparing `bchmnn.poodle-0.2.3/pyproject.toml` & `bchmnn.poodle-0.2.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bchmnn.poodle"
-version = "0.2.3"
+version = "0.2.4"
 description = "Python Moodle SDK"
 readme = "README.md"
 authors = [{ name = "Jacob Bachmann", email = "jacob.bachmann@posteo.de" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
@@ -38,15 +38,15 @@
 [project.urls]
 Homepage = "https://github.com/bchmnn/poodle"
 
 [tool.setuptools.package-data]
 "poodle" = ["py.typed"]
 
 [tool.bumpver]
-current_version = "0.2.3"
+current_version = "0.2.4"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "feat: release v{new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

