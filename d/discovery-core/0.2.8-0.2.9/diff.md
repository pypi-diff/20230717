# Comparing `tmp/discovery-core-0.2.8.tar.gz` & `tmp/discovery-core-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discovery-core-0.2.8.tar", last modified: Mon Jul 17 17:52:35 2023, max compression
+gzip compressed data, was "discovery-core-0.2.9.tar", last modified: Mon Jul 17 17:56:23 2023, max compression
```

## Comparing `discovery-core-0.2.8.tar` & `discovery-core-0.2.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-17 17:52:35.769205 discovery-core-0.2.8/
--rwxr-xr-x   0 doatridge   (503) staff       (20)     1087 2023-06-28 23:35:32.000000 discovery-core-0.2.8/LICENSE.txt
--rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2023-06-28 23:35:32.000000 discovery-core-0.2.8/MANIFEST.in
--rw-r--r--   0 doatridge   (503) staff       (20)    14094 2023-07-17 17:52:35.769442 discovery-core-0.2.8/PKG-INFO
--rw-r--r--   0 doatridge   (503) staff       (20)    13130 2023-06-28 23:35:32.000000 discovery-core-0.2.8/README.rst
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-17 17:52:35.750065 discovery-core-0.2.8/discovery_core.egg-info/
--rw-r--r--   0 doatridge   (503) staff       (20)    14094 2023-07-17 17:52:35.000000 discovery-core-0.2.8/discovery_core.egg-info/PKG-INFO
--rw-r--r--   0 doatridge   (503) staff       (20)     1092 2023-07-17 17:52:35.000000 discovery-core-0.2.8/discovery_core.egg-info/SOURCES.txt
--rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-07-17 17:52:35.000000 discovery-core-0.2.8/discovery_core.egg-info/dependency_links.txt
--rw-r--r--   0 doatridge   (503) staff       (20)       13 2023-07-17 17:52:35.000000 discovery-core-0.2.8/discovery_core.egg-info/top_level.txt
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-17 17:52:35.750435 discovery-core-0.2.8/ds_core/
--rw-r--r--   0 doatridge   (503) staff       (20)       73 2023-07-17 17:37:57.000000 discovery-core-0.2.8/ds_core/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-17 17:52:35.752447 discovery-core-0.2.8/ds_core/components/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.8/ds_core/components/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    63342 2023-06-29 23:15:54.000000 discovery-core-0.2.8/ds_core/components/abstract_component.py
--rw-r--r--   0 doatridge   (503) staff       (20)    23605 2023-07-15 23:59:50.000000 discovery-core-0.2.8/ds_core/components/core_commons.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-17 17:52:35.755194 discovery-core-0.2.8/ds_core/handlers/
--rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.8/ds_core/handlers/__init__.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    15258 2023-05-02 21:09:52.000000 discovery-core-0.2.8/ds_core/handlers/abstract_handlers.py
--rw-r--r--   0 doatridge   (503) staff       (20)     8150 2023-07-17 17:52:16.000000 discovery-core-0.2.8/ds_core/handlers/pyarrow_handlers.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-17 17:52:35.755976 discovery-core-0.2.8/ds_core/intent/
--rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.8/ds_core/intent/__init__.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    11255 2023-06-29 15:15:01.000000 discovery-core-0.2.8/ds_core/intent/abstract_intent.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-17 17:52:35.760639 discovery-core-0.2.8/ds_core/properties/
--rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.8/ds_core/properties/__init__.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    65710 2023-06-29 23:15:54.000000 discovery-core-0.2.8/ds_core/properties/abstract_properties.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)     2996 2022-09-22 17:31:08.000000 discovery-core-0.2.8/ds_core/properties/decorator_patterns.py
--rw-r--r--   0 doatridge   (503) staff       (20)    11271 2023-06-29 15:15:01.000000 discovery-core-0.2.8/ds_core/properties/property_manager.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)      110 2023-07-17 17:52:35.770283 discovery-core-0.2.8/setup.cfg
--rwxr-xr-x   0 doatridge   (503) staff       (20)     2085 2023-07-03 17:06:43.000000 discovery-core-0.2.8/setup.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-17 17:52:35.761589 discovery-core-0.2.8/test/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-29 15:06:28.000000 discovery-core-0.2.8/test/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-17 17:52:35.763207 discovery-core-0.2.8/test/components/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.8/test/components/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    31492 2023-06-29 16:42:17.000000 discovery-core-0.2.8/test/components/abstract_component_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)    15078 2023-07-13 23:46:04.000000 discovery-core-0.2.8/test/components/commons_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-17 17:52:35.764900 discovery-core-0.2.8/test/handlers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.8/test/handlers/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    11054 2023-06-29 16:24:13.000000 discovery-core-0.2.8/test/handlers/connector_contract_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2560 2023-06-29 16:24:13.000000 discovery-core-0.2.8/test/handlers/handler_factory_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-17 17:52:35.766463 discovery-core-0.2.8/test/intent/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.8/test/intent/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2899 2023-07-12 16:01:36.000000 discovery-core-0.2.8/test/intent/abstract_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     7100 2023-07-12 17:46:55.000000 discovery-core-0.2.8/test/intent/pyarrow_intent_model.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-17 17:52:35.768413 discovery-core-0.2.8/test/properties/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.8/test/properties/__init__.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    36169 2023-06-29 23:15:54.000000 discovery-core-0.2.8/test/properties/abstract_properties_manager_test.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)     9513 2023-06-29 16:47:52.000000 discovery-core-0.2.8/test/properties/property_manager_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-17 17:56:23.454125 discovery-core-0.2.9/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     1087 2023-06-28 23:35:32.000000 discovery-core-0.2.9/LICENSE.txt
+-rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2023-06-28 23:35:32.000000 discovery-core-0.2.9/MANIFEST.in
+-rw-r--r--   0 doatridge   (503) staff       (20)    14094 2023-07-17 17:56:23.454347 discovery-core-0.2.9/PKG-INFO
+-rw-r--r--   0 doatridge   (503) staff       (20)    13130 2023-06-28 23:35:32.000000 discovery-core-0.2.9/README.rst
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-17 17:56:23.430993 discovery-core-0.2.9/discovery_core.egg-info/
+-rw-r--r--   0 doatridge   (503) staff       (20)    14094 2023-07-17 17:56:23.000000 discovery-core-0.2.9/discovery_core.egg-info/PKG-INFO
+-rw-r--r--   0 doatridge   (503) staff       (20)     1092 2023-07-17 17:56:23.000000 discovery-core-0.2.9/discovery_core.egg-info/SOURCES.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-07-17 17:56:23.000000 discovery-core-0.2.9/discovery_core.egg-info/dependency_links.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)       13 2023-07-17 17:56:23.000000 discovery-core-0.2.9/discovery_core.egg-info/top_level.txt
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-17 17:56:23.431628 discovery-core-0.2.9/ds_core/
+-rw-r--r--   0 doatridge   (503) staff       (20)       73 2023-07-17 17:53:02.000000 discovery-core-0.2.9/ds_core/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-17 17:56:23.434335 discovery-core-0.2.9/ds_core/components/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.9/ds_core/components/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    63342 2023-06-29 23:15:54.000000 discovery-core-0.2.9/ds_core/components/abstract_component.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    23605 2023-07-15 23:59:50.000000 discovery-core-0.2.9/ds_core/components/core_commons.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-17 17:56:23.437331 discovery-core-0.2.9/ds_core/handlers/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.9/ds_core/handlers/__init__.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    15258 2023-05-02 21:09:52.000000 discovery-core-0.2.9/ds_core/handlers/abstract_handlers.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     8143 2023-07-17 17:55:59.000000 discovery-core-0.2.9/ds_core/handlers/pyarrow_handlers.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-17 17:56:23.438143 discovery-core-0.2.9/ds_core/intent/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.9/ds_core/intent/__init__.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    11255 2023-06-29 15:15:01.000000 discovery-core-0.2.9/ds_core/intent/abstract_intent.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-17 17:56:23.442822 discovery-core-0.2.9/ds_core/properties/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.9/ds_core/properties/__init__.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    65710 2023-06-29 23:15:54.000000 discovery-core-0.2.9/ds_core/properties/abstract_properties.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     2996 2022-09-22 17:31:08.000000 discovery-core-0.2.9/ds_core/properties/decorator_patterns.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11271 2023-06-29 15:15:01.000000 discovery-core-0.2.9/ds_core/properties/property_manager.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)      110 2023-07-17 17:56:23.455384 discovery-core-0.2.9/setup.cfg
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     2085 2023-07-03 17:06:43.000000 discovery-core-0.2.9/setup.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-17 17:56:23.443722 discovery-core-0.2.9/test/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-29 15:06:28.000000 discovery-core-0.2.9/test/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-17 17:56:23.445824 discovery-core-0.2.9/test/components/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.9/test/components/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    31492 2023-06-29 16:42:17.000000 discovery-core-0.2.9/test/components/abstract_component_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    15078 2023-07-13 23:46:04.000000 discovery-core-0.2.9/test/components/commons_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-17 17:56:23.448047 discovery-core-0.2.9/test/handlers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.9/test/handlers/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11054 2023-06-29 16:24:13.000000 discovery-core-0.2.9/test/handlers/connector_contract_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2560 2023-06-29 16:24:13.000000 discovery-core-0.2.9/test/handlers/handler_factory_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-17 17:56:23.450585 discovery-core-0.2.9/test/intent/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.9/test/intent/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2899 2023-07-12 16:01:36.000000 discovery-core-0.2.9/test/intent/abstract_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     7100 2023-07-12 17:46:55.000000 discovery-core-0.2.9/test/intent/pyarrow_intent_model.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-17 17:56:23.453255 discovery-core-0.2.9/test/properties/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.9/test/properties/__init__.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    36169 2023-06-29 23:15:54.000000 discovery-core-0.2.9/test/properties/abstract_properties_manager_test.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     9513 2023-06-29 16:47:52.000000 discovery-core-0.2.9/test/properties/property_manager_test.py
```

### Comparing `discovery-core-0.2.8/LICENSE.txt` & `discovery-core-0.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.8/PKG-INFO` & `discovery-core-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-core
-Version: 0.2.8
+Version: 0.2.9
 Summary: Augmented Intent Single Task Adaptive Components
 Home-page: http://github.com/gigas64/discovery-core
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Foundation SDK Machine learning AI component intent data science
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-core-0.2.8/README.rst` & `discovery-core-0.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.8/discovery_core.egg-info/PKG-INFO` & `discovery-core-0.2.9/discovery_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-core
-Version: 0.2.8
+Version: 0.2.9
 Summary: Augmented Intent Single Task Adaptive Components
 Home-page: http://github.com/gigas64/discovery-core
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Foundation SDK Machine learning AI component intent data science
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-core-0.2.8/discovery_core.egg-info/SOURCES.txt` & `discovery-core-0.2.9/discovery_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.8/ds_core/components/abstract_component.py` & `discovery-core-0.2.9/ds_core/components/abstract_component.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.8/ds_core/components/core_commons.py` & `discovery-core-0.2.9/ds_core/components/core_commons.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.8/ds_core/handlers/abstract_handlers.py` & `discovery-core-0.2.9/ds_core/handlers/abstract_handlers.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.8/ds_core/handlers/pyarrow_handlers.py` & `discovery-core-0.2.9/ds_core/handlers/pyarrow_handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
             return csv.read_csv(address, **load_params)
         # json
         if file_type.lower() in ['json']:
             return json.read_json(address, **load_params)
         # complex nested
         if file_type.lower() in ['txt']:
             with open(address) as f:
-                document = ast.literal_eval(f.read(address))
+                document = ast.literal_eval(f.read())
             return pa.Table.from_pylist(document)
 
         raise LookupError('The source format {} is not currently supported'.format(file_type))
 
     def exists(self) -> bool:
         """ Returns True is the file exists """
         if not isinstance(self.connector_contract, ConnectorContract):
```

### Comparing `discovery-core-0.2.8/ds_core/intent/abstract_intent.py` & `discovery-core-0.2.9/ds_core/intent/abstract_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.8/ds_core/properties/abstract_properties.py` & `discovery-core-0.2.9/ds_core/properties/abstract_properties.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.8/ds_core/properties/decorator_patterns.py` & `discovery-core-0.2.9/ds_core/properties/decorator_patterns.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.8/ds_core/properties/property_manager.py` & `discovery-core-0.2.9/ds_core/properties/property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.8/setup.py` & `discovery-core-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.8/test/components/abstract_component_test.py` & `discovery-core-0.2.9/test/components/abstract_component_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.8/test/components/commons_test.py` & `discovery-core-0.2.9/test/components/commons_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.8/test/handlers/connector_contract_test.py` & `discovery-core-0.2.9/test/handlers/connector_contract_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.8/test/handlers/handler_factory_test.py` & `discovery-core-0.2.9/test/handlers/handler_factory_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.8/test/intent/abstract_intent_test.py` & `discovery-core-0.2.9/test/intent/abstract_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.8/test/intent/pyarrow_intent_model.py` & `discovery-core-0.2.9/test/intent/pyarrow_intent_model.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.8/test/properties/abstract_properties_manager_test.py` & `discovery-core-0.2.9/test/properties/abstract_properties_manager_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.8/test/properties/property_manager_test.py` & `discovery-core-0.2.9/test/properties/property_manager_test.py`

 * *Files identical despite different names*

