# Comparing `tmp/dbt-glue-1.5.2.tar.gz` & `tmp/dbt-glue-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-glue-1.5.2.tar", last modified: Wed Jul  5 15:17:39 2023, max compression
+gzip compressed data, was "dbt-glue-1.5.3.tar", last modified: Mon Jul 17 09:35:23 2023, max compression
```

## Comparing `dbt-glue-1.5.2.tar` & `dbt-glue-1.5.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-05 15:17:39.215136 dbt-glue-1.5.2/
--rw-r--r--   0 menuetb    (504) staff       (20)    10142 2022-04-05 16:42:41.000000 dbt-glue-1.5.2/LICENSE
--rw-r--r--   0 menuetb    (504) staff       (20)       67 2022-04-05 16:42:41.000000 dbt-glue-1.5.2/NOTICE
--rw-r--r--   0 menuetb    (504) staff       (20)    44977 2023-07-05 15:17:39.214978 dbt-glue-1.5.2/PKG-INFO
--rw-r--r--   0 menuetb    (504) staff       (20)    44126 2023-07-05 15:16:41.000000 dbt-glue-1.5.2/README.md
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-05 15:17:39.206639 dbt-glue-1.5.2/dbt/
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-05 15:17:39.206338 dbt-glue-1.5.2/dbt/adapters/
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-05 15:17:39.209743 dbt-glue-1.5.2/dbt/adapters/glue/
--rw-r--r--   0 menuetb    (504) staff       (20)      394 2023-04-06 15:48:24.000000 dbt-glue-1.5.2/dbt/adapters/glue/__init__.py
--rw-r--r--   0 menuetb    (504) staff       (20)       17 2023-07-05 12:00:28.000000 dbt-glue-1.5.2/dbt/adapters/glue/__version__.py
--rw-r--r--   0 menuetb    (504) staff       (20)     3917 2023-06-29 08:34:49.000000 dbt-glue-1.5.2/dbt/adapters/glue/connections.py
--rw-r--r--   0 menuetb    (504) staff       (20)     2585 2023-07-05 15:16:41.000000 dbt-glue-1.5.2/dbt/adapters/glue/credentials.py
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-05 15:17:39.210597 dbt-glue-1.5.2/dbt/adapters/glue/gluedbapi/
--rw-r--r--   0 menuetb    (504) staff       (20)      140 2022-04-05 16:42:41.000000 dbt-glue-1.5.2/dbt/adapters/glue/gluedbapi/__init__.py
--rw-r--r--   0 menuetb    (504) staff       (20)     1216 2023-04-27 15:40:43.000000 dbt-glue-1.5.2/dbt/adapters/glue/gluedbapi/commons.py
--rw-r--r--   0 menuetb    (504) staff       (20)     9695 2023-07-05 15:16:41.000000 dbt-glue-1.5.2/dbt/adapters/glue/gluedbapi/connection.py
--rw-r--r--   0 menuetb    (504) staff       (20)     8225 2023-07-05 15:09:54.000000 dbt-glue-1.5.2/dbt/adapters/glue/gluedbapi/cursor.py
--rw-r--r--   0 menuetb    (504) staff       (20)    38143 2023-07-05 15:12:32.000000 dbt-glue-1.5.2/dbt/adapters/glue/impl.py
--rw-r--r--   0 menuetb    (504) staff       (20)     1264 2023-04-07 07:53:59.000000 dbt-glue-1.5.2/dbt/adapters/glue/relation.py
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-05 15:17:39.206747 dbt-glue-1.5.2/dbt/include/
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-05 15:17:39.211117 dbt-glue-1.5.2/dbt/include/glue/
--rw-r--r--   0 menuetb    (504) staff       (20)       51 2022-04-05 16:42:41.000000 dbt-glue-1.5.2/dbt/include/glue/__init__.py
--rw-r--r--   0 menuetb    (504) staff       (20)       72 2022-07-11 06:48:28.000000 dbt-glue-1.5.2/dbt/include/glue/dbt_project.yml
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-05 15:17:39.211353 dbt-glue-1.5.2/dbt/include/glue/macros/
--rw-r--r--   0 menuetb    (504) staff       (20)     5352 2023-01-17 10:30:07.000000 dbt-glue-1.5.2/dbt/include/glue/macros/adapters.sql
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-05 15:17:39.211842 dbt-glue-1.5.2/dbt/include/glue/macros/generic_test_sql/
--rw-r--r--   0 menuetb    (504) staff       (20)      494 2022-07-11 06:48:28.000000 dbt-glue-1.5.2/dbt/include/glue/macros/generic_test_sql/accepted_values.sql
--rw-r--r--   0 menuetb    (504) staff       (20)      370 2022-07-11 06:48:28.000000 dbt-glue-1.5.2/dbt/include/glue/macros/generic_test_sql/relationships.sql
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-05 15:17:39.212517 dbt-glue-1.5.2/dbt/include/glue/macros/materializations/
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-05 15:17:39.213072 dbt-glue-1.5.2/dbt/include/glue/macros/materializations/incremental/
--rw-r--r--   0 menuetb    (504) staff       (20)     4347 2023-06-19 12:11:48.000000 dbt-glue-1.5.2/dbt/include/glue/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 menuetb    (504) staff       (20)     1689 2023-07-05 12:59:31.000000 dbt-glue-1.5.2/dbt/include/glue/macros/materializations/incremental/strategies.sql
--rw-r--r--   0 menuetb    (504) staff       (20)     1436 2023-01-06 16:44:08.000000 dbt-glue-1.5.2/dbt/include/glue/macros/materializations/seed.sql
--rw-r--r--   0 menuetb    (504) staff       (20)    10334 2023-06-29 09:23:22.000000 dbt-glue-1.5.2/dbt/include/glue/macros/materializations/snapshot.sql
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-05 15:17:39.213235 dbt-glue-1.5.2/dbt/include/glue/macros/materializations/table/
--rw-r--r--   0 menuetb    (504) staff       (20)     1159 2022-11-03 13:40:21.000000 dbt-glue-1.5.2/dbt/include/glue/macros/materializations/table/iceberg_table_replace.sql
--rw-r--r--   0 menuetb    (504) staff       (20)      112 2022-07-11 06:48:28.000000 dbt-glue-1.5.2/dbt/include/glue/macros/materializations/view.sql
--rw-r--r--   0 menuetb    (504) staff       (20)      584 2023-06-15 08:24:37.000000 dbt-glue-1.5.2/dbt/include/glue/sample_profiles.yml
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-05 15:17:39.207375 dbt-glue-1.5.2/dbt/include/glue/tests/
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-05 15:17:39.213416 dbt-glue-1.5.2/dbt/include/glue/tests/generic/
--rw-r--r--   0 menuetb    (504) staff       (20)      290 2022-07-11 06:48:28.000000 dbt-glue-1.5.2/dbt/include/glue/tests/generic/builtin.sql
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-05 15:17:39.214594 dbt-glue-1.5.2/dbt_glue.egg-info/
--rw-r--r--   0 menuetb    (504) staff       (20)    44977 2023-07-05 15:17:39.000000 dbt-glue-1.5.2/dbt_glue.egg-info/PKG-INFO
--rw-r--r--   0 menuetb    (504) staff       (20)     1230 2023-07-05 15:17:39.000000 dbt-glue-1.5.2/dbt_glue.egg-info/SOURCES.txt
--rw-r--r--   0 menuetb    (504) staff       (20)        1 2023-07-05 15:17:39.000000 dbt-glue-1.5.2/dbt_glue.egg-info/dependency_links.txt
--rw-r--r--   0 menuetb    (504) staff       (20)        1 2022-05-12 16:43:26.000000 dbt-glue-1.5.2/dbt_glue.egg-info/not-zip-safe
--rw-r--r--   0 menuetb    (504) staff       (20)       46 2023-07-05 15:17:39.000000 dbt-glue-1.5.2/dbt_glue.egg-info/requires.txt
--rw-r--r--   0 menuetb    (504) staff       (20)        4 2023-07-05 15:17:39.000000 dbt-glue-1.5.2/dbt_glue.egg-info/top_level.txt
--rw-r--r--   0 menuetb    (504) staff       (20)       38 2023-07-05 15:17:39.215198 dbt-glue-1.5.2/setup.cfg
--rw-r--r--   0 menuetb    (504) staff       (20)     2857 2023-06-29 08:57:00.000000 dbt-glue-1.5.2/setup.py
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-17 09:35:23.126378 dbt-glue-1.5.3/
+-rw-r--r--   0 menuetb    (504) staff       (20)    10142 2022-04-05 16:42:41.000000 dbt-glue-1.5.3/LICENSE
+-rw-r--r--   0 menuetb    (504) staff       (20)       67 2022-04-05 16:42:41.000000 dbt-glue-1.5.3/NOTICE
+-rw-r--r--   0 menuetb    (504) staff       (20)    44977 2023-07-17 09:35:23.126216 dbt-glue-1.5.3/PKG-INFO
+-rw-r--r--   0 menuetb    (504) staff       (20)    44126 2023-07-05 15:16:41.000000 dbt-glue-1.5.3/README.md
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-17 09:35:23.118651 dbt-glue-1.5.3/dbt/
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-17 09:35:23.118465 dbt-glue-1.5.3/dbt/adapters/
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-17 09:35:23.121748 dbt-glue-1.5.3/dbt/adapters/glue/
+-rw-r--r--   0 menuetb    (504) staff       (20)      394 2023-04-06 15:48:24.000000 dbt-glue-1.5.3/dbt/adapters/glue/__init__.py
+-rw-r--r--   0 menuetb    (504) staff       (20)       17 2023-07-17 09:34:17.000000 dbt-glue-1.5.3/dbt/adapters/glue/__version__.py
+-rw-r--r--   0 menuetb    (504) staff       (20)     3917 2023-06-29 08:34:49.000000 dbt-glue-1.5.3/dbt/adapters/glue/connections.py
+-rw-r--r--   0 menuetb    (504) staff       (20)     2585 2023-07-05 15:16:41.000000 dbt-glue-1.5.3/dbt/adapters/glue/credentials.py
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-17 09:35:23.122421 dbt-glue-1.5.3/dbt/adapters/glue/gluedbapi/
+-rw-r--r--   0 menuetb    (504) staff       (20)      140 2022-04-05 16:42:41.000000 dbt-glue-1.5.3/dbt/adapters/glue/gluedbapi/__init__.py
+-rw-r--r--   0 menuetb    (504) staff       (20)     1216 2023-04-27 15:40:43.000000 dbt-glue-1.5.3/dbt/adapters/glue/gluedbapi/commons.py
+-rw-r--r--   0 menuetb    (504) staff       (20)     9946 2023-07-17 09:33:44.000000 dbt-glue-1.5.3/dbt/adapters/glue/gluedbapi/connection.py
+-rw-r--r--   0 menuetb    (504) staff       (20)     8225 2023-07-05 15:09:54.000000 dbt-glue-1.5.3/dbt/adapters/glue/gluedbapi/cursor.py
+-rw-r--r--   0 menuetb    (504) staff       (20)    38602 2023-07-17 09:33:44.000000 dbt-glue-1.5.3/dbt/adapters/glue/impl.py
+-rw-r--r--   0 menuetb    (504) staff       (20)     1264 2023-04-07 07:53:59.000000 dbt-glue-1.5.3/dbt/adapters/glue/relation.py
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-17 09:35:23.118709 dbt-glue-1.5.3/dbt/include/
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-17 09:35:23.123015 dbt-glue-1.5.3/dbt/include/glue/
+-rw-r--r--   0 menuetb    (504) staff       (20)       51 2022-04-05 16:42:41.000000 dbt-glue-1.5.3/dbt/include/glue/__init__.py
+-rw-r--r--   0 menuetb    (504) staff       (20)       72 2022-07-11 06:48:28.000000 dbt-glue-1.5.3/dbt/include/glue/dbt_project.yml
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-17 09:35:23.123253 dbt-glue-1.5.3/dbt/include/glue/macros/
+-rw-r--r--   0 menuetb    (504) staff       (20)     5352 2023-01-17 10:30:07.000000 dbt-glue-1.5.3/dbt/include/glue/macros/adapters.sql
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-17 09:35:23.123708 dbt-glue-1.5.3/dbt/include/glue/macros/generic_test_sql/
+-rw-r--r--   0 menuetb    (504) staff       (20)      494 2022-07-11 06:48:28.000000 dbt-glue-1.5.3/dbt/include/glue/macros/generic_test_sql/accepted_values.sql
+-rw-r--r--   0 menuetb    (504) staff       (20)      370 2022-07-11 06:48:28.000000 dbt-glue-1.5.3/dbt/include/glue/macros/generic_test_sql/relationships.sql
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-17 09:35:23.124302 dbt-glue-1.5.3/dbt/include/glue/macros/materializations/
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-17 09:35:23.124611 dbt-glue-1.5.3/dbt/include/glue/macros/materializations/incremental/
+-rw-r--r--   0 menuetb    (504) staff       (20)     4453 2023-07-17 09:33:44.000000 dbt-glue-1.5.3/dbt/include/glue/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 menuetb    (504) staff       (20)     1689 2023-07-05 12:59:31.000000 dbt-glue-1.5.3/dbt/include/glue/macros/materializations/incremental/strategies.sql
+-rw-r--r--   0 menuetb    (504) staff       (20)     1436 2023-01-06 16:44:08.000000 dbt-glue-1.5.3/dbt/include/glue/macros/materializations/seed.sql
+-rw-r--r--   0 menuetb    (504) staff       (20)    10334 2023-06-29 09:23:22.000000 dbt-glue-1.5.3/dbt/include/glue/macros/materializations/snapshot.sql
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-17 09:35:23.124867 dbt-glue-1.5.3/dbt/include/glue/macros/materializations/table/
+-rw-r--r--   0 menuetb    (504) staff       (20)     1159 2022-11-03 13:40:21.000000 dbt-glue-1.5.3/dbt/include/glue/macros/materializations/table/iceberg_table_replace.sql
+-rw-r--r--   0 menuetb    (504) staff       (20)      112 2022-07-11 06:48:28.000000 dbt-glue-1.5.3/dbt/include/glue/macros/materializations/view.sql
+-rw-r--r--   0 menuetb    (504) staff       (20)      584 2023-06-15 08:24:37.000000 dbt-glue-1.5.3/dbt/include/glue/sample_profiles.yml
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-17 09:35:23.119310 dbt-glue-1.5.3/dbt/include/glue/tests/
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-17 09:35:23.125028 dbt-glue-1.5.3/dbt/include/glue/tests/generic/
+-rw-r--r--   0 menuetb    (504) staff       (20)      290 2022-07-11 06:48:28.000000 dbt-glue-1.5.3/dbt/include/glue/tests/generic/builtin.sql
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-17 09:35:23.125943 dbt-glue-1.5.3/dbt_glue.egg-info/
+-rw-r--r--   0 menuetb    (504) staff       (20)    44977 2023-07-17 09:35:23.000000 dbt-glue-1.5.3/dbt_glue.egg-info/PKG-INFO
+-rw-r--r--   0 menuetb    (504) staff       (20)     1230 2023-07-17 09:35:23.000000 dbt-glue-1.5.3/dbt_glue.egg-info/SOURCES.txt
+-rw-r--r--   0 menuetb    (504) staff       (20)        1 2023-07-17 09:35:23.000000 dbt-glue-1.5.3/dbt_glue.egg-info/dependency_links.txt
+-rw-r--r--   0 menuetb    (504) staff       (20)        1 2022-05-12 16:43:26.000000 dbt-glue-1.5.3/dbt_glue.egg-info/not-zip-safe
+-rw-r--r--   0 menuetb    (504) staff       (20)       46 2023-07-17 09:35:23.000000 dbt-glue-1.5.3/dbt_glue.egg-info/requires.txt
+-rw-r--r--   0 menuetb    (504) staff       (20)        4 2023-07-17 09:35:23.000000 dbt-glue-1.5.3/dbt_glue.egg-info/top_level.txt
+-rw-r--r--   0 menuetb    (504) staff       (20)       38 2023-07-17 09:35:23.126430 dbt-glue-1.5.3/setup.cfg
+-rw-r--r--   0 menuetb    (504) staff       (20)     2857 2023-06-29 08:57:00.000000 dbt-glue-1.5.3/setup.py
```

### Comparing `dbt-glue-1.5.2/LICENSE` & `dbt-glue-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.5.2/PKG-INFO` & `dbt-glue-1.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-glue
-Version: 1.5.2
+Version: 1.5.3
 Summary: dbt (data build tool) adapter for Aws Glue
 Home-page: https://github.com/aws-samples/dbt-glue
 Author: moshirm,menuetb,mamallem,segnina
 Author-email: moshirm@amazon.fr, menuetb@amazon.fr, mamallem@amazon.fr, segnina@amazon.fr 
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `dbt-glue-1.5.2/README.md` & `dbt-glue-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.5.2/dbt/adapters/glue/connections.py` & `dbt-glue-1.5.3/dbt/adapters/glue/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.5.2/dbt/adapters/glue/credentials.py` & `dbt-glue-1.5.3/dbt/adapters/glue/credentials.py`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.5.2/dbt/adapters/glue/gluedbapi/commons.py` & `dbt-glue-1.5.3/dbt/adapters/glue/gluedbapi/commons.py`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.5.2/dbt/adapters/glue/gluedbapi/connection.py` & `dbt-glue-1.5.3/dbt/adapters/glue/gluedbapi/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import boto3
 from botocore.config import Config
 from waiter import wait
 from dbt.adapters.glue.gluedbapi.cursor import GlueCursor, GlueDictCursor
 from dbt.adapters.glue.credentials import GlueCredentials
 from dbt.adapters.glue.gluedbapi.commons import GlueStatement
 import time
+import threading
 import uuid
 from dbt.events import AdapterLogger
 
 logger = AdapterLogger("Glue")
 
 
 class GlueSessionState:
@@ -19,14 +20,15 @@
     PROVISIONING = "PROVISIONING"
     RUNNING = "RUNNING"
     CLOSED = "CLOSED"
 
 
 @dataclass
 class GlueConnection:
+    _boto3_client_lock = threading.Lock()
 
     def __init__(self, credentials: GlueCredentials, session_id: str = None):
         self.credentials = credentials
         self._session_id = session_id
         self._client = None
         self._session = None
         self._state = None
@@ -136,15 +138,18 @@
         config = Config(
             retries={
                 'max_attempts': 10,
                 'mode': 'adaptive'
             }
         )
         if not self._client:
-            self._client = boto3.client("glue", region_name=self.credentials.region, config=config)
+            # refernce on why lock is required - https://stackoverflow.com/a/61943955/6034432
+            with self._boto3_client_lock:
+                session = boto3.session.Session()
+                self._client = session.client("glue", region_name=self.credentials.region, config=config)
         return self._client
 
     def cancel_statement(self, statement_id):
         logger.debug("GlueConnection cancel_statement called")
         self.client.cancel_statement(
             SessionId=self.session_id,
             Id=statement_id
```

### Comparing `dbt-glue-1.5.2/dbt/adapters/glue/gluedbapi/cursor.py` & `dbt-glue-1.5.3/dbt/adapters/glue/gluedbapi/cursor.py`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.5.2/dbt/adapters/glue/impl.py` & `dbt-glue-1.5.3/dbt/adapters/glue/impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -635,15 +635,15 @@
     def hudi_write(self, write_mode, session, target_relation, custom_location):
         if custom_location == "empty":
             return f'''outputDf.write.format('org.apache.hudi').options(**combinedConf).mode('{write_mode}').save("{session.credentials.location}/{target_relation.schema}/{target_relation.name}/")'''
         else:
             return f'''outputDf.write.format('org.apache.hudi').options(**combinedConf).mode('{write_mode}').save("{custom_location}/")'''
 
     @available
-    def hudi_merge_table(self, target_relation, request, primary_key, partition_key, custom_location, hudi_config):
+    def hudi_merge_table(self, target_relation, request, primary_key, partition_key, custom_location, hudi_config, substitute_variables):
         session, client = self.get_connection()
         isTableExists = False
         if self.check_relation_exists(target_relation):
             isTableExists = True
         else:
             isTableExists = False
 
@@ -698,16 +698,24 @@
 
         code = f'''
 custom_glue_code_for_dbt_adapter
 from pyspark.sql import SparkSession
 from pyspark.sql.functions import *
 spark = SparkSession.builder \
 .config("spark.serializer", "org.apache.spark.serializer.KryoSerializer") \
+.config("hoodie.metadata.enable", "true") \
+.config("hoodie.enable.data.skipping", "true") \
+.config("hoodie.metadata.index.column.stats.enable", "true") \
+.config("hoodie.metadata.index.bloom.filter.enable", "true") \
 .getOrCreate()
-inputDf = spark.sql("""{request}""")
+request = """{request}"""
+substitute_variables = {str(substitute_variables)}
+for index, value in enumerate(substitute_variables):
+    request=eval(f"request.replace(f'<SUBSTITUTE_VARIABLE_{{index}}>',str(eval('{{value}}')))")
+inputDf = spark.sql(request)
 outputDf = inputDf.drop("dbt_unique_key").withColumn("update_hudi_ts",current_timestamp())
 if outputDf.count() > 0:
         parallelism = spark.conf.get("spark.default.parallelism")
         print("spark.default.parallelism: %s", parallelism)
         hudi_parallelism_options = {{
             "hoodie.upsert.shuffle.parallelism": parallelism,
             "hoodie.bulkinsert.shuffle.parallelism": parallelism,
```

### Comparing `dbt-glue-1.5.2/dbt/adapters/glue/relation.py` & `dbt-glue-1.5.3/dbt/adapters/glue/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.5.2/dbt/include/glue/macros/adapters.sql` & `dbt-glue-1.5.3/dbt/include/glue/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.5.2/dbt/include/glue/macros/materializations/incremental/incremental.sql` & `dbt-glue-1.5.3/dbt/include/glue/macros/materializations/incremental/incremental.sql`

 * *Files 2% similar despite different names*

```diff
@@ -30,18 +30,19 @@
   {% set is_incremental = 'False' %}
 
   {% call statement() %}
     set spark.sql.autoBroadcastJoinThreshold=-1
   {% endcall %}
 
   {{ run_hooks(pre_hooks) }}
+  {%- set substitute_variables = config.get('substitute_variables', default=[]) -%}
 
   {% if file_format == 'hudi' %}
         {%- set hudi_options = config.get('hudi_options', default={}) -%}
-        {{ adapter.hudi_merge_table(target_relation, sql, unique_key, partition_by, custom_location, hudi_options) }}
+        {{ adapter.hudi_merge_table(target_relation, sql, unique_key, partition_by, custom_location, hudi_options, substitute_variables) }}
         {% set build_sql = "select * from " + target_relation.schema + "." + target_relation.identifier + " limit 1 "%}
   {% elif file_format == 'iceberg' %}
         {{ adapter.iceberg_write(target_relation, sql, unique_key, partition_by, custom_location, strategy, table_properties) }}
         {% set build_sql = "select * from glue_catalog." + target_relation.schema + "." + target_relation.identifier + " limit 1 "%}
         {%- if expire_snapshots == 'True' -%}
   	      {%- set result = adapter.iceberg_expire_snapshots(target_relation) -%}
         {%- endif -%}
```

### Comparing `dbt-glue-1.5.2/dbt/include/glue/macros/materializations/incremental/strategies.sql` & `dbt-glue-1.5.3/dbt/include/glue/macros/materializations/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.5.2/dbt/include/glue/macros/materializations/seed.sql` & `dbt-glue-1.5.3/dbt/include/glue/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.5.2/dbt/include/glue/macros/materializations/snapshot.sql` & `dbt-glue-1.5.3/dbt/include/glue/macros/materializations/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.5.2/dbt/include/glue/macros/materializations/table/iceberg_table_replace.sql` & `dbt-glue-1.5.3/dbt/include/glue/macros/materializations/table/iceberg_table_replace.sql`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.5.2/dbt/include/glue/sample_profiles.yml` & `dbt-glue-1.5.3/dbt/include/glue/sample_profiles.yml`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.5.2/dbt_glue.egg-info/PKG-INFO` & `dbt-glue-1.5.3/dbt_glue.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-glue
-Version: 1.5.2
+Version: 1.5.3
 Summary: dbt (data build tool) adapter for Aws Glue
 Home-page: https://github.com/aws-samples/dbt-glue
 Author: moshirm,menuetb,mamallem,segnina
 Author-email: moshirm@amazon.fr, menuetb@amazon.fr, mamallem@amazon.fr, segnina@amazon.fr 
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `dbt-glue-1.5.2/dbt_glue.egg-info/SOURCES.txt` & `dbt-glue-1.5.3/dbt_glue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.5.2/setup.py` & `dbt-glue-1.5.3/setup.py`

 * *Files identical despite different names*

