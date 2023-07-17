# Comparing `tmp/ckanext-ckanpackager-2.2.8.tar.gz` & `tmp/ckanext-ckanpackager-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-ckanpackager-2.2.8.tar", last modified: Thu Jun 29 12:42:39 2023, max compression
+gzip compressed data, was "ckanext-ckanpackager-2.2.9.tar", last modified: Mon Jul 17 08:14:00 2023, max compression
```

## Comparing `ckanext-ckanpackager-2.2.8.tar` & `ckanext-ckanpackager-2.2.9.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:42:39.741821 ckanext-ckanpackager-2.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-29 12:42:28.000000 ckanext-ckanpackager-2.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-06-29 12:42:39.741821 ckanext-ckanpackager-2.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-06-29 12:42:28.000000 ckanext-ckanpackager-2.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:42:39.737821 ckanext-ckanpackager-2.2.8/ckanext/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-29 12:42:28.000000 ckanext-ckanpackager-2.2.8/ckanext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:42:39.737821 ckanext-ckanpackager-2.2.8/ckanext/ckanpackager/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-29 12:42:28.000000 ckanext-ckanpackager-2.2.8/ckanext/ckanpackager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-29 12:42:28.000000 ckanext-ckanpackager-2.2.8/ckanext/ckanpackager/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-29 12:42:28.000000 ckanext-ckanpackager-2.2.8/ckanext/ckanpackager/interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:42:39.737821 ckanext-ckanpackager-2.2.8/ckanext/ckanpackager/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 12:42:28.000000 ckanext-ckanpackager-2.2.8/ckanext/ckanpackager/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-29 12:42:28.000000 ckanext-ckanpackager-2.2.8/ckanext/ckanpackager/lib/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-06-29 12:42:28.000000 ckanext-ckanpackager-2.2.8/ckanext/ckanpackager/lib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:42:39.737821 ckanext-ckanpackager-2.2.8/ckanext/ckanpackager/logic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 12:42:28.000000 ckanext-ckanpackager-2.2.8/ckanext/ckanpackager/logic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-06-29 12:42:28.000000 ckanext-ckanpackager-2.2.8/ckanext/ckanpackager/logic/action.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-29 12:42:28.000000 ckanext-ckanpackager-2.2.8/ckanext/ckanpackager/logic/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:42:39.737821 ckanext-ckanpackager-2.2.8/ckanext/ckanpackager/model/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-29 12:42:28.000000 ckanext-ckanpackager-2.2.8/ckanext/ckanpackager/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-29 12:42:28.000000 ckanext-ckanpackager-2.2.8/ckanext/ckanpackager/model/stat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-29 12:42:28.000000 ckanext-ckanpackager-2.2.8/ckanext/ckanpackager/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:42:39.737821 ckanext-ckanpackager-2.2.8/ckanext/ckanpackager/routes/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-29 12:42:28.000000 ckanext-ckanpackager-2.2.8/ckanext/ckanpackager/routes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-06-29 12:42:28.000000 ckanext-ckanpackager-2.2.8/ckanext/ckanpackager/routes/packager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:42:39.737821 ckanext-ckanpackager-2.2.8/ckanext/ckanpackager/theme/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:42:39.737821 ckanext-ckanpackager-2.2.8/ckanext/ckanpackager/theme/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:42:39.737821 ckanext-ckanpackager-2.2.8/ckanext/ckanpackager/theme/assets/less/
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-29 12:42:28.000000 ckanext-ckanpackager-2.2.8/ckanext/ckanpackager/theme/assets/less/ckanpackager.less
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:42:39.737821 ckanext-ckanpackager-2.2.8/ckanext/ckanpackager/theme/assets/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:42:39.737821 ckanext-ckanpackager-2.2.8/ckanext/ckanpackager/theme/assets/scripts/modules/
--rw-r--r--   0 runner    (1001) docker     (123)    13051 2023-06-29 12:42:28.000000 ckanext-ckanpackager-2.2.8/ckanext/ckanpackager/theme/assets/scripts/modules/ckanpackager-download-link.js
--rwxr-xr-x   0 runner    (1001) docker     (123)      302 2023-06-29 12:42:28.000000 ckanext-ckanpackager-2.2.8/ckanext/ckanpackager/theme/assets/webassets.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:42:39.737821 ckanext-ckanpackager-2.2.8/ckanext/ckanpackager/theme/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:42:39.741821 ckanext-ckanpackager-2.2.8/ckanext/ckanpackager/theme/templates/ajax_snippets/
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-06-29 12:42:28.000000 ckanext-ckanpackager-2.2.8/ckanext/ckanpackager/theme/templates/ajax_snippets/ckanpackager_form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:42:39.737821 ckanext-ckanpackager-2.2.8/ckanext/ckanpackager/theme/templates/ckanpackager/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:42:39.741821 ckanext-ckanpackager-2.2.8/ckanext/ckanpackager/theme/templates/ckanpackager/snippets/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-29 12:42:28.000000 ckanext-ckanpackager-2.2.8/ckanext/ckanpackager/theme/templates/ckanpackager/snippets/package_resource.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:42:39.741821 ckanext-ckanpackager-2.2.8/ckanext_ckanpackager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-06-29 12:42:39.000000 ckanext-ckanpackager-2.2.8/ckanext_ckanpackager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-29 12:42:39.000000 ckanext-ckanpackager-2.2.8/ckanext_ckanpackager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 12:42:39.000000 ckanext-ckanpackager-2.2.8/ckanext_ckanpackager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-29 12:42:39.000000 ckanext-ckanpackager-2.2.8/ckanext_ckanpackager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 12:42:39.000000 ckanext-ckanpackager-2.2.8/ckanext_ckanpackager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-29 12:42:39.000000 ckanext-ckanpackager-2.2.8/ckanext_ckanpackager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-29 12:42:39.000000 ckanext-ckanpackager-2.2.8/ckanext_ckanpackager.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:42:39.737821 ckanext-ckanpackager-2.2.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:42:39.741821 ckanext-ckanpackager-2.2.8/docs/_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-29 12:42:28.000000 ckanext-ckanpackager-2.2.8/docs/_scripts/gen_api_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-06-29 12:42:28.000000 ckanext-ckanpackager-2.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 12:42:39.741821 ckanext-ckanpackager-2.2.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      210 2023-06-29 12:42:28.000000 ckanext-ckanpackager-2.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:42:39.741821 ckanext-ckanpackager-2.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-29 12:42:28.000000 ckanext-ckanpackager-2.2.8/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-29 12:42:28.000000 ckanext-ckanpackager-2.2.8/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:14:00.404229 ckanext-ckanpackager-2.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-17 08:13:48.000000 ckanext-ckanpackager-2.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-07-17 08:14:00.404229 ckanext-ckanpackager-2.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-07-17 08:13:48.000000 ckanext-ckanpackager-2.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:14:00.400229 ckanext-ckanpackager-2.2.9/ckanext/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-17 08:13:48.000000 ckanext-ckanpackager-2.2.9/ckanext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:14:00.400229 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-17 08:13:48.000000 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-17 08:13:48.000000 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-17 08:13:48.000000 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:14:00.400229 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:48.000000 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-17 08:13:48.000000 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/lib/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-07-17 08:13:48.000000 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/lib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:14:00.400229 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/logic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:48.000000 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/logic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-07-17 08:13:48.000000 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/logic/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-17 08:13:48.000000 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/logic/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:14:00.400229 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-17 08:13:48.000000 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-17 08:13:48.000000 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/model/stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-17 08:13:48.000000 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:14:00.400229 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/routes/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-17 08:13:48.000000 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/routes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-07-17 08:13:48.000000 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/routes/packager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:14:00.400229 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/theme/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:14:00.404229 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/theme/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:14:00.404229 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/theme/assets/less/
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-17 08:13:48.000000 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/theme/assets/less/ckanpackager.less
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:14:00.400229 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/theme/assets/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:14:00.404229 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/theme/assets/scripts/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)    13051 2023-07-17 08:13:48.000000 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/theme/assets/scripts/modules/ckanpackager-download-link.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)      302 2023-07-17 08:13:48.000000 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/theme/assets/webassets.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:14:00.400229 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/theme/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:14:00.404229 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/theme/templates/ajax_snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-17 08:13:48.000000 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/theme/templates/ajax_snippets/ckanpackager_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:14:00.400229 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/theme/templates/ckanpackager/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:14:00.404229 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/theme/templates/ckanpackager/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-17 08:13:48.000000 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/theme/templates/ckanpackager/snippets/package_resource.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:14:00.404229 ckanext-ckanpackager-2.2.9/ckanext_ckanpackager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-07-17 08:14:00.000000 ckanext-ckanpackager-2.2.9/ckanext_ckanpackager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-17 08:14:00.000000 ckanext-ckanpackager-2.2.9/ckanext_ckanpackager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 08:14:00.000000 ckanext-ckanpackager-2.2.9/ckanext_ckanpackager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-17 08:14:00.000000 ckanext-ckanpackager-2.2.9/ckanext_ckanpackager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 08:14:00.000000 ckanext-ckanpackager-2.2.9/ckanext_ckanpackager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-17 08:14:00.000000 ckanext-ckanpackager-2.2.9/ckanext_ckanpackager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-17 08:14:00.000000 ckanext-ckanpackager-2.2.9/ckanext_ckanpackager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:14:00.400229 ckanext-ckanpackager-2.2.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:14:00.404229 ckanext-ckanpackager-2.2.9/docs/_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-17 08:13:48.000000 ckanext-ckanpackager-2.2.9/docs/_scripts/gen_api_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-07-17 08:13:48.000000 ckanext-ckanpackager-2.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 08:14:00.404229 ckanext-ckanpackager-2.2.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      210 2023-07-17 08:13:48.000000 ckanext-ckanpackager-2.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:14:00.404229 ckanext-ckanpackager-2.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-17 08:13:48.000000 ckanext-ckanpackager-2.2.9/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-07-17 08:13:48.000000 ckanext-ckanpackager-2.2.9/tests/test_utils.py
```

### Comparing `ckanext-ckanpackager-2.2.8/LICENSE` & `ckanext-ckanpackager-2.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-ckanpackager-2.2.8/PKG-INFO` & `ckanext-ckanpackager-2.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-ckanpackager
-Version: 2.2.8
+Version: 2.2.9
 Summary: A CKAN extension that provides a user interface to download resources with ckanpackager.
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-ckanpackager
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-ckanpackager/blob/main/CHANGELOG.md
 Keywords: CKAN,data,ckanpackager
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 <!--header-start-->
-<img src="https://github.com/NaturalHistoryMuseum/ckanext-ckanpackager/raw/main/.github/nhm-logo.svg" align="left" width="150px" height="100px" hspace="40"/>
+<img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-ckanpackager
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-ckanpackager/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-ckanpackager/actions/workflows/main.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/NaturalHistoryMuseum/ckanext-ckanpackager/main?style=flat-square)](https://coveralls.io/github/NaturalHistoryMuseum/ckanext-ckanpackager)
 [![CKAN](https://img.shields.io/badge/ckan-2.9.7-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
 [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg?style=flat-square)](https://www.python.org/)
```

### Comparing `ckanext-ckanpackager-2.2.8/README.md` & `ckanext-ckanpackager-2.2.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <!--header-start-->
-<img src="https://github.com/NaturalHistoryMuseum/ckanext-ckanpackager/raw/main/.github/nhm-logo.svg" align="left" width="150px" height="100px" hspace="40"/>
+<img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-ckanpackager
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-ckanpackager/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-ckanpackager/actions/workflows/main.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/NaturalHistoryMuseum/ckanext-ckanpackager/main?style=flat-square)](https://coveralls.io/github/NaturalHistoryMuseum/ckanext-ckanpackager)
 [![CKAN](https://img.shields.io/badge/ckan-2.9.7-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
 [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg?style=flat-square)](https://www.python.org/)
```

### Comparing `ckanext-ckanpackager-2.2.8/ckanext/ckanpackager/cli.py` & `ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/cli.py`

 * *Files identical despite different names*

### Comparing `ckanext-ckanpackager-2.2.8/ckanext/ckanpackager/interfaces.py` & `ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/interfaces.py`

 * *Files identical despite different names*

### Comparing `ckanext-ckanpackager-2.2.8/ckanext/ckanpackager/lib/helpers.py` & `ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/lib/helpers.py`

 * *Files identical despite different names*

### Comparing `ckanext-ckanpackager-2.2.8/ckanext/ckanpackager/lib/utils.py` & `ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/lib/utils.py`

 * *Files identical despite different names*

### Comparing `ckanext-ckanpackager-2.2.8/ckanext/ckanpackager/logic/action.py` & `ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/logic/action.py`

 * *Files identical despite different names*

### Comparing `ckanext-ckanpackager-2.2.8/ckanext/ckanpackager/model/stat.py` & `ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/model/stat.py`

 * *Files identical despite different names*

### Comparing `ckanext-ckanpackager-2.2.8/ckanext/ckanpackager/plugin.py` & `ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-ckanpackager-2.2.8/ckanext/ckanpackager/routes/packager.py` & `ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/routes/packager.py`

 * *Files identical despite different names*

### Comparing `ckanext-ckanpackager-2.2.8/ckanext/ckanpackager/theme/assets/less/ckanpackager.less` & `ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/theme/assets/less/ckanpackager.less`

 * *Files identical despite different names*

### Comparing `ckanext-ckanpackager-2.2.8/ckanext/ckanpackager/theme/assets/scripts/modules/ckanpackager-download-link.js` & `ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/theme/assets/scripts/modules/ckanpackager-download-link.js`

 * *Files identical despite different names*

### Comparing `ckanext-ckanpackager-2.2.8/ckanext/ckanpackager/theme/templates/ajax_snippets/ckanpackager_form.html` & `ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/theme/templates/ajax_snippets/ckanpackager_form.html`

 * *Files identical despite different names*

### Comparing `ckanext-ckanpackager-2.2.8/ckanext/ckanpackager/theme/templates/ckanpackager/snippets/package_resource.html` & `ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/theme/templates/ckanpackager/snippets/package_resource.html`

 * *Files identical despite different names*

### Comparing `ckanext-ckanpackager-2.2.8/ckanext_ckanpackager.egg-info/PKG-INFO` & `ckanext-ckanpackager-2.2.9/ckanext_ckanpackager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-ckanpackager
-Version: 2.2.8
+Version: 2.2.9
 Summary: A CKAN extension that provides a user interface to download resources with ckanpackager.
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-ckanpackager
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-ckanpackager/blob/main/CHANGELOG.md
 Keywords: CKAN,data,ckanpackager
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 <!--header-start-->
-<img src="https://github.com/NaturalHistoryMuseum/ckanext-ckanpackager/raw/main/.github/nhm-logo.svg" align="left" width="150px" height="100px" hspace="40"/>
+<img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-ckanpackager
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-ckanpackager/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-ckanpackager/actions/workflows/main.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/NaturalHistoryMuseum/ckanext-ckanpackager/main?style=flat-square)](https://coveralls.io/github/NaturalHistoryMuseum/ckanext-ckanpackager)
 [![CKAN](https://img.shields.io/badge/ckan-2.9.7-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
 [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg?style=flat-square)](https://www.python.org/)
```

### Comparing `ckanext-ckanpackager-2.2.8/ckanext_ckanpackager.egg-info/SOURCES.txt` & `ckanext-ckanpackager-2.2.9/ckanext_ckanpackager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-ckanpackager-2.2.8/docs/_scripts/gen_api_pages.py` & `ckanext-ckanpackager-2.2.9/docs/_scripts/gen_api_pages.py`

 * *Files identical despite different names*

### Comparing `ckanext-ckanpackager-2.2.8/pyproject.toml` & `ckanext-ckanpackager-2.2.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ckanext-ckanpackager"
-version = "2.2.8"
+version = "2.2.9"
 description = "A CKAN extension that provides a user interface to download resources with ckanpackager."
 readme = "README.md"
 requires-python = ">=3.6"
 license = { text = "GPL-3.0-or-later" }
 authors = [
     { name = "Natural History Museum", email = "data@nhm.ac.uk" }
 ]
@@ -52,15 +52,15 @@
 exclude = ["tests", "docs"]
 
 [tool.setuptools.package-data]
 "ckanext.ckanpackager.theme" = ["*", "**/*"]
 
 [tool.commitizen]
 name = "cz_nhm"
-version = "2.2.8"
+version = "2.2.9"
 tag_format = "v$version"
 update_changelog_on_bump = true
 changelog_incremental = true
 version_files = [
     "pyproject.toml:version"
 ]
```

### Comparing `ckanext-ckanpackager-2.2.8/tests/test_helpers.py` & `ckanext-ckanpackager-2.2.9/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `ckanext-ckanpackager-2.2.8/tests/test_utils.py` & `ckanext-ckanpackager-2.2.9/tests/test_utils.py`

 * *Files identical despite different names*

