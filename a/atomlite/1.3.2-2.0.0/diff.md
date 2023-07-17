# Comparing `tmp/atomlite-1.3.2.tar.gz` & `tmp/atomlite-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atomlite-1.3.2.tar", last modified: Sat Jul  8 10:18:25 2023, max compression
+gzip compressed data, was "atomlite-2.0.0.tar", last modified: Mon Jul 17 12:09:40 2023, max compression
```

## Comparing `atomlite-1.3.2.tar` & `atomlite-2.0.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:18:25.506720 atomlite-1.3.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:18:25.506720 atomlite-1.3.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:18:25.506720 atomlite-1.3.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-08 10:17:48.000000 atomlite-1.3.2/.github/workflows/publish_release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-08 10:17:48.000000 atomlite-1.3.2/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-08 10:17:48.000000 atomlite-1.3.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-08 10:17:48.000000 atomlite-1.3.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-08 10:18:25.506720 atomlite-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-08 10:17:48.000000 atomlite-1.3.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:18:25.506720 atomlite-1.3.2/docker_testing_environment/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-08 10:17:48.000000 atomlite-1.3.2/docker_testing_environment/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:18:25.506720 atomlite-1.3.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-08 10:17:48.000000 atomlite-1.3.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:18:25.506720 atomlite-1.3.2/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:18:25.506720 atomlite-1.3.2/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 10:17:48.000000 atomlite-1.3.2/docs/source/_static/empty
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:18:25.506720 atomlite-1.3.2/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-08 10:17:48.000000 atomlite-1.3.2/docs/source/_templates/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-08 10:17:48.000000 atomlite-1.3.2/docs/source/_templates/module.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-08 10:17:48.000000 atomlite-1.3.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    12883 2023-07-08 10:17:48.000000 atomlite-1.3.2/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-08 10:17:48.000000 atomlite-1.3.2/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-08 10:17:48.000000 atomlite-1.3.2/justfile
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-08 10:17:48.000000 atomlite-1.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 10:18:25.506720 atomlite-1.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:18:25.506720 atomlite-1.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:18:25.506720 atomlite-1.3.2/src/atomlite/
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-08 10:17:48.000000 atomlite-1.3.2/src/atomlite/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:18:25.506720 atomlite-1.3.2/src/atomlite/_internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 10:17:48.000000 atomlite-1.3.2/src/atomlite/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11440 2023-07-08 10:17:48.000000 atomlite-1.3.2/src/atomlite/_internal/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-07-08 10:17:48.000000 atomlite-1.3.2/src/atomlite/_internal/json.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 10:17:48.000000 atomlite-1.3.2/src/atomlite/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:18:25.506720 atomlite-1.3.2/src/atomlite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-08 10:18:25.000000 atomlite-1.3.2/src/atomlite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-08 10:18:25.000000 atomlite-1.3.2/src/atomlite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 10:18:25.000000 atomlite-1.3.2/src/atomlite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-08 10:18:25.000000 atomlite-1.3.2/src/atomlite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-08 10:18:25.000000 atomlite-1.3.2/src/atomlite.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:18:25.506720 atomlite-1.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10179 2023-07-08 10:17:48.000000 atomlite-1.3.2/tests/test_database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:09:40.783454 atomlite-2.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:09:40.775454 atomlite-2.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:09:40.779454 atomlite-2.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-17 12:09:09.000000 atomlite-2.0.0/.github/workflows/publish_release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-17 12:09:09.000000 atomlite-2.0.0/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-17 12:09:09.000000 atomlite-2.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-17 12:09:09.000000 atomlite-2.0.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-17 12:09:40.783454 atomlite-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-17 12:09:09.000000 atomlite-2.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:09:40.779454 atomlite-2.0.0/docker_testing_environment/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-17 12:09:09.000000 atomlite-2.0.0/docker_testing_environment/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:09:40.779454 atomlite-2.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-17 12:09:09.000000 atomlite-2.0.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:09:40.779454 atomlite-2.0.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:09:40.779454 atomlite-2.0.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 12:09:09.000000 atomlite-2.0.0/docs/source/_static/empty
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:09:40.779454 atomlite-2.0.0/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-17 12:09:09.000000 atomlite-2.0.0/docs/source/_templates/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-17 12:09:09.000000 atomlite-2.0.0/docs/source/_templates/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-17 12:09:09.000000 atomlite-2.0.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12883 2023-07-17 12:09:09.000000 atomlite-2.0.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-17 12:09:09.000000 atomlite-2.0.0/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-17 12:09:09.000000 atomlite-2.0.0/justfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-17 12:09:09.000000 atomlite-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 12:09:40.783454 atomlite-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:09:40.775454 atomlite-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:09:40.779454 atomlite-2.0.0/src/atomlite/
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-17 12:09:09.000000 atomlite-2.0.0/src/atomlite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:09:40.783454 atomlite-2.0.0/src/atomlite/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 12:09:09.000000 atomlite-2.0.0/src/atomlite/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12560 2023-07-17 12:09:09.000000 atomlite-2.0.0/src/atomlite/_internal/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-07-17 12:09:09.000000 atomlite-2.0.0/src/atomlite/_internal/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 12:09:09.000000 atomlite-2.0.0/src/atomlite/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:09:40.783454 atomlite-2.0.0/src/atomlite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-17 12:09:40.000000 atomlite-2.0.0/src/atomlite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-17 12:09:40.000000 atomlite-2.0.0/src/atomlite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 12:09:40.000000 atomlite-2.0.0/src/atomlite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-17 12:09:40.000000 atomlite-2.0.0/src/atomlite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-17 12:09:40.000000 atomlite-2.0.0/src/atomlite.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:09:40.783454 atomlite-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    11602 2023-07-17 12:09:09.000000 atomlite-2.0.0/tests/test_database.py
```

### Comparing `atomlite-1.3.2/.github/workflows/publish_release.yaml` & `atomlite-2.0.0/.github/workflows/publish_release.yaml`

 * *Files identical despite different names*

### Comparing `atomlite-1.3.2/.github/workflows/tests.yaml` & `atomlite-2.0.0/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `atomlite-1.3.2/PKG-INFO` & `atomlite-2.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atomlite
-Version: 1.3.2
+Version: 2.0.0
 Maintainer-email: Lukas Turcani <lukasturcani93@gmail.com>
 Project-URL: github, https://github.com/lukasturcani/atomlite
 Project-URL: documentation, https://atomlite.readthedocs.io
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
```

### Comparing `atomlite-1.3.2/README.rst` & `atomlite-2.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `atomlite-1.3.2/docs/Makefile` & `atomlite-2.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `atomlite-1.3.2/docs/source/_templates/class.rst` & `atomlite-2.0.0/docs/source/_templates/class.rst`

 * *Files identical despite different names*

### Comparing `atomlite-1.3.2/docs/source/_templates/module.rst` & `atomlite-2.0.0/docs/source/_templates/module.rst`

 * *Files identical despite different names*

### Comparing `atomlite-1.3.2/docs/source/conf.py` & `atomlite-2.0.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `atomlite-1.3.2/docs/source/index.rst` & `atomlite-2.0.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `atomlite-1.3.2/justfile` & `atomlite-2.0.0/justfile`

 * *Files identical despite different names*

### Comparing `atomlite-1.3.2/pyproject.toml` & `atomlite-2.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `atomlite-1.3.2/src/atomlite/_internal/database.py` & `atomlite-2.0.0/src/atomlite/_internal/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,49 +152,74 @@
         if commit:
             self.connection.commit()
 
     def update_entries(
         self,
         entries: Entry | collections.abc.Iterable[Entry],
         merge_properties: bool = True,
+        upsert: bool = True,
         commit: bool = True,
     ) -> None:
         """
         Update molecules in the database.
 
         Parameters:
             entries (Entry | list[Entry]):
                 The molecule entries to update in the database.
             merge_properties:
                 If ``True``, the molecular properties will be
                 merged rather than replaced. Properties present
                 in both the update and the database will be
                 overwritten.
+            upsert:
+                If ``True``, entries will be added to the
+                database if missing.
             commit:
                 If ``True`` changes will be automatically
                 commited to the database file.
         """
         if isinstance(entries, Entry):
             entries = (entries,)
 
-        if merge_properties:
-            self.connection.executemany(
-                f"UPDATE {self._molecule_table} "
-                "SET molecule=:molecule, "
-                "properties=json_patch(properties,:properties) "
-                "WHERE key=:key",
-                map(_entry_to_sqlite, entries),
-            )
+        if upsert:
+            if merge_properties:
+                self.connection.executemany(
+                    f"INSERT INTO {self._molecule_table} "
+                    "VALUES (:key, :molecule, :properties) "
+                    "ON CONFLICT(key) DO UPDATE "
+                    "SET molecule=:molecule, "
+                    "properties=json_patch(properties,:properties) "
+                    "WHERE key=:key",
+                    map(_entry_to_sqlite, entries),
+                )
+            else:
+                self.connection.executemany(
+                    f"INSERT INTO {self._molecule_table} "
+                    "VALUES (:key, :molecule, :properties) "
+                    "ON CONFLICT(key) DO UPDATE "
+                    "SET molecule=:molecule, properties=:properties "
+                    "WHERE key=:key",
+                    map(_entry_to_sqlite, entries),
+                )
         else:
-            self.connection.executemany(
-                f"UPDATE {self._molecule_table} "
-                "SET molecule=:molecule, properties=:properties "
-                "WHERE key=:key",
-                map(_entry_to_sqlite, entries),
-            )
+            if merge_properties:
+                self.connection.executemany(
+                    f"UPDATE {self._molecule_table} "
+                    "SET molecule=:molecule, "
+                    "properties=json_patch(properties,:properties) "
+                    "WHERE key=:key",
+                    map(_entry_to_sqlite, entries),
+                )
+            else:
+                self.connection.executemany(
+                    f"UPDATE {self._molecule_table} "
+                    "SET molecule=:molecule, properties=:properties "
+                    "WHERE key=:key",
+                    map(_entry_to_sqlite, entries),
+                )
         if commit:
             self.connection.commit()
 
     def get_entries(
         self,
         keys: str | collections.abc.Iterable[str] | None = None,
     ) -> collections.abc.Iterator[Entry]:
```

### Comparing `atomlite-1.3.2/src/atomlite/_internal/json.py` & `atomlite-2.0.0/src/atomlite/_internal/json.py`

 * *Files identical despite different names*

### Comparing `atomlite-1.3.2/src/atomlite.egg-info/PKG-INFO` & `atomlite-2.0.0/src/atomlite.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atomlite
-Version: 1.3.2
+Version: 2.0.0
 Maintainer-email: Lukas Turcani <lukasturcani93@gmail.com>
 Project-URL: github, https://github.com/lukasturcani/atomlite
 Project-URL: documentation, https://atomlite.readthedocs.io
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
```

### Comparing `atomlite-1.3.2/src/atomlite.egg-info/SOURCES.txt` & `atomlite-2.0.0/src/atomlite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atomlite-1.3.2/tests/test_database.py` & `atomlite-2.0.0/tests/test_database.py`

 * *Files 3% similar despite different names*

```diff
@@ -93,15 +93,15 @@
     )
     database.add_entries(entry1)
     entry2 = atomlite.Entry.from_rdkit(
         key="first",
         molecule=rdkit.MolFromSmiles("CC"),
         properties={"b": 32},
     )
-    database.update_entries(entry2, merge_properties=False)
+    database.update_entries(entry2, merge_properties=False, upsert=False)
     entry = next(database.get_entries("first"))
     molecule = atomlite.json_to_rdkit(entry.molecule)
     assert molecule.GetNumAtoms() == 2
     assert entry.properties == {"b": 32}
 
 
 def test_properties_get_merged_on_entry_update(
@@ -114,21 +114,60 @@
     )
     database.add_entries(entry1)
     entry2 = atomlite.Entry.from_rdkit(
         key="first",
         molecule=rdkit.MolFromSmiles("CC"),
         properties={"b": 32},
     )
-    database.update_entries(entry2)
+    database.update_entries(entry2, upsert=False)
     entry = next(database.get_entries("first"))
     molecule = atomlite.json_to_rdkit(entry.molecule)
     assert molecule.GetNumAtoms() == 2
     assert entry.properties == {"a": 12, "b": 32}
 
 
+def test_upsert(
+    database: atomlite.Database,
+) -> None:
+    entry1 = atomlite.Entry.from_rdkit(
+        key="first",
+        molecule=rdkit.MolFromSmiles("C"),
+        properties={"a": 12, "b": 10},
+    )
+    database.update_entries(entry1, upsert=False)
+    assert len(list(database.get_entries("first"))) == 0
+    database.update_entries(entry1, upsert=True)
+    (result1,) = list(database.get_entries("first"))
+    molecule1 = atomlite.json_to_rdkit(result1.molecule)
+    assert molecule1.GetNumAtoms() == 1
+    assert result1.properties == {"a": 12, "b": 10}
+
+    entry2 = atomlite.Entry.from_rdkit(
+        key="first",
+        molecule=rdkit.MolFromSmiles("CC"),
+        properties={"b": 32},
+    )
+    database.update_entries(entry2, merge_properties=True, upsert=True)
+    (result2,) = list(database.get_entries("first"))
+    molecule2 = atomlite.json_to_rdkit(result2.molecule)
+    assert molecule2.GetNumAtoms() == 2
+    assert result2.properties == {"a": 12, "b": 32}
+
+    entry3 = atomlite.Entry.from_rdkit(
+        key="first",
+        molecule=rdkit.MolFromSmiles("CCC"),
+        properties={"b": 64},
+    )
+    database.update_entries(entry3, merge_properties=False, upsert=True)
+    (result3,) = list(database.get_entries("first"))
+    molecule3 = atomlite.json_to_rdkit(result3.molecule)
+    assert molecule3.GetNumAtoms() == 3
+    assert result3.properties == {"b": 64}
+
+
 def test_properties_get_merged_on_property_update(
     database: atomlite.Database,
 ) -> None:
     entry1 = atomlite.Entry.from_rdkit(
         key="first",
         molecule=rdkit.MolFromSmiles("C"),
         properties={"a": 12, "b": 10},
```

