# Comparing `tmp/seatable-api-2.6.6.tar.gz` & `tmp/seatable-api-2.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seatable-api-2.6.6.tar", last modified: Fri Jul 14 06:57:02 2023, max compression
+gzip compressed data, was "seatable-api-2.6.7.tar", last modified: Mon Jul 17 08:26:43 2023, max compression
```

## Comparing `seatable-api-2.6.6.tar` & `seatable-api-2.6.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 chengxiongchao   (501) staff       (20)        0 2023-07-14 06:57:02.442038 seatable-api-2.6.6/
--rw-r--r--   0 chengxiongchao   (501) staff       (20)    11357 2023-01-04 02:34:58.000000 seatable-api-2.6.6/LICENSE
--rw-r--r--   0 chengxiongchao   (501) staff       (20)      656 2023-07-14 06:57:02.437045 seatable-api-2.6.6/PKG-INFO
--rw-r--r--   0 chengxiongchao   (501) staff       (20)      300 2023-01-04 02:34:58.000000 seatable-api-2.6.6/README.md
-drwxr-xr-x   0 chengxiongchao   (501) staff       (20)        0 2023-07-14 06:57:02.428316 seatable-api-2.6.6/seatable_api/
--rw-r--r--   0 chengxiongchao   (501) staff       (20)      171 2023-01-04 02:34:58.000000 seatable-api-2.6.6/seatable_api/__init__.py
--rw-r--r--   0 chengxiongchao   (501) staff       (20)    11418 2023-01-04 02:34:58.000000 seatable-api-2.6.6/seatable_api/column.py
--rw-r--r--   0 chengxiongchao   (501) staff       (20)     1135 2023-01-04 02:34:58.000000 seatable-api-2.6.6/seatable_api/constants.py
--rw-r--r--   0 chengxiongchao   (501) staff       (20)     1322 2023-07-14 06:55:21.000000 seatable-api-2.6.6/seatable_api/context.py
--rw-r--r--   0 chengxiongchao   (501) staff       (20)    29097 2023-01-04 02:34:58.000000 seatable-api-2.6.6/seatable_api/convert_airtable.py
--rw-r--r--   0 chengxiongchao   (501) staff       (20)    13988 2023-01-04 02:34:58.000000 seatable-api-2.6.6/seatable_api/date_utils.py
--rw-r--r--   0 chengxiongchao   (501) staff       (20)      119 2023-04-03 02:56:24.000000 seatable-api-2.6.6/seatable_api/exception.py
--rw-r--r--   0 chengxiongchao   (501) staff       (20)    42361 2023-07-14 06:55:21.000000 seatable-api-2.6.6/seatable_api/main.py
--rw-r--r--   0 chengxiongchao   (501) staff       (20)     2876 2023-01-04 02:34:58.000000 seatable-api-2.6.6/seatable_api/message.py
--rw-r--r--   0 chengxiongchao   (501) staff       (20)     9400 2023-01-04 02:34:58.000000 seatable-api-2.6.6/seatable_api/query.py
--rw-r--r--   0 chengxiongchao   (501) staff       (20)     2744 2023-01-04 02:34:58.000000 seatable-api-2.6.6/seatable_api/socket_io.py
--rw-r--r--   0 chengxiongchao   (501) staff       (20)     6424 2023-01-04 02:34:58.000000 seatable-api-2.6.6/seatable_api/utils.py
-drwxr-xr-x   0 chengxiongchao   (501) staff       (20)        0 2023-07-14 06:57:02.432160 seatable-api-2.6.6/seatable_api.egg-info/
--rw-r--r--   0 chengxiongchao   (501) staff       (20)      656 2023-07-14 06:57:02.000000 seatable-api-2.6.6/seatable_api.egg-info/PKG-INFO
--rw-r--r--   0 chengxiongchao   (501) staff       (20)      546 2023-07-14 06:57:02.000000 seatable-api-2.6.6/seatable_api.egg-info/SOURCES.txt
--rw-r--r--   0 chengxiongchao   (501) staff       (20)        1 2023-07-14 06:57:02.000000 seatable-api-2.6.6/seatable_api.egg-info/dependency_links.txt
--rw-r--r--   0 chengxiongchao   (501) staff       (20)       47 2023-07-14 06:57:02.000000 seatable-api-2.6.6/seatable_api.egg-info/requires.txt
--rw-r--r--   0 chengxiongchao   (501) staff       (20)       19 2023-07-14 06:57:02.000000 seatable-api-2.6.6/seatable_api.egg-info/top_level.txt
--rw-r--r--   0 chengxiongchao   (501) staff       (20)       38 2023-07-14 06:57:02.442480 seatable-api-2.6.6/setup.cfg
--rw-r--r--   0 chengxiongchao   (501) staff       (20)      723 2023-07-14 06:56:35.000000 seatable-api-2.6.6/setup.py
-drwxr-xr-x   0 chengxiongchao   (501) staff       (20)        0 2023-07-14 06:57:02.434862 seatable-api-2.6.6/tests/
--rw-r--r--   0 chengxiongchao   (501) staff       (20)        0 2023-06-13 02:45:17.000000 seatable-api-2.6.6/tests/__init__.py
--rw-r--r--   0 chengxiongchao   (501) staff       (20)     5261 2023-06-13 02:45:20.000000 seatable-api-2.6.6/tests/dateutils_test.py
+drwxr-xr-x   0 skywalker   (501) staff       (20)        0 2023-07-17 08:26:43.036495 seatable-api-2.6.7/
+-rw-r--r--   0 skywalker   (501) staff       (20)    11357 2023-03-22 02:01:50.000000 seatable-api-2.6.7/LICENSE
+-rw-r--r--   0 skywalker   (501) staff       (20)      656 2023-07-17 08:26:43.036366 seatable-api-2.6.7/PKG-INFO
+-rw-r--r--   0 skywalker   (501) staff       (20)      300 2023-03-22 02:01:50.000000 seatable-api-2.6.7/README.md
+drwxr-xr-x   0 skywalker   (501) staff       (20)        0 2023-07-17 08:26:43.034819 seatable-api-2.6.7/seatable_api/
+-rw-r--r--   0 skywalker   (501) staff       (20)      171 2023-03-22 02:01:50.000000 seatable-api-2.6.7/seatable_api/__init__.py
+-rw-r--r--   0 skywalker   (501) staff       (20)    11418 2023-03-22 02:01:50.000000 seatable-api-2.6.7/seatable_api/column.py
+-rw-r--r--   0 skywalker   (501) staff       (20)     1135 2023-03-22 02:01:50.000000 seatable-api-2.6.7/seatable_api/constants.py
+-rw-r--r--   0 skywalker   (501) staff       (20)     1322 2023-07-10 10:10:12.000000 seatable-api-2.6.7/seatable_api/context.py
+-rw-r--r--   0 skywalker   (501) staff       (20)    29203 2023-07-17 08:23:32.000000 seatable-api-2.6.7/seatable_api/convert_airtable.py
+-rw-r--r--   0 skywalker   (501) staff       (20)    13988 2023-03-22 02:01:50.000000 seatable-api-2.6.7/seatable_api/date_utils.py
+-rw-r--r--   0 skywalker   (501) staff       (20)      119 2023-03-22 02:01:50.000000 seatable-api-2.6.7/seatable_api/exception.py
+-rw-r--r--   0 skywalker   (501) staff       (20)    42361 2023-07-10 10:10:12.000000 seatable-api-2.6.7/seatable_api/main.py
+-rw-r--r--   0 skywalker   (501) staff       (20)     2876 2023-03-22 02:01:50.000000 seatable-api-2.6.7/seatable_api/message.py
+-rw-r--r--   0 skywalker   (501) staff       (20)     9400 2023-03-22 02:01:50.000000 seatable-api-2.6.7/seatable_api/query.py
+-rw-r--r--   0 skywalker   (501) staff       (20)     2744 2023-03-22 02:01:50.000000 seatable-api-2.6.7/seatable_api/socket_io.py
+-rw-r--r--   0 skywalker   (501) staff       (20)     6424 2023-03-22 02:01:50.000000 seatable-api-2.6.7/seatable_api/utils.py
+drwxr-xr-x   0 skywalker   (501) staff       (20)        0 2023-07-17 08:26:43.035716 seatable-api-2.6.7/seatable_api.egg-info/
+-rw-r--r--   0 skywalker   (501) staff       (20)      656 2023-07-17 08:26:43.000000 seatable-api-2.6.7/seatable_api.egg-info/PKG-INFO
+-rw-r--r--   0 skywalker   (501) staff       (20)      546 2023-07-17 08:26:43.000000 seatable-api-2.6.7/seatable_api.egg-info/SOURCES.txt
+-rw-r--r--   0 skywalker   (501) staff       (20)        1 2023-07-17 08:26:43.000000 seatable-api-2.6.7/seatable_api.egg-info/dependency_links.txt
+-rw-r--r--   0 skywalker   (501) staff       (20)       47 2023-07-17 08:26:43.000000 seatable-api-2.6.7/seatable_api.egg-info/requires.txt
+-rw-r--r--   0 skywalker   (501) staff       (20)       19 2023-07-17 08:26:43.000000 seatable-api-2.6.7/seatable_api.egg-info/top_level.txt
+-rw-r--r--   0 skywalker   (501) staff       (20)       38 2023-07-17 08:26:43.036553 seatable-api-2.6.7/setup.cfg
+-rw-r--r--   0 skywalker   (501) staff       (20)      723 2023-07-17 08:26:31.000000 seatable-api-2.6.7/setup.py
+drwxr-xr-x   0 skywalker   (501) staff       (20)        0 2023-07-17 08:26:43.035967 seatable-api-2.6.7/tests/
+-rw-r--r--   0 skywalker   (501) staff       (20)        0 2023-03-22 02:01:50.000000 seatable-api-2.6.7/tests/__init__.py
+-rw-r--r--   0 skywalker   (501) staff       (20)     5261 2023-03-22 02:01:50.000000 seatable-api-2.6.7/tests/dateutils_test.py
```

### Comparing `seatable-api-2.6.6/LICENSE` & `seatable-api-2.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `seatable-api-2.6.6/PKG-INFO` & `seatable-api-2.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seatable-api
-Version: 2.6.6
+Version: 2.6.7
 Summary: Python client for SeaTable web api
 Home-page: https://github.com/seatable/seatable-api-python
 Author: seatable
 Author-email: support@seafile.com
 License: Apache Licence
 Platform: any
 Classifier: Programming Language :: Python
```

### Comparing `seatable-api-2.6.6/seatable_api/column.py` & `seatable-api-2.6.7/seatable_api/column.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.6.6/seatable_api/constants.py` & `seatable-api-2.6.7/seatable_api/constants.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.6.6/seatable_api/context.py` & `seatable-api-2.6.7/seatable_api/context.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.6.6/seatable_api/convert_airtable.py` & `seatable-api-2.6.7/seatable_api/convert_airtable.py`

 * *Files 0% similar despite different names*

```diff
@@ -301,15 +301,15 @@
                         item = str(item)
                         if item not in select_list:
                             select_list.append(item)
                 column_data = {'options': self.get_select_options(select_list)}
             elif column_type == ColumnTypes.COLLABORATOR:
                 column_type = ColumnTypes.TEXT
         except Exception as e:
-            print('[Warning] get', column_type.value, 'column data error:', e)
+            print('[Warning] get', column_type.value, column_name, 'column data error:', e)
         return column_type, column_data
 
     def get_column_type(self, values):
         column_type = ColumnTypes.TEXT
         try:
             type_list = []
             for value in values:
@@ -378,14 +378,16 @@
         columns = []
         for column_name, values in value_map.items():
             if column_name == '_id':
                 continue
             column_type = self.get_column_type(values)
             column_type, column_data = self.get_column_data(
                 link_map, table_name, column_name, column_type, values)
+            if column_type == ColumnTypes.LINK and not column_data:
+                continue
             column = {
                 'name': column_name,
                 'type': column_type,
                 'data': column_data,
             }
             columns.append(column)
         return columns
```

### Comparing `seatable-api-2.6.6/seatable_api/date_utils.py` & `seatable-api-2.6.7/seatable_api/date_utils.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.6.6/seatable_api/main.py` & `seatable-api-2.6.7/seatable_api/main.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.6.6/seatable_api/message.py` & `seatable-api-2.6.7/seatable_api/message.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.6.6/seatable_api/query.py` & `seatable-api-2.6.7/seatable_api/query.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.6.6/seatable_api/socket_io.py` & `seatable-api-2.6.7/seatable_api/socket_io.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.6.6/seatable_api/utils.py` & `seatable-api-2.6.7/seatable_api/utils.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.6.6/seatable_api.egg-info/PKG-INFO` & `seatable-api-2.6.7/seatable_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seatable-api
-Version: 2.6.6
+Version: 2.6.7
 Summary: Python client for SeaTable web api
 Home-page: https://github.com/seatable/seatable-api-python
 Author: seatable
 Author-email: support@seafile.com
 License: Apache Licence
 Platform: any
 Classifier: Programming Language :: Python
```

### Comparing `seatable-api-2.6.6/seatable_api.egg-info/SOURCES.txt` & `seatable-api-2.6.7/seatable_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seatable-api-2.6.6/setup.py` & `seatable-api-2.6.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-__version__ = '2.6.6'
+__version__ = '2.6.7'
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='seatable-api',
     version=__version__,
```

### Comparing `seatable-api-2.6.6/tests/dateutils_test.py` & `seatable-api-2.6.7/tests/dateutils_test.py`

 * *Files identical despite different names*

