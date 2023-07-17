# Comparing `tmp/ckanext-gbif-2.1.7.tar.gz` & `tmp/ckanext-gbif-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-gbif-2.1.7.tar", last modified: Tue Apr 11 08:19:46 2023, max compression
+gzip compressed data, was "ckanext-gbif-2.1.8.tar", last modified: Mon Jul 17 08:18:13 2023, max compression
```

## Comparing `ckanext-gbif-2.1.7.tar` & `ckanext-gbif-2.1.8.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:19:46.099636 ckanext-gbif-2.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-11 08:19:30.000000 ckanext-gbif-2.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-04-11 08:19:46.099636 ckanext-gbif-2.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-04-11 08:19:30.000000 ckanext-gbif-2.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:19:46.095636 ckanext-gbif-2.1.7/ckanext/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-11 08:19:30.000000 ckanext-gbif-2.1.7/ckanext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:19:46.095636 ckanext-gbif-2.1.7/ckanext/gbif/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-11 08:19:30.000000 ckanext-gbif-2.1.7/ckanext/gbif/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:19:46.095636 ckanext-gbif-2.1.7/ckanext/gbif/lib/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-11 08:19:30.000000 ckanext-gbif-2.1.7/ckanext/gbif/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9966 2023-04-11 08:19:30.000000 ckanext-gbif-2.1.7/ckanext/gbif/lib/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-04-11 08:19:30.000000 ckanext-gbif-2.1.7/ckanext/gbif/lib/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:19:46.095636 ckanext-gbif-2.1.7/ckanext/gbif/logic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:19:30.000000 ckanext-gbif-2.1.7/ckanext/gbif/logic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-11 08:19:30.000000 ckanext-gbif-2.1.7/ckanext/gbif/logic/action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-11 08:19:30.000000 ckanext-gbif-2.1.7/ckanext/gbif/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:19:46.095636 ckanext-gbif-2.1.7/ckanext/gbif/routes/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-11 08:19:30.000000 ckanext-gbif-2.1.7/ckanext/gbif/routes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-04-11 08:19:30.000000 ckanext-gbif-2.1.7/ckanext/gbif/routes/gbif.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:19:46.091636 ckanext-gbif-2.1.7/ckanext/gbif/theme/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:19:46.095636 ckanext-gbif-2.1.7/ckanext/gbif/theme/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:19:46.095636 ckanext-gbif-2.1.7/ckanext/gbif/theme/assets/less/
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-04-11 08:19:30.000000 ckanext-gbif-2.1.7/ckanext/gbif/theme/assets/less/gbif.less
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:19:46.095636 ckanext-gbif-2.1.7/ckanext/gbif/theme/assets/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-11 08:19:30.000000 ckanext-gbif-2.1.7/ckanext/gbif/theme/assets/scripts/gbif-dqi.js
--rwxr-xr-x   0 runner    (1001) docker     (123)      250 2023-04-11 08:19:30.000000 ckanext-gbif-2.1.7/ckanext/gbif/theme/assets/webassets.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:19:46.091636 ckanext-gbif-2.1.7/ckanext/gbif/theme/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:19:46.095636 ckanext-gbif-2.1.7/ckanext/gbif/theme/templates/record/
--rwxr-xr-x   0 runner    (1001) docker     (123)      310 2023-04-11 08:19:30.000000 ckanext-gbif-2.1.7/ckanext/gbif/theme/templates/record/dwc.html
--rwxr-xr-x   0 runner    (1001) docker     (123)     7148 2023-04-11 08:19:30.000000 ckanext-gbif-2.1.7/ckanext/gbif/theme/templates/record/gbif.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:19:46.095636 ckanext-gbif-2.1.7/ckanext/gbif/theme/templates/record/snippets/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-11 08:19:30.000000 ckanext-gbif-2.1.7/ckanext/gbif/theme/templates/record/snippets/external_links.html
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-11 08:19:30.000000 ckanext-gbif-2.1.7/ckanext/gbif/theme/templates/record/snippets/gbif-errors.html
--rwxr-xr-x   0 runner    (1001) docker     (123)      595 2023-04-11 08:19:30.000000 ckanext-gbif-2.1.7/ckanext/gbif/theme/templates/record/specimen.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:19:46.095636 ckanext-gbif-2.1.7/ckanext_gbif.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-04-11 08:19:46.000000 ckanext-gbif-2.1.7/ckanext_gbif.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-11 08:19:46.000000 ckanext-gbif-2.1.7/ckanext_gbif.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:19:46.000000 ckanext-gbif-2.1.7/ckanext_gbif.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-11 08:19:46.000000 ckanext-gbif-2.1.7/ckanext_gbif.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:19:45.000000 ckanext-gbif-2.1.7/ckanext_gbif.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-11 08:19:46.000000 ckanext-gbif-2.1.7/ckanext_gbif.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-11 08:19:46.000000 ckanext-gbif-2.1.7/ckanext_gbif.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:19:46.091636 ckanext-gbif-2.1.7/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:19:46.095636 ckanext-gbif-2.1.7/docs/_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-11 08:19:30.000000 ckanext-gbif-2.1.7/docs/_scripts/gen_api_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-11 08:19:30.000000 ckanext-gbif-2.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 08:19:46.099636 ckanext-gbif-2.1.7/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      202 2023-04-11 08:19:30.000000 ckanext-gbif-2.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:19:46.099636 ckanext-gbif-2.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-04-11 08:19:30.000000 ckanext-gbif-2.1.7/tests/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-04-11 08:19:30.000000 ckanext-gbif-2.1.7/tests/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:18:13.515346 ckanext-gbif-2.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-17 08:17:58.000000 ckanext-gbif-2.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-07-17 08:18:13.515346 ckanext-gbif-2.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-07-17 08:17:58.000000 ckanext-gbif-2.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:18:13.503346 ckanext-gbif-2.1.8/ckanext/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-17 08:17:58.000000 ckanext-gbif-2.1.8/ckanext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:18:13.507346 ckanext-gbif-2.1.8/ckanext/gbif/
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-17 08:17:58.000000 ckanext-gbif-2.1.8/ckanext/gbif/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:18:13.507346 ckanext-gbif-2.1.8/ckanext/gbif/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-17 08:17:58.000000 ckanext-gbif-2.1.8/ckanext/gbif/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9966 2023-07-17 08:17:58.000000 ckanext-gbif-2.1.8/ckanext/gbif/lib/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-07-17 08:17:58.000000 ckanext-gbif-2.1.8/ckanext/gbif/lib/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:18:13.507346 ckanext-gbif-2.1.8/ckanext/gbif/logic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:17:58.000000 ckanext-gbif-2.1.8/ckanext/gbif/logic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-17 08:17:58.000000 ckanext-gbif-2.1.8/ckanext/gbif/logic/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-07-17 08:17:58.000000 ckanext-gbif-2.1.8/ckanext/gbif/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:18:13.507346 ckanext-gbif-2.1.8/ckanext/gbif/routes/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-17 08:17:58.000000 ckanext-gbif-2.1.8/ckanext/gbif/routes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-17 08:17:58.000000 ckanext-gbif-2.1.8/ckanext/gbif/routes/gbif.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:18:13.499346 ckanext-gbif-2.1.8/ckanext/gbif/theme/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:18:13.507346 ckanext-gbif-2.1.8/ckanext/gbif/theme/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:18:13.511346 ckanext-gbif-2.1.8/ckanext/gbif/theme/assets/less/
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-17 08:17:58.000000 ckanext-gbif-2.1.8/ckanext/gbif/theme/assets/less/gbif.less
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:18:13.511346 ckanext-gbif-2.1.8/ckanext/gbif/theme/assets/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-17 08:17:58.000000 ckanext-gbif-2.1.8/ckanext/gbif/theme/assets/scripts/gbif-dqi.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)      250 2023-07-17 08:17:58.000000 ckanext-gbif-2.1.8/ckanext/gbif/theme/assets/webassets.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:18:13.499346 ckanext-gbif-2.1.8/ckanext/gbif/theme/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:18:13.511346 ckanext-gbif-2.1.8/ckanext/gbif/theme/templates/record/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      310 2023-07-17 08:17:58.000000 ckanext-gbif-2.1.8/ckanext/gbif/theme/templates/record/dwc.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7148 2023-07-17 08:17:58.000000 ckanext-gbif-2.1.8/ckanext/gbif/theme/templates/record/gbif.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:18:13.511346 ckanext-gbif-2.1.8/ckanext/gbif/theme/templates/record/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-17 08:17:58.000000 ckanext-gbif-2.1.8/ckanext/gbif/theme/templates/record/snippets/external_links.html
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-17 08:17:58.000000 ckanext-gbif-2.1.8/ckanext/gbif/theme/templates/record/snippets/gbif-errors.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)      595 2023-07-17 08:17:58.000000 ckanext-gbif-2.1.8/ckanext/gbif/theme/templates/record/specimen.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:18:13.515346 ckanext-gbif-2.1.8/ckanext_gbif.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-07-17 08:18:13.000000 ckanext-gbif-2.1.8/ckanext_gbif.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-17 08:18:13.000000 ckanext-gbif-2.1.8/ckanext_gbif.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 08:18:13.000000 ckanext-gbif-2.1.8/ckanext_gbif.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-17 08:18:13.000000 ckanext-gbif-2.1.8/ckanext_gbif.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 08:18:13.000000 ckanext-gbif-2.1.8/ckanext_gbif.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-17 08:18:13.000000 ckanext-gbif-2.1.8/ckanext_gbif.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-17 08:18:13.000000 ckanext-gbif-2.1.8/ckanext_gbif.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:18:13.503346 ckanext-gbif-2.1.8/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:18:13.515346 ckanext-gbif-2.1.8/docs/_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-17 08:17:58.000000 ckanext-gbif-2.1.8/docs/_scripts/gen_api_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-17 08:17:58.000000 ckanext-gbif-2.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 08:18:13.515346 ckanext-gbif-2.1.8/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      202 2023-07-17 08:17:58.000000 ckanext-gbif-2.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:18:13.515346 ckanext-gbif-2.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-17 08:17:58.000000 ckanext-gbif-2.1.8/tests/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-17 08:17:58.000000 ckanext-gbif-2.1.8/tests/test_helpers.py
```

### Comparing `ckanext-gbif-2.1.7/LICENSE` & `ckanext-gbif-2.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-gbif-2.1.7/PKG-INFO` & `ckanext-gbif-2.1.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-gbif
-Version: 2.1.7
+Version: 2.1.8
 Summary: A CKAN extension that that connects with the GBIF API.
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-gbif
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-gbif/blob/main/CHANGELOG.md
 Keywords: CKAN,data,gbif
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 <!--header-start-->
-<img src="https://github.com/NaturalHistoryMuseum/ckanext-gbif/raw/main/.github/nhm-logo.svg" align="left" width="150px" height="100px" hspace="40"/>
+<img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-gbif
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-gbif/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-gbif/actions/workflows/main.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/NaturalHistoryMuseum/ckanext-gbif/main?style=flat-square)](https://coveralls.io/github/NaturalHistoryMuseum/ckanext-gbif)
 [![CKAN](https://img.shields.io/badge/ckan-2.9.7-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
 [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg?style=flat-square)](https://www.python.org/)
```

### Comparing `ckanext-gbif-2.1.7/README.md` & `ckanext-gbif-2.1.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <!--header-start-->
-<img src="https://github.com/NaturalHistoryMuseum/ckanext-gbif/raw/main/.github/nhm-logo.svg" align="left" width="150px" height="100px" hspace="40"/>
+<img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-gbif
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-gbif/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-gbif/actions/workflows/main.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/NaturalHistoryMuseum/ckanext-gbif/main?style=flat-square)](https://coveralls.io/github/NaturalHistoryMuseum/ckanext-gbif)
 [![CKAN](https://img.shields.io/badge/ckan-2.9.7-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
 [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg?style=flat-square)](https://www.python.org/)
```

### Comparing `ckanext-gbif-2.1.7/ckanext/gbif/lib/errors.py` & `ckanext-gbif-2.1.8/ckanext/gbif/lib/errors.py`

 * *Files identical despite different names*

### Comparing `ckanext-gbif-2.1.7/ckanext/gbif/lib/helpers.py` & `ckanext-gbif-2.1.8/ckanext/gbif/lib/helpers.py`

 * *Files identical despite different names*

### Comparing `ckanext-gbif-2.1.7/ckanext/gbif/logic/action.py` & `ckanext-gbif-2.1.8/ckanext/gbif/logic/action.py`

 * *Files identical despite different names*

### Comparing `ckanext-gbif-2.1.7/ckanext/gbif/plugin.py` & `ckanext-gbif-2.1.8/ckanext/gbif/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-gbif-2.1.7/ckanext/gbif/routes/gbif.py` & `ckanext-gbif-2.1.8/ckanext/gbif/routes/gbif.py`

 * *Files identical despite different names*

### Comparing `ckanext-gbif-2.1.7/ckanext/gbif/theme/assets/less/gbif.less` & `ckanext-gbif-2.1.8/ckanext/gbif/theme/assets/less/gbif.less`

 * *Files identical despite different names*

### Comparing `ckanext-gbif-2.1.7/ckanext/gbif/theme/assets/scripts/gbif-dqi.js` & `ckanext-gbif-2.1.8/ckanext/gbif/theme/assets/scripts/gbif-dqi.js`

 * *Files identical despite different names*

### Comparing `ckanext-gbif-2.1.7/ckanext/gbif/theme/templates/record/gbif.html` & `ckanext-gbif-2.1.8/ckanext/gbif/theme/templates/record/gbif.html`

 * *Files identical despite different names*

### Comparing `ckanext-gbif-2.1.7/ckanext/gbif/theme/templates/record/snippets/external_links.html` & `ckanext-gbif-2.1.8/ckanext/gbif/theme/templates/record/snippets/external_links.html`

 * *Files identical despite different names*

### Comparing `ckanext-gbif-2.1.7/ckanext/gbif/theme/templates/record/snippets/gbif-errors.html` & `ckanext-gbif-2.1.8/ckanext/gbif/theme/templates/record/snippets/gbif-errors.html`

 * *Files identical despite different names*

### Comparing `ckanext-gbif-2.1.7/ckanext/gbif/theme/templates/record/specimen.html` & `ckanext-gbif-2.1.8/ckanext/gbif/theme/templates/record/specimen.html`

 * *Files identical despite different names*

### Comparing `ckanext-gbif-2.1.7/ckanext_gbif.egg-info/PKG-INFO` & `ckanext-gbif-2.1.8/ckanext_gbif.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-gbif
-Version: 2.1.7
+Version: 2.1.8
 Summary: A CKAN extension that that connects with the GBIF API.
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-gbif
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-gbif/blob/main/CHANGELOG.md
 Keywords: CKAN,data,gbif
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 <!--header-start-->
-<img src="https://github.com/NaturalHistoryMuseum/ckanext-gbif/raw/main/.github/nhm-logo.svg" align="left" width="150px" height="100px" hspace="40"/>
+<img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-gbif
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-gbif/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-gbif/actions/workflows/main.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/NaturalHistoryMuseum/ckanext-gbif/main?style=flat-square)](https://coveralls.io/github/NaturalHistoryMuseum/ckanext-gbif)
 [![CKAN](https://img.shields.io/badge/ckan-2.9.7-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
 [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg?style=flat-square)](https://www.python.org/)
```

### Comparing `ckanext-gbif-2.1.7/ckanext_gbif.egg-info/SOURCES.txt` & `ckanext-gbif-2.1.8/ckanext_gbif.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-gbif-2.1.7/docs/_scripts/gen_api_pages.py` & `ckanext-gbif-2.1.8/docs/_scripts/gen_api_pages.py`

 * *Files identical despite different names*

### Comparing `ckanext-gbif-2.1.7/pyproject.toml` & `ckanext-gbif-2.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ckanext-gbif"
-version = "2.1.7"
+version = "2.1.8"
 description = "A CKAN extension that that connects with the GBIF API."
 readme = "README.md"
 requires-python = ">=3.6"
 license = { text = "GPL-3.0-or-later" }
 authors = [
     { name = "Natural History Museum", email = "data@nhm.ac.uk" }
 ]
@@ -53,15 +53,15 @@
 exclude = ["tests", "docs"]
 
 [tool.setuptools.package-data]
 "ckanext.gbif.theme" = ["*", "**/*"]
 
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

### Comparing `ckanext-gbif-2.1.7/tests/test_actions.py` & `ckanext-gbif-2.1.8/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `ckanext-gbif-2.1.7/tests/test_helpers.py` & `ckanext-gbif-2.1.8/tests/test_helpers.py`

 * *Files identical despite different names*

