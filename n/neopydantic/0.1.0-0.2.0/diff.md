# Comparing `tmp/neopydantic-0.1.0.tar.gz` & `tmp/neopydantic-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neopydantic-0.1.0.tar", max compression
+gzip compressed data, was "neopydantic-0.2.0.tar", max compression
```

## Comparing `neopydantic-0.1.0.tar` & `neopydantic-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      126 2023-07-17 15:50:05.245406 neopydantic-0.1.0/NeoPydantic/__init__.py
--rw-r--r--   0        0        0     5532 2023-07-17 15:59:26.931072 neopydantic-0.1.0/NeoPydantic/create_operations.py
--rw-r--r--   0        0        0     4415 2023-07-17 15:59:26.925044 neopydantic-0.1.0/NeoPydantic/database_operations.py
--rw-r--r--   0        0        0     3546 2023-07-17 16:00:22.376645 neopydantic-0.1.0/NeoPydantic/graph_base.py
--rw-r--r--   0        0        0    10198 2023-07-17 15:59:26.982247 neopydantic-0.1.0/NeoPydantic/match_operations.py
--rw-r--r--   0        0        0      617 2023-07-17 16:06:46.734590 neopydantic-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      168 2023-07-17 16:02:34.855180 neopydantic-0.1.0/README.md
--rw-r--r--   0        0        0      950 1970-01-01 00:00:00.000000 neopydantic-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      126 2023-07-17 15:50:05.245406 neopydantic-0.2.0/NeoPydantic/__init__.py
+-rw-r--r--   0        0        0     5532 2023-07-17 15:59:26.931072 neopydantic-0.2.0/NeoPydantic/create_operations.py
+-rw-r--r--   0        0        0     4415 2023-07-17 15:59:26.925044 neopydantic-0.2.0/NeoPydantic/database_operations.py
+-rw-r--r--   0        0        0     3546 2023-07-17 16:00:22.376645 neopydantic-0.2.0/NeoPydantic/graph_base.py
+-rw-r--r--   0        0        0    10198 2023-07-17 15:59:26.982247 neopydantic-0.2.0/NeoPydantic/match_operations.py
+-rw-r--r--   0        0        0      616 2023-07-17 16:16:25.482283 neopydantic-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      168 2023-07-17 16:02:34.855180 neopydantic-0.2.0/README.md
+-rw-r--r--   0        0        0      949 1970-01-01 00:00:00.000000 neopydantic-0.2.0/PKG-INFO
```

### Comparing `neopydantic-0.1.0/NeoPydantic/create_operations.py` & `neopydantic-0.2.0/NeoPydantic/create_operations.py`

 * *Files identical despite different names*

### Comparing `neopydantic-0.1.0/NeoPydantic/database_operations.py` & `neopydantic-0.2.0/NeoPydantic/database_operations.py`

 * *Files identical despite different names*

### Comparing `neopydantic-0.1.0/NeoPydantic/graph_base.py` & `neopydantic-0.2.0/NeoPydantic/graph_base.py`

 * *Files identical despite different names*

### Comparing `neopydantic-0.1.0/NeoPydantic/match_operations.py` & `neopydantic-0.2.0/NeoPydantic/match_operations.py`

 * *Files identical despite different names*

### Comparing `neopydantic-0.1.0/pyproject.toml` & `neopydantic-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "neopydantic"
-version = "0.1.0"
+version = "0.2.0"
 description = ""
 authors = ["MichaelZag <Michael@MichaelZag.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = 'https://github.com/Michaelzag/NeoPydantic'
 repository = 'https://github.com/Michaelzag/NeoPydantic'
-keywords = ['Pyudantic', 'Neo4j', 'OGM', 'Neo4j-OG','MichaelZag']
+keywords = ['Pydantic', 'Neo4j', 'OGM', 'Neo4j-OG','MichaelZag']
 
 [tool.poetry.dependencies]
 python = "^3.11"
 pydantic = "^2.0.3"
 neo4j = "^5.10.0"
 black = "^23.7.0"
 bandit = "^1.7.5"
```

### Comparing `neopydantic-0.1.0/PKG-INFO` & `neopydantic-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: neopydantic
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 Home-page: https://github.com/Michaelzag/NeoPydantic
 License: MIT
-Keywords: Pyudantic,Neo4j,OGM,Neo4j-OG,MichaelZag
+Keywords: Pydantic,Neo4j,OGM,Neo4j-OG,MichaelZag
 Author: MichaelZag
 Author-email: Michael@MichaelZag.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bandit (>=1.7.5,<2.0.0)
```

