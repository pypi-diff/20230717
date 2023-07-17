# Comparing `tmp/gridappsd_field_bus-2023.7.1a7.tar.gz` & `tmp/gridappsd_field_bus-2023.7.1a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridappsd_field_bus-2023.7.1a7.tar", max compression
+gzip compressed data, was "gridappsd_field_bus-2023.7.1a8.tar", max compression
```

## Comparing `gridappsd_field_bus-2023.7.1a7.tar` & `gridappsd_field_bus-2023.7.1a8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2023-07-17 08:26:10.035592 gridappsd_field_bus-2023.7.1a7/README.md
--rw-r--r--   0        0        0        0 2023-07-17 08:26:10.035592 gridappsd_field_bus-2023.7.1a7/gridappsd/__no_init__here
--rw-r--r--   0        0        0      227 2023-07-17 08:26:10.039592 gridappsd_field_bus-2023.7.1a7/gridappsd/field_interface/__init__.py
--rw-r--r--   0        0        0      280 2023-07-17 08:26:10.039592 gridappsd_field_bus-2023.7.1a7/gridappsd/field_interface/agents/__init__.py
--rw-r--r--   0        0        0    15043 2023-07-17 08:26:10.039592 gridappsd_field_bus-2023.7.1a7/gridappsd/field_interface/agents/agents.py
--rw-r--r--   0        0        0     2034 2023-07-17 08:26:10.039592 gridappsd_field_bus-2023.7.1a7/gridappsd/field_interface/context.py
--rw-r--r--   0        0        0     1856 2023-07-17 08:26:10.039592 gridappsd_field_bus-2023.7.1a7/gridappsd/field_interface/gridappsd_field_bus.py
--rw-r--r--   0        0        0     7538 2023-07-17 08:26:10.039592 gridappsd_field_bus-2023.7.1a7/gridappsd/field_interface/interfaces.py
--rw-r--r--   0        0        0      892 2023-07-17 08:27:33.872237 gridappsd_field_bus-2023.7.1a7/pyproject.toml
--rw-r--r--   0        0        0      866 1970-01-01 00:00:00.000000 gridappsd_field_bus-2023.7.1a7/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-17 08:37:41.118630 gridappsd_field_bus-2023.7.1a8/README.md
+-rw-r--r--   0        0        0        0 2023-07-17 08:37:41.118630 gridappsd_field_bus-2023.7.1a8/gridappsd/__no_init__here
+-rw-r--r--   0        0        0      227 2023-07-17 08:37:41.118630 gridappsd_field_bus-2023.7.1a8/gridappsd/field_interface/__init__.py
+-rw-r--r--   0        0        0      280 2023-07-17 08:37:41.118630 gridappsd_field_bus-2023.7.1a8/gridappsd/field_interface/agents/__init__.py
+-rw-r--r--   0        0        0    15178 2023-07-17 08:37:41.118630 gridappsd_field_bus-2023.7.1a8/gridappsd/field_interface/agents/agents.py
+-rw-r--r--   0        0        0     2034 2023-07-17 08:37:41.118630 gridappsd_field_bus-2023.7.1a8/gridappsd/field_interface/context.py
+-rw-r--r--   0        0        0     1856 2023-07-17 08:37:41.118630 gridappsd_field_bus-2023.7.1a8/gridappsd/field_interface/gridappsd_field_bus.py
+-rw-r--r--   0        0        0     7538 2023-07-17 08:37:41.118630 gridappsd_field_bus-2023.7.1a8/gridappsd/field_interface/interfaces.py
+-rw-r--r--   0        0        0      892 2023-07-17 08:38:45.747178 gridappsd_field_bus-2023.7.1a8/pyproject.toml
+-rw-r--r--   0        0        0      866 1970-01-01 00:00:00.000000 gridappsd_field_bus-2023.7.1a8/PKG-INFO
```

### Comparing `gridappsd_field_bus-2023.7.1a7/gridappsd/field_interface/agents/agents.py` & `gridappsd_field_bus-2023.7.1a8/gridappsd/field_interface/agents/agents.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,18 @@
         if self.upstream_message_bus is not None:
             self.upstream_message_bus.connect()
         if self.downstream_message_bus is not None:
             self.downstream_message_bus.connect()
         if self.downstream_message_bus is None and self.upstream_message_bus is None:
             raise ValueError(
                 "Either upstream or downstream bus must be specified!")
-            
+
+        if ('context_manager' not in self.app_id):
+            self.agent_id = "da_" + self.app_id + "_" + self.downstream_message_bus.id
+        
         if self.agent_area_dict is None:
             context = LocalContext.get_context_by_message_bus(
                 self.downstream_message_bus)
             self.agent_area_dict = context['data']
 
         self.subscribe_to_measurement()
         self.subscribe_to_messages()
```

### Comparing `gridappsd_field_bus-2023.7.1a7/gridappsd/field_interface/context.py` & `gridappsd_field_bus-2023.7.1a8/gridappsd/field_interface/context.py`

 * *Files identical despite different names*

### Comparing `gridappsd_field_bus-2023.7.1a7/gridappsd/field_interface/gridappsd_field_bus.py` & `gridappsd_field_bus-2023.7.1a8/gridappsd/field_interface/gridappsd_field_bus.py`

 * *Files identical despite different names*

### Comparing `gridappsd_field_bus-2023.7.1a7/gridappsd/field_interface/interfaces.py` & `gridappsd_field_bus-2023.7.1a8/gridappsd/field_interface/interfaces.py`

 * *Files identical despite different names*

### Comparing `gridappsd_field_bus-2023.7.1a7/pyproject.toml` & `gridappsd_field_bus-2023.7.1a8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gridappsd-field-bus"
-version = "2023.7.1a7"
+version = "2023.7.1a8"
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
-gridappsd-python = "^2023.7.1a7"
+gridappsd-python = "^2023.7.1a8"
 cim-graph = "^2023.5.1a3"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^6.2.2"
 pytest-html = "^3.1.1"
 mock = "^4.0.3"
 docker = "^4.4.4"
```

### Comparing `gridappsd_field_bus-2023.7.1a7/PKG-INFO` & `gridappsd_field_bus-2023.7.1a8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: gridappsd-field-bus
-Version: 2023.7.1a7
+Version: 2023.7.1a8
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
-Requires-Dist: gridappsd-python (>=2023.7.1a7,<2024.0.0)
+Requires-Dist: gridappsd-python (>=2023.7.1a8,<2024.0.0)
 Project-URL: Repository, https://github.com/GRIDAPPSD/gridappsd-python
 Description-Content-Type: text/markdown
```

