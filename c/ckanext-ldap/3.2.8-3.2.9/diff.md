# Comparing `tmp/ckanext-ldap-3.2.8.tar.gz` & `tmp/ckanext-ldap-3.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-ldap-3.2.8.tar", last modified: Mon Feb 20 10:56:57 2023, max compression
+gzip compressed data, was "ckanext-ldap-3.2.9.tar", last modified: Tue Apr 11 08:21:58 2023, max compression
```

## Comparing `ckanext-ldap-3.2.8.tar` & `ckanext-ldap-3.2.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:56:57.856084 ckanext-ldap-3.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-02-20 10:56:40.000000 ckanext-ldap-3.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24301 2023-02-20 10:56:57.856084 ckanext-ldap-3.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23412 2023-02-20 10:56:40.000000 ckanext-ldap-3.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:56:57.852084 ckanext-ldap-3.2.8/ckanext/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-02-20 10:56:40.000000 ckanext-ldap-3.2.8/ckanext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:56:57.852084 ckanext-ldap-3.2.8/ckanext/ldap/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-02-20 10:56:40.000000 ckanext-ldap-3.2.8/ckanext/ldap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-02-20 10:56:40.000000 ckanext-ldap-3.2.8/ckanext/ldap/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:56:57.852084 ckanext-ldap-3.2.8/ckanext/ldap/lib/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-02-20 10:56:40.000000 ckanext-ldap-3.2.8/ckanext/ldap/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-02-20 10:56:40.000000 ckanext-ldap-3.2.8/ckanext/ldap/lib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-02-20 10:56:40.000000 ckanext-ldap-3.2.8/ckanext/ldap/lib/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6199 2023-02-20 10:56:40.000000 ckanext-ldap-3.2.8/ckanext/ldap/lib/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-02-20 10:56:40.000000 ckanext-ldap-3.2.8/ckanext/ldap/lib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:56:57.852084 ckanext-ldap-3.2.8/ckanext/ldap/logic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 10:56:40.000000 ckanext-ldap-3.2.8/ckanext/ldap/logic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-02-20 10:56:40.000000 ckanext-ldap-3.2.8/ckanext/ldap/logic/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:56:57.852084 ckanext-ldap-3.2.8/ckanext/ldap/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 10:56:40.000000 ckanext-ldap-3.2.8/ckanext/ldap/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-02-20 10:56:40.000000 ckanext-ldap-3.2.8/ckanext/ldap/model/ldap_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-02-20 10:56:40.000000 ckanext-ldap-3.2.8/ckanext/ldap/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:56:57.852084 ckanext-ldap-3.2.8/ckanext/ldap/routes/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-02-20 10:56:40.000000 ckanext-ldap-3.2.8/ckanext/ldap/routes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-02-20 10:56:40.000000 ckanext-ldap-3.2.8/ckanext/ldap/routes/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-02-20 10:56:40.000000 ckanext-ldap-3.2.8/ckanext/ldap/routes/login.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:56:57.852084 ckanext-ldap-3.2.8/ckanext/ldap/theme/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:56:57.852084 ckanext-ldap-3.2.8/ckanext/ldap/theme/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:56:57.852084 ckanext-ldap-3.2.8/ckanext/ldap/theme/templates/user/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-02-20 10:56:40.000000 ckanext-ldap-3.2.8/ckanext/ldap/theme/templates/user/login.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:56:57.856084 ckanext-ldap-3.2.8/ckanext_ldap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24301 2023-02-20 10:56:57.000000 ckanext-ldap-3.2.8/ckanext_ldap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-02-20 10:56:57.000000 ckanext-ldap-3.2.8/ckanext_ldap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 10:56:57.000000 ckanext-ldap-3.2.8/ckanext_ldap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-02-20 10:56:57.000000 ckanext-ldap-3.2.8/ckanext_ldap.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 10:56:57.000000 ckanext-ldap-3.2.8/ckanext_ldap.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-02-20 10:56:57.000000 ckanext-ldap-3.2.8/ckanext_ldap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-20 10:56:57.000000 ckanext-ldap-3.2.8/ckanext_ldap.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:56:57.852084 ckanext-ldap-3.2.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:56:57.856084 ckanext-ldap-3.2.8/docs/_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-02-20 10:56:40.000000 ckanext-ldap-3.2.8/docs/_scripts/gen_api_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-02-20 10:56:40.000000 ckanext-ldap-3.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-20 10:56:57.856084 ckanext-ldap-3.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-02-20 10:56:40.000000 ckanext-ldap-3.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:56:57.856084 ckanext-ldap-3.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-02-20 10:56:40.000000 ckanext-ldap-3.2.8/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-02-20 10:56:40.000000 ckanext-ldap-3.2.8/tests/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:21:58.809777 ckanext-ldap-3.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-11 08:21:46.000000 ckanext-ldap-3.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24301 2023-04-11 08:21:58.809777 ckanext-ldap-3.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23412 2023-04-11 08:21:46.000000 ckanext-ldap-3.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:21:58.801777 ckanext-ldap-3.2.9/ckanext/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-11 08:21:46.000000 ckanext-ldap-3.2.9/ckanext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:21:58.801777 ckanext-ldap-3.2.9/ckanext/ldap/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-11 08:21:46.000000 ckanext-ldap-3.2.9/ckanext/ldap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-11 08:21:46.000000 ckanext-ldap-3.2.9/ckanext/ldap/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:21:58.805776 ckanext-ldap-3.2.9/ckanext/ldap/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-11 08:21:46.000000 ckanext-ldap-3.2.9/ckanext/ldap/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-11 08:21:46.000000 ckanext-ldap-3.2.9/ckanext/ldap/lib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-11 08:21:46.000000 ckanext-ldap-3.2.9/ckanext/ldap/lib/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6199 2023-04-11 08:21:46.000000 ckanext-ldap-3.2.9/ckanext/ldap/lib/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-11 08:21:46.000000 ckanext-ldap-3.2.9/ckanext/ldap/lib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:21:58.805776 ckanext-ldap-3.2.9/ckanext/ldap/logic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:21:46.000000 ckanext-ldap-3.2.9/ckanext/ldap/logic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-04-11 08:21:46.000000 ckanext-ldap-3.2.9/ckanext/ldap/logic/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:21:58.805776 ckanext-ldap-3.2.9/ckanext/ldap/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:21:46.000000 ckanext-ldap-3.2.9/ckanext/ldap/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-11 08:21:46.000000 ckanext-ldap-3.2.9/ckanext/ldap/model/ldap_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-04-11 08:21:46.000000 ckanext-ldap-3.2.9/ckanext/ldap/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:21:58.805776 ckanext-ldap-3.2.9/ckanext/ldap/routes/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-11 08:21:46.000000 ckanext-ldap-3.2.9/ckanext/ldap/routes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-04-11 08:21:46.000000 ckanext-ldap-3.2.9/ckanext/ldap/routes/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-04-11 08:21:46.000000 ckanext-ldap-3.2.9/ckanext/ldap/routes/login.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:21:58.797777 ckanext-ldap-3.2.9/ckanext/ldap/theme/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:21:58.797777 ckanext-ldap-3.2.9/ckanext/ldap/theme/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:21:58.805776 ckanext-ldap-3.2.9/ckanext/ldap/theme/templates/user/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-11 08:21:46.000000 ckanext-ldap-3.2.9/ckanext/ldap/theme/templates/user/login.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:21:58.809777 ckanext-ldap-3.2.9/ckanext_ldap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24301 2023-04-11 08:21:58.000000 ckanext-ldap-3.2.9/ckanext_ldap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-11 08:21:58.000000 ckanext-ldap-3.2.9/ckanext_ldap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:21:58.000000 ckanext-ldap-3.2.9/ckanext_ldap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-11 08:21:58.000000 ckanext-ldap-3.2.9/ckanext_ldap.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:21:58.000000 ckanext-ldap-3.2.9/ckanext_ldap.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-11 08:21:58.000000 ckanext-ldap-3.2.9/ckanext_ldap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-11 08:21:58.000000 ckanext-ldap-3.2.9/ckanext_ldap.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:21:58.801777 ckanext-ldap-3.2.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:21:58.809777 ckanext-ldap-3.2.9/docs/_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-11 08:21:46.000000 ckanext-ldap-3.2.9/docs/_scripts/gen_api_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-11 08:21:46.000000 ckanext-ldap-3.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 08:21:58.809777 ckanext-ldap-3.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-11 08:21:46.000000 ckanext-ldap-3.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:21:58.809777 ckanext-ldap-3.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-04-11 08:21:46.000000 ckanext-ldap-3.2.9/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-11 08:21:46.000000 ckanext-ldap-3.2.9/tests/test_helpers.py
```

### Comparing `ckanext-ldap-3.2.8/LICENSE` & `ckanext-ldap-3.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-ldap-3.2.8/PKG-INFO` & `ckanext-ldap-3.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-ldap
-Version: 3.2.8
+Version: 3.2.9
 Summary: A CKAN extension that provides LDAP authentication.
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-ldap
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-ldap/blob/main/CHANGELOG.md
 Keywords: CKAN,data,ldap
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ckanext-ldap-3.2.8/README.md` & `ckanext-ldap-3.2.9/README.md`

 * *Files identical despite different names*

### Comparing `ckanext-ldap-3.2.8/ckanext/ldap/cli.py` & `ckanext-ldap-3.2.9/ckanext/ldap/cli.py`

 * *Files identical despite different names*

### Comparing `ckanext-ldap-3.2.8/ckanext/ldap/lib/helpers.py` & `ckanext-ldap-3.2.9/ckanext/ldap/lib/helpers.py`

 * *Files identical despite different names*

### Comparing `ckanext-ldap-3.2.8/ckanext/ldap/lib/search.py` & `ckanext-ldap-3.2.9/ckanext/ldap/lib/search.py`

 * *Files identical despite different names*

### Comparing `ckanext-ldap-3.2.8/ckanext/ldap/logic/auth.py` & `ckanext-ldap-3.2.9/ckanext/ldap/logic/auth.py`

 * *Files identical despite different names*

### Comparing `ckanext-ldap-3.2.8/ckanext/ldap/model/ldap_user.py` & `ckanext-ldap-3.2.9/ckanext/ldap/model/ldap_user.py`

 * *Files identical despite different names*

### Comparing `ckanext-ldap-3.2.8/ckanext/ldap/plugin.py` & `ckanext-ldap-3.2.9/ckanext/ldap/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-ldap-3.2.8/ckanext/ldap/routes/_helpers.py` & `ckanext-ldap-3.2.9/ckanext/ldap/routes/_helpers.py`

 * *Files identical despite different names*

### Comparing `ckanext-ldap-3.2.8/ckanext/ldap/routes/login.py` & `ckanext-ldap-3.2.9/ckanext/ldap/routes/login.py`

 * *Files identical despite different names*

### Comparing `ckanext-ldap-3.2.8/ckanext_ldap.egg-info/PKG-INFO` & `ckanext-ldap-3.2.9/ckanext_ldap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-ldap
-Version: 3.2.8
+Version: 3.2.9
 Summary: A CKAN extension that provides LDAP authentication.
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-ldap
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-ldap/blob/main/CHANGELOG.md
 Keywords: CKAN,data,ldap
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ckanext-ldap-3.2.8/ckanext_ldap.egg-info/SOURCES.txt` & `ckanext-ldap-3.2.9/ckanext_ldap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-ldap-3.2.8/docs/_scripts/gen_api_pages.py` & `ckanext-ldap-3.2.9/docs/_scripts/gen_api_pages.py`

 * *Files identical despite different names*

### Comparing `ckanext-ldap-3.2.8/pyproject.toml` & `ckanext-ldap-3.2.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ckanext-ldap"
-version = "3.2.8"
+version = "3.2.9"
 description = "A CKAN extension that provides LDAP authentication."
 readme = "README.md"
 requires-python = ">=3.6"
 license = { text = "GPL-3.0-or-later" }
 authors = [
     { name = "Natural History Museum", email = "data@nhm.ac.uk" }
 ]
@@ -52,15 +52,15 @@
 exclude = ["tests", "docs"]
 
 [tool.setuptools.package-data]
 "ckanext.ldap.theme" = ["*", "**/*"]
 
 [tool.commitizen]
 name = "cz_nhm"
-version = "3.2.8"
+version = "3.2.9"
 tag_format = "v$version"
 update_changelog_on_bump = true
 changelog_incremental = true
 version_files = [
     "pyproject.toml:version"
 ]
```

### Comparing `ckanext-ldap-3.2.8/tests/test_auth.py` & `ckanext-ldap-3.2.9/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `ckanext-ldap-3.2.8/tests/test_helpers.py` & `ckanext-ldap-3.2.9/tests/test_helpers.py`

 * *Files identical despite different names*

