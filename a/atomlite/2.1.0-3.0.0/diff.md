# Comparing `tmp/atomlite-2.1.0.tar.gz` & `tmp/atomlite-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atomlite-2.1.0.tar", last modified: Mon Jul 17 19:45:00 2023, max compression
+gzip compressed data, was "atomlite-3.0.0.tar", last modified: Mon Jul 17 20:15:02 2023, max compression
```

## Comparing `atomlite-2.1.0.tar` & `atomlite-3.0.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:45:00.282393 atomlite-2.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:45:00.278393 atomlite-2.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:45:00.282393 atomlite-2.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-17 19:44:25.000000 atomlite-2.1.0/.github/workflows/publish_release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-17 19:44:25.000000 atomlite-2.1.0/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-17 19:44:25.000000 atomlite-2.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-17 19:44:25.000000 atomlite-2.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-17 19:45:00.282393 atomlite-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-17 19:44:25.000000 atomlite-2.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:45:00.282393 atomlite-2.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-17 19:44:25.000000 atomlite-2.1.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:45:00.282393 atomlite-2.1.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:45:00.282393 atomlite-2.1.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 19:44:25.000000 atomlite-2.1.0/docs/source/_static/empty
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:45:00.282393 atomlite-2.1.0/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-17 19:44:25.000000 atomlite-2.1.0/docs/source/_templates/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-17 19:44:25.000000 atomlite-2.1.0/docs/source/_templates/module.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-17 19:44:25.000000 atomlite-2.1.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    12883 2023-07-17 19:44:25.000000 atomlite-2.1.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-17 19:44:25.000000 atomlite-2.1.0/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-17 19:44:25.000000 atomlite-2.1.0/justfile
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-17 19:44:25.000000 atomlite-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 19:45:00.282393 atomlite-2.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:45:00.278393 atomlite-2.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:45:00.282393 atomlite-2.1.0/src/atomlite/
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-17 19:44:25.000000 atomlite-2.1.0/src/atomlite/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:45:00.282393 atomlite-2.1.0/src/atomlite/_internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 19:44:25.000000 atomlite-2.1.0/src/atomlite/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12637 2023-07-17 19:44:25.000000 atomlite-2.1.0/src/atomlite/_internal/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-07-17 19:44:25.000000 atomlite-2.1.0/src/atomlite/_internal/json.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 19:44:25.000000 atomlite-2.1.0/src/atomlite/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:45:00.282393 atomlite-2.1.0/src/atomlite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-17 19:45:00.000000 atomlite-2.1.0/src/atomlite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-17 19:45:00.000000 atomlite-2.1.0/src/atomlite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 19:45:00.000000 atomlite-2.1.0/src/atomlite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-17 19:45:00.000000 atomlite-2.1.0/src/atomlite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-17 19:45:00.000000 atomlite-2.1.0/src/atomlite.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:45:00.282393 atomlite-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-07-17 19:44:25.000000 atomlite-2.1.0/tests/test_database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:15:02.180237 atomlite-3.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:15:02.176237 atomlite-3.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:15:02.180237 atomlite-3.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-17 20:14:31.000000 atomlite-3.0.0/.github/workflows/publish_release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-17 20:14:31.000000 atomlite-3.0.0/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-17 20:14:31.000000 atomlite-3.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-17 20:14:31.000000 atomlite-3.0.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-17 20:15:02.180237 atomlite-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-17 20:14:31.000000 atomlite-3.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:15:02.180237 atomlite-3.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-17 20:14:31.000000 atomlite-3.0.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:15:02.180237 atomlite-3.0.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:15:02.180237 atomlite-3.0.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:14:31.000000 atomlite-3.0.0/docs/source/_static/empty
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:15:02.180237 atomlite-3.0.0/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-17 20:14:31.000000 atomlite-3.0.0/docs/source/_templates/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-17 20:14:31.000000 atomlite-3.0.0/docs/source/_templates/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-17 20:14:31.000000 atomlite-3.0.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12883 2023-07-17 20:14:31.000000 atomlite-3.0.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-17 20:14:31.000000 atomlite-3.0.0/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-17 20:14:31.000000 atomlite-3.0.0/justfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-17 20:14:31.000000 atomlite-3.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 20:15:02.180237 atomlite-3.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:15:02.176237 atomlite-3.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:15:02.180237 atomlite-3.0.0/src/atomlite/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-17 20:14:31.000000 atomlite-3.0.0/src/atomlite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:15:02.180237 atomlite-3.0.0/src/atomlite/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:14:31.000000 atomlite-3.0.0/src/atomlite/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12461 2023-07-17 20:14:31.000000 atomlite-3.0.0/src/atomlite/_internal/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-07-17 20:14:31.000000 atomlite-3.0.0/src/atomlite/_internal/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:14:31.000000 atomlite-3.0.0/src/atomlite/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:15:02.180237 atomlite-3.0.0/src/atomlite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-17 20:15:02.000000 atomlite-3.0.0/src/atomlite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-17 20:15:02.000000 atomlite-3.0.0/src/atomlite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 20:15:02.000000 atomlite-3.0.0/src/atomlite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-17 20:15:02.000000 atomlite-3.0.0/src/atomlite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-17 20:15:02.000000 atomlite-3.0.0/src/atomlite.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:15:02.180237 atomlite-3.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-07-17 20:14:31.000000 atomlite-3.0.0/tests/test_database.py
```

### Comparing `atomlite-2.1.0/.github/workflows/publish_release.yaml` & `atomlite-3.0.0/.github/workflows/publish_release.yaml`

 * *Files identical despite different names*

### Comparing `atomlite-2.1.0/.github/workflows/tests.yaml` & `atomlite-3.0.0/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `atomlite-2.1.0/PKG-INFO` & `atomlite-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atomlite
-Version: 2.1.0
+Version: 3.0.0
 Maintainer-email: Lukas Turcani <lukasturcani93@gmail.com>
 Project-URL: github, https://github.com/lukasturcani/atomlite
 Project-URL: documentation, https://atomlite.readthedocs.io
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
```

### Comparing `atomlite-2.1.0/README.rst` & `atomlite-3.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `atomlite-2.1.0/docs/Makefile` & `atomlite-3.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `atomlite-2.1.0/docs/source/_templates/class.rst` & `atomlite-3.0.0/docs/source/_templates/class.rst`

 * *Files identical despite different names*

### Comparing `atomlite-2.1.0/docs/source/_templates/module.rst` & `atomlite-3.0.0/docs/source/_templates/module.rst`

 * *Files identical despite different names*

### Comparing `atomlite-2.1.0/docs/source/conf.py` & `atomlite-3.0.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `atomlite-2.1.0/docs/source/index.rst` & `atomlite-3.0.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `atomlite-2.1.0/justfile` & `atomlite-3.0.0/justfile`

 * *Files identical despite different names*

### Comparing `atomlite-2.1.0/pyproject.toml` & `atomlite-3.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `atomlite-2.1.0/src/atomlite/_internal/database.py` & `atomlite-3.0.0/src/atomlite/_internal/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,22 +81,14 @@
 
 def _property_entry_to_sqlite(entry: PropertyEntry) -> dict[str, Json]:
     d = asdict(entry)
     d["properties"] = json.dumps(d["properties"])
     return d
 
 
-class MoleculeNotFound(Exception):
-    """
-    Raised when a molecule is not found in the database.
-    """
-
-    pass
-
-
 class Database:
     """
     A molecular SQLite database.
     """
 
     connection: sqlite3.Connection
     """
@@ -278,39 +270,37 @@
             value is returned for a missing value as well as an
             exisiting value set to ``None``. If you need to
             distinguish between missing and ``None`` values you
             can use a different value to represent missing data,
             for example the string ``"MISSING"``.
 
         Parameters:
-            key: The key of the molecule.
+            key:
+                The key of the molecule.
             path:
                 A path to the property of the molecule. Valid
                 paths are described here_. You can also view various
                 code :ref:`examples<examples-valid-property-paths>`
                 in our docs.
         Returns:
-            The property.
-        Raises:
-            MoleculeNotFound:
-                If the molecule is not found in the database.
+            The property. ``None`` will be returned if `key`
+            is not present in the database or `path` leads to
+            a non-existent property.
 
         .. _here: https://www.sqlite.org/json1.html#path_arguments
         """
         result = self.connection.execute(
             "SELECT json_extract(properties,?), "
             "json_type(properties,?) "
             f"FROM {self._molecule_table} "
             "WHERE key=?",
             (path, path, key),
         ).fetchone()
         if result is None:
-            raise MoleculeNotFound(
-                "Can't get property of a molecule not in the database."
-            )
+            return None
         property, property_type = result
         if property_type == "object" or property_type == "array":
             return json.loads(property)
         elif property_type == "true" or property_type == "false":
             return bool(property)
         else:
             return property
```

### Comparing `atomlite-2.1.0/src/atomlite/_internal/json.py` & `atomlite-3.0.0/src/atomlite/_internal/json.py`

 * *Files identical despite different names*

### Comparing `atomlite-2.1.0/src/atomlite.egg-info/PKG-INFO` & `atomlite-3.0.0/src/atomlite.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atomlite
-Version: 2.1.0
+Version: 3.0.0
 Maintainer-email: Lukas Turcani <lukasturcani93@gmail.com>
 Project-URL: github, https://github.com/lukasturcani/atomlite
 Project-URL: documentation, https://atomlite.readthedocs.io
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
```

### Comparing `atomlite-2.1.0/src/atomlite.egg-info/SOURCES.txt` & `atomlite-3.0.0/src/atomlite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atomlite-2.1.0/tests/test_database.py` & `atomlite-3.0.0/tests/test_database.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,16 +51,15 @@
     database.add_entries(entry)
     assert database.get_property("first", "$.a.not_here") is None
 
 
 def test_get_property_from_missing_molecule(
     database: atomlite.Database,
 ) -> None:
-    with pytest.raises(atomlite.MoleculeNotFound):
-        database.get_property("first", "$.a.a")
+    assert database.get_property("first", "$.a.a") is None
 
 
 def test_get_property(database: atomlite.Database) -> None:
     entry = atomlite.Entry.from_rdkit(
         key="first",
         molecule=rdkit.MolFromSmiles("C"),
         properties={
```

