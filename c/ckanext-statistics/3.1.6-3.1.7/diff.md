# Comparing `tmp/ckanext-statistics-3.1.6.tar.gz` & `tmp/ckanext-statistics-3.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-statistics-3.1.6.tar", last modified: Tue Apr 11 08:26:56 2023, max compression
+gzip compressed data, was "ckanext-statistics-3.1.7.tar", last modified: Mon Jul 17 08:24:52 2023, max compression
```

## Comparing `ckanext-statistics-3.1.6.tar` & `ckanext-statistics-3.1.7.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:26:56.554536 ckanext-statistics-3.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-11 08:26:35.000000 ckanext-statistics-3.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-04-11 08:26:56.554536 ckanext-statistics-3.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-04-11 08:26:35.000000 ckanext-statistics-3.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:26:56.550536 ckanext-statistics-3.1.6/ckanext/
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-11 08:26:35.000000 ckanext-statistics-3.1.6/ckanext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:26:56.550536 ckanext-statistics-3.1.6/ckanext/statistics/
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-11 08:26:35.000000 ckanext-statistics-3.1.6/ckanext/statistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-04-11 08:26:35.000000 ckanext-statistics-3.1.6/ckanext/statistics/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:26:56.550536 ckanext-statistics-3.1.6/ckanext/statistics/data/
--rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-04-11 08:26:35.000000 ckanext-statistics-3.1.6/ckanext/statistics/data/data-portal-backfill.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:26:56.550536 ckanext-statistics-3.1.6/ckanext/statistics/lib/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-11 08:26:35.000000 ckanext-statistics-3.1.6/ckanext/statistics/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-04-11 08:26:35.000000 ckanext-statistics-3.1.6/ckanext/statistics/lib/dataset_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    10830 2023-04-11 08:26:35.000000 ckanext-statistics-3.1.6/ckanext/statistics/lib/download_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-04-11 08:26:35.000000 ckanext-statistics-3.1.6/ckanext/statistics/lib/statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:26:56.550536 ckanext-statistics-3.1.6/ckanext/statistics/logic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:26:35.000000 ckanext-statistics-3.1.6/ckanext/statistics/logic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-11 08:26:35.000000 ckanext-statistics-3.1.6/ckanext/statistics/logic/action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-11 08:26:35.000000 ckanext-statistics-3.1.6/ckanext/statistics/logic/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:26:56.554536 ckanext-statistics-3.1.6/ckanext/statistics/model/
--rwxr-xr-x   0 runner    (1001) docker     (123)      139 2023-04-11 08:26:35.000000 ckanext-statistics-3.1.6/ckanext/statistics/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-11 08:26:35.000000 ckanext-statistics-3.1.6/ckanext/statistics/model/gbif_download.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-11 08:26:35.000000 ckanext-statistics-3.1.6/ckanext/statistics/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:26:56.554536 ckanext-statistics-3.1.6/ckanext_statistics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-04-11 08:26:56.000000 ckanext-statistics-3.1.6/ckanext_statistics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-11 08:26:56.000000 ckanext-statistics-3.1.6/ckanext_statistics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:26:56.000000 ckanext-statistics-3.1.6/ckanext_statistics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-11 08:26:56.000000 ckanext-statistics-3.1.6/ckanext_statistics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:26:56.000000 ckanext-statistics-3.1.6/ckanext_statistics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-11 08:26:56.000000 ckanext-statistics-3.1.6/ckanext_statistics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-11 08:26:56.000000 ckanext-statistics-3.1.6/ckanext_statistics.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:26:56.550536 ckanext-statistics-3.1.6/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:26:56.554536 ckanext-statistics-3.1.6/docs/_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-11 08:26:35.000000 ckanext-statistics-3.1.6/docs/_scripts/gen_api_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-04-11 08:26:35.000000 ckanext-statistics-3.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 08:26:56.554536 ckanext-statistics-3.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-11 08:26:35.000000 ckanext-statistics-3.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:26:56.554536 ckanext-statistics-3.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    19974 2023-04-11 08:26:35.000000 ckanext-statistics-3.1.6/tests/test_download_statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:24:52.552147 ckanext-statistics-3.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-17 08:24:38.000000 ckanext-statistics-3.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-07-17 08:24:52.552147 ckanext-statistics-3.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-07-17 08:24:38.000000 ckanext-statistics-3.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:24:52.548147 ckanext-statistics-3.1.7/ckanext/
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-17 08:24:38.000000 ckanext-statistics-3.1.7/ckanext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:24:52.548147 ckanext-statistics-3.1.7/ckanext/statistics/
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-17 08:24:38.000000 ckanext-statistics-3.1.7/ckanext/statistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-07-17 08:24:38.000000 ckanext-statistics-3.1.7/ckanext/statistics/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:24:52.548147 ckanext-statistics-3.1.7/ckanext/statistics/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-07-17 08:24:38.000000 ckanext-statistics-3.1.7/ckanext/statistics/data/data-portal-backfill.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:24:52.548147 ckanext-statistics-3.1.7/ckanext/statistics/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-17 08:24:38.000000 ckanext-statistics-3.1.7/ckanext/statistics/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-07-17 08:24:38.000000 ckanext-statistics-3.1.7/ckanext/statistics/lib/dataset_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10830 2023-07-17 08:24:38.000000 ckanext-statistics-3.1.7/ckanext/statistics/lib/download_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-17 08:24:38.000000 ckanext-statistics-3.1.7/ckanext/statistics/lib/statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:24:52.552147 ckanext-statistics-3.1.7/ckanext/statistics/logic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:24:38.000000 ckanext-statistics-3.1.7/ckanext/statistics/logic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-17 08:24:38.000000 ckanext-statistics-3.1.7/ckanext/statistics/logic/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-17 08:24:38.000000 ckanext-statistics-3.1.7/ckanext/statistics/logic/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:24:52.552147 ckanext-statistics-3.1.7/ckanext/statistics/model/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      139 2023-07-17 08:24:38.000000 ckanext-statistics-3.1.7/ckanext/statistics/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-17 08:24:38.000000 ckanext-statistics-3.1.7/ckanext/statistics/model/gbif_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-17 08:24:38.000000 ckanext-statistics-3.1.7/ckanext/statistics/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:24:52.552147 ckanext-statistics-3.1.7/ckanext_statistics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-07-17 08:24:52.000000 ckanext-statistics-3.1.7/ckanext_statistics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-17 08:24:52.000000 ckanext-statistics-3.1.7/ckanext_statistics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 08:24:52.000000 ckanext-statistics-3.1.7/ckanext_statistics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-17 08:24:52.000000 ckanext-statistics-3.1.7/ckanext_statistics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 08:24:52.000000 ckanext-statistics-3.1.7/ckanext_statistics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-17 08:24:52.000000 ckanext-statistics-3.1.7/ckanext_statistics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-17 08:24:52.000000 ckanext-statistics-3.1.7/ckanext_statistics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:24:52.548147 ckanext-statistics-3.1.7/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:24:52.552147 ckanext-statistics-3.1.7/docs/_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-17 08:24:38.000000 ckanext-statistics-3.1.7/docs/_scripts/gen_api_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-17 08:24:38.000000 ckanext-statistics-3.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 08:24:52.552147 ckanext-statistics-3.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-17 08:24:38.000000 ckanext-statistics-3.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:24:52.552147 ckanext-statistics-3.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    19974 2023-07-17 08:24:38.000000 ckanext-statistics-3.1.7/tests/test_download_statistics.py
```

### Comparing `ckanext-statistics-3.1.6/LICENSE` & `ckanext-statistics-3.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-statistics-3.1.6/PKG-INFO` & `ckanext-statistics-3.1.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-statistics
-Version: 3.1.6
+Version: 3.1.7
 Summary: A CKAN extension for accessing instance statistics.
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-statistics
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-statistics/blob/main/CHANGELOG.md
 Keywords: CKAN,data,statistics
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 <!--header-start-->
-<img src="https://github.com/NaturalHistoryMuseum/ckanext-statistics/raw/main/.github/nhm-logo.svg" align="left" width="150px" height="100px" hspace="40"/>
+<img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-statistics
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-statistics/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-statistics/actions/workflows/main.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/NaturalHistoryMuseum/ckanext-statistics/main?style=flat-square)](https://coveralls.io/github/NaturalHistoryMuseum/ckanext-statistics)
 [![CKAN](https://img.shields.io/badge/ckan-2.9.7-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
 [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg?style=flat-square)](https://www.python.org/)
```

### Comparing `ckanext-statistics-3.1.6/README.md` & `ckanext-statistics-3.1.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <!--header-start-->
-<img src="https://github.com/NaturalHistoryMuseum/ckanext-statistics/raw/main/.github/nhm-logo.svg" align="left" width="150px" height="100px" hspace="40"/>
+<img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-statistics
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-statistics/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-statistics/actions/workflows/main.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/NaturalHistoryMuseum/ckanext-statistics/main?style=flat-square)](https://coveralls.io/github/NaturalHistoryMuseum/ckanext-statistics)
 [![CKAN](https://img.shields.io/badge/ckan-2.9.7-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
 [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg?style=flat-square)](https://www.python.org/)
```

### Comparing `ckanext-statistics-3.1.6/ckanext/statistics/cli.py` & `ckanext-statistics-3.1.7/ckanext/statistics/cli.py`

 * *Files identical despite different names*

### Comparing `ckanext-statistics-3.1.6/ckanext/statistics/data/data-portal-backfill.json` & `ckanext-statistics-3.1.7/ckanext/statistics/data/data-portal-backfill.json`

 * *Files identical despite different names*

### Comparing `ckanext-statistics-3.1.6/ckanext/statistics/lib/dataset_statistics.py` & `ckanext-statistics-3.1.7/ckanext/statistics/lib/dataset_statistics.py`

 * *Files identical despite different names*

### Comparing `ckanext-statistics-3.1.6/ckanext/statistics/lib/download_statistics.py` & `ckanext-statistics-3.1.7/ckanext/statistics/lib/download_statistics.py`

 * *Files identical despite different names*

### Comparing `ckanext-statistics-3.1.6/ckanext/statistics/lib/statistics.py` & `ckanext-statistics-3.1.7/ckanext/statistics/lib/statistics.py`

 * *Files identical despite different names*

### Comparing `ckanext-statistics-3.1.6/ckanext/statistics/logic/action.py` & `ckanext-statistics-3.1.7/ckanext/statistics/logic/action.py`

 * *Files identical despite different names*

### Comparing `ckanext-statistics-3.1.6/ckanext/statistics/logic/schema.py` & `ckanext-statistics-3.1.7/ckanext/statistics/logic/schema.py`

 * *Files identical despite different names*

### Comparing `ckanext-statistics-3.1.6/ckanext/statistics/model/gbif_download.py` & `ckanext-statistics-3.1.7/ckanext/statistics/model/gbif_download.py`

 * *Files identical despite different names*

### Comparing `ckanext-statistics-3.1.6/ckanext/statistics/plugin.py` & `ckanext-statistics-3.1.7/ckanext/statistics/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-statistics-3.1.6/ckanext_statistics.egg-info/PKG-INFO` & `ckanext-statistics-3.1.7/ckanext_statistics.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-statistics
-Version: 3.1.6
+Version: 3.1.7
 Summary: A CKAN extension for accessing instance statistics.
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-statistics
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-statistics/blob/main/CHANGELOG.md
 Keywords: CKAN,data,statistics
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 <!--header-start-->
-<img src="https://github.com/NaturalHistoryMuseum/ckanext-statistics/raw/main/.github/nhm-logo.svg" align="left" width="150px" height="100px" hspace="40"/>
+<img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-statistics
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-statistics/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-statistics/actions/workflows/main.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/NaturalHistoryMuseum/ckanext-statistics/main?style=flat-square)](https://coveralls.io/github/NaturalHistoryMuseum/ckanext-statistics)
 [![CKAN](https://img.shields.io/badge/ckan-2.9.7-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
 [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg?style=flat-square)](https://www.python.org/)
```

### Comparing `ckanext-statistics-3.1.6/ckanext_statistics.egg-info/SOURCES.txt` & `ckanext-statistics-3.1.7/ckanext_statistics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-statistics-3.1.6/docs/_scripts/gen_api_pages.py` & `ckanext-statistics-3.1.7/docs/_scripts/gen_api_pages.py`

 * *Files identical despite different names*

### Comparing `ckanext-statistics-3.1.6/pyproject.toml` & `ckanext-statistics-3.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ckanext-statistics"
-version = "3.1.6"
+version = "3.1.7"
 description = "A CKAN extension for accessing instance statistics."
 readme = "README.md"
 requires-python = ">=3.6"
 license = { text = "GPL-3.0-or-later" }
 authors = [
     { name = "Natural History Museum", email = "data@nhm.ac.uk" }
 ]
@@ -57,15 +57,15 @@
 
 [tool.setuptools.package-data]
 "ckanext.statistics.theme" = ["*", "**/*"]
 "ckanext.statistics.data" = ["*", "**/*"]
 
 [tool.commitizen]
 name = "cz_nhm"
-version = "3.1.6"
+version = "3.1.7"
 tag_format = "v$version"
 update_changelog_on_bump = true
 changelog_incremental = true
 version_files = [
     "pyproject.toml:version"
 ]
```

### Comparing `ckanext-statistics-3.1.6/tests/test_download_statistics.py` & `ckanext-statistics-3.1.7/tests/test_download_statistics.py`

 * *Files identical despite different names*

