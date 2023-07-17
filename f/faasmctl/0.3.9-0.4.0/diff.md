# Comparing `tmp/faasmctl-0.3.9.tar.gz` & `tmp/faasmctl-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faasmctl-0.3.9.tar", last modified: Sun Jul 16 11:36:59 2023, max compression
+gzip compressed data, was "faasmctl-0.4.0.tar", last modified: Mon Jul 17 09:25:00 2023, max compression
```

## Comparing `faasmctl-0.3.9.tar` & `faasmctl-0.4.0.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:36:59.933112 faasmctl-0.3.9/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-16 11:34:09.000000 faasmctl-0.3.9/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-16 11:36:59.933112 faasmctl-0.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-16 11:34:09.000000 faasmctl-0.3.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:36:59.925111 faasmctl-0.3.9/faasmctl/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-16 11:34:09.000000 faasmctl-0.3.9/faasmctl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-16 11:34:09.000000 faasmctl-0.3.9/faasmctl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:36:59.929112 faasmctl-0.3.9/faasmctl/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-16 11:34:09.000000 faasmctl-0.3.9/faasmctl/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-16 11:34:09.000000 faasmctl-0.3.9/faasmctl/tasks/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-16 11:34:09.000000 faasmctl-0.3.9/faasmctl/tasks/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-07-16 11:34:09.000000 faasmctl-0.3.9/faasmctl/tasks/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-16 11:34:09.000000 faasmctl-0.3.9/faasmctl/tasks/flush.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-16 11:34:09.000000 faasmctl-0.3.9/faasmctl/tasks/invoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-16 11:34:09.000000 faasmctl-0.3.9/faasmctl/tasks/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-16 11:34:09.000000 faasmctl-0.3.9/faasmctl/tasks/restart.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-16 11:34:09.000000 faasmctl-0.3.9/faasmctl/tasks/status.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-16 11:34:09.000000 faasmctl-0.3.9/faasmctl/tasks/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:36:59.933112 faasmctl-0.3.9/faasmctl/util/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-16 11:34:09.000000 faasmctl-0.3.9/faasmctl/util/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-16 11:34:09.000000 faasmctl-0.3.9/faasmctl/util/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-07-16 11:34:09.000000 faasmctl-0.3.9/faasmctl/util/compose.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-16 11:34:09.000000 faasmctl-0.3.9/faasmctl/util/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-07-16 11:34:09.000000 faasmctl-0.3.9/faasmctl/util/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-16 11:34:09.000000 faasmctl-0.3.9/faasmctl/util/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-16 11:34:09.000000 faasmctl-0.3.9/faasmctl/util/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-16 11:34:09.000000 faasmctl-0.3.9/faasmctl/util/faasm.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-16 11:34:09.000000 faasmctl-0.3.9/faasmctl/util/flush.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:36:59.933112 faasmctl-0.3.9/faasmctl/util/gen_proto/
--rw-r--r--   0 runner    (1001) docker     (123)     9147 2023-07-16 11:36:48.000000 faasmctl-0.3.9/faasmctl/util/gen_proto/faabric_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-07-16 11:36:48.000000 faasmctl-0.3.9/faasmctl/util/gen_proto/planner_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-07-16 11:34:09.000000 faasmctl-0.3.9/faasmctl/util/invoke.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-16 11:34:09.000000 faasmctl-0.3.9/faasmctl/util/message.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-16 11:34:09.000000 faasmctl-0.3.9/faasmctl/util/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-16 11:34:09.000000 faasmctl-0.3.9/faasmctl/util/planner.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-16 11:34:09.000000 faasmctl-0.3.9/faasmctl/util/random.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-16 11:34:09.000000 faasmctl-0.3.9/faasmctl/util/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-16 11:34:09.000000 faasmctl-0.3.9/faasmctl/util/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:36:59.929112 faasmctl-0.3.9/faasmctl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-16 11:36:59.000000 faasmctl-0.3.9/faasmctl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-16 11:36:59.000000 faasmctl-0.3.9/faasmctl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 11:36:59.000000 faasmctl-0.3.9/faasmctl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-16 11:36:59.000000 faasmctl-0.3.9/faasmctl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-16 11:36:59.000000 faasmctl-0.3.9/faasmctl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-16 11:36:59.000000 faasmctl-0.3.9/faasmctl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-16 11:34:09.000000 faasmctl-0.3.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-16 11:36:59.933112 faasmctl-0.3.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:25:00.732379 faasmctl-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-17 09:22:58.000000 faasmctl-0.4.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-17 09:25:00.732379 faasmctl-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-17 09:22:58.000000 faasmctl-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:25:00.720379 faasmctl-0.4.0/faasmctl/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-17 09:22:58.000000 faasmctl-0.4.0/faasmctl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-17 09:22:58.000000 faasmctl-0.4.0/faasmctl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:25:00.724379 faasmctl-0.4.0/faasmctl/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-17 09:22:58.000000 faasmctl-0.4.0/faasmctl/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-17 09:22:58.000000 faasmctl-0.4.0/faasmctl/tasks/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-17 09:22:58.000000 faasmctl-0.4.0/faasmctl/tasks/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-07-17 09:22:58.000000 faasmctl-0.4.0/faasmctl/tasks/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-17 09:22:58.000000 faasmctl-0.4.0/faasmctl/tasks/flush.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-17 09:22:58.000000 faasmctl-0.4.0/faasmctl/tasks/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-17 09:22:58.000000 faasmctl-0.4.0/faasmctl/tasks/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-17 09:22:58.000000 faasmctl-0.4.0/faasmctl/tasks/restart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-17 09:22:58.000000 faasmctl-0.4.0/faasmctl/tasks/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-17 09:22:58.000000 faasmctl-0.4.0/faasmctl/tasks/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:25:00.732379 faasmctl-0.4.0/faasmctl/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-17 09:22:58.000000 faasmctl-0.4.0/faasmctl/util/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-17 09:22:58.000000 faasmctl-0.4.0/faasmctl/util/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-07-17 09:22:58.000000 faasmctl-0.4.0/faasmctl/util/compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-17 09:22:58.000000 faasmctl-0.4.0/faasmctl/util/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-07-17 09:22:58.000000 faasmctl-0.4.0/faasmctl/util/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-17 09:22:58.000000 faasmctl-0.4.0/faasmctl/util/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-17 09:22:58.000000 faasmctl-0.4.0/faasmctl/util/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-17 09:22:58.000000 faasmctl-0.4.0/faasmctl/util/faasm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-17 09:22:58.000000 faasmctl-0.4.0/faasmctl/util/flush.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:25:00.732379 faasmctl-0.4.0/faasmctl/util/gen_proto/
+-rw-r--r--   0 runner    (1001) docker     (123)     9147 2023-07-17 09:24:51.000000 faasmctl-0.4.0/faasmctl/util/gen_proto/faabric_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-07-17 09:24:51.000000 faasmctl-0.4.0/faasmctl/util/gen_proto/planner_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-07-17 09:22:58.000000 faasmctl-0.4.0/faasmctl/util/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-07-17 09:22:58.000000 faasmctl-0.4.0/faasmctl/util/k8s.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-17 09:22:58.000000 faasmctl-0.4.0/faasmctl/util/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-17 09:22:58.000000 faasmctl-0.4.0/faasmctl/util/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-17 09:22:58.000000 faasmctl-0.4.0/faasmctl/util/planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-17 09:22:58.000000 faasmctl-0.4.0/faasmctl/util/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-17 09:22:58.000000 faasmctl-0.4.0/faasmctl/util/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-17 09:22:58.000000 faasmctl-0.4.0/faasmctl/util/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:25:00.720379 faasmctl-0.4.0/faasmctl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-17 09:25:00.000000 faasmctl-0.4.0/faasmctl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-17 09:25:00.000000 faasmctl-0.4.0/faasmctl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 09:25:00.000000 faasmctl-0.4.0/faasmctl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-17 09:25:00.000000 faasmctl-0.4.0/faasmctl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-17 09:25:00.000000 faasmctl-0.4.0/faasmctl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-17 09:25:00.000000 faasmctl-0.4.0/faasmctl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-17 09:22:58.000000 faasmctl-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-17 09:25:00.732379 faasmctl-0.4.0/setup.cfg
```

### Comparing `faasmctl-0.3.9/LICENSE.md` & `faasmctl-0.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.9/PKG-INFO` & `faasmctl-0.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faasmctl
-Version: 0.3.9
+Version: 0.4.0
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
-pip install faasmctl==0.3.9
+pip install faasmctl==0.4.0
 ```
 
 ## Usage
 
 `faasmctl` aggregates tasks related to deploying, managing, and interacting
 with running Faasm clusters. You can list all the available tasks with a
 short description using:
```

### Comparing `faasmctl-0.3.9/README.md` & `faasmctl-0.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 running [Faasm](https://github.com/faasm/faasm) cluster.
 
 ## Install
 
 To install `faasmctl` you need a working `pip` (virtual-)environment. Then:
 
 ```bash
-pip install faasmctl==0.3.9
+pip install faasmctl==0.4.0
 ```
 
 ## Usage
 
 `faasmctl` aggregates tasks related to deploying, managing, and interacting
 with running Faasm clusters. You can list all the available tasks with a
 short description using:
```

### Comparing `faasmctl-0.3.9/faasmctl/tasks/cli.py` & `faasmctl-0.4.0/faasmctl/tasks/cli.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.9/faasmctl/tasks/delete.py` & `faasmctl-0.4.0/faasmctl/tasks/restart.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,30 @@
-from faasmctl.util.compose import delete_compose_cluster
-from faasmctl.util.config import get_faasm_ini_file, get_faasm_ini_value
+from faasmctl.util.backend import COMPOSE_BACKEND
+from faasmctl.util.compose import run_compose_cmd
+from faasmctl.util.config import (
+    BACKEND_INI_STRING,
+    get_faasm_ini_file,
+    get_faasm_ini_value,
+)
 from invoke import task
 
 
-@task(default=True)
-def delete(ctx, ini_file=None):
+@task(default=True, iterable=["s"])
+def restart(ctx, s, ini_file=None):
     """
-    Delete a running Faasm cluster
+    Restart a running service in the cluster
 
     Parameters:
-    - ini_file (str): path to the cluster's INI file (FAASM_INI_FILE env. var
-                      if not found)
+    - s (str, repeateble): service to get the logs from
+    - ini_file (str): path to the cluster's INI file
     """
     if not ini_file:
         ini_file = get_faasm_ini_file()
 
-    backend = get_faasm_ini_value(ini_file, "Faasm", "backend")
-    if backend == "compose":
-        delete_compose_cluster(ini_file)
-    else:
-        raise RuntimeError("Unsupported backend: {}".format(backend))
+    backend = get_faasm_ini_value(ini_file, "Faasm", BACKEND_INI_STRING)
+    if backend != COMPOSE_BACKEND:
+        raise RuntimeError(
+            "Can only get a CLI shell for a cluster that is "
+            "running on a '{}' backend".format(COMPOSE_BACKEND)
+        )
+
+    run_compose_cmd(ini_file, "restart {}".format(" ".join(s)))
```

### Comparing `faasmctl-0.3.9/faasmctl/tasks/deploy.py` & `faasmctl-0.4.0/faasmctl/tasks/deploy.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,14 @@
-from faasmctl.util.compose import deploy_compose_cluster, run_compose_cmd
+from faasmctl.util.compose import (
+    deploy_compose_cluster,
+    populate_host_sysroot,
+    run_compose_cmd,
+)
 from faasmctl.util.deploy import fetch_faasm_code
+from faasmctl.util.k8s import DEFAULT_KUBECONFIG_PATH, deploy_k8s_cluster
 from invoke import task
 from os.path import abspath
 
 
 @task
 def compose(ctx, workers=2, mount_source=None, clean=False, ini_file=None):
     """
@@ -27,14 +32,18 @@
                 "env. variable is disabled, as local changes could be "
                 "erased!"
             )
         faasm_checkout, faasm_ver = fetch_faasm_code(
             faasm_source=mount_source, force=False
         )
         mount_source = True
+
+        # If mounting the source code, we need to populate the host's
+        # sysroot to mount it into the containers
+        populate_host_sysroot(faasm_checkout)
     else:
         # Otherwise, we will check out the code in a faasmctl-specific working
         # directoy
         mount_source = False
         faasm_checkout, faasm_ver = fetch_faasm_code(force=clean)
 
     return deploy_compose_cluster(faasm_checkout, workers, mount_source, ini_file)
@@ -59,7 +68,32 @@
     # right ini file, and picks up the correct env. variables)
     out_ini_file = compose(
         ctx, workers=0, mount_source=mount_source, clean=False, ini_file=ini_file
     )
 
     # Second, start the dist-test-server
     run_compose_cmd(out_ini_file, "up -d dist-test-server")
+
+
+@task
+def k8s(ctx, workers=2, context=None, ini_file=None):
+    """
+    Deploy a Faasm cluster on k8s
+
+    Parameters:
+    - workers (int): number of workers to deploy
+    - context (str): path to the k8s config to use (defaults to ~/.kube/config)
+    - ini_file (str): path to the ini_file to generate (if selected)
+
+    Returns:
+    - (str): path to the generated ini_file
+    """
+    # First, check-out the Faasm source if necessary (we need it for the k8s
+    # deployment files, eventually we could publish them as helm charts)
+    faasm_checkout, faasm_ver = fetch_faasm_code()
+
+    if not context:
+        context = DEFAULT_KUBECONFIG_PATH
+    else:
+        context = abspath(context)
+
+    return deploy_k8s_cluster(context, faasm_checkout, workers, ini_file)
```

### Comparing `faasmctl-0.3.9/faasmctl/tasks/flush.py` & `faasmctl-0.4.0/faasmctl/tasks/flush.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.9/faasmctl/tasks/invoke.py` & `faasmctl-0.4.0/faasmctl/tasks/invoke.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.9/faasmctl/tasks/logs.py` & `faasmctl-0.4.0/faasmctl/tasks/logs.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.9/faasmctl/tasks/restart.py` & `faasmctl-0.4.0/faasmctl/tasks/status.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,27 +4,26 @@
     BACKEND_INI_STRING,
     get_faasm_ini_file,
     get_faasm_ini_value,
 )
 from invoke import task
 
 
-@task(default=True, iterable=["s"])
-def restart(ctx, s, ini_file=None):
+@task(default=True)
+def services(ctx, ini_file=None):
     """
-    Restart a running service in the cluster
+    Get the status of the running services in the cluster
 
     Parameters:
-    - s (str, repeateble): service to get the logs from
     - ini_file (str): path to the cluster's INI file
     """
     if not ini_file:
         ini_file = get_faasm_ini_file()
 
     backend = get_faasm_ini_value(ini_file, "Faasm", BACKEND_INI_STRING)
     if backend != COMPOSE_BACKEND:
         raise RuntimeError(
             "Can only get a CLI shell for a cluster that is "
             "running on a '{}' backend".format(COMPOSE_BACKEND)
         )
 
-    run_compose_cmd(ini_file, "restart {}".format(" ".join(s)))
+    run_compose_cmd(ini_file, "ps -a")
```

### Comparing `faasmctl-0.3.9/faasmctl/util/compose.py` & `faasmctl-0.4.0/faasmctl/util/compose.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from faasmctl.util.config import get_faasm_ini_value
 from faasmctl.util.deploy import generate_ini_file
 from faasmctl.util.random import generate_gid
-from os import environ
-from os.path import isfile, join
+from os import environ, makedirs
+from os.path import exists, isfile, join
+from shutil import rmtree
 from subprocess import run
 from time import sleep
 
 
 def get_compose_env_vars(faasm_checkout, mount_source):
     env = {}
     if mount_source:
@@ -158,7 +159,71 @@
                 break
 
             print(
                 "Waiting for python virtual environment to be ready "
                 "at {} ...".format(venv_path)
             )
             sleep(3)
+
+
+def populate_host_sysroot(faasm_checkout, clean=False):
+    """
+    Populate the host's sysroot under `./dev/faasm-local` to be shared by
+    all containers in a compose cluster with mounted-in binaries and code
+    """
+    dirs_to_copy = {
+        "FAASM_CLI_IMAGE": ["runtime_root"],
+        "CPP_CLI_IMAGE": ["llvm-sysroot", "native", "toolchain"],
+        "PYTHON_CLI_IMAGE": ["python3.8"],
+    }
+
+    # TODO: should we make this variable configurable?
+    host_sysroot_path = join(faasm_checkout, "dev", "faasm-local")
+
+    if clean:
+        rmtree(host_sysroot_path)
+
+    if exists(host_sysroot_path):
+        return
+
+    makedirs(host_sysroot_path)
+
+    def copy_from_ctr_to_host(image_tag, dir_path):
+        """
+        Helper method to copy data from the sysroot inside a docker container
+        into the host's mounted (and shared) sysroot
+        """
+        ctr_path = join("/usr/local/faasm", dir_path)
+        host_path = join(host_sysroot_path, dir_path)
+
+        # Start a temporary ctr to copy from
+        tmp_ctr = "cp_sysroot_ctr"
+        run_cmd = "docker run -d --name {} {}".format(tmp_ctr, image_tag)
+        run(run_cmd, shell=True, check=True)
+
+        # Do the actual copy
+        try:
+            print("Populating {} from {}:{}".format(host_path, ctr_path, image_tag))
+            cp_cmd = "docker cp {}:{} {}".format(tmp_ctr, ctr_path, host_path)
+            run(cp_cmd, shell=True, check=True)
+        except Exception as e:
+            print("Caught exception copying: {}".format(e))
+
+        # Delete the tmp container unconditionally
+        del_cmd = "docker rm -f {}".format(tmp_ctr)
+        run(del_cmd, shell=True, check=True)
+
+    # Get the docker image tags from the .env file in Faasm's source checkout
+    env_file_path = join(faasm_checkout, ".env")
+    with open(env_file_path, "r") as fh:
+        env_file = fh.readlines()
+        env_file = [line.strip() for line in env_file]
+
+    # Get the actual image tag by finding the right line in the file. We are
+    # unncesserily iterating over the files three times, but we don't care
+    for image in dirs_to_copy:
+        image_tag = [line.split("=")[1] for line in env_file if line.startswith(image)]
+        assert len(image_tag) == 1
+        image_tag = image_tag[0]
+
+        for dir_path in dirs_to_copy[image]:
+            copy_from_ctr_to_host(image_tag, dir_path)
```

### Comparing `faasmctl-0.3.9/faasmctl/util/config.py` & `faasmctl-0.4.0/faasmctl/util/config.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.9/faasmctl/util/deploy.py` & `faasmctl-0.4.0/faasmctl/util/deploy.py`

 * *Files 12% similar despite different names*

```diff
@@ -64,17 +64,20 @@
                 " probably due to an issue in Faasm where some directories "
                 "in a compose cluster are root-owned (in the container). "
                 "Try running the following:\n{}".format(tmp_fix)
             )
             raise RuntimeError("Error. Try running:\n{}".format(tmp_fix))
 
     # FIXME: allow a purely detached faasm checkout. Right now, cpp's code
-    # source is _always_ mounted from clients/cpp
+    # source is _always_ mounted from clients/cpp, and so is clients/python,
+    # and transitively clients/python/third-party/cpp
     git_cmd = "git submodule update --init"
     run(git_cmd, shell=True, check=True, cwd=checkout_path)
+    git_cmd = "git submodule update --init ./third-party/cpp"
+    run(git_cmd, shell=True, check=True, cwd=join(checkout_path, "clients", "python"))
 
     faasm_ver = _check_version_mismatch(checkout_path)
 
     return checkout_path, faasm_ver
 
 
 def generate_ini_file(backend, out_file, **kwargs):
@@ -86,33 +89,48 @@
 
         upload_ip = LOCALHOST_IP
         upload_port = "8002"
         planner_ip = LOCALHOST_IP
         planner_port = "8080"
         worker_names = []
         worker_ips = []
+    elif backend == "k8s":
+        working_dir = kwargs["cwd"]
+        k8s_config = kwargs["k8s_config"]
+        k8s_namespace = kwargs["k8s_namespace"]
+
+        upload_ip = kwargs["upload_ip"]
+        upload_port = kwargs["upload_port"]
+        planner_ip = kwargs["planner_ip"]
+        planner_port = kwargs["planner_port"]
+        worker_names = kwargs["worker_names"]
+        worker_ips = kwargs["worker_ips"]
     else:
         raise RuntimeError("Backend {} not supported!".format(backend))
 
     if not out_file:
         out_file = "./faasm.ini"
 
     print("Generating Faasm INI file at: {}".format(out_file))
     with open(out_file, "w") as fh:
         fh.write("[Faasm]\n")
 
         # This comment line can't be outside of the Faasm section
         fh.write("# Auto-generated at {}\n".format(datetime.now()))
 
         fh.write("backend = {}\n".format(backend))
+        fh.write("working_dir = {}\n".format(working_dir))
         if backend == "compose":
-            fh.write("working_dir = {}\n".format(working_dir))
             fh.write("mount_source = {}\n".format(kwargs["mount_source"]))
+        elif backend == "k8s":
+            fh.write("k8s_config = {}\n".format(k8s_config))
         if backend == "compose":
             fh.write("cluster_name = {}\n".format(cluster_name))
+        elif backend == "k8s":
+            fh.write("k8s_namespace = {}\n".format(k8s_namespace))
         fh.write("upload_host = {}\n".format(upload_ip))
         if backend == "compose":
             fh.write("upload_host_in_docker = upload\n")
         fh.write("upload_port = {}\n".format(upload_port))
         fh.write("planner_host = {}\n".format(planner_ip))
         if backend == "compose":
             fh.write("planner_host_in_docker = planner\n")
```

### Comparing `faasmctl-0.3.9/faasmctl/util/docker.py` & `faasmctl-0.4.0/faasmctl/util/docker.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.9/faasmctl/util/flush.py` & `faasmctl-0.4.0/faasmctl/util/flush.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.9/faasmctl/util/gen_proto/faabric_pb2.py` & `faasmctl-0.4.0/faasmctl/util/gen_proto/faabric_pb2.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.9/faasmctl/util/gen_proto/planner_pb2.py` & `faasmctl-0.4.0/faasmctl/util/gen_proto/planner_pb2.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.9/faasmctl/util/invoke.py` & `faasmctl-0.4.0/faasmctl/util/invoke.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.9/faasmctl/util/planner.py` & `faasmctl-0.4.0/faasmctl/util/planner.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.9/faasmctl/util/upload.py` & `faasmctl-0.4.0/faasmctl/util/upload.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.9/faasmctl.egg-info/PKG-INFO` & `faasmctl-0.4.0/faasmctl.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faasmctl
-Version: 0.3.9
+Version: 0.4.0
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
-pip install faasmctl==0.3.9
+pip install faasmctl==0.4.0
 ```
 
 ## Usage
 
 `faasmctl` aggregates tasks related to deploying, managing, and interacting
 with running Faasm clusters. You can list all the available tasks with a
 short description using:
```

### Comparing `faasmctl-0.3.9/faasmctl.egg-info/SOURCES.txt` & `faasmctl-0.4.0/faasmctl.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 faasmctl/util/config.py
 faasmctl/util/deploy.py
 faasmctl/util/docker.py
 faasmctl/util/env.py
 faasmctl/util/faasm.py
 faasmctl/util/flush.py
 faasmctl/util/invoke.py
+faasmctl/util/k8s.py
 faasmctl/util/message.py
 faasmctl/util/network.py
 faasmctl/util/planner.py
 faasmctl/util/random.py
 faasmctl/util/upload.py
 faasmctl/util/version.py
 faasmctl/util/gen_proto/faabric_pb2.py
```

### Comparing `faasmctl-0.3.9/pyproject.toml` & `faasmctl-0.4.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "faasmctl"
-version = "0.3.9"
+version = "0.4.0"
 authors = [
   { name="Faasm Team", email="foo@bar.com" },
 ]
 description = "Command line tool to deploy, manage, and interact with Faasm"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

