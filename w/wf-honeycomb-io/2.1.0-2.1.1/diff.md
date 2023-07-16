# Comparing `tmp/wf-honeycomb-io-2.1.0.tar.gz` & `tmp/wf-honeycomb-io-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wf-honeycomb-io-2.1.0.tar", last modified: Tue Feb 28 18:17:45 2023, max compression
+gzip compressed data, was "wf-honeycomb-io-2.1.1.tar", last modified: Sun Jul 16 22:36:24 2023, max compression
```

## Comparing `wf-honeycomb-io-2.1.0.tar` & `wf-honeycomb-io-2.1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 tcquinn   (1001) tcquinn   (1001)        0 2023-02-28 18:17:45.410806 wf-honeycomb-io-2.1.0/
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     1088 2022-12-09 15:32:12.000000 wf-honeycomb-io-2.1.0/LICENSE
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)       34 2022-12-09 15:32:12.000000 wf-honeycomb-io-2.1.0/MANIFEST.in
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     1688 2023-02-28 18:17:45.410806 wf-honeycomb-io-2.1.0/PKG-INFO
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     1120 2022-12-09 15:32:12.000000 wf-honeycomb-io-2.1.0/README.md
-drwxrwxr-x   0 tcquinn   (1001) tcquinn   (1001)        0 2023-02-28 18:17:45.410806 wf-honeycomb-io-2.1.0/honeycomb_io/
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)      423 2023-02-28 18:16:33.000000 wf-honeycomb-io-2.1.0/honeycomb_io/__init__.py
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)    37295 2022-12-09 15:32:12.000000 wf-honeycomb-io-2.1.0/honeycomb_io/cameras.py
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     2298 2022-12-09 15:32:12.000000 wf-honeycomb-io-2.1.0/honeycomb_io/coordinate_spaces.py
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)    13045 2023-02-28 18:15:59.000000 wf-honeycomb-io-2.1.0/honeycomb_io/core.py
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     1137 2022-12-09 15:32:12.000000 wf-honeycomb-io-2.1.0/honeycomb_io/datapoints.py
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)    32763 2022-12-09 15:32:12.000000 wf-honeycomb-io-2.1.0/honeycomb_io/devices.py
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)    10947 2023-02-28 17:52:07.000000 wf-honeycomb-io-2.1.0/honeycomb_io/environments.py
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)      356 2022-12-09 15:32:12.000000 wf-honeycomb-io-2.1.0/honeycomb_io/exceptions.py
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     5057 2022-12-09 15:32:12.000000 wf-honeycomb-io-2.1.0/honeycomb_io/inference_executions.py
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     3786 2022-12-09 15:32:12.000000 wf-honeycomb-io-2.1.0/honeycomb_io/interactions.py
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)    14969 2022-12-09 15:32:12.000000 wf-honeycomb-io-2.1.0/honeycomb_io/materials.py
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)    15746 2022-12-09 15:32:12.000000 wf-honeycomb-io-2.1.0/honeycomb_io/persons.py
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)    30834 2022-12-09 15:32:12.000000 wf-honeycomb-io-2.1.0/honeycomb_io/poses.py
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     3326 2022-12-09 15:32:12.000000 wf-honeycomb-io-2.1.0/honeycomb_io/schema.py
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)    15022 2022-12-09 15:32:12.000000 wf-honeycomb-io-2.1.0/honeycomb_io/trays.py
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     2017 2022-12-09 15:32:12.000000 wf-honeycomb-io-2.1.0/honeycomb_io/utils.py
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)   125523 2022-12-09 15:32:12.000000 wf-honeycomb-io-2.1.0/honeycomb_io/uwb_data.py
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)       38 2023-02-28 18:17:45.410806 wf-honeycomb-io-2.1.0/setup.cfg
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     1766 2022-12-09 15:32:12.000000 wf-honeycomb-io-2.1.0/setup.py
-drwxrwxr-x   0 tcquinn   (1001) tcquinn   (1001)        0 2023-02-28 18:17:45.410806 wf-honeycomb-io-2.1.0/wf_honeycomb_io.egg-info/
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     1688 2023-02-28 18:17:45.000000 wf-honeycomb-io-2.1.0/wf_honeycomb_io.egg-info/PKG-INFO
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)      673 2023-02-28 18:17:45.000000 wf-honeycomb-io-2.1.0/wf_honeycomb_io.egg-info/SOURCES.txt
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)        1 2023-02-28 18:17:45.000000 wf-honeycomb-io-2.1.0/wf_honeycomb_io.egg-info/dependency_links.txt
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)       93 2023-02-28 18:17:45.000000 wf-honeycomb-io-2.1.0/wf_honeycomb_io.egg-info/requires.txt
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)       13 2023-02-28 18:17:45.000000 wf-honeycomb-io-2.1.0/wf_honeycomb_io.egg-info/top_level.txt
+drwxrwxr-x   0 tcquinn   (1001) tcquinn   (1001)        0 2023-07-16 22:36:24.599998 wf-honeycomb-io-2.1.1/
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     1088 2022-12-09 15:32:12.000000 wf-honeycomb-io-2.1.1/LICENSE
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)       34 2022-12-09 15:32:12.000000 wf-honeycomb-io-2.1.1/MANIFEST.in
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     1688 2023-07-16 22:36:24.599998 wf-honeycomb-io-2.1.1/PKG-INFO
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     1120 2022-12-09 15:32:12.000000 wf-honeycomb-io-2.1.1/README.md
+drwxrwxr-x   0 tcquinn   (1001) tcquinn   (1001)        0 2023-07-16 22:36:24.599998 wf-honeycomb-io-2.1.1/honeycomb_io/
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)      423 2023-07-16 22:35:32.000000 wf-honeycomb-io-2.1.1/honeycomb_io/__init__.py
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)    37295 2022-12-09 15:32:12.000000 wf-honeycomb-io-2.1.1/honeycomb_io/cameras.py
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     2298 2022-12-09 15:32:12.000000 wf-honeycomb-io-2.1.1/honeycomb_io/coordinate_spaces.py
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)    13045 2023-02-28 18:15:59.000000 wf-honeycomb-io-2.1.1/honeycomb_io/core.py
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     1137 2022-12-09 15:32:12.000000 wf-honeycomb-io-2.1.1/honeycomb_io/datapoints.py
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)    32763 2022-12-09 15:32:12.000000 wf-honeycomb-io-2.1.1/honeycomb_io/devices.py
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)    10947 2023-02-28 18:18:59.000000 wf-honeycomb-io-2.1.1/honeycomb_io/environments.py
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)      356 2022-12-09 15:32:12.000000 wf-honeycomb-io-2.1.1/honeycomb_io/exceptions.py
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     5057 2022-12-09 15:32:12.000000 wf-honeycomb-io-2.1.1/honeycomb_io/inference_executions.py
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     3786 2022-12-09 15:32:12.000000 wf-honeycomb-io-2.1.1/honeycomb_io/interactions.py
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)    14969 2022-12-09 15:32:12.000000 wf-honeycomb-io-2.1.1/honeycomb_io/materials.py
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)    15746 2022-12-09 15:32:12.000000 wf-honeycomb-io-2.1.1/honeycomb_io/persons.py
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)    30834 2022-12-09 15:32:12.000000 wf-honeycomb-io-2.1.1/honeycomb_io/poses.py
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     3326 2022-12-09 15:32:12.000000 wf-honeycomb-io-2.1.1/honeycomb_io/schema.py
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)    15022 2022-12-09 15:32:12.000000 wf-honeycomb-io-2.1.1/honeycomb_io/trays.py
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     2017 2022-12-09 15:32:12.000000 wf-honeycomb-io-2.1.1/honeycomb_io/utils.py
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)   125563 2023-07-16 22:34:17.000000 wf-honeycomb-io-2.1.1/honeycomb_io/uwb_data.py
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)       38 2023-07-16 22:36:24.599998 wf-honeycomb-io-2.1.1/setup.cfg
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     1766 2022-12-09 15:32:12.000000 wf-honeycomb-io-2.1.1/setup.py
+drwxrwxr-x   0 tcquinn   (1001) tcquinn   (1001)        0 2023-07-16 22:36:24.599998 wf-honeycomb-io-2.1.1/wf_honeycomb_io.egg-info/
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     1688 2023-07-16 22:36:24.000000 wf-honeycomb-io-2.1.1/wf_honeycomb_io.egg-info/PKG-INFO
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)      673 2023-07-16 22:36:24.000000 wf-honeycomb-io-2.1.1/wf_honeycomb_io.egg-info/SOURCES.txt
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)        1 2023-07-16 22:36:24.000000 wf-honeycomb-io-2.1.1/wf_honeycomb_io.egg-info/dependency_links.txt
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)       93 2023-07-16 22:36:24.000000 wf-honeycomb-io-2.1.1/wf_honeycomb_io.egg-info/requires.txt
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)       13 2023-07-16 22:36:24.000000 wf-honeycomb-io-2.1.1/wf_honeycomb_io.egg-info/top_level.txt
```

### Comparing `wf-honeycomb-io-2.1.0/LICENSE` & `wf-honeycomb-io-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wf-honeycomb-io-2.1.0/PKG-INFO` & `wf-honeycomb-io-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wf-honeycomb-io
-Version: 2.1.0
+Version: 2.1.1
 Summary: Tools for working with data in Wildflower's Honeycomb database
 Home-page: https://github.com/WildflowerSchools/wf-honeycomb-io
 Author: Theodore Quinn
 Author-email: ted.quinn@wildflowerschools.org
 License: UNKNOWN
 Keywords: database
 Platform: UNKNOWN
```

### Comparing `wf-honeycomb-io-2.1.0/README.md` & `wf-honeycomb-io-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `wf-honeycomb-io-2.1.0/honeycomb_io/cameras.py` & `wf-honeycomb-io-2.1.1/honeycomb_io/cameras.py`

 * *Files identical despite different names*

### Comparing `wf-honeycomb-io-2.1.0/honeycomb_io/coordinate_spaces.py` & `wf-honeycomb-io-2.1.1/honeycomb_io/coordinate_spaces.py`

 * *Files identical despite different names*

### Comparing `wf-honeycomb-io-2.1.0/honeycomb_io/core.py` & `wf-honeycomb-io-2.1.1/honeycomb_io/core.py`

 * *Files identical despite different names*

### Comparing `wf-honeycomb-io-2.1.0/honeycomb_io/datapoints.py` & `wf-honeycomb-io-2.1.1/honeycomb_io/datapoints.py`

 * *Files identical despite different names*

### Comparing `wf-honeycomb-io-2.1.0/honeycomb_io/devices.py` & `wf-honeycomb-io-2.1.1/honeycomb_io/devices.py`

 * *Files identical despite different names*

### Comparing `wf-honeycomb-io-2.1.0/honeycomb_io/environments.py` & `wf-honeycomb-io-2.1.1/honeycomb_io/environments.py`

 * *Files identical despite different names*

### Comparing `wf-honeycomb-io-2.1.0/honeycomb_io/inference_executions.py` & `wf-honeycomb-io-2.1.1/honeycomb_io/inference_executions.py`

 * *Files identical despite different names*

### Comparing `wf-honeycomb-io-2.1.0/honeycomb_io/interactions.py` & `wf-honeycomb-io-2.1.1/honeycomb_io/interactions.py`

 * *Files identical despite different names*

### Comparing `wf-honeycomb-io-2.1.0/honeycomb_io/materials.py` & `wf-honeycomb-io-2.1.1/honeycomb_io/materials.py`

 * *Files identical despite different names*

### Comparing `wf-honeycomb-io-2.1.0/honeycomb_io/persons.py` & `wf-honeycomb-io-2.1.1/honeycomb_io/persons.py`

 * *Files identical despite different names*

### Comparing `wf-honeycomb-io-2.1.0/honeycomb_io/poses.py` & `wf-honeycomb-io-2.1.1/honeycomb_io/poses.py`

 * *Files identical despite different names*

### Comparing `wf-honeycomb-io-2.1.0/honeycomb_io/schema.py` & `wf-honeycomb-io-2.1.1/honeycomb_io/schema.py`

 * *Files identical despite different names*

### Comparing `wf-honeycomb-io-2.1.0/honeycomb_io/trays.py` & `wf-honeycomb-io-2.1.1/honeycomb_io/trays.py`

 * *Files identical despite different names*

### Comparing `wf-honeycomb-io-2.1.0/honeycomb_io/utils.py` & `wf-honeycomb-io-2.1.1/honeycomb_io/utils.py`

 * *Files identical despite different names*

### Comparing `wf-honeycomb-io-2.1.0/honeycomb_io/uwb_data.py` & `wf-honeycomb-io-2.1.1/honeycomb_io/uwb_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -613,51 +613,51 @@
     uri=None,
     token_uri=None,
     audience=None,
     client_id=None,
     client_secret=None
 ):
     if data_type == 'position':
-        data_ids = write_position_data(
+        data_ids = write_cuwb_position_data(
             position_data=parsed_data,
             chunk_size=chunk_size,
             client=client,
             uri=uri,
             token_uri=token_uri,
             audience=audience,
             client_id=client_id,
             client_secret=client_secret
         )
         return data_ids
     elif data_type == 'accelerometer':
-        data_ids = write_accelerometer_data(
+        data_ids = write_cuwb_accelerometer_data(
             accelerometer_data=parsed_data,
             chunk_size=chunk_size,
             client=client,
             uri=uri,
             token_uri=token_uri,
             audience=audience,
             client_id=client_id,
             client_secret=client_secret
         )
         return data_ids
     elif data_type == 'gyroscope':
-        data_ids = write_gyroscope_data(
+        data_ids = write_cuwb_gyroscope_data(
             gyroscope_data=parsed_data,
             chunk_size=chunk_size,
             client=client,
             uri=uri,
             token_uri=token_uri,
             audience=audience,
             client_id=client_id,
             client_secret=client_secret
         )
         return data_ids
     elif data_type == 'magnetometer':
-        data_ids = write_magnetometer_data(
+        data_ids = write_cuwb_magnetometer_data(
             magnetometer_data=parsed_data,
             chunk_size=chunk_size,
             client=client,
             uri=uri,
             token_uri=token_uri,
             audience=audience,
             client_id=client_id,
@@ -665,15 +665,15 @@
         )
         return data_ids
     else:
         raise ValueError('Data type {} not currently supported'.format(
             data_type
         ))
 
-def write_position_data(
+def write_cuwb_position_data(
     position_data,
     chunk_size=1000,
     client=None,
     uri=None,
     token_uri=None,
     audience=None,
     client_id=None,
@@ -707,15 +707,15 @@
             'Encountered problem when attempting to write assignment data'
         )
     logger.info('Successfully wrote {} CUWB position observations to Honeycomb'.format(
         len(position_data_ids)
     ))
     return position_data_ids
 
-def write_accelerometer_data(
+def write_cuwb_accelerometer_data(
     accelerometer_data,
     chunk_size=1000,
     client=None,
     uri=None,
     token_uri=None,
     audience=None,
     client_id=None,
@@ -749,15 +749,15 @@
             'Encountered problem when attempting to write accelerometer data'
         )
     logger.info('Successfully wrote {} CUWB accelerometer observations to Honeycomb'.format(
         len(accelerometer_data_ids)
     ))
     return accelerometer_data_ids
 
-def write_gyroscope_data(
+def write_cuwb_gyroscope_data(
     gyroscope_data,
     chunk_size=1000,
     client=None,
     uri=None,
     token_uri=None,
     audience=None,
     client_id=None,
@@ -791,15 +791,15 @@
             'Encountered problem when attempting to write gyroscope data'
         )
     logger.info('Successfully wrote {} CUWB gyroscope observations to Honeycomb'.format(
         len(gyroscope_data_ids)
     ))
     return gyroscope_data_ids
 
-def write_magnetometer_data(
+def write_cuwb_magnetometer_data(
     magnetometer_data,
     chunk_size=1000,
     client=None,
     uri=None,
     token_uri=None,
     audience=None,
     client_id=None,
```

### Comparing `wf-honeycomb-io-2.1.0/setup.py` & `wf-honeycomb-io-2.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `wf-honeycomb-io-2.1.0/wf_honeycomb_io.egg-info/PKG-INFO` & `wf-honeycomb-io-2.1.1/wf_honeycomb_io.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wf-honeycomb-io
-Version: 2.1.0
+Version: 2.1.1
 Summary: Tools for working with data in Wildflower's Honeycomb database
 Home-page: https://github.com/WildflowerSchools/wf-honeycomb-io
 Author: Theodore Quinn
 Author-email: ted.quinn@wildflowerschools.org
 License: UNKNOWN
 Keywords: database
 Platform: UNKNOWN
```

### Comparing `wf-honeycomb-io-2.1.0/wf_honeycomb_io.egg-info/SOURCES.txt` & `wf-honeycomb-io-2.1.1/wf_honeycomb_io.egg-info/SOURCES.txt`

 * *Files identical despite different names*

