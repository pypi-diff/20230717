# Comparing `tmp/discovery-core-0.2.6.tar.gz` & `tmp/discovery-core-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discovery-core-0.2.6.tar", last modified: Sun Jul 16 00:03:08 2023, max compression
+gzip compressed data, was "discovery-core-0.2.7.tar", last modified: Mon Jul 17 17:37:25 2023, max compression
```

## Comparing `discovery-core-0.2.6.tar` & `discovery-core-0.2.7.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-16 00:03:08.929862 discovery-core-0.2.6/
--rwxr-xr-x   0 doatridge   (503) staff       (20)     1087 2023-06-28 23:35:32.000000 discovery-core-0.2.6/LICENSE.txt
--rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2023-06-28 23:35:32.000000 discovery-core-0.2.6/MANIFEST.in
--rw-r--r--   0 doatridge   (503) staff       (20)    14094 2023-07-16 00:03:08.930166 discovery-core-0.2.6/PKG-INFO
--rw-r--r--   0 doatridge   (503) staff       (20)    13130 2023-06-28 23:35:32.000000 discovery-core-0.2.6/README.rst
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-16 00:03:08.908328 discovery-core-0.2.6/discovery_core.egg-info/
--rw-r--r--   0 doatridge   (503) staff       (20)    14094 2023-07-16 00:03:08.000000 discovery-core-0.2.6/discovery_core.egg-info/PKG-INFO
--rw-r--r--   0 doatridge   (503) staff       (20)     1092 2023-07-16 00:03:08.000000 discovery-core-0.2.6/discovery_core.egg-info/SOURCES.txt
--rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-07-16 00:03:08.000000 discovery-core-0.2.6/discovery_core.egg-info/dependency_links.txt
--rw-r--r--   0 doatridge   (503) staff       (20)       13 2023-07-16 00:03:08.000000 discovery-core-0.2.6/discovery_core.egg-info/top_level.txt
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-16 00:03:08.908677 discovery-core-0.2.6/ds_core/
--rw-r--r--   0 doatridge   (503) staff       (20)       73 2023-07-13 23:49:08.000000 discovery-core-0.2.6/ds_core/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-16 00:03:08.910804 discovery-core-0.2.6/ds_core/components/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.6/ds_core/components/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    63342 2023-06-29 23:15:54.000000 discovery-core-0.2.6/ds_core/components/abstract_component.py
--rw-r--r--   0 doatridge   (503) staff       (20)    23605 2023-07-15 23:59:50.000000 discovery-core-0.2.6/ds_core/components/core_commons.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-16 00:03:08.912785 discovery-core-0.2.6/ds_core/handlers/
--rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.6/ds_core/handlers/__init__.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    15258 2023-05-02 21:09:52.000000 discovery-core-0.2.6/ds_core/handlers/abstract_handlers.py
--rw-r--r--   0 doatridge   (503) staff       (20)     7794 2023-06-29 15:03:02.000000 discovery-core-0.2.6/ds_core/handlers/pyarrow_handlers.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-16 00:03:08.913716 discovery-core-0.2.6/ds_core/intent/
--rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.6/ds_core/intent/__init__.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    11255 2023-06-29 15:15:01.000000 discovery-core-0.2.6/ds_core/intent/abstract_intent.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-16 00:03:08.917162 discovery-core-0.2.6/ds_core/properties/
--rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.6/ds_core/properties/__init__.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    65710 2023-06-29 23:15:54.000000 discovery-core-0.2.6/ds_core/properties/abstract_properties.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)     2996 2022-09-22 17:31:08.000000 discovery-core-0.2.6/ds_core/properties/decorator_patterns.py
--rw-r--r--   0 doatridge   (503) staff       (20)    11271 2023-06-29 15:15:01.000000 discovery-core-0.2.6/ds_core/properties/property_manager.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)      110 2023-07-16 00:03:08.931268 discovery-core-0.2.6/setup.cfg
--rwxr-xr-x   0 doatridge   (503) staff       (20)     2085 2023-07-03 17:06:43.000000 discovery-core-0.2.6/setup.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-16 00:03:08.918145 discovery-core-0.2.6/test/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-29 15:06:28.000000 discovery-core-0.2.6/test/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-16 00:03:08.920357 discovery-core-0.2.6/test/components/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.6/test/components/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    31492 2023-06-29 16:42:17.000000 discovery-core-0.2.6/test/components/abstract_component_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)    15078 2023-07-13 23:46:04.000000 discovery-core-0.2.6/test/components/commons_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-16 00:03:08.923220 discovery-core-0.2.6/test/handlers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.6/test/handlers/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    11054 2023-06-29 16:24:13.000000 discovery-core-0.2.6/test/handlers/connector_contract_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2560 2023-06-29 16:24:13.000000 discovery-core-0.2.6/test/handlers/handler_factory_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-16 00:03:08.925752 discovery-core-0.2.6/test/intent/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.6/test/intent/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2899 2023-07-12 16:01:36.000000 discovery-core-0.2.6/test/intent/abstract_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     7100 2023-07-12 17:46:55.000000 discovery-core-0.2.6/test/intent/pyarrow_intent_model.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-16 00:03:08.929010 discovery-core-0.2.6/test/properties/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.6/test/properties/__init__.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    36169 2023-06-29 23:15:54.000000 discovery-core-0.2.6/test/properties/abstract_properties_manager_test.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)     9513 2023-06-29 16:47:52.000000 discovery-core-0.2.6/test/properties/property_manager_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-17 17:37:25.761008 discovery-core-0.2.7/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     1087 2023-06-28 23:35:32.000000 discovery-core-0.2.7/LICENSE.txt
+-rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2023-06-28 23:35:32.000000 discovery-core-0.2.7/MANIFEST.in
+-rw-r--r--   0 doatridge   (503) staff       (20)    14094 2023-07-17 17:37:25.761218 discovery-core-0.2.7/PKG-INFO
+-rw-r--r--   0 doatridge   (503) staff       (20)    13130 2023-06-28 23:35:32.000000 discovery-core-0.2.7/README.rst
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-17 17:37:25.743692 discovery-core-0.2.7/discovery_core.egg-info/
+-rw-r--r--   0 doatridge   (503) staff       (20)    14094 2023-07-17 17:37:25.000000 discovery-core-0.2.7/discovery_core.egg-info/PKG-INFO
+-rw-r--r--   0 doatridge   (503) staff       (20)     1092 2023-07-17 17:37:25.000000 discovery-core-0.2.7/discovery_core.egg-info/SOURCES.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-07-17 17:37:25.000000 discovery-core-0.2.7/discovery_core.egg-info/dependency_links.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)       13 2023-07-17 17:37:25.000000 discovery-core-0.2.7/discovery_core.egg-info/top_level.txt
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-17 17:37:25.744058 discovery-core-0.2.7/ds_core/
+-rw-r--r--   0 doatridge   (503) staff       (20)       73 2023-07-16 00:04:59.000000 discovery-core-0.2.7/ds_core/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-17 17:37:25.746011 discovery-core-0.2.7/ds_core/components/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.7/ds_core/components/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    63342 2023-06-29 23:15:54.000000 discovery-core-0.2.7/ds_core/components/abstract_component.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    23605 2023-07-15 23:59:50.000000 discovery-core-0.2.7/ds_core/components/core_commons.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-17 17:37:25.749111 discovery-core-0.2.7/ds_core/handlers/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.7/ds_core/handlers/__init__.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    15258 2023-05-02 21:09:52.000000 discovery-core-0.2.7/ds_core/handlers/abstract_handlers.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     8119 2023-07-17 16:50:51.000000 discovery-core-0.2.7/ds_core/handlers/pyarrow_handlers.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-17 17:37:25.749775 discovery-core-0.2.7/ds_core/intent/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.7/ds_core/intent/__init__.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    11255 2023-06-29 15:15:01.000000 discovery-core-0.2.7/ds_core/intent/abstract_intent.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-17 17:37:25.752552 discovery-core-0.2.7/ds_core/properties/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.7/ds_core/properties/__init__.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    65710 2023-06-29 23:15:54.000000 discovery-core-0.2.7/ds_core/properties/abstract_properties.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     2996 2022-09-22 17:31:08.000000 discovery-core-0.2.7/ds_core/properties/decorator_patterns.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11271 2023-06-29 15:15:01.000000 discovery-core-0.2.7/ds_core/properties/property_manager.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)      110 2023-07-17 17:37:25.762208 discovery-core-0.2.7/setup.cfg
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     2085 2023-07-03 17:06:43.000000 discovery-core-0.2.7/setup.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-17 17:37:25.753194 discovery-core-0.2.7/test/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-29 15:06:28.000000 discovery-core-0.2.7/test/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-17 17:37:25.754907 discovery-core-0.2.7/test/components/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.7/test/components/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    31492 2023-06-29 16:42:17.000000 discovery-core-0.2.7/test/components/abstract_component_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    15078 2023-07-13 23:46:04.000000 discovery-core-0.2.7/test/components/commons_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-17 17:37:25.756523 discovery-core-0.2.7/test/handlers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.7/test/handlers/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11054 2023-06-29 16:24:13.000000 discovery-core-0.2.7/test/handlers/connector_contract_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2560 2023-06-29 16:24:13.000000 discovery-core-0.2.7/test/handlers/handler_factory_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-17 17:37:25.758094 discovery-core-0.2.7/test/intent/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.7/test/intent/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2899 2023-07-12 16:01:36.000000 discovery-core-0.2.7/test/intent/abstract_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     7100 2023-07-12 17:46:55.000000 discovery-core-0.2.7/test/intent/pyarrow_intent_model.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-17 17:37:25.760368 discovery-core-0.2.7/test/properties/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.7/test/properties/__init__.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    36169 2023-06-29 23:15:54.000000 discovery-core-0.2.7/test/properties/abstract_properties_manager_test.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     9513 2023-06-29 16:47:52.000000 discovery-core-0.2.7/test/properties/property_manager_test.py
```

### Comparing `discovery-core-0.2.6/LICENSE.txt` & `discovery-core-0.2.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.6/PKG-INFO` & `discovery-core-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-core
-Version: 0.2.6
+Version: 0.2.7
 Summary: Augmented Intent Single Task Adaptive Components
 Home-page: http://github.com/gigas64/discovery-core
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Foundation SDK Machine learning AI component intent data science
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-core-0.2.6/README.rst` & `discovery-core-0.2.7/README.rst`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.6/discovery_core.egg-info/PKG-INFO` & `discovery-core-0.2.7/discovery_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-core
-Version: 0.2.6
+Version: 0.2.7
 Summary: Augmented Intent Single Task Adaptive Components
 Home-page: http://github.com/gigas64/discovery-core
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Foundation SDK Machine learning AI component intent data science
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-core-0.2.6/discovery_core.egg-info/SOURCES.txt` & `discovery-core-0.2.7/discovery_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.6/ds_core/components/abstract_component.py` & `discovery-core-0.2.7/ds_core/components/abstract_component.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.6/ds_core/components/core_commons.py` & `discovery-core-0.2.7/ds_core/components/core_commons.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.6/ds_core/handlers/abstract_handlers.py` & `discovery-core-0.2.7/ds_core/handlers/abstract_handlers.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.6/ds_core/handlers/pyarrow_handlers.py` & `discovery-core-0.2.7/ds_core/handlers/pyarrow_handlers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import ast
 import os
 import pyarrow as pa
 import pyarrow.parquet as pq
 import pyarrow.feather as feather
 from pyarrow import csv
 from pyarrow import json
 
@@ -43,19 +44,25 @@
         # parquet
         if file_type.lower() in ['parquet', 'pqt', 'pq']:
             return pq.read_table(address, **load_params)
         # feathers
         if file_type.lower() in ['feather']:
             return feather.read_table(address, **load_params)
         # csv
-        if file_type.lower() in ['gzip', 'zip', 'tar', 'csv', 'tsv', 'txt']:
+        if file_type.lower() in ['csv']:
             return csv.read_csv(address, **load_params)
         # json
         if file_type.lower() in ['json']:
             return json.read_json(address, **load_params)
+        # complex nested
+        if file_type.lower() in ['txt']:
+            with open(address) as f:
+                document = ast.literal_eval(f.read())
+            return pa.Table.from_pylist(document)
+
         raise LookupError('The source format {} is not currently supported'.format(file_type))
 
     def exists(self) -> bool:
         """ Returns True is the file exists """
         if not isinstance(self.connector_contract, ConnectorContract):
             raise ValueError("The Pandas Connector Contract has not been set")
         _cc = self.connector_contract
@@ -140,17 +147,21 @@
             pq.write_table(canonical, _address, **write_params)
             return True
         # feather
         if file_type.lower() in ['feather']:
             feather.write_feather(canonical, _address, **write_params)
             return True
         # csv
-        if file_type.lower() in ['csv', 'tsv', 'txt']:
+        if file_type.lower() in ['csv', 'tsv']:
             csv.write_csv(canonical, _address, **write_params)
             return True
+        # complex nested
+        if file_type.lower() in ['txt']:
+            with open(_address, 'w') as f:
+                f.write(str(canonical))
         # not found
         raise LookupError('The file format {} is not currently supported for write'.format(file_type))
 
     def remove_canonical(self) -> bool:
         if not isinstance(self.connector_contract, ConnectorContract):
             return False
         _cc = self.connector_contract
```

### Comparing `discovery-core-0.2.6/ds_core/intent/abstract_intent.py` & `discovery-core-0.2.7/ds_core/intent/abstract_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.6/ds_core/properties/abstract_properties.py` & `discovery-core-0.2.7/ds_core/properties/abstract_properties.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.6/ds_core/properties/decorator_patterns.py` & `discovery-core-0.2.7/ds_core/properties/decorator_patterns.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.6/ds_core/properties/property_manager.py` & `discovery-core-0.2.7/ds_core/properties/property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.6/setup.py` & `discovery-core-0.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.6/test/components/abstract_component_test.py` & `discovery-core-0.2.7/test/components/abstract_component_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.6/test/components/commons_test.py` & `discovery-core-0.2.7/test/components/commons_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.6/test/handlers/connector_contract_test.py` & `discovery-core-0.2.7/test/handlers/connector_contract_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.6/test/handlers/handler_factory_test.py` & `discovery-core-0.2.7/test/handlers/handler_factory_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.6/test/intent/abstract_intent_test.py` & `discovery-core-0.2.7/test/intent/abstract_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.6/test/intent/pyarrow_intent_model.py` & `discovery-core-0.2.7/test/intent/pyarrow_intent_model.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.6/test/properties/abstract_properties_manager_test.py` & `discovery-core-0.2.7/test/properties/abstract_properties_manager_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.6/test/properties/property_manager_test.py` & `discovery-core-0.2.7/test/properties/property_manager_test.py`

 * *Files identical despite different names*

