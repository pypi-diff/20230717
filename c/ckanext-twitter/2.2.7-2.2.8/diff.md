# Comparing `tmp/ckanext-twitter-2.2.7.tar.gz` & `tmp/ckanext-twitter-2.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-twitter-2.2.7.tar", last modified: Tue Apr 11 08:35:17 2023, max compression
+gzip compressed data, was "ckanext-twitter-2.2.8.tar", last modified: Mon Jul 17 08:22:54 2023, max compression
```

## Comparing `ckanext-twitter-2.2.7.tar` & `ckanext-twitter-2.2.8.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:35:17.990094 ckanext-twitter-2.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-11 08:35:05.000000 ckanext-twitter-2.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9442 2023-04-11 08:35:17.990094 ckanext-twitter-2.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8497 2023-04-11 08:35:05.000000 ckanext-twitter-2.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:35:17.986094 ckanext-twitter-2.2.7/ckanext/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-11 08:35:05.000000 ckanext-twitter-2.2.7/ckanext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:35:17.986094 ckanext-twitter-2.2.7/ckanext/twitter/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-11 08:35:05.000000 ckanext-twitter-2.2.7/ckanext/twitter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:35:17.986094 ckanext-twitter-2.2.7/ckanext/twitter/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:35:05.000000 ckanext-twitter-2.2.7/ckanext/twitter/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-11 08:35:05.000000 ckanext-twitter-2.2.7/ckanext/twitter/lib/cache_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-04-11 08:35:05.000000 ckanext-twitter-2.2.7/ckanext/twitter/lib/config_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-04-11 08:35:05.000000 ckanext-twitter-2.2.7/ckanext/twitter/lib/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-04-11 08:35:05.000000 ckanext-twitter-2.2.7/ckanext/twitter/lib/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-04-11 08:35:05.000000 ckanext-twitter-2.2.7/ckanext/twitter/lib/twitter_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-11 08:35:05.000000 ckanext-twitter-2.2.7/ckanext/twitter/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:35:17.986094 ckanext-twitter-2.2.7/ckanext/twitter/routes/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-11 08:35:05.000000 ckanext-twitter-2.2.7/ckanext/twitter/routes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-11 08:35:05.000000 ckanext-twitter-2.2.7/ckanext/twitter/routes/tweet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:35:17.982094 ckanext-twitter-2.2.7/ckanext/twitter/theme/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:35:17.990094 ckanext-twitter-2.2.7/ckanext/twitter/theme/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:35:17.982094 ckanext-twitter-2.2.7/ckanext/twitter/theme/assets/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:35:17.990094 ckanext-twitter-2.2.7/ckanext/twitter/theme/assets/scripts/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-11 08:35:05.000000 ckanext-twitter-2.2.7/ckanext/twitter/theme/assets/scripts/modules/confirm-tweet.js
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-11 08:35:05.000000 ckanext-twitter-2.2.7/ckanext/twitter/theme/assets/webassets.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:35:17.982094 ckanext-twitter-2.2.7/ckanext/twitter/theme/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:35:17.990094 ckanext-twitter-2.2.7/ckanext/twitter/theme/templates/ajax_snippets/
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-11 08:35:05.000000 ckanext-twitter-2.2.7/ckanext/twitter/theme/templates/ajax_snippets/edit_tweet.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:35:17.990094 ckanext-twitter-2.2.7/ckanext/twitter/theme/templates/package/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-11 08:35:05.000000 ckanext-twitter-2.2.7/ckanext/twitter/theme/templates/package/base.html
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-11 08:35:05.000000 ckanext-twitter-2.2.7/ckanext/twitter/theme/templates/package/read_base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:35:17.990094 ckanext-twitter-2.2.7/ckanext_twitter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9442 2023-04-11 08:35:17.000000 ckanext-twitter-2.2.7/ckanext_twitter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-11 08:35:17.000000 ckanext-twitter-2.2.7/ckanext_twitter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:35:17.000000 ckanext-twitter-2.2.7/ckanext_twitter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-11 08:35:17.000000 ckanext-twitter-2.2.7/ckanext_twitter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:35:17.000000 ckanext-twitter-2.2.7/ckanext_twitter.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-11 08:35:17.000000 ckanext-twitter-2.2.7/ckanext_twitter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-11 08:35:17.000000 ckanext-twitter-2.2.7/ckanext_twitter.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:35:17.982094 ckanext-twitter-2.2.7/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:35:17.990094 ckanext-twitter-2.2.7/docs/_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-11 08:35:05.000000 ckanext-twitter-2.2.7/docs/_scripts/gen_api_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-11 08:35:05.000000 ckanext-twitter-2.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 08:35:17.990094 ckanext-twitter-2.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-11 08:35:05.000000 ckanext-twitter-2.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:35:17.990094 ckanext-twitter-2.2.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-04-11 08:35:05.000000 ckanext-twitter-2.2.7/tests/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-04-11 08:35:05.000000 ckanext-twitter-2.2.7/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-11 08:35:05.000000 ckanext-twitter-2.2.7/tests/test_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-11 08:35:05.000000 ckanext-twitter-2.2.7/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-04-11 08:35:05.000000 ckanext-twitter-2.2.7/tests/test_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-04-11 08:35:05.000000 ckanext-twitter-2.2.7/tests/test_routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-04-11 08:35:05.000000 ckanext-twitter-2.2.7/tests/test_templatehelpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:22:54.974515 ckanext-twitter-2.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-17 08:22:43.000000 ckanext-twitter-2.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-07-17 08:22:54.974515 ckanext-twitter-2.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-07-17 08:22:43.000000 ckanext-twitter-2.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:22:54.970515 ckanext-twitter-2.2.8/ckanext/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-17 08:22:43.000000 ckanext-twitter-2.2.8/ckanext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:22:54.970515 ckanext-twitter-2.2.8/ckanext/twitter/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-17 08:22:43.000000 ckanext-twitter-2.2.8/ckanext/twitter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:22:54.974515 ckanext-twitter-2.2.8/ckanext/twitter/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:22:43.000000 ckanext-twitter-2.2.8/ckanext/twitter/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-17 08:22:43.000000 ckanext-twitter-2.2.8/ckanext/twitter/lib/cache_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-07-17 08:22:43.000000 ckanext-twitter-2.2.8/ckanext/twitter/lib/config_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-17 08:22:43.000000 ckanext-twitter-2.2.8/ckanext/twitter/lib/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-07-17 08:22:43.000000 ckanext-twitter-2.2.8/ckanext/twitter/lib/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-07-17 08:22:43.000000 ckanext-twitter-2.2.8/ckanext/twitter/lib/twitter_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-07-17 08:22:43.000000 ckanext-twitter-2.2.8/ckanext/twitter/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:22:54.974515 ckanext-twitter-2.2.8/ckanext/twitter/routes/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-17 08:22:43.000000 ckanext-twitter-2.2.8/ckanext/twitter/routes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-17 08:22:43.000000 ckanext-twitter-2.2.8/ckanext/twitter/routes/tweet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:22:54.970515 ckanext-twitter-2.2.8/ckanext/twitter/theme/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:22:54.974515 ckanext-twitter-2.2.8/ckanext/twitter/theme/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:22:54.970515 ckanext-twitter-2.2.8/ckanext/twitter/theme/assets/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:22:54.974515 ckanext-twitter-2.2.8/ckanext/twitter/theme/assets/scripts/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-07-17 08:22:43.000000 ckanext-twitter-2.2.8/ckanext/twitter/theme/assets/scripts/modules/confirm-tweet.js
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-17 08:22:43.000000 ckanext-twitter-2.2.8/ckanext/twitter/theme/assets/webassets.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:22:54.970515 ckanext-twitter-2.2.8/ckanext/twitter/theme/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:22:54.974515 ckanext-twitter-2.2.8/ckanext/twitter/theme/templates/ajax_snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-17 08:22:43.000000 ckanext-twitter-2.2.8/ckanext/twitter/theme/templates/ajax_snippets/edit_tweet.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:22:54.974515 ckanext-twitter-2.2.8/ckanext/twitter/theme/templates/package/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-17 08:22:43.000000 ckanext-twitter-2.2.8/ckanext/twitter/theme/templates/package/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-17 08:22:43.000000 ckanext-twitter-2.2.8/ckanext/twitter/theme/templates/package/read_base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:22:54.974515 ckanext-twitter-2.2.8/ckanext_twitter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-07-17 08:22:54.000000 ckanext-twitter-2.2.8/ckanext_twitter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-17 08:22:54.000000 ckanext-twitter-2.2.8/ckanext_twitter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 08:22:54.000000 ckanext-twitter-2.2.8/ckanext_twitter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-17 08:22:54.000000 ckanext-twitter-2.2.8/ckanext_twitter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 08:22:54.000000 ckanext-twitter-2.2.8/ckanext_twitter.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-17 08:22:54.000000 ckanext-twitter-2.2.8/ckanext_twitter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-17 08:22:54.000000 ckanext-twitter-2.2.8/ckanext_twitter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:22:54.970515 ckanext-twitter-2.2.8/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:22:54.974515 ckanext-twitter-2.2.8/docs/_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-17 08:22:43.000000 ckanext-twitter-2.2.8/docs/_scripts/gen_api_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-07-17 08:22:43.000000 ckanext-twitter-2.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 08:22:54.974515 ckanext-twitter-2.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-17 08:22:43.000000 ckanext-twitter-2.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:22:54.974515 ckanext-twitter-2.2.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-07-17 08:22:43.000000 ckanext-twitter-2.2.8/tests/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-17 08:22:43.000000 ckanext-twitter-2.2.8/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-17 08:22:43.000000 ckanext-twitter-2.2.8/tests/test_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-17 08:22:43.000000 ckanext-twitter-2.2.8/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-07-17 08:22:43.000000 ckanext-twitter-2.2.8/tests/test_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-07-17 08:22:43.000000 ckanext-twitter-2.2.8/tests/test_routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-07-17 08:22:43.000000 ckanext-twitter-2.2.8/tests/test_templatehelpers.py
```

### Comparing `ckanext-twitter-2.2.7/LICENSE` & `ckanext-twitter-2.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-twitter-2.2.7/PKG-INFO` & `ckanext-twitter-2.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-twitter
-Version: 2.2.7
+Version: 2.2.8
 Summary: A CKAN extension that enables users to post a tweet every time a dataset is created or updated.
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-twitter
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-twitter/blob/main/CHANGELOG.md
 Keywords: CKAN,data,twitter
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 <!--header-start-->
-<img src="https://github.com/NaturalHistoryMuseum/ckanext-twitter/raw/main/.github/nhm-logo.svg" align="left" width="150px" height="100px" hspace="40"/>
+<img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-twitter
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-twitter/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-twitter/actions/workflows/main.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/NaturalHistoryMuseum/ckanext-twitter/main?style=flat-square)](https://coveralls.io/github/NaturalHistoryMuseum/ckanext-twitter)
 [![CKAN](https://img.shields.io/badge/ckan-2.9.7-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
 [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg?style=flat-square)](https://www.python.org/)
```

### Comparing `ckanext-twitter-2.2.7/README.md` & `ckanext-twitter-2.2.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <!--header-start-->
-<img src="https://github.com/NaturalHistoryMuseum/ckanext-twitter/raw/main/.github/nhm-logo.svg" align="left" width="150px" height="100px" hspace="40"/>
+<img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-twitter
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-twitter/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-twitter/actions/workflows/main.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/NaturalHistoryMuseum/ckanext-twitter/main?style=flat-square)](https://coveralls.io/github/NaturalHistoryMuseum/ckanext-twitter)
 [![CKAN](https://img.shields.io/badge/ckan-2.9.7-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
 [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg?style=flat-square)](https://www.python.org/)
```

### Comparing `ckanext-twitter-2.2.7/ckanext/twitter/lib/cache_helpers.py` & `ckanext-twitter-2.2.8/ckanext/twitter/lib/cache_helpers.py`

 * *Files identical despite different names*

### Comparing `ckanext-twitter-2.2.7/ckanext/twitter/lib/config_helpers.py` & `ckanext-twitter-2.2.8/ckanext/twitter/lib/config_helpers.py`

 * *Files identical despite different names*

### Comparing `ckanext-twitter-2.2.7/ckanext/twitter/lib/helpers.py` & `ckanext-twitter-2.2.8/ckanext/twitter/lib/helpers.py`

 * *Files identical despite different names*

### Comparing `ckanext-twitter-2.2.7/ckanext/twitter/lib/parsers.py` & `ckanext-twitter-2.2.8/ckanext/twitter/lib/parsers.py`

 * *Files identical despite different names*

### Comparing `ckanext-twitter-2.2.7/ckanext/twitter/lib/twitter_api.py` & `ckanext-twitter-2.2.8/ckanext/twitter/lib/twitter_api.py`

 * *Files identical despite different names*

### Comparing `ckanext-twitter-2.2.7/ckanext/twitter/plugin.py` & `ckanext-twitter-2.2.8/ckanext/twitter/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-twitter-2.2.7/ckanext/twitter/routes/tweet.py` & `ckanext-twitter-2.2.8/ckanext/twitter/routes/tweet.py`

 * *Files identical despite different names*

### Comparing `ckanext-twitter-2.2.7/ckanext/twitter/theme/assets/scripts/modules/confirm-tweet.js` & `ckanext-twitter-2.2.8/ckanext/twitter/theme/assets/scripts/modules/confirm-tweet.js`

 * *Files identical despite different names*

### Comparing `ckanext-twitter-2.2.7/ckanext/twitter/theme/templates/ajax_snippets/edit_tweet.html` & `ckanext-twitter-2.2.8/ckanext/twitter/theme/templates/ajax_snippets/edit_tweet.html`

 * *Files identical despite different names*

### Comparing `ckanext-twitter-2.2.7/ckanext_twitter.egg-info/PKG-INFO` & `ckanext-twitter-2.2.8/ckanext_twitter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-twitter
-Version: 2.2.7
+Version: 2.2.8
 Summary: A CKAN extension that enables users to post a tweet every time a dataset is created or updated.
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-twitter
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-twitter/blob/main/CHANGELOG.md
 Keywords: CKAN,data,twitter
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 <!--header-start-->
-<img src="https://github.com/NaturalHistoryMuseum/ckanext-twitter/raw/main/.github/nhm-logo.svg" align="left" width="150px" height="100px" hspace="40"/>
+<img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-twitter
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-twitter/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-twitter/actions/workflows/main.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/NaturalHistoryMuseum/ckanext-twitter/main?style=flat-square)](https://coveralls.io/github/NaturalHistoryMuseum/ckanext-twitter)
 [![CKAN](https://img.shields.io/badge/ckan-2.9.7-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
 [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg?style=flat-square)](https://www.python.org/)
```

### Comparing `ckanext-twitter-2.2.7/ckanext_twitter.egg-info/SOURCES.txt` & `ckanext-twitter-2.2.8/ckanext_twitter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-twitter-2.2.7/docs/_scripts/gen_api_pages.py` & `ckanext-twitter-2.2.8/docs/_scripts/gen_api_pages.py`

 * *Files identical despite different names*

### Comparing `ckanext-twitter-2.2.7/pyproject.toml` & `ckanext-twitter-2.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ckanext-twitter"
-version = "2.2.7"
+version = "2.2.8"
 description = "A CKAN extension that enables users to post a tweet every time a dataset is created or updated."
 readme = "README.md"
 requires-python = ">=3.6"
 license = { text = "GPL-3.0-or-later" }
 authors = [
     { name = "Natural History Museum", email = "data@nhm.ac.uk" }
 ]
@@ -52,15 +52,15 @@
 exclude = ["tests", "docs"]
 
 [tool.setuptools.package-data]
 "ckanext.twitter.theme" = ["*", "**/*"]
 
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

### Comparing `ckanext-twitter-2.2.7/tests/test_authentication.py` & `ckanext-twitter-2.2.8/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `ckanext-twitter-2.2.7/tests/test_config.py` & `ckanext-twitter-2.2.8/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `ckanext-twitter-2.2.7/tests/test_controller.py` & `ckanext-twitter-2.2.8/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `ckanext-twitter-2.2.7/tests/test_dataset.py` & `ckanext-twitter-2.2.8/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `ckanext-twitter-2.2.7/tests/test_generation.py` & `ckanext-twitter-2.2.8/tests/test_generation.py`

 * *Files identical despite different names*

### Comparing `ckanext-twitter-2.2.7/tests/test_routes.py` & `ckanext-twitter-2.2.8/tests/test_routes.py`

 * *Files identical despite different names*

### Comparing `ckanext-twitter-2.2.7/tests/test_templatehelpers.py` & `ckanext-twitter-2.2.8/tests/test_templatehelpers.py`

 * *Files identical despite different names*

