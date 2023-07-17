# Comparing `tmp/hubmap-commons-2.1.7.tar.gz` & `tmp/hubmap-commons-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hubmap-commons-2.1.7.tar", last modified: Fri Jul 14 15:38:59 2023, max compression
+gzip compressed data, was "hubmap-commons-2.1.8.tar", last modified: Mon Jul 17 15:44:24 2023, max compression
```

## Comparing `hubmap-commons-2.1.7.tar` & `hubmap-commons-2.1.8.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2023-07-14 15:38:59.360231 hubmap-commons-2.1.7/
--rw-r--r--   0 ZHY19      (503) staff       (20)     3354 2023-07-14 15:38:59.359991 hubmap-commons-2.1.7/PKG-INFO
--rw-r--r--   0 ZHY19      (503) staff       (20)     2893 2023-07-14 15:38:14.000000 hubmap-commons-2.1.7/README.md
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2023-07-14 15:38:59.338535 hubmap-commons-2.1.7/hubmap_commons/
--rw-r--r--   0 ZHY19      (503) staff       (20)    20007 2023-07-14 15:38:14.000000 hubmap-commons-2.1.7/hubmap_commons/21f293b0-globus-groups.json
--rw-r--r--   0 ZHY19      (503) staff       (20)     3095 2023-07-14 15:38:14.000000 hubmap-commons-2.1.7/hubmap_commons/21f293b0-process-user.json
--rw-r--r--   0 ZHY19      (503) staff       (20)     3665 2023-07-14 15:38:14.000000 hubmap-commons-2.1.7/hubmap_commons/S3_worker.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     5788 2023-07-14 15:38:14.000000 hubmap-commons-2.1.7/hubmap_commons/activity.py
--rw-r--r--   0 ZHY19      (503) staff       (20)      221 2023-07-14 15:38:14.000000 hubmap-commons-2.1.7/hubmap_commons/autherror.py
--rw-r--r--   0 ZHY19      (503) staff       (20)    12776 2023-07-14 15:38:14.000000 hubmap-commons-2.1.7/hubmap_commons/c4018852-globus-groups.json
--rw-r--r--   0 ZHY19      (503) staff       (20)     3095 2023-07-14 15:38:14.000000 hubmap-commons-2.1.7/hubmap_commons/c4018852-process-user.json
--rw-r--r--   0 ZHY19      (503) staff       (20)    59930 2023-07-14 15:38:14.000000 hubmap-commons-2.1.7/hubmap_commons/entity.py
--rw-r--r--   0 ZHY19      (503) staff       (20)      567 2023-07-14 15:38:14.000000 hubmap-commons-2.1.7/hubmap_commons/exceptions.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     6278 2023-07-14 15:38:14.000000 hubmap-commons-2.1.7/hubmap_commons/file_helper.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     3066 2023-07-14 15:38:14.000000 hubmap-commons-2.1.7/hubmap_commons/globus_file_helper.py
--rw-r--r--   0 ZHY19      (503) staff       (20)    40463 2023-07-14 15:38:14.000000 hubmap-commons-2.1.7/hubmap_commons/hm_auth.py
--rw-r--r--   0 ZHY19      (503) staff       (20)      318 2023-07-14 15:38:14.000000 hubmap-commons-2.1.7/hubmap_commons/hubmap-globus-roles.json
--rw-r--r--   0 ZHY19      (503) staff       (20)    13204 2023-07-14 15:38:14.000000 hubmap-commons-2.1.7/hubmap_commons/hubmap_const.py
--rw-r--r--   0 ZHY19      (503) staff       (20)      471 2023-07-14 15:38:14.000000 hubmap-commons-2.1.7/hubmap_commons/hubmap_error.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     7813 2023-07-14 15:38:14.000000 hubmap-commons-2.1.7/hubmap_commons/metadata.py
--rw-r--r--   0 ZHY19      (503) staff       (20)    14445 2023-07-14 15:38:14.000000 hubmap-commons-2.1.7/hubmap_commons/neo4j_connection.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     1165 2023-07-14 15:38:14.000000 hubmap-commons-2.1.7/hubmap_commons/neo4j_driver.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     1178 2023-07-14 15:38:14.000000 hubmap-commons-2.1.7/hubmap_commons/net_helper.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     2269 2023-07-14 15:38:14.000000 hubmap-commons-2.1.7/hubmap_commons/properties.py
--rw-r--r--   0 ZHY19      (503) staff       (20)    31839 2023-07-14 15:38:14.000000 hubmap-commons-2.1.7/hubmap_commons/provenance.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     5461 2023-07-14 15:38:14.000000 hubmap-commons-2.1.7/hubmap_commons/schema_tools.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     1034 2023-07-14 15:38:14.000000 hubmap-commons-2.1.7/hubmap_commons/singleton_metaclass.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     1681 2023-07-14 15:38:14.000000 hubmap-commons-2.1.7/hubmap_commons/string_helper.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     1112 2023-07-14 15:38:14.000000 hubmap-commons-2.1.7/hubmap_commons/test_helper.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     5728 2023-07-14 15:38:14.000000 hubmap-commons-2.1.7/hubmap_commons/test_ws.py
--rw-r--r--   0 ZHY19      (503) staff       (20)    13275 2023-07-14 15:38:14.000000 hubmap-commons-2.1.7/hubmap_commons/type_client.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     5896 2023-07-14 15:38:14.000000 hubmap-commons-2.1.7/hubmap_commons/uuid_generator.py
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2023-07-14 15:38:59.343554 hubmap-commons-2.1.7/hubmap_commons.egg-info/
--rw-r--r--   0 ZHY19      (503) staff       (20)     3354 2023-07-14 15:38:59.000000 hubmap-commons-2.1.7/hubmap_commons.egg-info/PKG-INFO
--rw-r--r--   0 ZHY19      (503) staff       (20)     1311 2023-07-14 15:38:59.000000 hubmap-commons-2.1.7/hubmap_commons.egg-info/SOURCES.txt
--rw-r--r--   0 ZHY19      (503) staff       (20)        1 2023-07-14 15:38:59.000000 hubmap-commons-2.1.7/hubmap_commons.egg-info/dependency_links.txt
--rw-r--r--   0 ZHY19      (503) staff       (20)      162 2023-07-14 15:38:59.000000 hubmap-commons-2.1.7/hubmap_commons.egg-info/requires.txt
--rw-r--r--   0 ZHY19      (503) staff       (20)       15 2023-07-14 15:38:59.000000 hubmap-commons-2.1.7/hubmap_commons.egg-info/top_level.txt
--rw-r--r--   0 ZHY19      (503) staff       (20)       38 2023-07-14 15:38:59.360289 hubmap-commons-2.1.7/setup.cfg
--rw-r--r--   0 ZHY19      (503) staff       (20)     1433 2023-07-14 15:38:14.000000 hubmap-commons-2.1.7/setup.py
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2023-07-14 15:38:59.359580 hubmap-commons-2.1.7/tests/
--rw-r--r--   0 ZHY19      (503) staff       (20)      250 2023-07-14 15:38:14.000000 hubmap-commons-2.1.7/tests/test_dummy_type_client.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     2847 2023-07-14 15:38:15.000000 hubmap-commons-2.1.7/tests/test_group_write_check.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     3580 2023-07-14 15:38:15.000000 hubmap-commons-2.1.7/tests/test_neo4j_connection.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     2119 2023-07-14 15:38:15.000000 hubmap-commons-2.1.7/tests/test_provenance.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     6152 2023-07-14 15:38:15.000000 hubmap-commons-2.1.7/tests/test_schema_tools.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     1048 2023-07-14 15:38:15.000000 hubmap-commons-2.1.7/tests/test_singleton_meta.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     8065 2023-07-14 15:38:15.000000 hubmap-commons-2.1.7/tests/test_type_client.py
+drwxr-xr-x   0 zhy19     (1000) zhy19     (1000)        0 2023-07-17 15:44:24.918007 hubmap-commons-2.1.8/
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     3354 2023-07-17 15:44:24.913006 hubmap-commons-2.1.8/PKG-INFO
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     2893 2023-05-30 14:57:39.000000 hubmap-commons-2.1.8/README.md
+drwxr-xr-x   0 zhy19     (1000) zhy19     (1000)        0 2023-07-17 15:44:24.909006 hubmap-commons-2.1.8/hubmap_commons/
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)    20007 2023-07-17 15:42:54.000000 hubmap-commons-2.1.8/hubmap_commons/21f293b0-globus-groups.json
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     4461 2023-07-17 15:42:54.000000 hubmap-commons-2.1.8/hubmap_commons/21f293b0-process-user.json
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     3665 2023-05-30 14:57:39.000000 hubmap-commons-2.1.8/hubmap_commons/S3_worker.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     5788 2023-05-30 14:57:39.000000 hubmap-commons-2.1.8/hubmap_commons/activity.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)      221 2023-05-30 14:57:39.000000 hubmap-commons-2.1.8/hubmap_commons/autherror.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)    12776 2023-05-30 14:57:39.000000 hubmap-commons-2.1.8/hubmap_commons/c4018852-globus-groups.json
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     3095 2023-05-30 14:57:39.000000 hubmap-commons-2.1.8/hubmap_commons/c4018852-process-user.json
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)    59930 2023-05-30 14:57:39.000000 hubmap-commons-2.1.8/hubmap_commons/entity.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)      567 2023-05-30 14:57:39.000000 hubmap-commons-2.1.8/hubmap_commons/exceptions.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     6278 2023-05-30 14:57:39.000000 hubmap-commons-2.1.8/hubmap_commons/file_helper.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     3066 2023-05-30 14:57:39.000000 hubmap-commons-2.1.8/hubmap_commons/globus_file_helper.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)    40463 2023-05-30 14:57:39.000000 hubmap-commons-2.1.8/hubmap_commons/hm_auth.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)      318 2023-05-30 14:57:39.000000 hubmap-commons-2.1.8/hubmap_commons/hubmap-globus-roles.json
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)    13204 2023-05-30 14:57:39.000000 hubmap-commons-2.1.8/hubmap_commons/hubmap_const.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)      471 2023-05-30 14:57:39.000000 hubmap-commons-2.1.8/hubmap_commons/hubmap_error.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     7813 2023-05-30 14:57:39.000000 hubmap-commons-2.1.8/hubmap_commons/metadata.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)    14445 2023-05-30 14:57:39.000000 hubmap-commons-2.1.8/hubmap_commons/neo4j_connection.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     1165 2023-05-30 14:57:39.000000 hubmap-commons-2.1.8/hubmap_commons/neo4j_driver.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     1178 2023-05-30 14:57:39.000000 hubmap-commons-2.1.8/hubmap_commons/net_helper.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     2269 2023-05-30 14:57:39.000000 hubmap-commons-2.1.8/hubmap_commons/properties.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)    31839 2023-05-30 14:57:39.000000 hubmap-commons-2.1.8/hubmap_commons/provenance.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     5461 2023-05-30 14:57:39.000000 hubmap-commons-2.1.8/hubmap_commons/schema_tools.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     1034 2023-05-30 14:57:39.000000 hubmap-commons-2.1.8/hubmap_commons/singleton_metaclass.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     1681 2023-05-30 14:57:39.000000 hubmap-commons-2.1.8/hubmap_commons/string_helper.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     1112 2023-05-30 14:57:39.000000 hubmap-commons-2.1.8/hubmap_commons/test_helper.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     5728 2023-05-30 14:57:39.000000 hubmap-commons-2.1.8/hubmap_commons/test_ws.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)    13275 2023-05-30 14:57:39.000000 hubmap-commons-2.1.8/hubmap_commons/type_client.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     5896 2023-05-30 14:57:39.000000 hubmap-commons-2.1.8/hubmap_commons/uuid_generator.py
+drwxr-xr-x   0 zhy19     (1000) zhy19     (1000)        0 2023-07-17 15:44:24.911006 hubmap-commons-2.1.8/hubmap_commons.egg-info/
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     3354 2023-07-17 15:44:24.000000 hubmap-commons-2.1.8/hubmap_commons.egg-info/PKG-INFO
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     1311 2023-07-17 15:44:24.000000 hubmap-commons-2.1.8/hubmap_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)        1 2023-07-17 15:44:24.000000 hubmap-commons-2.1.8/hubmap_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)      162 2023-07-17 15:44:24.000000 hubmap-commons-2.1.8/hubmap_commons.egg-info/requires.txt
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)       15 2023-07-17 15:44:24.000000 hubmap-commons-2.1.8/hubmap_commons.egg-info/top_level.txt
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)       38 2023-07-17 15:44:24.918007 hubmap-commons-2.1.8/setup.cfg
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     1433 2023-07-17 15:42:54.000000 hubmap-commons-2.1.8/setup.py
+drwxr-xr-x   0 zhy19     (1000) zhy19     (1000)        0 2023-07-17 15:44:24.913006 hubmap-commons-2.1.8/tests/
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)      250 2023-05-30 14:57:39.000000 hubmap-commons-2.1.8/tests/test_dummy_type_client.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     2847 2023-05-30 14:57:39.000000 hubmap-commons-2.1.8/tests/test_group_write_check.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     3580 2023-05-30 14:57:39.000000 hubmap-commons-2.1.8/tests/test_neo4j_connection.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     2119 2023-05-30 14:57:39.000000 hubmap-commons-2.1.8/tests/test_provenance.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     6152 2023-05-30 14:57:39.000000 hubmap-commons-2.1.8/tests/test_schema_tools.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     1048 2023-05-30 14:57:39.000000 hubmap-commons-2.1.8/tests/test_singleton_meta.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     8065 2023-05-30 14:57:39.000000 hubmap-commons-2.1.8/tests/test_type_client.py
```

### Comparing `hubmap-commons-2.1.7/PKG-INFO` & `hubmap-commons-2.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hubmap-commons
-Version: 2.1.7
+Version: 2.1.8
 Summary: The common utilities used by the HuMBAP web services
 Home-page: https://github.com/hubmapconsortium/commons
 Author: HuBMAP Consortium
 Author-email: api-developers@hubmapconsortium.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hubmap-commons-2.1.7/README.md` & `hubmap-commons-2.1.8/README.md`

 * *Files identical despite different names*

### Comparing `hubmap-commons-2.1.7/hubmap_commons/21f293b0-globus-groups.json` & `hubmap-commons-2.1.8/hubmap_commons/21f293b0-globus-groups.json`

 * *Files identical despite different names*

### Comparing `hubmap-commons-2.1.7/hubmap_commons/S3_worker.py` & `hubmap-commons-2.1.8/hubmap_commons/S3_worker.py`

 * *Files identical despite different names*

### Comparing `hubmap-commons-2.1.7/hubmap_commons/activity.py` & `hubmap-commons-2.1.8/hubmap_commons/activity.py`

 * *Files identical despite different names*

### Comparing `hubmap-commons-2.1.7/hubmap_commons/c4018852-globus-groups.json` & `hubmap-commons-2.1.8/hubmap_commons/c4018852-globus-groups.json`

 * *Files identical despite different names*

### Comparing `hubmap-commons-2.1.7/hubmap_commons/c4018852-process-user.json` & `hubmap-commons-2.1.8/hubmap_commons/c4018852-process-user.json`

 * *Files identical despite different names*

### Comparing `hubmap-commons-2.1.7/hubmap_commons/entity.py` & `hubmap-commons-2.1.8/hubmap_commons/entity.py`

 * *Files identical despite different names*

### Comparing `hubmap-commons-2.1.7/hubmap_commons/exceptions.py` & `hubmap-commons-2.1.8/hubmap_commons/exceptions.py`

 * *Files identical despite different names*

### Comparing `hubmap-commons-2.1.7/hubmap_commons/file_helper.py` & `hubmap-commons-2.1.8/hubmap_commons/file_helper.py`

 * *Files identical despite different names*

### Comparing `hubmap-commons-2.1.7/hubmap_commons/globus_file_helper.py` & `hubmap-commons-2.1.8/hubmap_commons/globus_file_helper.py`

 * *Files identical despite different names*

### Comparing `hubmap-commons-2.1.7/hubmap_commons/hm_auth.py` & `hubmap-commons-2.1.8/hubmap_commons/hm_auth.py`

 * *Files identical despite different names*

### Comparing `hubmap-commons-2.1.7/hubmap_commons/hubmap_const.py` & `hubmap-commons-2.1.8/hubmap_commons/hubmap_const.py`

 * *Files identical despite different names*

### Comparing `hubmap-commons-2.1.7/hubmap_commons/metadata.py` & `hubmap-commons-2.1.8/hubmap_commons/metadata.py`

 * *Files identical despite different names*

### Comparing `hubmap-commons-2.1.7/hubmap_commons/neo4j_connection.py` & `hubmap-commons-2.1.8/hubmap_commons/neo4j_connection.py`

 * *Files identical despite different names*

### Comparing `hubmap-commons-2.1.7/hubmap_commons/neo4j_driver.py` & `hubmap-commons-2.1.8/hubmap_commons/neo4j_driver.py`

 * *Files identical despite different names*

### Comparing `hubmap-commons-2.1.7/hubmap_commons/net_helper.py` & `hubmap-commons-2.1.8/hubmap_commons/net_helper.py`

 * *Files identical despite different names*

### Comparing `hubmap-commons-2.1.7/hubmap_commons/properties.py` & `hubmap-commons-2.1.8/hubmap_commons/properties.py`

 * *Files identical despite different names*

### Comparing `hubmap-commons-2.1.7/hubmap_commons/provenance.py` & `hubmap-commons-2.1.8/hubmap_commons/provenance.py`

 * *Files identical despite different names*

### Comparing `hubmap-commons-2.1.7/hubmap_commons/schema_tools.py` & `hubmap-commons-2.1.8/hubmap_commons/schema_tools.py`

 * *Files identical despite different names*

### Comparing `hubmap-commons-2.1.7/hubmap_commons/singleton_metaclass.py` & `hubmap-commons-2.1.8/hubmap_commons/singleton_metaclass.py`

 * *Files identical despite different names*

### Comparing `hubmap-commons-2.1.7/hubmap_commons/string_helper.py` & `hubmap-commons-2.1.8/hubmap_commons/string_helper.py`

 * *Files identical despite different names*

### Comparing `hubmap-commons-2.1.7/hubmap_commons/test_helper.py` & `hubmap-commons-2.1.8/hubmap_commons/test_helper.py`

 * *Files identical despite different names*

### Comparing `hubmap-commons-2.1.7/hubmap_commons/test_ws.py` & `hubmap-commons-2.1.8/hubmap_commons/test_ws.py`

 * *Files identical despite different names*

### Comparing `hubmap-commons-2.1.7/hubmap_commons/type_client.py` & `hubmap-commons-2.1.8/hubmap_commons/type_client.py`

 * *Files identical despite different names*

### Comparing `hubmap-commons-2.1.7/hubmap_commons/uuid_generator.py` & `hubmap-commons-2.1.8/hubmap_commons/uuid_generator.py`

 * *Files identical despite different names*

### Comparing `hubmap-commons-2.1.7/hubmap_commons.egg-info/PKG-INFO` & `hubmap-commons-2.1.8/hubmap_commons.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hubmap-commons
-Version: 2.1.7
+Version: 2.1.8
 Summary: The common utilities used by the HuMBAP web services
 Home-page: https://github.com/hubmapconsortium/commons
 Author: HuBMAP Consortium
 Author-email: api-developers@hubmapconsortium.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hubmap-commons-2.1.7/hubmap_commons.egg-info/SOURCES.txt` & `hubmap-commons-2.1.8/hubmap_commons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hubmap-commons-2.1.7/setup.py` & `hubmap-commons-2.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="hubmap-commons",
-    version="2.1.7",
+    version="2.1.8",
     author="HuBMAP Consortium",
     author_email="api-developers@hubmapconsortium.org",
     description="The common utilities used by the HuMBAP web services",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/hubmapconsortium/commons",
     packages=['hubmap_commons'],
```

### Comparing `hubmap-commons-2.1.7/tests/test_group_write_check.py` & `hubmap-commons-2.1.8/tests/test_group_write_check.py`

 * *Files identical despite different names*

### Comparing `hubmap-commons-2.1.7/tests/test_neo4j_connection.py` & `hubmap-commons-2.1.8/tests/test_neo4j_connection.py`

 * *Files identical despite different names*

### Comparing `hubmap-commons-2.1.7/tests/test_provenance.py` & `hubmap-commons-2.1.8/tests/test_provenance.py`

 * *Files identical despite different names*

### Comparing `hubmap-commons-2.1.7/tests/test_schema_tools.py` & `hubmap-commons-2.1.8/tests/test_schema_tools.py`

 * *Files identical despite different names*

### Comparing `hubmap-commons-2.1.7/tests/test_singleton_meta.py` & `hubmap-commons-2.1.8/tests/test_singleton_meta.py`

 * *Files identical despite different names*

### Comparing `hubmap-commons-2.1.7/tests/test_type_client.py` & `hubmap-commons-2.1.8/tests/test_type_client.py`

 * *Files identical despite different names*

