# Comparing `tmp/ckanext-list-2.1.7.tar.gz` & `tmp/ckanext-list-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-list-2.1.7.tar", last modified: Tue Apr 11 08:22:42 2023, max compression
+gzip compressed data, was "ckanext-list-2.1.8.tar", last modified: Mon Jul 17 08:19:24 2023, max compression
```

## Comparing `ckanext-list-2.1.7.tar` & `ckanext-list-2.1.8.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:22:42.488824 ckanext-list-2.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-11 08:22:30.000000 ckanext-list-2.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-04-11 08:22:42.488824 ckanext-list-2.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-04-11 08:22:30.000000 ckanext-list-2.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:22:42.484824 ckanext-list-2.1.7/ckanext/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-11 08:22:30.000000 ckanext-list-2.1.7/ckanext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:22:42.488824 ckanext-list-2.1.7/ckanext/list/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-11 08:22:30.000000 ckanext-list-2.1.7/ckanext/list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-11 08:22:30.000000 ckanext-list-2.1.7/ckanext/list/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:22:42.488824 ckanext-list-2.1.7/ckanext/list/logic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:22:30.000000 ckanext-list-2.1.7/ckanext/list/logic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-11 08:22:30.000000 ckanext-list-2.1.7/ckanext/list/logic/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-04-11 08:22:30.000000 ckanext-list-2.1.7/ckanext/list/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:22:42.484824 ckanext-list-2.1.7/ckanext/list/theme/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:22:42.488824 ckanext-list-2.1.7/ckanext/list/theme/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:22:42.488824 ckanext-list-2.1.7/ckanext/list/theme/assets/less/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-11 08:22:30.000000 ckanext-list-2.1.7/ckanext/list/theme/assets/less/list.less
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-11 08:22:30.000000 ckanext-list-2.1.7/ckanext/list/theme/assets/less/view-controls.less
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:22:42.488824 ckanext-list-2.1.7/ckanext/list/theme/assets/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     9732 2023-04-11 08:22:30.000000 ckanext-list-2.1.7/ckanext/list/theme/assets/scripts/list-view.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:22:42.488824 ckanext-list-2.1.7/ckanext/list/theme/assets/scripts/modules/
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-11 08:22:30.000000 ckanext-list-2.1.7/ckanext/list/theme/assets/scripts/modules/list.js
--rwxr-xr-x   0 runner    (1001) docker     (123)      460 2023-04-11 08:22:30.000000 ckanext-list-2.1.7/ckanext/list/theme/assets/webassets.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:22:42.484824 ckanext-list-2.1.7/ckanext/list/theme/public/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:22:42.488824 ckanext-list-2.1.7/ckanext/list/theme/public/mustache_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-11 08:22:30.000000 ckanext-list-2.1.7/ckanext/list/theme/public/mustache_templates/list.mustache
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:22:42.484824 ckanext-list-2.1.7/ckanext/list/theme/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:22:42.488824 ckanext-list-2.1.7/ckanext/list/theme/templates/list/
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-11 08:22:30.000000 ckanext-list-2.1.7/ckanext/list/theme/templates/list/list_form.html
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-11 08:22:30.000000 ckanext-list-2.1.7/ckanext/list/theme/templates/list/list_view.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:22:42.488824 ckanext-list-2.1.7/ckanext_list.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-04-11 08:22:42.000000 ckanext-list-2.1.7/ckanext_list.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-11 08:22:42.000000 ckanext-list-2.1.7/ckanext_list.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:22:42.000000 ckanext-list-2.1.7/ckanext_list.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-11 08:22:42.000000 ckanext-list-2.1.7/ckanext_list.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:22:42.000000 ckanext-list-2.1.7/ckanext_list.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-11 08:22:42.000000 ckanext-list-2.1.7/ckanext_list.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-11 08:22:42.000000 ckanext-list-2.1.7/ckanext_list.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:22:42.484824 ckanext-list-2.1.7/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:22:42.488824 ckanext-list-2.1.7/docs/_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-11 08:22:30.000000 ckanext-list-2.1.7/docs/_scripts/gen_api_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-11 08:22:30.000000 ckanext-list-2.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 08:22:42.488824 ckanext-list-2.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-11 08:22:30.000000 ckanext-list-2.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:22:42.488824 ckanext-list-2.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-11 08:22:30.000000 ckanext-list-2.1.7/tests/test_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-11 08:22:30.000000 ckanext-list-2.1.7/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-04-11 08:22:30.000000 ckanext-list-2.1.7/tests/test_validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:19:24.656398 ckanext-list-2.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-17 08:19:13.000000 ckanext-list-2.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-07-17 08:19:24.656398 ckanext-list-2.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-07-17 08:19:13.000000 ckanext-list-2.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:19:24.652398 ckanext-list-2.1.8/ckanext/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-17 08:19:13.000000 ckanext-list-2.1.8/ckanext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:19:24.652398 ckanext-list-2.1.8/ckanext/list/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-17 08:19:13.000000 ckanext-list-2.1.8/ckanext/list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-17 08:19:13.000000 ckanext-list-2.1.8/ckanext/list/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:19:24.652398 ckanext-list-2.1.8/ckanext/list/logic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:19:13.000000 ckanext-list-2.1.8/ckanext/list/logic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-17 08:19:13.000000 ckanext-list-2.1.8/ckanext/list/logic/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-07-17 08:19:13.000000 ckanext-list-2.1.8/ckanext/list/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:19:24.652398 ckanext-list-2.1.8/ckanext/list/theme/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:19:24.652398 ckanext-list-2.1.8/ckanext/list/theme/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:19:24.652398 ckanext-list-2.1.8/ckanext/list/theme/assets/less/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-17 08:19:13.000000 ckanext-list-2.1.8/ckanext/list/theme/assets/less/list.less
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-17 08:19:13.000000 ckanext-list-2.1.8/ckanext/list/theme/assets/less/view-controls.less
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:19:24.652398 ckanext-list-2.1.8/ckanext/list/theme/assets/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     9732 2023-07-17 08:19:13.000000 ckanext-list-2.1.8/ckanext/list/theme/assets/scripts/list-view.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:19:24.656398 ckanext-list-2.1.8/ckanext/list/theme/assets/scripts/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-17 08:19:13.000000 ckanext-list-2.1.8/ckanext/list/theme/assets/scripts/modules/list.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)      460 2023-07-17 08:19:13.000000 ckanext-list-2.1.8/ckanext/list/theme/assets/webassets.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:19:24.652398 ckanext-list-2.1.8/ckanext/list/theme/public/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:19:24.656398 ckanext-list-2.1.8/ckanext/list/theme/public/mustache_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-17 08:19:13.000000 ckanext-list-2.1.8/ckanext/list/theme/public/mustache_templates/list.mustache
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:19:24.652398 ckanext-list-2.1.8/ckanext/list/theme/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:19:24.656398 ckanext-list-2.1.8/ckanext/list/theme/templates/list/
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-17 08:19:13.000000 ckanext-list-2.1.8/ckanext/list/theme/templates/list/list_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-17 08:19:13.000000 ckanext-list-2.1.8/ckanext/list/theme/templates/list/list_view.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:19:24.656398 ckanext-list-2.1.8/ckanext_list.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-07-17 08:19:24.000000 ckanext-list-2.1.8/ckanext_list.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-17 08:19:24.000000 ckanext-list-2.1.8/ckanext_list.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 08:19:24.000000 ckanext-list-2.1.8/ckanext_list.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-17 08:19:24.000000 ckanext-list-2.1.8/ckanext_list.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 08:19:24.000000 ckanext-list-2.1.8/ckanext_list.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-17 08:19:24.000000 ckanext-list-2.1.8/ckanext_list.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-17 08:19:24.000000 ckanext-list-2.1.8/ckanext_list.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:19:24.652398 ckanext-list-2.1.8/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:19:24.656398 ckanext-list-2.1.8/docs/_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-17 08:19:13.000000 ckanext-list-2.1.8/docs/_scripts/gen_api_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-17 08:19:13.000000 ckanext-list-2.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 08:19:24.656398 ckanext-list-2.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-17 08:19:13.000000 ckanext-list-2.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:19:24.656398 ckanext-list-2.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-17 08:19:13.000000 ckanext-list-2.1.8/tests/test_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-17 08:19:13.000000 ckanext-list-2.1.8/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-07-17 08:19:13.000000 ckanext-list-2.1.8/tests/test_validators.py
```

### Comparing `ckanext-list-2.1.7/LICENSE` & `ckanext-list-2.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-list-2.1.7/PKG-INFO` & `ckanext-list-2.1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-list
-Version: 2.1.7
+Version: 2.1.8
 Summary: A CKAN extension that adds a list view for resources.
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-list
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-list/blob/main/CHANGELOG.md
 Keywords: CKAN,data,list
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 <!--header-start-->
-<img src="https://github.com/NaturalHistoryMuseum/ckanext-list/raw/main/.github/nhm-logo.svg" align="left" width="150px" height="100px" hspace="40"/>
+<img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-list
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-list/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-list/actions/workflows/main.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/NaturalHistoryMuseum/ckanext-list/main?style=flat-square)](https://coveralls.io/github/NaturalHistoryMuseum/ckanext-list)
 [![CKAN](https://img.shields.io/badge/ckan-2.9.7-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
 [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg?style=flat-square)](https://www.python.org/)
```

### Comparing `ckanext-list-2.1.7/README.md` & `ckanext-list-2.1.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <!--header-start-->
-<img src="https://github.com/NaturalHistoryMuseum/ckanext-list/raw/main/.github/nhm-logo.svg" align="left" width="150px" height="100px" hspace="40"/>
+<img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-list
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-list/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-list/actions/workflows/main.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/NaturalHistoryMuseum/ckanext-list/main?style=flat-square)](https://coveralls.io/github/NaturalHistoryMuseum/ckanext-list)
 [![CKAN](https://img.shields.io/badge/ckan-2.9.7-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
 [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg?style=flat-square)](https://www.python.org/)
```

### Comparing `ckanext-list-2.1.7/ckanext/list/lib.py` & `ckanext-list-2.1.8/ckanext/list/lib.py`

 * *Files identical despite different names*

### Comparing `ckanext-list-2.1.7/ckanext/list/logic/validators.py` & `ckanext-list-2.1.8/ckanext/list/logic/validators.py`

 * *Files identical despite different names*

### Comparing `ckanext-list-2.1.7/ckanext/list/plugin.py` & `ckanext-list-2.1.8/ckanext/list/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-list-2.1.7/ckanext/list/theme/assets/less/list.less` & `ckanext-list-2.1.8/ckanext/list/theme/assets/less/list.less`

 * *Files identical despite different names*

### Comparing `ckanext-list-2.1.7/ckanext/list/theme/assets/less/view-controls.less` & `ckanext-list-2.1.8/ckanext/list/theme/assets/less/view-controls.less`

 * *Files identical despite different names*

### Comparing `ckanext-list-2.1.7/ckanext/list/theme/assets/scripts/list-view.js` & `ckanext-list-2.1.8/ckanext/list/theme/assets/scripts/list-view.js`

 * *Files identical despite different names*

### Comparing `ckanext-list-2.1.7/ckanext/list/theme/assets/scripts/modules/list.js` & `ckanext-list-2.1.8/ckanext/list/theme/assets/scripts/modules/list.js`

 * *Files identical despite different names*

### Comparing `ckanext-list-2.1.7/ckanext/list/theme/public/mustache_templates/list.mustache` & `ckanext-list-2.1.8/ckanext/list/theme/public/mustache_templates/list.mustache`

 * *Files identical despite different names*

### Comparing `ckanext-list-2.1.7/ckanext/list/theme/templates/list/list_form.html` & `ckanext-list-2.1.8/ckanext/list/theme/templates/list/list_form.html`

 * *Files identical despite different names*

### Comparing `ckanext-list-2.1.7/ckanext/list/theme/templates/list/list_view.html` & `ckanext-list-2.1.8/ckanext/list/theme/templates/list/list_view.html`

 * *Files identical despite different names*

### Comparing `ckanext-list-2.1.7/ckanext_list.egg-info/PKG-INFO` & `ckanext-list-2.1.8/ckanext_list.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-list
-Version: 2.1.7
+Version: 2.1.8
 Summary: A CKAN extension that adds a list view for resources.
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-list
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-list/blob/main/CHANGELOG.md
 Keywords: CKAN,data,list
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 <!--header-start-->
-<img src="https://github.com/NaturalHistoryMuseum/ckanext-list/raw/main/.github/nhm-logo.svg" align="left" width="150px" height="100px" hspace="40"/>
+<img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-list
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-list/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-list/actions/workflows/main.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/NaturalHistoryMuseum/ckanext-list/main?style=flat-square)](https://coveralls.io/github/NaturalHistoryMuseum/ckanext-list)
 [![CKAN](https://img.shields.io/badge/ckan-2.9.7-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
 [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg?style=flat-square)](https://www.python.org/)
```

### Comparing `ckanext-list-2.1.7/ckanext_list.egg-info/SOURCES.txt` & `ckanext-list-2.1.8/ckanext_list.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-list-2.1.7/docs/_scripts/gen_api_pages.py` & `ckanext-list-2.1.8/docs/_scripts/gen_api_pages.py`

 * *Files identical despite different names*

### Comparing `ckanext-list-2.1.7/pyproject.toml` & `ckanext-list-2.1.8/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ckanext-list"
-version = "2.1.7"
+version = "2.1.8"
 description = "A CKAN extension that adds a list view for resources."
 readme = "README.md"
 requires-python = ">=3.6"
 license = { text = "GPL-3.0-or-later" }
 authors = [
     { name = "Natural History Museum", email = "data@nhm.ac.uk" }
 ]
@@ -51,15 +51,15 @@
 exclude = ["tests", "docs"]
 
 [tool.setuptools.package-data]
 "ckanext.list.theme" = ["*", "**/*"]
 
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

### Comparing `ckanext-list-2.1.7/tests/test_lib.py` & `ckanext-list-2.1.8/tests/test_lib.py`

 * *Files identical despite different names*

### Comparing `ckanext-list-2.1.7/tests/test_validators.py` & `ckanext-list-2.1.8/tests/test_validators.py`

 * *Files identical despite different names*

