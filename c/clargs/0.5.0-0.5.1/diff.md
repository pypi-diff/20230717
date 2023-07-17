# Comparing `tmp/clargs-0.5.0.tar.gz` & `tmp/clargs-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clargs-0.5.0.tar", last modified: Mon Jul 17 12:10:35 2023, max compression
+gzip compressed data, was "clargs-0.5.1.tar", last modified: Mon Jul 17 12:49:42 2023, max compression
```

## Comparing `clargs-0.5.0.tar` & `clargs-0.5.1.tar`

### file list

```diff
@@ -1,21 +1,34 @@
-drwxr-xr-x   0 reinoud    (501) staff       (20)        0 2023-07-17 12:10:35.819815 clargs-0.5.0/
--rw-r--r--   0 reinoud    (501) staff       (20)     1070 2023-07-10 11:44:42.000000 clargs-0.5.0/LICENCE.txt
--rw-r--r--   0 reinoud    (501) staff       (20)     5677 2023-07-17 12:10:35.819702 clargs-0.5.0/PKG-INFO
--rw-r--r--   0 reinoud    (501) staff       (20)     5144 2023-07-17 10:43:27.000000 clargs-0.5.0/README.md
--rw-r--r--   0 reinoud    (501) staff       (20)      686 2023-07-17 11:39:15.000000 clargs-0.5.0/pyproject.toml
--rw-r--r--   0 reinoud    (501) staff       (20)       38 2023-07-17 12:10:35.819853 clargs-0.5.0/setup.cfg
-drwxr-xr-x   0 reinoud    (501) staff       (20)        0 2023-07-17 12:10:35.817179 clargs-0.5.0/src/
-drwxr-xr-x   0 reinoud    (501) staff       (20)        0 2023-07-17 12:10:35.818532 clargs-0.5.0/src/clargs/
--rw-r--r--   0 reinoud    (501) staff       (20)      620 2023-07-17 10:57:24.000000 clargs-0.5.0/src/clargs/__init__.py
--rw-r--r--   0 reinoud    (501) staff       (20)     9280 2023-07-17 10:57:24.000000 clargs-0.5.0/src/clargs/aap_from_data.py
--rw-r--r--   0 reinoud    (501) staff       (20)     9604 2023-07-17 10:57:24.000000 clargs-0.5.0/src/clargs/clargs.py
--rw-r--r--   0 reinoud    (501) staff       (20)     5600 2023-07-17 11:04:01.000000 clargs-0.5.0/src/clargs/docsparser.py
--rw-r--r--   0 reinoud    (501) staff       (20)      988 2023-07-17 11:16:40.000000 clargs-0.5.0/src/clargs/helper_types.py
-drwxr-xr-x   0 reinoud    (501) staff       (20)        0 2023-07-17 12:10:35.819017 clargs-0.5.0/src/clargs.egg-info/
--rw-r--r--   0 reinoud    (501) staff       (20)     5677 2023-07-17 12:10:35.000000 clargs-0.5.0/src/clargs.egg-info/PKG-INFO
--rw-r--r--   0 reinoud    (501) staff       (20)      340 2023-07-17 12:10:35.000000 clargs-0.5.0/src/clargs.egg-info/SOURCES.txt
--rw-r--r--   0 reinoud    (501) staff       (20)        1 2023-07-17 12:10:35.000000 clargs-0.5.0/src/clargs.egg-info/dependency_links.txt
--rw-r--r--   0 reinoud    (501) staff       (20)        7 2023-07-17 12:10:35.000000 clargs-0.5.0/src/clargs.egg-info/top_level.txt
-drwxr-xr-x   0 reinoud    (501) staff       (20)        0 2023-07-17 12:10:35.819279 clargs-0.5.0/test/
--rw-r--r--   0 reinoud    (501) staff       (20)     6519 2023-07-17 10:57:24.000000 clargs-0.5.0/test/test_docsparser.py
--rw-r--r--   0 reinoud    (501) staff       (20)    23344 2023-07-17 11:48:06.000000 clargs-0.5.0/test/test_simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:49:42.819741 clargs-0.5.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:49:42.819741 clargs-0.5.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:49:42.819741 clargs-0.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-17 12:49:33.000000 clargs-0.5.1/.github/workflows/run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-17 12:49:33.000000 clargs-0.5.1/.github/workflows/upload.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-17 12:49:33.000000 clargs-0.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-17 12:49:33.000000 clargs-0.5.1/LICENCE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-07-17 12:49:42.819741 clargs-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-07-17 12:49:33.000000 clargs-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:49:42.819741 clargs-0.5.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-17 12:49:33.000000 clargs-0.5.1/examples/0_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-17 12:49:33.000000 clargs-0.5.1/examples/1_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-07-17 12:49:33.000000 clargs-0.5.1/examples/2_show_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-07-17 12:49:33.000000 clargs-0.5.1/examples/3_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-07-17 12:49:33.000000 clargs-0.5.1/examples/4_parse_groups.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-07-17 12:49:33.000000 clargs-0.5.1/examples/__generate_example_output__.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-17 12:49:33.000000 clargs-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 12:49:42.819741 clargs-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:49:42.819741 clargs-0.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:49:42.819741 clargs-0.5.1/src/clargs/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-17 12:49:33.000000 clargs-0.5.1/src/clargs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9280 2023-07-17 12:49:33.000000 clargs-0.5.1/src/clargs/aap_from_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9604 2023-07-17 12:49:33.000000 clargs-0.5.1/src/clargs/clargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-07-17 12:49:33.000000 clargs-0.5.1/src/clargs/docsparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-17 12:49:33.000000 clargs-0.5.1/src/clargs/helper_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:49:42.819741 clargs-0.5.1/src/clargs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-07-17 12:49:42.000000 clargs-0.5.1/src/clargs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-17 12:49:42.000000 clargs-0.5.1/src/clargs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 12:49:42.000000 clargs-0.5.1/src/clargs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-17 12:49:42.000000 clargs-0.5.1/src/clargs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:49:42.819741 clargs-0.5.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-07-17 12:49:33.000000 clargs-0.5.1/test/test_docsparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23344 2023-07-17 12:49:33.000000 clargs-0.5.1/test/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-17 12:49:33.000000 clargs-0.5.1/tox.ini
```

### Comparing `clargs-0.5.0/LICENCE.txt` & `clargs-0.5.1/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `clargs-0.5.0/PKG-INFO` & `clargs-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: clargs
-Version: 0.5.0
+Version: 0.5.1
 Summary: Easily generate commandline apps from your functions, based on type hints
 Author-email: Claude <pypi@claude.nl>
 Project-URL: Homepage, https://github.com/reinhrst/clargs
 Project-URL: Bug Tracker, https://github.com/reinhrst/clargs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 
 # Clargs
 
 The goal of the `clargs` package is to create commandline interfaces from function signatures.
```

### Comparing `clargs-0.5.0/README.md` & `clargs-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `clargs-0.5.0/src/clargs/__init__.py` & `clargs-0.5.1/src/clargs/__init__.py`

 * *Files identical despite different names*

### Comparing `clargs-0.5.0/src/clargs/aap_from_data.py` & `clargs-0.5.1/src/clargs/aap_from_data.py`

 * *Files identical despite different names*

### Comparing `clargs-0.5.0/src/clargs/clargs.py` & `clargs-0.5.1/src/clargs/clargs.py`

 * *Files identical despite different names*

### Comparing `clargs-0.5.0/src/clargs/docsparser.py` & `clargs-0.5.1/src/clargs/docsparser.py`

 * *Files identical despite different names*

### Comparing `clargs-0.5.0/src/clargs/helper_types.py` & `clargs-0.5.1/src/clargs/helper_types.py`

 * *Files identical despite different names*

### Comparing `clargs-0.5.0/src/clargs.egg-info/PKG-INFO` & `clargs-0.5.1/src/clargs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: clargs
-Version: 0.5.0
+Version: 0.5.1
 Summary: Easily generate commandline apps from your functions, based on type hints
 Author-email: Claude <pypi@claude.nl>
 Project-URL: Homepage, https://github.com/reinhrst/clargs
 Project-URL: Bug Tracker, https://github.com/reinhrst/clargs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 
 # Clargs
 
 The goal of the `clargs` package is to create commandline interfaces from function signatures.
```

### Comparing `clargs-0.5.0/test/test_docsparser.py` & `clargs-0.5.1/test/test_docsparser.py`

 * *Files identical despite different names*

### Comparing `clargs-0.5.0/test/test_simple.py` & `clargs-0.5.1/test/test_simple.py`

 * *Files identical despite different names*

