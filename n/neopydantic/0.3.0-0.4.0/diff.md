# Comparing `tmp/neopydantic-0.3.0.tar.gz` & `tmp/neopydantic-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neopydantic-0.3.0.tar", max compression
+gzip compressed data, was "neopydantic-0.4.0.tar", max compression
```

## Comparing `neopydantic-0.3.0.tar` & `neopydantic-0.4.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      197 2023-07-17 16:23:12.835695 neopydantic-0.3.0/NeoPydantic/__init__.py
--rw-r--r--   0        0        0     5532 2023-07-17 15:59:26.931072 neopydantic-0.3.0/NeoPydantic/create_operations.py
--rw-r--r--   0        0        0     4415 2023-07-17 15:59:26.925044 neopydantic-0.3.0/NeoPydantic/database_operations.py
--rw-r--r--   0        0        0     3546 2023-07-17 16:00:22.376645 neopydantic-0.3.0/NeoPydantic/graph_base.py
--rw-r--r--   0        0        0    10198 2023-07-17 15:59:26.982247 neopydantic-0.3.0/NeoPydantic/match_operations.py
--rw-r--r--   0        0        0      616 2023-07-17 16:23:27.444374 neopydantic-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      168 2023-07-17 16:02:34.855180 neopydantic-0.3.0/README.md
--rw-r--r--   0        0        0      949 1970-01-01 00:00:00.000000 neopydantic-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      197 2023-07-17 16:23:12.835695 neopydantic-0.4.0/neopydantic/__init__.py
+-rw-r--r--   0        0        0     5532 2023-07-17 15:59:26.931072 neopydantic-0.4.0/neopydantic/create_operations.py
+-rw-r--r--   0        0        0     4415 2023-07-17 15:59:26.925044 neopydantic-0.4.0/neopydantic/database_operations.py
+-rw-r--r--   0        0        0     3546 2023-07-17 16:00:22.376645 neopydantic-0.4.0/neopydantic/graph_base.py
+-rw-r--r--   0        0        0    10198 2023-07-17 15:59:26.982247 neopydantic-0.4.0/neopydantic/match_operations.py
+-rw-r--r--   0        0        0      616 2023-07-17 16:26:54.672306 neopydantic-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      168 2023-07-17 16:02:34.855180 neopydantic-0.4.0/README.md
+-rw-r--r--   0        0        0      949 1970-01-01 00:00:00.000000 neopydantic-0.4.0/PKG-INFO
```

### Comparing `neopydantic-0.3.0/NeoPydantic/create_operations.py` & `neopydantic-0.4.0/neopydantic/create_operations.py`

 * *Files identical despite different names*

### Comparing `neopydantic-0.3.0/NeoPydantic/database_operations.py` & `neopydantic-0.4.0/neopydantic/database_operations.py`

 * *Files identical despite different names*

### Comparing `neopydantic-0.3.0/NeoPydantic/graph_base.py` & `neopydantic-0.4.0/neopydantic/graph_base.py`

 * *Files identical despite different names*

### Comparing `neopydantic-0.3.0/NeoPydantic/match_operations.py` & `neopydantic-0.4.0/neopydantic/match_operations.py`

 * *Files identical despite different names*

### Comparing `neopydantic-0.3.0/pyproject.toml` & `neopydantic-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neopydantic"
-version = "0.3.0"
+version = "0.4.0"
 description = ""
 authors = ["MichaelZag <Michael@MichaelZag.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = 'https://github.com/Michaelzag/NeoPydantic'
 repository = 'https://github.com/Michaelzag/NeoPydantic'
 keywords = ['Pydantic', 'Neo4j', 'OGM', 'Neo4j-OG','MichaelZag']
```

### Comparing `neopydantic-0.3.0/PKG-INFO` & `neopydantic-0.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neopydantic
-Version: 0.3.0
+Version: 0.4.0
 Summary: 
 Home-page: https://github.com/Michaelzag/NeoPydantic
 License: MIT
 Keywords: Pydantic,Neo4j,OGM,Neo4j-OG,MichaelZag
 Author: MichaelZag
 Author-email: Michael@MichaelZag.com
 Requires-Python: >=3.11,<4.0
```

