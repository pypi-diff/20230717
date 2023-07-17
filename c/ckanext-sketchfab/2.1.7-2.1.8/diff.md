# Comparing `tmp/ckanext-sketchfab-2.1.7.tar.gz` & `tmp/ckanext-sketchfab-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-sketchfab-2.1.7.tar", last modified: Tue Apr 11 08:26:02 2023, max compression
+gzip compressed data, was "ckanext-sketchfab-2.1.8.tar", last modified: Mon Jul 17 08:25:32 2023, max compression
```

## Comparing `ckanext-sketchfab-2.1.7.tar` & `ckanext-sketchfab-2.1.8.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:26:02.684827 ckanext-sketchfab-2.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-11 08:25:44.000000 ckanext-sketchfab-2.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-04-11 08:26:02.684827 ckanext-sketchfab-2.1.7/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     3772 2023-04-11 08:25:44.000000 ckanext-sketchfab-2.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:26:02.676828 ckanext-sketchfab-2.1.7/ckanext/
--rwxr-xr-x   0 runner    (1001) docker     (123)      310 2023-04-11 08:25:44.000000 ckanext-sketchfab-2.1.7/ckanext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:26:02.676828 ckanext-sketchfab-2.1.7/ckanext/sketchfab/
--rwxr-xr-x   0 runner    (1001) docker     (123)      310 2023-04-11 08:25:44.000000 ckanext-sketchfab-2.1.7/ckanext/sketchfab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:26:02.676828 ckanext-sketchfab-2.1.7/ckanext/sketchfab/logic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:25:44.000000 ckanext-sketchfab-2.1.7/ckanext/sketchfab/logic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-11 08:25:44.000000 ckanext-sketchfab-2.1.7/ckanext/sketchfab/logic/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-11 08:25:44.000000 ckanext-sketchfab-2.1.7/ckanext/sketchfab/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:26:02.672827 ckanext-sketchfab-2.1.7/ckanext/sketchfab/theme/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:26:02.676828 ckanext-sketchfab-2.1.7/ckanext/sketchfab/theme/templates/
--rwxr-xr-x   0 runner    (1001) docker     (123)      571 2023-04-11 08:25:44.000000 ckanext-sketchfab-2.1.7/ckanext/sketchfab/theme/templates/sketchfab_form.html
--rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-04-11 08:25:44.000000 ckanext-sketchfab-2.1.7/ckanext/sketchfab/theme/templates/sketchfab_view.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:26:02.680827 ckanext-sketchfab-2.1.7/ckanext_sketchfab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-04-11 08:26:02.000000 ckanext-sketchfab-2.1.7/ckanext_sketchfab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-11 08:26:02.000000 ckanext-sketchfab-2.1.7/ckanext_sketchfab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:26:02.000000 ckanext-sketchfab-2.1.7/ckanext_sketchfab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-11 08:26:02.000000 ckanext-sketchfab-2.1.7/ckanext_sketchfab.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:26:02.000000 ckanext-sketchfab-2.1.7/ckanext_sketchfab.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-11 08:26:02.000000 ckanext-sketchfab-2.1.7/ckanext_sketchfab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-11 08:26:02.000000 ckanext-sketchfab-2.1.7/ckanext_sketchfab.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:26:02.672827 ckanext-sketchfab-2.1.7/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:26:02.680827 ckanext-sketchfab-2.1.7/docs/_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-04-11 08:25:44.000000 ckanext-sketchfab-2.1.7/docs/_scripts/gen_api_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-04-11 08:25:44.000000 ckanext-sketchfab-2.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 08:26:02.684827 ckanext-sketchfab-2.1.7/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      207 2023-04-11 08:25:44.000000 ckanext-sketchfab-2.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:26:02.684827 ckanext-sketchfab-2.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-11 08:25:44.000000 ckanext-sketchfab-2.1.7/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-11 08:25:44.000000 ckanext-sketchfab-2.1.7/tests/test_sketchfab_view.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-11 08:25:44.000000 ckanext-sketchfab-2.1.7/tests/test_validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:25:32.837899 ckanext-sketchfab-2.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-17 08:25:14.000000 ckanext-sketchfab-2.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-07-17 08:25:32.837899 ckanext-sketchfab-2.1.8/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3727 2023-07-17 08:25:14.000000 ckanext-sketchfab-2.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:25:32.833899 ckanext-sketchfab-2.1.8/ckanext/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      310 2023-07-17 08:25:14.000000 ckanext-sketchfab-2.1.8/ckanext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:25:32.833899 ckanext-sketchfab-2.1.8/ckanext/sketchfab/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      310 2023-07-17 08:25:14.000000 ckanext-sketchfab-2.1.8/ckanext/sketchfab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:25:32.837899 ckanext-sketchfab-2.1.8/ckanext/sketchfab/logic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:25:14.000000 ckanext-sketchfab-2.1.8/ckanext/sketchfab/logic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-17 08:25:14.000000 ckanext-sketchfab-2.1.8/ckanext/sketchfab/logic/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-17 08:25:14.000000 ckanext-sketchfab-2.1.8/ckanext/sketchfab/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:25:32.833899 ckanext-sketchfab-2.1.8/ckanext/sketchfab/theme/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:25:32.837899 ckanext-sketchfab-2.1.8/ckanext/sketchfab/theme/templates/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      571 2023-07-17 08:25:14.000000 ckanext-sketchfab-2.1.8/ckanext/sketchfab/theme/templates/sketchfab_form.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-07-17 08:25:14.000000 ckanext-sketchfab-2.1.8/ckanext/sketchfab/theme/templates/sketchfab_view.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:25:32.837899 ckanext-sketchfab-2.1.8/ckanext_sketchfab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-07-17 08:25:32.000000 ckanext-sketchfab-2.1.8/ckanext_sketchfab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-17 08:25:32.000000 ckanext-sketchfab-2.1.8/ckanext_sketchfab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 08:25:32.000000 ckanext-sketchfab-2.1.8/ckanext_sketchfab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-17 08:25:32.000000 ckanext-sketchfab-2.1.8/ckanext_sketchfab.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 08:25:32.000000 ckanext-sketchfab-2.1.8/ckanext_sketchfab.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-17 08:25:32.000000 ckanext-sketchfab-2.1.8/ckanext_sketchfab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-17 08:25:32.000000 ckanext-sketchfab-2.1.8/ckanext_sketchfab.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:25:32.833899 ckanext-sketchfab-2.1.8/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:25:32.837899 ckanext-sketchfab-2.1.8/docs/_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-17 08:25:14.000000 ckanext-sketchfab-2.1.8/docs/_scripts/gen_api_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-17 08:25:14.000000 ckanext-sketchfab-2.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 08:25:32.837899 ckanext-sketchfab-2.1.8/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      207 2023-07-17 08:25:14.000000 ckanext-sketchfab-2.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:25:32.837899 ckanext-sketchfab-2.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-17 08:25:14.000000 ckanext-sketchfab-2.1.8/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-17 08:25:14.000000 ckanext-sketchfab-2.1.8/tests/test_sketchfab_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-17 08:25:14.000000 ckanext-sketchfab-2.1.8/tests/test_validators.py
```

### Comparing `ckanext-sketchfab-2.1.7/LICENSE` & `ckanext-sketchfab-2.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-sketchfab-2.1.7/PKG-INFO` & `ckanext-sketchfab-2.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-sketchfab
-Version: 2.1.7
+Version: 2.1.8
 Summary: A CKAN extension for embedding Sketchfab models as views.
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-sketchfab
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-sketchfab/blob/main/CHANGELOG.md
 Keywords: CKAN,data,sketchfab
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 <!--header-start-->
-<img src="https://github.com/NaturalHistoryMuseum/ckanext-sketchfab/raw/main/.github/nhm-logo.svg" align="left" width="150px" height="100px" hspace="40"/>
+<img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-sketchfab
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-sketchfab/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-sketchfab/actions/workflows/main.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/NaturalHistoryMuseum/ckanext-sketchfab/main?style=flat-square)](https://coveralls.io/github/NaturalHistoryMuseum/ckanext-sketchfab)
 [![CKAN](https://img.shields.io/badge/ckan-2.9.7-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
 [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg?style=flat-square)](https://www.python.org/)
```

### Comparing `ckanext-sketchfab-2.1.7/README.md` & `ckanext-sketchfab-2.1.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <!--header-start-->
-<img src="https://github.com/NaturalHistoryMuseum/ckanext-sketchfab/raw/main/.github/nhm-logo.svg" align="left" width="150px" height="100px" hspace="40"/>
+<img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-sketchfab
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-sketchfab/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-sketchfab/actions/workflows/main.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/NaturalHistoryMuseum/ckanext-sketchfab/main?style=flat-square)](https://coveralls.io/github/NaturalHistoryMuseum/ckanext-sketchfab)
 [![CKAN](https://img.shields.io/badge/ckan-2.9.7-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
 [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg?style=flat-square)](https://www.python.org/)
```

### Comparing `ckanext-sketchfab-2.1.7/ckanext/sketchfab/logic/validators.py` & `ckanext-sketchfab-2.1.8/ckanext/sketchfab/logic/validators.py`

 * *Files identical despite different names*

### Comparing `ckanext-sketchfab-2.1.7/ckanext/sketchfab/plugin.py` & `ckanext-sketchfab-2.1.8/ckanext/sketchfab/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-sketchfab-2.1.7/ckanext/sketchfab/theme/templates/sketchfab_form.html` & `ckanext-sketchfab-2.1.8/ckanext/sketchfab/theme/templates/sketchfab_form.html`

 * *Files identical despite different names*

### Comparing `ckanext-sketchfab-2.1.7/ckanext_sketchfab.egg-info/PKG-INFO` & `ckanext-sketchfab-2.1.8/ckanext_sketchfab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-sketchfab
-Version: 2.1.7
+Version: 2.1.8
 Summary: A CKAN extension for embedding Sketchfab models as views.
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-sketchfab
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-sketchfab/blob/main/CHANGELOG.md
 Keywords: CKAN,data,sketchfab
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 <!--header-start-->
-<img src="https://github.com/NaturalHistoryMuseum/ckanext-sketchfab/raw/main/.github/nhm-logo.svg" align="left" width="150px" height="100px" hspace="40"/>
+<img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-sketchfab
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-sketchfab/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-sketchfab/actions/workflows/main.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/NaturalHistoryMuseum/ckanext-sketchfab/main?style=flat-square)](https://coveralls.io/github/NaturalHistoryMuseum/ckanext-sketchfab)
 [![CKAN](https://img.shields.io/badge/ckan-2.9.7-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
 [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg?style=flat-square)](https://www.python.org/)
```

### Comparing `ckanext-sketchfab-2.1.7/ckanext_sketchfab.egg-info/SOURCES.txt` & `ckanext-sketchfab-2.1.8/ckanext_sketchfab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-sketchfab-2.1.7/docs/_scripts/gen_api_pages.py` & `ckanext-sketchfab-2.1.8/docs/_scripts/gen_api_pages.py`

 * *Files identical despite different names*

### Comparing `ckanext-sketchfab-2.1.7/pyproject.toml` & `ckanext-sketchfab-2.1.8/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ckanext-sketchfab"
-version = "2.1.7"
+version = "2.1.8"
 description = "A CKAN extension for embedding Sketchfab models as views."
 readme = "README.md"
 requires-python = ">=3.6"
 license = { text = "GPL-3.0-or-later" }
 authors = [
     { name = "Natural History Museum", email = "data@nhm.ac.uk" }
 ]
@@ -51,15 +51,15 @@
 exclude = ["tests", "docs"]
 
 [tool.setuptools.package-data]
 "ckanext.sketchfab.theme" = ["*", "**/*"]
 
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

### Comparing `ckanext-sketchfab-2.1.7/tests/test_sketchfab_view.py` & `ckanext-sketchfab-2.1.8/tests/test_sketchfab_view.py`

 * *Files identical despite different names*

### Comparing `ckanext-sketchfab-2.1.7/tests/test_validators.py` & `ckanext-sketchfab-2.1.8/tests/test_validators.py`

 * *Files identical despite different names*

