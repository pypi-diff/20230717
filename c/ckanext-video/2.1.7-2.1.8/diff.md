# Comparing `tmp/ckanext-video-2.1.7.tar.gz` & `tmp/ckanext-video-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-video-2.1.7.tar", last modified: Tue Apr 11 08:44:22 2023, max compression
+gzip compressed data, was "ckanext-video-2.1.8.tar", last modified: Mon Jul 17 08:30:10 2023, max compression
```

## Comparing `ckanext-video-2.1.7.tar` & `ckanext-video-2.1.8.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:44:22.402120 ckanext-video-2.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-11 08:44:11.000000 ckanext-video-2.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-04-11 08:44:22.402120 ckanext-video-2.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-04-11 08:44:11.000000 ckanext-video-2.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:44:22.398120 ckanext-video-2.1.7/ckanext/
--rwxr-xr-x   0 runner    (1001) docker     (123)      306 2023-04-11 08:44:11.000000 ckanext-video-2.1.7/ckanext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:44:22.398120 ckanext-video-2.1.7/ckanext/video/
--rwxr-xr-x   0 runner    (1001) docker     (123)      306 2023-04-11 08:44:11.000000 ckanext-video-2.1.7/ckanext/video/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:44:22.402120 ckanext-video-2.1.7/ckanext/video/logic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:44:11.000000 ckanext-video-2.1.7/ckanext/video/logic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-11 08:44:11.000000 ckanext-video-2.1.7/ckanext/video/logic/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-04-11 08:44:11.000000 ckanext-video-2.1.7/ckanext/video/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-11 08:44:11.000000 ckanext-video-2.1.7/ckanext/video/providers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:44:22.398120 ckanext-video-2.1.7/ckanext/video/theme/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:44:22.402120 ckanext-video-2.1.7/ckanext/video/theme/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-11 08:44:11.000000 ckanext-video-2.1.7/ckanext/video/theme/templates/video_form.html
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-11 08:44:11.000000 ckanext-video-2.1.7/ckanext/video/theme/templates/video_view.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:44:22.402120 ckanext-video-2.1.7/ckanext_video.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-04-11 08:44:22.000000 ckanext-video-2.1.7/ckanext_video.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-11 08:44:22.000000 ckanext-video-2.1.7/ckanext_video.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:44:22.000000 ckanext-video-2.1.7/ckanext_video.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-11 08:44:22.000000 ckanext-video-2.1.7/ckanext_video.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:44:22.000000 ckanext-video-2.1.7/ckanext_video.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-11 08:44:22.000000 ckanext-video-2.1.7/ckanext_video.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-11 08:44:22.000000 ckanext-video-2.1.7/ckanext_video.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:44:22.398120 ckanext-video-2.1.7/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:44:22.402120 ckanext-video-2.1.7/docs/_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-11 08:44:11.000000 ckanext-video-2.1.7/docs/_scripts/gen_api_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-11 08:44:11.000000 ckanext-video-2.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 08:44:22.402120 ckanext-video-2.1.7/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-04-11 08:44:11.000000 ckanext-video-2.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:44:22.402120 ckanext-video-2.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-11 08:44:11.000000 ckanext-video-2.1.7/tests/test_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-11 08:44:11.000000 ckanext-video-2.1.7/tests/test_view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:30:10.478835 ckanext-video-2.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-17 08:29:59.000000 ckanext-video-2.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-07-17 08:30:10.474835 ckanext-video-2.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-07-17 08:29:59.000000 ckanext-video-2.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:30:10.474835 ckanext-video-2.1.8/ckanext/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      306 2023-07-17 08:29:59.000000 ckanext-video-2.1.8/ckanext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:30:10.474835 ckanext-video-2.1.8/ckanext/video/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      306 2023-07-17 08:29:59.000000 ckanext-video-2.1.8/ckanext/video/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:30:10.474835 ckanext-video-2.1.8/ckanext/video/logic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:29:59.000000 ckanext-video-2.1.8/ckanext/video/logic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 08:29:59.000000 ckanext-video-2.1.8/ckanext/video/logic/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-17 08:29:59.000000 ckanext-video-2.1.8/ckanext/video/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-17 08:29:59.000000 ckanext-video-2.1.8/ckanext/video/providers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:30:10.474835 ckanext-video-2.1.8/ckanext/video/theme/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:30:10.474835 ckanext-video-2.1.8/ckanext/video/theme/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-17 08:29:59.000000 ckanext-video-2.1.8/ckanext/video/theme/templates/video_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-17 08:29:59.000000 ckanext-video-2.1.8/ckanext/video/theme/templates/video_view.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:30:10.474835 ckanext-video-2.1.8/ckanext_video.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-07-17 08:30:10.000000 ckanext-video-2.1.8/ckanext_video.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-17 08:30:10.000000 ckanext-video-2.1.8/ckanext_video.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 08:30:10.000000 ckanext-video-2.1.8/ckanext_video.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-17 08:30:10.000000 ckanext-video-2.1.8/ckanext_video.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 08:30:10.000000 ckanext-video-2.1.8/ckanext_video.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-17 08:30:10.000000 ckanext-video-2.1.8/ckanext_video.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-17 08:30:10.000000 ckanext-video-2.1.8/ckanext_video.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:30:10.474835 ckanext-video-2.1.8/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:30:10.474835 ckanext-video-2.1.8/docs/_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-17 08:29:59.000000 ckanext-video-2.1.8/docs/_scripts/gen_api_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-17 08:29:59.000000 ckanext-video-2.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 08:30:10.478835 ckanext-video-2.1.8/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-07-17 08:29:59.000000 ckanext-video-2.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:30:10.474835 ckanext-video-2.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-17 08:29:59.000000 ckanext-video-2.1.8/tests/test_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-17 08:29:59.000000 ckanext-video-2.1.8/tests/test_view.py
```

### Comparing `ckanext-video-2.1.7/LICENSE` & `ckanext-video-2.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-video-2.1.7/PKG-INFO` & `ckanext-video-2.1.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-video
-Version: 2.1.7
+Version: 2.1.8
 Summary: A CKAN extension for embedding Youtube or Vimeo videos as views.
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-video
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-video/blob/main/CHANGELOG.md
 Keywords: CKAN,data,video
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 <!--header-start-->
-<img src="https://github.com/NaturalHistoryMuseum/ckanext-video/raw/main/.github/nhm-logo.svg" align="left" width="150px" height="100px" hspace="40"/>
+<img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-video
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-video/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-video/actions/workflows/main.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/NaturalHistoryMuseum/ckanext-video/main?style=flat-square)](https://coveralls.io/github/NaturalHistoryMuseum/ckanext-video)
 [![CKAN](https://img.shields.io/badge/ckan-2.9.7-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
 [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg?style=flat-square)](https://www.python.org/)
```

### Comparing `ckanext-video-2.1.7/README.md` & `ckanext-video-2.1.8/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <!--header-start-->
-<img src="https://github.com/NaturalHistoryMuseum/ckanext-video/raw/main/.github/nhm-logo.svg" align="left" width="150px" height="100px" hspace="40"/>
+<img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-video
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-video/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-video/actions/workflows/main.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/NaturalHistoryMuseum/ckanext-video/main?style=flat-square)](https://coveralls.io/github/NaturalHistoryMuseum/ckanext-video)
 [![CKAN](https://img.shields.io/badge/ckan-2.9.7-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
 [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg?style=flat-square)](https://www.python.org/)
```

### Comparing `ckanext-video-2.1.7/ckanext/video/logic/validators.py` & `ckanext-video-2.1.8/ckanext/video/logic/validators.py`

 * *Files identical despite different names*

### Comparing `ckanext-video-2.1.7/ckanext/video/plugin.py` & `ckanext-video-2.1.8/ckanext/video/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-video-2.1.7/ckanext/video/theme/templates/video_form.html` & `ckanext-video-2.1.8/ckanext/video/theme/templates/video_form.html`

 * *Files identical despite different names*

### Comparing `ckanext-video-2.1.7/ckanext_video.egg-info/PKG-INFO` & `ckanext-video-2.1.8/ckanext_video.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-video
-Version: 2.1.7
+Version: 2.1.8
 Summary: A CKAN extension for embedding Youtube or Vimeo videos as views.
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-video
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-video/blob/main/CHANGELOG.md
 Keywords: CKAN,data,video
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 <!--header-start-->
-<img src="https://github.com/NaturalHistoryMuseum/ckanext-video/raw/main/.github/nhm-logo.svg" align="left" width="150px" height="100px" hspace="40"/>
+<img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-video
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-video/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-video/actions/workflows/main.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/NaturalHistoryMuseum/ckanext-video/main?style=flat-square)](https://coveralls.io/github/NaturalHistoryMuseum/ckanext-video)
 [![CKAN](https://img.shields.io/badge/ckan-2.9.7-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
 [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg?style=flat-square)](https://www.python.org/)
```

### Comparing `ckanext-video-2.1.7/ckanext_video.egg-info/SOURCES.txt` & `ckanext-video-2.1.8/ckanext_video.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-video-2.1.7/docs/_scripts/gen_api_pages.py` & `ckanext-video-2.1.8/docs/_scripts/gen_api_pages.py`

 * *Files identical despite different names*

### Comparing `ckanext-video-2.1.7/pyproject.toml` & `ckanext-video-2.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ckanext-video"
-version = "2.1.7"
+version = "2.1.8"
 description = "A CKAN extension for embedding Youtube or Vimeo videos as views."
 readme = "README.md"
 requires-python = ">=3.6"
 license = { text = "GPL-3.0-or-later" }
 authors = [
     { name = "Natural History Museum", email = "data@nhm.ac.uk" }
 ]
@@ -51,15 +51,15 @@
 exclude = ["tests", "docs"]
 
 [tool.setuptools.package-data]
 "ckanext.video.theme" = ["*", "**/*"]
 
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

### Comparing `ckanext-video-2.1.7/tests/test_validators.py` & `ckanext-video-2.1.8/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `ckanext-video-2.1.7/tests/test_view.py` & `ckanext-video-2.1.8/tests/test_view.py`

 * *Files identical despite different names*

