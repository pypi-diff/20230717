# Comparing `tmp/macrometa-source-mongo-0.0.46.tar.gz` & `tmp/macrometa-source-mongo-0.0.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-mongo-0.0.46.tar", max compression
+gzip compressed data, was "macrometa-source-mongo-0.0.47.tar", max compression
```

## Comparing `macrometa-source-mongo-0.0.46.tar` & `macrometa-source-mongo-0.0.47.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    10765 2023-06-20 15:02:15.649089 macrometa-source-mongo-0.0.46/LICENSE
--rw-r--r--   0        0        0    22504 2023-06-20 15:02:15.649089 macrometa-source-mongo-0.0.46/macrometa_source_mongo/__init__.py
--rw-r--r--   0        0        0     6577 2023-06-20 15:02:15.649089 macrometa-source-mongo-0.0.46/macrometa_source_mongo/connection.py
--rw-r--r--   0        0        0      895 2023-06-20 15:02:15.649089 macrometa-source-mongo-0.0.46/macrometa_source_mongo/exceptions.py
--rw-r--r--   0        0        0     7252 2023-06-20 15:02:15.649089 macrometa-source-mongo-0.0.46/macrometa_source_mongo/helper.py
--rw-r--r--   0        0        0    10251 2023-06-20 15:02:15.649089 macrometa-source-mongo-0.0.46/macrometa_source_mongo/sync_strategies/common.py
--rw-r--r--   0        0        0     3647 2023-06-20 15:02:15.649089 macrometa-source-mongo-0.0.46/macrometa_source_mongo/sync_strategies/full_table.py
--rw-r--r--   0        0        0     7181 2023-06-20 15:02:15.649089 macrometa-source-mongo-0.0.46/macrometa_source_mongo/sync_strategies/log_based.py
--rw-r--r--   0        0        0     2292 2023-06-20 15:02:15.649089 macrometa-source-mongo-0.0.46/macrometa_source_mongo/sync_strategies/sample_data.py
--rw-r--r--   0        0        0     1548 2023-06-20 15:02:15.893093 macrometa-source-mongo-0.0.46/pyproject.toml
--rw-r--r--   0        0        0     1095 1970-01-01 00:00:00.000000 macrometa-source-mongo-0.0.46/setup.py
--rw-r--r--   0        0        0      956 1970-01-01 00:00:00.000000 macrometa-source-mongo-0.0.46/PKG-INFO
+-rw-r--r--   0        0        0    10765 2023-07-17 10:18:35.414112 macrometa-source-mongo-0.0.47/LICENSE
+-rw-r--r--   0        0        0    23259 2023-07-17 10:18:35.414112 macrometa-source-mongo-0.0.47/macrometa_source_mongo/__init__.py
+-rw-r--r--   0        0        0     6577 2023-07-17 10:18:35.414112 macrometa-source-mongo-0.0.47/macrometa_source_mongo/connection.py
+-rw-r--r--   0        0        0      895 2023-07-17 10:18:35.414112 macrometa-source-mongo-0.0.47/macrometa_source_mongo/exceptions.py
+-rw-r--r--   0        0        0     7252 2023-07-17 10:18:35.414112 macrometa-source-mongo-0.0.47/macrometa_source_mongo/helper.py
+-rw-r--r--   0        0        0    10251 2023-07-17 10:18:35.414112 macrometa-source-mongo-0.0.47/macrometa_source_mongo/sync_strategies/common.py
+-rw-r--r--   0        0        0     3647 2023-07-17 10:18:35.414112 macrometa-source-mongo-0.0.47/macrometa_source_mongo/sync_strategies/full_table.py
+-rw-r--r--   0        0        0     7239 2023-07-17 10:18:35.414112 macrometa-source-mongo-0.0.47/macrometa_source_mongo/sync_strategies/log_based.py
+-rw-r--r--   0        0        0     2292 2023-07-17 10:18:35.414112 macrometa-source-mongo-0.0.47/macrometa_source_mongo/sync_strategies/sample_data.py
+-rw-r--r--   0        0        0     1577 2023-07-17 10:18:35.690125 macrometa-source-mongo-0.0.47/pyproject.toml
+-rw-r--r--   0        0        0     1125 1970-01-01 00:00:00.000000 macrometa-source-mongo-0.0.47/setup.py
+-rw-r--r--   0        0        0     1000 1970-01-01 00:00:00.000000 macrometa-source-mongo-0.0.47/PKG-INFO
```

### Comparing `macrometa-source-mongo-0.0.46/LICENSE` & `macrometa-source-mongo-0.0.47/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.46/macrometa_source_mongo/__init__.py` & `macrometa-source-mongo-0.0.47/macrometa_source_mongo/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 #!/usr/bin/env python3
 import copy
 import json
+import os
 import sys
 from typing import List, Dict
 
 import pkg_resources
 import singer
 from pymongo import MongoClient
 from singer import metadata, metrics, utils
 from c8connector import (
     C8Connector, ConfigProperty, Sample, Schema,
     ConfigAttributeType, SchemaAttribute, ValidationException)
 
+from prometheus_client import CollectorRegistry, start_http_server, Counter
 from macrometa_source_mongo.sync_strategies import log_based
 from macrometa_source_mongo.sync_strategies import common
 from macrometa_source_mongo.sync_strategies import full_table
 from macrometa_source_mongo.sync_strategies.sample_data import fetch_samples
 from macrometa_source_mongo.connection import create_certficate_files, delete_certficate_files, \
     get_connection_string, get_user_databases
 from macrometa_source_mongo.exceptions import InvalidReplicationMethodException, NoReadPrivilegeException
@@ -35,14 +37,19 @@
 ]
 
 REQUIRED_CONFIG_KEYS_NON_SRV = REQUIRED_CONFIG_KEYS + ['port']
 
 LOG_BASED_METHOD = 'LOG_BASED'
 FULL_TABLE_METHOD = 'FULL_TABLE'
 
+region_label = os.getenv("GDN_FEDERATION", "NA")
+tenant_label = os.getenv("GDN_TENANT", "NA")
+fabric_label = os.getenv("GDN_FABRIC", "NA")
+workflow_label = os.getenv("WORKFLOW_UUID", "NA")
+
 
 class MongoSourceConnector(C8Connector):
     """MongoSourceConnector's C8Connector impl."""
 
     def name(self) -> str:
         """Returns the name of the connector."""
         return "MongoDB"
@@ -457,14 +464,21 @@
     LOGGER.info(common.get_sync_summary(catalog, replication_method))
 
 
 def main_impl():
     """
     Main function
     """
+    # Create a custom CollectorRegistry
+    registry_package = CollectorRegistry()
+    ingest_errors = Counter('ingest_errors', 'Total number of errors during ingestion',
+                        ['region', 'tenant', 'fabric', 'workflow'], registry=registry_package)
+    LOGGER.info("Mongo source is starting the metrics server.")
+    start_http_server(8000, registry=registry_package)
+
     args = utils.parse_args(REQUIRED_CONFIG_KEYS)
     config = args.config
     srv = config.get('srv', False)
 
     if not srv:
         args = utils.parse_args(REQUIRED_CONFIG_KEYS_NON_SRV)
         config = args.config
@@ -480,14 +494,15 @@
 
         if args.discover:
             do_discover(client, config)
         elif args.catalog:
             state = args.state or {}
             do_sync(client, args.catalog.to_dict(), config, args.config.get('replication_method', FULL_TABLE_METHOD), state)
     except Exception as e:
+        ingest_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
         delete_certficate_files(config)
         raise e
     delete_certficate_files(config)
 
 
 def main():
     """
```

### Comparing `macrometa-source-mongo-0.0.46/macrometa_source_mongo/connection.py` & `macrometa-source-mongo-0.0.47/macrometa_source_mongo/connection.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.46/macrometa_source_mongo/exceptions.py` & `macrometa-source-mongo-0.0.47/macrometa_source_mongo/exceptions.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.46/macrometa_source_mongo/helper.py` & `macrometa-source-mongo-0.0.47/macrometa_source_mongo/helper.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.46/macrometa_source_mongo/sync_strategies/common.py` & `macrometa-source-mongo-0.0.47/macrometa_source_mongo/sync_strategies/common.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.46/macrometa_source_mongo/sync_strategies/full_table.py` & `macrometa-source-mongo-0.0.47/macrometa_source_mongo/sync_strategies/full_table.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.46/macrometa_source_mongo/sync_strategies/log_based.py` & `macrometa-source-mongo-0.0.47/macrometa_source_mongo/sync_strategies/log_based.py`

 * *Files 6% similar despite different names*

```diff
@@ -84,14 +84,15 @@
                             }}],
                             max_await_time_ms=DEFAULT_AWAIT_TIME_MS,
                             start_after=get_bookmark_key_from_state(stream_ids, state)
                     ) as cursor:
                 while cursor.alive:
                 
                     change = cursor.try_next()
+                    time_extracted = utils.now()
                     # Get resume token from '_data' to resume LOG_BASED
                     resume_token = {
                         '_data': cursor.resume_token['_data']
                     }
         
                     # After MAX_AWAIT_TIME_MS has elapsed, the cursor will return None.
                     if change is None:
@@ -101,35 +102,35 @@
                     operation = change['operationType']
 
                     if operation == 'delete':
                         # Delete ops only contain the _id of the row deleted
                         singer.write_message(common.row_to_singer_record(
                             stream=streams_to_sync[tap_stream_id],
                             row={'_id': change['documentKey']['_id']},
-                            time_extracted=utils.now(),
+                            time_extracted=time_extracted,
                             time_deleted=change[
                                 'clusterTime'].as_datetime()))  # returns python's datetime.datetime instance in UTC
 
                         rows_saved[tap_stream_id] += 1
 
                     elif operation == 'insert':
                         singer.write_message(common.row_to_singer_record(stream=streams_to_sync[tap_stream_id],
                                                                          row=change['fullDocument'],
-                                                                         time_extracted=utils.now(),
+                                                                         time_extracted=time_extracted,
                                                                          time_deleted=None))
         
                         rows_saved[tap_stream_id] += 1
 
                     elif operation == 'update':
                         # update operation only return _id and updated fields in the row,
                         query = {'_id': change['documentKey']['_id']}
                         row = database[streams_to_sync[tap_stream_id]['table_name']].find_one(query)
                         singer.write_message(common.row_to_singer_record(stream=streams_to_sync[tap_stream_id],
                                                                          row=row,
-                                                                         time_extracted=utils.now(),
+                                                                         time_extracted=time_extracted,
                                                                          time_deleted=None))
 
                         rows_saved[tap_stream_id] += 1
 
                     # update the states of all streams
                     state = update_bookmarks(state, stream_ids, resume_token)
```

### Comparing `macrometa-source-mongo-0.0.46/macrometa_source_mongo/sync_strategies/sample_data.py` & `macrometa-source-mongo-0.0.47/macrometa_source_mongo/sync_strategies/sample_data.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.46/pyproject.toml` & `macrometa-source-mongo-0.0.47/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-mongo"
-version='0.0.46'
+version='0.0.47'
 description = "Macrometa Source for extracting data from MongoDB."
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
@@ -29,14 +29,15 @@
 python = ">=3.8.1,<3.11"
 pipelinewise-singer-python = "1.2.0"
 c8connector = ">=0.0.24"
 pymongo = {version = "^4.0",extras = ["srv"]}
 tzlocal = "2.1.*"
 terminaltables = "3.1.*"
 dnspython = "2.1.*"
+prometheus-client = "0.16.0"
 
 [tool.poetry.scripts]
 # CLI declaration
 macrometa-source-mongo = 'macrometa_source_mongo:main'
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/Macrometacorp/macrometa-source-mongo/issues"
```

### Comparing `macrometa-source-mongo-0.0.46/setup.py` & `macrometa-source-mongo-0.0.47/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,24 +12,25 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['c8connector>=0.0.24',
  'dnspython>=2.1.0,<2.2.0',
  'pipelinewise-singer-python==1.2.0',
+ 'prometheus-client==0.16.0',
  'pymongo[srv]>=4.0,<5.0',
  'terminaltables>=3.1.0,<3.2.0',
  'tzlocal>=2.1.0,<2.2.0']
 
 entry_points = \
 {'console_scripts': ['macrometa-source-mongo = macrometa_source_mongo:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-mongo',
-    'version': '0.0.46',
+    'version': '0.0.47',
     'description': 'Macrometa Source for extracting data from MongoDB.',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-source-mongo-0.0.46/PKG-INFO` & `macrometa-source-mongo-0.0.47/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-source-mongo
-Version: 0.0.46
+Version: 0.0.47
 Summary: Macrometa Source for extracting data from MongoDB.
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,MongoDB,Source
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
@@ -12,11 +12,12 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Requires-Dist: c8connector (>=0.0.24)
 Requires-Dist: dnspython (>=2.1.0,<2.2.0)
 Requires-Dist: pipelinewise-singer-python (==1.2.0)
+Requires-Dist: prometheus-client (==0.16.0)
 Requires-Dist: pymongo[srv] (>=4.0,<5.0)
 Requires-Dist: terminaltables (>=3.1.0,<3.2.0)
 Requires-Dist: tzlocal (>=2.1.0,<2.2.0)
 Project-URL: Bug Tracker, https://github.com/Macrometacorp/macrometa-source-mongo/issues
```

