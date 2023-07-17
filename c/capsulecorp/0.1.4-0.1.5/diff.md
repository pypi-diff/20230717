# Comparing `tmp/capsulecorp-0.1.4.tar.gz` & `tmp/capsulecorp-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capsulecorp-0.1.4.tar", last modified: Mon Jul 17 14:08:42 2023, max compression
+gzip compressed data, was "capsulecorp-0.1.5.tar", last modified: Mon Jul 17 15:40:40 2023, max compression
```

## Comparing `capsulecorp-0.1.4.tar` & `capsulecorp-0.1.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-17 14:08:42.187548 capsulecorp-0.1.4/
--rw-r--r--   0 daless383   (502) staff       (20)    11357 2023-02-13 20:25:15.000000 capsulecorp-0.1.4/LICENSE
--rw-r--r--   0 daless383   (502) staff       (20)      461 2023-07-17 14:08:42.186850 capsulecorp-0.1.4/PKG-INFO
--rw-r--r--   0 daless383   (502) staff       (20)       99 2023-02-13 20:25:15.000000 capsulecorp-0.1.4/README.md
-drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-17 14:08:42.175995 capsulecorp-0.1.4/capsulecorp/
--rw-r--r--   0 daless383   (502) staff       (20)       63 2023-02-14 15:14:02.000000 capsulecorp-0.1.4/capsulecorp/__init__.py
--rw-r--r--   0 daless383   (502) staff       (20)     7967 2023-05-04 16:53:29.000000 capsulecorp-0.1.4/capsulecorp/query_driver.py
-drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-17 14:08:42.185700 capsulecorp-0.1.4/capsulecorp/utilities/
--rw-r--r--   0 daless383   (502) staff       (20)        0 2023-07-13 15:20:45.000000 capsulecorp-0.1.4/capsulecorp/utilities/__init__.py
--rw-r--r--   0 daless383   (502) staff       (20)     8765 2023-07-17 14:02:23.000000 capsulecorp-0.1.4/capsulecorp/utilities/databricks_utils.py
--rw-r--r--   0 daless383   (502) staff       (20)     1441 2023-07-10 20:48:28.000000 capsulecorp-0.1.4/capsulecorp/utilities/github_utils.py
--rw-r--r--   0 daless383   (502) staff       (20)     2320 2023-05-18 14:36:49.000000 capsulecorp-0.1.4/capsulecorp/utilities/slack_utils.py
--rw-r--r--   0 daless383   (502) staff       (20)    14740 2023-07-06 17:37:40.000000 capsulecorp-0.1.4/capsulecorp/utils.py
--rw-r--r--   0 daless383   (502) staff       (20)      269 2023-07-17 14:01:22.000000 capsulecorp-0.1.4/capsulecorp/version.py
-drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-17 14:08:42.181481 capsulecorp-0.1.4/capsulecorp.egg-info/
--rw-r--r--   0 daless383   (502) staff       (20)      461 2023-07-17 14:08:41.000000 capsulecorp-0.1.4/capsulecorp.egg-info/PKG-INFO
--rw-r--r--   0 daless383   (502) staff       (20)      462 2023-07-17 14:08:42.000000 capsulecorp-0.1.4/capsulecorp.egg-info/SOURCES.txt
--rw-r--r--   0 daless383   (502) staff       (20)        1 2023-07-17 14:08:41.000000 capsulecorp-0.1.4/capsulecorp.egg-info/dependency_links.txt
--rw-r--r--   0 daless383   (502) staff       (20)      106 2023-07-17 14:08:41.000000 capsulecorp-0.1.4/capsulecorp.egg-info/requires.txt
--rw-r--r--   0 daless383   (502) staff       (20)       12 2023-07-17 14:08:41.000000 capsulecorp-0.1.4/capsulecorp.egg-info/top_level.txt
--rw-r--r--   0 daless383   (502) staff       (20)       86 2023-02-14 15:04:49.000000 capsulecorp-0.1.4/pyproject.toml
--rw-r--r--   0 daless383   (502) staff       (20)       38 2023-07-17 14:08:42.187750 capsulecorp-0.1.4/setup.cfg
--rw-r--r--   0 daless383   (502) staff       (20)     6621 2023-07-12 13:53:07.000000 capsulecorp-0.1.4/setup.py
+drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-17 15:40:40.108888 capsulecorp-0.1.5/
+-rw-r--r--   0 daless383   (502) staff       (20)    11357 2023-02-13 20:25:15.000000 capsulecorp-0.1.5/LICENSE
+-rw-r--r--   0 daless383   (502) staff       (20)      461 2023-07-17 15:40:40.108205 capsulecorp-0.1.5/PKG-INFO
+-rw-r--r--   0 daless383   (502) staff       (20)       99 2023-02-13 20:25:15.000000 capsulecorp-0.1.5/README.md
+drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-17 15:40:40.093542 capsulecorp-0.1.5/capsulecorp/
+-rw-r--r--   0 daless383   (502) staff       (20)       63 2023-02-14 15:14:02.000000 capsulecorp-0.1.5/capsulecorp/__init__.py
+-rw-r--r--   0 daless383   (502) staff       (20)     7967 2023-05-04 16:53:29.000000 capsulecorp-0.1.5/capsulecorp/query_driver.py
+drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-17 15:40:40.106946 capsulecorp-0.1.5/capsulecorp/utilities/
+-rw-r--r--   0 daless383   (502) staff       (20)        0 2023-07-13 15:20:45.000000 capsulecorp-0.1.5/capsulecorp/utilities/__init__.py
+-rw-r--r--   0 daless383   (502) staff       (20)     8809 2023-07-17 15:36:01.000000 capsulecorp-0.1.5/capsulecorp/utilities/databricks_utils.py
+-rw-r--r--   0 daless383   (502) staff       (20)     1441 2023-07-10 20:48:28.000000 capsulecorp-0.1.5/capsulecorp/utilities/github_utils.py
+-rw-r--r--   0 daless383   (502) staff       (20)     2320 2023-05-18 14:36:49.000000 capsulecorp-0.1.5/capsulecorp/utilities/slack_utils.py
+-rw-r--r--   0 daless383   (502) staff       (20)    14740 2023-07-06 17:37:40.000000 capsulecorp-0.1.5/capsulecorp/utils.py
+-rw-r--r--   0 daless383   (502) staff       (20)      269 2023-07-17 15:39:14.000000 capsulecorp-0.1.5/capsulecorp/version.py
+drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-17 15:40:40.099238 capsulecorp-0.1.5/capsulecorp.egg-info/
+-rw-r--r--   0 daless383   (502) staff       (20)      461 2023-07-17 15:40:39.000000 capsulecorp-0.1.5/capsulecorp.egg-info/PKG-INFO
+-rw-r--r--   0 daless383   (502) staff       (20)      462 2023-07-17 15:40:40.000000 capsulecorp-0.1.5/capsulecorp.egg-info/SOURCES.txt
+-rw-r--r--   0 daless383   (502) staff       (20)        1 2023-07-17 15:40:39.000000 capsulecorp-0.1.5/capsulecorp.egg-info/dependency_links.txt
+-rw-r--r--   0 daless383   (502) staff       (20)      106 2023-07-17 15:40:39.000000 capsulecorp-0.1.5/capsulecorp.egg-info/requires.txt
+-rw-r--r--   0 daless383   (502) staff       (20)       12 2023-07-17 15:40:39.000000 capsulecorp-0.1.5/capsulecorp.egg-info/top_level.txt
+-rw-r--r--   0 daless383   (502) staff       (20)       86 2023-02-14 15:04:49.000000 capsulecorp-0.1.5/pyproject.toml
+-rw-r--r--   0 daless383   (502) staff       (20)       38 2023-07-17 15:40:40.109120 capsulecorp-0.1.5/setup.cfg
+-rw-r--r--   0 daless383   (502) staff       (20)     6621 2023-07-12 13:53:07.000000 capsulecorp-0.1.5/setup.py
```

### Comparing `capsulecorp-0.1.4/LICENSE` & `capsulecorp-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `capsulecorp-0.1.4/capsulecorp/query_driver.py` & `capsulecorp-0.1.5/capsulecorp/query_driver.py`

 * *Files identical despite different names*

### Comparing `capsulecorp-0.1.4/capsulecorp/utilities/databricks_utils.py` & `capsulecorp-0.1.5/capsulecorp/utilities/databricks_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 import os
 import base64
 import json
 import requests
 from databricks_cli.sdk.api_client import ApiClient
 from databricks_cli.sdk.service import WorkspaceService
+from databricks_cli.dbfs.cli import DbfsApi
 
 
 def update_global_init_script(host, token, script_text, script_id, name):
     """
         This method will update a DataBricks global init script.
 
         Args:
```

### Comparing `capsulecorp-0.1.4/capsulecorp/utilities/github_utils.py` & `capsulecorp-0.1.5/capsulecorp/utilities/github_utils.py`

 * *Files identical despite different names*

### Comparing `capsulecorp-0.1.4/capsulecorp/utilities/slack_utils.py` & `capsulecorp-0.1.5/capsulecorp/utilities/slack_utils.py`

 * *Files identical despite different names*

### Comparing `capsulecorp-0.1.4/capsulecorp/utils.py` & `capsulecorp-0.1.5/capsulecorp/utils.py`

 * *Files identical despite different names*

### Comparing `capsulecorp-0.1.4/setup.py` & `capsulecorp-0.1.5/setup.py`

 * *Files identical despite different names*

