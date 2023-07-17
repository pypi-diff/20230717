# Comparing `tmp/cluster_tools-1.60.tar.gz` & `tmp/cluster_tools-1.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cluster_tools-1.60.tar", last modified: Thu Aug  5 13:31:35 2021, max compression
+gzip compressed data, was "dist/cluster_tools-1.61.tar", last modified: Tue Nov  2 12:48:55 2021, max compression
```

## Comparing `cluster_tools-1.60.tar` & `cluster_tools-1.61.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-05 13:31:35.000000 cluster_tools-1.60/
--rw-rw-r--   0 root         (0) root         (0)     1312 2021-08-05 13:19:10.000000 cluster_tools-1.60/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-05 13:31:35.000000 cluster_tools-1.60/dockered-slurm/
--rw-rw-r--   0 root         (0) root         (0)      914 2021-08-05 13:19:10.000000 cluster_tools-1.60/dockered-slurm/how-to.md
--rw-rw-r--   0 root         (0) root         (0)     2512 2021-08-05 13:19:10.000000 cluster_tools-1.60/dockered-slurm/README.md
--rw-rw-r--   0 root         (0) root         (0)     1072 2021-08-05 13:19:10.000000 cluster_tools-1.60/dockered-slurm/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      721 2021-08-05 13:19:10.000000 cluster_tools-1.60/dockered-slurm/slurmdbd.conf
--rwxrwxr-x   0 root         (0) root         (0)     1588 2021-08-05 13:19:10.000000 cluster_tools-1.60/dockered-slurm/docker-entrypoint.sh
--rw-rw-r--   0 root         (0) root         (0)     2043 2021-08-05 13:19:10.000000 cluster_tools-1.60/dockered-slurm/slurm.conf
--rw-rw-r--   0 root         (0) root         (0)     3688 2021-08-05 13:19:10.000000 cluster_tools-1.60/dockered-slurm/Dockerfile
--rw-rw-r--   0 root         (0) root         (0)     1074 2021-08-05 13:19:10.000000 cluster_tools-1.60/dockered-slurm/setup-pbs.sh
--rw-rw-r--   0 root         (0) root         (0)      175 2021-08-05 13:19:10.000000 cluster_tools-1.60/dockered-slurm/pbs.conf
--rwxrwxr-x   0 root         (0) root         (0)      152 2021-08-05 13:19:10.000000 cluster_tools-1.60/dockered-slurm/register_cluster.sh
--rw-rw-r--   0 root         (0) root         (0)     1754 2021-08-05 13:19:10.000000 cluster_tools-1.60/dockered-slurm/docker-compose.yml
--rw-rw-r--   0 root         (0) root         (0)     1071 2021-08-05 13:19:10.000000 cluster_tools-1.60/LICENSE
--rw-r--r--   0 root         (0) root         (0)       38 2021-08-05 13:31:35.000000 cluster_tools-1.60/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-05 13:31:35.000000 cluster_tools-1.60/cluster_tools.egg-info/
--rw-r--r--   0 root         (0) root         (0)      929 2021-08-05 13:31:35.000000 cluster_tools-1.60/cluster_tools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-08-05 13:31:35.000000 cluster_tools-1.60/cluster_tools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2021-08-05 13:31:35.000000 cluster_tools-1.60/cluster_tools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2021-08-05 13:31:35.000000 cluster_tools-1.60/cluster_tools.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      392 2021-08-05 13:31:35.000000 cluster_tools-1.60/cluster_tools.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     1733 2021-08-05 13:19:10.000000 cluster_tools-1.60/.gitignore
--rw-rw-r--   0 root         (0) root         (0)    18278 2021-08-05 13:19:10.000000 cluster_tools-1.60/test.py
--rw-rw-r--   0 root         (0) root         (0)      734 2021-08-05 13:19:10.000000 cluster_tools-1.60/setup.py
--rw-rw-r--   0 root         (0) root         (0)     1609 2021-08-05 13:19:10.000000 cluster_tools-1.60/slurm_example.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-05 13:31:35.000000 cluster_tools-1.60/cluster_tools/
--rw-rw-r--   0 root         (0) root         (0)     2287 2021-08-05 13:19:10.000000 cluster_tools-1.60/cluster_tools/pickling.py
--rw-rw-r--   0 root         (0) root         (0)    10391 2021-08-05 13:19:10.000000 cluster_tools-1.60/cluster_tools/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2354 2021-08-05 13:19:10.000000 cluster_tools-1.60/cluster_tools/tailf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-05 13:31:35.000000 cluster_tools-1.60/cluster_tools/schedulers/
--rw-rw-r--   0 root         (0) root         (0)    16623 2021-08-05 13:19:10.000000 cluster_tools-1.60/cluster_tools/schedulers/cluster_executor.py
--rw-rw-r--   0 root         (0) root         (0)        0 2021-08-05 13:19:10.000000 cluster_tools-1.60/cluster_tools/schedulers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5804 2021-08-05 13:19:10.000000 cluster_tools-1.60/cluster_tools/schedulers/pbs.py
--rw-rw-r--   0 root         (0) root         (0)     6414 2021-08-05 13:19:10.000000 cluster_tools-1.60/cluster_tools/schedulers/slurm.py
--rw-rw-r--   0 root         (0) root         (0)     5046 2021-08-05 13:19:10.000000 cluster_tools-1.60/cluster_tools/remote.py
--rw-rw-r--   0 root         (0) root         (0)     7574 2021-08-05 13:19:10.000000 cluster_tools-1.60/cluster_tools/util.py
--rw-rw-r--   0 root         (0) root         (0)     4634 2021-08-05 13:19:10.000000 cluster_tools-1.60/cluster_tools/multiprocessing_logging_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-05 13:31:35.000000 cluster_tools-1.60/.github/
--rw-rw-r--   0 root         (0) root         (0)      125 2021-08-05 13:19:10.000000 cluster_tools-1.60/.github/dependabot.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-05 13:31:35.000000 cluster_tools-1.60/.circleci/
--rwxrwxr-x   0 root         (0) root         (0)     3089 2021-08-05 13:19:10.000000 cluster_tools-1.60/.circleci/config.yml
--rw-rw-r--   0 root         (0) root         (0)    13768 2021-08-05 13:19:10.000000 cluster_tools-1.60/.pylintrc
--rw-r--r--   0 root         (0) root         (0)      392 2021-08-05 13:31:35.000000 cluster_tools-1.60/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-02 12:48:55.000000 cluster_tools-1.61/
+-rw-rw-r--   0 root         (0) root         (0)     1312 2021-11-02 12:32:20.000000 cluster_tools-1.61/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-02 12:48:55.000000 cluster_tools-1.61/dockered-slurm/
+-rw-rw-r--   0 root         (0) root         (0)      914 2021-11-02 12:32:20.000000 cluster_tools-1.61/dockered-slurm/how-to.md
+-rw-rw-r--   0 root         (0) root         (0)     2482 2021-11-02 12:32:20.000000 cluster_tools-1.61/dockered-slurm/README.md
+-rw-rw-r--   0 root         (0) root         (0)     1072 2021-11-02 12:32:20.000000 cluster_tools-1.61/dockered-slurm/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      721 2021-11-02 12:32:20.000000 cluster_tools-1.61/dockered-slurm/slurmdbd.conf
+-rwxrwxr-x   0 root         (0) root         (0)     1588 2021-11-02 12:32:20.000000 cluster_tools-1.61/dockered-slurm/docker-entrypoint.sh
+-rw-rw-r--   0 root         (0) root         (0)     2058 2021-11-02 12:32:20.000000 cluster_tools-1.61/dockered-slurm/slurm.conf
+-rw-rw-r--   0 root         (0) root         (0)     3688 2021-11-02 12:32:20.000000 cluster_tools-1.61/dockered-slurm/Dockerfile
+-rw-rw-r--   0 root         (0) root         (0)     1074 2021-11-02 12:32:20.000000 cluster_tools-1.61/dockered-slurm/setup-pbs.sh
+-rw-rw-r--   0 root         (0) root         (0)      175 2021-11-02 12:32:20.000000 cluster_tools-1.61/dockered-slurm/pbs.conf
+-rwxrwxr-x   0 root         (0) root         (0)      152 2021-11-02 12:32:20.000000 cluster_tools-1.61/dockered-slurm/register_cluster.sh
+-rw-rw-r--   0 root         (0) root         (0)     1790 2021-11-02 12:32:20.000000 cluster_tools-1.61/dockered-slurm/docker-compose.yml
+-rw-rw-r--   0 root         (0) root         (0)     1071 2021-11-02 12:32:20.000000 cluster_tools-1.61/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       38 2021-11-02 12:48:55.000000 cluster_tools-1.61/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-02 12:48:55.000000 cluster_tools-1.61/cluster_tools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      929 2021-11-02 12:48:55.000000 cluster_tools-1.61/cluster_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-11-02 12:48:55.000000 cluster_tools-1.61/cluster_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2021-11-02 12:48:55.000000 cluster_tools-1.61/cluster_tools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2021-11-02 12:48:55.000000 cluster_tools-1.61/cluster_tools.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      392 2021-11-02 12:48:55.000000 cluster_tools-1.61/cluster_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     1748 2021-11-02 12:32:20.000000 cluster_tools-1.61/.gitignore
+-rw-rw-r--   0 root         (0) root         (0)    24458 2021-11-02 12:32:20.000000 cluster_tools-1.61/test.py
+-rw-rw-r--   0 root         (0) root         (0)      734 2021-11-02 12:32:20.000000 cluster_tools-1.61/setup.py
+-rw-rw-r--   0 root         (0) root         (0)     1609 2021-11-02 12:32:20.000000 cluster_tools-1.61/slurm_example.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-02 12:48:55.000000 cluster_tools-1.61/cluster_tools/
+-rw-rw-r--   0 root         (0) root         (0)     2309 2021-11-02 12:32:20.000000 cluster_tools-1.61/cluster_tools/pickling.py
+-rw-rw-r--   0 root         (0) root         (0)    10391 2021-11-02 12:32:20.000000 cluster_tools-1.61/cluster_tools/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2216 2021-11-02 12:32:20.000000 cluster_tools-1.61/cluster_tools/tailf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-02 12:48:55.000000 cluster_tools-1.61/cluster_tools/schedulers/
+-rw-rw-r--   0 root         (0) root         (0)    19079 2021-11-02 12:32:20.000000 cluster_tools-1.61/cluster_tools/schedulers/cluster_executor.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-11-02 12:32:20.000000 cluster_tools-1.61/cluster_tools/schedulers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6060 2021-11-02 12:32:20.000000 cluster_tools-1.61/cluster_tools/schedulers/pbs.py
+-rw-rw-r--   0 root         (0) root         (0)    12156 2021-11-02 12:32:20.000000 cluster_tools-1.61/cluster_tools/schedulers/slurm.py
+-rw-rw-r--   0 root         (0) root         (0)     5251 2021-11-02 12:32:20.000000 cluster_tools-1.61/cluster_tools/remote.py
+-rw-rw-r--   0 root         (0) root         (0)     7598 2021-11-02 12:32:20.000000 cluster_tools-1.61/cluster_tools/util.py
+-rw-rw-r--   0 root         (0) root         (0)     4634 2021-11-02 12:32:20.000000 cluster_tools-1.61/cluster_tools/multiprocessing_logging_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-02 12:48:55.000000 cluster_tools-1.61/.github/
+-rw-rw-r--   0 root         (0) root         (0)      125 2021-11-02 12:32:20.000000 cluster_tools-1.61/.github/dependabot.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-02 12:48:55.000000 cluster_tools-1.61/.circleci/
+-rwxrwxr-x   0 root         (0) root         (0)     3089 2021-11-02 12:32:20.000000 cluster_tools-1.61/.circleci/config.yml
+-rw-rw-r--   0 root         (0) root         (0)    14052 2021-11-02 12:32:20.000000 cluster_tools-1.61/.pylintrc
+-rw-r--r--   0 root         (0) root         (0)      392 2021-11-02 12:48:55.000000 cluster_tools-1.61/PKG-INFO
```

### Comparing `cluster_tools-1.60/README.md` & `cluster_tools-1.61/README.md`

 * *Files identical despite different names*

### Comparing `cluster_tools-1.60/dockered-slurm/how-to.md` & `cluster_tools-1.61/dockered-slurm/how-to.md`

 * *Files identical despite different names*

### Comparing `cluster_tools-1.60/dockered-slurm/README.md` & `cluster_tools-1.61/dockered-slurm/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -96,9 +96,9 @@
 
 ## Deleting the Cluster
 
 To remove all containers and volumes, run:
 
 ```console
 $ docker-compose rm -sf
-$ docker volume rm slurm-docker-cluster_etc_munge slurm-docker-cluster_etc_slurm slurm-docker-cluster_slurm_jobdir slurm-docker-cluster_var_lib_mysql slurm-docker-cluster_var_log_slurm
+$ docker volume rm dockered-slurm_etc_munge dockered-slurm_etc_slurm dockered-slurm_slurm_jobdir dockered-slurm_var_lib_mysql dockered-slurm_var_log_slurm
 ```
```

### Comparing `cluster_tools-1.60/dockered-slurm/LICENSE` & `cluster_tools-1.61/dockered-slurm/LICENSE`

 * *Files identical despite different names*

### Comparing `cluster_tools-1.60/dockered-slurm/slurmdbd.conf` & `cluster_tools-1.61/dockered-slurm/slurmdbd.conf`

 * *Files identical despite different names*

### Comparing `cluster_tools-1.60/dockered-slurm/docker-entrypoint.sh` & `cluster_tools-1.61/dockered-slurm/docker-entrypoint.sh`

 * *Files identical despite different names*

### Comparing `cluster_tools-1.60/dockered-slurm/slurm.conf` & `cluster_tools-1.61/dockered-slurm/slurm.conf`

 * *Files 3% similar despite different names*

```diff
@@ -88,7 +88,9 @@
 #AccountingStorageUser=
 #
 # COMPUTE NODES
 NodeName=c[1-2] RealMemory=1000 State=UNKNOWN
 #
 # PARTITIONS
 PartitionName=normal Default=yes Nodes=c[1-2] Priority=50 DefMemPerCPU=500 Shared=NO MaxNodes=1 MaxTime=5-00:00:00 DefaultTime=5-00:00:00 State=UP
+#
+# JOB ARRAYS
```

### Comparing `cluster_tools-1.60/dockered-slurm/Dockerfile` & `cluster_tools-1.61/dockered-slurm/Dockerfile`

 * *Files identical despite different names*

### Comparing `cluster_tools-1.60/dockered-slurm/setup-pbs.sh` & `cluster_tools-1.61/dockered-slurm/setup-pbs.sh`

 * *Files identical despite different names*

### Comparing `cluster_tools-1.60/dockered-slurm/docker-compose.yml` & `cluster_tools-1.61/dockered-slurm/docker-compose.yml`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,16 @@
     depends_on:
       - mysql
 
   slurmctld:
     image: slurm-docker-cluster:latest
     command: ["slurmctld"]
     container_name: slurmctld
+    environment:
+      USER: "root"
     hostname: slurmctld
     volumes:
       - etc_munge:/etc/munge
       - etc_slurm:/etc/slurm
       - ./slurm_jobdir:/data
       - ..:/cluster_tools
       - var_log_slurm:/var/log/slurm
```

### Comparing `cluster_tools-1.60/LICENSE` & `cluster_tools-1.61/LICENSE`

 * *Files identical despite different names*

### Comparing `cluster_tools-1.60/cluster_tools.egg-info/SOURCES.txt` & `cluster_tools-1.61/cluster_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cluster_tools-1.60/.gitignore` & `cluster_tools-1.61/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 .coverage.*
 .cache
 nosetests.xml
 coverage.xml
 *.cover
 .hypothesis/
 .pytest_cache/
+test_cfut_dir/
 
 # Translations
 *.mo
 *.pot
 
 # Django stuff:
 *.log
```

### Comparing `cluster_tools-1.60/test.py` & `cluster_tools-1.61/test.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import cluster_tools
+from cluster_tools.util import call
 import concurrent.futures
 import time
 import logging
 from enum import Enum
 from functools import partial
 import os
 import pytest
 import shutil
 import contextlib
 import io
 import multiprocessing as mp
 from pathlib import Path
 import tempfile
+from collections import Counter
 
 # "Worker" functions.
 def square(n):
     return n * n
 
 
 def sleep(duration):
@@ -368,14 +370,181 @@
         future = exc.submit(square, 2)
         assert future.result() == 4
 
     assert os.path.exists(cfut_dir)
     assert len(os.listdir(cfut_dir)) == 2
 
 
+def test_slurm_max_submit_user():
+    max_submit_jobs = 6
+
+    # MaxSubmitJobs can either be defined at the user or at the qos level
+    for command in ["user root", "qos normal"]:
+        executor = cluster_tools.get_executor("slurm", debug=True)
+        original_max_submit_jobs = executor.get_max_submit_jobs()
+
+        _, _, exit_code = call(
+            f"echo y | sacctmgr modify {command} set MaxSubmitJobs={max_submit_jobs}"
+        )
+        try:
+            assert exit_code == 0
+
+            new_max_submit_jobs = executor.get_max_submit_jobs()
+            assert new_max_submit_jobs == max_submit_jobs
+
+            with executor:
+                futures = executor.map_to_futures(square, range(10))
+
+                result = [fut.result() for fut in futures]
+                assert result == [i ** 2 for i in range(10)]
+
+                job_ids = {fut.cluster_jobid for fut in futures}
+                # The 10 work packages should have been scheduled as 5 separate jobs,
+                # because the cluster_tools schedule at most 1/3 of MaxSubmitJobs at once.
+                assert len(job_ids) == 5
+        finally:
+            _, _, exit_code = call(
+                f"echo y | sacctmgr modify {command} set MaxSubmitJobs=-1"
+            )
+            assert exit_code == 0
+            reset_max_submit_jobs = executor.get_max_submit_jobs()
+            assert reset_max_submit_jobs == original_max_submit_jobs
+
+
+def test_slurm_deferred_submit():
+    max_submit_jobs = 1
+
+    # Only one job can be scheduled at a time
+    _, _, exit_code = call(
+        f"echo y | sacctmgr modify qos normal set MaxSubmitJobs={max_submit_jobs}"
+    )
+    executor = cluster_tools.get_executor("slurm", debug=True)
+
+    try:
+        with executor:
+            time_of_start = time.time()
+            futures = executor.map_to_futures(sleep, [0.5, 0.5])
+            time_of_futures = time.time()
+            concurrent.futures.wait(futures)
+            time_of_result = time.time()
+
+            # The futures should be returned before each job was scheduled
+            assert time_of_futures - time_of_start < 0.5
+
+            # Computing the results should have taken at least two seconds
+            # since only one job is scheduled at a time and each job takes 0.5 seconds
+            assert time_of_result - time_of_start > 1
+    finally:
+        _, _, exit_code = call(
+            "echo y | sacctmgr modify qos normal set MaxSubmitJobs=-1"
+        )
+
+
+def wait_until_first_job_was_submitted(executor):
+    # Since the job submission is not synchronous, we need to poll
+    # to find out when the first job was submitted
+    while executor.get_number_of_submitted_jobs() <= 0:
+        time.sleep(0.1)
+
+
+def test_slurm_deferred_submit_shutdown():
+    # Test that the SlurmExecutor stops scheduling jobs in a separate thread
+    # once it was killed even if the executor was used multiple times and
+    # therefore started multiple job submission threads
+    max_submit_jobs = 1
+
+    # Only one job can be scheduled at a time
+    _, _, exit_code = call(
+        f"echo y | sacctmgr modify qos normal set MaxSubmitJobs={max_submit_jobs}"
+    )
+    executor = cluster_tools.get_executor("slurm", debug=True)
+
+    try:
+        # Use the executor twice to start multiple job submission threads
+        executor.map_to_futures(sleep, [0.5] * 10)
+        executor.map_to_futures(sleep, [0.5] * 10)
+
+        wait_until_first_job_was_submitted(executor)
+
+        for submit_thread in executor.submit_threads:
+            assert submit_thread.is_alive()
+
+        with pytest.raises(SystemExit) as pytest_wrapped_e:
+            executor.handle_kill(None, None)
+        assert pytest_wrapped_e.type == SystemExit
+        assert pytest_wrapped_e.value.code == 130
+
+        # Wait for the threads to die down, but less than it would take to submit all jobs
+        # which would take ~5 seconds since only one job is scheduled at a time
+        for submit_thread in executor.submit_threads:
+            submit_thread.join(1)
+            assert not submit_thread.is_alive()
+
+        # Wait for scheduled jobs to finish, so that the queue is empty again
+        while executor.get_number_of_submitted_jobs() > 0:
+            time.sleep(0.5)
+
+    finally:
+        _, _, exit_code = call(
+            "echo y | sacctmgr modify qos normal set MaxSubmitJobs=-1"
+        )
+
+
+def test_slurm_number_of_submitted_jobs():
+    number_of_jobs = 6
+    executor = cluster_tools.get_executor("slurm", debug=True)
+
+    assert executor.get_number_of_submitted_jobs() == 0
+
+    with executor:
+        futures = executor.map_to_futures(sleep, [1] * number_of_jobs)
+
+        wait_until_first_job_was_submitted(executor)
+
+        assert executor.get_number_of_submitted_jobs() == number_of_jobs
+
+        concurrent.futures.wait(futures)
+        assert executor.get_number_of_submitted_jobs() == 0
+
+
+def test_slurm_max_array_size():
+    max_array_size = 2
+
+    executor = cluster_tools.get_executor("slurm", debug=True)
+    original_max_array_size = executor.get_max_array_size()
+
+    command = f"MaxArraySize={max_array_size}"
+    _, _, exit_code = call(
+        f"echo -e '{command}' >> /etc/slurm/slurm.conf && scontrol reconfigure"
+    )
+
+    try:
+        assert exit_code == 0
+
+        new_max_array_size = executor.get_max_array_size()
+        assert new_max_array_size == max_array_size
+
+        with executor:
+            futures = executor.map_to_futures(square, range(6))
+            concurrent.futures.wait(futures)
+            job_ids = [fut.cluster_jobid for fut in futures]
+
+            # Count how often each job_id occurs which corresponds to the array size of the job
+            occurences = list(Counter(job_ids).values())
+
+            assert all(array_size <= max_array_size for array_size in occurences)
+    finally:
+        _, _, exit_code = call(
+            f"sed -i 's/{command}//g' /etc/slurm/slurm.conf && scontrol reconfigure"
+        )
+        assert exit_code == 0
+        reset_max_array_size = executor.get_max_array_size()
+        assert reset_max_array_size == original_max_array_size
+
+
 def test_executor_args():
     def pass_with(exc):
         with exc:
             pass
 
     pass_with(
         cluster_tools.get_executor(
@@ -486,15 +655,15 @@
 
 
 def accept_high_mem(data):
     return len(data)
 
 
 @pytest.mark.skip(
-    reason="This test is does not pass on the CI. Probably because the machine does not have enough RAM."
+    reason="This test does not pass on the CI. Probably because the machine does not have enough RAM."
 )
 def test_high_ram_usage():
     very_long_string = " " * 10 ** 6 * 2500
 
     os.environ["MULTIPROCESSING_VIA_IO"] = "True"
 
     with cluster_tools.get_executor("multiprocessing") as executor:
@@ -561,16 +730,17 @@
             # Schedule failing jobs and verify that only a preliminary output exists
 
             futs = executor.map_to_futures(
                 fail,
                 list(a_range),
                 output_pickle_path_getter=partial(output_pickle_path_getter, tmp_dir),
             )
-            with pytest.raises(Exception):
-                [fut.result() for fut in futs]
+            for fut in futs:
+                with pytest.raises(Exception):
+                    fut.result()
 
             for idx in a_range:
                 output_pickle_path = Path(output_pickle_path_getter(tmp_dir, idx))
                 preliminary_output_path = Path(f"{output_pickle_path}.preliminary")
 
                 assert (
                     preliminary_output_path.exists()
@@ -582,15 +752,15 @@
             # Schedule succeeding jobs with same output paths
             futs = executor.map_to_futures(
                 square,
                 list(a_range),
                 output_pickle_path_getter=partial(output_pickle_path_getter, tmp_dir),
             )
             for (fut, job_index) in zip(futs, a_range):
-                fut.result() == square(job_index)
+                assert fut.result() == square(job_index)
 
             for idx in a_range:
                 output_pickle_path = Path(output_pickle_path_getter(tmp_dir, idx))
                 preliminary_output_path = Path(f"{output_pickle_path}.preliminary")
                 assert output_pickle_path.exists(), "Final output file should exist"
                 assert (
                     not preliminary_output_path.exists()
```

### Comparing `cluster_tools-1.60/setup.py` & `cluster_tools-1.61/setup.py`

 * *Files identical despite different names*

### Comparing `cluster_tools-1.60/slurm_example.py` & `cluster_tools-1.61/slurm_example.py`

 * *Files identical despite different names*

### Comparing `cluster_tools-1.60/cluster_tools/pickling.py` & `cluster_tools-1.61/cluster_tools/pickling.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 import sys
 import os
-import io
-import logging
 
 use_cloudpickle = "USE_CLOUDPICKLE" in os.environ
 
 if use_cloudpickle:
     import cloudpickle
 
     pickle_strategy = cloudpickle
 else:
     import pickle
 
     pickle_strategy = pickle
-import importlib
 from .util import warn_after
 
 WARNING_TIMEOUT = 10 * 60  # seconds
 
 
 def file_path_to_absolute_module(file_path):
     """
     Given a file path, return an import path.
     :param file_path: A file path.
     :return:
     """
     assert os.path.exists(file_path)
-    file_loc, ext = os.path.splitext(file_path)
+    file_loc, _ = os.path.splitext(file_path)
     directory, module = os.path.split(file_loc)
     module_path = [module]
     while True:
         if os.path.exists(os.path.join(directory, "__init__.py")):
             directory, package = os.path.split(directory)
             module_path.append(package)
         else:
@@ -76,9 +73,11 @@
 
         return super(RenameUnpickler, self).find_class(renamed_module, name)
 
 
 @warn_after("pickle.load", WARNING_TIMEOUT)
 def load(f, custom_main_path=None):
     unpickler = RenameUnpickler(f)
-    unpickler.custom_main_path = custom_main_path
+    unpickler.custom_main_path = (  # pylint: disable=attribute-defined-outside-init
+        custom_main_path
+    )
     return unpickler.load()
```

### Comparing `cluster_tools-1.60/cluster_tools/__init__.py` & `cluster_tools-1.61/cluster_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `cluster_tools-1.60/cluster_tools/tailf.py` & `cluster_tools-1.61/cluster_tools/tailf.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,33 +4,33 @@
 
 import os
 import sys
 import time
 
 
 class Tail(object):
-    """ Represents a tail command. """
+    """Represents a tail command."""
 
     def __init__(self, tailed_file, callback=sys.stdout.write):
-        """ Initiate a Tail instance.
-            Check for file validity, assigns callback function to standard out.
-            
-            Arguments:
-                tailed_file - File to be followed. """
+        """Initiate a Tail instance.
+        Check for file validity, assigns callback function to standard out.
+
+        Arguments:
+            tailed_file - File to be followed."""
 
         self.tailed_file = tailed_file
         self.callback = callback
         self.is_cancelled = False
 
     def follow(self, seconds=1):
-        """ Do a tail follow. If a callback function is registered it is called with every new line. 
+        """Do a tail follow. If a callback function is registered it is called with every new line.
         Else printed to standard out.
-    
+
         Arguments:
-            seconds - Number of seconds to wait between each iteration; Defaults to 1. """
+            seconds - Number of seconds to wait between each iteration; Defaults to 1."""
 
         self.check_file_validity(self.tailed_file)
         with open(self.tailed_file, errors="replace") as file_:
             # Don't seek, since we want to print the entire file here.
             while True:
                 line = file_.readline()
                 if not line:
@@ -44,26 +44,22 @@
                 else:
                     self.callback(line)
 
     def cancel(self):
         self.is_cancelled = True
 
     def register_callback(self, func):
-        """ Overrides default callback function to provided function. """
+        """Overrides default callback function to provided function."""
         self.callback = func
 
     def check_file_validity(self, file_):
-        """ Check whether the a given file exists, readable and is a file """
+        """Check whether the a given file exists, readable and is a file"""
         if not os.access(file_, os.F_OK):
             raise TailError("File '%s' does not exist" % (file_))
         if not os.access(file_, os.R_OK):
             raise TailError("File '%s' not readable" % (file_))
         if os.path.isdir(file_):
             raise TailError("File '%s' is a directory" % (file_))
 
 
 class TailError(Exception):
-    def __init__(self, msg):
-        self.message = msg
-
-    def __str__(self):
-        return self.message
+    pass
```

### Comparing `cluster_tools-1.60/cluster_tools/schedulers/cluster_executor.py` & `cluster_tools-1.61/cluster_tools/schedulers/cluster_executor.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 from cluster_tools import pickling
 from cluster_tools.pickling import file_path_to_absolute_module
 import time
 from abc import abstractmethod
 import logging
 from typing import Union
 from cluster_tools.tailf import Tail
-import shutil
+from functools import partial
 
 
 class RemoteException(Exception):
-    def __init__(self, error, job_id):
+    def __init__(self, error, job_id):  # pylint: disable=super-init-not-called
         self.error = error
         self.job_id = job_id
 
     def __str__(self):
         return str(self.job_id) + "\n" + self.error.strip()
 
 
@@ -35,30 +35,30 @@
     def __init__(
         self,
         debug=False,
         keep_logs=True,
         cfut_dir=None,
         job_resources=None,
         job_name=None,
-        additional_setup_lines=[],
+        additional_setup_lines=None,
         **kwargs,
     ):
         """
         `kwargs` can be the following optional parameters:
             `logging_config`: An object containing a `level` key specifying the desired log level and/or a
                 `format` key specifying the desired log format string. Cannot be specified together
                 with `logging_setup_fn`.
             `logging_setup_fn`: A function setting up custom logging. The function will be called for
                 remotely executed code (slurm, pbs) to re-setup logging. The function will be called with the
                 default log file name. If the caller sets up file logging, this log file name should be adapted,
                 for example, by adding a .mylog suffix. Cannot be specified together with `logging_config`.
         """
         self.debug = debug
         self.job_resources = job_resources
-        self.additional_setup_lines = additional_setup_lines
+        self.additional_setup_lines = additional_setup_lines or []
         self.job_name = job_name
         self.was_requested_to_shutdown = False
         self.cfut_dir = (
             cfut_dir if cfut_dir is not None else os.getenv("CFUT_DIR", ".cfut")
         )
         self.files_to_clean_up = []
 
@@ -88,42 +88,49 @@
             "logging_config" in kwargs and "logging_setup_fn" in kwargs
         ), "Specify either logging_config OR logging_setup_fn but not both at once"
         if "logging_config" in kwargs:
             self.meta_data["logging_config"] = kwargs["logging_config"]
         if "logging_setup_fn" in kwargs:
             self.meta_data["logging_setup_fn"] = kwargs["logging_setup_fn"]
 
-    def handle_kill(self, signum, frame):
+    def handle_kill(self, _signum, _frame):
         self.wait_thread.stop()
         job_ids = ",".join(str(id) for id in self.jobs.keys())
         print(
             "A termination signal was registered. The following jobs are still running on the cluster:\n{}".format(
                 job_ids
             )
         )
         sys.exit(130)
 
     @abstractmethod
     def check_for_crashed_job(self, job_id) -> Union["failed", "ignore", "completed"]:
         pass
 
     def _start(self, workerid, job_count=None, job_name=None):
-        """Start a job with the given worker ID and return an ID
-        identifying the new job. The job should run ``python -m
+        """Start job(s) with the given worker ID and return IDs
+        identifying the new job(s). The job should run ``python -m
         cfut.remote <workerid>.
         """
 
-        jobid = self.inner_submit(
+        jobids_futures, job_index_ranges = self.inner_submit(
             f"{sys.executable} -m cluster_tools.remote {workerid} {self.cfut_dir}",
             job_name=self.job_name if self.job_name is not None else job_name,
             additional_setup_lines=self.additional_setup_lines,
             job_count=job_count,
         )
 
-        return jobid
+        # Since not all jobs may be submitted immediately, cluster executors return
+        # jobid futures in the inner_submit function. Also, since it may not be allowed
+        # to submit all jobs at once, the jobs may be submitted in batches with each batch
+        # containing a subset of all jobs identified by a separate jobid. The job_index_ranges
+        # array of (start_index, end_index) tuples, indicates which of the job_count
+        # jobs were submitted in each batch. start_index is inclusive whereas end_index
+        # is not.
+        return jobids_futures, job_index_ranges
 
     @abstractmethod
     def inner_submit(self, *args, **kwargs):
         pass
 
     def _cleanup(self, jobid):
         """Given a job ID as returned by _start, perform any necessary
@@ -145,16 +152,17 @@
         return os.path.join(cfut_dir, cls.format_log_file_name(jobid, suffix))
 
     @classmethod
     @abstractmethod
     def get_job_id_string(self):
         pass
 
-    def get_temp_file_path(self, file_name):
-        return os.path.join(self.cfut_dir, file_name)
+    @staticmethod
+    def get_temp_file_path(cfut_dir, file_name):
+        return os.path.join(cfut_dir, file_name)
 
     @staticmethod
     def format_infile_name(cfut_dir, job_id):
         return os.path.join(cfut_dir, "cfut.in.%s.pickle" % job_id)
 
     @staticmethod
     def format_outfile_name(cfut_dir, job_id):
@@ -260,15 +268,17 @@
         if os.path.exists(preliminary_output_pickle_path):
             logging.warning(
                 f"Deleting stale output file at {preliminary_output_pickle_path}..."
             )
             os.unlink(preliminary_output_pickle_path)
 
         job_name = get_function_name(fun)
-        jobid = self._start(workerid, job_name=job_name)
+        jobids_futures, _ = self._start(workerid, job_name=job_name)
+        # Only a single job was submitted
+        jobid = jobids_futures[0].result()
 
         if self.debug:
             print("job submitted: %i" % jobid, file=sys.stderr)
 
         # Thread will wait for it to finish.
         self.wait_thread.waitFor(preliminary_output_pickle_path, jobid)
 
@@ -310,15 +320,14 @@
 
         pickled_function_path = self.get_function_pickle_path(workerid)
         self.files_to_clean_up.append(pickled_function_path)
         with open(pickled_function_path, "wb") as file:
             pickling.dump(fun, file)
         self.store_main_path_to_meta_file(workerid)
 
-        # Submit jobs eagerly
         for index, arg in enumerate(allArgs):
             fut = self.create_enriched_future()
             workerid_with_index = self.get_workerid_with_index(workerid, index)
 
             if output_pickle_path_getter is None:
                 output_pickle_path = self.format_outfile_name(
                     self.cfut_dir, workerid_with_index
@@ -331,57 +340,97 @@
             )
             if os.path.exists(preliminary_output_pickle_path):
                 logging.warning(
                     f"Deleting stale output file at {preliminary_output_pickle_path}..."
                 )
                 os.unlink(preliminary_output_pickle_path)
 
-            # Start the job.
             serialized_function_info = pickling.dumps(
                 (pickled_function_path, [arg], {}, self.meta_data, output_pickle_path)
             )
             infile_name = self.format_infile_name(self.cfut_dir, workerid_with_index)
 
             with open(infile_name, "wb") as f:
                 f.write(serialized_function_info)
 
             futs_with_output_paths.append((fut, output_pickle_path))
 
+        with self.jobs_lock:
+            # Use a separate loop to avoid having to acquire the jobs_lock many times
+            # or for the full duration of the above loop
+            for index in range(len(futs_with_output_paths)):
+                workerid_with_index = self.get_workerid_with_index(workerid, index)
+                # Register the job in the jobs array, although the jobid is not known yet.
+                # Otherwise it might happen that self.jobs becomes empty, but some of the jobs were
+                # not even submitted yet.
+                self.jobs[workerid_with_index] = "pending"
+
         job_count = len(allArgs)
         job_name = get_function_name(fun)
-        jobid = self._start(workerid, job_count, job_name)
+        jobids_futures, job_index_ranges = self._start(workerid, job_count, job_name)
+
+        number_of_batches = len(jobids_futures)
+        for batch_index, (jobid_future, (job_index_start, job_index_end)) in enumerate(
+            zip(jobids_futures, job_index_ranges)
+        ):
+            jobid_future.add_done_callback(
+                partial(
+                    self.register_jobs,
+                    futs_with_output_paths[job_index_start:job_index_end],
+                    workerid,
+                    should_keep_output,
+                    job_index_start,
+                    f"{batch_index + 1}/{number_of_batches}",
+                )
+            )
 
+        return [fut for (fut, _) in futs_with_output_paths]
+
+    def register_jobs(
+        self,
+        futs_with_output_paths,
+        workerid,
+        should_keep_output,
+        job_index_offset,
+        batch_description,
+        jobid_future,
+    ):
+        jobid = jobid_future.result()
         if self.debug:
+
             print(
-                "main job submitted: %i. consists of %i subjobs." % (jobid, job_count),
+                "Submitted array job {} with JobId {} and {} subjobs.".format(
+                    batch_description, jobid, len(futs_with_output_paths)
+                ),
                 file=sys.stderr,
             )
 
-        with self.jobs_lock:
-            for index, (fut, output_pickle_path) in enumerate(futs_with_output_paths):
-                jobid_with_index = self.get_jobid_with_index(jobid, index)
-                # Thread will wait for it to finish.
-
-                outfile_name = output_pickle_path
-                self.wait_thread.waitFor(
-                    with_preliminary_postfix(outfile_name), jobid_with_index
-                )
+        for array_index, (fut, output_path) in enumerate(futs_with_output_paths):
+            jobid_with_index = self.get_jobid_with_index(jobid, array_index)
 
-                fut.cluster_jobid = jobid
-                fut.cluster_jobindex = index
+            # Thread will wait for it to finish.
+            self.wait_thread.waitFor(
+                with_preliminary_postfix(output_path), jobid_with_index
+            )
 
+            fut.cluster_jobid = jobid
+            fut.cluster_jobindex = array_index
+
+            job_index = job_index_offset + array_index
+            workerid_with_index = self.get_workerid_with_index(workerid, job_index)
+            # Remove the pending jobs entry and add the correct one
+            with self.jobs_lock:
+                del self.jobs[workerid_with_index]
                 self.jobs[jobid_with_index] = (
                     fut,
                     workerid_with_index,
-                    outfile_name,
+                    output_path,
                     should_keep_output,
                 )
 
-        return [fut for (fut, _) in futs_with_output_paths]
-
     def shutdown(self, wait=True):
         """Close the pool."""
         self.was_requested_to_shutdown = True
         if wait:
             with self.jobs_lock:
                 if self.jobs:
                     self.jobs_empty_cond.wait()
```

### Comparing `cluster_tools-1.60/cluster_tools/schedulers/pbs.py` & `cluster_tools-1.61/cluster_tools/schedulers/pbs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """Abstracts access to a PBS cluster via its command-line tools.
 """
 import re
 import os
-import threading
-import time
 from cluster_tools.util import chcall, random_string, call
 from .cluster_executor import ClusterExecutor
 import logging
 from typing import Union
+from concurrent import futures
 
 
 # qstat vs. checkjob
 PBS_STATES = {
     "Failure": [],
     "Success": [
         "C",  # Completed
@@ -48,43 +47,46 @@
         return cls.get_current_job_id()
 
     def submit_text(self, job):
         """Submits a PBS job represented as a job file string. Returns
         the job ID.
         """
 
-        filename = self.get_temp_file_path("_temp_pbs_{}.sh".format(random_string()))
+        filename = self.get_temp_file_path(
+            self.cfut_dir, "_temp_pbs_{}.sh".format(random_string())
+        )
         with open(filename, "w") as f:
             f.write(job)
         jobid_desc, _ = chcall("qsub -V {}".format(filename))
         match = re.search("^[0-9]+", jobid_desc.decode("utf-8"))
         assert match is not None
         jobid = match.group(0)
 
         print("jobid", jobid)
         # os.unlink(filename)
         return int(jobid)
 
     def inner_submit(
-        self, cmdline, job_name=None, additional_setup_lines=[], job_count=None
+        self, cmdline, job_name=None, additional_setup_lines=None, job_count=None
     ):
-        """Starts a PBS job that runs the specified shell command line.
-        """
+        """Starts a PBS job that runs the specified shell command line."""
+        if additional_setup_lines is None:
+            additional_setup_lines = []
 
         # if job_count is None else "$PBS_JOBID.$PBS_ARRAY_INDEX"
         # $PBS_JOBID will also include an array index if it's a job array
         log_path = self.format_log_file_path(self.cfut_dir, "$PBS_JOBID")
         print("log_path", log_path)
 
         job_resources_line = ""
         if self.job_resources is not None:
             specs = []
             for resource, value in self.job_resources.items():
                 if resource == "time":
-                    resource == "walltime"
+                    resource = "walltime"
                 specs.append("{}={}".format(resource, value))
             if len(specs) > 0:
                 job_resources_line = "#PBS -l {}".format(",".join(specs))
 
         job_array_line = ""
         if job_count is not None:
             if job_count == 1:
@@ -105,15 +107,19 @@
             job_resources_line,
             *additional_setup_lines,
             "export PATH=$PBS_O_PATH",
             "cd $PBS_O_WORKDIR",
             "{}".format(cmdline),
         ]
 
-        return self.submit_text("\n".join(script_lines))
+        job_id = self.submit_text("\n".join(script_lines))
+        job_id_future = futures.Future()
+        job_id_future.set_result(job_id)
+
+        return [job_id_future], [(0, job_count or 1)]
 
     def check_for_crashed_job(self, job_id) -> Union["failed", "ignore", "completed"]:
         if len(str(job_id).split("_")) >= 2:
             a, b = job_id.split("_")
             job_id = f"{a}[{b}]"
 
         # If the output file was not found, we determine the job status so that
@@ -134,15 +140,15 @@
                 job_state = job_state_search.group(1)
 
                 if job_state in PBS_STATES["Failure"]:
                     return "failed"
                 elif job_state in PBS_STATES["Ignore"]:
                     return "ignore"
                 elif job_state in PBS_STATES["Unclear"]:
-                    logging.warn(
+                    logging.warning(
                         "The job state for {} is {}. It's unclear whether the job will recover. Will wait further".format(
                             job_id, job_state
                         )
                     )
                     return "ignore"
                 elif job_state in PBS_STATES["Success"]:
                     return "completed"
```

### Comparing `cluster_tools-1.60/cluster_tools/remote.py` & `cluster_tools-1.61/cluster_tools/remote.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,20 +26,23 @@
     main_meta_path = get_executor_class().get_main_meta_path(cfut_dir, workerid)
     if os.path.exists(main_meta_path):
         with open(main_meta_path, "r") as file:
             custom_main_path = file.read()
     return custom_main_path
 
 
-def worker(workerid, job_array_index, cfut_dir):
+def worker(workerid, job_array_index, job_array_index_offset, cfut_dir):
     """Called to execute a job on a remote host."""
 
-    workerid_with_idx = (
-        worker_id + "_" + job_array_index if job_array_index is not None else workerid
-    )
+    if job_array_index is not None:
+        workerid_with_idx = (
+            worker_id + "_" + str(int(job_array_index_offset) + int(job_array_index))
+        )
+    else:
+        workerid_with_idx = worker_id
 
     executor = get_executor_class()
     try:
         input_file_name = executor.format_infile_name(cfut_dir, workerid_with_idx)
         print("trying to read: ", input_file_name)
         print("working dir: ", os.getcwd())
 
@@ -66,15 +69,15 @@
                 executor.get_current_job_id(), workerid_with_idx
             )
         )
         result = True, fun(*args, **kwargs)
         logging.info("Job computation completed.")
         out = pickling.dumps(result)
 
-    except Exception as e:
+    except Exception:
         print(traceback.format_exc())
 
         result = False, format_remote_exc()
         logging.warning("Job computation failed.")
         out = pickling.dumps(result)
 
     # The .preliminary postfix is added since the output can
@@ -122,13 +125,14 @@
         if "level" in logging_config:
             logger.setLevel(logging_config["level"])
 
 
 if __name__ == "__main__":
     worker_id = sys.argv[1]
     cfut_dir = sys.argv[2]
+    job_array_index_offset = sys.argv[3] if len(sys.argv) > 3 else "0"
     job_array_index = get_executor_class().get_job_array_index()
 
-    worker(worker_id, job_array_index, cfut_dir)
+    worker(worker_id, job_array_index, job_array_index_offset, cfut_dir)
     # This is a workaround for the case that some subprocesses are still hanging around and are waited for.
     # If this point is reached, results were written to disk and we can "safely" shut down everything.
     sys.exit()
```

### Comparing `cluster_tools-1.60/cluster_tools/util.py` & `cluster_tools-1.61/cluster_tools/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import subprocess
 import random
 import string
 import os
 import threading
 import time
 import logging
-import re
-import types
 
 
 def local_filename(filename=""):
     return os.path.join(os.getenv("CFUT_DIR", ".cfut"), filename)
 
 
 # Instantiate a dedicate generator to avoid being dependent on
@@ -41,15 +39,15 @@
     stdout, stderr = proc.communicate(stdin)
     return stdout, stderr, proc.returncode
 
 
 class CommandError(Exception):
     """Raised when a shell command exits abnormally."""
 
-    def __init__(self, command, code, stderr):
+    def __init__(self, command, code, stderr):  # pylint: disable=super-init-not-called
         self.command = command
         self.code = code
         self.stderr = stderr
 
     def __str__(self):
         return "%s exited with status %i: %s" % (
             repr(self.command),
@@ -75,29 +73,29 @@
 
     def outer(fn):
         def inner(*args, **kwargs):
             exceeded_timeout = [False]
             start_time = time.time()
 
             def warn_function():
-                logging.warn(
+                logging.warning(
                     "Function {} is taking suspiciously long (longer than {} seconds)".format(
                         job, seconds
                     )
                 )
                 exceeded_timeout[0] = True
 
             timer = threading.Timer(seconds, warn_function)
             timer.start()
 
             try:
                 result = fn(*args, **kwargs)
                 if exceeded_timeout[0]:
                     end_time = time.time()
-                    logging.warn(
+                    logging.warning(
                         "Function {} succeeded after all (took {} seconds)".format(
                             job, int(end_time - start_time)
                         )
                     )
             finally:
                 timer.cancel()
             return result
```

### Comparing `cluster_tools-1.60/cluster_tools/multiprocessing_logging_handler.py` & `cluster_tools-1.61/cluster_tools/multiprocessing_logging_handler.py`

 * *Files identical despite different names*

### Comparing `cluster_tools-1.60/.circleci/config.yml` & `cluster_tools-1.61/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `cluster_tools-1.60/.pylintrc` & `cluster_tools-1.61/.pylintrc`

 * *Files 3% similar despite different names*

```diff
@@ -50,26 +50,26 @@
 # all. Valid levels: HIGH, INFERENCE, INFERENCE_FAILURE, UNDEFINED
 confidence=
 
 # Enable the message, report, category or checker with the given id(s). You can
 # either give multiple identifier separated by comma (,) or put this option
 # multiple time (only on the command line, not in the configuration file where
 # it should appear only once). See also the "--disable" option for examples.
-#enable=
+enable=useless-suppression
 
 # Disable the message, report, category or checker with the given id(s). You
 # can either give multiple identifiers separated by comma (,) or put this
 # option multiple times (only on the command line, not in the configuration
 # file where it should appear only once).You can also use "--disable=all" to
 # disable everything first and then reenable specific checks. For example, if
 # you want to run only the similarities checker, you can use "--disable=all
 # --enable=similarities". If you want to run only the classes checker, but have
 # no Warning level messages displayed, use"--disable=all --enable=classes
 # --disable=W"
-disable=import-star-module-level,old-octal-literal,oct-method,print-statement,unpacking-in-except,parameter-unpacking,backtick,old-raise-syntax,old-ne-operator,long-suffix,dict-view-method,dict-iter-method,metaclass-assignment,next-method-called,raising-string,indexing-exception,raw_input-builtin,long-builtin,file-builtin,execfile-builtin,coerce-builtin,cmp-builtin,buffer-builtin,basestring-builtin,apply-builtin,filter-builtin-not-iterating,using-cmp-argument,useless-suppression,range-builtin-not-iterating,suppressed-message,no-absolute-import,old-division,cmp-method,reload-builtin,zip-builtin-not-iterating,intern-builtin,unichr-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,input-builtin,round-builtin,hex-method,nonzero-method,map-builtin-not-iterating,R,C,W
+disable=unspecified-encoding,import-star-module-level,old-octal-literal,oct-method,print-statement,unpacking-in-except,parameter-unpacking,backtick,old-raise-syntax,old-ne-operator,long-suffix,dict-view-method,dict-iter-method,metaclass-assignment,next-method-called,raising-string,indexing-exception,raw_input-builtin,long-builtin,file-builtin,execfile-builtin,coerce-builtin,cmp-builtin,buffer-builtin,basestring-builtin,apply-builtin,filter-builtin-not-iterating,using-cmp-argument,range-builtin-not-iterating,suppressed-message,no-absolute-import,old-division,cmp-method,reload-builtin,zip-builtin-not-iterating,intern-builtin,unichr-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,input-builtin,round-builtin,hex-method,nonzero-method,map-builtin-not-iterating,bad-indentation,logging-format-interpolation,redefined-outer-name,protected-access,broad-except,duplicate-string-formatting-argument,unnecessary-pass,arguments-differ,logging-fstring-interpolation,fixme,global-statement,R,C,logging-not-lazy,f-string-without-interpolation
 
 
 [REPORTS]
 
 # Set the output format. Available formats are text, parseable, colorized, msvs
 # (visual studio) and html. You can also give a reporter class, eg
 # mypackage.mymodule.MyReporterClass.
@@ -78,15 +78,15 @@
 # Put messages in a separate file for each module / package specified on the
 # command line instead of printing them on stdout. Reports (if any) will be
 # written in a file name "pylint_global.[txt|html]". This option is deprecated
 # and it will be removed in Pylint 2.0.
 files-output=no
 
 # Tells whether to display a full report or only the messages
-reports=yes
+reports=no
 
 # Python expression which should return a note less than 10 (10 is the highest
 # note). You have access to the variables errors warning, statement which
 # respectively contain the number of errors / warnings messages and the total
 # number of statements analyzed. This is used by the global evaluation report
 # (RP0004).
 evaluation=10.0 - ((float(5 * error + warning + refactor + convention) / statement) * 10)
```

