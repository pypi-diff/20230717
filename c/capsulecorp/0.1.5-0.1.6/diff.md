# Comparing `tmp/capsulecorp-0.1.5.tar.gz` & `tmp/capsulecorp-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capsulecorp-0.1.5.tar", last modified: Mon Jul 17 15:40:40 2023, max compression
+gzip compressed data, was "capsulecorp-0.1.6.tar", last modified: Mon Jul 17 16:04:33 2023, max compression
```

## Comparing `capsulecorp-0.1.5.tar` & `capsulecorp-0.1.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-17 15:40:40.108888 capsulecorp-0.1.5/
--rw-r--r--   0 daless383   (502) staff       (20)    11357 2023-02-13 20:25:15.000000 capsulecorp-0.1.5/LICENSE
--rw-r--r--   0 daless383   (502) staff       (20)      461 2023-07-17 15:40:40.108205 capsulecorp-0.1.5/PKG-INFO
--rw-r--r--   0 daless383   (502) staff       (20)       99 2023-02-13 20:25:15.000000 capsulecorp-0.1.5/README.md
-drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-17 15:40:40.093542 capsulecorp-0.1.5/capsulecorp/
--rw-r--r--   0 daless383   (502) staff       (20)       63 2023-02-14 15:14:02.000000 capsulecorp-0.1.5/capsulecorp/__init__.py
--rw-r--r--   0 daless383   (502) staff       (20)     7967 2023-05-04 16:53:29.000000 capsulecorp-0.1.5/capsulecorp/query_driver.py
-drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-17 15:40:40.106946 capsulecorp-0.1.5/capsulecorp/utilities/
--rw-r--r--   0 daless383   (502) staff       (20)        0 2023-07-13 15:20:45.000000 capsulecorp-0.1.5/capsulecorp/utilities/__init__.py
--rw-r--r--   0 daless383   (502) staff       (20)     8809 2023-07-17 15:36:01.000000 capsulecorp-0.1.5/capsulecorp/utilities/databricks_utils.py
--rw-r--r--   0 daless383   (502) staff       (20)     1441 2023-07-10 20:48:28.000000 capsulecorp-0.1.5/capsulecorp/utilities/github_utils.py
--rw-r--r--   0 daless383   (502) staff       (20)     2320 2023-05-18 14:36:49.000000 capsulecorp-0.1.5/capsulecorp/utilities/slack_utils.py
--rw-r--r--   0 daless383   (502) staff       (20)    14740 2023-07-06 17:37:40.000000 capsulecorp-0.1.5/capsulecorp/utils.py
--rw-r--r--   0 daless383   (502) staff       (20)      269 2023-07-17 15:39:14.000000 capsulecorp-0.1.5/capsulecorp/version.py
-drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-17 15:40:40.099238 capsulecorp-0.1.5/capsulecorp.egg-info/
--rw-r--r--   0 daless383   (502) staff       (20)      461 2023-07-17 15:40:39.000000 capsulecorp-0.1.5/capsulecorp.egg-info/PKG-INFO
--rw-r--r--   0 daless383   (502) staff       (20)      462 2023-07-17 15:40:40.000000 capsulecorp-0.1.5/capsulecorp.egg-info/SOURCES.txt
--rw-r--r--   0 daless383   (502) staff       (20)        1 2023-07-17 15:40:39.000000 capsulecorp-0.1.5/capsulecorp.egg-info/dependency_links.txt
--rw-r--r--   0 daless383   (502) staff       (20)      106 2023-07-17 15:40:39.000000 capsulecorp-0.1.5/capsulecorp.egg-info/requires.txt
--rw-r--r--   0 daless383   (502) staff       (20)       12 2023-07-17 15:40:39.000000 capsulecorp-0.1.5/capsulecorp.egg-info/top_level.txt
--rw-r--r--   0 daless383   (502) staff       (20)       86 2023-02-14 15:04:49.000000 capsulecorp-0.1.5/pyproject.toml
--rw-r--r--   0 daless383   (502) staff       (20)       38 2023-07-17 15:40:40.109120 capsulecorp-0.1.5/setup.cfg
--rw-r--r--   0 daless383   (502) staff       (20)     6621 2023-07-12 13:53:07.000000 capsulecorp-0.1.5/setup.py
+drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-17 16:04:33.573022 capsulecorp-0.1.6/
+-rw-r--r--   0 daless383   (502) staff       (20)    11357 2023-02-13 20:25:15.000000 capsulecorp-0.1.6/LICENSE
+-rw-r--r--   0 daless383   (502) staff       (20)      461 2023-07-17 16:04:33.572540 capsulecorp-0.1.6/PKG-INFO
+-rw-r--r--   0 daless383   (502) staff       (20)       99 2023-02-13 20:25:15.000000 capsulecorp-0.1.6/README.md
+drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-17 16:04:33.562995 capsulecorp-0.1.6/capsulecorp/
+-rw-r--r--   0 daless383   (502) staff       (20)       63 2023-02-14 15:14:02.000000 capsulecorp-0.1.6/capsulecorp/__init__.py
+-rw-r--r--   0 daless383   (502) staff       (20)     7967 2023-05-04 16:53:29.000000 capsulecorp-0.1.6/capsulecorp/query_driver.py
+drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-17 16:04:33.571665 capsulecorp-0.1.6/capsulecorp/utilities/
+-rw-r--r--   0 daless383   (502) staff       (20)        0 2023-07-13 15:20:45.000000 capsulecorp-0.1.6/capsulecorp/utilities/__init__.py
+-rw-r--r--   0 daless383   (502) staff       (20)     8833 2023-07-17 16:00:44.000000 capsulecorp-0.1.6/capsulecorp/utilities/databricks_utils.py
+-rw-r--r--   0 daless383   (502) staff       (20)     1441 2023-07-10 20:48:28.000000 capsulecorp-0.1.6/capsulecorp/utilities/github_utils.py
+-rw-r--r--   0 daless383   (502) staff       (20)     2320 2023-05-18 14:36:49.000000 capsulecorp-0.1.6/capsulecorp/utilities/slack_utils.py
+-rw-r--r--   0 daless383   (502) staff       (20)    14740 2023-07-06 17:37:40.000000 capsulecorp-0.1.6/capsulecorp/utils.py
+-rw-r--r--   0 daless383   (502) staff       (20)      269 2023-07-17 16:00:59.000000 capsulecorp-0.1.6/capsulecorp/version.py
+drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-17 16:04:33.567905 capsulecorp-0.1.6/capsulecorp.egg-info/
+-rw-r--r--   0 daless383   (502) staff       (20)      461 2023-07-17 16:04:32.000000 capsulecorp-0.1.6/capsulecorp.egg-info/PKG-INFO
+-rw-r--r--   0 daless383   (502) staff       (20)      462 2023-07-17 16:04:33.000000 capsulecorp-0.1.6/capsulecorp.egg-info/SOURCES.txt
+-rw-r--r--   0 daless383   (502) staff       (20)        1 2023-07-17 16:04:32.000000 capsulecorp-0.1.6/capsulecorp.egg-info/dependency_links.txt
+-rw-r--r--   0 daless383   (502) staff       (20)      106 2023-07-17 16:04:33.000000 capsulecorp-0.1.6/capsulecorp.egg-info/requires.txt
+-rw-r--r--   0 daless383   (502) staff       (20)       12 2023-07-17 16:04:33.000000 capsulecorp-0.1.6/capsulecorp.egg-info/top_level.txt
+-rw-r--r--   0 daless383   (502) staff       (20)       86 2023-02-14 15:04:49.000000 capsulecorp-0.1.6/pyproject.toml
+-rw-r--r--   0 daless383   (502) staff       (20)       38 2023-07-17 16:04:33.573186 capsulecorp-0.1.6/setup.cfg
+-rw-r--r--   0 daless383   (502) staff       (20)     6621 2023-07-12 13:53:07.000000 capsulecorp-0.1.6/setup.py
```

### Comparing `capsulecorp-0.1.5/LICENSE` & `capsulecorp-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `capsulecorp-0.1.5/capsulecorp/query_driver.py` & `capsulecorp-0.1.6/capsulecorp/query_driver.py`

 * *Files identical despite different names*

### Comparing `capsulecorp-0.1.5/capsulecorp/utilities/databricks_utils.py` & `capsulecorp-0.1.6/capsulecorp/utilities/databricks_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -260,11 +260,12 @@
     handle = dbfs_api.client.create(dbfs_path, True)['handle']
     with open(src_path, 'rb') as local_file:
         while True:
             contents = local_file.read(2 ** 20)
             if len(contents) == 0:
                 break
             # add_block should not take a bytes object.
-            dbfs_api.client.add_block(handle, b64encode(contents).decode())
+            dbfs_api.client.add_block(
+                handle, base64.b64encode(contents).decode())
         dbfs_api.client.close(handle)
 
     return
```

### Comparing `capsulecorp-0.1.5/capsulecorp/utilities/github_utils.py` & `capsulecorp-0.1.6/capsulecorp/utilities/github_utils.py`

 * *Files identical despite different names*

### Comparing `capsulecorp-0.1.5/capsulecorp/utilities/slack_utils.py` & `capsulecorp-0.1.6/capsulecorp/utilities/slack_utils.py`

 * *Files identical despite different names*

### Comparing `capsulecorp-0.1.5/capsulecorp/utils.py` & `capsulecorp-0.1.6/capsulecorp/utils.py`

 * *Files identical despite different names*

### Comparing `capsulecorp-0.1.5/setup.py` & `capsulecorp-0.1.6/setup.py`

 * *Files identical despite different names*

