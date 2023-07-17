# Comparing `tmp/pydanticneo4j-0.1.0.tar.gz` & `tmp/pydanticneo4j-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydanticneo4j-0.1.0.tar", max compression
+gzip compressed data, was "pydanticneo4j-0.1.1.tar", max compression
```

## Comparing `pydanticneo4j-0.1.0.tar` & `pydanticneo4j-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      840 2023-07-17 19:18:37.364323 pydanticneo4j-0.1.0/PydanticNeo4j/__init__.py
--rw-r--r--   0        0        0     5756 2023-07-17 18:59:47.287301 pydanticneo4j-0.1.0/PydanticNeo4j/create_operations.py
--rw-r--r--   0        0        0     4468 2023-07-17 18:21:59.136803 pydanticneo4j-0.1.0/PydanticNeo4j/database_operations.py
--rw-r--r--   0        0        0     3131 2023-07-17 17:12:07.586416 pydanticneo4j-0.1.0/PydanticNeo4j/graph_base_models.py
--rw-r--r--   0        0        0    10473 2023-07-17 18:57:27.287819 pydanticneo4j-0.1.0/PydanticNeo4j/match_operations.py
--rw-r--r--   0        0        0     1268 2023-07-17 19:16:54.906537 pydanticneo4j-0.1.0/PydanticNeo4j/pydantic_neo4j.py
--rw-r--r--   0        0        0      639 2023-07-17 19:19:01.049777 pydanticneo4j-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      234 2023-07-17 19:16:54.901537 pydanticneo4j-0.1.0/README.md
--rw-r--r--   0        0        0     1031 1970-01-01 00:00:00.000000 pydanticneo4j-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      840 2023-07-17 19:18:37.364323 pydanticneo4j-0.1.1/PydanticNeo4j/__init__.py
+-rw-r--r--   0        0        0     5756 2023-07-17 18:59:47.287301 pydanticneo4j-0.1.1/PydanticNeo4j/create_operations.py
+-rw-r--r--   0        0        0     4468 2023-07-17 18:21:59.136803 pydanticneo4j-0.1.1/PydanticNeo4j/database_operations.py
+-rw-r--r--   0        0        0     3131 2023-07-17 17:12:07.586416 pydanticneo4j-0.1.1/PydanticNeo4j/graph_base_models.py
+-rw-r--r--   0        0        0    10473 2023-07-17 18:57:27.287819 pydanticneo4j-0.1.1/PydanticNeo4j/match_operations.py
+-rw-r--r--   0        0        0     1268 2023-07-17 19:16:54.906537 pydanticneo4j-0.1.1/PydanticNeo4j/pydantic_neo4j.py
+-rw-r--r--   0        0        0      639 2023-07-17 19:33:47.290872 pydanticneo4j-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      234 2023-07-17 19:16:54.901537 pydanticneo4j-0.1.1/README.md
+-rw-r--r--   0        0        0     1031 1970-01-01 00:00:00.000000 pydanticneo4j-0.1.1/PKG-INFO
```

### Comparing `pydanticneo4j-0.1.0/PydanticNeo4j/__init__.py` & `pydanticneo4j-0.1.1/PydanticNeo4j/__init__.py`

 * *Files identical despite different names*

### Comparing `pydanticneo4j-0.1.0/PydanticNeo4j/create_operations.py` & `pydanticneo4j-0.1.1/PydanticNeo4j/create_operations.py`

 * *Files identical despite different names*

### Comparing `pydanticneo4j-0.1.0/PydanticNeo4j/database_operations.py` & `pydanticneo4j-0.1.1/PydanticNeo4j/database_operations.py`

 * *Files identical despite different names*

### Comparing `pydanticneo4j-0.1.0/PydanticNeo4j/graph_base_models.py` & `pydanticneo4j-0.1.1/PydanticNeo4j/graph_base_models.py`

 * *Files identical despite different names*

### Comparing `pydanticneo4j-0.1.0/PydanticNeo4j/match_operations.py` & `pydanticneo4j-0.1.1/PydanticNeo4j/match_operations.py`

 * *Files identical despite different names*

### Comparing `pydanticneo4j-0.1.0/PydanticNeo4j/pydantic_neo4j.py` & `pydanticneo4j-0.1.1/PydanticNeo4j/pydantic_neo4j.py`

 * *Files identical despite different names*

### Comparing `pydanticneo4j-0.1.0/PKG-INFO` & `pydanticneo4j-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydanticneo4j
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Home-page: https://github.com/Michaelzag/PydanticNeo4j
 License: MIT
 Keywords: neo4j-pydantic,Pydantic,Neo4j,OGM,Neo4j-OG,MichaelZag
 Author: MichaelZag
 Author-email: Michael@MichaelZag.com
 Requires-Python: >=3.11,<4.0
```

