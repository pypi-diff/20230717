# Comparing `tmp/acdh_cidoc_pyutils-0.8.tar.gz` & `tmp/acdh_cidoc_pyutils-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acdh_cidoc_pyutils-0.8.tar", last modified: Thu Jan 26 09:31:03 2023, max compression
+gzip compressed data, was "acdh_cidoc_pyutils-0.9.tar", last modified: Thu Jan 26 13:18:34 2023, max compression
```

## Comparing `acdh_cidoc_pyutils-0.8.tar` & `acdh_cidoc_pyutils-0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 09:31:03.411444 acdh_cidoc_pyutils-0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-01-26 09:30:53.000000 acdh_cidoc_pyutils-0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10459 2023-01-26 09:31:03.411444 acdh_cidoc_pyutils-0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9969 2023-01-26 09:30:53.000000 acdh_cidoc_pyutils-0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 09:31:03.407444 acdh_cidoc_pyutils-0.8/acdh_cidoc_pyutils/
--rw-r--r--   0 runner    (1001) docker     (123)     8597 2023-01-26 09:30:53.000000 acdh_cidoc_pyutils-0.8/acdh_cidoc_pyutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-01-26 09:30:53.000000 acdh_cidoc_pyutils-0.8/acdh_cidoc_pyutils/namespaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 09:31:03.411444 acdh_cidoc_pyutils-0.8/acdh_cidoc_pyutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10459 2023-01-26 09:31:03.000000 acdh_cidoc_pyutils-0.8/acdh_cidoc_pyutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-01-26 09:31:03.000000 acdh_cidoc_pyutils-0.8/acdh_cidoc_pyutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-26 09:31:03.000000 acdh_cidoc_pyutils-0.8/acdh_cidoc_pyutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-26 09:31:03.000000 acdh_cidoc_pyutils-0.8/acdh_cidoc_pyutils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-01-26 09:31:03.000000 acdh_cidoc_pyutils-0.8/acdh_cidoc_pyutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-01-26 09:31:03.000000 acdh_cidoc_pyutils-0.8/acdh_cidoc_pyutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-26 09:31:03.411444 acdh_cidoc_pyutils-0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-01-26 09:30:54.000000 acdh_cidoc_pyutils-0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 13:18:34.461477 acdh_cidoc_pyutils-0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-01-26 13:18:26.000000 acdh_cidoc_pyutils-0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-01-26 13:18:34.461477 acdh_cidoc_pyutils-0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11562 2023-01-26 13:18:26.000000 acdh_cidoc_pyutils-0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 13:18:34.457477 acdh_cidoc_pyutils-0.9/acdh_cidoc_pyutils/
+-rw-r--r--   0 runner    (1001) docker     (123)     9859 2023-01-26 13:18:26.000000 acdh_cidoc_pyutils-0.9/acdh_cidoc_pyutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-01-26 13:18:26.000000 acdh_cidoc_pyutils-0.9/acdh_cidoc_pyutils/namespaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 13:18:34.461477 acdh_cidoc_pyutils-0.9/acdh_cidoc_pyutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-01-26 13:18:34.000000 acdh_cidoc_pyutils-0.9/acdh_cidoc_pyutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-01-26 13:18:34.000000 acdh_cidoc_pyutils-0.9/acdh_cidoc_pyutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-26 13:18:34.000000 acdh_cidoc_pyutils-0.9/acdh_cidoc_pyutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-26 13:18:34.000000 acdh_cidoc_pyutils-0.9/acdh_cidoc_pyutils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-01-26 13:18:34.000000 acdh_cidoc_pyutils-0.9/acdh_cidoc_pyutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-01-26 13:18:34.000000 acdh_cidoc_pyutils-0.9/acdh_cidoc_pyutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-26 13:18:34.461477 acdh_cidoc_pyutils-0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-01-26 13:18:26.000000 acdh_cidoc_pyutils-0.9/setup.py
```

### Comparing `acdh_cidoc_pyutils-0.8/LICENSE` & `acdh_cidoc_pyutils-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `acdh_cidoc_pyutils-0.8/PKG-INFO` & `acdh_cidoc_pyutils-0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,68 @@
-Metadata-Version: 2.1
-Name: acdh_cidoc_pyutils
-Version: 0.8
-Summary: Helper functions for the generation of CIDOC CRMish RDF
-Home-page: https://github.com/acdh-oeaw/acdh-cidoc-pyutils
-Author: Peter Andorfer
-Author-email: peter.andorfer@oeaw.ac.at
-License: MIT license
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![flake8 Lint](https://github.com/acdh-oeaw/acdh-cidoc-pyutils/actions/workflows/lint.yml/badge.svg)](https://github.com/acdh-oeaw/acdh-cidoc-pyutils/actions/workflows/lint.yml)
 [![Test](https://github.com/acdh-oeaw/acdh-cidoc-pyutils/actions/workflows/test.yml/badge.svg)](https://github.com/acdh-oeaw/acdh-cidoc-pyutils/actions/workflows/test.yml)
 [![codecov](https://codecov.io/gh/acdh-oeaw/acdh-cidoc-pyutils/branch/main/graph/badge.svg?token=XRF7ANN1TM)](https://codecov.io/gh/acdh-oeaw/acdh-cidoc-pyutils)
 [![PyPI version](https://badge.fury.io/py/acdh-cidoc-pyutils.svg)](https://badge.fury.io/py/acdh-cidoc-pyutils)
 
 # acdh-cidoc-pyutils
-Helper functions for the generation of CIDOC CRMish RDF
+Helper functions for the generation of CIDOC CRMish RDF (from XML/TEI data)
 
-## Usage
+## Installation
 
 * install via `pip install acdh-cidoc-pyutils`
 
+## Examples
+
+### extract birth/death triples from `tei:person`
+
+```python
+import lxml.etree as ET
+from rdflib import URIRef
+from acdh_cidoc_pyutils import make_birth_death_entities, NSMAP
+
+sample = """
+<TEI xmlns="http://www.tei-c.org/ns/1.0">
+    <person xml:id="DWpers0091" sortKey="Gulbransson_Olaf_Leonhard">
+        <persName type="pref">Gulbransson, Olaf</persName>
+        <birth when="1873-05-26">
+            26. 5. 1873<placeName key="#DWplace00139">Christiania (Oslo)</placeName>
+        </birth>
+        <death>
+            <date when-iso="1905-07-04">04.07.1905</date>
+            <settlement key="pmb50">
+                <placeName type="pref">Wien</placeName>
+                <location><geo>48.2066 16.37341</geo></location>
+            </settlement>
+        </death>
+        
+    </person>
+</TEI>"""
+
+doc = ET.fromstring(sample)
+x = doc.xpath(".//tei:person[1]", namespaces=NSMAP)[0]
+xml_id = x.attrib["{http://www.w3.org/XML/1998/namespace}id"].lower()
+item_id = f"https://foo/bar/{xml_id}"
+subj = URIRef(item_id)
+event_graph, birth_uri, birth_timestamp = make_birth_death_entities(
+    subj, x, event_type="death", verbose=True
+)
+event_graph.serialize(format="turtle")
+# returns
+```
+```ttl
+@prefix ns1: <http://www.cidoc-crm.org/cidoc-crm/> .
+@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
+
+<https://foo/bar/dwpers0091/death> a ns1:E69_Death ;
+    rdfs:label "Geburt von Gulbransson, Olaf Leonhard"@fr ;
+    ns1:P100_was_death_of <https://foo/bar/dwpers0091> ;
+    ns1:P4_has_time-span <https://foo/bar/dwpers0091/death/timestamp> .
+```
+
+
 ### create `ns1:P168_place_is_defined_by "Point(456 123)"^^<geo:wktLiteral> .` from tei:coords
 ```python
 import lxml.etree as ET
 from rdflib import Graph, URIRef, RDF
 from acdh_cidoc_pyutils import coordinates_to_p168, NSMAP, CIDOC
 sample = """
 <TEI xmlns="http://www.tei-c.org/ns/1.0">
@@ -45,15 +79,15 @@
     item_id = f"https://foo/bar/{xml_id}"
     subj = URIRef(item_id)
     g.add((subj, RDF.type, CIDOC["E53_Place"]))
     g += coordinates_to_p168(subj, x)
 print(g.serialize())
 # returns
 ```
-```rdf
+```ttl
 ...
     ns1:P168_place_is_defined_by "Point(456 123)"^^<geo:wktLiteral> .
 ...
 ```
 * Function parameter `verbose` prints information in case the given xpath does not return expected results which is a text node with two numbers separated by a given separator (default value is `separator=" "`)
 * Function parameter `inverse` (default: `inverse=False`) changes the order of the coordinates.
 
@@ -144,15 +178,15 @@
     g.add((subj, RDF.type, CIDOC["E53_Place"]))
     g += make_ed42_identifiers(
         subj, x, type_domain="http://hansi/4/ever", default_lang="it"
     )
 print(g.serialize(format="turtle"))
 # returns
 ```
-```rdf
+```ttl
 @prefix ns1: <http://www.cidoc-crm.org/cidoc-crm/> .
 @prefix owl: <http://www.w3.org/2002/07/owl#> .
 @prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
 
 <https://foo/bar/dwplace00092> a ns1:E53_Place ;
     ns1:P1_is_identified_by <https://foo/bar/dwplace00092/identifier/DWplace00092>,
         <https://foo/bar/dwplace00092/identifier/idno/0>,
@@ -215,15 +249,15 @@
     g += make_appelations(
         subj, x, type_domain="http://hansi/4/ever", default_lang="it"
     )
 
 g.serialize(format="ttl")
 # returns
 ```
-```rdf
+```ttl
 @prefix ns1: <http://www.cidoc-crm.org/cidoc-crm/> .
 @prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
 
 <https://foo/bar/dwplace00092> a ns1:E53_Place ;
     ns1:P1_is_identified_by <https://foo/bar/dwplace00092/appelation/0>,
         <https://foo/bar/dwplace00092/appelation/1>,
         <https://foo/bar/dwplace00092/appelation/2> .
@@ -289,8 +323,8 @@
 ```
 
 
 ## development
 
 * `pip install -r requirements_dev.txt`
 * `flake8` -> linting
-* `coveage run -m pytest` -> runs tests and creates coverage stats
+* `coveage run -m pytest` -> runs tests and creates coverage stats
```

### Comparing `acdh_cidoc_pyutils-0.8/README.md` & `acdh_cidoc_pyutils-0.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,83 @@
+Metadata-Version: 2.1
+Name: acdh_cidoc_pyutils
+Version: 0.9
+Summary: Helper functions for the generation of CIDOC CRMish RDF
+Home-page: https://github.com/acdh-oeaw/acdh-cidoc-pyutils
+Author: Peter Andorfer
+Author-email: peter.andorfer@oeaw.ac.at
+License: MIT license
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![flake8 Lint](https://github.com/acdh-oeaw/acdh-cidoc-pyutils/actions/workflows/lint.yml/badge.svg)](https://github.com/acdh-oeaw/acdh-cidoc-pyutils/actions/workflows/lint.yml)
 [![Test](https://github.com/acdh-oeaw/acdh-cidoc-pyutils/actions/workflows/test.yml/badge.svg)](https://github.com/acdh-oeaw/acdh-cidoc-pyutils/actions/workflows/test.yml)
 [![codecov](https://codecov.io/gh/acdh-oeaw/acdh-cidoc-pyutils/branch/main/graph/badge.svg?token=XRF7ANN1TM)](https://codecov.io/gh/acdh-oeaw/acdh-cidoc-pyutils)
 [![PyPI version](https://badge.fury.io/py/acdh-cidoc-pyutils.svg)](https://badge.fury.io/py/acdh-cidoc-pyutils)
 
 # acdh-cidoc-pyutils
-Helper functions for the generation of CIDOC CRMish RDF
+Helper functions for the generation of CIDOC CRMish RDF (from XML/TEI data)
 
-## Usage
+## Installation
 
 * install via `pip install acdh-cidoc-pyutils`
 
+## Examples
+
+### extract birth/death triples from `tei:person`
+
+```python
+import lxml.etree as ET
+from rdflib import URIRef
+from acdh_cidoc_pyutils import make_birth_death_entities, NSMAP
+
+sample = """
+<TEI xmlns="http://www.tei-c.org/ns/1.0">
+    <person xml:id="DWpers0091" sortKey="Gulbransson_Olaf_Leonhard">
+        <persName type="pref">Gulbransson, Olaf</persName>
+        <birth when="1873-05-26">
+            26. 5. 1873<placeName key="#DWplace00139">Christiania (Oslo)</placeName>
+        </birth>
+        <death>
+            <date when-iso="1905-07-04">04.07.1905</date>
+            <settlement key="pmb50">
+                <placeName type="pref">Wien</placeName>
+                <location><geo>48.2066 16.37341</geo></location>
+            </settlement>
+        </death>
+        
+    </person>
+</TEI>"""
+
+doc = ET.fromstring(sample)
+x = doc.xpath(".//tei:person[1]", namespaces=NSMAP)[0]
+xml_id = x.attrib["{http://www.w3.org/XML/1998/namespace}id"].lower()
+item_id = f"https://foo/bar/{xml_id}"
+subj = URIRef(item_id)
+event_graph, birth_uri, birth_timestamp = make_birth_death_entities(
+    subj, x, event_type="death", verbose=True
+)
+event_graph.serialize(format="turtle")
+# returns
+```
+```ttl
+@prefix ns1: <http://www.cidoc-crm.org/cidoc-crm/> .
+@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
+
+<https://foo/bar/dwpers0091/death> a ns1:E69_Death ;
+    rdfs:label "Geburt von Gulbransson, Olaf Leonhard"@fr ;
+    ns1:P100_was_death_of <https://foo/bar/dwpers0091> ;
+    ns1:P4_has_time-span <https://foo/bar/dwpers0091/death/timestamp> .
+```
+
+
 ### create `ns1:P168_place_is_defined_by "Point(456 123)"^^<geo:wktLiteral> .` from tei:coords
 ```python
 import lxml.etree as ET
 from rdflib import Graph, URIRef, RDF
 from acdh_cidoc_pyutils import coordinates_to_p168, NSMAP, CIDOC
 sample = """
 <TEI xmlns="http://www.tei-c.org/ns/1.0">
@@ -30,15 +94,15 @@
     item_id = f"https://foo/bar/{xml_id}"
     subj = URIRef(item_id)
     g.add((subj, RDF.type, CIDOC["E53_Place"]))
     g += coordinates_to_p168(subj, x)
 print(g.serialize())
 # returns
 ```
-```rdf
+```ttl
 ...
     ns1:P168_place_is_defined_by "Point(456 123)"^^<geo:wktLiteral> .
 ...
 ```
 * Function parameter `verbose` prints information in case the given xpath does not return expected results which is a text node with two numbers separated by a given separator (default value is `separator=" "`)
 * Function parameter `inverse` (default: `inverse=False`) changes the order of the coordinates.
 
@@ -129,15 +193,15 @@
     g.add((subj, RDF.type, CIDOC["E53_Place"]))
     g += make_ed42_identifiers(
         subj, x, type_domain="http://hansi/4/ever", default_lang="it"
     )
 print(g.serialize(format="turtle"))
 # returns
 ```
-```rdf
+```ttl
 @prefix ns1: <http://www.cidoc-crm.org/cidoc-crm/> .
 @prefix owl: <http://www.w3.org/2002/07/owl#> .
 @prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
 
 <https://foo/bar/dwplace00092> a ns1:E53_Place ;
     ns1:P1_is_identified_by <https://foo/bar/dwplace00092/identifier/DWplace00092>,
         <https://foo/bar/dwplace00092/identifier/idno/0>,
@@ -200,15 +264,15 @@
     g += make_appelations(
         subj, x, type_domain="http://hansi/4/ever", default_lang="it"
     )
 
 g.serialize(format="ttl")
 # returns
 ```
-```rdf
+```ttl
 @prefix ns1: <http://www.cidoc-crm.org/cidoc-crm/> .
 @prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
 
 <https://foo/bar/dwplace00092> a ns1:E53_Place ;
     ns1:P1_is_identified_by <https://foo/bar/dwplace00092/appelation/0>,
         <https://foo/bar/dwplace00092/appelation/1>,
         <https://foo/bar/dwplace00092/appelation/2> .
@@ -274,8 +338,8 @@
 ```
 
 
 ## development
 
 * `pip install -r requirements_dev.txt`
 * `flake8` -> linting
-* `coveage run -m pytest` -> runs tests and creates coverage stats
+* `coveage run -m pytest` -> runs tests and creates coverage stats
```

### Comparing `acdh_cidoc_pyutils-0.8/acdh_cidoc_pyutils/__init__.py` & `acdh_cidoc_pyutils-0.9/acdh_cidoc_pyutils/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -231,7 +231,44 @@
                         OWL.sameAs,
                         URIRef(
                             x.text,
                         ),
                     )
                 )
     return g
+
+
+def make_birth_death_entities(
+    subj: URIRef,
+    node: Element,
+    event_type="birth",
+    verbose=False,
+    default_prefix="Geburt von",
+    default_lang="de",
+):
+    g = Graph()
+    name_node = node.xpath(".//tei:persName[1]", namespaces=NSMAP)[0]
+    label, label_lang = make_entity_label(name_node, default_lang=default_lang)
+    if event_type not in ["birth", "death"]:
+        return (g, None, None)
+    if event_type == "birth":
+        cidoc_property = CIDOC["P98_brought_into_life"]
+        cidoc_class = CIDOC["E67_Birth"]
+    else:
+        cidoc_property = CIDOC["P100_was_death_of"]
+        cidoc_class = CIDOC["E69_Death"]
+    xpath_expr = f".//tei:{event_type}[1]"
+    try:
+        node.xpath(xpath_expr, namespaces=NSMAP)[0]
+    except IndexError as e:
+        if verbose:
+            print(subj, e)
+            return (g, None, None)
+    event_uri = URIRef(f"{subj}/{event_type}")
+    time_stamp_uri = URIRef(f"{event_uri}/timestamp")
+    g.set((event_uri, cidoc_property, subj))
+    g.set((event_uri, RDF.type, cidoc_class))
+    g.add(
+        (event_uri, RDFS.label, Literal(f"{default_prefix} {label}", lang=label_lang))
+    )
+    g.set((event_uri, CIDOC["P4_has_time-span"], time_stamp_uri))
+    return (g, event_uri, time_stamp_uri)
```

### Comparing `acdh_cidoc_pyutils-0.8/acdh_cidoc_pyutils.egg-info/PKG-INFO` & `acdh_cidoc_pyutils-0.9/acdh_cidoc_pyutils.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acdh-cidoc-pyutils
-Version: 0.8
+Version: 0.9
 Summary: Helper functions for the generation of CIDOC CRMish RDF
 Home-page: https://github.com/acdh-oeaw/acdh-cidoc-pyutils
 Author: Peter Andorfer
 Author-email: peter.andorfer@oeaw.ac.at
 License: MIT license
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -15,20 +15,69 @@
 
 [![flake8 Lint](https://github.com/acdh-oeaw/acdh-cidoc-pyutils/actions/workflows/lint.yml/badge.svg)](https://github.com/acdh-oeaw/acdh-cidoc-pyutils/actions/workflows/lint.yml)
 [![Test](https://github.com/acdh-oeaw/acdh-cidoc-pyutils/actions/workflows/test.yml/badge.svg)](https://github.com/acdh-oeaw/acdh-cidoc-pyutils/actions/workflows/test.yml)
 [![codecov](https://codecov.io/gh/acdh-oeaw/acdh-cidoc-pyutils/branch/main/graph/badge.svg?token=XRF7ANN1TM)](https://codecov.io/gh/acdh-oeaw/acdh-cidoc-pyutils)
 [![PyPI version](https://badge.fury.io/py/acdh-cidoc-pyutils.svg)](https://badge.fury.io/py/acdh-cidoc-pyutils)
 
 # acdh-cidoc-pyutils
-Helper functions for the generation of CIDOC CRMish RDF
+Helper functions for the generation of CIDOC CRMish RDF (from XML/TEI data)
 
-## Usage
+## Installation
 
 * install via `pip install acdh-cidoc-pyutils`
 
+## Examples
+
+### extract birth/death triples from `tei:person`
+
+```python
+import lxml.etree as ET
+from rdflib import URIRef
+from acdh_cidoc_pyutils import make_birth_death_entities, NSMAP
+
+sample = """
+<TEI xmlns="http://www.tei-c.org/ns/1.0">
+    <person xml:id="DWpers0091" sortKey="Gulbransson_Olaf_Leonhard">
+        <persName type="pref">Gulbransson, Olaf</persName>
+        <birth when="1873-05-26">
+            26. 5. 1873<placeName key="#DWplace00139">Christiania (Oslo)</placeName>
+        </birth>
+        <death>
+            <date when-iso="1905-07-04">04.07.1905</date>
+            <settlement key="pmb50">
+                <placeName type="pref">Wien</placeName>
+                <location><geo>48.2066 16.37341</geo></location>
+            </settlement>
+        </death>
+        
+    </person>
+</TEI>"""
+
+doc = ET.fromstring(sample)
+x = doc.xpath(".//tei:person[1]", namespaces=NSMAP)[0]
+xml_id = x.attrib["{http://www.w3.org/XML/1998/namespace}id"].lower()
+item_id = f"https://foo/bar/{xml_id}"
+subj = URIRef(item_id)
+event_graph, birth_uri, birth_timestamp = make_birth_death_entities(
+    subj, x, event_type="death", verbose=True
+)
+event_graph.serialize(format="turtle")
+# returns
+```
+```ttl
+@prefix ns1: <http://www.cidoc-crm.org/cidoc-crm/> .
+@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
+
+<https://foo/bar/dwpers0091/death> a ns1:E69_Death ;
+    rdfs:label "Geburt von Gulbransson, Olaf Leonhard"@fr ;
+    ns1:P100_was_death_of <https://foo/bar/dwpers0091> ;
+    ns1:P4_has_time-span <https://foo/bar/dwpers0091/death/timestamp> .
+```
+
+
 ### create `ns1:P168_place_is_defined_by "Point(456 123)"^^<geo:wktLiteral> .` from tei:coords
 ```python
 import lxml.etree as ET
 from rdflib import Graph, URIRef, RDF
 from acdh_cidoc_pyutils import coordinates_to_p168, NSMAP, CIDOC
 sample = """
 <TEI xmlns="http://www.tei-c.org/ns/1.0">
@@ -45,15 +94,15 @@
     item_id = f"https://foo/bar/{xml_id}"
     subj = URIRef(item_id)
     g.add((subj, RDF.type, CIDOC["E53_Place"]))
     g += coordinates_to_p168(subj, x)
 print(g.serialize())
 # returns
 ```
-```rdf
+```ttl
 ...
     ns1:P168_place_is_defined_by "Point(456 123)"^^<geo:wktLiteral> .
 ...
 ```
 * Function parameter `verbose` prints information in case the given xpath does not return expected results which is a text node with two numbers separated by a given separator (default value is `separator=" "`)
 * Function parameter `inverse` (default: `inverse=False`) changes the order of the coordinates.
 
@@ -144,15 +193,15 @@
     g.add((subj, RDF.type, CIDOC["E53_Place"]))
     g += make_ed42_identifiers(
         subj, x, type_domain="http://hansi/4/ever", default_lang="it"
     )
 print(g.serialize(format="turtle"))
 # returns
 ```
-```rdf
+```ttl
 @prefix ns1: <http://www.cidoc-crm.org/cidoc-crm/> .
 @prefix owl: <http://www.w3.org/2002/07/owl#> .
 @prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
 
 <https://foo/bar/dwplace00092> a ns1:E53_Place ;
     ns1:P1_is_identified_by <https://foo/bar/dwplace00092/identifier/DWplace00092>,
         <https://foo/bar/dwplace00092/identifier/idno/0>,
@@ -215,15 +264,15 @@
     g += make_appelations(
         subj, x, type_domain="http://hansi/4/ever", default_lang="it"
     )
 
 g.serialize(format="ttl")
 # returns
 ```
-```rdf
+```ttl
 @prefix ns1: <http://www.cidoc-crm.org/cidoc-crm/> .
 @prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
 
 <https://foo/bar/dwplace00092> a ns1:E53_Place ;
     ns1:P1_is_identified_by <https://foo/bar/dwplace00092/appelation/0>,
         <https://foo/bar/dwplace00092/appelation/1>,
         <https://foo/bar/dwplace00092/appelation/2> .
```

### Comparing `acdh_cidoc_pyutils-0.8/setup.py` & `acdh_cidoc_pyutils-0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,10 +32,10 @@
     include_package_data=True,
     name="acdh_cidoc_pyutils",
     packages=find_packages(include=["acdh_cidoc_pyutils", "acdh_cidoc_pyutils.*"]),
     setup_requires=[],
     test_suite="tests",
     tests_require=[],
     url="https://github.com/acdh-oeaw/acdh-cidoc-pyutils",
-    version="v0.8",
+    version="v0.9",
     zip_safe=False,
 )
```

