# Comparing `tmp/neopydantic-0.4.6.tar.gz` & `tmp/neopydantic-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neopydantic-0.4.6.tar", max compression
+gzip compressed data, was "neopydantic-0.4.7.tar", max compression
```

## Comparing `neopydantic-0.4.6.tar` & `neopydantic-0.4.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      700 2023-07-17 17:19:52.989723 neopydantic-0.4.6/neopydantic/__init__.py
--rw-r--r--   0        0        0     5611 2023-07-17 17:17:06.673995 neopydantic-0.4.6/neopydantic/create_operations.py
--rw-r--r--   0        0        0     4426 2023-07-17 17:12:07.597420 neopydantic-0.4.6/neopydantic/database_operations.py
--rw-r--r--   0        0        0     3131 2023-07-17 17:12:07.586416 neopydantic-0.4.6/neopydantic/graph_base_models.py
--rw-r--r--   0        0        0    10212 2023-07-17 17:17:06.663011 neopydantic-0.4.6/neopydantic/match_operations.py
--rw-r--r--   0        0        0      475 2023-07-17 17:12:07.582417 neopydantic-0.4.6/neopydantic/neopydantic.py
--rw-r--r--   0        0        0        0 2023-07-17 17:01:26.874471 neopydantic-0.4.6/neopydantic/operations/__init__.py
--rw-r--r--   0        0        0      616 2023-07-17 17:19:58.192628 neopydantic-0.4.6/pyproject.toml
--rw-r--r--   0        0        0      168 2023-07-17 16:02:34.855180 neopydantic-0.4.6/README.md
--rw-r--r--   0        0        0      949 1970-01-01 00:00:00.000000 neopydantic-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0      700 2023-07-17 17:19:52.989723 neopydantic-0.4.7/neopydantic/__init__.py
+-rw-r--r--   0        0        0     5611 2023-07-17 17:17:06.673995 neopydantic-0.4.7/neopydantic/create_operations.py
+-rw-r--r--   0        0        0     4426 2023-07-17 17:12:07.597420 neopydantic-0.4.7/neopydantic/database_operations.py
+-rw-r--r--   0        0        0     3131 2023-07-17 17:12:07.586416 neopydantic-0.4.7/neopydantic/graph_base_models.py
+-rw-r--r--   0        0        0    10212 2023-07-17 17:17:06.663011 neopydantic-0.4.7/neopydantic/match_operations.py
+-rw-r--r--   0        0        0      934 2023-07-17 17:26:56.428710 neopydantic-0.4.7/neopydantic/neopydantic.py
+-rw-r--r--   0        0        0        0 2023-07-17 17:01:26.874471 neopydantic-0.4.7/neopydantic/operations/__init__.py
+-rw-r--r--   0        0        0      616 2023-07-17 17:26:56.432711 neopydantic-0.4.7/pyproject.toml
+-rw-r--r--   0        0        0      168 2023-07-17 16:02:34.855180 neopydantic-0.4.7/README.md
+-rw-r--r--   0        0        0      949 1970-01-01 00:00:00.000000 neopydantic-0.4.7/PKG-INFO
```

### Comparing `neopydantic-0.4.6/neopydantic/__init__.py` & `neopydantic-0.4.7/neopydantic/__init__.py`

 * *Files identical despite different names*

### Comparing `neopydantic-0.4.6/neopydantic/create_operations.py` & `neopydantic-0.4.7/neopydantic/create_operations.py`

 * *Files identical despite different names*

### Comparing `neopydantic-0.4.6/neopydantic/database_operations.py` & `neopydantic-0.4.7/neopydantic/database_operations.py`

 * *Files identical despite different names*

### Comparing `neopydantic-0.4.6/neopydantic/graph_base_models.py` & `neopydantic-0.4.7/neopydantic/graph_base_models.py`

 * *Files identical despite different names*

### Comparing `neopydantic-0.4.6/neopydantic/match_operations.py` & `neopydantic-0.4.7/neopydantic/match_operations.py`

 * *Files identical despite different names*

### Comparing `neopydantic-0.4.6/pyproject.toml` & `neopydantic-0.4.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neopydantic"
-version = "0.4.6"
+version = "0.4.7"
 description = ""
 authors = ["MichaelZag <Michael@MichaelZag.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = 'https://github.com/Michaelzag/NeoPydantic'
 repository = 'https://github.com/Michaelzag/NeoPydantic'
 keywords = ['Pydantic', 'Neo4j', 'OGM', 'Neo4j-OG','MichaelZag']
```

### Comparing `neopydantic-0.4.6/PKG-INFO` & `neopydantic-0.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neopydantic
-Version: 0.4.6
+Version: 0.4.7
 Summary: 
 Home-page: https://github.com/Michaelzag/NeoPydantic
 License: MIT
 Keywords: Pydantic,Neo4j,OGM,Neo4j-OG,MichaelZag
 Author: MichaelZag
 Author-email: Michael@MichaelZag.com
 Requires-Python: >=3.11,<4.0
```

