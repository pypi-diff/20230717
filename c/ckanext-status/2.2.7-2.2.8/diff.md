# Comparing `tmp/ckanext-status-2.2.7.tar.gz` & `tmp/ckanext-status-2.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-status-2.2.7.tar", last modified: Tue Apr 11 08:35:07 2023, max compression
+gzip compressed data, was "ckanext-status-2.2.8.tar", last modified: Mon Jul 17 08:25:11 2023, max compression
```

## Comparing `ckanext-status-2.2.7.tar` & `ckanext-status-2.2.8.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:35:07.132813 ckanext-status-2.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-11 08:34:50.000000 ckanext-status-2.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-04-11 08:35:07.132813 ckanext-status-2.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-04-11 08:34:50.000000 ckanext-status-2.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:35:07.128813 ckanext-status-2.2.7/ckanext/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-11 08:34:50.000000 ckanext-status-2.2.7/ckanext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:35:07.128813 ckanext-status-2.2.7/ckanext/status/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-11 08:34:50.000000 ckanext-status-2.2.7/ckanext/status/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:35:07.128813 ckanext-status-2.2.7/ckanext/status/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:34:50.000000 ckanext-status-2.2.7/ckanext/status/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-11 08:34:50.000000 ckanext-status-2.2.7/ckanext/status/lib/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-11 08:34:50.000000 ckanext-status-2.2.7/ckanext/status/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:35:07.124813 ckanext-status-2.2.7/ckanext/status/theme/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:35:07.128813 ckanext-status-2.2.7/ckanext/status/theme/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:35:07.128813 ckanext-status-2.2.7/ckanext/status/theme/assets/less/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-11 08:34:50.000000 ckanext-status-2.2.7/ckanext/status/theme/assets/less/status.less
--rwxr-xr-x   0 runner    (1001) docker     (123)      103 2023-04-11 08:34:50.000000 ckanext-status-2.2.7/ckanext/status/theme/assets/webassets.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:35:07.128813 ckanext-status-2.2.7/ckanext/status/theme/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:35:07.128813 ckanext-status-2.2.7/ckanext/status/theme/templates/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-11 08:34:50.000000 ckanext-status-2.2.7/ckanext/status/theme/templates/admin/config.html
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-11 08:34:50.000000 ckanext-status-2.2.7/ckanext/status/theme/templates/page.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:35:07.132813 ckanext-status-2.2.7/ckanext_status.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-04-11 08:35:07.000000 ckanext-status-2.2.7/ckanext_status.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-11 08:35:07.000000 ckanext-status-2.2.7/ckanext_status.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:35:07.000000 ckanext-status-2.2.7/ckanext_status.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-11 08:35:07.000000 ckanext-status-2.2.7/ckanext_status.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:35:06.000000 ckanext-status-2.2.7/ckanext_status.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-11 08:35:07.000000 ckanext-status-2.2.7/ckanext_status.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-11 08:35:07.000000 ckanext-status-2.2.7/ckanext_status.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:35:07.124813 ckanext-status-2.2.7/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:35:07.132813 ckanext-status-2.2.7/docs/_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-11 08:34:50.000000 ckanext-status-2.2.7/docs/_scripts/gen_api_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-11 08:34:50.000000 ckanext-status-2.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 08:35:07.132813 ckanext-status-2.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-11 08:34:50.000000 ckanext-status-2.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:35:07.132813 ckanext-status-2.2.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-11 08:34:50.000000 ckanext-status-2.2.7/tests/test_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:25:11.719305 ckanext-status-2.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-17 08:25:00.000000 ckanext-status-2.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-07-17 08:25:11.719305 ckanext-status-2.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-07-17 08:25:00.000000 ckanext-status-2.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:25:11.715305 ckanext-status-2.2.8/ckanext/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-17 08:25:00.000000 ckanext-status-2.2.8/ckanext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:25:11.715305 ckanext-status-2.2.8/ckanext/status/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-17 08:25:00.000000 ckanext-status-2.2.8/ckanext/status/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:25:11.715305 ckanext-status-2.2.8/ckanext/status/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:25:00.000000 ckanext-status-2.2.8/ckanext/status/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-17 08:25:00.000000 ckanext-status-2.2.8/ckanext/status/lib/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-17 08:25:00.000000 ckanext-status-2.2.8/ckanext/status/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:25:11.715305 ckanext-status-2.2.8/ckanext/status/theme/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:25:11.715305 ckanext-status-2.2.8/ckanext/status/theme/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:25:11.715305 ckanext-status-2.2.8/ckanext/status/theme/assets/less/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-17 08:25:00.000000 ckanext-status-2.2.8/ckanext/status/theme/assets/less/status.less
+-rwxr-xr-x   0 runner    (1001) docker     (123)      103 2023-07-17 08:25:00.000000 ckanext-status-2.2.8/ckanext/status/theme/assets/webassets.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:25:11.715305 ckanext-status-2.2.8/ckanext/status/theme/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:25:11.715305 ckanext-status-2.2.8/ckanext/status/theme/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-17 08:25:00.000000 ckanext-status-2.2.8/ckanext/status/theme/templates/admin/config.html
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-17 08:25:00.000000 ckanext-status-2.2.8/ckanext/status/theme/templates/page.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:25:11.719305 ckanext-status-2.2.8/ckanext_status.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-07-17 08:25:11.000000 ckanext-status-2.2.8/ckanext_status.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-17 08:25:11.000000 ckanext-status-2.2.8/ckanext_status.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 08:25:11.000000 ckanext-status-2.2.8/ckanext_status.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-17 08:25:11.000000 ckanext-status-2.2.8/ckanext_status.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 08:25:11.000000 ckanext-status-2.2.8/ckanext_status.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-17 08:25:11.000000 ckanext-status-2.2.8/ckanext_status.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-17 08:25:11.000000 ckanext-status-2.2.8/ckanext_status.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:25:11.715305 ckanext-status-2.2.8/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:25:11.719305 ckanext-status-2.2.8/docs/_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-17 08:25:00.000000 ckanext-status-2.2.8/docs/_scripts/gen_api_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-17 08:25:00.000000 ckanext-status-2.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 08:25:11.719305 ckanext-status-2.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-17 08:25:00.000000 ckanext-status-2.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:25:11.719305 ckanext-status-2.2.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-17 08:25:00.000000 ckanext-status-2.2.8/tests/test_status.py
```

### Comparing `ckanext-status-2.2.7/LICENSE` & `ckanext-status-2.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-status-2.2.7/PKG-INFO` & `ckanext-status-2.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-status
-Version: 2.2.7
+Version: 2.2.8
 Summary: A CKAN extension that adds a 'status' bar to the top of the page.
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-status
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-status/blob/main/CHANGELOG.md
 Keywords: CKAN,data,status
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 <!--header-start-->
-<img src="https://github.com/NaturalHistoryMuseum/ckanext-status/raw/main/.github/nhm-logo.svg" align="left" width="150px" height="100px" hspace="40"/>
+<img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-status
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-status/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-status/actions/workflows/main.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/NaturalHistoryMuseum/ckanext-status/main?style=flat-square)](https://coveralls.io/github/NaturalHistoryMuseum/ckanext-status)
 [![CKAN](https://img.shields.io/badge/ckan-2.9.7-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
 [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg?style=flat-square)](https://www.python.org/)
```

### Comparing `ckanext-status-2.2.7/README.md` & `ckanext-status-2.2.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <!--header-start-->
-<img src="https://github.com/NaturalHistoryMuseum/ckanext-status/raw/main/.github/nhm-logo.svg" align="left" width="150px" height="100px" hspace="40"/>
+<img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-status
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-status/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-status/actions/workflows/main.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/NaturalHistoryMuseum/ckanext-status/main?style=flat-square)](https://coveralls.io/github/NaturalHistoryMuseum/ckanext-status)
 [![CKAN](https://img.shields.io/badge/ckan-2.9.7-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
 [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg?style=flat-square)](https://www.python.org/)
```

### Comparing `ckanext-status-2.2.7/ckanext/status/plugin.py` & `ckanext-status-2.2.8/ckanext/status/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-status-2.2.7/ckanext_status.egg-info/PKG-INFO` & `ckanext-status-2.2.8/ckanext_status.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-status
-Version: 2.2.7
+Version: 2.2.8
 Summary: A CKAN extension that adds a 'status' bar to the top of the page.
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-status
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-status/blob/main/CHANGELOG.md
 Keywords: CKAN,data,status
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 <!--header-start-->
-<img src="https://github.com/NaturalHistoryMuseum/ckanext-status/raw/main/.github/nhm-logo.svg" align="left" width="150px" height="100px" hspace="40"/>
+<img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-status
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-status/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-status/actions/workflows/main.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/NaturalHistoryMuseum/ckanext-status/main?style=flat-square)](https://coveralls.io/github/NaturalHistoryMuseum/ckanext-status)
 [![CKAN](https://img.shields.io/badge/ckan-2.9.7-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
 [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg?style=flat-square)](https://www.python.org/)
```

### Comparing `ckanext-status-2.2.7/ckanext_status.egg-info/SOURCES.txt` & `ckanext-status-2.2.8/ckanext_status.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-status-2.2.7/docs/_scripts/gen_api_pages.py` & `ckanext-status-2.2.8/docs/_scripts/gen_api_pages.py`

 * *Files identical despite different names*

### Comparing `ckanext-status-2.2.7/pyproject.toml` & `ckanext-status-2.2.8/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ckanext-status"
-version = "2.2.7"
+version = "2.2.8"
 description = "A CKAN extension that adds a 'status' bar to the top of the page."
 readme = "README.md"
 requires-python = ">=3.6"
 license = { text = "GPL-3.0-or-later" }
 authors = [
     { name = "Natural History Museum", email = "data@nhm.ac.uk" }
 ]
@@ -51,15 +51,15 @@
 exclude = ["tests", "docs"]
 
 [tool.setuptools.package-data]
 "ckanext.status.theme" = ["*", "**/*"]
 
 [tool.commitizen]
 name = "cz_nhm"
-version = "2.2.7"
+version = "2.2.8"
 tag_format = "v$version"
 update_changelog_on_bump = true
 changelog_incremental = true
 version_files = [
     "pyproject.toml:version"
 ]
```

### Comparing `ckanext-status-2.2.7/tests/test_status.py` & `ckanext-status-2.2.8/tests/test_status.py`

 * *Files identical despite different names*

