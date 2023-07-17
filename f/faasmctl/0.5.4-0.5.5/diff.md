# Comparing `tmp/faasmctl-0.5.4.tar.gz` & `tmp/faasmctl-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faasmctl-0.5.4.tar", last modified: Mon Jul 17 21:28:16 2023, max compression
+gzip compressed data, was "faasmctl-0.5.5.tar", last modified: Mon Jul 17 21:34:05 2023, max compression
```

## Comparing `faasmctl-0.5.4.tar` & `faasmctl-0.5.5.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:28:16.507284 faasmctl-0.5.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-07-17 21:26:16.000000 faasmctl-0.5.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-17 21:28:16.507284 faasmctl-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-17 21:26:16.000000 faasmctl-0.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:28:16.495284 faasmctl-0.5.4/faasmctl/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-17 21:26:16.000000 faasmctl-0.5.4/faasmctl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-17 21:26:16.000000 faasmctl-0.5.4/faasmctl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:28:16.499284 faasmctl-0.5.4/faasmctl/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-17 21:26:16.000000 faasmctl-0.5.4/faasmctl/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-17 21:26:16.000000 faasmctl-0.5.4/faasmctl/tasks/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-17 21:26:16.000000 faasmctl-0.5.4/faasmctl/tasks/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-07-17 21:26:16.000000 faasmctl-0.5.4/faasmctl/tasks/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-17 21:26:16.000000 faasmctl-0.5.4/faasmctl/tasks/flush.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-17 21:26:16.000000 faasmctl-0.5.4/faasmctl/tasks/invoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-17 21:26:16.000000 faasmctl-0.5.4/faasmctl/tasks/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-17 21:26:16.000000 faasmctl-0.5.4/faasmctl/tasks/restart.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-17 21:26:16.000000 faasmctl-0.5.4/faasmctl/tasks/status.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-17 21:26:16.000000 faasmctl-0.5.4/faasmctl/tasks/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:28:16.507284 faasmctl-0.5.4/faasmctl/util/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-17 21:26:16.000000 faasmctl-0.5.4/faasmctl/util/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-17 21:26:16.000000 faasmctl-0.5.4/faasmctl/util/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     8490 2023-07-17 21:26:16.000000 faasmctl-0.5.4/faasmctl/util/compose.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-17 21:26:16.000000 faasmctl-0.5.4/faasmctl/util/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-07-17 21:26:16.000000 faasmctl-0.5.4/faasmctl/util/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-17 21:26:16.000000 faasmctl-0.5.4/faasmctl/util/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-17 21:26:16.000000 faasmctl-0.5.4/faasmctl/util/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-17 21:26:16.000000 faasmctl-0.5.4/faasmctl/util/faasm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-17 21:26:16.000000 faasmctl-0.5.4/faasmctl/util/flush.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:28:16.507284 faasmctl-0.5.4/faasmctl/util/gen_proto/
--rw-r--r--   0 runner    (1001) docker     (123)     9147 2023-07-17 21:28:07.000000 faasmctl-0.5.4/faasmctl/util/gen_proto/faabric_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-07-17 21:28:07.000000 faasmctl-0.5.4/faasmctl/util/gen_proto/planner_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-07-17 21:26:16.000000 faasmctl-0.5.4/faasmctl/util/invoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-07-17 21:26:16.000000 faasmctl-0.5.4/faasmctl/util/k8s.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-17 21:26:16.000000 faasmctl-0.5.4/faasmctl/util/message.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-17 21:26:16.000000 faasmctl-0.5.4/faasmctl/util/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-17 21:26:16.000000 faasmctl-0.5.4/faasmctl/util/planner.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-17 21:26:16.000000 faasmctl-0.5.4/faasmctl/util/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-17 21:26:16.000000 faasmctl-0.5.4/faasmctl/util/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-17 21:26:16.000000 faasmctl-0.5.4/faasmctl/util/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:28:16.499284 faasmctl-0.5.4/faasmctl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-17 21:28:16.000000 faasmctl-0.5.4/faasmctl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-17 21:28:16.000000 faasmctl-0.5.4/faasmctl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 21:28:16.000000 faasmctl-0.5.4/faasmctl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-17 21:28:16.000000 faasmctl-0.5.4/faasmctl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-17 21:28:16.000000 faasmctl-0.5.4/faasmctl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-17 21:28:16.000000 faasmctl-0.5.4/faasmctl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-17 21:26:16.000000 faasmctl-0.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-17 21:28:16.507284 faasmctl-0.5.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:34:05.459586 faasmctl-0.5.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-07-17 21:32:01.000000 faasmctl-0.5.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-17 21:34:05.459586 faasmctl-0.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-17 21:32:01.000000 faasmctl-0.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:34:05.447585 faasmctl-0.5.5/faasmctl/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-17 21:32:01.000000 faasmctl-0.5.5/faasmctl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-17 21:32:01.000000 faasmctl-0.5.5/faasmctl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:34:05.451585 faasmctl-0.5.5/faasmctl/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-17 21:32:01.000000 faasmctl-0.5.5/faasmctl/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-17 21:32:01.000000 faasmctl-0.5.5/faasmctl/tasks/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-17 21:32:01.000000 faasmctl-0.5.5/faasmctl/tasks/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-07-17 21:32:01.000000 faasmctl-0.5.5/faasmctl/tasks/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-17 21:32:01.000000 faasmctl-0.5.5/faasmctl/tasks/flush.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-17 21:32:01.000000 faasmctl-0.5.5/faasmctl/tasks/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-17 21:32:01.000000 faasmctl-0.5.5/faasmctl/tasks/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-17 21:32:01.000000 faasmctl-0.5.5/faasmctl/tasks/restart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-17 21:32:01.000000 faasmctl-0.5.5/faasmctl/tasks/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-17 21:32:01.000000 faasmctl-0.5.5/faasmctl/tasks/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:34:05.459586 faasmctl-0.5.5/faasmctl/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-17 21:32:01.000000 faasmctl-0.5.5/faasmctl/util/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-17 21:32:01.000000 faasmctl-0.5.5/faasmctl/util/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-07-17 21:32:01.000000 faasmctl-0.5.5/faasmctl/util/compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-17 21:32:01.000000 faasmctl-0.5.5/faasmctl/util/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-07-17 21:32:01.000000 faasmctl-0.5.5/faasmctl/util/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-17 21:32:01.000000 faasmctl-0.5.5/faasmctl/util/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-17 21:32:01.000000 faasmctl-0.5.5/faasmctl/util/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-17 21:32:01.000000 faasmctl-0.5.5/faasmctl/util/faasm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-17 21:32:01.000000 faasmctl-0.5.5/faasmctl/util/flush.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:34:05.459586 faasmctl-0.5.5/faasmctl/util/gen_proto/
+-rw-r--r--   0 runner    (1001) docker     (123)     9147 2023-07-17 21:33:56.000000 faasmctl-0.5.5/faasmctl/util/gen_proto/faabric_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-07-17 21:33:56.000000 faasmctl-0.5.5/faasmctl/util/gen_proto/planner_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-07-17 21:32:01.000000 faasmctl-0.5.5/faasmctl/util/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-07-17 21:32:01.000000 faasmctl-0.5.5/faasmctl/util/k8s.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-17 21:32:01.000000 faasmctl-0.5.5/faasmctl/util/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-17 21:32:01.000000 faasmctl-0.5.5/faasmctl/util/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-17 21:32:01.000000 faasmctl-0.5.5/faasmctl/util/planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-17 21:32:01.000000 faasmctl-0.5.5/faasmctl/util/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-17 21:32:01.000000 faasmctl-0.5.5/faasmctl/util/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-17 21:32:01.000000 faasmctl-0.5.5/faasmctl/util/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:34:05.451585 faasmctl-0.5.5/faasmctl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-17 21:34:05.000000 faasmctl-0.5.5/faasmctl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-17 21:34:05.000000 faasmctl-0.5.5/faasmctl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 21:34:05.000000 faasmctl-0.5.5/faasmctl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-17 21:34:05.000000 faasmctl-0.5.5/faasmctl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-17 21:34:05.000000 faasmctl-0.5.5/faasmctl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-17 21:34:05.000000 faasmctl-0.5.5/faasmctl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-17 21:32:01.000000 faasmctl-0.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-17 21:34:05.459586 faasmctl-0.5.5/setup.cfg
```

### Comparing `faasmctl-0.5.4/LICENSE.md` & `faasmctl-0.5.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `faasmctl-0.5.4/PKG-INFO` & `faasmctl-0.5.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faasmctl
-Version: 0.5.4
+Version: 0.5.5
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
-pip install faasmctl==0.5.4
+pip install faasmctl==0.5.5
 ```
 
 ## Usage
 
 `faasmctl` aggregates tasks related to deploying, managing, and interacting
 with running Faasm clusters. You can list all the available tasks with a
 short description using:
```

### Comparing `faasmctl-0.5.4/README.md` & `faasmctl-0.5.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 running [Faasm](https://github.com/faasm/faasm) cluster.
 
 ## Install
 
 To install `faasmctl` you need a working `pip` (virtual-)environment. Then:
 
 ```bash
-pip install faasmctl==0.5.4
+pip install faasmctl==0.5.5
 ```
 
 ## Usage
 
 `faasmctl` aggregates tasks related to deploying, managing, and interacting
 with running Faasm clusters. You can list all the available tasks with a
 short description using:
```

### Comparing `faasmctl-0.5.4/faasmctl/tasks/cli.py` & `faasmctl-0.5.5/faasmctl/tasks/cli.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.5.4/faasmctl/tasks/delete.py` & `faasmctl-0.5.5/faasmctl/tasks/delete.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.5.4/faasmctl/tasks/deploy.py` & `faasmctl-0.5.5/faasmctl/tasks/deploy.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.5.4/faasmctl/tasks/flush.py` & `faasmctl-0.5.5/faasmctl/tasks/flush.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.5.4/faasmctl/tasks/invoke.py` & `faasmctl-0.5.5/faasmctl/tasks/invoke.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.5.4/faasmctl/tasks/logs.py` & `faasmctl-0.5.5/faasmctl/tasks/logs.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.5.4/faasmctl/tasks/restart.py` & `faasmctl-0.5.5/faasmctl/tasks/restart.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.5.4/faasmctl/tasks/status.py` & `faasmctl-0.5.5/faasmctl/tasks/status.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.5.4/faasmctl/util/compose.py` & `faasmctl-0.5.5/faasmctl/util/compose.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,15 +171,19 @@
     all containers in a compose cluster with mounted-in binaries and code
     """
     dirs_to_copy = {
         "FAASM_CLI_IMAGE": ["runtime_root"],
         "CPP_CLI_IMAGE": ["llvm-sysroot", "native", "toolchain"],
         "PYTHON_CLI_IMAGE": [
             "python3.8",
+            # We are specific about which bits to copy from the llvm-sysroot
+            # for the python functions. Overwriting all the sysroot with the
+            # one tracked in the CPython image is unneccessary
             join("llvm-sysroot", "lib", "wasm32-wasi", "libpython3.8.a"),
+            join("llvm-sysroot", "lib", "include", "python3.8"),
         ],
     }
 
     # TODO: should we make this variable configurable?
     host_sysroot_path = join(faasm_checkout, "dev", "faasm-local")
 
     if clean:
```

### Comparing `faasmctl-0.5.4/faasmctl/util/config.py` & `faasmctl-0.5.5/faasmctl/util/config.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.5.4/faasmctl/util/deploy.py` & `faasmctl-0.5.5/faasmctl/util/deploy.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.5.4/faasmctl/util/docker.py` & `faasmctl-0.5.5/faasmctl/util/docker.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.5.4/faasmctl/util/flush.py` & `faasmctl-0.5.5/faasmctl/util/flush.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.5.4/faasmctl/util/gen_proto/faabric_pb2.py` & `faasmctl-0.5.5/faasmctl/util/gen_proto/faabric_pb2.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.5.4/faasmctl/util/gen_proto/planner_pb2.py` & `faasmctl-0.5.5/faasmctl/util/gen_proto/planner_pb2.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.5.4/faasmctl/util/invoke.py` & `faasmctl-0.5.5/faasmctl/util/invoke.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.5.4/faasmctl/util/k8s.py` & `faasmctl-0.5.5/faasmctl/util/k8s.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.5.4/faasmctl/util/planner.py` & `faasmctl-0.5.5/faasmctl/util/planner.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.5.4/faasmctl/util/upload.py` & `faasmctl-0.5.5/faasmctl/util/upload.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.5.4/faasmctl.egg-info/PKG-INFO` & `faasmctl-0.5.5/faasmctl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faasmctl
-Version: 0.5.4
+Version: 0.5.5
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
-pip install faasmctl==0.5.4
+pip install faasmctl==0.5.5
 ```
 
 ## Usage
 
 `faasmctl` aggregates tasks related to deploying, managing, and interacting
 with running Faasm clusters. You can list all the available tasks with a
 short description using:
```

### Comparing `faasmctl-0.5.4/faasmctl.egg-info/SOURCES.txt` & `faasmctl-0.5.5/faasmctl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `faasmctl-0.5.4/pyproject.toml` & `faasmctl-0.5.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "faasmctl"
-version = "0.5.4"
+version = "0.5.5"
 authors = [
   { name="Faasm Team", email="foo@bar.com" },
 ]
 description = "Command line tool to deploy, manage, and interact with Faasm"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

