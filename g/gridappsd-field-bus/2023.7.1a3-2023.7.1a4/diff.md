# Comparing `tmp/gridappsd_field_bus-2023.7.1a3.tar.gz` & `tmp/gridappsd_field_bus-2023.7.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridappsd_field_bus-2023.7.1a3.tar", max compression
+gzip compressed data, was "gridappsd_field_bus-2023.7.1a4.tar", max compression
```

## Comparing `gridappsd_field_bus-2023.7.1a3.tar` & `gridappsd_field_bus-2023.7.1a4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2023-07-17 05:57:42.254320 gridappsd_field_bus-2023.7.1a3/README.md
--rw-r--r--   0        0        0        0 2023-07-17 05:57:42.254320 gridappsd_field_bus-2023.7.1a3/gridappsd/__no_init__here
--rw-r--r--   0        0        0      227 2023-07-17 05:57:42.254320 gridappsd_field_bus-2023.7.1a3/gridappsd/field_interface/__init__.py
--rw-r--r--   0        0        0      280 2023-07-17 05:57:42.254320 gridappsd_field_bus-2023.7.1a3/gridappsd/field_interface/agents/__init__.py
--rw-r--r--   0        0        0    14992 2023-07-17 05:57:42.254320 gridappsd_field_bus-2023.7.1a3/gridappsd/field_interface/agents/agents.py
--rw-r--r--   0        0        0     2034 2023-07-17 05:57:42.254320 gridappsd_field_bus-2023.7.1a3/gridappsd/field_interface/context.py
--rw-r--r--   0        0        0     1856 2023-07-17 05:57:42.254320 gridappsd_field_bus-2023.7.1a3/gridappsd/field_interface/gridappsd_field_bus.py
--rw-r--r--   0        0        0     7538 2023-07-17 05:57:42.254320 gridappsd_field_bus-2023.7.1a3/gridappsd/field_interface/interfaces.py
--rw-r--r--   0        0        0      892 2023-07-17 05:58:43.770271 gridappsd_field_bus-2023.7.1a3/pyproject.toml
--rw-r--r--   0        0        0      866 1970-01-01 00:00:00.000000 gridappsd_field_bus-2023.7.1a3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-17 07:32:46.754521 gridappsd_field_bus-2023.7.1a4/README.md
+-rw-r--r--   0        0        0        0 2023-07-17 07:32:46.754521 gridappsd_field_bus-2023.7.1a4/gridappsd/__no_init__here
+-rw-r--r--   0        0        0      227 2023-07-17 07:32:46.754521 gridappsd_field_bus-2023.7.1a4/gridappsd/field_interface/__init__.py
+-rw-r--r--   0        0        0      280 2023-07-17 07:32:46.754521 gridappsd_field_bus-2023.7.1a4/gridappsd/field_interface/agents/__init__.py
+-rw-r--r--   0        0        0    14998 2023-07-17 07:32:46.754521 gridappsd_field_bus-2023.7.1a4/gridappsd/field_interface/agents/agents.py
+-rw-r--r--   0        0        0     2034 2023-07-17 07:32:46.754521 gridappsd_field_bus-2023.7.1a4/gridappsd/field_interface/context.py
+-rw-r--r--   0        0        0     1856 2023-07-17 07:32:46.754521 gridappsd_field_bus-2023.7.1a4/gridappsd/field_interface/gridappsd_field_bus.py
+-rw-r--r--   0        0        0     7538 2023-07-17 07:32:46.754521 gridappsd_field_bus-2023.7.1a4/gridappsd/field_interface/interfaces.py
+-rw-r--r--   0        0        0      892 2023-07-17 07:33:58.666844 gridappsd_field_bus-2023.7.1a4/pyproject.toml
+-rw-r--r--   0        0        0      866 1970-01-01 00:00:00.000000 gridappsd_field_bus-2023.7.1a4/PKG-INFO
```

### Comparing `gridappsd_field_bus-2023.7.1a3/gridappsd/field_interface/agents/agents.py` & `gridappsd_field_bus-2023.7.1a4/gridappsd/field_interface/agents/agents.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,18 +132,18 @@
             _log.debug(f"subscribing to simulation output on topic {topic}")
             self.downstream_message_bus.subscribe(topic,
                                                   self.on_simulation_output)
 
     def subscribe_to_messages(self):
 
         self.downstream_message_bus.subscribe(
-            t.field_message_bus_topic(self.downstream_message_bus),
+            t.field_message_bus_topic(self.downstream_message_bus.id),
             self.on_downstream_message)
         self.upstream_message_bus.subscribe(
-            t.field_message_bus_topic(self.upstream_message_bus),
+            t.field_message_bus_topic(self.upstream_message_bus.id),
             self.on_upstream_message)
 
         _log.debug(
             f"Subscribing to messages on application topics: \n {t.field_message_bus_app_topic(self.downstream_message_bus.id, self.app_id)} \
                                                                     \n {t.field_message_bus_app_topic(self.upstream_message_bus.id, self.app_id)}"
         )
         self.downstream_message_bus.subscribe(
```

### Comparing `gridappsd_field_bus-2023.7.1a3/gridappsd/field_interface/context.py` & `gridappsd_field_bus-2023.7.1a4/gridappsd/field_interface/context.py`

 * *Files identical despite different names*

### Comparing `gridappsd_field_bus-2023.7.1a3/gridappsd/field_interface/gridappsd_field_bus.py` & `gridappsd_field_bus-2023.7.1a4/gridappsd/field_interface/gridappsd_field_bus.py`

 * *Files identical despite different names*

### Comparing `gridappsd_field_bus-2023.7.1a3/gridappsd/field_interface/interfaces.py` & `gridappsd_field_bus-2023.7.1a4/gridappsd/field_interface/interfaces.py`

 * *Files identical despite different names*

### Comparing `gridappsd_field_bus-2023.7.1a3/pyproject.toml` & `gridappsd_field_bus-2023.7.1a4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gridappsd-field-bus"
-version = "2023.7.1a3"
+version = "2023.7.1a4"
 description = "GridAPPS-D Field Bus Implementation"
 authors = [
     "C. Allwardt <3979063+craig8@users.noreply.github.com>",
     "P. Sharma <poorva.sharma@pnnl.gov",
     "A. Fisher <andrew.fisher@pnnl.gov"
 ]
 license = "BSD-3-Clause"
@@ -20,15 +20,15 @@
 packages = [
     { include = 'gridappsd'}
 ]
 
 
 [tool.poetry.dependencies]
 python = ">=3.7.9,<4.0"
-gridappsd-python = "^2023.7.1a3"
+gridappsd-python = "^2023.7.1a4"
 cim-graph = "^2023.5.1a3"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^6.2.2"
 pytest-html = "^3.1.1"
 mock = "^4.0.3"
 docker = "^4.4.4"
```

### Comparing `gridappsd_field_bus-2023.7.1a3/PKG-INFO` & `gridappsd_field_bus-2023.7.1a4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: gridappsd-field-bus
-Version: 2023.7.1a3
+Version: 2023.7.1a4
 Summary: GridAPPS-D Field Bus Implementation
 Home-page: https://gridappsd.readthedocs.io
 License: BSD-3-Clause
 Keywords: gridappsd,grid,activmq,powergrid,simulation,library
 Author: C. Allwardt
 Author-email: 3979063+craig8@users.noreply.github.com
 Requires-Python: >=3.7.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cim-graph (>=2023.5.1a3,<2024.0.0)
-Requires-Dist: gridappsd-python (>=2023.7.1a3,<2024.0.0)
+Requires-Dist: gridappsd-python (>=2023.7.1a4,<2024.0.0)
 Project-URL: Repository, https://github.com/GRIDAPPSD/gridappsd-python
 Description-Content-Type: text/markdown
```

