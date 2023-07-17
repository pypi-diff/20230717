# Comparing `tmp/ckanext-contact-2.3.0.tar.gz` & `tmp/ckanext-contact-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-contact-2.3.0.tar", last modified: Tue Apr 11 08:14:57 2023, max compression
+gzip compressed data, was "ckanext-contact-2.3.1.tar", last modified: Mon Jul 17 08:15:26 2023, max compression
```

## Comparing `ckanext-contact-2.3.0.tar` & `ckanext-contact-2.3.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:14:57.304059 ckanext-contact-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-11 08:14:39.000000 ckanext-contact-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-04-11 08:14:57.304059 ckanext-contact-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-04-11 08:14:39.000000 ckanext-contact-2.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:14:57.300058 ckanext-contact-2.3.0/ckanext/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-11 08:14:39.000000 ckanext-contact-2.3.0/ckanext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:14:57.300058 ckanext-contact-2.3.0/ckanext/contact/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-11 08:14:39.000000 ckanext-contact-2.3.0/ckanext/contact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-11 08:14:39.000000 ckanext-contact-2.3.0/ckanext/contact/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-11 08:14:39.000000 ckanext-contact-2.3.0/ckanext/contact/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-11 08:14:39.000000 ckanext-contact-2.3.0/ckanext/contact/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-11 08:14:39.000000 ckanext-contact-2.3.0/ckanext/contact/recaptcha.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:14:57.300058 ckanext-contact-2.3.0/ckanext/contact/routes/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-11 08:14:39.000000 ckanext-contact-2.3.0/ckanext/contact/routes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-04-11 08:14:39.000000 ckanext-contact-2.3.0/ckanext/contact/routes/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-04-11 08:14:39.000000 ckanext-contact-2.3.0/ckanext/contact/routes/contact.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:14:57.296059 ckanext-contact-2.3.0/ckanext/contact/theme/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:14:57.300058 ckanext-contact-2.3.0/ckanext/contact/theme/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:14:57.300058 ckanext-contact-2.3.0/ckanext/contact/theme/assets/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-11 08:14:39.000000 ckanext-contact-2.3.0/ckanext/contact/theme/assets/modules/form-contact.js
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-04-11 08:14:39.000000 ckanext-contact-2.3.0/ckanext/contact/theme/assets/modules/modal-contact.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:14:57.300058 ckanext-contact-2.3.0/ckanext/contact/theme/assets/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-04-11 08:14:39.000000 ckanext-contact-2.3.0/ckanext/contact/theme/assets/scripts/recaptcha_helpers.js
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-11 08:14:39.000000 ckanext-contact-2.3.0/ckanext/contact/theme/assets/webassets.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:14:57.300058 ckanext-contact-2.3.0/ckanext/contact/theme/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:14:57.300058 ckanext-contact-2.3.0/ckanext/contact/theme/templates/ajax_snippets/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-11 08:14:39.000000 ckanext-contact-2.3.0/ckanext/contact/theme/templates/ajax_snippets/contact_form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:14:57.300058 ckanext-contact-2.3.0/ckanext/contact/theme/templates/contact/
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-11 08:14:39.000000 ckanext-contact-2.3.0/ckanext/contact/theme/templates/contact/form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:14:57.300058 ckanext-contact-2.3.0/ckanext/contact/theme/templates/contact/snippets/
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-11 08:14:39.000000 ckanext-contact-2.3.0/ckanext/contact/theme/templates/contact/snippets/form.html
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-11 08:14:39.000000 ckanext-contact-2.3.0/ckanext/contact/theme/templates/contact/snippets/modal_link.html
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-11 08:14:39.000000 ckanext-contact-2.3.0/ckanext/contact/theme/templates/contact/success.html
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-11 08:14:39.000000 ckanext-contact-2.3.0/ckanext/contact/theme/templates/header.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:14:57.304059 ckanext-contact-2.3.0/ckanext_contact.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-04-11 08:14:57.000000 ckanext-contact-2.3.0/ckanext_contact.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-11 08:14:57.000000 ckanext-contact-2.3.0/ckanext_contact.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:14:57.000000 ckanext-contact-2.3.0/ckanext_contact.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-11 08:14:57.000000 ckanext-contact-2.3.0/ckanext_contact.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:14:57.000000 ckanext-contact-2.3.0/ckanext_contact.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-11 08:14:57.000000 ckanext-contact-2.3.0/ckanext_contact.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-11 08:14:57.000000 ckanext-contact-2.3.0/ckanext_contact.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:14:57.300058 ckanext-contact-2.3.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:14:57.304059 ckanext-contact-2.3.0/docs/_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-11 08:14:39.000000 ckanext-contact-2.3.0/docs/_scripts/gen_api_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-11 08:14:39.000000 ckanext-contact-2.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 08:14:57.304059 ckanext-contact-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-11 08:14:39.000000 ckanext-contact-2.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:14:57.300058 ckanext-contact-2.3.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:14:57.304059 ckanext-contact-2.3.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:14:39.000000 ckanext-contact-2.3.0/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-11 08:14:39.000000 ckanext-contact-2.3.0/tests/unit/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-04-11 08:14:39.000000 ckanext-contact-2.3.0/tests/unit/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:15:26.444877 ckanext-contact-2.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-17 08:15:10.000000 ckanext-contact-2.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6528 2023-07-17 08:15:26.444877 ckanext-contact-2.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-07-17 08:15:10.000000 ckanext-contact-2.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:15:26.440877 ckanext-contact-2.3.1/ckanext/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-17 08:15:10.000000 ckanext-contact-2.3.1/ckanext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:15:26.440877 ckanext-contact-2.3.1/ckanext/contact/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-17 08:15:10.000000 ckanext-contact-2.3.1/ckanext/contact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-17 08:15:10.000000 ckanext-contact-2.3.1/ckanext/contact/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-17 08:15:10.000000 ckanext-contact-2.3.1/ckanext/contact/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-07-17 08:15:10.000000 ckanext-contact-2.3.1/ckanext/contact/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-17 08:15:10.000000 ckanext-contact-2.3.1/ckanext/contact/recaptcha.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:15:26.440877 ckanext-contact-2.3.1/ckanext/contact/routes/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-17 08:15:10.000000 ckanext-contact-2.3.1/ckanext/contact/routes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-07-17 08:15:10.000000 ckanext-contact-2.3.1/ckanext/contact/routes/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-07-17 08:15:10.000000 ckanext-contact-2.3.1/ckanext/contact/routes/contact.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:15:26.436877 ckanext-contact-2.3.1/ckanext/contact/theme/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:15:26.440877 ckanext-contact-2.3.1/ckanext/contact/theme/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:15:26.440877 ckanext-contact-2.3.1/ckanext/contact/theme/assets/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-17 08:15:10.000000 ckanext-contact-2.3.1/ckanext/contact/theme/assets/modules/form-contact.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-07-17 08:15:10.000000 ckanext-contact-2.3.1/ckanext/contact/theme/assets/modules/modal-contact.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:15:26.440877 ckanext-contact-2.3.1/ckanext/contact/theme/assets/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-07-17 08:15:10.000000 ckanext-contact-2.3.1/ckanext/contact/theme/assets/scripts/recaptcha_helpers.js
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-17 08:15:10.000000 ckanext-contact-2.3.1/ckanext/contact/theme/assets/webassets.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:15:26.440877 ckanext-contact-2.3.1/ckanext/contact/theme/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:15:26.440877 ckanext-contact-2.3.1/ckanext/contact/theme/templates/ajax_snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-17 08:15:10.000000 ckanext-contact-2.3.1/ckanext/contact/theme/templates/ajax_snippets/contact_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:15:26.440877 ckanext-contact-2.3.1/ckanext/contact/theme/templates/contact/
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-17 08:15:10.000000 ckanext-contact-2.3.1/ckanext/contact/theme/templates/contact/form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:15:26.440877 ckanext-contact-2.3.1/ckanext/contact/theme/templates/contact/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-07-17 08:15:10.000000 ckanext-contact-2.3.1/ckanext/contact/theme/templates/contact/snippets/form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-17 08:15:10.000000 ckanext-contact-2.3.1/ckanext/contact/theme/templates/contact/snippets/modal_link.html
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-17 08:15:10.000000 ckanext-contact-2.3.1/ckanext/contact/theme/templates/contact/success.html
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-17 08:15:10.000000 ckanext-contact-2.3.1/ckanext/contact/theme/templates/header.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:15:26.440877 ckanext-contact-2.3.1/ckanext_contact.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6528 2023-07-17 08:15:26.000000 ckanext-contact-2.3.1/ckanext_contact.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-17 08:15:26.000000 ckanext-contact-2.3.1/ckanext_contact.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 08:15:26.000000 ckanext-contact-2.3.1/ckanext_contact.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-17 08:15:26.000000 ckanext-contact-2.3.1/ckanext_contact.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 08:15:26.000000 ckanext-contact-2.3.1/ckanext_contact.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-17 08:15:26.000000 ckanext-contact-2.3.1/ckanext_contact.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-17 08:15:26.000000 ckanext-contact-2.3.1/ckanext_contact.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:15:26.440877 ckanext-contact-2.3.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:15:26.444877 ckanext-contact-2.3.1/docs/_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-17 08:15:10.000000 ckanext-contact-2.3.1/docs/_scripts/gen_api_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-17 08:15:10.000000 ckanext-contact-2.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 08:15:26.444877 ckanext-contact-2.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-17 08:15:10.000000 ckanext-contact-2.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:15:26.440877 ckanext-contact-2.3.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:15:26.444877 ckanext-contact-2.3.1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:15:10.000000 ckanext-contact-2.3.1/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-17 08:15:10.000000 ckanext-contact-2.3.1/tests/unit/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-07-17 08:15:10.000000 ckanext-contact-2.3.1/tests/unit/test_helpers.py
```

### Comparing `ckanext-contact-2.3.0/LICENSE` & `ckanext-contact-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-contact-2.3.0/PKG-INFO` & `ckanext-contact-2.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-contact
-Version: 2.3.0
+Version: 2.3.1
 Summary: A CKAN extension for adding popup contact forms to pages.
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-contact
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-contact/blob/main/CHANGELOG.md
 Keywords: CKAN,data,contact
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 <!--header-start-->
-<img src="https://github.com/NaturalHistoryMuseum/ckanext-contact/raw/main/.github/nhm-logo.svg" align="left" width="150px" height="100px" hspace="40"/>
+<img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-contact
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-contact/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-contact/actions/workflows/main.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/NaturalHistoryMuseum/ckanext-contact/main?style=flat-square)](https://coveralls.io/github/NaturalHistoryMuseum/ckanext-contact)
 [![CKAN](https://img.shields.io/badge/ckan-2.9.7-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
 [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg?style=flat-square)](https://www.python.org/)
```

### Comparing `ckanext-contact-2.3.0/README.md` & `ckanext-contact-2.3.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <!--header-start-->
-<img src="https://github.com/NaturalHistoryMuseum/ckanext-contact/raw/main/.github/nhm-logo.svg" align="left" width="150px" height="100px" hspace="40"/>
+<img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-contact
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-contact/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-contact/actions/workflows/main.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/NaturalHistoryMuseum/ckanext-contact/main?style=flat-square)](https://coveralls.io/github/NaturalHistoryMuseum/ckanext-contact)
 [![CKAN](https://img.shields.io/badge/ckan-2.9.7-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
 [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg?style=flat-square)](https://www.python.org/)
```

### Comparing `ckanext-contact-2.3.0/ckanext/contact/interfaces.py` & `ckanext-contact-2.3.1/ckanext/contact/interfaces.py`

 * *Files identical despite different names*

### Comparing `ckanext-contact-2.3.0/ckanext/contact/plugin.py` & `ckanext-contact-2.3.1/ckanext/contact/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-contact-2.3.0/ckanext/contact/recaptcha.py` & `ckanext-contact-2.3.1/ckanext/contact/recaptcha.py`

 * *Files identical despite different names*

### Comparing `ckanext-contact-2.3.0/ckanext/contact/routes/_helpers.py` & `ckanext-contact-2.3.1/ckanext/contact/routes/_helpers.py`

 * *Files identical despite different names*

### Comparing `ckanext-contact-2.3.0/ckanext/contact/routes/contact.py` & `ckanext-contact-2.3.1/ckanext/contact/routes/contact.py`

 * *Files identical despite different names*

### Comparing `ckanext-contact-2.3.0/ckanext/contact/theme/assets/modules/form-contact.js` & `ckanext-contact-2.3.1/ckanext/contact/theme/assets/modules/form-contact.js`

 * *Files identical despite different names*

### Comparing `ckanext-contact-2.3.0/ckanext/contact/theme/assets/modules/modal-contact.js` & `ckanext-contact-2.3.1/ckanext/contact/theme/assets/modules/modal-contact.js`

 * *Files identical despite different names*

### Comparing `ckanext-contact-2.3.0/ckanext/contact/theme/assets/scripts/recaptcha_helpers.js` & `ckanext-contact-2.3.1/ckanext/contact/theme/assets/scripts/recaptcha_helpers.js`

 * *Files identical despite different names*

### Comparing `ckanext-contact-2.3.0/ckanext/contact/theme/templates/ajax_snippets/contact_form.html` & `ckanext-contact-2.3.1/ckanext/contact/theme/templates/ajax_snippets/contact_form.html`

 * *Files identical despite different names*

### Comparing `ckanext-contact-2.3.0/ckanext/contact/theme/templates/contact/form.html` & `ckanext-contact-2.3.1/ckanext/contact/theme/templates/contact/form.html`

 * *Files identical despite different names*

### Comparing `ckanext-contact-2.3.0/ckanext/contact/theme/templates/contact/snippets/form.html` & `ckanext-contact-2.3.1/ckanext/contact/theme/templates/contact/snippets/form.html`

 * *Files identical despite different names*

### Comparing `ckanext-contact-2.3.0/ckanext/contact/theme/templates/contact/success.html` & `ckanext-contact-2.3.1/ckanext/contact/theme/templates/contact/success.html`

 * *Files identical despite different names*

### Comparing `ckanext-contact-2.3.0/ckanext_contact.egg-info/PKG-INFO` & `ckanext-contact-2.3.1/ckanext_contact.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-contact
-Version: 2.3.0
+Version: 2.3.1
 Summary: A CKAN extension for adding popup contact forms to pages.
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-contact
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-contact/blob/main/CHANGELOG.md
 Keywords: CKAN,data,contact
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 <!--header-start-->
-<img src="https://github.com/NaturalHistoryMuseum/ckanext-contact/raw/main/.github/nhm-logo.svg" align="left" width="150px" height="100px" hspace="40"/>
+<img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-contact
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-contact/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-contact/actions/workflows/main.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/NaturalHistoryMuseum/ckanext-contact/main?style=flat-square)](https://coveralls.io/github/NaturalHistoryMuseum/ckanext-contact)
 [![CKAN](https://img.shields.io/badge/ckan-2.9.7-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
 [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg?style=flat-square)](https://www.python.org/)
```

### Comparing `ckanext-contact-2.3.0/ckanext_contact.egg-info/SOURCES.txt` & `ckanext-contact-2.3.1/ckanext_contact.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-contact-2.3.0/docs/_scripts/gen_api_pages.py` & `ckanext-contact-2.3.1/docs/_scripts/gen_api_pages.py`

 * *Files identical despite different names*

### Comparing `ckanext-contact-2.3.0/pyproject.toml` & `ckanext-contact-2.3.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ckanext-contact"
-version = "2.3.0"
+version = "2.3.1"
 description = "A CKAN extension for adding popup contact forms to pages."
 readme = "README.md"
 requires-python = ">=3.6"
 license = { text = "GPL-3.0-or-later" }
 authors = [
     { name = "Natural History Museum", email = "data@nhm.ac.uk" }
 ]
@@ -51,15 +51,15 @@
 exclude = ["tests", "docs"]
 
 [tool.setuptools.package-data]
 "ckanext.contact.theme" = ["*", "**/*"]
 
 [tool.commitizen]
 name = "cz_nhm"
-version = "2.3.0"
+version = "2.3.1"
 tag_format = "v$version"
 update_changelog_on_bump = true
 changelog_incremental = true
 version_files = [
     "pyproject.toml:version"
 ]
```

### Comparing `ckanext-contact-2.3.0/tests/unit/test_auth.py` & `ckanext-contact-2.3.1/tests/unit/test_auth.py`

 * *Files identical despite different names*

### Comparing `ckanext-contact-2.3.0/tests/unit/test_helpers.py` & `ckanext-contact-2.3.1/tests/unit/test_helpers.py`

 * *Files identical despite different names*

