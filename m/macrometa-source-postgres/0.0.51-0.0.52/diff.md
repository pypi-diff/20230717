# Comparing `tmp/macrometa-source-postgres-0.0.51.tar.gz` & `tmp/macrometa-source-postgres-0.0.52.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-postgres-0.0.51.tar", max compression
+gzip compressed data, was "macrometa-source-postgres-0.0.52.tar", max compression
```

## Comparing `macrometa-source-postgres-0.0.51.tar` & `macrometa-source-postgres-0.0.52.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11899 2023-06-28 12:48:11.776575 macrometa-source-postgres-0.0.51/LICENSE
--rw-r--r--   0        0        0    35738 2023-06-28 12:48:11.776575 macrometa-source-postgres-0.0.51/macrometa_source_postgres/__init__.py
--rw-r--r--   0        0        0     8690 2023-06-28 12:48:11.776575 macrometa-source-postgres-0.0.51/macrometa_source_postgres/connection.py
--rw-r--r--   0        0        0    20349 2023-06-28 12:48:11.776575 macrometa-source-postgres-0.0.51/macrometa_source_postgres/helper.py
--rw-r--r--   0        0        0        0 2023-06-28 12:48:11.776575 macrometa-source-postgres-0.0.51/macrometa_source_postgres/sync_strategies/__init__.py
--rw-r--r--   0        0        0     1212 2023-06-28 12:48:11.776575 macrometa-source-postgres-0.0.51/macrometa_source_postgres/sync_strategies/common.py
--rw-r--r--   0        0        0     8974 2023-06-28 12:48:11.776575 macrometa-source-postgres-0.0.51/macrometa_source_postgres/sync_strategies/full_table.py
--rw-r--r--   0        0        0    28161 2023-06-28 12:48:11.776575 macrometa-source-postgres-0.0.51/macrometa_source_postgres/sync_strategies/log_based.py
--rw-r--r--   0        0        0     3698 2023-06-28 12:48:11.776575 macrometa-source-postgres-0.0.51/macrometa_source_postgres/sync_strategies/sample_data.py
--rw-r--r--   0        0        0     1512 2023-06-28 12:48:12.028580 macrometa-source-postgres-0.0.51/pyproject.toml
--rw-r--r--   0        0        0     1077 1970-01-01 00:00:00.000000 macrometa-source-postgres-0.0.51/setup.py
--rw-r--r--   0        0        0      877 1970-01-01 00:00:00.000000 macrometa-source-postgres-0.0.51/PKG-INFO
+-rw-r--r--   0        0        0    11899 2023-07-17 14:10:34.760492 macrometa-source-postgres-0.0.52/LICENSE
+-rw-r--r--   0        0        0    36495 2023-07-17 14:10:34.760492 macrometa-source-postgres-0.0.52/macrometa_source_postgres/__init__.py
+-rw-r--r--   0        0        0     8690 2023-07-17 14:10:34.760492 macrometa-source-postgres-0.0.52/macrometa_source_postgres/connection.py
+-rw-r--r--   0        0        0    20349 2023-07-17 14:10:34.760492 macrometa-source-postgres-0.0.52/macrometa_source_postgres/helper.py
+-rw-r--r--   0        0        0        0 2023-07-17 14:10:34.760492 macrometa-source-postgres-0.0.52/macrometa_source_postgres/sync_strategies/__init__.py
+-rw-r--r--   0        0        0     1212 2023-07-17 14:10:34.760492 macrometa-source-postgres-0.0.52/macrometa_source_postgres/sync_strategies/common.py
+-rw-r--r--   0        0        0     9019 2023-07-17 14:10:34.760492 macrometa-source-postgres-0.0.52/macrometa_source_postgres/sync_strategies/full_table.py
+-rw-r--r--   0        0        0    28173 2023-07-17 14:10:34.760492 macrometa-source-postgres-0.0.52/macrometa_source_postgres/sync_strategies/log_based.py
+-rw-r--r--   0        0        0     3698 2023-07-17 14:10:34.760492 macrometa-source-postgres-0.0.52/macrometa_source_postgres/sync_strategies/sample_data.py
+-rw-r--r--   0        0        0     1541 2023-07-17 14:10:35.028486 macrometa-source-postgres-0.0.52/pyproject.toml
+-rw-r--r--   0        0        0     1107 1970-01-01 00:00:00.000000 macrometa-source-postgres-0.0.52/setup.py
+-rw-r--r--   0        0        0      921 1970-01-01 00:00:00.000000 macrometa-source-postgres-0.0.52/PKG-INFO
```

### Comparing `macrometa-source-postgres-0.0.51/LICENSE` & `macrometa-source-postgres-0.0.52/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.51/macrometa_source_postgres/__init__.py` & `macrometa-source-postgres-0.0.52/macrometa_source_postgres/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import argparse
 import copy
 import itertools
+import os
 
 import pkg_resources
 import psycopg2
 import psycopg2.extensions
 import psycopg2.extras
 import singer
 import singer.schema
 import uuid
 from c8connector import (
     C8Connector, ConfigProperty, Sample, Schema,
     ConfigAttributeType, SchemaAttributeType, SchemaAttribute, ValidationException)
 from pathlib import Path
+from prometheus_client import CollectorRegistry, start_http_server, Counter
 from singer import utils, metadata, get_bookmark
 from singer.catalog import Catalog
 from typing import Dict
 
 import macrometa_source_postgres.connection as postgres
 import macrometa_source_postgres.sync_strategies.common as sync_common
 from macrometa_source_postgres.helper import (
@@ -34,14 +36,18 @@
     'port',
     'user',
     'password',
     'filter_schemas',
     'filter_table'
 ]
 
+region_label = os.getenv("GDN_FEDERATION", "NA")
+tenant_label = os.getenv("GDN_TENANT", "NA")
+fabric_label = os.getenv("GDN_FABRIC", "NA")
+workflow_label = os.getenv("WORKFLOW_UUID", "NA")
 
 class PostgresSourceConnector(C8Connector):
     """PostgresSourceConnector's C8Connector impl."""
 
     def name(self) -> str:
         """Returns the name of the connector."""
         return "PostgreSQL"
@@ -726,14 +732,21 @@
     return args
 
 
 def main_impl():
     """
     Main method
     """
+    # Create a custom CollectorRegistry
+    registry_package = CollectorRegistry()
+    ingest_errors = Counter('ingest_errors', 'Total number of errors during ingestion',
+                        ['region', 'tenant', 'fabric', 'workflow'], registry=registry_package)
+    LOGGER.info("Postgres source is starting the metrics server.")
+    start_http_server(8000, registry=registry_package)
+
     args = parse_args(REQUIRED_CONFIG_KEYS)
     conn_config = {
         # Required config keys
         'host': args.config['host'],
         'user': args.config['user'],
         'password': args.config['password'],
         'port': args.config['port'],
@@ -767,14 +780,15 @@
             state_file = args.state_file
             do_sync(conn_config, args.catalog.to_dict() if args.catalog else args.properties,
                     conn_config.get('replication_method'), state, state_file)
         else:
             LOGGER.info("No properties were selected")
     except Exception as e:
         LOGGER.warn("Exception raised: %s", e)
+        ingest_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
         delete_certficate_files(conn_config)
         raise e
     delete_certficate_files(conn_config)
 
 
 def main():
     """
```

### Comparing `macrometa-source-postgres-0.0.51/macrometa_source_postgres/connection.py` & `macrometa-source-postgres-0.0.52/macrometa_source_postgres/connection.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.51/macrometa_source_postgres/helper.py` & `macrometa-source-postgres-0.0.52/macrometa_source_postgres/helper.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.51/macrometa_source_postgres/sync_strategies/common.py` & `macrometa-source-postgres-0.0.52/macrometa_source_postgres/sync_strategies/common.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.51/macrometa_source_postgres/sync_strategies/full_table.py` & `macrometa-source-postgres-0.0.52/macrometa_source_postgres/sync_strategies/full_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,18 +20,14 @@
     :param dict conn_info: dictionary of connection parameters to connect to PostgreSQL
     :param dict stream: dictionary of stream metadata
     :param dict state: dictionary representing the state of the replication process
     :param list desired_columns: list of desired columns for the view
     :param dict md_map: dictionary mapping metadata to the relevant stream
     :return: updated state dictionary representing the state of the replication process
     """
-
-    # Get the current time for time_extracted
-    time_extracted = utils.now()
-
     # Get the current version of the stream, or generate a new one
     current_version = singer.get_bookmark(state, stream['tap_stream_id'], 'version')
     if current_version is None:
         current_version = int(time.time() * 1000)
         state = singer.write_bookmark(state, stream['tap_stream_id'], 'version', current_version)
         singer.write_message(singer.StateMessage(value=copy.deepcopy(state)))
 
@@ -58,14 +54,16 @@
                              f"{postgres.fully_qualified_table_name(schema_name, stream['table_name'])}"
 
                 LOGGER.info("Fetching rows with iterator size of %s for SQL query: '%s'", cur.itersize, select_sql)
                 cur.execute(select_sql)
 
                 # Iterate through the records returned by the query
                 for rows_saved, rec in enumerate(cur, start=1):
+                    # Get the current time for time_extracted
+                    time_extracted = utils.now()
                     # Convert the record to a Singer message and write it to the target
                     record_message = postgres.selected_row_to_singer_message(stream,
                                                                             rec,
                                                                             current_version,
                                                                             desired_columns,
                                                                             time_extracted,
                                                                             md_map)
@@ -91,16 +89,14 @@
     :param dict conn_info: dictionary of connection parameters to connect to PostgreSQL
     :param dict stream: dictionary of stream metadata
     :param dict state: dictionary representing the state of the replication process
     :param list desired_columns: list of desired columns for the table
     :param dict md_map: dictionary mapping metadata to the relevant stream
     :return: updated state dictionary representing the state of the replication process
     """
-    time_extracted = utils.now()
-
     # check the version if it already exists
     first_run = singer.get_bookmark(state, stream['tap_stream_id'], 'version') is None
 
     # xmin indicates that we were interrupted last time
     if singer.get_bookmark(state, stream['tap_stream_id'], 'xmin') is None:
         nascent_stream_version = int(time.time() * 1000)
     else:
@@ -157,14 +153,15 @@
                                       FROM {fq_table_name}
                                      ORDER BY xmin::text ASC"""
 
                 LOGGER.info("Fetching rows with iterator size of %s for SQL query: '%s'", cur.itersize, select_sql)
                 cur.execute(select_sql)
 
                 for rows_saved, rec in enumerate(cur, start=1):
+                    time_extracted = utils.now()
                     xmin = rec['xmin']
                     rec = rec[:-1]
                     record_message = postgres.selected_row_to_singer_message(stream,
                                                                             rec,
                                                                             nascent_stream_version,
                                                                             desired_columns,
                                                                             time_extracted,
```

### Comparing `macrometa-source-postgres-0.0.51/macrometa_source_postgres/sync_strategies/log_based.py` & `macrometa-source-postgres-0.0.52/macrometa_source_postgres/sync_strategies/log_based.py`

 * *Files 0% similar despite different names*

```diff
@@ -526,15 +526,14 @@
         [
             get_bookmark(state_committed, s['tap_stream_id'], 'lsn')
             for s in logical_streams
         ]
     )
     start_lsn = lsn_committed
     lsn_to_flush = None
-    time_extracted = utils.now()
     slot = locate_replication_slot(conn_info)
     lsn_last_processed = None
     lsn_currently_processing = None
     lsn_processed_count = 0
     break_at_end_lsn = conn_info['break_at_end_lsn']
     poll_interval = 10
     poll_timestamp = None
@@ -589,14 +588,15 @@
             if msg:
                 if (break_at_end_lsn) and (msg.data_start > end_lsn):
                     LOGGER.info('The latest wal message %s is beyond the end_lsn %s, stopping replication.',
                                 int_to_lsn(msg.data_start),
                                 int_to_lsn(end_lsn))
                     break
 
+                time_extracted = utils.now()
                 state = consume_message(logical_streams, state, msg, time_extracted, conn_info)
 
                 # To ensure that we only flush to an LSN that has been entirely completed, when using wal2json
                 # with the write-in-chunks option, multiple messages can have the same LSN.
                 if lsn_currently_processing is None:
                     lsn_currently_processing = msg.data_start
                     LOGGER.info('The initial write-ahead log (WAL) message has been received: %s',
```

### Comparing `macrometa-source-postgres-0.0.51/macrometa_source_postgres/sync_strategies/sample_data.py` & `macrometa-source-postgres-0.0.52/macrometa_source_postgres/sync_strategies/sample_data.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.51/pyproject.toml` & `macrometa-source-postgres-0.0.52/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-postgres"
-version='0.0.51'
+version='0.0.52'
 description = "Macrometa Source for extracting data from PostgreSQL."
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
@@ -27,14 +27,15 @@
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.11"
 pipelinewise-singer-python = "1.2.0"
 c8connector = ">=0.0.24"
 psycopg2-binary = "2.9.3"
 strict-rfc3339 = "0.7"
+prometheus-client = "0.16.0"
 
 [tool.poetry.scripts]
 # CLI declaration
 macrometa-source-postgres = 'macrometa_source_postgres:main'
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/Macrometacorp/macrometa-source-postgres/issues"
```

### Comparing `macrometa-source-postgres-0.0.51/setup.py` & `macrometa-source-postgres-0.0.52/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,24 +11,25 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['c8connector>=0.0.24',
  'pipelinewise-singer-python==1.2.0',
+ 'prometheus-client==0.16.0',
  'psycopg2-binary==2.9.3',
  'strict-rfc3339==0.7']
 
 entry_points = \
 {'console_scripts': ['macrometa-source-postgres = '
                      'macrometa_source_postgres:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-postgres',
-    'version': '0.0.51',
+    'version': '0.0.52',
     'description': 'Macrometa Source for extracting data from PostgreSQL.',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-source-postgres-0.0.51/PKG-INFO` & `macrometa-source-postgres-0.0.52/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: macrometa-source-postgres
-Version: 0.0.51
+Version: 0.0.52
 Summary: Macrometa Source for extracting data from PostgreSQL.
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,PostgreSQL,Source
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Requires-Dist: c8connector (>=0.0.24)
 Requires-Dist: pipelinewise-singer-python (==1.2.0)
+Requires-Dist: prometheus-client (==0.16.0)
 Requires-Dist: psycopg2-binary (==2.9.3)
 Requires-Dist: strict-rfc3339 (==0.7)
 Project-URL: Bug Tracker, https://github.com/Macrometacorp/macrometa-source-postgres/issues
```

