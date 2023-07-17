# Comparing `tmp/ckanext-iiif-3.0.8.tar.gz` & `tmp/ckanext-iiif-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-iiif-3.0.8.tar", last modified: Tue May  9 09:38:58 2023, max compression
+gzip compressed data, was "ckanext-iiif-3.0.9.tar", last modified: Mon Jul 17 08:20:09 2023, max compression
```

## Comparing `ckanext-iiif-3.0.8.tar` & `ckanext-iiif-3.0.9.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:38:58.125044 ckanext-iiif-3.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-09 09:38:46.000000 ckanext-iiif-3.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8336 2023-05-09 09:38:58.125044 ckanext-iiif-3.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7497 2023-05-09 09:38:46.000000 ckanext-iiif-3.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:38:58.121044 ckanext-iiif-3.0.8/ckanext/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-09 09:38:46.000000 ckanext-iiif-3.0.8/ckanext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:38:58.121044 ckanext-iiif-3.0.8/ckanext/iiif/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-09 09:38:46.000000 ckanext-iiif-3.0.8/ckanext/iiif/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:38:58.121044 ckanext-iiif-3.0.8/ckanext/iiif/builders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 09:38:46.000000 ckanext-iiif-3.0.8/ckanext/iiif/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-09 09:38:46.000000 ckanext-iiif-3.0.8/ckanext/iiif/builders/abc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10137 2023-05-09 09:38:46.000000 ckanext-iiif-3.0.8/ckanext/iiif/builders/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-09 09:38:46.000000 ckanext-iiif-3.0.8/ckanext/iiif/builders/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-09 09:38:46.000000 ckanext-iiif-3.0.8/ckanext/iiif/interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:38:58.121044 ckanext-iiif-3.0.8/ckanext/iiif/logic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 09:38:46.000000 ckanext-iiif-3.0.8/ckanext/iiif/logic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-05-09 09:38:46.000000 ckanext-iiif-3.0.8/ckanext/iiif/logic/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-09 09:38:46.000000 ckanext-iiif-3.0.8/ckanext/iiif/logic/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-05-09 09:38:46.000000 ckanext-iiif-3.0.8/ckanext/iiif/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:38:58.121044 ckanext-iiif-3.0.8/ckanext/iiif/routes/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-09 09:38:46.000000 ckanext-iiif-3.0.8/ckanext/iiif/routes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-09 09:38:46.000000 ckanext-iiif-3.0.8/ckanext/iiif/routes/iiif.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:38:58.121044 ckanext-iiif-3.0.8/ckanext_iiif.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8336 2023-05-09 09:38:58.000000 ckanext-iiif-3.0.8/ckanext_iiif.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-09 09:38:58.000000 ckanext-iiif-3.0.8/ckanext_iiif.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 09:38:58.000000 ckanext-iiif-3.0.8/ckanext_iiif.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-09 09:38:58.000000 ckanext-iiif-3.0.8/ckanext_iiif.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 09:38:57.000000 ckanext-iiif-3.0.8/ckanext_iiif.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-09 09:38:58.000000 ckanext-iiif-3.0.8/ckanext_iiif.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-09 09:38:58.000000 ckanext-iiif-3.0.8/ckanext_iiif.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:38:58.117044 ckanext-iiif-3.0.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:38:58.121044 ckanext-iiif-3.0.8/docs/_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-09 09:38:46.000000 ckanext-iiif-3.0.8/docs/_scripts/gen_api_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-09 09:38:46.000000 ckanext-iiif-3.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 09:38:58.125044 ckanext-iiif-3.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-09 09:38:46.000000 ckanext-iiif-3.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:38:58.117044 ckanext-iiif-3.0.8/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:38:58.125044 ckanext-iiif-3.0.8/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 09:38:46.000000 ckanext-iiif-3.0.8/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-05-09 09:38:46.000000 ckanext-iiif-3.0.8/tests/integration/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-09 09:38:46.000000 ckanext-iiif-3.0.8/tests/integration/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-09 09:38:46.000000 ckanext-iiif-3.0.8/tests/integration/test_iiif_route.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:38:58.125044 ckanext-iiif-3.0.8/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 09:38:46.000000 ckanext-iiif-3.0.8/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:38:58.125044 ckanext-iiif-3.0.8/tests/unit/builders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 09:38:46.000000 ckanext-iiif-3.0.8/tests/unit/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14324 2023-05-09 09:38:46.000000 ckanext-iiif-3.0.8/tests/unit/builders/test_manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-09 09:38:46.000000 ckanext-iiif-3.0.8/tests/unit/builders/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:38:58.125044 ckanext-iiif-3.0.8/tests/unit/logic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 09:38:46.000000 ckanext-iiif-3.0.8/tests/unit/logic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-05-09 09:38:46.000000 ckanext-iiif-3.0.8/tests/unit/logic/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-09 09:38:46.000000 ckanext-iiif-3.0.8/tests/unit/logic/test_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:38:58.125044 ckanext-iiif-3.0.8/tests/unit/routes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 09:38:46.000000 ckanext-iiif-3.0.8/tests/unit/routes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-09 09:38:46.000000 ckanext-iiif-3.0.8/tests/unit/routes/test_iiif.py
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-05-09 09:38:46.000000 ckanext-iiif-3.0.8/tests/unit/test_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:20:09.802005 ckanext-iiif-3.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-17 08:19:59.000000 ckanext-iiif-3.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-07-17 08:20:09.802005 ckanext-iiif-3.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-07-17 08:19:59.000000 ckanext-iiif-3.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:20:09.798005 ckanext-iiif-3.0.9/ckanext/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-17 08:19:59.000000 ckanext-iiif-3.0.9/ckanext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:20:09.798005 ckanext-iiif-3.0.9/ckanext/iiif/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-17 08:19:59.000000 ckanext-iiif-3.0.9/ckanext/iiif/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:20:09.798005 ckanext-iiif-3.0.9/ckanext/iiif/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:19:59.000000 ckanext-iiif-3.0.9/ckanext/iiif/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-17 08:19:59.000000 ckanext-iiif-3.0.9/ckanext/iiif/builders/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10137 2023-07-17 08:19:59.000000 ckanext-iiif-3.0.9/ckanext/iiif/builders/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-17 08:19:59.000000 ckanext-iiif-3.0.9/ckanext/iiif/builders/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-17 08:19:59.000000 ckanext-iiif-3.0.9/ckanext/iiif/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:20:09.798005 ckanext-iiif-3.0.9/ckanext/iiif/logic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:19:59.000000 ckanext-iiif-3.0.9/ckanext/iiif/logic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-07-17 08:19:59.000000 ckanext-iiif-3.0.9/ckanext/iiif/logic/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-17 08:19:59.000000 ckanext-iiif-3.0.9/ckanext/iiif/logic/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-07-17 08:19:59.000000 ckanext-iiif-3.0.9/ckanext/iiif/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:20:09.798005 ckanext-iiif-3.0.9/ckanext/iiif/routes/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-17 08:19:59.000000 ckanext-iiif-3.0.9/ckanext/iiif/routes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-17 08:19:59.000000 ckanext-iiif-3.0.9/ckanext/iiif/routes/iiif.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:20:09.798005 ckanext-iiif-3.0.9/ckanext_iiif.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-07-17 08:20:09.000000 ckanext-iiif-3.0.9/ckanext_iiif.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-17 08:20:09.000000 ckanext-iiif-3.0.9/ckanext_iiif.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 08:20:09.000000 ckanext-iiif-3.0.9/ckanext_iiif.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-17 08:20:09.000000 ckanext-iiif-3.0.9/ckanext_iiif.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 08:20:09.000000 ckanext-iiif-3.0.9/ckanext_iiif.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-17 08:20:09.000000 ckanext-iiif-3.0.9/ckanext_iiif.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-17 08:20:09.000000 ckanext-iiif-3.0.9/ckanext_iiif.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:20:09.794005 ckanext-iiif-3.0.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:20:09.798005 ckanext-iiif-3.0.9/docs/_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-17 08:19:59.000000 ckanext-iiif-3.0.9/docs/_scripts/gen_api_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-07-17 08:19:59.000000 ckanext-iiif-3.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 08:20:09.802005 ckanext-iiif-3.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-17 08:19:59.000000 ckanext-iiif-3.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:20:09.794005 ckanext-iiif-3.0.9/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:20:09.798005 ckanext-iiif-3.0.9/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:19:59.000000 ckanext-iiif-3.0.9/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-17 08:19:59.000000 ckanext-iiif-3.0.9/tests/integration/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-17 08:19:59.000000 ckanext-iiif-3.0.9/tests/integration/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-17 08:19:59.000000 ckanext-iiif-3.0.9/tests/integration/test_iiif_route.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:20:09.798005 ckanext-iiif-3.0.9/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:19:59.000000 ckanext-iiif-3.0.9/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:20:09.798005 ckanext-iiif-3.0.9/tests/unit/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:19:59.000000 ckanext-iiif-3.0.9/tests/unit/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14324 2023-07-17 08:19:59.000000 ckanext-iiif-3.0.9/tests/unit/builders/test_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-17 08:19:59.000000 ckanext-iiif-3.0.9/tests/unit/builders/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:20:09.802005 ckanext-iiif-3.0.9/tests/unit/logic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:19:59.000000 ckanext-iiif-3.0.9/tests/unit/logic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-07-17 08:19:59.000000 ckanext-iiif-3.0.9/tests/unit/logic/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-17 08:19:59.000000 ckanext-iiif-3.0.9/tests/unit/logic/test_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:20:09.802005 ckanext-iiif-3.0.9/tests/unit/routes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:19:59.000000 ckanext-iiif-3.0.9/tests/unit/routes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-17 08:19:59.000000 ckanext-iiif-3.0.9/tests/unit/routes/test_iiif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-07-17 08:19:59.000000 ckanext-iiif-3.0.9/tests/unit/test_plugin.py
```

### Comparing `ckanext-iiif-3.0.8/LICENSE` & `ckanext-iiif-3.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-iiif-3.0.8/PKG-INFO` & `ckanext-iiif-3.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-iiif
-Version: 3.0.8
+Version: 3.0.9
 Summary: IIIF for CKAN
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-iiif
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-iiif/blob/main/CHANGELOG.md
 Keywords: CKAN,data,iiif
 Classifier: Development Status :: 3 - Alpha
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 <!--header-start-->
-<img src="https://github.com/NaturalHistoryMuseum/ckanext-iiif/raw/main/.github/nhm-logo.svg" align="left" width="150px" height="100px" hspace="40"/>
+<img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-iiif
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-iiif/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-iiif/actions/workflows/main.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/NaturalHistoryMuseum/ckanext-iiif/main?style=flat-square)](https://coveralls.io/github/NaturalHistoryMuseum/ckanext-iiif)
 [![CKAN](https://img.shields.io/badge/ckan-2.9.7-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
 [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg?style=flat-square)](https://www.python.org/)
```

### Comparing `ckanext-iiif-3.0.8/README.md` & `ckanext-iiif-3.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <!--header-start-->
-<img src="https://github.com/NaturalHistoryMuseum/ckanext-iiif/raw/main/.github/nhm-logo.svg" align="left" width="150px" height="100px" hspace="40"/>
+<img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-iiif
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-iiif/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-iiif/actions/workflows/main.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/NaturalHistoryMuseum/ckanext-iiif/main?style=flat-square)](https://coveralls.io/github/NaturalHistoryMuseum/ckanext-iiif)
 [![CKAN](https://img.shields.io/badge/ckan-2.9.7-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
 [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg?style=flat-square)](https://www.python.org/)
```

### Comparing `ckanext-iiif-3.0.8/ckanext/iiif/builders/abc.py` & `ckanext-iiif-3.0.9/ckanext/iiif/builders/abc.py`

 * *Files identical despite different names*

### Comparing `ckanext-iiif-3.0.8/ckanext/iiif/builders/manifest.py` & `ckanext-iiif-3.0.9/ckanext/iiif/builders/manifest.py`

 * *Files identical despite different names*

### Comparing `ckanext-iiif-3.0.8/ckanext/iiif/builders/utils.py` & `ckanext-iiif-3.0.9/ckanext/iiif/builders/utils.py`

 * *Files identical despite different names*

### Comparing `ckanext-iiif-3.0.8/ckanext/iiif/logic/actions.py` & `ckanext-iiif-3.0.9/ckanext/iiif/logic/actions.py`

 * *Files identical despite different names*

### Comparing `ckanext-iiif-3.0.8/ckanext/iiif/plugin.py` & `ckanext-iiif-3.0.9/ckanext/iiif/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-iiif-3.0.8/ckanext_iiif.egg-info/PKG-INFO` & `ckanext-iiif-3.0.9/ckanext_iiif.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-iiif
-Version: 3.0.8
+Version: 3.0.9
 Summary: IIIF for CKAN
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-iiif
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-iiif/blob/main/CHANGELOG.md
 Keywords: CKAN,data,iiif
 Classifier: Development Status :: 3 - Alpha
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 <!--header-start-->
-<img src="https://github.com/NaturalHistoryMuseum/ckanext-iiif/raw/main/.github/nhm-logo.svg" align="left" width="150px" height="100px" hspace="40"/>
+<img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-iiif
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-iiif/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-iiif/actions/workflows/main.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/NaturalHistoryMuseum/ckanext-iiif/main?style=flat-square)](https://coveralls.io/github/NaturalHistoryMuseum/ckanext-iiif)
 [![CKAN](https://img.shields.io/badge/ckan-2.9.7-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
 [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg?style=flat-square)](https://www.python.org/)
```

### Comparing `ckanext-iiif-3.0.8/ckanext_iiif.egg-info/SOURCES.txt` & `ckanext-iiif-3.0.9/ckanext_iiif.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-iiif-3.0.8/docs/_scripts/gen_api_pages.py` & `ckanext-iiif-3.0.9/docs/_scripts/gen_api_pages.py`

 * *Files identical despite different names*

### Comparing `ckanext-iiif-3.0.8/pyproject.toml` & `ckanext-iiif-3.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ckanext-iiif"
-version = "3.0.8"
+version = "3.0.9"
 description = "IIIF for CKAN"
 readme = "README.md"
 requires-python = ">=3.6"
 license = { text = "GPL-3.0-or-later" }
 authors = [
     { name = "Natural History Museum", email = "data@nhm.ac.uk" }
 ]
@@ -51,15 +51,15 @@
 exclude = ["tests", "docs"]
 
 [tool.setuptools.package-data]
 "ckanext.iiif.theme" = ["*", "**/*"]
 
 [tool.commitizen]
 name = "cz_nhm"
-version = "3.0.8"
+version = "3.0.9"
 tag_format = "v$version"
 update_changelog_on_bump = true
 changelog_incremental = true
 version_files = [
     "pyproject.toml:version"
 ]
```

### Comparing `ckanext-iiif-3.0.8/tests/integration/test_actions.py` & `ckanext-iiif-3.0.9/tests/integration/test_actions.py`

 * *Files identical despite different names*

### Comparing `ckanext-iiif-3.0.8/tests/integration/test_auth.py` & `ckanext-iiif-3.0.9/tests/integration/test_auth.py`

 * *Files identical despite different names*

### Comparing `ckanext-iiif-3.0.8/tests/integration/test_iiif_route.py` & `ckanext-iiif-3.0.9/tests/integration/test_iiif_route.py`

 * *Files identical despite different names*

### Comparing `ckanext-iiif-3.0.8/tests/unit/builders/test_manifest.py` & `ckanext-iiif-3.0.9/tests/unit/builders/test_manifest.py`

 * *Files identical despite different names*

### Comparing `ckanext-iiif-3.0.8/tests/unit/logic/test_actions.py` & `ckanext-iiif-3.0.9/tests/unit/logic/test_actions.py`

 * *Files identical despite different names*

### Comparing `ckanext-iiif-3.0.8/tests/unit/routes/test_iiif.py` & `ckanext-iiif-3.0.9/tests/unit/routes/test_iiif.py`

 * *Files identical despite different names*

### Comparing `ckanext-iiif-3.0.8/tests/unit/test_plugin.py` & `ckanext-iiif-3.0.9/tests/unit/test_plugin.py`

 * *Files identical despite different names*

