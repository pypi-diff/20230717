# Comparing `tmp/salure_helpers_elastic-0.0.1.tar.gz` & `tmp/salure_helpers_elastic-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/salure_helpers_elastic-0.0.1.tar", last modified: Tue May  9 11:20:42 2023, max compression
+gzip compressed data, was "dist/salure_helpers_elastic-0.0.2.tar", last modified: Mon Jul 17 11:21:59 2023, max compression
```

## Comparing `salure_helpers_elastic-0.0.1.tar` & `salure_helpers_elastic-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 11:20:42.000000 salure_helpers_elastic-0.0.1/
--rw-r--r--   0 root         (0) root         (0)      265 2023-05-09 11:20:42.000000 salure_helpers_elastic-0.0.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 11:20:42.000000 salure_helpers_elastic-0.0.1/salure_helpers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 11:20:42.000000 salure_helpers_elastic-0.0.1/salure_helpers/elastic/
--rw-rw-rw-   0 root         (0) root         (0)       50 2023-05-09 11:20:27.000000 salure_helpers_elastic-0.0.1/salure_helpers/elastic/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15486 2023-05-09 11:20:27.000000 salure_helpers_elastic-0.0.1/salure_helpers/elastic/elastic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 11:20:42.000000 salure_helpers_elastic-0.0.1/salure_helpers_elastic.egg-info/
--rw-r--r--   0 root         (0) root         (0)      265 2023-05-09 11:20:42.000000 salure_helpers_elastic-0.0.1/salure_helpers_elastic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      351 2023-05-09 11:20:42.000000 salure_helpers_elastic-0.0.1/salure_helpers_elastic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 11:20:42.000000 salure_helpers_elastic-0.0.1/salure_helpers_elastic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 11:20:42.000000 salure_helpers_elastic-0.0.1/salure_helpers_elastic.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       64 2023-05-09 11:20:42.000000 salure_helpers_elastic-0.0.1/salure_helpers_elastic.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-05-09 11:20:42.000000 salure_helpers_elastic-0.0.1/salure_helpers_elastic.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-09 11:20:42.000000 salure_helpers_elastic-0.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      484 2023-05-09 11:20:27.000000 salure_helpers_elastic-0.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 11:21:59.000000 salure_helpers_elastic-0.0.2/
+-rw-r--r--   0 root         (0) root         (0)      265 2023-07-17 11:21:59.000000 salure_helpers_elastic-0.0.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 11:21:59.000000 salure_helpers_elastic-0.0.2/salure_helpers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 11:21:59.000000 salure_helpers_elastic-0.0.2/salure_helpers/elastic/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-07-17 11:21:47.000000 salure_helpers_elastic-0.0.2/salure_helpers/elastic/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15999 2023-07-17 11:21:47.000000 salure_helpers_elastic-0.0.2/salure_helpers/elastic/elastic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 11:21:59.000000 salure_helpers_elastic-0.0.2/salure_helpers_elastic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      265 2023-07-17 11:21:59.000000 salure_helpers_elastic-0.0.2/salure_helpers_elastic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      351 2023-07-17 11:21:59.000000 salure_helpers_elastic-0.0.2/salure_helpers_elastic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 11:21:59.000000 salure_helpers_elastic-0.0.2/salure_helpers_elastic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 11:21:59.000000 salure_helpers_elastic-0.0.2/salure_helpers_elastic.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       64 2023-07-17 11:21:59.000000 salure_helpers_elastic-0.0.2/salure_helpers_elastic.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-17 11:21:59.000000 salure_helpers_elastic-0.0.2/salure_helpers_elastic.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-17 11:21:59.000000 salure_helpers_elastic-0.0.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      484 2023-07-17 11:21:47.000000 salure_helpers_elastic-0.0.2/setup.py
```

### Comparing `salure_helpers_elastic-0.0.1/salure_helpers/elastic/elastic.py` & `salure_helpers_elastic-0.0.2/salure_helpers/elastic/elastic.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,18 +11,24 @@
     def __init__(self, api_key: str = None):
         """
         A package to create indexes, users, roles, getting data, etc.
         :param api_key: The api key to connect to elasticsearch if not provided in the .env file
         """
         try:
             self.verify = False
-            self.elasticsearch_host = f'https://{os.getenv("ELASTIC_HOST", "localhost")}:{os.getenv("ELASTIC_PORT", "9200")}'
-            self.kibana_host = f'http://{os.getenv("ELASTIC_HOST", "localhost")}:{os.getenv("KIBANA_PORT", "5601")}'
-            self.elastic_token = os.getenv('ELASTIC_API_KEY', api_key)
-            self.client_user = os.getenv('SALURECONNECT_CUSTOMER_NAME', 'default')
+            if os.getenv('SALURECONNECT_ENVIRONMENT') == 'prod':
+                self.elasticsearch_host = f'https://{os.getenv("ELASTIC_HOST_LIVE", "localhost")}:{os.getenv("ELASTIC_PORT_LIVE", "9200")}'
+                self.kibana_host = f'http://{os.getenv("ELASTIC_HOST_LIVE", "localhost")}:{os.getenv("KIBANA_PORT_LIVE", "5601")}'
+                self.elastic_token = os.getenv('ELASTIC_API_KEY_LIVE', api_key)
+            else:
+                self.elasticsearch_host = f'https://{os.getenv("ELASTIC_HOST_STAGING", "localhost")}:{os.getenv("ELASTIC_PORT_STAGING", "9200")}'
+                self.kibana_host = f'http://{os.getenv("ELASTIC_HOST_STAGING", "localhost")}:{os.getenv("KIBANA_PORT_STAGING", "5601")}'
+                self.elastic_token = os.getenv('ELASTIC_API_KEY_STAGING', api_key)
+
+            self.client_user = os.getenv('SALURECONNECT_CUSTOMER_NAME', 'default').lower().replace(' ', '_')
             self.space_name = os.getenv('ELASTIC_SPACE', 'default')
             self.timestamp = int(datetime.datetime.now().timestamp())
             self.elastic_headers = {
                 'Content-Type': 'application/json',
                 'Authorization': f'ApiKey {self.elastic_token}'
             }
             self.kibana_headers = {
```

