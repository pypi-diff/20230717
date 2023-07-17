# Comparing `tmp/capsulecorp-0.1.3.tar.gz` & `tmp/capsulecorp-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capsulecorp-0.1.3.tar", last modified: Thu Jul 13 16:38:13 2023, max compression
+gzip compressed data, was "capsulecorp-0.1.4.tar", last modified: Mon Jul 17 14:08:42 2023, max compression
```

## Comparing `capsulecorp-0.1.3.tar` & `capsulecorp-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-13 16:38:13.389714 capsulecorp-0.1.3/
--rw-r--r--   0 daless383   (502) staff       (20)    11357 2023-02-13 20:25:15.000000 capsulecorp-0.1.3/LICENSE
--rw-r--r--   0 daless383   (502) staff       (20)      461 2023-07-13 16:38:13.388980 capsulecorp-0.1.3/PKG-INFO
--rw-r--r--   0 daless383   (502) staff       (20)       99 2023-02-13 20:25:15.000000 capsulecorp-0.1.3/README.md
-drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-13 16:38:13.374502 capsulecorp-0.1.3/capsulecorp/
--rw-r--r--   0 daless383   (502) staff       (20)       63 2023-02-14 15:14:02.000000 capsulecorp-0.1.3/capsulecorp/__init__.py
--rw-r--r--   0 daless383   (502) staff       (20)     7967 2023-05-04 16:53:29.000000 capsulecorp-0.1.3/capsulecorp/query_driver.py
-drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-13 16:38:13.387205 capsulecorp-0.1.3/capsulecorp/utilities/
--rw-r--r--   0 daless383   (502) staff       (20)        0 2023-07-13 15:20:45.000000 capsulecorp-0.1.3/capsulecorp/utilities/__init__.py
--rw-r--r--   0 daless383   (502) staff       (20)     7717 2023-07-13 16:29:38.000000 capsulecorp-0.1.3/capsulecorp/utilities/databricks_utils.py
--rw-r--r--   0 daless383   (502) staff       (20)     1441 2023-07-10 20:48:28.000000 capsulecorp-0.1.3/capsulecorp/utilities/github_utils.py
--rw-r--r--   0 daless383   (502) staff       (20)     2320 2023-05-18 14:36:49.000000 capsulecorp-0.1.3/capsulecorp/utilities/slack_utils.py
--rw-r--r--   0 daless383   (502) staff       (20)    14740 2023-07-06 17:37:40.000000 capsulecorp-0.1.3/capsulecorp/utils.py
--rw-r--r--   0 daless383   (502) staff       (20)      269 2023-07-13 14:23:27.000000 capsulecorp-0.1.3/capsulecorp/version.py
-drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-13 16:38:13.380462 capsulecorp-0.1.3/capsulecorp.egg-info/
--rw-r--r--   0 daless383   (502) staff       (20)      461 2023-07-13 16:38:12.000000 capsulecorp-0.1.3/capsulecorp.egg-info/PKG-INFO
--rw-r--r--   0 daless383   (502) staff       (20)      462 2023-07-13 16:38:13.000000 capsulecorp-0.1.3/capsulecorp.egg-info/SOURCES.txt
--rw-r--r--   0 daless383   (502) staff       (20)        1 2023-07-13 16:38:12.000000 capsulecorp-0.1.3/capsulecorp.egg-info/dependency_links.txt
--rw-r--r--   0 daless383   (502) staff       (20)      106 2023-07-13 16:38:13.000000 capsulecorp-0.1.3/capsulecorp.egg-info/requires.txt
--rw-r--r--   0 daless383   (502) staff       (20)       12 2023-07-13 16:38:13.000000 capsulecorp-0.1.3/capsulecorp.egg-info/top_level.txt
--rw-r--r--   0 daless383   (502) staff       (20)       86 2023-02-14 15:04:49.000000 capsulecorp-0.1.3/pyproject.toml
--rw-r--r--   0 daless383   (502) staff       (20)       38 2023-07-13 16:38:13.390142 capsulecorp-0.1.3/setup.cfg
--rw-r--r--   0 daless383   (502) staff       (20)     6621 2023-07-12 13:53:07.000000 capsulecorp-0.1.3/setup.py
+drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-17 14:08:42.187548 capsulecorp-0.1.4/
+-rw-r--r--   0 daless383   (502) staff       (20)    11357 2023-02-13 20:25:15.000000 capsulecorp-0.1.4/LICENSE
+-rw-r--r--   0 daless383   (502) staff       (20)      461 2023-07-17 14:08:42.186850 capsulecorp-0.1.4/PKG-INFO
+-rw-r--r--   0 daless383   (502) staff       (20)       99 2023-02-13 20:25:15.000000 capsulecorp-0.1.4/README.md
+drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-17 14:08:42.175995 capsulecorp-0.1.4/capsulecorp/
+-rw-r--r--   0 daless383   (502) staff       (20)       63 2023-02-14 15:14:02.000000 capsulecorp-0.1.4/capsulecorp/__init__.py
+-rw-r--r--   0 daless383   (502) staff       (20)     7967 2023-05-04 16:53:29.000000 capsulecorp-0.1.4/capsulecorp/query_driver.py
+drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-17 14:08:42.185700 capsulecorp-0.1.4/capsulecorp/utilities/
+-rw-r--r--   0 daless383   (502) staff       (20)        0 2023-07-13 15:20:45.000000 capsulecorp-0.1.4/capsulecorp/utilities/__init__.py
+-rw-r--r--   0 daless383   (502) staff       (20)     8765 2023-07-17 14:02:23.000000 capsulecorp-0.1.4/capsulecorp/utilities/databricks_utils.py
+-rw-r--r--   0 daless383   (502) staff       (20)     1441 2023-07-10 20:48:28.000000 capsulecorp-0.1.4/capsulecorp/utilities/github_utils.py
+-rw-r--r--   0 daless383   (502) staff       (20)     2320 2023-05-18 14:36:49.000000 capsulecorp-0.1.4/capsulecorp/utilities/slack_utils.py
+-rw-r--r--   0 daless383   (502) staff       (20)    14740 2023-07-06 17:37:40.000000 capsulecorp-0.1.4/capsulecorp/utils.py
+-rw-r--r--   0 daless383   (502) staff       (20)      269 2023-07-17 14:01:22.000000 capsulecorp-0.1.4/capsulecorp/version.py
+drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-17 14:08:42.181481 capsulecorp-0.1.4/capsulecorp.egg-info/
+-rw-r--r--   0 daless383   (502) staff       (20)      461 2023-07-17 14:08:41.000000 capsulecorp-0.1.4/capsulecorp.egg-info/PKG-INFO
+-rw-r--r--   0 daless383   (502) staff       (20)      462 2023-07-17 14:08:42.000000 capsulecorp-0.1.4/capsulecorp.egg-info/SOURCES.txt
+-rw-r--r--   0 daless383   (502) staff       (20)        1 2023-07-17 14:08:41.000000 capsulecorp-0.1.4/capsulecorp.egg-info/dependency_links.txt
+-rw-r--r--   0 daless383   (502) staff       (20)      106 2023-07-17 14:08:41.000000 capsulecorp-0.1.4/capsulecorp.egg-info/requires.txt
+-rw-r--r--   0 daless383   (502) staff       (20)       12 2023-07-17 14:08:41.000000 capsulecorp-0.1.4/capsulecorp.egg-info/top_level.txt
+-rw-r--r--   0 daless383   (502) staff       (20)       86 2023-02-14 15:04:49.000000 capsulecorp-0.1.4/pyproject.toml
+-rw-r--r--   0 daless383   (502) staff       (20)       38 2023-07-17 14:08:42.187750 capsulecorp-0.1.4/setup.cfg
+-rw-r--r--   0 daless383   (502) staff       (20)     6621 2023-07-12 13:53:07.000000 capsulecorp-0.1.4/setup.py
```

### Comparing `capsulecorp-0.1.3/LICENSE` & `capsulecorp-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `capsulecorp-0.1.3/capsulecorp/query_driver.py` & `capsulecorp-0.1.4/capsulecorp/query_driver.py`

 * *Files identical despite different names*

### Comparing `capsulecorp-0.1.3/capsulecorp/utilities/databricks_utils.py` & `capsulecorp-0.1.4/capsulecorp/utilities/databricks_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -233,7 +233,37 @@
     # Parse the directory name from the full notebook path
     dir_name = os.path.dirname(notebook_path.split(user)[1])
     # Initialize DataBricks API Client and Workspace API
     databricks_client = ApiClient(host=host, token=token, verify=True)
     workspace_service = WorkspaceService(databricks_client)
     # Make the directory
     return workspace_service.mkdirs(user + dir_name)
+
+
+def put_file(host, token, src_path, dbfs_path):
+    """
+        Uploads a file from the local filesystem to Databricks File System.
+
+        Args:
+            host (str): URL of DataBricks workspace
+            token (str): DataBricks API token
+            src_path (str): The path of the file on the local filesystem.
+            dbfs_path (str): DBFS path where the file will be uploaded.
+
+        Returns:
+            TODO: Add success boolean
+    """
+    # Connect to databricks
+    databricks_client = ApiClient(host=host, token=token, verify=True)
+    dbfs_api = DbfsApi(databricks_client)
+    # Read file and upload to dbfs
+    handle = dbfs_api.client.create(dbfs_path, True)['handle']
+    with open(src_path, 'rb') as local_file:
+        while True:
+            contents = local_file.read(2 ** 20)
+            if len(contents) == 0:
+                break
+            # add_block should not take a bytes object.
+            dbfs_api.client.add_block(handle, b64encode(contents).decode())
+        dbfs_api.client.close(handle)
+
+    return
```

### Comparing `capsulecorp-0.1.3/capsulecorp/utilities/github_utils.py` & `capsulecorp-0.1.4/capsulecorp/utilities/github_utils.py`

 * *Files identical despite different names*

### Comparing `capsulecorp-0.1.3/capsulecorp/utilities/slack_utils.py` & `capsulecorp-0.1.4/capsulecorp/utilities/slack_utils.py`

 * *Files identical despite different names*

### Comparing `capsulecorp-0.1.3/capsulecorp/utils.py` & `capsulecorp-0.1.4/capsulecorp/utils.py`

 * *Files identical despite different names*

### Comparing `capsulecorp-0.1.3/setup.py` & `capsulecorp-0.1.4/setup.py`

 * *Files identical despite different names*

