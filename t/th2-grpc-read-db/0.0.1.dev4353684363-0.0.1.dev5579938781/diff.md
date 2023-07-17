# Comparing `tmp/th2_grpc_read_db-0.0.1.dev4353684363.tar.gz` & `tmp/th2_grpc_read_db-0.0.1.dev5579938781.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_grpc_read_db-0.0.1.dev4353684363.tar", last modified: Tue Mar  7 11:37:32 2023, max compression
+gzip compressed data, was "dist/th2_grpc_read_db-0.0.1.dev5579938781.tar", last modified: Mon Jul 17 19:49:51 2023, max compression
```

## Comparing `th2_grpc_read_db-0.0.1.dev4353684363.tar` & `th2_grpc_read_db-0.0.1.dev5579938781.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 11:37:32.000000 th2_grpc_read_db-0.0.1.dev4353684363/
--rw-r--r--   0 runner    (1001) docker     (122)      617 2023-03-07 11:37:32.000000 th2_grpc_read_db-0.0.1.dev4353684363/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      236 2023-03-07 11:36:23.000000 th2_grpc_read_db-0.0.1.dev4353684363/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-03-07 11:36:23.000000 th2_grpc_read_db-0.0.1.dev4353684363/package_info.json
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-07 11:37:32.000000 th2_grpc_read_db-0.0.1.dev4353684363/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4495 2023-03-07 11:36:23.000000 th2_grpc_read_db-0.0.1.dev4353684363/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 11:37:32.000000 th2_grpc_read_db-0.0.1.dev4353684363/th2_grpc_read_db/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-07 11:37:32.000000 th2_grpc_read_db-0.0.1.dev4353684363/th2_grpc_read_db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-07 11:37:32.000000 th2_grpc_read_db-0.0.1.dev4353684363/th2_grpc_read_db/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     1310 2023-03-07 11:36:23.000000 th2_grpc_read_db-0.0.1.dev4353684363/th2_grpc_read_db/read_db.proto
--rw-r--r--   0 runner    (1001) docker     (122)     4526 2023-03-07 11:37:32.000000 th2_grpc_read_db-0.0.1.dev4353684363/th2_grpc_read_db/read_db_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)     8899 2023-03-07 11:37:32.000000 th2_grpc_read_db-0.0.1.dev4353684363/th2_grpc_read_db/read_db_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     5934 2023-03-07 11:37:32.000000 th2_grpc_read_db-0.0.1.dev4353684363/th2_grpc_read_db/read_db_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)      660 2023-03-07 11:37:14.000000 th2_grpc_read_db-0.0.1.dev4353684363/th2_grpc_read_db/read_db_service.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 11:37:32.000000 th2_grpc_read_db-0.0.1.dev4353684363/th2_grpc_read_db.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      617 2023-03-07 11:37:32.000000 th2_grpc_read_db-0.0.1.dev4353684363/th2_grpc_read_db.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      459 2023-03-07 11:37:32.000000 th2_grpc_read_db-0.0.1.dev4353684363/th2_grpc_read_db.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-07 11:37:32.000000 th2_grpc_read_db-0.0.1.dev4353684363/th2_grpc_read_db.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-03-07 11:37:32.000000 th2_grpc_read_db-0.0.1.dev4353684363/th2_grpc_read_db.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-03-07 11:37:32.000000 th2_grpc_read_db-0.0.1.dev4353684363/th2_grpc_read_db.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 19:49:51.000000 th2_grpc_read_db-0.0.1.dev5579938781/
+-rw-r--r--   0 runner    (1001) docker     (122)      617 2023-07-17 19:49:51.000000 th2_grpc_read_db-0.0.1.dev5579938781/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      236 2023-07-17 19:48:31.000000 th2_grpc_read_db-0.0.1.dev5579938781/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-07-17 19:48:32.000000 th2_grpc_read_db-0.0.1.dev5579938781/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-17 19:49:51.000000 th2_grpc_read_db-0.0.1.dev5579938781/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4495 2023-07-17 19:48:31.000000 th2_grpc_read_db-0.0.1.dev5579938781/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 19:49:51.000000 th2_grpc_read_db-0.0.1.dev5579938781/th2_grpc_read_db/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 19:49:51.000000 th2_grpc_read_db-0.0.1.dev5579938781/th2_grpc_read_db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 19:49:51.000000 th2_grpc_read_db-0.0.1.dev5579938781/th2_grpc_read_db/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     1310 2023-07-17 19:48:31.000000 th2_grpc_read_db-0.0.1.dev5579938781/th2_grpc_read_db/read_db.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     4526 2023-07-17 19:49:50.000000 th2_grpc_read_db-0.0.1.dev5579938781/th2_grpc_read_db/read_db_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8899 2023-07-17 19:49:50.000000 th2_grpc_read_db-0.0.1.dev5579938781/th2_grpc_read_db/read_db_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     5934 2023-07-17 19:49:50.000000 th2_grpc_read_db-0.0.1.dev5579938781/th2_grpc_read_db/read_db_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)      660 2023-07-17 19:49:24.000000 th2_grpc_read_db-0.0.1.dev5579938781/th2_grpc_read_db/read_db_service.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 19:49:51.000000 th2_grpc_read_db-0.0.1.dev5579938781/th2_grpc_read_db.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      617 2023-07-17 19:49:51.000000 th2_grpc_read_db-0.0.1.dev5579938781/th2_grpc_read_db.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      459 2023-07-17 19:49:51.000000 th2_grpc_read_db-0.0.1.dev5579938781/th2_grpc_read_db.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-17 19:49:51.000000 th2_grpc_read_db-0.0.1.dev5579938781/th2_grpc_read_db.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-07-17 19:49:51.000000 th2_grpc_read_db-0.0.1.dev5579938781/th2_grpc_read_db.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-17 19:49:51.000000 th2_grpc_read_db-0.0.1.dev5579938781/th2_grpc_read_db.egg-info/top_level.txt
```

### Comparing `th2_grpc_read_db-0.0.1.dev4353684363/PKG-INFO` & `th2_grpc_read_db-0.0.1.dev5579938781/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: th2_grpc_read_db
-Version: 0.0.1.dev4353684363
+Version: 0.0.1.dev5579938781
 Summary: th2_grpc_read_db
 Home-page: https://github.com/th2-net/th2-read-db
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # gRPC for read-db
```

### Comparing `th2_grpc_read_db-0.0.1.dev4353684363/setup.py` & `th2_grpc_read_db-0.0.1.dev5579938781/setup.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_read_db-0.0.1.dev4353684363/th2_grpc_read_db/read_db.proto` & `th2_grpc_read_db-0.0.1.dev5579938781/th2_grpc_read_db/read_db.proto`

 * *Files identical despite different names*

### Comparing `th2_grpc_read_db-0.0.1.dev4353684363/th2_grpc_read_db/read_db_pb2.py` & `th2_grpc_read_db-0.0.1.dev5579938781/th2_grpc_read_db/read_db_pb2.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_read_db-0.0.1.dev4353684363/th2_grpc_read_db/read_db_pb2.pyi` & `th2_grpc_read_db-0.0.1.dev5579938781/th2_grpc_read_db/read_db_pb2.pyi`

 * *Files identical despite different names*

### Comparing `th2_grpc_read_db-0.0.1.dev4353684363/th2_grpc_read_db/read_db_pb2_grpc.py` & `th2_grpc_read_db-0.0.1.dev5579938781/th2_grpc_read_db/read_db_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_read_db-0.0.1.dev4353684363/th2_grpc_read_db/read_db_service.py` & `th2_grpc_read_db-0.0.1.dev5579938781/th2_grpc_read_db/read_db_service.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_read_db-0.0.1.dev4353684363/th2_grpc_read_db.egg-info/PKG-INFO` & `th2_grpc_read_db-0.0.1.dev5579938781/th2_grpc_read_db.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: th2-grpc-read-db
-Version: 0.0.1.dev4353684363
+Version: 0.0.1.dev5579938781
 Summary: th2_grpc_read_db
 Home-page: https://github.com/th2-net/th2-read-db
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # gRPC for read-db
```

