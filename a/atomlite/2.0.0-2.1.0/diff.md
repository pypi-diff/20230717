# Comparing `tmp/atomlite-2.0.0.tar.gz` & `tmp/atomlite-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atomlite-2.0.0.tar", last modified: Mon Jul 17 12:09:40 2023, max compression
+gzip compressed data, was "atomlite-2.1.0.tar", last modified: Mon Jul 17 19:45:00 2023, max compression
```

## Comparing `atomlite-2.0.0.tar` & `atomlite-2.1.0.tar`

### file list

```diff
@@ -1,41 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:09:40.783454 atomlite-2.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:09:40.775454 atomlite-2.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:09:40.779454 atomlite-2.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-17 12:09:09.000000 atomlite-2.0.0/.github/workflows/publish_release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-17 12:09:09.000000 atomlite-2.0.0/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-17 12:09:09.000000 atomlite-2.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-17 12:09:09.000000 atomlite-2.0.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-17 12:09:40.783454 atomlite-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-17 12:09:09.000000 atomlite-2.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:09:40.779454 atomlite-2.0.0/docker_testing_environment/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-17 12:09:09.000000 atomlite-2.0.0/docker_testing_environment/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:09:40.779454 atomlite-2.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-17 12:09:09.000000 atomlite-2.0.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:09:40.779454 atomlite-2.0.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:09:40.779454 atomlite-2.0.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 12:09:09.000000 atomlite-2.0.0/docs/source/_static/empty
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:09:40.779454 atomlite-2.0.0/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-17 12:09:09.000000 atomlite-2.0.0/docs/source/_templates/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-17 12:09:09.000000 atomlite-2.0.0/docs/source/_templates/module.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-17 12:09:09.000000 atomlite-2.0.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    12883 2023-07-17 12:09:09.000000 atomlite-2.0.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-17 12:09:09.000000 atomlite-2.0.0/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-17 12:09:09.000000 atomlite-2.0.0/justfile
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-17 12:09:09.000000 atomlite-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 12:09:40.783454 atomlite-2.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:09:40.775454 atomlite-2.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:09:40.779454 atomlite-2.0.0/src/atomlite/
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-17 12:09:09.000000 atomlite-2.0.0/src/atomlite/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:09:40.783454 atomlite-2.0.0/src/atomlite/_internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 12:09:09.000000 atomlite-2.0.0/src/atomlite/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12560 2023-07-17 12:09:09.000000 atomlite-2.0.0/src/atomlite/_internal/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-07-17 12:09:09.000000 atomlite-2.0.0/src/atomlite/_internal/json.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 12:09:09.000000 atomlite-2.0.0/src/atomlite/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:09:40.783454 atomlite-2.0.0/src/atomlite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-17 12:09:40.000000 atomlite-2.0.0/src/atomlite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-17 12:09:40.000000 atomlite-2.0.0/src/atomlite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 12:09:40.000000 atomlite-2.0.0/src/atomlite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-17 12:09:40.000000 atomlite-2.0.0/src/atomlite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-17 12:09:40.000000 atomlite-2.0.0/src/atomlite.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:09:40.783454 atomlite-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    11602 2023-07-17 12:09:09.000000 atomlite-2.0.0/tests/test_database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:45:00.282393 atomlite-2.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:45:00.278393 atomlite-2.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:45:00.282393 atomlite-2.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-17 19:44:25.000000 atomlite-2.1.0/.github/workflows/publish_release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-17 19:44:25.000000 atomlite-2.1.0/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-17 19:44:25.000000 atomlite-2.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-17 19:44:25.000000 atomlite-2.1.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-17 19:45:00.282393 atomlite-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-17 19:44:25.000000 atomlite-2.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:45:00.282393 atomlite-2.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-17 19:44:25.000000 atomlite-2.1.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:45:00.282393 atomlite-2.1.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:45:00.282393 atomlite-2.1.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 19:44:25.000000 atomlite-2.1.0/docs/source/_static/empty
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:45:00.282393 atomlite-2.1.0/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-17 19:44:25.000000 atomlite-2.1.0/docs/source/_templates/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-17 19:44:25.000000 atomlite-2.1.0/docs/source/_templates/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-17 19:44:25.000000 atomlite-2.1.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12883 2023-07-17 19:44:25.000000 atomlite-2.1.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-17 19:44:25.000000 atomlite-2.1.0/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-17 19:44:25.000000 atomlite-2.1.0/justfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-17 19:44:25.000000 atomlite-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 19:45:00.282393 atomlite-2.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:45:00.278393 atomlite-2.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:45:00.282393 atomlite-2.1.0/src/atomlite/
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-17 19:44:25.000000 atomlite-2.1.0/src/atomlite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:45:00.282393 atomlite-2.1.0/src/atomlite/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 19:44:25.000000 atomlite-2.1.0/src/atomlite/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12637 2023-07-17 19:44:25.000000 atomlite-2.1.0/src/atomlite/_internal/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-07-17 19:44:25.000000 atomlite-2.1.0/src/atomlite/_internal/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 19:44:25.000000 atomlite-2.1.0/src/atomlite/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:45:00.282393 atomlite-2.1.0/src/atomlite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-17 19:45:00.000000 atomlite-2.1.0/src/atomlite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-17 19:45:00.000000 atomlite-2.1.0/src/atomlite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 19:45:00.000000 atomlite-2.1.0/src/atomlite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-17 19:45:00.000000 atomlite-2.1.0/src/atomlite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-17 19:45:00.000000 atomlite-2.1.0/src/atomlite.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:45:00.282393 atomlite-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-07-17 19:44:25.000000 atomlite-2.1.0/tests/test_database.py
```

### Comparing `atomlite-2.0.0/.github/workflows/publish_release.yaml` & `atomlite-2.1.0/.github/workflows/publish_release.yaml`

 * *Files identical despite different names*

### Comparing `atomlite-2.0.0/.github/workflows/tests.yaml` & `atomlite-2.1.0/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `atomlite-2.0.0/PKG-INFO` & `atomlite-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atomlite
-Version: 2.0.0
+Version: 2.1.0
 Maintainer-email: Lukas Turcani <lukasturcani93@gmail.com>
 Project-URL: github, https://github.com/lukasturcani/atomlite
 Project-URL: documentation, https://atomlite.readthedocs.io
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
```

### Comparing `atomlite-2.0.0/README.rst` & `atomlite-2.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `atomlite-2.0.0/docs/Makefile` & `atomlite-2.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `atomlite-2.0.0/docs/source/_templates/class.rst` & `atomlite-2.1.0/docs/source/_templates/class.rst`

 * *Files identical despite different names*

### Comparing `atomlite-2.0.0/docs/source/_templates/module.rst` & `atomlite-2.1.0/docs/source/_templates/module.rst`

 * *Files identical despite different names*

### Comparing `atomlite-2.0.0/docs/source/conf.py` & `atomlite-2.1.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `atomlite-2.0.0/docs/source/index.rst` & `atomlite-2.1.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `atomlite-2.0.0/justfile` & `atomlite-2.1.0/justfile`

 * *Files identical despite different names*

### Comparing `atomlite-2.0.0/pyproject.toml` & `atomlite-2.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `atomlite-2.0.0/src/atomlite/_internal/database.py` & `atomlite-2.1.0/src/atomlite/_internal/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,15 @@
                 The name of the table which stores the molecules.
         """
         self._molecule_table = molecule_table
         self.connection = sqlite3.connect(database)
         self.connection.execute(
             f"CREATE TABLE IF NOT EXISTS {molecule_table}("
             "key TEXT PRIMARY KEY NOT NULL, "
-            "molecule JSON NOT NULL, "
+            "molecule JSON, "
             "properties JSON NOT NULL)",
         )
 
     def add_entries(
         self,
         entries: Entry | collections.abc.Iterable[Entry],
         commit: bool = True,
@@ -238,15 +238,16 @@
                 The keys of the molecules to retrieve from the
                 database. If ``None``, all entries will be returned.
         Yields:
             A molecular entry matching `keys`.
         """
         if keys is None:
             for key, molecule, properties in self.connection.execute(
-                f"SELECT * FROM {self._molecule_table}",
+                f"SELECT * FROM {self._molecule_table} "
+                "WHERE molecule IS NOT NULL",
             ):
                 yield Entry(
                     key=key,
                     molecule=json.loads(molecule),
                     properties=json.loads(properties),
                 )
             return
@@ -262,19 +263,15 @@
         ):
             yield Entry(
                 key=key,
                 molecule=json.loads(molecule),
                 properties=json.loads(properties),
             )
 
-    def get_property(
-        self,
-        key: str,
-        path: str,
-    ) -> "Json":
+    def get_property(self, key: str, path: str) -> "Json":
         """
         Get the property of a molecule.
 
         .. note::
 
             If `path` does not lead to a property which exists,
             ``None`` will be returned. This means that the same
@@ -324,40 +321,38 @@
         path: str,
         property: float | str | bool | None,
         commit: bool = True,
     ) -> None:
         """
         Set the property of molecule.
 
-        .. note::
-
-            If `key` does not exist in the database, this function
-            will finish successfully but it will not change the database.
-
         Parameters:
             key:
                 The key of the molecule.
             path:
                 A path to the property of the molecule. Valid
                 paths are described here_. You can also view various
                 code :ref:`examples<examples-valid-property-paths>`
                 in our docs.
             property:
                 The desired value of the property.
             commit:
                 If ``True`` changes will be automatically
                 commited to the database file.
+
+        .. _here: https://www.sqlite.org/json1.html#path_arguments
         """
         self.connection.execute(
-            f"UPDATE {self._molecule_table} "
-            "SET properties=json_set(properties,?,?) "
-            "WHERE key=?",
-            (path, property, key),
+            f"INSERT INTO {self._molecule_table} (key,properties)"
+            "VALUES (:key,json_set('{}',:path,:property)) "
+            "ON CONFLICT(key) DO UPDATE "
+            "SET properties=json_set(properties,:path,:property) "
+            "WHERE key=:key",
+            {"key": key, "path": path, "property": property},
         )
-
         if commit:
             self.connection.commit()
 
     def update_properties(
         self,
         entries: PropertyEntry | collections.abc.Iterable[PropertyEntry],
         merge_properties: bool = True,
```

### Comparing `atomlite-2.0.0/src/atomlite/_internal/json.py` & `atomlite-2.1.0/src/atomlite/_internal/json.py`

 * *Files identical despite different names*

### Comparing `atomlite-2.0.0/src/atomlite.egg-info/PKG-INFO` & `atomlite-2.1.0/src/atomlite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atomlite
-Version: 2.0.0
+Version: 2.1.0
 Maintainer-email: Lukas Turcani <lukasturcani93@gmail.com>
 Project-URL: github, https://github.com/lukasturcani/atomlite
 Project-URL: documentation, https://atomlite.readthedocs.io
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
```

### Comparing `atomlite-2.0.0/src/atomlite.egg-info/SOURCES.txt` & `atomlite-2.1.0/src/atomlite.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 .gitignore
 .readthedocs.yaml
 README.rst
 justfile
 pyproject.toml
 .github/workflows/publish_release.yaml
 .github/workflows/tests.yaml
-docker_testing_environment/Dockerfile
 docs/Makefile
 docs/source/conf.py
 docs/source/index.rst
 docs/source/modules.rst
 docs/source/_static/empty
 docs/source/_templates/class.rst
 docs/source/_templates/module.rst
```

### Comparing `atomlite-2.0.0/tests/test_database.py` & `atomlite-2.1.0/tests/test_database.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,18 @@
                 "b": 12,
             },
         },
     )
     database.add_entries(entry)
     database.set_property("first", "$.a.c", 12)
     assert database.get_property("first", "$.a.c") == 12
+    database.set_property("second", "$.d.e", "hi")
+    assert database.get_property("second", "$.d.e") == "hi"
+    (entry,) = database.get_entries()
+    assert entry.key == "first"
 
 
 def test_get_missing_property(database: atomlite.Database) -> None:
     entry = atomlite.Entry.from_rdkit(
         key="first",
         molecule=rdkit.MolFromSmiles("C"),
         properties={
```

