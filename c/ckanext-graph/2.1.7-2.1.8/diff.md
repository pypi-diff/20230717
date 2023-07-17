# Comparing `tmp/ckanext-graph-2.1.7.tar.gz` & `tmp/ckanext-graph-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-graph-2.1.7.tar", last modified: Tue Apr 11 08:20:56 2023, max compression
+gzip compressed data, was "ckanext-graph-2.1.8.tar", last modified: Mon Jul 17 08:23:15 2023, max compression
```

## Comparing `ckanext-graph-2.1.7.tar` & `ckanext-graph-2.1.8.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:20:56.179341 ckanext-graph-2.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-11 08:20:45.000000 ckanext-graph-2.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-04-11 08:20:56.179341 ckanext-graph-2.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-04-11 08:20:45.000000 ckanext-graph-2.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:20:56.175341 ckanext-graph-2.1.7/ckanext/
--rwxr-xr-x   0 runner    (1001) docker     (123)      306 2023-04-11 08:20:45.000000 ckanext-graph-2.1.7/ckanext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:20:56.175341 ckanext-graph-2.1.7/ckanext/graph/
--rwxr-xr-x   0 runner    (1001) docker     (123)      306 2023-04-11 08:20:45.000000 ckanext-graph-2.1.7/ckanext/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-04-11 08:20:45.000000 ckanext-graph-2.1.7/ckanext/graph/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:20:56.175341 ckanext-graph-2.1.7/ckanext/graph/lib/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-11 08:20:45.000000 ckanext-graph-2.1.7/ckanext/graph/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-04-11 08:20:45.000000 ckanext-graph-2.1.7/ckanext/graph/lib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:20:56.179341 ckanext-graph-2.1.7/ckanext/graph/logic/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-11 08:20:45.000000 ckanext-graph-2.1.7/ckanext/graph/logic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-04-11 08:20:45.000000 ckanext-graph-2.1.7/ckanext/graph/logic/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     7593 2023-04-11 08:20:45.000000 ckanext-graph-2.1.7/ckanext/graph/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:20:56.175341 ckanext-graph-2.1.7/ckanext/graph/theme/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:20:56.179341 ckanext-graph-2.1.7/ckanext/graph/theme/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:20:56.179341 ckanext-graph-2.1.7/ckanext/graph/theme/assets/less/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-11 08:20:45.000000 ckanext-graph-2.1.7/ckanext/graph/theme/assets/less/graph.less
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:20:56.175341 ckanext-graph-2.1.7/ckanext/graph/theme/assets/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:20:56.179341 ckanext-graph-2.1.7/ckanext/graph/theme/assets/scripts/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-04-11 08:20:45.000000 ckanext-graph-2.1.7/ckanext/graph/theme/assets/scripts/modules/graph.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:20:56.179341 ckanext-graph-2.1.7/ckanext/graph/theme/assets/vendor/
--rw-r--r--   0 runner    (1001) docker     (123)    41772 2023-04-11 08:20:45.000000 ckanext-graph-2.1.7/ckanext/graph/theme/assets/vendor/excanvas.js
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-04-11 08:20:45.000000 ckanext-graph-2.1.7/ckanext/graph/theme/assets/vendor/jquery.flot.barnumbers.js
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-04-11 08:20:45.000000 ckanext-graph-2.1.7/ckanext/graph/theme/assets/vendor/jquery.flot.categories.js
--rw-r--r--   0 runner    (1001) docker     (123)   122941 2023-04-11 08:20:45.000000 ckanext-graph-2.1.7/ckanext/graph/theme/assets/vendor/jquery.flot.js
--rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-04-11 08:20:45.000000 ckanext-graph-2.1.7/ckanext/graph/theme/assets/vendor/jquery.flot.tickrotor.js
--rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-04-11 08:20:45.000000 ckanext-graph-2.1.7/ckanext/graph/theme/assets/vendor/jquery.flot.time.js
--rwxr-xr-x   0 runner    (1001) docker     (123)      480 2023-04-11 08:20:45.000000 ckanext-graph-2.1.7/ckanext/graph/theme/assets/webassets.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:20:56.175341 ckanext-graph-2.1.7/ckanext/graph/theme/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:20:56.179341 ckanext-graph-2.1.7/ckanext/graph/theme/templates/graph/
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-04-11 08:20:45.000000 ckanext-graph-2.1.7/ckanext/graph/theme/templates/graph/form.html
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-11 08:20:45.000000 ckanext-graph-2.1.7/ckanext/graph/theme/templates/graph/view.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:20:56.179341 ckanext-graph-2.1.7/ckanext_graph.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-04-11 08:20:56.000000 ckanext-graph-2.1.7/ckanext_graph.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-11 08:20:56.000000 ckanext-graph-2.1.7/ckanext_graph.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:20:56.000000 ckanext-graph-2.1.7/ckanext_graph.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-11 08:20:56.000000 ckanext-graph-2.1.7/ckanext_graph.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:20:55.000000 ckanext-graph-2.1.7/ckanext_graph.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-11 08:20:56.000000 ckanext-graph-2.1.7/ckanext_graph.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-11 08:20:56.000000 ckanext-graph-2.1.7/ckanext_graph.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:20:56.175341 ckanext-graph-2.1.7/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:20:56.179341 ckanext-graph-2.1.7/docs/_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-11 08:20:45.000000 ckanext-graph-2.1.7/docs/_scripts/gen_api_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-11 08:20:45.000000 ckanext-graph-2.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 08:20:56.179341 ckanext-graph-2.1.7/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-04-11 08:20:45.000000 ckanext-graph-2.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:20:56.179341 ckanext-graph-2.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-04-11 08:20:45.000000 ckanext-graph-2.1.7/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:23:15.936628 ckanext-graph-2.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-17 08:23:01.000000 ckanext-graph-2.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-07-17 08:23:15.936628 ckanext-graph-2.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-07-17 08:23:01.000000 ckanext-graph-2.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:23:15.932628 ckanext-graph-2.1.8/ckanext/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      306 2023-07-17 08:23:01.000000 ckanext-graph-2.1.8/ckanext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:23:15.932628 ckanext-graph-2.1.8/ckanext/graph/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      306 2023-07-17 08:23:01.000000 ckanext-graph-2.1.8/ckanext/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-07-17 08:23:01.000000 ckanext-graph-2.1.8/ckanext/graph/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:23:15.932628 ckanext-graph-2.1.8/ckanext/graph/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-17 08:23:01.000000 ckanext-graph-2.1.8/ckanext/graph/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-17 08:23:01.000000 ckanext-graph-2.1.8/ckanext/graph/lib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:23:15.932628 ckanext-graph-2.1.8/ckanext/graph/logic/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-17 08:23:01.000000 ckanext-graph-2.1.8/ckanext/graph/logic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-07-17 08:23:01.000000 ckanext-graph-2.1.8/ckanext/graph/logic/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7593 2023-07-17 08:23:01.000000 ckanext-graph-2.1.8/ckanext/graph/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:23:15.932628 ckanext-graph-2.1.8/ckanext/graph/theme/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:23:15.932628 ckanext-graph-2.1.8/ckanext/graph/theme/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:23:15.932628 ckanext-graph-2.1.8/ckanext/graph/theme/assets/less/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-17 08:23:01.000000 ckanext-graph-2.1.8/ckanext/graph/theme/assets/less/graph.less
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:23:15.932628 ckanext-graph-2.1.8/ckanext/graph/theme/assets/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:23:15.932628 ckanext-graph-2.1.8/ckanext/graph/theme/assets/scripts/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-07-17 08:23:01.000000 ckanext-graph-2.1.8/ckanext/graph/theme/assets/scripts/modules/graph.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:23:15.932628 ckanext-graph-2.1.8/ckanext/graph/theme/assets/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)    41772 2023-07-17 08:23:01.000000 ckanext-graph-2.1.8/ckanext/graph/theme/assets/vendor/excanvas.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-07-17 08:23:01.000000 ckanext-graph-2.1.8/ckanext/graph/theme/assets/vendor/jquery.flot.barnumbers.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-07-17 08:23:01.000000 ckanext-graph-2.1.8/ckanext/graph/theme/assets/vendor/jquery.flot.categories.js
+-rw-r--r--   0 runner    (1001) docker     (123)   122941 2023-07-17 08:23:01.000000 ckanext-graph-2.1.8/ckanext/graph/theme/assets/vendor/jquery.flot.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-07-17 08:23:01.000000 ckanext-graph-2.1.8/ckanext/graph/theme/assets/vendor/jquery.flot.tickrotor.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-07-17 08:23:01.000000 ckanext-graph-2.1.8/ckanext/graph/theme/assets/vendor/jquery.flot.time.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)      480 2023-07-17 08:23:01.000000 ckanext-graph-2.1.8/ckanext/graph/theme/assets/webassets.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:23:15.932628 ckanext-graph-2.1.8/ckanext/graph/theme/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:23:15.932628 ckanext-graph-2.1.8/ckanext/graph/theme/templates/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-17 08:23:01.000000 ckanext-graph-2.1.8/ckanext/graph/theme/templates/graph/form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-17 08:23:01.000000 ckanext-graph-2.1.8/ckanext/graph/theme/templates/graph/view.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:23:15.932628 ckanext-graph-2.1.8/ckanext_graph.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-07-17 08:23:15.000000 ckanext-graph-2.1.8/ckanext_graph.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-17 08:23:15.000000 ckanext-graph-2.1.8/ckanext_graph.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 08:23:15.000000 ckanext-graph-2.1.8/ckanext_graph.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-17 08:23:15.000000 ckanext-graph-2.1.8/ckanext_graph.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 08:23:15.000000 ckanext-graph-2.1.8/ckanext_graph.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-17 08:23:15.000000 ckanext-graph-2.1.8/ckanext_graph.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-17 08:23:15.000000 ckanext-graph-2.1.8/ckanext_graph.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:23:15.932628 ckanext-graph-2.1.8/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:23:15.936628 ckanext-graph-2.1.8/docs/_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-17 08:23:01.000000 ckanext-graph-2.1.8/docs/_scripts/gen_api_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-17 08:23:01.000000 ckanext-graph-2.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 08:23:15.936628 ckanext-graph-2.1.8/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-07-17 08:23:01.000000 ckanext-graph-2.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:23:15.936628 ckanext-graph-2.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-07-17 08:23:01.000000 ckanext-graph-2.1.8/tests/test_utils.py
```

### Comparing `ckanext-graph-2.1.7/LICENSE` & `ckanext-graph-2.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-graph-2.1.7/PKG-INFO` & `ckanext-graph-2.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-graph
-Version: 2.1.7
+Version: 2.1.8
 Summary: A CKAN extension that adds a graph view for resources.
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-graph
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-graph/blob/main/CHANGELOG.md
 Keywords: CKAN,data,graph
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 <!--header-start-->
-<img src="https://github.com/NaturalHistoryMuseum/ckanext-graph/raw/main/.github/nhm-logo.svg" align="left" width="150px" height="100px" hspace="40"/>
+<img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-graph
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-graph/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-graph/actions/workflows/main.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/NaturalHistoryMuseum/ckanext-graph/main?style=flat-square)](https://coveralls.io/github/NaturalHistoryMuseum/ckanext-graph)
 [![CKAN](https://img.shields.io/badge/ckan-2.9.7-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
 [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg?style=flat-square)](https://www.python.org/)
```

### Comparing `ckanext-graph-2.1.7/README.md` & `ckanext-graph-2.1.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <!--header-start-->
-<img src="https://github.com/NaturalHistoryMuseum/ckanext-graph/raw/main/.github/nhm-logo.svg" align="left" width="150px" height="100px" hspace="40"/>
+<img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-graph
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-graph/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-graph/actions/workflows/main.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/NaturalHistoryMuseum/ckanext-graph/main?style=flat-square)](https://coveralls.io/github/NaturalHistoryMuseum/ckanext-graph)
 [![CKAN](https://img.shields.io/badge/ckan-2.9.7-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
 [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg?style=flat-square)](https://www.python.org/)
```

### Comparing `ckanext-graph-2.1.7/ckanext/graph/db.py` & `ckanext-graph-2.1.8/ckanext/graph/db.py`

 * *Files identical despite different names*

### Comparing `ckanext-graph-2.1.7/ckanext/graph/lib/utils.py` & `ckanext-graph-2.1.8/ckanext/graph/lib/utils.py`

 * *Files identical despite different names*

### Comparing `ckanext-graph-2.1.7/ckanext/graph/logic/validators.py` & `ckanext-graph-2.1.8/ckanext/graph/logic/validators.py`

 * *Files identical despite different names*

### Comparing `ckanext-graph-2.1.7/ckanext/graph/plugin.py` & `ckanext-graph-2.1.8/ckanext/graph/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-graph-2.1.7/ckanext/graph/theme/assets/scripts/modules/graph.js` & `ckanext-graph-2.1.8/ckanext/graph/theme/assets/scripts/modules/graph.js`

 * *Files identical despite different names*

### Comparing `ckanext-graph-2.1.7/ckanext/graph/theme/assets/vendor/excanvas.js` & `ckanext-graph-2.1.8/ckanext/graph/theme/assets/vendor/excanvas.js`

 * *Files identical despite different names*

### Comparing `ckanext-graph-2.1.7/ckanext/graph/theme/assets/vendor/jquery.flot.barnumbers.js` & `ckanext-graph-2.1.8/ckanext/graph/theme/assets/vendor/jquery.flot.barnumbers.js`

 * *Files identical despite different names*

### Comparing `ckanext-graph-2.1.7/ckanext/graph/theme/assets/vendor/jquery.flot.categories.js` & `ckanext-graph-2.1.8/ckanext/graph/theme/assets/vendor/jquery.flot.categories.js`

 * *Files identical despite different names*

### Comparing `ckanext-graph-2.1.7/ckanext/graph/theme/assets/vendor/jquery.flot.js` & `ckanext-graph-2.1.8/ckanext/graph/theme/assets/vendor/jquery.flot.js`

 * *Files identical despite different names*

### Comparing `ckanext-graph-2.1.7/ckanext/graph/theme/assets/vendor/jquery.flot.tickrotor.js` & `ckanext-graph-2.1.8/ckanext/graph/theme/assets/vendor/jquery.flot.tickrotor.js`

 * *Files identical despite different names*

### Comparing `ckanext-graph-2.1.7/ckanext/graph/theme/assets/vendor/jquery.flot.time.js` & `ckanext-graph-2.1.8/ckanext/graph/theme/assets/vendor/jquery.flot.time.js`

 * *Files identical despite different names*

### Comparing `ckanext-graph-2.1.7/ckanext/graph/theme/templates/graph/form.html` & `ckanext-graph-2.1.8/ckanext/graph/theme/templates/graph/form.html`

 * *Files identical despite different names*

### Comparing `ckanext-graph-2.1.7/ckanext/graph/theme/templates/graph/view.html` & `ckanext-graph-2.1.8/ckanext/graph/theme/templates/graph/view.html`

 * *Files identical despite different names*

### Comparing `ckanext-graph-2.1.7/ckanext_graph.egg-info/PKG-INFO` & `ckanext-graph-2.1.8/ckanext_graph.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-graph
-Version: 2.1.7
+Version: 2.1.8
 Summary: A CKAN extension that adds a graph view for resources.
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-graph
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-graph/blob/main/CHANGELOG.md
 Keywords: CKAN,data,graph
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 <!--header-start-->
-<img src="https://github.com/NaturalHistoryMuseum/ckanext-graph/raw/main/.github/nhm-logo.svg" align="left" width="150px" height="100px" hspace="40"/>
+<img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-graph
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-graph/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-graph/actions/workflows/main.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/NaturalHistoryMuseum/ckanext-graph/main?style=flat-square)](https://coveralls.io/github/NaturalHistoryMuseum/ckanext-graph)
 [![CKAN](https://img.shields.io/badge/ckan-2.9.7-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
 [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg?style=flat-square)](https://www.python.org/)
```

### Comparing `ckanext-graph-2.1.7/ckanext_graph.egg-info/SOURCES.txt` & `ckanext-graph-2.1.8/ckanext_graph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-graph-2.1.7/docs/_scripts/gen_api_pages.py` & `ckanext-graph-2.1.8/docs/_scripts/gen_api_pages.py`

 * *Files identical despite different names*

### Comparing `ckanext-graph-2.1.7/pyproject.toml` & `ckanext-graph-2.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ckanext-graph"
-version = "2.1.7"
+version = "2.1.8"
 description = "A CKAN extension that adds a graph view for resources."
 readme = "README.md"
 requires-python = ">=3.6"
 license = { text = "GPL-3.0-or-later" }
 authors = [
     { name = "Natural History Museum", email = "data@nhm.ac.uk" }
 ]
@@ -51,15 +51,15 @@
 exclude = ["tests", "docs"]
 
 [tool.setuptools.package-data]
 "ckanext.graph.theme" = ["*", "**/*"]
 
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

### Comparing `ckanext-graph-2.1.7/tests/test_utils.py` & `ckanext-graph-2.1.8/tests/test_utils.py`

 * *Files identical despite different names*

