# Comparing `tmp/faasmctl-0.4.2.tar.gz` & `tmp/faasmctl-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faasmctl-0.4.2.tar", last modified: Mon Jul 17 10:21:49 2023, max compression
+gzip compressed data, was "faasmctl-0.5.0.tar", last modified: Mon Jul 17 20:14:37 2023, max compression
```

## Comparing `faasmctl-0.4.2.tar` & `faasmctl-0.5.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:21:49.062049 faasmctl-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-17 10:18:01.000000 faasmctl-0.4.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-17 10:21:49.062049 faasmctl-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-17 10:18:01.000000 faasmctl-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:21:49.054049 faasmctl-0.4.2/faasmctl/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-17 10:18:01.000000 faasmctl-0.4.2/faasmctl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-17 10:18:01.000000 faasmctl-0.4.2/faasmctl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:21:49.058049 faasmctl-0.4.2/faasmctl/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-17 10:18:01.000000 faasmctl-0.4.2/faasmctl/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-17 10:18:01.000000 faasmctl-0.4.2/faasmctl/tasks/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-17 10:18:01.000000 faasmctl-0.4.2/faasmctl/tasks/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-07-17 10:18:01.000000 faasmctl-0.4.2/faasmctl/tasks/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-17 10:18:01.000000 faasmctl-0.4.2/faasmctl/tasks/flush.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-17 10:18:01.000000 faasmctl-0.4.2/faasmctl/tasks/invoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-17 10:18:01.000000 faasmctl-0.4.2/faasmctl/tasks/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-17 10:18:01.000000 faasmctl-0.4.2/faasmctl/tasks/restart.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-17 10:18:01.000000 faasmctl-0.4.2/faasmctl/tasks/status.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-17 10:18:01.000000 faasmctl-0.4.2/faasmctl/tasks/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:21:49.058049 faasmctl-0.4.2/faasmctl/util/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-17 10:18:01.000000 faasmctl-0.4.2/faasmctl/util/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-17 10:18:01.000000 faasmctl-0.4.2/faasmctl/util/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-07-17 10:18:01.000000 faasmctl-0.4.2/faasmctl/util/compose.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-17 10:18:01.000000 faasmctl-0.4.2/faasmctl/util/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-07-17 10:18:01.000000 faasmctl-0.4.2/faasmctl/util/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-17 10:18:01.000000 faasmctl-0.4.2/faasmctl/util/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-17 10:18:01.000000 faasmctl-0.4.2/faasmctl/util/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-17 10:18:01.000000 faasmctl-0.4.2/faasmctl/util/faasm.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-17 10:18:01.000000 faasmctl-0.4.2/faasmctl/util/flush.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:21:49.062049 faasmctl-0.4.2/faasmctl/util/gen_proto/
--rw-r--r--   0 runner    (1001) docker     (123)     9147 2023-07-17 10:21:36.000000 faasmctl-0.4.2/faasmctl/util/gen_proto/faabric_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-07-17 10:21:36.000000 faasmctl-0.4.2/faasmctl/util/gen_proto/planner_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-07-17 10:18:01.000000 faasmctl-0.4.2/faasmctl/util/invoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-07-17 10:18:01.000000 faasmctl-0.4.2/faasmctl/util/k8s.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-17 10:18:01.000000 faasmctl-0.4.2/faasmctl/util/message.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-17 10:18:01.000000 faasmctl-0.4.2/faasmctl/util/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-17 10:18:01.000000 faasmctl-0.4.2/faasmctl/util/planner.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-17 10:18:01.000000 faasmctl-0.4.2/faasmctl/util/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-17 10:18:01.000000 faasmctl-0.4.2/faasmctl/util/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-17 10:18:01.000000 faasmctl-0.4.2/faasmctl/util/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:21:49.054049 faasmctl-0.4.2/faasmctl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-17 10:21:49.000000 faasmctl-0.4.2/faasmctl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-17 10:21:49.000000 faasmctl-0.4.2/faasmctl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 10:21:49.000000 faasmctl-0.4.2/faasmctl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-17 10:21:49.000000 faasmctl-0.4.2/faasmctl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-17 10:21:49.000000 faasmctl-0.4.2/faasmctl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-17 10:21:49.000000 faasmctl-0.4.2/faasmctl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-17 10:18:01.000000 faasmctl-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-17 10:21:49.062049 faasmctl-0.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:14:37.653576 faasmctl-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-07-17 20:11:28.000000 faasmctl-0.5.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-17 20:14:37.653576 faasmctl-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-17 20:11:28.000000 faasmctl-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:14:37.645576 faasmctl-0.5.0/faasmctl/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-17 20:11:28.000000 faasmctl-0.5.0/faasmctl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-17 20:11:28.000000 faasmctl-0.5.0/faasmctl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:14:37.649576 faasmctl-0.5.0/faasmctl/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-17 20:11:28.000000 faasmctl-0.5.0/faasmctl/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-17 20:11:28.000000 faasmctl-0.5.0/faasmctl/tasks/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-17 20:11:28.000000 faasmctl-0.5.0/faasmctl/tasks/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-07-17 20:11:28.000000 faasmctl-0.5.0/faasmctl/tasks/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-17 20:11:28.000000 faasmctl-0.5.0/faasmctl/tasks/flush.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-17 20:11:28.000000 faasmctl-0.5.0/faasmctl/tasks/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-17 20:11:28.000000 faasmctl-0.5.0/faasmctl/tasks/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-17 20:11:28.000000 faasmctl-0.5.0/faasmctl/tasks/restart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-17 20:11:28.000000 faasmctl-0.5.0/faasmctl/tasks/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-17 20:11:28.000000 faasmctl-0.5.0/faasmctl/tasks/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:14:37.653576 faasmctl-0.5.0/faasmctl/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-17 20:11:28.000000 faasmctl-0.5.0/faasmctl/util/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-17 20:11:28.000000 faasmctl-0.5.0/faasmctl/util/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-07-17 20:11:28.000000 faasmctl-0.5.0/faasmctl/util/compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-17 20:11:28.000000 faasmctl-0.5.0/faasmctl/util/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-07-17 20:11:28.000000 faasmctl-0.5.0/faasmctl/util/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-17 20:11:28.000000 faasmctl-0.5.0/faasmctl/util/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-17 20:11:28.000000 faasmctl-0.5.0/faasmctl/util/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-17 20:11:28.000000 faasmctl-0.5.0/faasmctl/util/faasm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-17 20:11:28.000000 faasmctl-0.5.0/faasmctl/util/flush.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:14:37.653576 faasmctl-0.5.0/faasmctl/util/gen_proto/
+-rw-r--r--   0 runner    (1001) docker     (123)     9147 2023-07-17 20:14:25.000000 faasmctl-0.5.0/faasmctl/util/gen_proto/faabric_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-07-17 20:14:25.000000 faasmctl-0.5.0/faasmctl/util/gen_proto/planner_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-07-17 20:11:28.000000 faasmctl-0.5.0/faasmctl/util/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-07-17 20:11:28.000000 faasmctl-0.5.0/faasmctl/util/k8s.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-17 20:11:28.000000 faasmctl-0.5.0/faasmctl/util/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-17 20:11:28.000000 faasmctl-0.5.0/faasmctl/util/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-17 20:11:28.000000 faasmctl-0.5.0/faasmctl/util/planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-17 20:11:28.000000 faasmctl-0.5.0/faasmctl/util/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-17 20:11:28.000000 faasmctl-0.5.0/faasmctl/util/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-17 20:11:28.000000 faasmctl-0.5.0/faasmctl/util/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:14:37.645576 faasmctl-0.5.0/faasmctl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-17 20:14:37.000000 faasmctl-0.5.0/faasmctl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-17 20:14:37.000000 faasmctl-0.5.0/faasmctl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 20:14:37.000000 faasmctl-0.5.0/faasmctl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-17 20:14:37.000000 faasmctl-0.5.0/faasmctl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-17 20:14:37.000000 faasmctl-0.5.0/faasmctl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-17 20:14:37.000000 faasmctl-0.5.0/faasmctl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-17 20:11:28.000000 faasmctl-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-17 20:14:37.653576 faasmctl-0.5.0/setup.cfg
```

### Comparing `faasmctl-0.4.2/LICENSE.md` & `faasmctl-0.5.0/LICENSE.md`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright [yyyy] [name of copyright owner]
+   Copyright 2023 - Faasm Team
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `faasmctl-0.4.2/PKG-INFO` & `faasmctl-0.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faasmctl
-Version: 0.4.2
+Version: 0.5.0
 Summary: Command line tool to deploy, manage, and interact with Faasm
 Author-email: Faasm Team <foo@bar.com>
 Project-URL: Homepage, https://github.com/faasm/faasmctl
 Project-URL: Bug Tracker, https://github.com/faasm/faasmctl/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -17,15 +17,15 @@
 running [Faasm](https://github.com/faasm/faasm) cluster.
 
 ## Install
 
 To install `faasmctl` you need a working `pip` (virtual-)environment. Then:
 
 ```bash
-pip install faasmctl==0.4.2
+pip install faasmctl==0.5.0
 ```
 
 ## Usage
 
 `faasmctl` aggregates tasks related to deploying, managing, and interacting
 with running Faasm clusters. You can list all the available tasks with a
 short description using:
```

### Comparing `faasmctl-0.4.2/README.md` & `faasmctl-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 running [Faasm](https://github.com/faasm/faasm) cluster.
 
 ## Install
 
 To install `faasmctl` you need a working `pip` (virtual-)environment. Then:
 
 ```bash
-pip install faasmctl==0.4.2
+pip install faasmctl==0.5.0
 ```
 
 ## Usage
 
 `faasmctl` aggregates tasks related to deploying, managing, and interacting
 with running Faasm clusters. You can list all the available tasks with a
 short description using:
```

### Comparing `faasmctl-0.4.2/faasmctl/tasks/cli.py` & `faasmctl-0.5.0/faasmctl/tasks/cli.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.4.2/faasmctl/tasks/delete.py` & `faasmctl-0.5.0/faasmctl/tasks/delete.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.4.2/faasmctl/tasks/deploy.py` & `faasmctl-0.5.0/faasmctl/tasks/deploy.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.4.2/faasmctl/tasks/flush.py` & `faasmctl-0.5.0/faasmctl/tasks/flush.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.4.2/faasmctl/tasks/invoke.py` & `faasmctl-0.5.0/faasmctl/tasks/invoke.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.4.2/faasmctl/tasks/logs.py` & `faasmctl-0.5.0/faasmctl/tasks/logs.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.4.2/faasmctl/tasks/restart.py` & `faasmctl-0.5.0/faasmctl/tasks/restart.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.4.2/faasmctl/tasks/status.py` & `faasmctl-0.5.0/faasmctl/tasks/status.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.4.2/faasmctl/util/compose.py` & `faasmctl-0.5.0/faasmctl/util/compose.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.4.2/faasmctl/util/config.py` & `faasmctl-0.5.0/faasmctl/util/config.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.4.2/faasmctl/util/deploy.py` & `faasmctl-0.5.0/faasmctl/util/deploy.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.4.2/faasmctl/util/docker.py` & `faasmctl-0.5.0/faasmctl/util/docker.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.4.2/faasmctl/util/flush.py` & `faasmctl-0.5.0/faasmctl/util/flush.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.4.2/faasmctl/util/gen_proto/faabric_pb2.py` & `faasmctl-0.5.0/faasmctl/util/gen_proto/faabric_pb2.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.4.2/faasmctl/util/gen_proto/planner_pb2.py` & `faasmctl-0.5.0/faasmctl/util/gen_proto/planner_pb2.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.4.2/faasmctl/util/k8s.py` & `faasmctl-0.5.0/faasmctl/util/k8s.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.4.2/faasmctl/util/planner.py` & `faasmctl-0.5.0/faasmctl/util/planner.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from faasmctl.util.config import get_faasm_planner_host_port
 from faasmctl.util.gen_proto.planner_pb2 import HttpMessage
 from google.protobuf.json_format import MessageToJson
 from requests import post
 
 PLANNER_JSON_MESSAGE_FAILED = {"dead": "beef"}
 
 # ----------
@@ -35,19 +36,20 @@
 
 
 # ----------
 # RESET
 # ----------
 
 
-def reset(host, port):
+def reset():
     """
     Reset the planner with an HTTP request. Reset clears the available hosts,
     and the scheduling state
     """
+    host, port = get_faasm_planner_host_port()
     url = "http://{}:{}".format(host, port)
 
     planner_msg = prepare_planner_msg("RESET")
 
     response = post(url, data=planner_msg, timeout=None)
 
     if response.status_code != 200:
```

### Comparing `faasmctl-0.4.2/faasmctl.egg-info/PKG-INFO` & `faasmctl-0.5.0/faasmctl.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faasmctl
-Version: 0.4.2
+Version: 0.5.0
 Summary: Command line tool to deploy, manage, and interact with Faasm
 Author-email: Faasm Team <foo@bar.com>
 Project-URL: Homepage, https://github.com/faasm/faasmctl
 Project-URL: Bug Tracker, https://github.com/faasm/faasmctl/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -17,15 +17,15 @@
 running [Faasm](https://github.com/faasm/faasm) cluster.
 
 ## Install
 
 To install `faasmctl` you need a working `pip` (virtual-)environment. Then:
 
 ```bash
-pip install faasmctl==0.4.2
+pip install faasmctl==0.5.0
 ```
 
 ## Usage
 
 `faasmctl` aggregates tasks related to deploying, managing, and interacting
 with running Faasm clusters. You can list all the available tasks with a
 short description using:
```

### Comparing `faasmctl-0.4.2/faasmctl.egg-info/SOURCES.txt` & `faasmctl-0.5.0/faasmctl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `faasmctl-0.4.2/pyproject.toml` & `faasmctl-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "faasmctl"
-version = "0.4.2"
+version = "0.5.0"
 authors = [
   { name="Faasm Team", email="foo@bar.com" },
 ]
 description = "Command line tool to deploy, manage, and interact with Faasm"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

