# Comparing `tmp/crate-0.9.4.tar.gz` & `tmp/crate-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/crate-0.9.4.tar", last modified: Fri May  9 15:44:53 2014, max compression
+gzip compressed data, was "dist/crate-0.9.5.tar", last modified: Tue May 13 20:03:14 2014, max compression
```

## Comparing `crate-0.9.4.tar` & `crate-0.9.5.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 philipp    (501) staff       (20)        0 2014-05-09 15:44:53.000000 crate-0.9.4/
--rw-r--r--   0 philipp    (501) staff       (20)     2003 2014-05-09 14:34:27.000000 crate-0.9.4/DEVELOP.rst
-drwxr-xr-x   0 philipp    (501) staff       (20)        0 2014-05-09 15:44:53.000000 crate-0.9.4/docs/
--rw-r--r--   0 philipp    (501) staff       (20)      587 2014-05-05 16:02:56.000000 crate-0.9.4/docs/advanced_usage.txt
--rw-r--r--   0 philipp    (501) staff       (20)     2766 2013-10-01 07:09:38.000000 crate-0.9.4/docs/blobs.txt
--rw-r--r--   0 philipp    (501) staff       (20)     4927 2014-05-09 14:34:27.000000 crate-0.9.4/docs/client.txt
--rw-r--r--   0 philipp    (501) staff       (20)     1814 2014-05-09 14:34:27.000000 crate-0.9.4/docs/https.txt
--rw-r--r--   0 philipp    (501) staff       (20)      205 2014-05-09 14:34:27.000000 crate-0.9.4/docs/index.txt
--rw-r--r--   0 philipp    (501) staff       (20)       17 2014-05-09 14:34:27.000000 crate-0.9.4/docs/requirements.txt
--rw-r--r--   0 philipp    (501) staff       (20)     8112 2014-05-09 14:34:27.000000 crate-0.9.4/docs/sqlalchemy.txt
--rw-r--r--   0 philipp    (501) staff       (20)    12029 2014-04-08 15:00:28.000000 crate-0.9.4/LICENSE
--rw-r--r--   0 philipp    (501) staff       (20)      125 2013-10-01 07:09:38.000000 crate-0.9.4/MANIFEST.in
--rw-r--r--   0 philipp    (501) staff       (20)    14363 2014-05-09 15:44:53.000000 crate-0.9.4/PKG-INFO
--rw-r--r--   0 philipp    (501) staff       (20)     2847 2014-05-09 14:34:27.000000 crate-0.9.4/README.rst
--rw-r--r--   0 philipp    (501) staff       (20)       82 2014-05-09 15:44:53.000000 crate-0.9.4/setup.cfg
--rw-r--r--   0 philipp    (501) staff       (20)     3201 2014-05-09 14:34:27.000000 crate-0.9.4/setup.py
-drwxr-xr-x   0 philipp    (501) staff       (20)        0 2014-05-09 15:44:53.000000 crate-0.9.4/src/
-drwxr-xr-x   0 philipp    (501) staff       (20)        0 2014-05-09 15:44:53.000000 crate-0.9.4/src/crate/
--rw-r--r--   0 philipp    (501) staff       (20)     1227 2014-04-08 15:00:28.000000 crate-0.9.4/src/crate/__init__.py
-drwxr-xr-x   0 philipp    (501) staff       (20)        0 2014-05-09 15:44:53.000000 crate-0.9.4/src/crate/client/
--rw-r--r--   0 philipp    (501) staff       (20)     1251 2014-05-09 15:42:10.000000 crate-0.9.4/src/crate/client/__init__.py
--rw-r--r--   0 philipp    (501) staff       (20)     3273 2014-05-09 14:34:27.000000 crate-0.9.4/src/crate/client/blob.py
--rw-r--r--   0 philipp    (501) staff       (20)     1881 2014-05-09 14:34:27.000000 crate-0.9.4/src/crate/client/blob.txt
--rw-r--r--   0 philipp    (501) staff       (20)     1745 2014-04-08 15:00:28.000000 crate-0.9.4/src/crate/client/compat.py
--rw-r--r--   0 philipp    (501) staff       (20)     3520 2014-05-09 14:34:27.000000 crate-0.9.4/src/crate/client/connection.py
--rw-r--r--   0 philipp    (501) staff       (20)     1086 2013-10-01 07:09:38.000000 crate-0.9.4/src/crate/client/connection.txt
--rw-r--r--   0 philipp    (501) staff       (20)     6215 2014-05-09 14:34:27.000000 crate-0.9.4/src/crate/client/cursor.py
--rw-r--r--   0 philipp    (501) staff       (20)     4752 2014-05-09 14:34:27.000000 crate-0.9.4/src/crate/client/cursor.txt
--rw-r--r--   0 philipp    (501) staff       (20)     2188 2014-04-08 15:00:28.000000 crate-0.9.4/src/crate/client/exceptions.py
--rw-r--r--   0 philipp    (501) staff       (20)    13804 2014-05-09 15:35:38.000000 crate-0.9.4/src/crate/client/http.py
--rw-r--r--   0 philipp    (501) staff       (20)     5930 2014-05-09 14:34:27.000000 crate-0.9.4/src/crate/client/http.txt
-drwxr-xr-x   0 philipp    (501) staff       (20)        0 2014-05-09 15:44:53.000000 crate-0.9.4/src/crate/client/sqlalchemy/
--rw-r--r--   0 philipp    (501) staff       (20)     1057 2014-04-08 15:00:28.000000 crate-0.9.4/src/crate/client/sqlalchemy/__init__.py
--rw-r--r--   0 philipp    (501) staff       (20)     5590 2014-04-08 15:00:28.000000 crate-0.9.4/src/crate/client/sqlalchemy/compiler.py
--rw-r--r--   0 philipp    (501) staff       (20)     5658 2014-04-08 15:00:28.000000 crate-0.9.4/src/crate/client/sqlalchemy/dialect.py
--rw-r--r--   0 philipp    (501) staff       (20)     4549 2014-05-09 14:34:27.000000 crate-0.9.4/src/crate/client/sqlalchemy/itests.txt
-drwxr-xr-x   0 philipp    (501) staff       (20)        0 2014-05-09 15:44:53.000000 crate-0.9.4/src/crate/client/sqlalchemy/tests/
--rw-r--r--   0 philipp    (501) staff       (20)      463 2014-05-09 14:34:27.000000 crate-0.9.4/src/crate/client/sqlalchemy/tests/__init__.py
--rw-r--r--   0 philipp    (501) staff       (20)     2171 2014-05-09 14:34:27.000000 crate-0.9.4/src/crate/client/sqlalchemy/tests/connection_test.py
--rw-r--r--   0 philipp    (501) staff       (20)     3080 2014-05-09 14:34:27.000000 crate-0.9.4/src/crate/client/sqlalchemy/tests/datetime_test.py
--rw-r--r--   0 philipp    (501) staff       (20)    14284 2014-05-09 14:34:27.000000 crate-0.9.4/src/crate/client/sqlalchemy/tests/dict_test.py
--rw-r--r--   0 philipp    (501) staff       (20)     3776 2014-04-08 15:00:28.000000 crate-0.9.4/src/crate/client/sqlalchemy/types.py
--rw-r--r--   0 philipp    (501) staff       (20)     1478 2014-04-08 15:00:28.000000 crate-0.9.4/src/crate/client/test_cursor.py
--rw-r--r--   0 philipp    (501) staff       (20)     9379 2014-05-09 15:35:38.000000 crate-0.9.4/src/crate/client/test_http.py
-drwxr-xr-x   0 philipp    (501) staff       (20)        0 2014-05-09 15:44:53.000000 crate-0.9.4/src/crate/testing/
--rw-r--r--   0 philipp    (501) staff       (20)       10 2013-10-01 07:09:38.000000 crate-0.9.4/src/crate/testing/__init__.py
--rw-r--r--   0 philipp    (501) staff       (20)     3290 2014-05-09 14:34:27.000000 crate-0.9.4/src/crate/testing/layer.py
--rw-r--r--   0 philipp    (501) staff       (20)     1131 2014-05-09 14:34:27.000000 crate-0.9.4/src/crate/testing/layer.txt
-drwxr-xr-x   0 philipp    (501) staff       (20)        0 2014-05-09 15:44:53.000000 crate-0.9.4/src/crate.egg-info/
--rw-r--r--   0 philipp    (501) staff       (20)        1 2014-05-09 15:44:52.000000 crate-0.9.4/src/crate.egg-info/dependency_links.txt
--rw-r--r--   0 philipp    (501) staff       (20)       68 2014-05-09 15:44:52.000000 crate-0.9.4/src/crate.egg-info/entry_points.txt
--rw-r--r--   0 philipp    (501) staff       (20)        6 2014-05-09 15:44:52.000000 crate-0.9.4/src/crate.egg-info/namespace_packages.txt
--rw-r--r--   0 philipp    (501) staff       (20)    14363 2014-05-09 15:44:52.000000 crate-0.9.4/src/crate.egg-info/PKG-INFO
--rw-r--r--   0 philipp    (501) staff       (20)      130 2014-05-09 15:44:52.000000 crate-0.9.4/src/crate.egg-info/requires.txt
--rw-r--r--   0 philipp    (501) staff       (20)     1298 2014-05-09 15:44:53.000000 crate-0.9.4/src/crate.egg-info/SOURCES.txt
--rw-r--r--   0 philipp    (501) staff       (20)        6 2014-05-09 15:44:52.000000 crate-0.9.4/src/crate.egg-info/top_level.txt
+drwxr-xr-x   0 lui        (501) staff       (20)        0 2014-05-13 20:03:14.000000 crate-0.9.5/
+-rw-r--r--   0 lui        (501) staff       (20)     2003 2014-05-12 07:47:12.000000 crate-0.9.5/DEVELOP.rst
+drwxr-xr-x   0 lui        (501) staff       (20)        0 2014-05-13 20:03:14.000000 crate-0.9.5/docs/
+-rw-r--r--   0 lui        (501) staff       (20)      587 2014-04-07 07:50:12.000000 crate-0.9.5/docs/advanced_usage.txt
+-rw-r--r--   0 lui        (501) staff       (20)     2766 2014-04-07 07:50:12.000000 crate-0.9.5/docs/blobs.txt
+-rw-r--r--   0 lui        (501) staff       (20)     4927 2014-04-19 19:51:37.000000 crate-0.9.5/docs/client.txt
+-rw-r--r--   0 lui        (501) staff       (20)     1814 2014-04-19 19:51:37.000000 crate-0.9.5/docs/https.txt
+-rw-r--r--   0 lui        (501) staff       (20)      205 2014-05-12 07:47:12.000000 crate-0.9.5/docs/index.txt
+-rw-r--r--   0 lui        (501) staff       (20)       17 2014-05-12 07:47:12.000000 crate-0.9.5/docs/requirements.txt
+-rw-r--r--   0 lui        (501) staff       (20)     8112 2014-05-12 07:47:12.000000 crate-0.9.5/docs/sqlalchemy.txt
+-rw-r--r--   0 lui        (501) staff       (20)    12029 2014-04-07 07:50:12.000000 crate-0.9.5/LICENSE
+-rw-r--r--   0 lui        (501) staff       (20)      125 2014-04-07 07:50:12.000000 crate-0.9.5/MANIFEST.in
+-rw-r--r--   0 lui        (501) staff       (20)    14363 2014-05-13 20:03:14.000000 crate-0.9.5/PKG-INFO
+-rw-r--r--   0 lui        (501) staff       (20)     2847 2014-05-12 07:47:12.000000 crate-0.9.5/README.rst
+-rw-r--r--   0 lui        (501) staff       (20)       82 2014-05-13 20:03:14.000000 crate-0.9.5/setup.cfg
+-rw-r--r--   0 lui        (501) staff       (20)     3201 2014-05-12 07:47:12.000000 crate-0.9.5/setup.py
+drwxr-xr-x   0 lui        (501) staff       (20)        0 2014-05-13 20:03:14.000000 crate-0.9.5/src/
+drwxr-xr-x   0 lui        (501) staff       (20)        0 2014-05-13 20:03:14.000000 crate-0.9.5/src/crate/
+-rw-r--r--   0 lui        (501) staff       (20)     1227 2014-04-07 07:50:12.000000 crate-0.9.5/src/crate/__init__.py
+drwxr-xr-x   0 lui        (501) staff       (20)        0 2014-05-13 20:03:14.000000 crate-0.9.5/src/crate/client/
+-rw-r--r--   0 lui        (501) staff       (20)     1251 2014-05-13 19:51:59.000000 crate-0.9.5/src/crate/client/__init__.py
+-rw-r--r--   0 lui        (501) staff       (20)     3273 2014-04-19 19:51:37.000000 crate-0.9.5/src/crate/client/blob.py
+-rw-r--r--   0 lui        (501) staff       (20)     1881 2014-04-19 19:51:37.000000 crate-0.9.5/src/crate/client/blob.txt
+-rw-r--r--   0 lui        (501) staff       (20)     1745 2014-04-07 07:50:12.000000 crate-0.9.5/src/crate/client/compat.py
+-rw-r--r--   0 lui        (501) staff       (20)     3520 2014-04-07 07:50:12.000000 crate-0.9.5/src/crate/client/connection.py
+-rw-r--r--   0 lui        (501) staff       (20)     1086 2014-04-07 07:50:12.000000 crate-0.9.5/src/crate/client/connection.txt
+-rw-r--r--   0 lui        (501) staff       (20)     6215 2014-04-07 07:50:12.000000 crate-0.9.5/src/crate/client/cursor.py
+-rw-r--r--   0 lui        (501) staff       (20)     4752 2014-04-07 07:50:12.000000 crate-0.9.5/src/crate/client/cursor.txt
+-rw-r--r--   0 lui        (501) staff       (20)     2188 2014-04-07 07:50:12.000000 crate-0.9.5/src/crate/client/exceptions.py
+-rw-r--r--   0 lui        (501) staff       (20)    13804 2014-05-12 07:47:12.000000 crate-0.9.5/src/crate/client/http.py
+-rw-r--r--   0 lui        (501) staff       (20)     5930 2014-04-19 19:51:37.000000 crate-0.9.5/src/crate/client/http.txt
+drwxr-xr-x   0 lui        (501) staff       (20)        0 2014-05-13 20:03:14.000000 crate-0.9.5/src/crate/client/sqlalchemy/
+-rw-r--r--   0 lui        (501) staff       (20)     1057 2014-04-07 07:50:12.000000 crate-0.9.5/src/crate/client/sqlalchemy/__init__.py
+-rw-r--r--   0 lui        (501) staff       (20)     5665 2014-05-13 19:16:40.000000 crate-0.9.5/src/crate/client/sqlalchemy/compiler.py
+-rw-r--r--   0 lui        (501) staff       (20)     5658 2014-04-07 07:50:12.000000 crate-0.9.5/src/crate/client/sqlalchemy/dialect.py
+-rw-r--r--   0 lui        (501) staff       (20)     4549 2014-04-07 07:50:12.000000 crate-0.9.5/src/crate/client/sqlalchemy/itests.txt
+drwxr-xr-x   0 lui        (501) staff       (20)        0 2014-05-13 20:03:14.000000 crate-0.9.5/src/crate/client/sqlalchemy/tests/
+-rw-r--r--   0 lui        (501) staff       (20)      566 2014-05-13 18:55:07.000000 crate-0.9.5/src/crate/client/sqlalchemy/tests/__init__.py
+-rw-r--r--   0 lui        (501) staff       (20)     2264 2014-05-13 18:55:07.000000 crate-0.9.5/src/crate/client/sqlalchemy/tests/compiler_test.py
+-rw-r--r--   0 lui        (501) staff       (20)     2171 2014-04-07 07:50:12.000000 crate-0.9.5/src/crate/client/sqlalchemy/tests/connection_test.py
+-rw-r--r--   0 lui        (501) staff       (20)     3080 2014-04-07 07:50:12.000000 crate-0.9.5/src/crate/client/sqlalchemy/tests/datetime_test.py
+-rw-r--r--   0 lui        (501) staff       (20)    14284 2014-04-07 07:50:12.000000 crate-0.9.5/src/crate/client/sqlalchemy/tests/dict_test.py
+-rw-r--r--   0 lui        (501) staff       (20)     3776 2014-04-07 07:50:12.000000 crate-0.9.5/src/crate/client/sqlalchemy/types.py
+-rw-r--r--   0 lui        (501) staff       (20)     1478 2014-04-07 07:50:12.000000 crate-0.9.5/src/crate/client/test_cursor.py
+-rw-r--r--   0 lui        (501) staff       (20)     9380 2014-05-13 19:03:47.000000 crate-0.9.5/src/crate/client/test_http.py
+drwxr-xr-x   0 lui        (501) staff       (20)        0 2014-05-13 20:03:14.000000 crate-0.9.5/src/crate/testing/
+-rw-r--r--   0 lui        (501) staff       (20)       10 2014-04-07 07:50:12.000000 crate-0.9.5/src/crate/testing/__init__.py
+-rw-r--r--   0 lui        (501) staff       (20)     3290 2014-04-19 19:51:37.000000 crate-0.9.5/src/crate/testing/layer.py
+-rw-r--r--   0 lui        (501) staff       (20)     1131 2014-04-19 19:51:37.000000 crate-0.9.5/src/crate/testing/layer.txt
+drwxr-xr-x   0 lui        (501) staff       (20)        0 2014-05-13 20:03:14.000000 crate-0.9.5/src/crate.egg-info/
+-rw-r--r--   0 lui        (501) staff       (20)        1 2014-05-13 20:03:14.000000 crate-0.9.5/src/crate.egg-info/dependency_links.txt
+-rw-r--r--   0 lui        (501) staff       (20)       68 2014-05-13 20:03:14.000000 crate-0.9.5/src/crate.egg-info/entry_points.txt
+-rw-r--r--   0 lui        (501) staff       (20)        6 2014-05-13 20:03:14.000000 crate-0.9.5/src/crate.egg-info/namespace_packages.txt
+-rw-r--r--   0 lui        (501) staff       (20)    14363 2014-05-13 20:03:14.000000 crate-0.9.5/src/crate.egg-info/PKG-INFO
+-rw-r--r--   0 lui        (501) staff       (20)      130 2014-05-13 20:03:14.000000 crate-0.9.5/src/crate.egg-info/requires.txt
+-rw-r--r--   0 lui        (501) staff       (20)     1349 2014-05-13 20:03:14.000000 crate-0.9.5/src/crate.egg-info/SOURCES.txt
+-rw-r--r--   0 lui        (501) staff       (20)        6 2014-05-13 20:03:14.000000 crate-0.9.5/src/crate.egg-info/top_level.txt
```

### Comparing `crate-0.9.4/DEVELOP.rst` & `crate-0.9.5/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `crate-0.9.4/docs/advanced_usage.txt` & `crate-0.9.5/docs/advanced_usage.txt`

 * *Files identical despite different names*

### Comparing `crate-0.9.4/docs/blobs.txt` & `crate-0.9.5/docs/blobs.txt`

 * *Files identical despite different names*

### Comparing `crate-0.9.4/docs/client.txt` & `crate-0.9.5/docs/client.txt`

 * *Files identical despite different names*

### Comparing `crate-0.9.4/docs/https.txt` & `crate-0.9.5/docs/https.txt`

 * *Files identical despite different names*

### Comparing `crate-0.9.4/docs/sqlalchemy.txt` & `crate-0.9.5/docs/sqlalchemy.txt`

 * *Files identical despite different names*

### Comparing `crate-0.9.4/LICENSE` & `crate-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `crate-0.9.4/PKG-INFO` & `crate-0.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: crate
-Version: 0.9.4
+Version: 0.9.5
 Summary: Crate Data Python client
 Home-page: https://github.com/crate/crate-python
 Author: CRATE Technology GmbH
 Author-email: office@crate.io
 License: Apache License 2.0
 Description: .. image:: https://cdn.crate.io/web/1.0.0/img/logo-solid.png
            :width: 155px
```

### Comparing `crate-0.9.4/README.rst` & `crate-0.9.5/README.rst`

 * *Files identical despite different names*

### Comparing `crate-0.9.4/setup.py` & `crate-0.9.5/setup.py`

 * *Files identical despite different names*

### Comparing `crate-0.9.4/src/crate/__init__.py` & `crate-0.9.5/src/crate/__init__.py`

 * *Files identical despite different names*

### Comparing `crate-0.9.4/src/crate/client/__init__.py` & `crate-0.9.5/src/crate/client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,12 +20,12 @@
 # software solely pursuant to the terms of the relevant commercial agreement.
 
 from .connection import connect
 from .exceptions import Error
 
 # version string read from setup.py using a regex. Take care not to break the
 # regex!
-__version__ = "0.9.4"
+__version__ = "0.9.5"
 
 apilevel = "2.0"
 threadsafety = 2
 paramstyle = "qmark"
```

### Comparing `crate-0.9.4/src/crate/client/blob.py` & `crate-0.9.5/src/crate/client/blob.py`

 * *Files identical despite different names*

### Comparing `crate-0.9.4/src/crate/client/blob.txt` & `crate-0.9.5/src/crate/client/blob.txt`

 * *Files identical despite different names*

### Comparing `crate-0.9.4/src/crate/client/compat.py` & `crate-0.9.5/src/crate/client/compat.py`

 * *Files identical despite different names*

### Comparing `crate-0.9.4/src/crate/client/connection.py` & `crate-0.9.5/src/crate/client/connection.py`

 * *Files identical despite different names*

### Comparing `crate-0.9.4/src/crate/client/connection.txt` & `crate-0.9.5/src/crate/client/connection.txt`

 * *Files identical despite different names*

### Comparing `crate-0.9.4/src/crate/client/cursor.py` & `crate-0.9.5/src/crate/client/cursor.py`

 * *Files identical despite different names*

### Comparing `crate-0.9.4/src/crate/client/cursor.txt` & `crate-0.9.5/src/crate/client/cursor.txt`

 * *Files identical despite different names*

### Comparing `crate-0.9.4/src/crate/client/exceptions.py` & `crate-0.9.5/src/crate/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `crate-0.9.4/src/crate/client/http.py` & `crate-0.9.5/src/crate/client/http.py`

 * *Files identical despite different names*

### Comparing `crate-0.9.4/src/crate/client/http.txt` & `crate-0.9.5/src/crate/client/http.txt`

 * *Files identical despite different names*

### Comparing `crate-0.9.4/src/crate/client/sqlalchemy/__init__.py` & `crate-0.9.5/src/crate/client/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `crate-0.9.4/src/crate/client/sqlalchemy/compiler.py` & `crate-0.9.5/src/crate/client/sqlalchemy/compiler.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         "col = ?", ({"x": 1, "y": 2}
 
     but crate supports
 
         "col['x'] = ?, col['y'] = ?", (1, 2)
 
     by using the `Craty` (`MutableDict`) type.
-    The update statement is only rewritten if a item of the MutableDict was
+    The update statement is only rewritten if an item of the MutableDict was
     changed.
     """
 
     newmultiparams = []
     for params in multiparams:
         newparams = {}
         for key, val in params.items():
@@ -69,15 +69,16 @@
     # use CrateCompiler specific visit_update
     clauseelement._crate_specific = True
     return clauseelement, multiparams, params
 
 
 @sa.event.listens_for(sa.engine.Engine, "before_execute", retval=True)
 def crate_before_execute(conn, clauseelement, multiparams, params):
-    if isinstance(clauseelement, sa.sql.expression.Update):
+    is_crate = type(conn.dialect).__name__ == 'CrateDialect'
+    if is_crate and isinstance(clauseelement, sa.sql.expression.Update):
         return rewrite_update(clauseelement, multiparams, params)
     return clauseelement, multiparams, params
 
 
 class CrateCompiler(SQLCompiler):
 
     def visit_getitem_binary(self, binary, operator, **kw):
```

### Comparing `crate-0.9.4/src/crate/client/sqlalchemy/dialect.py` & `crate-0.9.5/src/crate/client/sqlalchemy/dialect.py`

 * *Files identical despite different names*

### Comparing `crate-0.9.4/src/crate/client/sqlalchemy/itests.txt` & `crate-0.9.5/src/crate/client/sqlalchemy/itests.txt`

 * *Files identical despite different names*

### Comparing `crate-0.9.4/src/crate/client/sqlalchemy/tests/connection_test.py` & `crate-0.9.5/src/crate/client/sqlalchemy/tests/connection_test.py`

 * *Files identical despite different names*

### Comparing `crate-0.9.4/src/crate/client/sqlalchemy/tests/datetime_test.py` & `crate-0.9.5/src/crate/client/sqlalchemy/tests/datetime_test.py`

 * *Files identical despite different names*

### Comparing `crate-0.9.4/src/crate/client/sqlalchemy/tests/dict_test.py` & `crate-0.9.5/src/crate/client/sqlalchemy/tests/dict_test.py`

 * *Files identical despite different names*

### Comparing `crate-0.9.4/src/crate/client/sqlalchemy/types.py` & `crate-0.9.5/src/crate/client/sqlalchemy/types.py`

 * *Files identical despite different names*

### Comparing `crate-0.9.4/src/crate/client/test_cursor.py` & `crate-0.9.5/src/crate/client/test_cursor.py`

 * *Files identical despite different names*

### Comparing `crate-0.9.4/src/crate/client/test_http.py` & `crate-0.9.5/src/crate/client/test_http.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
             return mock_response
 
 
 class HttpClientTest(TestCase):
 
     def test_no_connection_exception(self):
         client = Client()
-        self.assertRaises(ConnectionError, client.sql, 'select 1')
+        self.assertRaises(ProgrammingError, client.sql, 'select 1')
 
     @patch('crate.client.http.Server', FakeServerRaisingGeneralException)
     def test_http_error_is_re_raised(self):
         client = Client()
         self.assertRaises(ProgrammingError, client.sql, 'select 1')
 
     @patch('crate.client.http.Server', FakeServerRaisingGeneralException)
```

### Comparing `crate-0.9.4/src/crate/testing/layer.py` & `crate-0.9.5/src/crate/testing/layer.py`

 * *Files identical despite different names*

### Comparing `crate-0.9.4/src/crate/testing/layer.txt` & `crate-0.9.5/src/crate/testing/layer.txt`

 * *Files identical despite different names*

### Comparing `crate-0.9.4/src/crate.egg-info/PKG-INFO` & `crate-0.9.5/src/crate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: crate
-Version: 0.9.4
+Version: 0.9.5
 Summary: Crate Data Python client
 Home-page: https://github.com/crate/crate-python
 Author: CRATE Technology GmbH
 Author-email: office@crate.io
 License: Apache License 2.0
 Description: .. image:: https://cdn.crate.io/web/1.0.0/img/logo-solid.png
            :width: 155px
```

### Comparing `crate-0.9.4/src/crate.egg-info/SOURCES.txt` & `crate-0.9.5/src/crate.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -34,13 +34,14 @@
 src/crate/client/test_http.py
 src/crate/client/sqlalchemy/__init__.py
 src/crate/client/sqlalchemy/compiler.py
 src/crate/client/sqlalchemy/dialect.py
 src/crate/client/sqlalchemy/itests.txt
 src/crate/client/sqlalchemy/types.py
 src/crate/client/sqlalchemy/tests/__init__.py
+src/crate/client/sqlalchemy/tests/compiler_test.py
 src/crate/client/sqlalchemy/tests/connection_test.py
 src/crate/client/sqlalchemy/tests/datetime_test.py
 src/crate/client/sqlalchemy/tests/dict_test.py
 src/crate/testing/__init__.py
 src/crate/testing/layer.py
 src/crate/testing/layer.txt
```

