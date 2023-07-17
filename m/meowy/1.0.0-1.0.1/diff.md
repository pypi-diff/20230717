# Comparing `tmp/meowy-1.0.0.tar.gz` & `tmp/meowy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meowy-1.0.0.tar", max compression
+gzip compressed data, was "meowy-1.0.1.tar", max compression
```

## Comparing `meowy-1.0.0.tar` & `meowy-1.0.1.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1086 2023-07-06 14:01:55.999316 meowy-1.0.0/LICENSE
--rw-r--r--   0        0        0      915 2023-07-07 11:46:58.141795 meowy-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      591 2023-07-07 11:48:00.611883 meowy-1.0.0/README.md
--rw-r--r--   0        0        0      183 2023-07-07 11:38:07.532835 meowy-1.0.0/src/meowy/__init__.py
--rw-r--r--   0        0        0      282 2023-07-07 11:24:39.525943 meowy-1.0.0/src/meowy/client.py
--rw-r--r--   0        0        0        6 2023-07-07 11:38:59.081588 meowy-1.0.0/src/meowy/manager/__init__.py
--rw-r--r--   0        0        0      444 2023-07-07 11:37:54.357618 meowy-1.0.0/src/meowy/manager/image.py
--rw-r--r--   0        0        0        6 2023-07-07 11:24:36.052355 meowy-1.0.0/src/meowy/struct/__init__.py
--rw-r--r--   0        0        0      114 2023-07-07 11:37:47.971287 meowy-1.0.0/src/meowy/struct/image.py
--rw-r--r--   0        0        0     1447 1970-01-01 00:00:00.000000 meowy-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-07-06 14:01:55.999316 meowy-1.0.1/LICENSE
+-rw-r--r--   0        0        0      915 2023-07-17 14:23:34.241189 meowy-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      591 2023-07-07 11:49:40.327444 meowy-1.0.1/README.md
+-rw-r--r--   0        0        0      183 2023-07-07 11:38:07.532835 meowy-1.0.1/src/meowy/__init__.py
+-rw-r--r--   0        0        0      282 2023-07-07 11:24:39.525943 meowy-1.0.1/src/meowy/client.py
+-rw-r--r--   0        0        0        6 2023-07-07 11:38:59.081588 meowy-1.0.1/src/meowy/manager/__init__.py
+-rw-r--r--   0        0        0      444 2023-07-07 11:37:54.357618 meowy-1.0.1/src/meowy/manager/image.py
+-rw-r--r--   0        0        0        0 2023-07-17 14:23:18.423442 meowy-1.0.1/src/meowy/py.typed
+-rw-r--r--   0        0        0        6 2023-07-07 11:24:36.052355 meowy-1.0.1/src/meowy/struct/__init__.py
+-rw-r--r--   0        0        0      114 2023-07-07 11:37:47.971287 meowy-1.0.1/src/meowy/struct/image.py
+-rw-r--r--   0        0        0     1447 1970-01-01 00:00:00.000000 meowy-1.0.1/PKG-INFO
```

### Comparing `meowy-1.0.0/LICENSE` & `meowy-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `meowy-1.0.0/pyproject.toml` & `meowy-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "meowy"
-version = "1.0.0"
+version = "1.0.1"
 description = "🐱 An unofficial The Cat API wrapper for Python"
 license = "MIT"
 authors = ["elaresai <elaresai@gmail.com>"]
 maintainers = ["elaresai <elaresai@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/elaresai/meowy"
 repository = "https://github.com/elaresai/meowy"
 classifiers = [
     "License :: OSI Approved :: MIT License",
 
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.8",
 
     "Topic :: Software Development :: Libraries",
 ]
 packages = [{ include = "meowy", from = "src" }]
 
 [tool.poetry.dependencies]
 python = ">=3.8.0,<3.12"
```

### Comparing `meowy-1.0.0/README.md` & `meowy-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `meowy-1.0.0/PKG-INFO` & `meowy-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meowy
-Version: 1.0.0
+Version: 1.0.1
 Summary: 🐱 An unofficial The Cat API wrapper for Python
 Home-page: https://github.com/elaresai/meowy
 License: MIT
 Author: elaresai
 Author-email: elaresai@gmail.com
 Maintainer: elaresai
 Maintainer-email: elaresai@gmail.com
```

