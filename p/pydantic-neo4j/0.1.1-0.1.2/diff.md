# Comparing `tmp/pydantic_neo4j-0.1.1.tar.gz` & `tmp/pydantic_neo4j-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_neo4j-0.1.1.tar", max compression
+gzip compressed data, was "pydantic_neo4j-0.1.2.tar", max compression
```

## Comparing `pydantic_neo4j-0.1.1.tar` & `pydantic_neo4j-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      840 2023-07-17 19:18:37.364323 pydantic_neo4j-0.1.1/pydantic-neo4j/__init__.py
--rw-r--r--   0        0        0     5756 2023-07-17 18:59:47.287301 pydantic_neo4j-0.1.1/pydantic-neo4j/create_operations.py
--rw-r--r--   0        0        0     4468 2023-07-17 18:21:59.136803 pydantic_neo4j-0.1.1/pydantic-neo4j/database_operations.py
--rw-r--r--   0        0        0     3131 2023-07-17 17:12:07.586416 pydantic_neo4j-0.1.1/pydantic-neo4j/graph_base_models.py
--rw-r--r--   0        0        0    10473 2023-07-17 18:57:27.287819 pydantic_neo4j-0.1.1/pydantic-neo4j/match_operations.py
--rw-r--r--   0        0        0     1268 2023-07-17 19:16:54.906537 pydantic_neo4j-0.1.1/pydantic-neo4j/pydantic_neo4j.py
--rw-r--r--   0        0        0      603 2023-07-17 20:19:57.691754 pydantic_neo4j-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      234 2023-07-17 19:16:54.901537 pydantic_neo4j-0.1.1/README.md
--rw-r--r--   0        0        0      840 1970-01-01 00:00:00.000000 pydantic_neo4j-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      709 2023-07-17 20:31:16.591559 pydantic_neo4j-0.1.2/pydantic-neo4j/__init__.py
+-rw-r--r--   0        0        0     5756 2023-07-17 18:59:47.287301 pydantic_neo4j-0.1.2/pydantic-neo4j/create_operations.py
+-rw-r--r--   0        0        0     4468 2023-07-17 18:21:59.136803 pydantic_neo4j-0.1.2/pydantic-neo4j/database_operations.py
+-rw-r--r--   0        0        0     3131 2023-07-17 17:12:07.586416 pydantic_neo4j-0.1.2/pydantic-neo4j/graph_base_models.py
+-rw-r--r--   0        0        0    10473 2023-07-17 18:57:27.287819 pydantic_neo4j-0.1.2/pydantic-neo4j/match_operations.py
+-rw-r--r--   0        0        0     1268 2023-07-17 19:16:54.906537 pydantic_neo4j-0.1.2/pydantic-neo4j/pydantic_neo4j.py
+-rw-r--r--   0        0        0      603 2023-07-17 20:31:33.834339 pydantic_neo4j-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      235 2023-07-17 20:27:32.715091 pydantic_neo4j-0.1.2/README.md
+-rw-r--r--   0        0        0      841 1970-01-01 00:00:00.000000 pydantic_neo4j-0.1.2/PKG-INFO
```

### Comparing `pydantic_neo4j-0.1.1/pydantic-neo4j/__init__.py` & `pydantic_neo4j-0.1.2/pydantic-neo4j/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 from .pydantic_neo4j import PydanticNeo4j as PydanticNeo4j
-from .create_operations import CreateUtilities as CreateUtilities
-from .match_operations import MatchUtilities as MatchUtilities
 from .graph_base_models import NodeModel as NodeModel
 from .graph_base_models import RelationshipModel as RelationshipModel
 from .graph_base_models import RelationshipQueryModel as RelationshipQueryModel
 from .graph_base_models import SequenceCriteriaModel as SequenceCriteriaModel
 from .graph_base_models import SequenceQueryModel as SequenceQueryModel
 from .graph_base_models import SequenceNodeModel as SequenceNodeModel
```

### Comparing `pydantic_neo4j-0.1.1/pydantic-neo4j/create_operations.py` & `pydantic_neo4j-0.1.2/pydantic-neo4j/create_operations.py`

 * *Files identical despite different names*

### Comparing `pydantic_neo4j-0.1.1/pydantic-neo4j/database_operations.py` & `pydantic_neo4j-0.1.2/pydantic-neo4j/database_operations.py`

 * *Files identical despite different names*

### Comparing `pydantic_neo4j-0.1.1/pydantic-neo4j/graph_base_models.py` & `pydantic_neo4j-0.1.2/pydantic-neo4j/graph_base_models.py`

 * *Files identical despite different names*

### Comparing `pydantic_neo4j-0.1.1/pydantic-neo4j/match_operations.py` & `pydantic_neo4j-0.1.2/pydantic-neo4j/match_operations.py`

 * *Files identical despite different names*

### Comparing `pydantic_neo4j-0.1.1/pydantic-neo4j/pydantic_neo4j.py` & `pydantic_neo4j-0.1.2/pydantic-neo4j/pydantic_neo4j.py`

 * *Files identical despite different names*

### Comparing `pydantic_neo4j-0.1.1/pyproject.toml` & `pydantic_neo4j-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-neo4j"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["MichaelZag <Michael@MichaelZag.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = 'https://github.com/Michaelzag/PydanticNeo4j'
 repository = 'https://github.com/Michaelzag/PydanticNeo4j'
 keywords = ['neo4j-pydantic','Pydantic', 'Neo4j', 'OGM', 'Neo4j-OG','MichaelZag']
```

### Comparing `pydantic_neo4j-0.1.1/PKG-INFO` & `pydantic_neo4j-0.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-neo4j
-Version: 0.1.1
+Version: 0.1.2
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
-pip install PydanticNeo4j
+pip install pydantic-neo4j
 ```
 
 ### Usage
 
 
 
 ### API
```

