# Comparing `tmp/ckanext-webview-1.1.7.tar.gz` & `tmp/ckanext-webview-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-webview-1.1.7.tar", last modified: Tue Apr 11 08:47:00 2023, max compression
+gzip compressed data, was "ckanext-webview-1.1.8.tar", last modified: Mon Jul 17 08:31:35 2023, max compression
```

## Comparing `ckanext-webview-1.1.7.tar` & `ckanext-webview-1.1.8.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:47:00.420163 ckanext-webview-1.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-11 08:46:44.000000 ckanext-webview-1.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-04-11 08:47:00.420163 ckanext-webview-1.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-04-11 08:46:44.000000 ckanext-webview-1.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:47:00.416164 ckanext-webview-1.1.7/ckanext/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-11 08:46:44.000000 ckanext-webview-1.1.7/ckanext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:47:00.416164 ckanext-webview-1.1.7/ckanext/webview/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-11 08:46:44.000000 ckanext-webview-1.1.7/ckanext/webview/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:47:00.420163 ckanext-webview-1.1.7/ckanext/webview/logic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:46:44.000000 ckanext-webview-1.1.7/ckanext/webview/logic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-11 08:46:44.000000 ckanext-webview-1.1.7/ckanext/webview/logic/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-04-11 08:46:44.000000 ckanext-webview-1.1.7/ckanext/webview/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:47:00.416164 ckanext-webview-1.1.7/ckanext/webview/theme/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:47:00.420163 ckanext-webview-1.1.7/ckanext/webview/theme/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:47:00.420163 ckanext-webview-1.1.7/ckanext/webview/theme/assets/less/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-11 08:46:44.000000 ckanext-webview-1.1.7/ckanext/webview/theme/assets/less/webview.less
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-11 08:46:44.000000 ckanext-webview-1.1.7/ckanext/webview/theme/assets/webassets.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:47:00.416164 ckanext-webview-1.1.7/ckanext/webview/theme/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:47:00.420163 ckanext-webview-1.1.7/ckanext/webview/theme/templates/views/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-11 08:46:44.000000 ckanext-webview-1.1.7/ckanext/webview/theme/templates/views/web_view.html
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-11 08:46:44.000000 ckanext-webview-1.1.7/ckanext/webview/theme/templates/views/web_view_form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:47:00.420163 ckanext-webview-1.1.7/ckanext_webview.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-04-11 08:47:00.000000 ckanext-webview-1.1.7/ckanext_webview.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-11 08:47:00.000000 ckanext-webview-1.1.7/ckanext_webview.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:47:00.000000 ckanext-webview-1.1.7/ckanext_webview.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-11 08:47:00.000000 ckanext-webview-1.1.7/ckanext_webview.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:47:00.000000 ckanext-webview-1.1.7/ckanext_webview.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-11 08:47:00.000000 ckanext-webview-1.1.7/ckanext_webview.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-11 08:47:00.000000 ckanext-webview-1.1.7/ckanext_webview.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:47:00.416164 ckanext-webview-1.1.7/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:47:00.420163 ckanext-webview-1.1.7/docs/_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-11 08:46:44.000000 ckanext-webview-1.1.7/docs/_scripts/gen_api_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-11 08:46:44.000000 ckanext-webview-1.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 08:47:00.420163 ckanext-webview-1.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-11 08:46:44.000000 ckanext-webview-1.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:47:00.420163 ckanext-webview-1.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-04-11 08:46:44.000000 ckanext-webview-1.1.7/tests/test_validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:31:35.549337 ckanext-webview-1.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-17 08:31:20.000000 ckanext-webview-1.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-07-17 08:31:35.549337 ckanext-webview-1.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-07-17 08:31:20.000000 ckanext-webview-1.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:31:35.549337 ckanext-webview-1.1.8/ckanext/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-17 08:31:20.000000 ckanext-webview-1.1.8/ckanext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:31:35.549337 ckanext-webview-1.1.8/ckanext/webview/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-17 08:31:20.000000 ckanext-webview-1.1.8/ckanext/webview/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:31:35.549337 ckanext-webview-1.1.8/ckanext/webview/logic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:31:20.000000 ckanext-webview-1.1.8/ckanext/webview/logic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-17 08:31:20.000000 ckanext-webview-1.1.8/ckanext/webview/logic/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-17 08:31:20.000000 ckanext-webview-1.1.8/ckanext/webview/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:31:35.549337 ckanext-webview-1.1.8/ckanext/webview/theme/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:31:35.549337 ckanext-webview-1.1.8/ckanext/webview/theme/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:31:35.549337 ckanext-webview-1.1.8/ckanext/webview/theme/assets/less/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-17 08:31:20.000000 ckanext-webview-1.1.8/ckanext/webview/theme/assets/less/webview.less
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-17 08:31:20.000000 ckanext-webview-1.1.8/ckanext/webview/theme/assets/webassets.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:31:35.549337 ckanext-webview-1.1.8/ckanext/webview/theme/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:31:35.549337 ckanext-webview-1.1.8/ckanext/webview/theme/templates/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-17 08:31:20.000000 ckanext-webview-1.1.8/ckanext/webview/theme/templates/views/web_view.html
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-17 08:31:20.000000 ckanext-webview-1.1.8/ckanext/webview/theme/templates/views/web_view_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:31:35.549337 ckanext-webview-1.1.8/ckanext_webview.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-07-17 08:31:35.000000 ckanext-webview-1.1.8/ckanext_webview.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-17 08:31:35.000000 ckanext-webview-1.1.8/ckanext_webview.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 08:31:35.000000 ckanext-webview-1.1.8/ckanext_webview.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-17 08:31:35.000000 ckanext-webview-1.1.8/ckanext_webview.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 08:31:35.000000 ckanext-webview-1.1.8/ckanext_webview.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-17 08:31:35.000000 ckanext-webview-1.1.8/ckanext_webview.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-17 08:31:35.000000 ckanext-webview-1.1.8/ckanext_webview.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:31:35.549337 ckanext-webview-1.1.8/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:31:35.549337 ckanext-webview-1.1.8/docs/_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-17 08:31:20.000000 ckanext-webview-1.1.8/docs/_scripts/gen_api_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-17 08:31:20.000000 ckanext-webview-1.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 08:31:35.549337 ckanext-webview-1.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-17 08:31:20.000000 ckanext-webview-1.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:31:35.549337 ckanext-webview-1.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-17 08:31:20.000000 ckanext-webview-1.1.8/tests/test_validators.py
```

### Comparing `ckanext-webview-1.1.7/LICENSE` & `ckanext-webview-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-webview-1.1.7/PKG-INFO` & `ckanext-webview-1.1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-webview
-Version: 1.1.7
+Version: 1.1.8
 Summary: A CKAN extension that adds a view for displaying generic/arbitrary URLs.
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-webview
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-webview/blob/main/CHANGELOG.md
 Keywords: CKAN,data,webview
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 <!--header-start-->
-<img src="https://github.com/NaturalHistoryMuseum/ckanext-webview/raw/main/.github/nhm-logo.svg" align="left" width="150px" height="100px" hspace="40"/>
+<img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-webview
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-webview/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-webview/actions/workflows/main.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/NaturalHistoryMuseum/ckanext-webview/main?style=flat-square)](https://coveralls.io/github/NaturalHistoryMuseum/ckanext-webview)
 [![CKAN](https://img.shields.io/badge/ckan-2.9.7-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
 [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg?style=flat-square)](https://www.python.org/)
```

### Comparing `ckanext-webview-1.1.7/README.md` & `ckanext-webview-1.1.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <!--header-start-->
-<img src="https://github.com/NaturalHistoryMuseum/ckanext-webview/raw/main/.github/nhm-logo.svg" align="left" width="150px" height="100px" hspace="40"/>
+<img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-webview
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-webview/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-webview/actions/workflows/main.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/NaturalHistoryMuseum/ckanext-webview/main?style=flat-square)](https://coveralls.io/github/NaturalHistoryMuseum/ckanext-webview)
 [![CKAN](https://img.shields.io/badge/ckan-2.9.7-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
 [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg?style=flat-square)](https://www.python.org/)
```

### Comparing `ckanext-webview-1.1.7/ckanext/webview/logic/validators.py` & `ckanext-webview-1.1.8/ckanext/webview/logic/validators.py`

 * *Files identical despite different names*

### Comparing `ckanext-webview-1.1.7/ckanext/webview/plugin.py` & `ckanext-webview-1.1.8/ckanext/webview/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-webview-1.1.7/ckanext_webview.egg-info/PKG-INFO` & `ckanext-webview-1.1.8/ckanext_webview.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-webview
-Version: 1.1.7
+Version: 1.1.8
 Summary: A CKAN extension that adds a view for displaying generic/arbitrary URLs.
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-webview
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-webview/blob/main/CHANGELOG.md
 Keywords: CKAN,data,webview
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 <!--header-start-->
-<img src="https://github.com/NaturalHistoryMuseum/ckanext-webview/raw/main/.github/nhm-logo.svg" align="left" width="150px" height="100px" hspace="40"/>
+<img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-webview
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-webview/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-webview/actions/workflows/main.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/NaturalHistoryMuseum/ckanext-webview/main?style=flat-square)](https://coveralls.io/github/NaturalHistoryMuseum/ckanext-webview)
 [![CKAN](https://img.shields.io/badge/ckan-2.9.7-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
 [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg?style=flat-square)](https://www.python.org/)
```

### Comparing `ckanext-webview-1.1.7/ckanext_webview.egg-info/SOURCES.txt` & `ckanext-webview-1.1.8/ckanext_webview.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-webview-1.1.7/docs/_scripts/gen_api_pages.py` & `ckanext-webview-1.1.8/docs/_scripts/gen_api_pages.py`

 * *Files identical despite different names*

### Comparing `ckanext-webview-1.1.7/pyproject.toml` & `ckanext-webview-1.1.8/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ckanext-webview"
-version = "1.1.7"
+version = "1.1.8"
 description = "A CKAN extension that adds a view for displaying generic/arbitrary URLs."
 readme = "README.md"
 requires-python = ">=3.6"
 license = { text = "GPL-3.0-or-later" }
 authors = [
     { name = "Natural History Museum", email = "data@nhm.ac.uk" }
 ]
@@ -51,15 +51,15 @@
 exclude = ["tests", "docs"]
 
 [tool.setuptools.package-data]
 "ckanext.webview.theme" = ["*", "**/*"]
 
 [tool.commitizen]
 name = "cz_nhm"
-version = "1.1.7"
+version = "1.1.8"
 tag_format = "v$version"
 update_changelog_on_bump = true
 changelog_incremental = true
 version_files = [
     "pyproject.toml:version"
 ]
```

### Comparing `ckanext-webview-1.1.7/tests/test_validators.py` & `ckanext-webview-1.1.8/tests/test_validators.py`

 * *Files identical despite different names*

