# Comparing `tmp/woofy-1.0.0.tar.gz` & `tmp/woofy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "woofy-1.0.0.tar", max compression
+gzip compressed data, was "woofy-1.0.1.tar", max compression
```

## Comparing `woofy-1.0.0.tar` & `woofy-1.0.1.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1086 2023-07-07 11:50:47.481091 woofy-1.0.0/LICENSE
--rw-r--r--   0        0        0      917 2023-07-07 12:01:05.326692 woofy-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      592 2023-07-07 12:00:49.712214 woofy-1.0.0/README.md
--rw-r--r--   0        0        0      183 2023-07-07 11:58:14.218216 woofy-1.0.0/src/woofy/__init__.py
--rw-r--r--   0        0        0      282 2023-07-07 11:56:55.865237 woofy-1.0.0/src/woofy/client.py
--rw-r--r--   0        0        0        6 2023-07-07 11:57:23.681233 woofy-1.0.0/src/woofy/manager/__init__.py
--rw-r--r--   0        0        0      444 2023-07-07 11:57:44.372577 woofy-1.0.0/src/woofy/manager/image.py
--rw-r--r--   0        0        0        6 2023-07-07 11:57:21.004450 woofy-1.0.0/src/woofy/struct/__init__.py
--rw-r--r--   0        0        0      114 2023-07-07 11:57:57.114858 woofy-1.0.0/src/woofy/struct/image.py
--rw-r--r--   0        0        0     1446 1970-01-01 00:00:00.000000 woofy-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-07-07 11:50:47.481091 woofy-1.0.1/LICENSE
+-rw-r--r--   0        0        0      917 2023-07-17 14:26:16.439909 woofy-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      592 2023-07-07 12:00:49.712214 woofy-1.0.1/README.md
+-rw-r--r--   0        0        0      183 2023-07-07 11:58:14.218216 woofy-1.0.1/src/woofy/__init__.py
+-rw-r--r--   0        0        0      282 2023-07-07 11:56:55.865237 woofy-1.0.1/src/woofy/client.py
+-rw-r--r--   0        0        0        6 2023-07-07 11:57:23.681233 woofy-1.0.1/src/woofy/manager/__init__.py
+-rw-r--r--   0        0        0      444 2023-07-07 11:57:44.372577 woofy-1.0.1/src/woofy/manager/image.py
+-rw-r--r--   0        0        0        0 2023-07-17 14:26:00.513817 woofy-1.0.1/src/woofy/py.typed
+-rw-r--r--   0        0        0        6 2023-07-07 11:57:21.004450 woofy-1.0.1/src/woofy/struct/__init__.py
+-rw-r--r--   0        0        0      114 2023-07-07 11:57:57.114858 woofy-1.0.1/src/woofy/struct/image.py
+-rw-r--r--   0        0        0     1446 1970-01-01 00:00:00.000000 woofy-1.0.1/PKG-INFO
```

### Comparing `woofy-1.0.0/LICENSE` & `woofy-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `woofy-1.0.0/pyproject.toml` & `woofy-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "woofy"
-version = "1.0.0"
+version = "1.0.1"
 description = "🐶 An unofficial The Dog API wrapper for Python"
 license = "MIT"
 authors = ["elaresai <elaresai@gmail.com>"]
 maintainers = ["elaresai <elaresai@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/elaresai/woofy"
 repository = "https://github.com/elaresai/woofy"
 classifiers = [
     "License :: OSI Approved :: MIT License",
 
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.8",
 
     "Topic :: Software Development :: Libraries",
 ]
 packages = [{ include = "woofy", from = "src" }]
 
 
 [tool.poetry.dependencies]
```

### Comparing `woofy-1.0.0/README.md` & `woofy-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `woofy-1.0.0/PKG-INFO` & `woofy-1.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: woofy
-Version: 1.0.0
+Version: 1.0.1
 Summary: 🐶 An unofficial The Dog API wrapper for Python
 Home-page: https://github.com/elaresai/woofy
 License: MIT
 Author: elaresai
 Author-email: elaresai@gmail.com
 Maintainer: elaresai
 Maintainer-email: elaresai@gmail.com
```

