# Comparing `tmp/neopydantic-0.4.4.tar.gz` & `tmp/neopydantic-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neopydantic-0.4.4.tar", max compression
+gzip compressed data, was "neopydantic-0.4.5.tar", max compression
```

## Comparing `neopydantic-0.4.4.tar` & `neopydantic-0.4.5.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0      429 2023-07-17 16:51:04.663034 neopydantic-0.4.4/neopydantic/__init__.py
--rw-r--r--   0        0        0     5539 2023-07-17 16:51:04.658030 neopydantic-0.4.4/neopydantic/create_operations.py
--rw-r--r--   0        0        0     4422 2023-07-17 16:51:04.668034 neopydantic-0.4.4/neopydantic/database_operations.py
--rw-r--r--   0        0        0     3546 2023-07-17 16:00:22.376645 neopydantic-0.4.4/neopydantic/graph_base_models.py
--rw-r--r--   0        0        0    10198 2023-07-17 15:59:26.982247 neopydantic-0.4.4/neopydantic/match_operations.py
--rw-r--r--   0        0        0      616 2023-07-17 16:51:11.831668 neopydantic-0.4.4/pyproject.toml
--rw-r--r--   0        0        0      168 2023-07-17 16:02:34.855180 neopydantic-0.4.4/README.md
--rw-r--r--   0        0        0      949 1970-01-01 00:00:00.000000 neopydantic-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0      729 2023-07-17 17:17:06.680998 neopydantic-0.4.5/neopydantic/__init__.py
+-rw-r--r--   0        0        0     5611 2023-07-17 17:17:06.673995 neopydantic-0.4.5/neopydantic/create_operations.py
+-rw-r--r--   0        0        0     4426 2023-07-17 17:12:07.597420 neopydantic-0.4.5/neopydantic/database_operations.py
+-rw-r--r--   0        0        0     3131 2023-07-17 17:12:07.586416 neopydantic-0.4.5/neopydantic/graph_base_models.py
+-rw-r--r--   0        0        0    10212 2023-07-17 17:17:06.663011 neopydantic-0.4.5/neopydantic/match_operations.py
+-rw-r--r--   0        0        0      475 2023-07-17 17:12:07.582417 neopydantic-0.4.5/neopydantic/neopydantic.py
+-rw-r--r--   0        0        0        0 2023-07-17 17:01:26.874471 neopydantic-0.4.5/neopydantic/operations/__init__.py
+-rw-r--r--   0        0        0      616 2023-07-17 17:17:43.724093 neopydantic-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0      168 2023-07-17 16:02:34.855180 neopydantic-0.4.5/README.md
+-rw-r--r--   0        0        0      949 1970-01-01 00:00:00.000000 neopydantic-0.4.5/PKG-INFO
```

### Comparing `neopydantic-0.4.4/neopydantic/create_operations.py` & `neopydantic-0.4.5/neopydantic/create_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,20 @@
 
 from graph_base_models import NodeModel, Neo4jModel, RelationshipModel
 from database_operations import DatabaseOperations
 from match_operations import MatchUtilities
 
 
 class CreateUtilities:
-    dbops = DatabaseOperations()
-    matchops = MatchUtilities()
+
+    def __int__(self, db: DatabaseOperations, matchops: MatchUtilities):
+        self.dbops = db
+        self.matchops = matchops
+
+
 
     @staticmethod
     def str_to_class(model: Type[Neo4jModel], **kwargs) -> Any | None:
         """Return a class instance from a string reference"""
         try:
             module_ = importlib.import_module(model.__module__)
             class_ = getattr(module_, model.__name__)(**kwargs)
```

### Comparing `neopydantic-0.4.4/neopydantic/database_operations.py` & `neopydantic-0.4.5/neopydantic/database_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,17 +8,19 @@
 
 from typing import Any, Type
 
 from graph_base_models import Neo4jModel
 
 
 class DatabaseOperations:
+
     def __init__(self, uri, username, password):
         self.driver = neo4j.AsyncGraphDatabase.driver(uri, auth=(username, password))
 
+
     async def run_query(self, query: str, **kwargs) -> neo4j.EagerResult:
         async with self.driver.session() as session:
             result = await session.run(query, **kwargs)
             eager_results = await result.to_eager_result()
         return eager_results
 
     @staticmethod
```

### Comparing `neopydantic-0.4.4/neopydantic/graph_base_models.py` & `neopydantic-0.4.5/neopydantic/graph_base_models.py`

 * *Files 20% similar despite different names*

```diff
@@ -55,27 +55,14 @@
     def get_fields(self) -> Dict[str, Any]:
         fields = {}
         for field, value in self.__class__.model_fields.items():
             if field != "start_node" and field != "end_node":
                 fields[field] = getattr(self, field)
         return fields
 
-    """
-    def is_eq_fuzzy(self, other) -> bool:
-        return (self.is_fuzzy(other.rel_from) and
-                self.is_fuzzy(other.rel_to) and
-                self.is_fuzzy(other.relationship))
-    """
-    """
-    def __eq__(self, other):
-        return (self.is_exact(other.rel_from) and
-                self.is_exact(other.rel_to) and
-                self.is_fuzzy(other.relationship))
-    """
-
 
 class RelationshipQueryModel(BaseModel):
     start_node_name: Optional[str] = Field(default="")
     start_criteria: Optional[Dict] = Field(default_factory=dict)
     end_node_name: Optional[str] = Field(default="")
     end_criteria: Optional[Dict] = Field(default_factory=dict)
     relationship_name: Optional[str] = Field(default="")
```

### Comparing `neopydantic-0.4.4/neopydantic/match_operations.py` & `neopydantic-0.4.5/neopydantic/match_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import uuid
 from datetime import datetime
 
 from typing import Union
 import neo4j
 from pydantic import create_model
 
-from app.Models.neo4j.graph_base import (
+from graph_base_models import (
     NodeModel,
     RelationshipModel,
     SequenceNodeModel,
     SequenceQueryModel,
 )
 
-from app.Neo4jUtility.database_operations import DatabaseOperations
+from database_operations import DatabaseOperations
 
 
 class MatchUtilities:
-    dbops = DatabaseOperations()
+    def __int__(self, db: DatabaseOperations):
+        self.dbops = db
+
 
     @staticmethod
     def get_node_prefix(node_name: str, node_prefix: str) -> str:
         if node_name != "":
             node_query = f"{node_prefix}:{node_name}"
         else:
             node_query = node_prefix
```

### Comparing `neopydantic-0.4.4/pyproject.toml` & `neopydantic-0.4.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neopydantic"
-version = "0.4.4"
+version = "0.4.5"
 description = ""
 authors = ["MichaelZag <Michael@MichaelZag.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = 'https://github.com/Michaelzag/NeoPydantic'
 repository = 'https://github.com/Michaelzag/NeoPydantic'
 keywords = ['Pydantic', 'Neo4j', 'OGM', 'Neo4j-OG','MichaelZag']
```

### Comparing `neopydantic-0.4.4/PKG-INFO` & `neopydantic-0.4.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neopydantic
-Version: 0.4.4
+Version: 0.4.5
 Summary: 
 Home-page: https://github.com/Michaelzag/NeoPydantic
 License: MIT
 Keywords: Pydantic,Neo4j,OGM,Neo4j-OG,MichaelZag
 Author: MichaelZag
 Author-email: Michael@MichaelZag.com
 Requires-Python: >=3.11,<4.0
```

