# Comparing `tmp/macrometa-source-oracle-0.0.37.tar.gz` & `tmp/macrometa-source-oracle-0.0.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-oracle-0.0.37.tar", max compression
+gzip compressed data, was "macrometa-source-oracle-0.0.38.tar", max compression
```

## Comparing `macrometa-source-oracle-0.0.37.tar` & `macrometa-source-oracle-0.0.38.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rwxr-xr-x   0        0        0     9713 2023-06-14 08:52:56.726589 macrometa-source-oracle-0.0.37/LICENSE
--rw-r--r--   0        0        0     1707 2023-06-14 08:52:56.726589 macrometa-source-oracle-0.0.37/README.md
--rw-r--r--   0        0        0    43158 2023-06-14 08:52:56.726589 macrometa-source-oracle-0.0.37/macrometa_source_oracle/__init__.py
--rwxr-xr-x   0        0        0     7524 2023-06-14 08:52:56.726589 macrometa-source-oracle-0.0.37/macrometa_source_oracle/connection.py
--rwxr-xr-x   0        0        0        0 2023-06-14 08:52:56.726589 macrometa-source-oracle-0.0.37/macrometa_source_oracle/sync_strategies/__init__.py
--rwxr-xr-x   0        0        0     4779 2023-06-14 08:52:56.726589 macrometa-source-oracle-0.0.37/macrometa_source_oracle/sync_strategies/common.py
--rwxr-xr-x   0        0        0     4874 2023-06-14 08:52:56.726589 macrometa-source-oracle-0.0.37/macrometa_source_oracle/sync_strategies/full_table.py
--rwxr-xr-x   0        0        0    17662 2023-06-14 08:52:56.726589 macrometa-source-oracle-0.0.37/macrometa_source_oracle/sync_strategies/log_based.py
--rw-r--r--   0        0        0     1571 2023-06-14 08:52:56.802590 macrometa-source-oracle-0.0.37/pyproject.toml
--rw-r--r--   0        0        0     2747 1970-01-01 00:00:00.000000 macrometa-source-oracle-0.0.37/setup.py
--rw-r--r--   0        0        0     2715 1970-01-01 00:00:00.000000 macrometa-source-oracle-0.0.37/PKG-INFO
+-rwxr-xr-x   0        0        0     9713 2023-07-17 14:09:02.028172 macrometa-source-oracle-0.0.38/LICENSE
+-rw-r--r--   0        0        0     1707 2023-07-17 14:09:02.028172 macrometa-source-oracle-0.0.38/README.md
+-rw-r--r--   0        0        0    43914 2023-07-17 14:09:02.032172 macrometa-source-oracle-0.0.38/macrometa_source_oracle/__init__.py
+-rwxr-xr-x   0        0        0     7524 2023-07-17 14:09:02.032172 macrometa-source-oracle-0.0.38/macrometa_source_oracle/connection.py
+-rwxr-xr-x   0        0        0        0 2023-07-17 14:09:02.032172 macrometa-source-oracle-0.0.38/macrometa_source_oracle/sync_strategies/__init__.py
+-rwxr-xr-x   0        0        0     4779 2023-07-17 14:09:02.032172 macrometa-source-oracle-0.0.38/macrometa_source_oracle/sync_strategies/common.py
+-rwxr-xr-x   0        0        0     4880 2023-07-17 14:09:02.032172 macrometa-source-oracle-0.0.38/macrometa_source_oracle/sync_strategies/full_table.py
+-rwxr-xr-x   0        0        0    17662 2023-07-17 14:09:02.032172 macrometa-source-oracle-0.0.38/macrometa_source_oracle/sync_strategies/log_based.py
+-rw-r--r--   0        0        0     1600 2023-07-17 14:09:02.128174 macrometa-source-oracle-0.0.38/pyproject.toml
+-rw-r--r--   0        0        0     2777 1970-01-01 00:00:00.000000 macrometa-source-oracle-0.0.38/setup.py
+-rw-r--r--   0        0        0     2759 1970-01-01 00:00:00.000000 macrometa-source-oracle-0.0.38/PKG-INFO
```

### Comparing `macrometa-source-oracle-0.0.37/LICENSE` & `macrometa-source-oracle-0.0.38/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-source-oracle-0.0.37/README.md` & `macrometa-source-oracle-0.0.38/README.md`

 * *Files identical despite different names*

### Comparing `macrometa-source-oracle-0.0.37/macrometa_source_oracle/__init__.py` & `macrometa-source-oracle-0.0.38/macrometa_source_oracle/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 #!/usr/bin/env python3
 # pylint: disable=missing-docstring,not-an-iterable,too-many-locals,too-many-arguments,invalid-name
 
 import collections
 import copy
 import itertools
+import os
 
 import pkg_resources
 import singer
 import singer.schema
 from c8connector import C8Connector, ConfigProperty, Sample, SchemaAttribute, SchemaAttributeType, \
                         ConfigAttributeType, ValidationException
 from c8connector import Schema as C8Schema
+from prometheus_client import CollectorRegistry, start_http_server, Counter
 from singer import utils, metadata, get_bookmark
 from singer.catalog import Catalog, CatalogEntry
 from singer.schema import Schema
 
 import macrometa_source_oracle.connection as orc_db
 import macrometa_source_oracle.sync_strategies.common as common
 import macrometa_source_oracle.sync_strategies.full_table as full_table
@@ -43,14 +45,19 @@
     'host',
     'port',
     'user',
     'password',
     'service_name'
 ]
 
+region_label = os.getenv("GDN_FEDERATION", "NA")
+tenant_label = os.getenv("GDN_TENANT", "NA")
+fabric_label = os.getenv("GDN_FABRIC", "NA")
+workflow_label = os.getenv("WORKFLOW_UUID", "NA")
+
 
 class OracleSourceConnector(C8Connector):
     """OracleSourceConnector's C8Connector impl."""
 
     def name(self) -> str:
         """Returns the name of the connector."""
         return "OracleDB"
@@ -995,14 +1002,21 @@
         if replication_method == 'LOG_BASED':
             return True
 
     return False
 
 
 def main_impl():
+    # Create a custom CollectorRegistry
+    registry_package = CollectorRegistry()
+    ingest_errors = Counter('ingest_errors', 'Total number of errors during ingestion',
+                        ['region', 'tenant', 'fabric', 'workflow'], registry=registry_package)
+    LOGGER.info("Oracle source is starting the metrics server.")
+    start_http_server(8000, registry=registry_package)
+
     args = utils.parse_args(REQUIRED_CONFIG_KEYS)
     conn_config = {'user': args.config['user'],
                    'password': args.config['password'],
                    'host': args.config['host'],
                    'port': args.config['port'],
                    'service_name': args.config['service_name'],
                    'multitenant': args.config.get('multitenant', False),
@@ -1024,14 +1038,15 @@
         elif args.catalog:
             state = args.state
             do_sync(conn_config, args.catalog, args.config.get('replication_method', "FULL_TABLE"), state)
         else:
             LOGGER.info("No properties were selected")
     except Exception as e:
         LOGGER.warn('Exception raised: %s', e)
+        ingest_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
         orc_db.delete_wallet_file(conn_config)
         raise e
     orc_db.delete_wallet_file(conn_config)
 
 
 def main():
     try:
```

### Comparing `macrometa-source-oracle-0.0.37/macrometa_source_oracle/connection.py` & `macrometa-source-oracle-0.0.38/macrometa_source_oracle/connection.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-oracle-0.0.37/macrometa_source_oracle/sync_strategies/common.py` & `macrometa-source-oracle-0.0.38/macrometa_source_oracle/sync_strategies/common.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-oracle-0.0.37/macrometa_source_oracle/sync_strategies/full_table.py` & `macrometa-source-oracle-0.0.38/macrometa_source_oracle/sync_strategies/full_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,14 @@
    :return: Updated state
    """
    connection = orc_db.open_connection(conn_config)
    connection.outputtypehandler = common.OutputTypeHandler
 
    cursor = connection.cursor()
    set_session_parameters(cursor, conn_config)
-   time_extracted = utils.now()
 
    first_run = singer.get_bookmark(state, stream.tap_stream_id, 'version') is None
    stream_version = get_stream_version(state, stream)
    state = update_state_version(state, stream, stream_version)
 
    md = metadata.to_map(stream.metadata)
    schema_name = md.get(()).get('schema-name')
@@ -91,19 +90,19 @@
                             FROM {escaped_schema}.{escaped_table}
                             {f'WHERE ORA_ROWSCN >= {str(ora_rowscn)}' if ora_rowscn else ''}
                             ORDER BY ORA_ROWSCN ASC"""
          )
 
       rows_saved = 0
       for row in execute_select(cursor, select_sql):
+          time_extracted = utils.now()
           ora_rowscn = None
           if not is_view:
               ora_rowscn = row[-1]
               row = row[:-1]
-
           record_message = common.row_to_singer_message(stream, row, stream_version, desired_columns, time_extracted)
           singer.write_message(record_message)
 
           if not is_view:
               state = singer.write_bookmark(state, stream.tap_stream_id, 'ORA_ROWSCN', ora_rowscn)
               rows_saved += 1
               if rows_saved % UPDATE_BOOKMARK_PERIOD == 0:
```

### Comparing `macrometa-source-oracle-0.0.37/macrometa_source_oracle/sync_strategies/log_based.py` & `macrometa-source-oracle-0.0.38/macrometa_source_oracle/sync_strategies/log_based.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-oracle-0.0.37/pyproject.toml` & `macrometa-source-oracle-0.0.38/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-oracle"
-version='0.0.37'
+version='0.0.38'
 description = "Macrometa source oracle connector for reading from oracle databases."
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 readme = "README.md"
 homepage = "https://www.macrometa.com/"
 keywords = [
     "ELT",
@@ -29,14 +29,15 @@
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.11"
 c8connector = ">=0.0.24"
 pipelinewise-singer-python = "1.2.0"
 oracledb = "^1.2.2"
 strict-rfc3339 = "^0.7"
+prometheus-client = "0.16.0"
 
 [tool.poetry.scripts]
 macrometa-source-oracle = "macrometa_source_oracle:main"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/Macrometacorp/macrometa-source-oracle/issues"
```

### Comparing `macrometa-source-oracle-0.0.37/setup.py` & `macrometa-source-oracle-0.0.38/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,22 +7,23 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['c8connector>=0.0.24',
  'oracledb>=1.2.2,<2.0.0',
  'pipelinewise-singer-python==1.2.0',
+ 'prometheus-client==0.16.0',
  'strict-rfc3339>=0.7,<0.8']
 
 entry_points = \
 {'console_scripts': ['macrometa-source-oracle = macrometa_source_oracle:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-oracle',
-    'version': '0.0.37',
+    'version': '0.0.38',
     'description': 'Macrometa source oracle connector for reading from oracle databases.',
     'long_description': '# macrometa-source-oracle\n\nMacrometa source connector that extracts data from a [Oracle](https://www.oracle.com/database/) database and produces JSON-formatted data following the [Singer spec](https://github.com/singer-io/getting-started/blob/master/docs/SPEC.md).\n\n## How to use it\n\n### Install and Run\n\nFirst, make sure Python 3 is installed on your system or follow these\ninstallation instructions for [Mac](http://docs.python-guide.org/en/latest/starting/install3/osx/) or\n[Ubuntu](https://www.digitalocean.com/community/tutorials/how-to-install-python-3-and-set-up-a-local-programming-environment-on-ubuntu-16-04).\n\n\nIt\'s recommended to use a virtualenv:\n\n```bash\n  python3 -m venv venv\n  pip install macrometa-source-oracle\n```\n\nor from source using,\n1. Install poetry using https://python-poetry.org/docs/#installation\n2. Run \n    ```bash\n    poetry build\n    pip install dist/macrometa_source_oracle-<version>*.whl\n    ```\n\n### Configuration\n\nRunning the the macrometa source connector independently requires a `config.json` file. \n\nExample configuration:\n\n```json\n{\n  "host": "dev.oracledb.io",\n  "port": 1521,\n  "user": "C##HELLO",\n  "password": "password",\n  "service_name": "ORCLCDB",\n  "filter_schema": "C##HELLO",\n  "filter_table": "CUSTOMERS",\n  "replication_method": "LOG_BASED",\n  "pdb_name": "ORCLPDB1",\n  "multitenant": true,\n  "scn_window_size": 10\n}\n```\n\nYou can run a discover run using the previous `config.json` file to acquire all the tables definition\n \n```\nmacrometa-source-oracle --config /tmp/config.json --discover >> /tmp/catalog.json\n```\n\nThen use the catalog.json to run a full export:\n\n```\nmacrometa-source-oracle --config /tmp/config.json --catalog /tmp/catalog.json\n```\n\n',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://www.macrometa.com/',
```

### Comparing `macrometa-source-oracle-0.0.37/PKG-INFO` & `macrometa-source-oracle-0.0.38/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-source-oracle
-Version: 0.0.37
+Version: 0.0.38
 Summary: Macrometa source oracle connector for reading from oracle databases.
 Home-page: https://www.macrometa.com/
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,Oracle,Source
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Dist: c8connector (>=0.0.24)
 Requires-Dist: oracledb (>=1.2.2,<2.0.0)
 Requires-Dist: pipelinewise-singer-python (==1.2.0)
+Requires-Dist: prometheus-client (==0.16.0)
 Requires-Dist: strict-rfc3339 (>=0.7,<0.8)
 Project-URL: Bug Tracker, https://github.com/Macrometacorp/macrometa-source-oracle/issues
 Description-Content-Type: text/markdown
 
 # macrometa-source-oracle
 
 Macrometa source connector that extracts data from a [Oracle](https://www.oracle.com/database/) database and produces JSON-formatted data following the [Singer spec](https://github.com/singer-io/getting-started/blob/master/docs/SPEC.md).
```

