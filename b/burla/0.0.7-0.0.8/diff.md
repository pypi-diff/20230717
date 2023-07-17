# Comparing `tmp/burla-0.0.7.tar.gz` & `tmp/burla-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "burla-0.0.7.tar", max compression
+gzip compressed data, was "burla-0.0.8.tar", max compression
```

## Comparing `burla-0.0.7.tar` & `burla-0.0.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      503 2023-07-17 15:45:57.027703 burla-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      175 2023-07-13 18:25:13.491110 burla-0.0.7/src/burla/__init__.py
--rw-r--r--   0        0        0     1352 2023-07-12 19:34:52.816658 burla-0.0.7/src/burla/_logstream.py
--rw-r--r--   0        0        0      907 2023-07-13 18:24:57.649392 burla-0.0.7/src/burla/config.py
--rw-r--r--   0        0        0     4064 2023-07-17 15:56:22.078209 burla-0.0.7/src/burla/remote_parallel_map.py
--rw-r--r--   0        0        0      616 1970-01-01 00:00:00.000000 burla-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      503 2023-07-17 19:06:21.951421 burla-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      175 2023-07-13 18:25:13.491110 burla-0.0.8/src/burla/__init__.py
+-rw-r--r--   0        0        0     1352 2023-07-12 19:34:52.816658 burla-0.0.8/src/burla/_logstream.py
+-rw-r--r--   0        0        0      907 2023-07-13 18:24:57.649392 burla-0.0.8/src/burla/config.py
+-rw-r--r--   0        0        0     4148 2023-07-17 19:06:03.804535 burla-0.0.8/src/burla/remote_parallel_map.py
+-rw-r--r--   0        0        0      616 1970-01-01 00:00:00.000000 burla-0.0.8/PKG-INFO
```

### Comparing `burla-0.0.7/src/burla/_logstream.py` & `burla-0.0.8/src/burla/_logstream.py`

 * *Files identical despite different names*

### Comparing `burla-0.0.7/src/burla/config.py` & `burla-0.0.8/src/burla/config.py`

 * *Files identical despite different names*

### Comparing `burla-0.0.7/src/burla/remote_parallel_map.py` & `burla-0.0.8/src/burla/remote_parallel_map.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,19 +12,20 @@
 from tblib import pickling_support
 
 from burla._logstream import print_logs_from_queue
 from burla.config import load_api_key_from_local_config
 
 pickling_support.install()
 
-BURLA_SERVICE_URL = "https://burla-webservice-gxc7eo4ala-uc.a.run.app"
-JOB_ENV_REPO = "us-east4-docker.pkg.dev/burla-389321/burla-job-environments"
-
+BURLA_SERVICE_URL = "https://burla-webservice-production-gxc7eo4ala-uc.a.run.app"
+# BURLA_SERVICE_URL = "https://burla-webservice-gxc7eo4ala-uc.a.run.app"
 # BURLA_SERVICE_URL = "https://127.0.0.1:5000"
 
+JOB_ENV_REPO = "us-east4-docker.pkg.dev/burla-389321/burla-job-environments"
+
 JOB_STATUS_POLL_RATE_SEC = 6  # how often to check for job completion
 TIMEOUT_MIN = 60 * 12  # max time a Burla job can run for
 
 
 class JobTimeoutError(Exception):
     def __init__(self, job_id, timeout):
         super().__init__(f"Burla job with id: '{job_id}' timed out after {timeout} seconds.")
```

### Comparing `burla-0.0.7/PKG-INFO` & `burla-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: burla
-Version: 0.0.7
+Version: 0.0.8
 Summary: Make your python script 100x faster
 Author: Jake Zuliani
 Author-email: jake@burla.dev
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

