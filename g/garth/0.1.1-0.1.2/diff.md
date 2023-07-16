# Comparing `tmp/garth-0.1.1.tar.gz` & `tmp/garth-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garth-0.1.1.tar", last modified: Sun Jul 16 23:00:29 2023, max compression
+gzip compressed data, was "garth-0.1.2.tar", last modified: Sun Jul 16 23:03:12 2023, max compression
```

## Comparing `garth-0.1.1.tar` & `garth-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       25 2023-07-12 03:23:05.160417 garth-0.1.1/README.md
--rw-r--r--   0        0        0       55 2023-07-16 13:04:44.324498 garth-0.1.1/garth/__init__.py
--rw-r--r--   0        0        0      986 2023-07-16 18:57:12.229760 garth-0.1.1/garth/auth_token.py
--rw-r--r--   0        0        0     2219 2023-07-16 18:38:38.109518 garth-0.1.1/garth/http.py
--rw-r--r--   0        0        0     2716 2023-07-16 19:10:10.106829 garth-0.1.1/garth/sso.py
--rw-r--r--   0        0        0        0 2023-07-16 18:57:56.389343 garth-0.1.1/garth/version.py
--rw-r--r--   0        0        0      531 2023-07-16 23:00:29.760009 garth-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      282 1970-01-01 00:00:00.000000 garth-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       25 2023-07-12 03:23:05.160417 garth-0.1.2/README.md
+-rw-r--r--   0        0        0       55 2023-07-16 13:04:44.324498 garth-0.1.2/garth/__init__.py
+-rw-r--r--   0        0        0      986 2023-07-16 18:57:12.229760 garth-0.1.2/garth/auth_token.py
+-rw-r--r--   0        0        0     2219 2023-07-16 18:38:38.109518 garth-0.1.2/garth/http.py
+-rw-r--r--   0        0        0     2716 2023-07-16 19:10:10.106829 garth-0.1.2/garth/sso.py
+-rw-r--r--   0        0        0        0 2023-07-16 18:57:56.389343 garth-0.1.2/garth/version.py
+-rw-r--r--   0        0        0      531 2023-07-16 23:03:12.697787 garth-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      282 1970-01-01 00:00:00.000000 garth-0.1.2/PKG-INFO
```

### Comparing `garth-0.1.1/garth/auth_token.py` & `garth-0.1.2/garth/auth_token.py`

 * *Files identical despite different names*

### Comparing `garth-0.1.1/garth/http.py` & `garth-0.1.2/garth/http.py`

 * *Files identical despite different names*

### Comparing `garth-0.1.1/garth/sso.py` & `garth-0.1.2/garth/sso.py`

 * *Files identical despite different names*

### Comparing `garth-0.1.1/pyproject.toml` & `garth-0.1.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [project]
 name = "garth"
-version = "0.1.1"
+version = "0.1.2"
 description = "Garmin SSO auth"
 authors = [
     { name = "Matin Tamizi", email = "mtamizi@duck.com" },
 ]
 dependencies = [
     "fire>=0.5.0",
-    "requests>=2.31.0",
+    "requests>=2.27.0",
 ]
 requires-python = ">=3.10"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
```

