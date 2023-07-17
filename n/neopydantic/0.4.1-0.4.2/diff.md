# Comparing `tmp/neopydantic-0.4.1.tar.gz` & `tmp/neopydantic-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neopydantic-0.4.1.tar", max compression
+gzip compressed data, was "neopydantic-0.4.2.tar", max compression
```

## Comparing `neopydantic-0.4.1.tar` & `neopydantic-0.4.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      199 2023-07-17 16:33:02.003737 neopydantic-0.4.1/neopydantic/__init__.py
--rw-r--r--   0        0        0     5535 2023-07-17 16:33:01.998735 neopydantic-0.4.1/neopydantic/CreateOperations.py
--rw-r--r--   0        0        0     4420 2023-07-17 16:33:02.007737 neopydantic-0.4.1/neopydantic/DatabaseOperations.py
--rw-r--r--   0        0        0     3546 2023-07-17 16:00:22.376645 neopydantic-0.4.1/neopydantic/GraphBaseModels.py
--rw-r--r--   0        0        0    10198 2023-07-17 15:59:26.982247 neopydantic-0.4.1/neopydantic/MatchOperations.py
--rw-r--r--   0        0        0      616 2023-07-17 16:33:10.380308 neopydantic-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      168 2023-07-17 16:02:34.855180 neopydantic-0.4.1/README.md
--rw-r--r--   0        0        0      949 1970-01-01 00:00:00.000000 neopydantic-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      296 2023-07-17 16:41:00.464297 neopydantic-0.4.2/neopydantic/__init__.py
+-rw-r--r--   0        0        0     5535 2023-07-17 16:33:01.998735 neopydantic-0.4.2/neopydantic/CreateOperations.py
+-rw-r--r--   0        0        0     4420 2023-07-17 16:33:02.007737 neopydantic-0.4.2/neopydantic/DatabaseOperations.py
+-rw-r--r--   0        0        0     3546 2023-07-17 16:00:22.376645 neopydantic-0.4.2/neopydantic/GraphBaseModels.py
+-rw-r--r--   0        0        0    10198 2023-07-17 15:59:26.982247 neopydantic-0.4.2/neopydantic/MatchOperations.py
+-rw-r--r--   0        0        0      616 2023-07-17 16:41:18.300604 neopydantic-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      168 2023-07-17 16:02:34.855180 neopydantic-0.4.2/README.md
+-rw-r--r--   0        0        0      949 1970-01-01 00:00:00.000000 neopydantic-0.4.2/PKG-INFO
```

### Comparing `neopydantic-0.4.1/neopydantic/CreateOperations.py` & `neopydantic-0.4.2/neopydantic/CreateOperations.py`

 * *Files identical despite different names*

### Comparing `neopydantic-0.4.1/neopydantic/DatabaseOperations.py` & `neopydantic-0.4.2/neopydantic/DatabaseOperations.py`

 * *Files identical despite different names*

### Comparing `neopydantic-0.4.1/neopydantic/GraphBaseModels.py` & `neopydantic-0.4.2/neopydantic/GraphBaseModels.py`

 * *Files identical despite different names*

### Comparing `neopydantic-0.4.1/neopydantic/MatchOperations.py` & `neopydantic-0.4.2/neopydantic/MatchOperations.py`

 * *Files identical despite different names*

### Comparing `neopydantic-0.4.1/pyproject.toml` & `neopydantic-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neopydantic"
-version = "0.4.1"
+version = "0.4.2"
 description = ""
 authors = ["MichaelZag <Michael@MichaelZag.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = 'https://github.com/Michaelzag/NeoPydantic'
 repository = 'https://github.com/Michaelzag/NeoPydantic'
 keywords = ['Pydantic', 'Neo4j', 'OGM', 'Neo4j-OG','MichaelZag']
```

### Comparing `neopydantic-0.4.1/PKG-INFO` & `neopydantic-0.4.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neopydantic
-Version: 0.4.1
+Version: 0.4.2
 Summary: 
 Home-page: https://github.com/Michaelzag/NeoPydantic
 License: MIT
 Keywords: Pydantic,Neo4j,OGM,Neo4j-OG,MichaelZag
 Author: MichaelZag
 Author-email: Michael@MichaelZag.com
 Requires-Python: >=3.11,<4.0
```

