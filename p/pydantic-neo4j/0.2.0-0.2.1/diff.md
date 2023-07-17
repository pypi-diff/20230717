# Comparing `tmp/pydantic_neo4j-0.2.0.tar.gz` & `tmp/pydantic_neo4j-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_neo4j-0.2.0.tar", max compression
+gzip compressed data, was "pydantic_neo4j-0.2.1.tar", max compression
```

## Comparing `pydantic_neo4j-0.2.0.tar` & `pydantic_neo4j-0.2.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      709 2023-07-17 20:31:16.591559 pydantic_neo4j-0.2.0/pydantic_neo4j/__init__.py
--rw-r--r--   0        0        0     5756 2023-07-17 18:59:47.287301 pydantic_neo4j-0.2.0/pydantic_neo4j/create_operations.py
--rw-r--r--   0        0        0     4468 2023-07-17 18:21:59.136803 pydantic_neo4j-0.2.0/pydantic_neo4j/database_operations.py
--rw-r--r--   0        0        0     3131 2023-07-17 17:12:07.586416 pydantic_neo4j-0.2.0/pydantic_neo4j/graph_base_models.py
--rw-r--r--   0        0        0    10473 2023-07-17 18:57:27.287819 pydantic_neo4j-0.2.0/pydantic_neo4j/match_operations.py
--rw-r--r--   0        0        0     1268 2023-07-17 19:16:54.906537 pydantic_neo4j-0.2.0/pydantic_neo4j/pydantic_neo4j.py
--rw-r--r--   0        0        0      603 2023-07-17 21:32:08.660885 pydantic_neo4j-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4662 2023-07-17 21:31:30.229591 pydantic_neo4j-0.2.0/README.md
--rw-r--r--   0        0        0     5139 1970-01-01 00:00:00.000000 pydantic_neo4j-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      709 2023-07-17 21:35:03.897555 pydantic_neo4j-0.2.1/pydantic_neo4j/__init__.py
+-rw-r--r--   0        0        0     5756 2023-07-17 21:35:03.897555 pydantic_neo4j-0.2.1/pydantic_neo4j/create_operations.py
+-rw-r--r--   0        0        0     4468 2023-07-17 21:35:03.902896 pydantic_neo4j-0.2.1/pydantic_neo4j/database_operations.py
+-rw-r--r--   0        0        0     3131 2023-07-17 21:35:03.903866 pydantic_neo4j-0.2.1/pydantic_neo4j/graph_base_models.py
+-rw-r--r--   0        0        0    10473 2023-07-17 21:35:03.903866 pydantic_neo4j-0.2.1/pydantic_neo4j/match_operations.py
+-rw-r--r--   0        0        0     1268 2023-07-17 21:35:03.903866 pydantic_neo4j-0.2.1/pydantic_neo4j/pydantic_neo4j.py
+-rw-r--r--   0        0        0      603 2023-07-17 21:41:40.813037 pydantic_neo4j-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4736 2023-07-17 21:41:20.964929 pydantic_neo4j-0.2.1/README.md
+-rw-r--r--   0        0        0     5209 1970-01-01 00:00:00.000000 pydantic_neo4j-0.2.1/PKG-INFO
```

### Comparing `pydantic_neo4j-0.2.0/pydantic_neo4j/__init__.py` & `pydantic_neo4j-0.2.1/pydantic_neo4j/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic_neo4j-0.2.0/pydantic_neo4j/create_operations.py` & `pydantic_neo4j-0.2.1/pydantic_neo4j/create_operations.py`

 * *Files identical despite different names*

### Comparing `pydantic_neo4j-0.2.0/pydantic_neo4j/database_operations.py` & `pydantic_neo4j-0.2.1/pydantic_neo4j/database_operations.py`

 * *Files identical despite different names*

### Comparing `pydantic_neo4j-0.2.0/pydantic_neo4j/graph_base_models.py` & `pydantic_neo4j-0.2.1/pydantic_neo4j/graph_base_models.py`

 * *Files identical despite different names*

### Comparing `pydantic_neo4j-0.2.0/pydantic_neo4j/match_operations.py` & `pydantic_neo4j-0.2.1/pydantic_neo4j/match_operations.py`

 * *Files identical despite different names*

### Comparing `pydantic_neo4j-0.2.0/pydantic_neo4j/pydantic_neo4j.py` & `pydantic_neo4j-0.2.1/pydantic_neo4j/pydantic_neo4j.py`

 * *Files identical despite different names*

### Comparing `pydantic_neo4j-0.2.0/pyproject.toml` & `pydantic_neo4j-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-neo4j"
-version = "0.2.0"
+version = "0.2.1"
 description = ""
 authors = ["MichaelZag <Michael@MichaelZag.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = 'https://github.com/Michaelzag/PydanticNeo4j'
 repository = 'https://github.com/Michaelzag/PydanticNeo4j'
 keywords = ['neo4j-pydantic','Pydantic', 'Neo4j', 'OGM', 'Neo4j-OG','MichaelZag']
```

### Comparing `pydantic_neo4j-0.2.0/README.md` & `pydantic_neo4j-0.2.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 
 
-### Purpose of the Package
+## Purpose of the Package
 + To translate from Pydantic models to Neo4j Graphs
 
-### Getting Started
+## Getting Started
 + Install the package
 ```bash
 pip install pydantic-neo4j
 ```
 
-### Usage
+## Usage
 + Import the package and models
 ```python
 from pydantic_neo4j import (PydanticNeo4j, 
                             RelationshipQueryModel,
                             NodeModel,
                             SequenceCriteriaModel, 
                             SequenceQueryModel, 
                             SequenceNodeModel)
 ```
+___
 + Initialize the class and get the utilities
 ```python
 
 pydantic_neo4j = PydanticNeo4j(username='neo4j', password='neo4j', uri='neo4j://localhost:7687)
 match_util = pydantic_neo4j.match_utilities
 create_util = pydantic_neo4j.create_utilities
 database_operations = pydantic_neo4j.database_operations
 ```
+___
 + Create some Pydantic models
 ```python
 class Manufacturer(NodeModel):
     name: str
 
 class Design(NodeModel):
     color: str
@@ -40,16 +42,15 @@
     
 class IsOrderable(RelationshipModel):
     pass
 
 class Produces(RelationshipModel):
     design_revision: int
 ```
-
-
+___
 + Create the nodes and relationships. All relationships must have a start_node and end_node
 ```python
 relationships = []
 
 manufacturer = Manufacturer(name="Acme")
 design = Design(color="red")
 produces = Produces(design_revision=3, start_node=manufacturer, end_node=design)
@@ -66,53 +67,55 @@
 relationships.append(is_orderable)
 ```
 
 + Add the nodes and relationships to the graph
 ```python
 await create_util.create_relationships(relationships=relationships)
 ````
+___
 + Query the graph for a single node. Lets find a manufacturer
 ```python
 nodes = await match_util.node_query(node_name='Manufacturer')
-
+___
 ```
 + Query the graph for multiple nodes. Lets find all nodes that are active
 ```python
 nodes = await match_util.node_query(criteria={'active': True})
 ```
-
+___
 + Query the graph for a single relationship. Lets find a manufacturer that produces a red design
 ```python
 query = RelationshipQueryModel(
     start_node_name="Manufacturer",
     start_criteria={},
     end_node_name="Design",
     end_criteria={"color": "red"},
     relationship_name="Produces",
     relationship_criteria={})
 result = await match_util.match_relationship(query=query)
 ```
-
+___
 + Query the graph for multiple relationships. Lets find all manufacturers that make a widget component
 + This uses a sequence, which is a series of relationships. Similar to Neo4j Path
 ```python
 sequence_query = SequenceQueryModel()
 
 sequence_query.node_sequence.append(SequenceCriteriaModel(name='Manufacturer'))
-sequence_query.relationship_sequence.append(SequenceCriteriaModel()) # a relationship with no criteria specified
+sequence_query.relationship_sequence.append(SequenceCriteriaModel()) # a relationship with no criteria
 sequence_query.node_sequence.append(SequenceCriteriaModel() # a node with no criteria specified
-sequence_query.relationship_sequence.append(SequenceCriteriaModel()) #a realtoinship with no criteria specified
-sequence_query.node_sequence.append(SequenceCriteriaModel(component_type="widget", include_with_return=True)
+sequence_query.relationship_sequence.append(SequenceCriteriaModel()) #a realtoinship with no criteria
+sequence_query.node_sequence.append(SequenceCriteriaModel(component_type="widget", 
+                                                          include_with_return=True))
 ```
 + The sequence query must always have 1 more node than relationship.
 + The order is important, and is a sequence. node - relationship - node - relationship - node
 ```python
 result = await match_util.sequence_query(sequence_query=sequence_query)
 ```
-
+___
 + Run a specific query, lets delete everything
 ```python
 await database_operations.run_query(query=f"match (n) detach delete n")
 ```
 
 
 
@@ -121,29 +124,30 @@
 + Update a node
 ```python
 nodes = await match_util.node_query(name='Manufacturer', criteria={name='Acme'})
 for graph_id, node in nodes.items():
     node.name = "Acme2"
     await create_util.update_node(node=node)
 ```
+___
 + Update a relationship
 ```python
     query = RelationshipQueryModel(
     start_node_name="Manufacturer",
     start_criteria={},
     end_node_name="Design",
     end_criteria={"color": "red"},
     relationship_name="Produces",
     relationship_criteria={})
     result = await match_util.match_relationship(query=query)
     for graph_id, relationship in result.items():
         relationship.design_revision = 4
         await create_util.update_relationship(relationship=relationship)
 ```
-
+___
 + Delete a node
 ```python
 nodes = await match_util.node_query(name='Manufacturer', criteria={name='Acme'})
 for graph_id, node in nodes.items():
     await create_util.delete_node(node=node)
 ```
```

### Comparing `pydantic_neo4j-0.2.0/PKG-INFO` & `pydantic_neo4j-0.2.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-neo4j
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 Home-page: https://github.com/Michaelzag/PydanticNeo4j
 License: MIT
 Keywords: neo4j-pydantic,Pydantic,Neo4j,OGM,Neo4j-OG,MichaelZag
 Author: MichaelZag
 Author-email: Michael@MichaelZag.com
 Requires-Python: >=3.11,<4.0
@@ -14,41 +14,43 @@
 Requires-Dist: neo4j (>=5.10.0,<6.0.0)
 Requires-Dist: pydantic (>=2.0.3,<3.0.0)
 Project-URL: Repository, https://github.com/Michaelzag/PydanticNeo4j
 Description-Content-Type: text/markdown
 
 
 
-### Purpose of the Package
+## Purpose of the Package
 + To translate from Pydantic models to Neo4j Graphs
 
-### Getting Started
+## Getting Started
 + Install the package
 ```bash
 pip install pydantic-neo4j
 ```
 
-### Usage
+## Usage
 + Import the package and models
 ```python
 from pydantic_neo4j import (PydanticNeo4j, 
                             RelationshipQueryModel,
                             NodeModel,
                             SequenceCriteriaModel, 
                             SequenceQueryModel, 
                             SequenceNodeModel)
 ```
+___
 + Initialize the class and get the utilities
 ```python
 
 pydantic_neo4j = PydanticNeo4j(username='neo4j', password='neo4j', uri='neo4j://localhost:7687)
 match_util = pydantic_neo4j.match_utilities
 create_util = pydantic_neo4j.create_utilities
 database_operations = pydantic_neo4j.database_operations
 ```
+___
 + Create some Pydantic models
 ```python
 class Manufacturer(NodeModel):
     name: str
 
 class Design(NodeModel):
     color: str
@@ -58,16 +60,15 @@
     
 class IsOrderable(RelationshipModel):
     pass
 
 class Produces(RelationshipModel):
     design_revision: int
 ```
-
-
+___
 + Create the nodes and relationships. All relationships must have a start_node and end_node
 ```python
 relationships = []
 
 manufacturer = Manufacturer(name="Acme")
 design = Design(color="red")
 produces = Produces(design_revision=3, start_node=manufacturer, end_node=design)
@@ -84,53 +85,55 @@
 relationships.append(is_orderable)
 ```
 
 + Add the nodes and relationships to the graph
 ```python
 await create_util.create_relationships(relationships=relationships)
 ````
+___
 + Query the graph for a single node. Lets find a manufacturer
 ```python
 nodes = await match_util.node_query(node_name='Manufacturer')
-
+___
 ```
 + Query the graph for multiple nodes. Lets find all nodes that are active
 ```python
 nodes = await match_util.node_query(criteria={'active': True})
 ```
-
+___
 + Query the graph for a single relationship. Lets find a manufacturer that produces a red design
 ```python
 query = RelationshipQueryModel(
     start_node_name="Manufacturer",
     start_criteria={},
     end_node_name="Design",
     end_criteria={"color": "red"},
     relationship_name="Produces",
     relationship_criteria={})
 result = await match_util.match_relationship(query=query)
 ```
-
+___
 + Query the graph for multiple relationships. Lets find all manufacturers that make a widget component
 + This uses a sequence, which is a series of relationships. Similar to Neo4j Path
 ```python
 sequence_query = SequenceQueryModel()
 
 sequence_query.node_sequence.append(SequenceCriteriaModel(name='Manufacturer'))
-sequence_query.relationship_sequence.append(SequenceCriteriaModel()) # a relationship with no criteria specified
+sequence_query.relationship_sequence.append(SequenceCriteriaModel()) # a relationship with no criteria
 sequence_query.node_sequence.append(SequenceCriteriaModel() # a node with no criteria specified
-sequence_query.relationship_sequence.append(SequenceCriteriaModel()) #a realtoinship with no criteria specified
-sequence_query.node_sequence.append(SequenceCriteriaModel(component_type="widget", include_with_return=True)
+sequence_query.relationship_sequence.append(SequenceCriteriaModel()) #a realtoinship with no criteria
+sequence_query.node_sequence.append(SequenceCriteriaModel(component_type="widget", 
+                                                          include_with_return=True))
 ```
 + The sequence query must always have 1 more node than relationship.
 + The order is important, and is a sequence. node - relationship - node - relationship - node
 ```python
 result = await match_util.sequence_query(sequence_query=sequence_query)
 ```
-
+___
 + Run a specific query, lets delete everything
 ```python
 await database_operations.run_query(query=f"match (n) detach delete n")
 ```
 
 
 
@@ -139,29 +142,30 @@
 + Update a node
 ```python
 nodes = await match_util.node_query(name='Manufacturer', criteria={name='Acme'})
 for graph_id, node in nodes.items():
     node.name = "Acme2"
     await create_util.update_node(node=node)
 ```
+___
 + Update a relationship
 ```python
     query = RelationshipQueryModel(
     start_node_name="Manufacturer",
     start_criteria={},
     end_node_name="Design",
     end_criteria={"color": "red"},
     relationship_name="Produces",
     relationship_criteria={})
     result = await match_util.match_relationship(query=query)
     for graph_id, relationship in result.items():
         relationship.design_revision = 4
         await create_util.update_relationship(relationship=relationship)
 ```
-
+___
 + Delete a node
 ```python
 nodes = await match_util.node_query(name='Manufacturer', criteria={name='Acme'})
 for graph_id, node in nodes.items():
     await create_util.delete_node(node=node)
 ```
```

