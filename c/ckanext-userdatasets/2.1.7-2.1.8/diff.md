# Comparing `tmp/ckanext-userdatasets-2.1.7.tar.gz` & `tmp/ckanext-userdatasets-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-userdatasets-2.1.7.tar", last modified: Tue Apr 11 08:36:38 2023, max compression
+gzip compressed data, was "ckanext-userdatasets-2.1.8.tar", last modified: Mon Jul 17 08:27:57 2023, max compression
```

## Comparing `ckanext-userdatasets-2.1.7.tar` & `ckanext-userdatasets-2.1.8.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:36:38.235465 ckanext-userdatasets-2.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-11 08:36:15.000000 ckanext-userdatasets-2.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-04-11 08:36:38.235465 ckanext-userdatasets-2.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-04-11 08:36:15.000000 ckanext-userdatasets-2.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:36:38.227465 ckanext-userdatasets-2.1.7/ckanext/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-11 08:36:15.000000 ckanext-userdatasets-2.1.7/ckanext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:36:38.227465 ckanext-userdatasets-2.1.7/ckanext/userdatasets/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-11 08:36:15.000000 ckanext-userdatasets-2.1.7/ckanext/userdatasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:36:38.227465 ckanext-userdatasets-2.1.7/ckanext/userdatasets/logic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:36:15.000000 ckanext-userdatasets-2.1.7/ckanext/userdatasets/logic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:36:38.231465 ckanext-userdatasets-2.1.7/ckanext/userdatasets/logic/action/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:36:15.000000 ckanext-userdatasets-2.1.7/ckanext/userdatasets/logic/action/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-11 08:36:15.000000 ckanext-userdatasets-2.1.7/ckanext/userdatasets/logic/action/create.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-11 08:36:15.000000 ckanext-userdatasets-2.1.7/ckanext/userdatasets/logic/action/get.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-11 08:36:15.000000 ckanext-userdatasets-2.1.7/ckanext/userdatasets/logic/action/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:36:38.231465 ckanext-userdatasets-2.1.7/ckanext/userdatasets/logic/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:36:15.000000 ckanext-userdatasets-2.1.7/ckanext/userdatasets/logic/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-04-11 08:36:15.000000 ckanext-userdatasets-2.1.7/ckanext/userdatasets/logic/auth/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-04-11 08:36:15.000000 ckanext-userdatasets-2.1.7/ckanext/userdatasets/logic/auth/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-04-11 08:36:15.000000 ckanext-userdatasets-2.1.7/ckanext/userdatasets/logic/auth/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-04-11 08:36:15.000000 ckanext-userdatasets-2.1.7/ckanext/userdatasets/logic/auth/update.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-11 08:36:15.000000 ckanext-userdatasets-2.1.7/ckanext/userdatasets/logic/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-04-11 08:36:15.000000 ckanext-userdatasets-2.1.7/ckanext/userdatasets/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:36:38.235465 ckanext-userdatasets-2.1.7/ckanext_userdatasets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-04-11 08:36:38.000000 ckanext-userdatasets-2.1.7/ckanext_userdatasets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-11 08:36:38.000000 ckanext-userdatasets-2.1.7/ckanext_userdatasets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:36:38.000000 ckanext-userdatasets-2.1.7/ckanext_userdatasets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-11 08:36:38.000000 ckanext-userdatasets-2.1.7/ckanext_userdatasets.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:36:37.000000 ckanext-userdatasets-2.1.7/ckanext_userdatasets.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-11 08:36:38.000000 ckanext-userdatasets-2.1.7/ckanext_userdatasets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-11 08:36:38.000000 ckanext-userdatasets-2.1.7/ckanext_userdatasets.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:36:38.227465 ckanext-userdatasets-2.1.7/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:36:38.235465 ckanext-userdatasets-2.1.7/docs/_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-04-11 08:36:15.000000 ckanext-userdatasets-2.1.7/docs/_scripts/gen_api_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-11 08:36:15.000000 ckanext-userdatasets-2.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 08:36:38.235465 ckanext-userdatasets-2.1.7/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      210 2023-04-11 08:36:15.000000 ckanext-userdatasets-2.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:36:38.235465 ckanext-userdatasets-2.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    14959 2023-04-11 08:36:15.000000 ckanext-userdatasets-2.1.7/tests/test_auth_actions_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)     8523 2023-04-11 08:36:15.000000 ckanext-userdatasets-2.1.7/tests/test_functional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:27:57.497065 ckanext-userdatasets-2.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-17 08:27:43.000000 ckanext-userdatasets-2.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-07-17 08:27:57.497065 ckanext-userdatasets-2.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-07-17 08:27:43.000000 ckanext-userdatasets-2.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:27:57.493065 ckanext-userdatasets-2.1.8/ckanext/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-17 08:27:43.000000 ckanext-userdatasets-2.1.8/ckanext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:27:57.493065 ckanext-userdatasets-2.1.8/ckanext/userdatasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-17 08:27:43.000000 ckanext-userdatasets-2.1.8/ckanext/userdatasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:27:57.493065 ckanext-userdatasets-2.1.8/ckanext/userdatasets/logic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:27:43.000000 ckanext-userdatasets-2.1.8/ckanext/userdatasets/logic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:27:57.493065 ckanext-userdatasets-2.1.8/ckanext/userdatasets/logic/action/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:27:43.000000 ckanext-userdatasets-2.1.8/ckanext/userdatasets/logic/action/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-17 08:27:43.000000 ckanext-userdatasets-2.1.8/ckanext/userdatasets/logic/action/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-17 08:27:43.000000 ckanext-userdatasets-2.1.8/ckanext/userdatasets/logic/action/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-17 08:27:43.000000 ckanext-userdatasets-2.1.8/ckanext/userdatasets/logic/action/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:27:57.493065 ckanext-userdatasets-2.1.8/ckanext/userdatasets/logic/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:27:43.000000 ckanext-userdatasets-2.1.8/ckanext/userdatasets/logic/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-17 08:27:43.000000 ckanext-userdatasets-2.1.8/ckanext/userdatasets/logic/auth/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-07-17 08:27:43.000000 ckanext-userdatasets-2.1.8/ckanext/userdatasets/logic/auth/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-17 08:27:43.000000 ckanext-userdatasets-2.1.8/ckanext/userdatasets/logic/auth/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-07-17 08:27:43.000000 ckanext-userdatasets-2.1.8/ckanext/userdatasets/logic/auth/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-17 08:27:43.000000 ckanext-userdatasets-2.1.8/ckanext/userdatasets/logic/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-17 08:27:43.000000 ckanext-userdatasets-2.1.8/ckanext/userdatasets/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:27:57.497065 ckanext-userdatasets-2.1.8/ckanext_userdatasets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-07-17 08:27:57.000000 ckanext-userdatasets-2.1.8/ckanext_userdatasets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-17 08:27:57.000000 ckanext-userdatasets-2.1.8/ckanext_userdatasets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 08:27:57.000000 ckanext-userdatasets-2.1.8/ckanext_userdatasets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-17 08:27:57.000000 ckanext-userdatasets-2.1.8/ckanext_userdatasets.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 08:27:57.000000 ckanext-userdatasets-2.1.8/ckanext_userdatasets.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-17 08:27:57.000000 ckanext-userdatasets-2.1.8/ckanext_userdatasets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-17 08:27:57.000000 ckanext-userdatasets-2.1.8/ckanext_userdatasets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:27:57.493065 ckanext-userdatasets-2.1.8/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:27:57.497065 ckanext-userdatasets-2.1.8/docs/_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-17 08:27:43.000000 ckanext-userdatasets-2.1.8/docs/_scripts/gen_api_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-07-17 08:27:43.000000 ckanext-userdatasets-2.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 08:27:57.497065 ckanext-userdatasets-2.1.8/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      210 2023-07-17 08:27:43.000000 ckanext-userdatasets-2.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:27:57.497065 ckanext-userdatasets-2.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    14959 2023-07-17 08:27:43.000000 ckanext-userdatasets-2.1.8/tests/test_auth_actions_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8523 2023-07-17 08:27:43.000000 ckanext-userdatasets-2.1.8/tests/test_functional.py
```

### Comparing `ckanext-userdatasets-2.1.7/LICENSE` & `ckanext-userdatasets-2.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-userdatasets-2.1.7/PKG-INFO` & `ckanext-userdatasets-2.1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-userdatasets
-Version: 2.1.7
+Version: 2.1.8
 Summary: A CKAN extension that allows organisation members to create datasets, and edit or delete the datasets they have created.
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-userdatasets
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-userdatasets/blob/main/CHANGELOG.md
 Keywords: CKAN,data,userdatasets
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 <!--header-start-->
-<img src="https://github.com/NaturalHistoryMuseum/ckanext-userdatasets/raw/main/.github/nhm-logo.svg" align="left" width="150px" height="100px" hspace="40"/>
+<img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-userdatasets
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-userdatasets/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-userdatasets/actions/workflows/main.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/NaturalHistoryMuseum/ckanext-userdatasets/main?style=flat-square)](https://coveralls.io/github/NaturalHistoryMuseum/ckanext-userdatasets)
 [![CKAN](https://img.shields.io/badge/ckan-2.9.7-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
 [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg?style=flat-square)](https://www.python.org/)
```

### Comparing `ckanext-userdatasets-2.1.7/README.md` & `ckanext-userdatasets-2.1.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <!--header-start-->
-<img src="https://github.com/NaturalHistoryMuseum/ckanext-userdatasets/raw/main/.github/nhm-logo.svg" align="left" width="150px" height="100px" hspace="40"/>
+<img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-userdatasets
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-userdatasets/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-userdatasets/actions/workflows/main.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/NaturalHistoryMuseum/ckanext-userdatasets/main?style=flat-square)](https://coveralls.io/github/NaturalHistoryMuseum/ckanext-userdatasets)
 [![CKAN](https://img.shields.io/badge/ckan-2.9.7-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
 [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg?style=flat-square)](https://www.python.org/)
```

### Comparing `ckanext-userdatasets-2.1.7/ckanext/userdatasets/logic/action/create.py` & `ckanext-userdatasets-2.1.8/ckanext/userdatasets/logic/action/create.py`

 * *Files identical despite different names*

### Comparing `ckanext-userdatasets-2.1.7/ckanext/userdatasets/logic/action/get.py` & `ckanext-userdatasets-2.1.8/ckanext/userdatasets/logic/action/get.py`

 * *Files identical despite different names*

### Comparing `ckanext-userdatasets-2.1.7/ckanext/userdatasets/logic/action/update.py` & `ckanext-userdatasets-2.1.8/ckanext/userdatasets/logic/action/update.py`

 * *Files identical despite different names*

### Comparing `ckanext-userdatasets-2.1.7/ckanext/userdatasets/logic/auth/auth.py` & `ckanext-userdatasets-2.1.8/ckanext/userdatasets/logic/auth/auth.py`

 * *Files identical despite different names*

### Comparing `ckanext-userdatasets-2.1.7/ckanext/userdatasets/logic/auth/create.py` & `ckanext-userdatasets-2.1.8/ckanext/userdatasets/logic/auth/create.py`

 * *Files identical despite different names*

### Comparing `ckanext-userdatasets-2.1.7/ckanext/userdatasets/logic/auth/delete.py` & `ckanext-userdatasets-2.1.8/ckanext/userdatasets/logic/auth/delete.py`

 * *Files identical despite different names*

### Comparing `ckanext-userdatasets-2.1.7/ckanext/userdatasets/logic/auth/update.py` & `ckanext-userdatasets-2.1.8/ckanext/userdatasets/logic/auth/update.py`

 * *Files identical despite different names*

### Comparing `ckanext-userdatasets-2.1.7/ckanext/userdatasets/logic/validators.py` & `ckanext-userdatasets-2.1.8/ckanext/userdatasets/logic/validators.py`

 * *Files identical despite different names*

### Comparing `ckanext-userdatasets-2.1.7/ckanext/userdatasets/plugin.py` & `ckanext-userdatasets-2.1.8/ckanext/userdatasets/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-userdatasets-2.1.7/ckanext_userdatasets.egg-info/PKG-INFO` & `ckanext-userdatasets-2.1.8/ckanext_userdatasets.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-userdatasets
-Version: 2.1.7
+Version: 2.1.8
 Summary: A CKAN extension that allows organisation members to create datasets, and edit or delete the datasets they have created.
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-userdatasets
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-userdatasets/blob/main/CHANGELOG.md
 Keywords: CKAN,data,userdatasets
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 <!--header-start-->
-<img src="https://github.com/NaturalHistoryMuseum/ckanext-userdatasets/raw/main/.github/nhm-logo.svg" align="left" width="150px" height="100px" hspace="40"/>
+<img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-userdatasets
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-userdatasets/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-userdatasets/actions/workflows/main.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/NaturalHistoryMuseum/ckanext-userdatasets/main?style=flat-square)](https://coveralls.io/github/NaturalHistoryMuseum/ckanext-userdatasets)
 [![CKAN](https://img.shields.io/badge/ckan-2.9.7-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
 [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg?style=flat-square)](https://www.python.org/)
```

### Comparing `ckanext-userdatasets-2.1.7/ckanext_userdatasets.egg-info/SOURCES.txt` & `ckanext-userdatasets-2.1.8/ckanext_userdatasets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-userdatasets-2.1.7/docs/_scripts/gen_api_pages.py` & `ckanext-userdatasets-2.1.8/docs/_scripts/gen_api_pages.py`

 * *Files identical despite different names*

### Comparing `ckanext-userdatasets-2.1.7/pyproject.toml` & `ckanext-userdatasets-2.1.8/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ckanext-userdatasets"
-version = "2.1.7"
+version = "2.1.8"
 description = "A CKAN extension that allows organisation members to create datasets, and edit or delete the datasets they have created."
 readme = "README.md"
 requires-python = ">=3.6"
 license = { text = "GPL-3.0-or-later" }
 authors = [
     { name = "Natural History Museum", email = "data@nhm.ac.uk" }
 ]
@@ -51,15 +51,15 @@
 exclude = ["tests", "docs"]
 
 [tool.setuptools.package-data]
 "ckanext.userdatasets.theme" = ["*", "**/*"]
 
 [tool.commitizen]
 name = "cz_nhm"
-version = "2.1.7"
+version = "2.1.8"
 tag_format = "v$version"
 update_changelog_on_bump = true
 changelog_incremental = true
 version_files = [
     "pyproject.toml:version"
 ]
```

### Comparing `ckanext-userdatasets-2.1.7/tests/test_auth_actions_unit.py` & `ckanext-userdatasets-2.1.8/tests/test_auth_actions_unit.py`

 * *Files identical despite different names*

### Comparing `ckanext-userdatasets-2.1.7/tests/test_functional.py` & `ckanext-userdatasets-2.1.8/tests/test_functional.py`

 * *Files identical despite different names*

