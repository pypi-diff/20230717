# Comparing `tmp/banking_logging-0.2.2.tar.gz` & `tmp/banking_logging-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "banking_logging-0.2.2.tar", last modified: Sun Jul 16 23:50:39 2023, max compression
+gzip compressed data, was "banking_logging-0.2.3.tar", last modified: Mon Jul 17 00:00:40 2023, max compression
```

## Comparing `banking_logging-0.2.2.tar` & `banking_logging-0.2.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 23:50:39.312856 banking_logging-0.2.2/
--rw-rw-rw-   0        0        0      253 2023-07-16 23:50:39.311047 banking_logging-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      985 2023-05-27 16:57:34.000000 banking_logging-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-16 23:50:39.293942 banking_logging-0.2.2/banking_logging/
--rw-rw-rw-   0        0        0       32 2023-05-27 16:48:39.000000 banking_logging-0.2.2/banking_logging/__init__.py
--rw-rw-rw-   0        0        0     7810 2023-07-16 23:50:11.000000 banking_logging-0.2.2/banking_logging/banking_logging.py
-drwxrwxrwx   0        0        0        0 2023-07-16 23:50:39.310051 banking_logging-0.2.2/banking_logging.egg-info/
--rw-rw-rw-   0        0        0      253 2023-07-16 23:50:39.000000 banking_logging-0.2.2/banking_logging.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-07-16 23:50:39.000000 banking_logging-0.2.2/banking_logging.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 23:50:39.000000 banking_logging-0.2.2/banking_logging.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-16 23:50:39.000000 banking_logging-0.2.2/banking_logging.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-16 23:50:39.312940 banking_logging-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      628 2023-07-16 23:50:21.000000 banking_logging-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 00:00:40.499889 banking_logging-0.2.3/
+-rw-rw-rw-   0        0        0      253 2023-07-17 00:00:40.499889 banking_logging-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0      985 2023-05-27 16:57:34.000000 banking_logging-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 00:00:40.481152 banking_logging-0.2.3/banking_logging/
+-rw-rw-rw-   0        0        0       32 2023-05-27 16:48:39.000000 banking_logging-0.2.3/banking_logging/__init__.py
+-rw-rw-rw-   0        0        0     7631 2023-07-16 23:59:42.000000 banking_logging-0.2.3/banking_logging/banking_logging.py
+drwxrwxrwx   0        0        0        0 2023-07-17 00:00:40.497892 banking_logging-0.2.3/banking_logging.egg-info/
+-rw-rw-rw-   0        0        0      253 2023-07-17 00:00:40.000000 banking_logging-0.2.3/banking_logging.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-07-17 00:00:40.000000 banking_logging-0.2.3/banking_logging.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 00:00:40.000000 banking_logging-0.2.3/banking_logging.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-17 00:00:40.000000 banking_logging-0.2.3/banking_logging.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 00:00:40.500892 banking_logging-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      628 2023-07-17 00:00:28.000000 banking_logging-0.2.3/setup.py
```

### Comparing `banking_logging-0.2.2/README.md` & `banking_logging-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `banking_logging-0.2.2/banking_logging/banking_logging.py` & `banking_logging-0.2.3/banking_logging/banking_logging.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,25 +19,18 @@
 
 #
 class LocalTimer:
     def __init__(self, conn_log, log_table):
         self.conn_log = conn_log
         self.log_table = log_table
 
-    def new_call(self):
-        query = """
-        SELECT max(call_id)
-        FROM {0}
-        ;
-        """.format(self.log_table)
-        result = pandas.read_sql(sql=text(query), con=self.conn_log).values[0][0]
-        if result is None:
-            return 0
-        else:
-            return result + 1
+    @staticmethod
+    def new_call(group):
+        code = str(uuid.uuid5(namespace=uuid.NAMESPACE_OID, name=group))
+        return code
 
     def log_start(self, call_id_reporter, group, method):
         query = table('timings_reported',
                       column('service_name'),
                       column('internal'),
                       column('call_id_reporter'), column('group'), column('method'),
                       column('status'), column('timestamp')).insert() \
```

### Comparing `banking_logging-0.2.2/setup.py` & `banking_logging-0.2.3/setup.py`

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
-            'version': '0.2.2',
+            'version': '0.2.3',
             'long_description': '',
             'python_requires': '>=3.10',
             'install_requires': []}
 
 setup(**metadata)
```

