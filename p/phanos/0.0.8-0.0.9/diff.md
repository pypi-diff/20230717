# Comparing `tmp/phanos-0.0.8.tar.gz` & `tmp/phanos-0.0.9.tar.gz`

## Comparing `phanos-0.0.8.tar` & `phanos-0.0.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 phanos-0.0.8/CHANGELOG.md
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 phanos-0.0.8/Pipfile
--rw-r--r--   0        0        0    22933 2020-02-02 00:00:00.000000 phanos-0.0.8/Pipfile.lock
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 phanos-0.0.8/requirements.txt
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 phanos-0.0.8/deactivate/pyvenv.cfg
--rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 phanos-0.0.8/deactivate/bin/Activate.ps1
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 phanos-0.0.8/deactivate/bin/activate
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 phanos-0.0.8/deactivate/bin/activate.csh
--rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 phanos-0.0.8/deactivate/bin/activate.fish
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.8/deactivate/bin/pip
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.8/deactivate/bin/pip3
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.8/deactivate/bin/pip3.10
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.8/deactivate/bin/pip3.11
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.0.8/deactivate/bin/python -> python3.11
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.0.8/deactivate/bin/python3 -> python3.11
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.0.8/deactivate/bin/python3.11 -> /usr/bin/python3.11
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 phanos-0.0.8/src/phanos/__init__.py
--rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 phanos-0.0.8/src/phanos/log.py
--rw-r--r--   0        0        0    17210 2020-02-02 00:00:00.000000 phanos-0.0.8/src/phanos/metrics.py
--rw-r--r--   0        0        0    16975 2020-02-02 00:00:00.000000 phanos-0.0.8/src/phanos/publisher.py
--rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 phanos-0.0.8/src/phanos/tree.py
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 phanos-0.0.8/test/__init__.py
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 phanos-0.0.8/test/dummy_api.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 phanos-0.0.8/test/requirements.txt
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 phanos-0.0.8/test/run_tests.py
--rw-r--r--   0        0        0    20704 2020-02-02 00:00:00.000000 phanos-0.0.8/test/test_metric.py
--rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 phanos-0.0.8/test/testing_data.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 phanos-0.0.8/.gitignore
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 phanos-0.0.8/LICENSE
--rw-r--r--   0        0        0     4631 2020-02-02 00:00:00.000000 phanos-0.0.8/README.md
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 phanos-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     5361 2020-02-02 00:00:00.000000 phanos-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 phanos-0.0.9/CHANGELOG.md
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 phanos-0.0.9/Pipfile
+-rw-r--r--   0        0        0    22933 2020-02-02 00:00:00.000000 phanos-0.0.9/Pipfile.lock
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 phanos-0.0.9/requirements.txt
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 phanos-0.0.9/deactivate/pyvenv.cfg
+-rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 phanos-0.0.9/deactivate/bin/Activate.ps1
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 phanos-0.0.9/deactivate/bin/activate
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 phanos-0.0.9/deactivate/bin/activate.csh
+-rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 phanos-0.0.9/deactivate/bin/activate.fish
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.9/deactivate/bin/pip
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.9/deactivate/bin/pip3
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.9/deactivate/bin/pip3.10
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.9/deactivate/bin/pip3.11
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.0.9/deactivate/bin/python -> python3.11
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.0.9/deactivate/bin/python3 -> python3.11
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.0.9/deactivate/bin/python3.11 -> /usr/bin/python3.11
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 phanos-0.0.9/src/phanos/__init__.py
+-rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 phanos-0.0.9/src/phanos/log.py
+-rw-r--r--   0        0        0    17085 2020-02-02 00:00:00.000000 phanos-0.0.9/src/phanos/metrics.py
+-rw-r--r--   0        0        0    17201 2020-02-02 00:00:00.000000 phanos-0.0.9/src/phanos/publisher.py
+-rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 phanos-0.0.9/src/phanos/tree.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 phanos-0.0.9/test/__init__.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 phanos-0.0.9/test/dummy_api.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 phanos-0.0.9/test/requirements.txt
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 phanos-0.0.9/test/run_tests.py
+-rw-r--r--   0        0        0    20704 2020-02-02 00:00:00.000000 phanos-0.0.9/test/test_metric.py
+-rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 phanos-0.0.9/test/testing_data.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 phanos-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 phanos-0.0.9/LICENSE
+-rw-r--r--   0        0        0     4631 2020-02-02 00:00:00.000000 phanos-0.0.9/README.md
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 phanos-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     5361 2020-02-02 00:00:00.000000 phanos-0.0.9/PKG-INFO
```

### Comparing `phanos-0.0.8/Pipfile.lock` & `phanos-0.0.9/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `phanos-0.0.8/deactivate/bin/Activate.ps1` & `phanos-0.0.9/deactivate/bin/Activate.ps1`

 * *Files identical despite different names*

### Comparing `phanos-0.0.8/deactivate/bin/activate` & `phanos-0.0.9/deactivate/bin/activate`

 * *Files identical despite different names*

### Comparing `phanos-0.0.8/deactivate/bin/activate.csh` & `phanos-0.0.9/deactivate/bin/activate.csh`

 * *Files identical despite different names*

### Comparing `phanos-0.0.8/deactivate/bin/activate.fish` & `phanos-0.0.9/deactivate/bin/activate.fish`

 * *Files identical despite different names*

### Comparing `phanos-0.0.8/src/phanos/log.py` & `phanos-0.0.9/src/phanos/log.py`

 * *Files identical despite different names*

### Comparing `phanos-0.0.8/src/phanos/metrics.py` & `phanos-0.0.9/src/phanos/metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,17 +140,14 @@
                     f"{self.store_operation.__qualname__}: expected labels: {self.label_names}, "
                     f"labels given: {label_values.keys()}"
                 )
                 raise ValueError("Unknown or missing label")
             if operation is None:
                 operation = self.default_operation
             self.method.append(method)
-            self.debug(
-                "metric %s stored operation %s, value %s", self.name, operation, value
-            )
             self.operations[operation](value, args, kwargs)
         except KeyError as exc:
             self.error(
                 f"{self.store_operation.__qualname__}: operation {operation} unknown."
                 f"Known operations: {self.operations.keys()}"
             )
             raise ValueError("Unknown operation") from exc
```

### Comparing `phanos-0.0.8/src/phanos/publisher.py` & `phanos-0.0.9/src/phanos/publisher.py`

 * *Files 2% similar despite different names*

```diff
@@ -423,15 +423,15 @@
             if self._handlers and self.handle_records:
                 self.debug("after func execution")
                 self._after_func(*args, **kwargs)
 
                 if self.current_node.parent == self._root:
                     self.debug("after root execution")
                     self._after_root_func(*args, **kwargs)
-                    self.handle_records_clear()
+                    self._handle_records_clear()
 
                 self.current_node = self.current_node.parent
                 self.current_node.delete_child()
             return result
 
         return inner
 
@@ -477,18 +477,24 @@
             self.time_profile.store_operation(
                 operation="stop", method=self.current_node.context, label_values={}
             )
         # users custom metrics operation recording
         if callable(self.after_func):
             self.after_func(fn_result=fn_result, *args, **kwargs)
 
-    def handle_records_clear(self) -> None:
+    def _handle_records_clear(self) -> None:
         """Pass records to each registered Handler and clear stored records"""
         # send records and log em
         for metric in self._metrics.values():
             records = metric.to_records()
             for handler in self._handlers.values():
                 self.debug(
                     f"handler %s handling metric %s", handler.handler_name, metric.name
                 )
                 handler.handle(records, metric.name)
             metric.cleanup()
+
+    def force_handle_records_clear(self) -> None:
+        """Method to force records handling with Method tree clear"""
+        # send records and log em
+        self._handle_records_clear()
+        self._root.clear_tree()
```

### Comparing `phanos-0.0.8/src/phanos/tree.py` & `phanos-0.0.9/src/phanos/tree.py`

 * *Files identical despite different names*

### Comparing `phanos-0.0.8/test/dummy_api.py` & `phanos-0.0.9/test/dummy_api.py`

 * *Files identical despite different names*

### Comparing `phanos-0.0.8/test/run_tests.py` & `phanos-0.0.9/test/run_tests.py`

 * *Files identical despite different names*

### Comparing `phanos-0.0.8/test/test_metric.py` & `phanos-0.0.9/test/test_metric.py`

 * *Files identical despite different names*

### Comparing `phanos-0.0.8/test/testing_data.py` & `phanos-0.0.9/test/testing_data.py`

 * *Files identical despite different names*

### Comparing `phanos-0.0.8/.gitignore` & `phanos-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `phanos-0.0.8/LICENSE` & `phanos-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `phanos-0.0.8/README.md` & `phanos-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `phanos-0.0.8/pyproject.toml` & `phanos-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "phanos"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Miroslav Bulička", email="bulickamiroslav@gmail.com" },
 ]
 description = "Python client to gather data for Prometheus logging in server with multiple instances and workers."
 readme = "README.md"
 requires-python = ">=3.10.6"
 classifiers = [
```

### Comparing `phanos-0.0.8/PKG-INFO` & `phanos-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phanos
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python client to gather data for Prometheus logging in server with multiple instances and workers.
 Project-URL: Homepage, https://github.com/kajotgames/phanos
 Project-URL: Bug Tracker, https://github.com/kajotgames/phanos/issues
 Author-email: Miroslav Bulička <bulickamiroslav@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

