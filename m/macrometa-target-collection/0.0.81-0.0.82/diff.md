# Comparing `tmp/macrometa-target-collection-0.0.81.tar.gz` & `tmp/macrometa-target-collection-0.0.82.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-collection-0.0.81.tar", last modified: Fri Jul 14 08:39:22 2023, max compression
+gzip compressed data, was "macrometa-target-collection-0.0.82.tar", last modified: Mon Jul 17 05:29:03 2023, max compression
```

## Comparing `macrometa-target-collection-0.0.81.tar` & `macrometa-target-collection-0.0.82.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:39:22.439684 macrometa-target-collection-0.0.81/
--rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-07-14 08:38:55.000000 macrometa-target-collection-0.0.81/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-07-14 08:39:22.443684 macrometa-target-collection-0.0.81/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-14 08:38:55.000000 macrometa-target-collection-0.0.81/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:39:22.439684 macrometa-target-collection-0.0.81/macrometa_target_collection/
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-07-14 08:38:55.000000 macrometa-target-collection-0.0.81/macrometa_target_collection/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16271 2023-07-14 08:38:55.000000 macrometa-target-collection-0.0.81/macrometa_target_collection/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:39:22.439684 macrometa-target-collection-0.0.81/macrometa_target_collection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-07-14 08:39:22.000000 macrometa-target-collection-0.0.81/macrometa_target_collection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-14 08:39:22.000000 macrometa-target-collection-0.0.81/macrometa_target_collection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 08:39:22.000000 macrometa-target-collection-0.0.81/macrometa_target_collection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-14 08:39:22.000000 macrometa-target-collection-0.0.81/macrometa_target_collection.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-14 08:39:22.000000 macrometa-target-collection-0.0.81/macrometa_target_collection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-14 08:39:22.000000 macrometa-target-collection-0.0.81/macrometa_target_collection.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-14 08:38:55.000000 macrometa-target-collection-0.0.81/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-14 08:39:22.443684 macrometa-target-collection-0.0.81/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 05:29:03.271810 macrometa-target-collection-0.0.82/
+-rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-07-17 05:28:38.000000 macrometa-target-collection-0.0.82/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-07-17 05:29:03.271810 macrometa-target-collection-0.0.82/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-17 05:28:38.000000 macrometa-target-collection-0.0.82/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 05:29:03.271810 macrometa-target-collection-0.0.82/macrometa_target_collection/
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-07-17 05:28:38.000000 macrometa-target-collection-0.0.82/macrometa_target_collection/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16617 2023-07-17 05:28:38.000000 macrometa-target-collection-0.0.82/macrometa_target_collection/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 05:29:03.271810 macrometa-target-collection-0.0.82/macrometa_target_collection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-07-17 05:29:03.000000 macrometa-target-collection-0.0.82/macrometa_target_collection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-17 05:29:03.000000 macrometa-target-collection-0.0.82/macrometa_target_collection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 05:29:03.000000 macrometa-target-collection-0.0.82/macrometa_target_collection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-17 05:29:03.000000 macrometa-target-collection-0.0.82/macrometa_target_collection.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-17 05:29:03.000000 macrometa-target-collection-0.0.82/macrometa_target_collection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-17 05:29:03.000000 macrometa-target-collection-0.0.82/macrometa_target_collection.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-17 05:28:38.000000 macrometa-target-collection-0.0.82/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-17 05:29:03.271810 macrometa-target-collection-0.0.82/setup.cfg
```

### Comparing `macrometa-target-collection-0.0.81/LICENSE` & `macrometa-target-collection-0.0.82/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.81/PKG-INFO` & `macrometa-target-collection-0.0.82/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.81
+Version: 0.0.82
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.81/macrometa_target_collection/__init__.py` & `macrometa-target-collection-0.0.82/macrometa_target_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.81/macrometa_target_collection/main.py` & `macrometa-target-collection-0.0.82/macrometa_target_collection/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,52 +14,51 @@
 import jsonschema
 import requests
 from adjust_precision_for_schema import adjust_decimal_precision_for_schema
 from c8 import C8Client, DocumentInsertError, DocumentUpdateError, DocumentRevisionError
 from c8.collection import StandardCollection
 from c8connector import ensure_datetime
 from jsonschema import Draft4Validator
-from prometheus_client import Counter, Gauge, start_http_server
+from prometheus_client import CollectorRegistry, Counter, Gauge, start_http_server
 from singer import get_logger
 from typing import AsyncIterable
 
 from macrometa_target_collection import extract_gdn_host
 
 logger = get_logger('macrometa_target_collection')
 
 DEFAULT_BATCH_SIZE_ROWS = 500
 DEFAULT_BATCH_FLUSH_INTERVAL = 10
 DEFAULT_MIN_BATCH_FLUSH_TIME_GAP = 10
 
 # Prometheus metrics
-ingested_bytes = Counter('ingested_bytes', 'Total number of bytes ingested', ['region', 'tenant', 'fabric', 'workflow'])
+# Create a custom CollectorRegistry
+registry_package = CollectorRegistry()
+ingested_bytes = Counter('ingested_bytes', 'Total number of bytes ingested', ['region', 'tenant', 'fabric', 'workflow'],
+                         registry=registry_package)
 ingested_documents = Counter('ingested_documents', 'Total number of documents ingested',
-                             ['region', 'tenant', 'fabric', 'workflow'])
+                             ['region', 'tenant', 'fabric', 'workflow'], registry=registry_package)
 ingest_errors = Counter('ingest_errors', 'Total number of errors during ingestion',
-                        ['region', 'tenant', 'fabric', 'workflow'])
+                        ['region', 'tenant', 'fabric', 'workflow'], registry=registry_package)
 ingest_lag = Gauge('ingest_lag', 'Average time lag between data changes in GDN collections and external data sources',
-                   ['region', 'tenant', 'fabric', 'workflow'])
+                   ['region', 'tenant', 'fabric', 'workflow'], registry=registry_package)
 export_lag = Gauge("export_lag", "The average time from when the data changes in GDN collections are reflected in external data sources",
-                   ['region', 'tenant', 'fabric', 'workflow'])
+                   ['region', 'tenant', 'fabric', 'workflow'], registry=registry_package)
 export_errors = Counter("export_errors", "Total count of errors while exporting data from GDN collections",
-                        ['region', 'tenant', 'fabric', 'workflow'])
+                        ['region', 'tenant', 'fabric', 'workflow'], registry=registry_package)
 scrape_complete_flag = Counter("scrape_complete_flag", "Flag to check if the last scrape has been completed",
-                               ['workflow'])
+                               ['workflow'], registry=registry_package)
 
 region_label = os.getenv("GDN_FEDERATION", "NA")
 tenant_label = os.getenv("GDN_TENANT", "NA")
 fabric_label = os.getenv("GDN_FABRIC", "NA")
 workflow_label = os.getenv("WORKFLOW_UUID", "NA")
 metric_service_url = os.getenv("METRIC_SERVICE_API")
 is_metrics_enabled = os.getenv("MACROMETA_TARGET_COLLECTION_IS_METRICS_ENABLED", 'False')
 
-# Start the Prometheus HTTP server for exposing metrics
-logger.info("Macrometa target is starting the metrics server.")
-start_http_server(8001)
-
 
 class RecordBatch:
     """Class wrapping the record batch in order to make it thread safe."""
 
     def __init__(self, config: dict):
         self._list = list()
         self._delete_list = set()
@@ -335,14 +334,17 @@
         timedelta = datetime.now(timezone.utc) - record_batch.last_executed_time
         if timedelta.total_seconds() >= record_batch.min_time_gap:
             # if batch has records that need to be processed but haven't reached batch size then process them.
             try_upsert(collection, record_batch, force=True)
 
 
 async def main_impl():
+    # Start the Prometheus HTTP server for exposing metrics
+    logger.info("Macrometa target is starting the metrics server.")
+    start_http_server(8001, registry=registry_package)
     parser = argparse.ArgumentParser()
     parser.add_argument('-c', '--config', help='Config file')
     args = parser.parse_args()
     if args.config:
         with open(args.config) as input_json:
             config = json.load(input_json)
     else:
```

### Comparing `macrometa-target-collection-0.0.81/macrometa_target_collection.egg-info/PKG-INFO` & `macrometa-target-collection-0.0.82/macrometa_target_collection.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.81
+Version: 0.0.82
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.81/pyproject.toml` & `macrometa-target-collection-0.0.82/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "macrometa-target-collection"
-version = "0.0.81"
+version = "0.0.82"
 authors = [
     { name = "Macrometa", email = "info@macrometa.co" },
 ]
 description = "Singer.io target for writing to Macrometa GDN collections"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
```

