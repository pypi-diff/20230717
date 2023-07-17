# Comparing `tmp/dassana-0.8.8.tar.gz` & `tmp/dassana-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dassana-0.8.8.tar", last modified: Tue Jun 27 04:20:34 2023, max compression
+gzip compressed data, was "dassana-0.8.9.tar", last modified: Sat Jul  8 09:42:14 2023, max compression
```

## Comparing `dassana-0.8.8.tar` & `dassana-0.8.9.tar`

### file list

```diff
@@ -1,18 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 04:20:34.030220 dassana-0.8.8/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-27 04:20:34.030220 dassana-0.8.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-27 04:20:21.000000 dassana-0.8.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 04:20:34.030220 dassana-0.8.8/dassana/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-27 04:20:21.000000 dassana-0.8.8/dassana/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8553 2023-06-27 04:20:21.000000 dassana-0.8.8/dassana/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-06-27 04:20:21.000000 dassana-0.8.8/dassana/dassana_env.py
--rw-r--r--   0 runner    (1001) docker     (123)    16334 2023-06-27 04:20:21.000000 dassana-0.8.8/dassana/data_pipes.py
--rw-r--r--   0 runner    (1001) docker     (123)    14437 2023-06-27 04:20:21.000000 dassana-0.8.8/dassana/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 04:20:34.030220 dassana-0.8.8/dassana.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-27 04:20:33.000000 dassana-0.8.8/dassana.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-27 04:20:34.000000 dassana-0.8.8/dassana.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 04:20:33.000000 dassana-0.8.8/dassana.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 04:20:33.000000 dassana-0.8.8/dassana.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-27 04:20:33.000000 dassana-0.8.8/dassana.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-27 04:20:33.000000 dassana-0.8.8/dassana.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 04:20:34.030220 dassana-0.8.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-27 04:20:21.000000 dassana-0.8.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 09:42:14.062353 dassana-0.8.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-08 09:42:14.062353 dassana-0.8.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-08 09:42:02.000000 dassana-0.8.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 09:42:14.058354 dassana-0.8.9/dassana/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 09:42:02.000000 dassana-0.8.9/dassana/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10036 2023-07-08 09:42:02.000000 dassana-0.8.9/dassana/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-08 09:42:02.000000 dassana-0.8.9/dassana/dassana_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 09:42:14.062353 dassana-0.8.9/dassana.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-08 09:42:14.000000 dassana-0.8.9/dassana.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-08 09:42:14.000000 dassana-0.8.9/dassana.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 09:42:14.000000 dassana-0.8.9/dassana.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 09:42:14.000000 dassana-0.8.9/dassana.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-08 09:42:14.000000 dassana-0.8.9/dassana.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-08 09:42:14.000000 dassana-0.8.9/dassana.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 09:42:14.062353 dassana-0.8.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-08 09:42:02.000000 dassana-0.8.9/setup.py
```

### Comparing `dassana-0.8.8/dassana/common.py` & `dassana-0.8.9/dassana/common.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,90 +2,139 @@
 import time
 from google.cloud import storage
 import boto3
 import os
 import gzip
 import requests
 import logging
-from kubernetes import client, config
-import base64
+from .dassana_env import *
+import datetime
 
-auth_url = os.environ.get("DASSANA_JWT_ISSUER")
-app_url = os.environ.get("DASSANA_APP_SERVICE_HOST")
-tenant_id = os.environ.get("DASSANA_TENANT_ID")
-debug = int(os.environ.get("DASSANA_DEBUG", 0))
-app_id = os.environ.get("DASSANA_APP_ID")
-ingestion_service_url = os.environ.get("DASSANA_INGESTION_SERVICE_URL")
-
-def get_client_secret():
-    if os.getenv("KUBERNETES_SERVICE_HOST"):
-        config.load_incluster_config()
+logging.basicConfig(level=logging.INFO)
+
+auth_url = get_auth_url()
+app_url = get_app_url()
+debug = get_if_debug()
+ingestion_service_url = get_ingestion_srv_url()
+client_id = get_client_id()
+client_secret = get_client_secret()
+
+class AuthenticationError(Exception):
+    """Exception Raised when credentials in configuration are invalid"""
+
+    def __init__(self, message):
+        super().__init__()
+        self.message = message
+
+    def __str__(self):
+        return f"Source authentication failure: {self.message}"
+
+
+class InternalError(Exception):
+    """Exception Raised for AppServices, Ingestion, or Upstream
+    Attributes:
+        source -- error origin
+        message -- upstream response
+    """
+
+    def __init__(self, source, message=""):
+        self.source = source
+        self.message = message
+        super().__init__(self.message)
+
+    def __str__(self):
+        return json.dumps({"source": self.source, "message": self.message})
+
+def datetime_handler(val):
+    if isinstance(val, datetime.datetime):
+        return val.isoformat()
+    return str(val)
+
+def get_ingestion_config(ingestion_config_id, app_id, tenant_id):
+    url = f"https://{app_url}/app/{app_id}/ingestionConfig/{ingestion_config_id}"
+    access_token = get_access_token()
+    headers = {
+        "x-dassana-tenant-id": tenant_id,
+        "Authorization": f"Bearer {access_token}", 
+    }
+    if app_url.endswith("svc.cluster.local:443"):
+        response = requests.request("GET", url, headers=headers, verify=False)
+    else:
+        response = requests.request("GET", url, headers=headers)
+    try:
+        ingestion_config = response.json() 
+    except:
+        raise InternalError(url, response.json())
+    return ingestion_config
+
+def patch_ingestion_config(payload, ingestion_config_id, app_id, tenant_id):
+    url = f"https://{app_url}/app/{app_id}/ingestionConfig/{ingestion_config_id}"
+    access_token = get_access_token()
+    headers = {
+        "x-dassana-tenant-id": tenant_id,
+        "Authorization": f"Bearer {access_token}",
+    }
+    if app_url.endswith("svc.cluster.local:443"):
+        response = requests.request("PATCH", url, headers=headers, json=payload, verify=False)
     else:
-        config.load_kube_config()
-        if debug:
-            return os.getenv("DASSANA_SERVICE_CLIENT_SECRET")
-    v1 = client.CoreV1Api()
-    secret_res = v1.read_namespaced_secret("ingestion-srv-secrets", "ingestion-srv")
-    secret_b64 = secret_res.data["dassana.auth.client-secret"]
-    secret = base64.b64decode(secret_b64)
-    return secret
+        response = requests.request("PATCH", url, headers=headers, json=payload)
+    resp=response.json()
+    return resp
 
 def get_access_token():
     url = f"{auth_url}/oauth/token"
     if auth_url.endswith("svc.cluster.local"):
         response = requests.post(
             url,
             data={
                 "grant_type": "client_credentials",
-                "client_id": "ingestion-srv",
-                "client_secret": get_client_secret(),
+                "client_id": client_id,
+                "client_secret": client_secret,
             },
             verify=False
         )  
     else:
         response = requests.post(
             url,
             data={
                 "grant_type": "client_credentials",
-                "client_id": "ingestion-srv",
-                "client_secret": get_client_secret(),
+                "client_id": client_id,
+                "client_secret": client_secret,
             }
         )
-    # try:
-    access_token = response.json()["access_token"]
-    # except:
-    #     raise InternalError(url, response.json())
+    try:
+        access_token = response.json()["access_token"]
+    except:
+        raise InternalError(url, response.json())
     return access_token
 
 def update_ingestion_to_done(job_id, tenant_id, metadata = {}):
     
     access_token = get_access_token()
     headers = {
         "x-dassana-tenant-id": tenant_id,
         "Authorization": f"Bearer {access_token}", 
     }
     res = requests.post(ingestion_service_url +"/job/"+job_id+"/"+"done", headers=headers, json={
         "metadata": metadata
     })
     print("Ingestion status updated to done")
-    # print(res.json())
     return res.json()
 
 def cancel_ingestion_job(job_id, tenant_id, metadata = {}):
     
     access_token = get_access_token()
     headers = {
         "x-dassana-tenant-id": tenant_id,
         "Authorization": f"Bearer {access_token}", 
     }
     res = requests.post(ingestion_service_url +"/job/"+job_id+"/"+"failed", headers=headers, json={
         "metadata": metadata
     })
     print("Ingestion status updated to failed")
-    # print(res.json())
     return res.json()
 
 def get_ingestion_details(tenant_id, source, record_type, config_id, metadata, priority, is_snapshot):
     access_token = get_access_token()
 
     headers = {
         "x-dassana-tenant-id": tenant_id,
@@ -105,15 +154,15 @@
     
     res = requests.post(ingestion_service_url +"/job/", headers=headers, json=json_body)
     if(res.status_code == 200):
         return res.json()
 
     return 0
 
-def report_status(status, additionalContext, timeTakenInSec, recordsIngested, ingestion_config_id):
+def report_status(status, additionalContext, timeTakenInSec, recordsIngested, ingestion_config_id, app_id, tenant_id):
     reportingURL = f"https://{app_url}/app/v1/{app_id}/status"
 
     headers = {
         "x-dassana-tenant-id": tenant_id,
         "Authorization": f"Bearer {get_access_token()}",
     }
 
@@ -198,15 +247,15 @@
         self.bytes_written = self.file.tell()
         if self.bytes_written >= 99 * 1000 * 1000:
             self.file.close()
             self.compress_file()
             self.upload_to_cloud()
             self.file_path = self.get_file_path()
             self.file = open(self.file_path, 'a')
-            print("Ingested data: " + self.bytes_written)
+            print(f"Ingested data: {self.bytes_written} bytes")
             self.bytes_written = 0
             
 
     def upload_to_cloud(self):
         if self.client is None:
             raise ValueError("Client not initialized.")
 
@@ -236,12 +285,13 @@
             os.remove("service_account.json")
 
     def close(self):
         self.file.close()
         if self.bytes_written > 0:
             self.compress_file()
             self.upload_to_cloud()
-            print("Ingested remaining data: ", self.bytes_written)
+            print(f"Ingested remaining data: {self.bytes_written} bytes")
             self.bytes_written = 0
         update_ingestion_to_done(self.job_id, self.tenant_id)
         if os.path.exists("service_account.json"):
             os.remove("service_account.json")
+
```

