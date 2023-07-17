# Comparing `tmp/pydantic_neo4j-0.1.2.tar.gz` & `tmp/pydantic_neo4j-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_neo4j-0.1.2.tar", max compression
+gzip compressed data, was "pydantic_neo4j-0.1.3.tar", max compression
```

## Comparing `pydantic_neo4j-0.1.2.tar` & `pydantic_neo4j-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      709 2023-07-17 20:31:16.591559 pydantic_neo4j-0.1.2/pydantic-neo4j/__init__.py
--rw-r--r--   0        0        0     5756 2023-07-17 18:59:47.287301 pydantic_neo4j-0.1.2/pydantic-neo4j/create_operations.py
--rw-r--r--   0        0        0     4468 2023-07-17 18:21:59.136803 pydantic_neo4j-0.1.2/pydantic-neo4j/database_operations.py
--rw-r--r--   0        0        0     3131 2023-07-17 17:12:07.586416 pydantic_neo4j-0.1.2/pydantic-neo4j/graph_base_models.py
--rw-r--r--   0        0        0    10473 2023-07-17 18:57:27.287819 pydantic_neo4j-0.1.2/pydantic-neo4j/match_operations.py
--rw-r--r--   0        0        0     1268 2023-07-17 19:16:54.906537 pydantic_neo4j-0.1.2/pydantic-neo4j/pydantic_neo4j.py
--rw-r--r--   0        0        0      603 2023-07-17 20:31:33.834339 pydantic_neo4j-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      235 2023-07-17 20:27:32.715091 pydantic_neo4j-0.1.2/README.md
--rw-r--r--   0        0        0      841 1970-01-01 00:00:00.000000 pydantic_neo4j-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      709 2023-07-17 20:31:16.591559 pydantic_neo4j-0.1.3/pydantic_neo4j/__init__.py
+-rw-r--r--   0        0        0     5756 2023-07-17 18:59:47.287301 pydantic_neo4j-0.1.3/pydantic_neo4j/create_operations.py
+-rw-r--r--   0        0        0     4468 2023-07-17 18:21:59.136803 pydantic_neo4j-0.1.3/pydantic_neo4j/database_operations.py
+-rw-r--r--   0        0        0     3131 2023-07-17 17:12:07.586416 pydantic_neo4j-0.1.3/pydantic_neo4j/graph_base_models.py
+-rw-r--r--   0        0        0    10473 2023-07-17 18:57:27.287819 pydantic_neo4j-0.1.3/pydantic_neo4j/match_operations.py
+-rw-r--r--   0        0        0     1268 2023-07-17 19:16:54.906537 pydantic_neo4j-0.1.3/pydantic_neo4j/pydantic_neo4j.py
+-rw-r--r--   0        0        0      603 2023-07-17 20:40:52.792879 pydantic_neo4j-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      235 2023-07-17 20:39:48.826278 pydantic_neo4j-0.1.3/README.md
+-rw-r--r--   0        0        0      841 1970-01-01 00:00:00.000000 pydantic_neo4j-0.1.3/PKG-INFO
```

### Comparing `pydantic_neo4j-0.1.2/pydantic-neo4j/__init__.py` & `pydantic_neo4j-0.1.3/pydantic_neo4j/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic_neo4j-0.1.2/pydantic-neo4j/create_operations.py` & `pydantic_neo4j-0.1.3/pydantic_neo4j/create_operations.py`

 * *Files identical despite different names*

### Comparing `pydantic_neo4j-0.1.2/pydantic-neo4j/database_operations.py` & `pydantic_neo4j-0.1.3/pydantic_neo4j/database_operations.py`

 * *Files identical despite different names*

### Comparing `pydantic_neo4j-0.1.2/pydantic-neo4j/graph_base_models.py` & `pydantic_neo4j-0.1.3/pydantic_neo4j/graph_base_models.py`

 * *Files identical despite different names*

### Comparing `pydantic_neo4j-0.1.2/pydantic-neo4j/match_operations.py` & `pydantic_neo4j-0.1.3/pydantic_neo4j/match_operations.py`

 * *Files identical despite different names*

### Comparing `pydantic_neo4j-0.1.2/pydantic-neo4j/pydantic_neo4j.py` & `pydantic_neo4j-0.1.3/pydantic_neo4j/pydantic_neo4j.py`

 * *Files identical despite different names*

### Comparing `pydantic_neo4j-0.1.2/pyproject.toml` & `pydantic_neo4j-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "pydantic-neo4j"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["MichaelZag <Michael@MichaelZag.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = 'https://github.com/Michaelzag/PydanticNeo4j'
 repository = 'https://github.com/Michaelzag/PydanticNeo4j'
 keywords = ['neo4j-pydantic','Pydantic', 'Neo4j', 'OGM', 'Neo4j-OG','MichaelZag']
 packages = [
-    { include = "pydantic-neo4j" },
+    { include = "pydantic_neo4j" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 pydantic = "^2.0.3"
 neo4j = "^5.10.0"
```

### Comparing `pydantic_neo4j-0.1.2/PKG-INFO` & `pydantic_neo4j-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-neo4j
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Home-page: https://github.com/Michaelzag/PydanticNeo4j
 License: MIT
 Keywords: neo4j-pydantic,Pydantic,Neo4j,OGM,Neo4j-OG,MichaelZag
 Author: MichaelZag
 Author-email: Michael@MichaelZag.com
 Requires-Python: >=3.11,<4.0
@@ -20,15 +20,15 @@
 
 ### Purpose of the Package
 + To translate from Pydantic models to Neo4j Graphs
 
 ### Getting Started
 + Install the package
 ```bash
-pip install pydantic-neo4j
+pip install pydantic_neo4j
 ```
 
 ### Usage
 
 
 
 ### API
```

