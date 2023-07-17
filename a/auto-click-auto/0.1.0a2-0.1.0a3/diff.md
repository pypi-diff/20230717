# Comparing `tmp/auto_click_auto-0.1.0a2.tar.gz` & `tmp/auto_click_auto-0.1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_click_auto-0.1.0a2.tar", max compression
+gzip compressed data, was "auto_click_auto-0.1.0a3.tar", max compression
```

## Comparing `auto_click_auto-0.1.0a2.tar` & `auto_click_auto-0.1.0a3.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1082 2023-07-17 19:49:12.934242 auto_click_auto-0.1.0a2/LICENSE
--rw-r--r--   0        0        0     5252 2023-07-17 19:49:12.934242 auto_click_auto-0.1.0a2/README.md
--rw-r--r--   0        0        0       99 2023-07-17 19:49:12.934242 auto_click_auto-0.1.0a2/auto_click_auto/__init__.py
--rw-r--r--   0        0        0      532 2023-07-17 19:49:12.934242 auto_click_auto-0.1.0a2/auto_click_auto/constants.py
--rw-r--r--   0        0        0     5271 2023-07-17 19:49:12.934242 auto_click_auto-0.1.0a2/auto_click_auto/core.py
--rw-r--r--   0        0        0      460 2023-07-17 19:49:12.934242 auto_click_auto-0.1.0a2/auto_click_auto/exceptions.py
--rw-r--r--   0        0        0     2823 2023-07-17 19:49:12.934242 auto_click_auto-0.1.0a2/auto_click_auto/utils.py
--rw-r--r--   0        0        0     1476 2023-07-17 19:49:12.934242 auto_click_auto-0.1.0a2/pyproject.toml
--rw-r--r--   0        0        0     6553 1970-01-01 00:00:00.000000 auto_click_auto-0.1.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-07-17 20:18:43.651763 auto_click_auto-0.1.0a3/LICENSE
+-rw-r--r--   0        0        0     5252 2023-07-17 20:18:43.651763 auto_click_auto-0.1.0a3/README.md
+-rw-r--r--   0        0        0       99 2023-07-17 20:18:43.651763 auto_click_auto-0.1.0a3/auto_click_auto/__init__.py
+-rw-r--r--   0        0        0      532 2023-07-17 20:18:43.651763 auto_click_auto-0.1.0a3/auto_click_auto/constants.py
+-rw-r--r--   0        0        0     5271 2023-07-17 20:18:43.651763 auto_click_auto-0.1.0a3/auto_click_auto/core.py
+-rw-r--r--   0        0        0      460 2023-07-17 20:18:43.651763 auto_click_auto-0.1.0a3/auto_click_auto/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-17 20:18:43.651763 auto_click_auto-0.1.0a3/auto_click_auto/py.typed
+-rw-r--r--   0        0        0     2823 2023-07-17 20:18:43.651763 auto_click_auto-0.1.0a3/auto_click_auto/utils.py
+-rw-r--r--   0        0        0     1476 2023-07-17 20:18:43.651763 auto_click_auto-0.1.0a3/pyproject.toml
+-rw-r--r--   0        0        0     6553 1970-01-01 00:00:00.000000 auto_click_auto-0.1.0a3/PKG-INFO
```

### Comparing `auto_click_auto-0.1.0a2/LICENSE` & `auto_click_auto-0.1.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `auto_click_auto-0.1.0a2/README.md` & `auto_click_auto-0.1.0a3/README.md`

 * *Files identical despite different names*

### Comparing `auto_click_auto-0.1.0a2/auto_click_auto/constants.py` & `auto_click_auto-0.1.0a3/auto_click_auto/constants.py`

 * *Files identical despite different names*

### Comparing `auto_click_auto-0.1.0a2/auto_click_auto/core.py` & `auto_click_auto-0.1.0a3/auto_click_auto/core.py`

 * *Files identical despite different names*

### Comparing `auto_click_auto-0.1.0a2/auto_click_auto/utils.py` & `auto_click_auto-0.1.0a3/auto_click_auto/utils.py`

 * *Files identical despite different names*

### Comparing `auto_click_auto-0.1.0a2/pyproject.toml` & `auto_click_auto-0.1.0a3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "auto-click-auto"
-version = "0.1.0-alpha.2"
+version = "0.1.0-alpha.3"
 description = "Automatically enable tab autocompletion for shells in Click CLI applications."
 authors = ["Konstantinos Papadopoulos <konpap1996@yahoo.com>"]
 maintainers = ["Konstantinos Papadopoulos <konpap1996@yahoo.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/KAUTH/auto-click-auto"
 repository = "https://github.com/KAUTH/auto-click-auto"
```

### Comparing `auto_click_auto-0.1.0a2/PKG-INFO` & `auto_click_auto-0.1.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-click-auto
-Version: 0.1.0a2
+Version: 0.1.0a3
 Summary: Automatically enable tab autocompletion for shells in Click CLI applications.
 Home-page: https://github.com/KAUTH/auto-click-auto
 License: MIT
 Keywords: click,autocomplete,shell
 Author: Konstantinos Papadopoulos
 Author-email: konpap1996@yahoo.com
 Maintainer: Konstantinos Papadopoulos
```

