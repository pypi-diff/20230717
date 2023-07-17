# Comparing `tmp/dms-influx2-0.3.3.tar.gz` & `tmp/dms-influx2-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\dms-influx2-0.3.3.tar", last modified: Fri Jul 14 12:57:15 2023, max compression
+gzip compressed data, was "dist\dms-influx2-0.3.4.tar", last modified: Mon Jul 17 06:12:24 2023, max compression
```

## Comparing `dms-influx2-0.3.3.tar` & `dms-influx2-0.3.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 12:57:15.619992 dms-influx2-0.3.3/
--rw-rw-rw-   0        0        0      556 2023-07-14 12:57:15.618992 dms-influx2-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0      190 2023-01-09 21:18:36.000000 dms-influx2-0.3.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 12:57:15.613953 dms-influx2-0.3.3/dms_influx2/
--rw-rw-rw-   0        0        0        0 2023-01-09 21:18:36.000000 dms-influx2-0.3.3/dms_influx2/__init__.py
--rw-rw-rw-   0        0        0     5108 2023-01-09 21:18:36.000000 dms-influx2-0.3.3/dms_influx2/authorizations.py
--rw-rw-rw-   0        0        0     6376 2023-03-22 11:19:56.000000 dms-influx2-0.3.3/dms_influx2/buckets.py
--rw-rw-rw-   0        0        0     5591 2023-01-19 07:18:35.000000 dms-influx2-0.3.3/dms_influx2/checks.py
--rw-rw-rw-   0        0        0      630 2023-01-09 21:18:36.000000 dms-influx2-0.3.3/dms_influx2/decorators.py
--rw-rw-rw-   0        0        0     2729 2023-07-03 09:35:10.000000 dms-influx2-0.3.3/dms_influx2/delete.py
--rw-rw-rw-   0        0        0     1487 2023-01-19 06:30:10.000000 dms-influx2-0.3.3/dms_influx2/dtv_files.py
--rw-rw-rw-   0        0        0      327 2023-01-09 21:18:36.000000 dms-influx2-0.3.3/dms_influx2/exceptions.py
--rw-rw-rw-   0        0        0    25256 2023-07-14 12:55:32.000000 dms-influx2-0.3.3/dms_influx2/lib.py
--rw-rw-rw-   0        0        0     3562 2023-01-09 21:18:36.000000 dms-influx2-0.3.3/dms_influx2/notifications.py
--rw-rw-rw-   0        0        0     1012 2023-01-09 21:18:36.000000 dms-influx2-0.3.3/dms_influx2/organisations.py
--rw-rw-rw-   0        0        0     7217 2023-07-04 18:39:09.000000 dms-influx2-0.3.3/dms_influx2/query.py
--rw-rw-rw-   0        0        0        0 2023-01-18 17:42:37.000000 dms-influx2-0.3.3/dms_influx2/sync.py
--rw-rw-rw-   0        0        0     4025 2023-01-09 21:18:36.000000 dms-influx2-0.3.3/dms_influx2/tasks.py
--rw-rw-rw-   0        0        0     1203 2023-01-26 19:35:58.000000 dms-influx2-0.3.3/dms_influx2/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-14 12:57:15.616993 dms-influx2-0.3.3/dms_influx2.egg-info/
--rw-rw-rw-   0        0        0      556 2023-07-14 12:57:15.000000 dms-influx2-0.3.3/dms_influx2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      636 2023-07-14 12:57:15.000000 dms-influx2-0.3.3/dms_influx2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 12:57:15.000000 dms-influx2-0.3.3/dms_influx2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       89 2023-07-14 12:57:15.000000 dms-influx2-0.3.3/dms_influx2.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-14 12:57:15.000000 dms-influx2-0.3.3/dms_influx2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 12:57:15.619992 dms-influx2-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0     3023 2023-07-14 12:56:51.000000 dms-influx2-0.3.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-14 12:57:15.618992 dms-influx2-0.3.3/tests/
--rw-rw-rw-   0        0        0     1882 2023-07-03 09:02:50.000000 dms-influx2-0.3.3/tests/test_auth.py
--rw-rw-rw-   0        0        0     4632 2023-07-03 09:02:50.000000 dms-influx2-0.3.3/tests/test_buckets.py
--rw-rw-rw-   0        0        0     2018 2023-07-03 09:11:49.000000 dms-influx2-0.3.3/tests/test_copy-values.py
--rw-rw-rw-   0        0        0    16796 2023-07-14 12:09:20.000000 dms-influx2-0.3.3/tests/test_data.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:12:24.439363 dms-influx2-0.3.4/
+-rw-rw-rw-   0        0        0      556 2023-07-17 06:12:24.438365 dms-influx2-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2023-01-09 21:18:36.000000 dms-influx2-0.3.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 06:12:24.433359 dms-influx2-0.3.4/dms_influx2/
+-rw-rw-rw-   0        0        0        0 2023-01-09 21:18:36.000000 dms-influx2-0.3.4/dms_influx2/__init__.py
+-rw-rw-rw-   0        0        0     5108 2023-01-09 21:18:36.000000 dms-influx2-0.3.4/dms_influx2/authorizations.py
+-rw-rw-rw-   0        0        0     6376 2023-03-22 11:19:56.000000 dms-influx2-0.3.4/dms_influx2/buckets.py
+-rw-rw-rw-   0        0        0     5591 2023-01-19 07:18:35.000000 dms-influx2-0.3.4/dms_influx2/checks.py
+-rw-rw-rw-   0        0        0      630 2023-01-09 21:18:36.000000 dms-influx2-0.3.4/dms_influx2/decorators.py
+-rw-rw-rw-   0        0        0     2729 2023-07-03 09:35:10.000000 dms-influx2-0.3.4/dms_influx2/delete.py
+-rw-rw-rw-   0        0        0     1487 2023-01-19 06:30:10.000000 dms-influx2-0.3.4/dms_influx2/dtv_files.py
+-rw-rw-rw-   0        0        0      327 2023-01-09 21:18:36.000000 dms-influx2-0.3.4/dms_influx2/exceptions.py
+-rw-rw-rw-   0        0        0    25730 2023-07-14 15:05:32.000000 dms-influx2-0.3.4/dms_influx2/lib.py
+-rw-rw-rw-   0        0        0     3562 2023-01-09 21:18:36.000000 dms-influx2-0.3.4/dms_influx2/notifications.py
+-rw-rw-rw-   0        0        0     1012 2023-01-09 21:18:36.000000 dms-influx2-0.3.4/dms_influx2/organisations.py
+-rw-rw-rw-   0        0        0     7217 2023-07-04 18:39:09.000000 dms-influx2-0.3.4/dms_influx2/query.py
+-rw-rw-rw-   0        0        0        0 2023-01-18 17:42:37.000000 dms-influx2-0.3.4/dms_influx2/sync.py
+-rw-rw-rw-   0        0        0     4025 2023-01-09 21:18:36.000000 dms-influx2-0.3.4/dms_influx2/tasks.py
+-rw-rw-rw-   0        0        0     1203 2023-01-26 19:35:58.000000 dms-influx2-0.3.4/dms_influx2/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:12:24.436365 dms-influx2-0.3.4/dms_influx2.egg-info/
+-rw-rw-rw-   0        0        0      556 2023-07-17 06:12:24.000000 dms-influx2-0.3.4/dms_influx2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      636 2023-07-17 06:12:24.000000 dms-influx2-0.3.4/dms_influx2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 06:12:24.000000 dms-influx2-0.3.4/dms_influx2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       89 2023-07-17 06:12:24.000000 dms-influx2-0.3.4/dms_influx2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-17 06:12:24.000000 dms-influx2-0.3.4/dms_influx2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 06:12:24.439363 dms-influx2-0.3.4/setup.cfg
+-rw-rw-rw-   0        0        0     3023 2023-07-17 06:11:13.000000 dms-influx2-0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:12:24.438365 dms-influx2-0.3.4/tests/
+-rw-rw-rw-   0        0        0     1882 2023-07-03 09:02:50.000000 dms-influx2-0.3.4/tests/test_auth.py
+-rw-rw-rw-   0        0        0     4632 2023-07-03 09:02:50.000000 dms-influx2-0.3.4/tests/test_buckets.py
+-rw-rw-rw-   0        0        0     2018 2023-07-03 09:11:49.000000 dms-influx2-0.3.4/tests/test_copy-values.py
+-rw-rw-rw-   0        0        0    16796 2023-07-14 12:09:20.000000 dms-influx2-0.3.4/tests/test_data.py
```

### Comparing `dms-influx2-0.3.3/PKG-INFO` & `dms-influx2-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dms-influx2
-Version: 0.3.3
+Version: 0.3.4
 Summary: Library to connect and retrieve data from DMS influxdb
 Home-page: https://github.com/belingarb/dms-influx2
 Author: Bozidar Belingar
 Author-email: bozidar.belingar@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dms-influx2-0.3.3/dms_influx2/authorizations.py` & `dms-influx2-0.3.4/dms_influx2/authorizations.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.3/dms_influx2/buckets.py` & `dms-influx2-0.3.4/dms_influx2/buckets.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.3/dms_influx2/checks.py` & `dms-influx2-0.3.4/dms_influx2/checks.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.3/dms_influx2/decorators.py` & `dms-influx2-0.3.4/dms_influx2/decorators.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.3/dms_influx2/delete.py` & `dms-influx2-0.3.4/dms_influx2/delete.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.3/dms_influx2/dtv_files.py` & `dms-influx2-0.3.4/dms_influx2/dtv_files.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.3/dms_influx2/lib.py` & `dms-influx2-0.3.4/dms_influx2/lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -590,14 +590,22 @@
                         fn: (r) =>
                         ({{r with _value: (math.round(x: r._value * {decimal_places_number}) / {decimal_places_number}),}}),
                     )
                     |> to(bucket: "{downsampled_bucket}", org: "{self.org}")
             '''
         self.query_api().query(query=query)
 
-        self.delete_api().delete_data(bucket=bucket, time_from=time_from, time_to=time_to)
+        if measurement:
+            predicates = self.delete_api().delete_data(bucket=bucket,
+                                                       time_from=time_from,
+                                                       time_to=time_to,
+                                                       measurements=[measurement])
+        else:
+            predicates = self.delete_api().delete_data(bucket=bucket,
+                                                       time_from=time_from,
+                                                       time_to=time_to)
 
         query = f'''
             from(bucket: "{downsampled_bucket}") |> range(start: -100y)
                 |> to(bucket: "{bucket}", org: "{self.org}")
         '''
         self.query_api().query(query=query)
```

### Comparing `dms-influx2-0.3.3/dms_influx2/notifications.py` & `dms-influx2-0.3.4/dms_influx2/notifications.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.3/dms_influx2/organisations.py` & `dms-influx2-0.3.4/dms_influx2/organisations.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.3/dms_influx2/query.py` & `dms-influx2-0.3.4/dms_influx2/query.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.3/dms_influx2/tasks.py` & `dms-influx2-0.3.4/dms_influx2/tasks.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.3/dms_influx2/utils.py` & `dms-influx2-0.3.4/dms_influx2/utils.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.3/dms_influx2.egg-info/PKG-INFO` & `dms-influx2-0.3.4/dms_influx2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dms-influx2
-Version: 0.3.3
+Version: 0.3.4
 Summary: Library to connect and retrieve data from DMS influxdb
 Home-page: https://github.com/belingarb/dms-influx2
 Author: Bozidar Belingar
 Author-email: bozidar.belingar@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dms-influx2-0.3.3/dms_influx2.egg-info/SOURCES.txt` & `dms-influx2-0.3.4/dms_influx2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.3/setup.py` & `dms-influx2-0.3.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 NAME = 'dms-influx2'
 DESCRIPTION = 'Library to connect and retrieve data from DMS influxdb'
 URL = 'https://github.com/belingarb/dms-influx2'
 EMAIL = 'bozidar.belingar@gmail.com'
 AUTHOR = 'Bozidar Belingar'
 REQUIRES_PYTHON = '>=3.8.0'
-VERSION = '0.3.3'
+VERSION = '0.3.4'
 
 # Get required packages from requirements.txt file
 with open('requirements/base.txt') as f:
     REQUIRED = f.read().splitlines()
 
 dir_path = os.path.abspath(os.path.dirname(__file__))
```

### Comparing `dms-influx2-0.3.3/tests/test_auth.py` & `dms-influx2-0.3.4/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.3/tests/test_buckets.py` & `dms-influx2-0.3.4/tests/test_buckets.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.3/tests/test_copy-values.py` & `dms-influx2-0.3.4/tests/test_copy-values.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.3/tests/test_data.py` & `dms-influx2-0.3.4/tests/test_data.py`

 * *Files identical despite different names*

