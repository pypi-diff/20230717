# Comparing `tmp/banking_logging-0.2.1.tar.gz` & `tmp/banking_logging-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "banking_logging-0.2.1.tar", last modified: Sun Jul 16 23:44:42 2023, max compression
+gzip compressed data, was "banking_logging-0.2.2.tar", last modified: Sun Jul 16 23:50:39 2023, max compression
```

## Comparing `banking_logging-0.2.1.tar` & `banking_logging-0.2.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 23:44:42.879435 banking_logging-0.2.1/
--rw-rw-rw-   0        0        0      253 2023-07-16 23:44:42.878433 banking_logging-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      985 2023-05-27 16:57:34.000000 banking_logging-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-16 23:44:42.847210 banking_logging-0.2.1/banking_logging/
--rw-rw-rw-   0        0        0       32 2023-05-27 16:48:39.000000 banking_logging-0.2.1/banking_logging/__init__.py
--rw-rw-rw-   0        0        0     7805 2023-07-16 23:35:46.000000 banking_logging-0.2.1/banking_logging/banking_logging.py
-drwxrwxrwx   0        0        0        0 2023-07-16 23:44:42.876434 banking_logging-0.2.1/banking_logging.egg-info/
--rw-rw-rw-   0        0        0      253 2023-07-16 23:44:42.000000 banking_logging-0.2.1/banking_logging.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-07-16 23:44:42.000000 banking_logging-0.2.1/banking_logging.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 23:44:42.000000 banking_logging-0.2.1/banking_logging.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-16 23:44:42.000000 banking_logging-0.2.1/banking_logging.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-16 23:44:42.879435 banking_logging-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      628 2023-07-16 23:44:21.000000 banking_logging-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 23:50:39.312856 banking_logging-0.2.2/
+-rw-rw-rw-   0        0        0      253 2023-07-16 23:50:39.311047 banking_logging-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      985 2023-05-27 16:57:34.000000 banking_logging-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 23:50:39.293942 banking_logging-0.2.2/banking_logging/
+-rw-rw-rw-   0        0        0       32 2023-05-27 16:48:39.000000 banking_logging-0.2.2/banking_logging/__init__.py
+-rw-rw-rw-   0        0        0     7810 2023-07-16 23:50:11.000000 banking_logging-0.2.2/banking_logging/banking_logging.py
+drwxrwxrwx   0        0        0        0 2023-07-16 23:50:39.310051 banking_logging-0.2.2/banking_logging.egg-info/
+-rw-rw-rw-   0        0        0      253 2023-07-16 23:50:39.000000 banking_logging-0.2.2/banking_logging.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-07-16 23:50:39.000000 banking_logging-0.2.2/banking_logging.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 23:50:39.000000 banking_logging-0.2.2/banking_logging.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-16 23:50:39.000000 banking_logging-0.2.2/banking_logging.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-16 23:50:39.312940 banking_logging-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      628 2023-07-16 23:50:21.000000 banking_logging-0.2.2/setup.py
```

### Comparing `banking_logging-0.2.1/README.md` & `banking_logging-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `banking_logging-0.2.1/banking_logging/banking_logging.py` & `banking_logging-0.2.2/banking_logging/banking_logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
     def __init__(self, service_name, service_pw, api):
         self.service_name = service_name
         self.service_pw = service_pw
         self.api = api
 
     @staticmethod
     def new_call(group):
-        code = uuid.uuid5(namespace=uuid.NAMESPACE_OID, name=group)
+        code = str(uuid.uuid5(namespace=uuid.NAMESPACE_OID, name=group))
         return code
 
     def log_start(self, call_id_reporter, group, method_used):
         http = urllib3.PoolManager()
         method = "timer_send_timing"
 
         query = {
```

### Comparing `banking_logging-0.2.1/setup.py` & `banking_logging-0.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,13 +8,13 @@
             'maintainer_email': 'edazizovv@gmail.com',
             'description': 'Shared loggers for banking_api project',
             'license': 'Proprietary',
             'url': '',
             'download_url': '',
             'packages': setuptools.find_packages(),
             'include_package_data': True,
-            'version': '0.2.1',
+            'version': '0.2.2',
             'long_description': '',
             'python_requires': '>=3.10',
             'install_requires': []}
 
 setup(**metadata)
```

