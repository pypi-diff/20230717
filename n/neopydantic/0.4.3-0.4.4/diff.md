# Comparing `tmp/neopydantic-0.4.3.tar.gz` & `tmp/neopydantic-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neopydantic-0.4.3.tar", max compression
+gzip compressed data, was "neopydantic-0.4.4.tar", max compression
```

## Comparing `neopydantic-0.4.3.tar` & `neopydantic-0.4.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      417 2023-07-17 16:47:25.626801 neopydantic-0.4.3/neopydantic/__init__.py
--rw-r--r--   0        0        0     5535 2023-07-17 16:33:01.998735 neopydantic-0.4.3/neopydantic/CreateOperations.py
--rw-r--r--   0        0        0     4420 2023-07-17 16:33:02.007737 neopydantic-0.4.3/neopydantic/DatabaseOperations.py
--rw-r--r--   0        0        0     3546 2023-07-17 16:00:22.376645 neopydantic-0.4.3/neopydantic/GraphBaseModels.py
--rw-r--r--   0        0        0    10198 2023-07-17 15:59:26.982247 neopydantic-0.4.3/neopydantic/MatchOperations.py
--rw-r--r--   0        0        0      616 2023-07-17 16:47:44.881524 neopydantic-0.4.3/pyproject.toml
--rw-r--r--   0        0        0      168 2023-07-17 16:02:34.855180 neopydantic-0.4.3/README.md
--rw-r--r--   0        0        0      949 1970-01-01 00:00:00.000000 neopydantic-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0      429 2023-07-17 16:51:04.663034 neopydantic-0.4.4/neopydantic/__init__.py
+-rw-r--r--   0        0        0     5539 2023-07-17 16:51:04.658030 neopydantic-0.4.4/neopydantic/create_operations.py
+-rw-r--r--   0        0        0     4422 2023-07-17 16:51:04.668034 neopydantic-0.4.4/neopydantic/database_operations.py
+-rw-r--r--   0        0        0     3546 2023-07-17 16:00:22.376645 neopydantic-0.4.4/neopydantic/graph_base_models.py
+-rw-r--r--   0        0        0    10198 2023-07-17 15:59:26.982247 neopydantic-0.4.4/neopydantic/match_operations.py
+-rw-r--r--   0        0        0      616 2023-07-17 16:51:11.831668 neopydantic-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0      168 2023-07-17 16:02:34.855180 neopydantic-0.4.4/README.md
+-rw-r--r--   0        0        0      949 1970-01-01 00:00:00.000000 neopydantic-0.4.4/PKG-INFO
```

### Comparing `neopydantic-0.4.3/neopydantic/CreateOperations.py` & `neopydantic-0.4.4/neopydantic/create_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import importlib
 import uuid
 from typing import Type, Any
 
 import neo4j
 
-from GraphBaseModels import NodeModel, Neo4jModel, RelationshipModel
-from DatabaseOperations import DatabaseOperations
-from MatchOperations import MatchUtilities
+from graph_base_models import NodeModel, Neo4jModel, RelationshipModel
+from database_operations import DatabaseOperations
+from match_operations import MatchUtilities
 
 
 class CreateUtilities:
     dbops = DatabaseOperations()
     matchops = MatchUtilities()
 
     @staticmethod
```

### Comparing `neopydantic-0.4.3/neopydantic/DatabaseOperations.py` & `neopydantic-0.4.4/neopydantic/database_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import string
 import uuid
 
 import neo4j
 
 from typing import Any, Type
 
-from GraphBaseModels import Neo4jModel
+from graph_base_models import Neo4jModel
 
 
 class DatabaseOperations:
     def __init__(self, uri, username, password):
         self.driver = neo4j.AsyncGraphDatabase.driver(uri, auth=(username, password))
 
     async def run_query(self, query: str, **kwargs) -> neo4j.EagerResult:
```

### Comparing `neopydantic-0.4.3/neopydantic/GraphBaseModels.py` & `neopydantic-0.4.4/neopydantic/graph_base_models.py`

 * *Files identical despite different names*

### Comparing `neopydantic-0.4.3/neopydantic/MatchOperations.py` & `neopydantic-0.4.4/neopydantic/match_operations.py`

 * *Files identical despite different names*

### Comparing `neopydantic-0.4.3/pyproject.toml` & `neopydantic-0.4.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neopydantic"
-version = "0.4.3"
+version = "0.4.4"
 description = ""
 authors = ["MichaelZag <Michael@MichaelZag.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = 'https://github.com/Michaelzag/NeoPydantic'
 repository = 'https://github.com/Michaelzag/NeoPydantic'
 keywords = ['Pydantic', 'Neo4j', 'OGM', 'Neo4j-OG','MichaelZag']
```

### Comparing `neopydantic-0.4.3/PKG-INFO` & `neopydantic-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neopydantic
-Version: 0.4.3
+Version: 0.4.4
 Summary: 
 Home-page: https://github.com/Michaelzag/NeoPydantic
 License: MIT
 Keywords: Pydantic,Neo4j,OGM,Neo4j-OG,MichaelZag
 Author: MichaelZag
 Author-email: Michael@MichaelZag.com
 Requires-Python: >=3.11,<4.0
```

