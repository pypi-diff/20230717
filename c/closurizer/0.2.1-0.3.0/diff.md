# Comparing `tmp/closurizer-0.2.1.tar.gz` & `tmp/closurizer-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "closurizer-0.2.1.tar", max compression
+gzip compressed data, was "closurizer-0.3.0.tar", max compression
```

## Comparing `closurizer-0.2.1.tar` & `closurizer-0.3.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      641 2023-07-13 00:15:40.582102 closurizer-0.2.1/closurizer/cli.py
--rw-r--r--   0        0        0     4352 2023-07-13 00:15:40.582102 closurizer-0.2.1/closurizer/closurizer.py
--rw-r--r--   0        0        0      463 2023-07-13 00:15:40.582102 closurizer-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      575 1970-01-01 00:00:00.000000 closurizer-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      641 2023-07-17 17:22:40.145031 closurizer-0.3.0/closurizer/cli.py
+-rw-r--r--   0        0        0     4698 2023-07-17 17:22:40.145031 closurizer-0.3.0/closurizer/closurizer.py
+-rw-r--r--   0        0        0      463 2023-07-17 17:22:40.145031 closurizer-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      575 1970-01-01 00:00:00.000000 closurizer-0.3.0/PKG-INFO
```

### Comparing `closurizer-0.2.1/closurizer/cli.py` & `closurizer-0.3.0/closurizer/cli.py`

 * *Files identical despite different names*

### Comparing `closurizer-0.2.1/closurizer/closurizer.py` & `closurizer-0.3.0/closurizer/closurizer.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,22 +5,24 @@
 import tarfile
 
 
 def _string_agg(key, rows):
     return [key, "|".join(row[1] for row in rows)]
 
 
-def _cut_left_join(ltable, rtable, field, attribute):
+def _cut_left_join(ltable, rtable, field, attribute, rename_attribute = None):
+    if rename_attribute is None:
+        rename_attribute = attribute
     return etl.leftjoin(ltable,
-                        (etl.cut(rtable, ['id', attribute]).rename(attribute, f"{field}_{attribute}")),
+                        (etl.cut(rtable, ['id', attribute]).rename(attribute, f"{field}_{rename_attribute}")),
                         lkey=field,
                         rkey="id")
 
 def _length(value):
-    if value is None:
+    if value is None or value == "":
         return 0
     else:
         return len(value.split("|"))
 
 def _length_of_field_values(rec, fields):
     value = 0
     for field in fields:
@@ -88,16 +90,22 @@
                            .rename('ancestor_labels', 'closure_label'))
 
     for field in fields:
         edges = _cut_left_join(edges, nodes, field, "namespace")
         edges = _cut_left_join(edges, nodes, field, "category")
         edges = _cut_left_join(edges, closure_id_table, field, "closure")
         edges = _cut_left_join(edges, closure_label_table, field, "closure_label")
-        edges = etl.leftjoin(edges, (etl.cut(nodes, ["id", "name"]).rename("name", f"{field}_label")), lkey=field,
-                             rkey="id")
+        # only add taxon labels to subject & object
+        edges = _cut_left_join(edges, nodes, field, "name", rename_attribute="label")
+
+        if field in ['subject', 'object']:
+            edges = _cut_left_join(edges, nodes, field, "in_taxon", rename_attribute="taxon")
+            edges = _cut_left_join(edges, nodes, field, "in_taxon_label", rename_attribute="taxon_label")
+
+
 
     print("Adding evidence counts...")
 
     edges = etl.addfield(edges, 'evidence_count',
                          lambda rec: _length_of_field_values(rec, evidence_fields))
 
     print("Denormalizing...")
```

### Comparing `closurizer-0.2.1/PKG-INFO` & `closurizer-0.3.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: closurizer
-Version: 0.2.1
+Version: 0.3.0
 Summary: Add closure expansion fields to kgx files following the Golr pattern
 Author: Kevin Schaper
 Author-email: kevin@tislab.org
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

