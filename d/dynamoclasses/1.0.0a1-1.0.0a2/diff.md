# Comparing `tmp/dynamoclasses-1.0.0a1.tar.gz` & `tmp/dynamoclasses-1.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dynamoclasses-1.0.0a1.tar", last modified: Tue Apr  3 21:14:19 2018, max compression
+gzip compressed data, was "dist/dynamoclasses-1.0.0a2.tar", last modified: Mon Jul 17 13:09:31 2023, max compression
```

## Comparing `dynamoclasses-1.0.0a1.tar` & `dynamoclasses-1.0.0a2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 ewdurbin   (501) staff       (20)        0 2018-04-03 21:14:18.000000 dynamoclasses-1.0.0a1/
--rw-r--r--   0 ewdurbin   (501) staff       (20)     2281 2018-04-03 21:14:18.000000 dynamoclasses-1.0.0a1/PKG-INFO
-drwxr-xr-x   0 ewdurbin   (501) staff       (20)        0 2018-04-03 21:14:18.000000 dynamoclasses-1.0.0a1/dynamoclasses.egg-info/
--rw-r--r--   0 ewdurbin   (501) staff       (20)     2281 2018-04-03 21:14:18.000000 dynamoclasses-1.0.0a1/dynamoclasses.egg-info/PKG-INFO
--rw-r--r--   0 ewdurbin   (501) staff       (20)      310 2018-04-03 21:14:18.000000 dynamoclasses-1.0.0a1/dynamoclasses.egg-info/SOURCES.txt
--rw-r--r--   0 ewdurbin   (501) staff       (20)       31 2018-04-03 21:14:18.000000 dynamoclasses-1.0.0a1/dynamoclasses.egg-info/requires.txt
--rw-r--r--   0 ewdurbin   (501) staff       (20)       14 2018-04-03 21:14:18.000000 dynamoclasses-1.0.0a1/dynamoclasses.egg-info/top_level.txt
--rw-r--r--   0 ewdurbin   (501) staff       (20)        1 2018-04-03 21:14:18.000000 dynamoclasses-1.0.0a1/dynamoclasses.egg-info/dependency_links.txt
--rw-r--r--   0 ewdurbin   (501) staff       (20)     1297 2018-04-03 21:11:44.000000 dynamoclasses-1.0.0a1/README.md
-drwxr-xr-x   0 ewdurbin   (501) staff       (20)        0 2018-04-03 21:14:18.000000 dynamoclasses-1.0.0a1/dynamoclasses/
-drwxr-xr-x   0 ewdurbin   (501) staff       (20)        0 2018-04-03 21:14:18.000000 dynamoclasses-1.0.0a1/dynamoclasses/test/
--rw-r--r--   0 ewdurbin   (501) staff       (20)     2555 2018-04-03 19:42:17.000000 dynamoclasses-1.0.0a1/dynamoclasses/test/test_dynamoclasses.py
--rw-r--r--   0 ewdurbin   (501) staff       (20)        0 2018-04-02 17:45:06.000000 dynamoclasses-1.0.0a1/dynamoclasses/test/__init__.py
--rw-r--r--   0 ewdurbin   (501) staff       (20)     4090 2018-04-03 21:11:46.000000 dynamoclasses-1.0.0a1/dynamoclasses/__init__.py
--rw-r--r--   0 ewdurbin   (501) staff       (20)     1274 2018-04-03 21:12:52.000000 dynamoclasses-1.0.0a1/setup.py
--rw-r--r--   0 ewdurbin   (501) staff       (20)       67 2018-04-03 21:14:18.000000 dynamoclasses-1.0.0a1/setup.cfg
+drwxr-xr-x   0 ee         (501) staff       (20)        0 2023-07-17 13:09:31.000000 dynamoclasses-1.0.0a2/
+-rw-r--r--   0 ee         (501) staff       (20)     2270 2023-07-17 13:09:31.000000 dynamoclasses-1.0.0a2/PKG-INFO
+drwxr-xr-x   0 ee         (501) staff       (20)        0 2023-07-17 13:09:31.000000 dynamoclasses-1.0.0a2/dynamoclasses.egg-info/
+-rw-r--r--   0 ee         (501) staff       (20)     2270 2023-07-17 13:09:31.000000 dynamoclasses-1.0.0a2/dynamoclasses.egg-info/PKG-INFO
+-rw-r--r--   0 ee         (501) staff       (20)      310 2023-07-17 13:09:31.000000 dynamoclasses-1.0.0a2/dynamoclasses.egg-info/SOURCES.txt
+-rw-r--r--   0 ee         (501) staff       (20)       31 2023-07-17 13:09:31.000000 dynamoclasses-1.0.0a2/dynamoclasses.egg-info/requires.txt
+-rw-r--r--   0 ee         (501) staff       (20)       14 2023-07-17 13:09:31.000000 dynamoclasses-1.0.0a2/dynamoclasses.egg-info/top_level.txt
+-rw-r--r--   0 ee         (501) staff       (20)        1 2023-07-17 13:09:31.000000 dynamoclasses-1.0.0a2/dynamoclasses.egg-info/dependency_links.txt
+-rw-r--r--   0 ee         (501) staff       (20)     1297 2023-07-17 13:07:55.000000 dynamoclasses-1.0.0a2/README.md
+drwxr-xr-x   0 ee         (501) staff       (20)        0 2023-07-17 13:09:31.000000 dynamoclasses-1.0.0a2/dynamoclasses/
+drwxr-xr-x   0 ee         (501) staff       (20)        0 2023-07-17 13:09:31.000000 dynamoclasses-1.0.0a2/dynamoclasses/test/
+-rw-r--r--   0 ee         (501) staff       (20)     2555 2023-07-17 13:07:55.000000 dynamoclasses-1.0.0a2/dynamoclasses/test/test_dynamoclasses.py
+-rw-r--r--   0 ee         (501) staff       (20)        0 2023-07-17 13:07:55.000000 dynamoclasses-1.0.0a2/dynamoclasses/test/__init__.py
+-rw-r--r--   0 ee         (501) staff       (20)     4085 2023-07-17 13:07:55.000000 dynamoclasses-1.0.0a2/dynamoclasses/__init__.py
+-rw-r--r--   0 ee         (501) staff       (20)     1263 2023-07-17 13:08:23.000000 dynamoclasses-1.0.0a2/setup.py
+-rw-r--r--   0 ee         (501) staff       (20)       67 2023-07-17 13:09:31.000000 dynamoclasses-1.0.0a2/setup.cfg
```

### Comparing `dynamoclasses-1.0.0a1/PKG-INFO` & `dynamoclasses-1.0.0a2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: dynamoclasses
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: DynamoDB ORM using dataclasses
 Home-page: https://github.com/ewdurbin/dynamoclasses
-Author: Ernest W. Durbin III
+Author: Ee Durbin
 Author-email: ewdurbin@gmail.com
 License: UNKNOWN
-Project-URL: Bug Reports, https://github.com/ewdurbin/dynamoclasses/issues
 Project-URL: Source, https://github.com/ewdurbin/dynamoclasses/
+Project-URL: Bug Reports, https://github.com/ewdurbin/dynamoclasses/issues
 Description: DynamoClasses
         =============
         
         API interface for [Amazon Web Services DynamoDB](https://aws.amazon.com/dynamodb/) built on top of [PEP 557 Data Classes](https://www.python.org/dev/peps/pep-0557/).
         
         The goal is to have something that is fully a `dataclass` class, but gets some helpers bolted on allowing for retrieving/storing the objects in DynamoDB.
```

### Comparing `dynamoclasses-1.0.0a1/dynamoclasses.egg-info/PKG-INFO` & `dynamoclasses-1.0.0a2/dynamoclasses.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: dynamoclasses
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: DynamoDB ORM using dataclasses
 Home-page: https://github.com/ewdurbin/dynamoclasses
-Author: Ernest W. Durbin III
+Author: Ee Durbin
 Author-email: ewdurbin@gmail.com
 License: UNKNOWN
-Project-URL: Bug Reports, https://github.com/ewdurbin/dynamoclasses/issues
 Project-URL: Source, https://github.com/ewdurbin/dynamoclasses/
+Project-URL: Bug Reports, https://github.com/ewdurbin/dynamoclasses/issues
 Description: DynamoClasses
         =============
         
         API interface for [Amazon Web Services DynamoDB](https://aws.amazon.com/dynamodb/) built on top of [PEP 557 Data Classes](https://www.python.org/dev/peps/pep-0557/).
         
         The goal is to have something that is fully a `dataclass` class, but gets some helpers bolted on allowing for retrieving/storing the objects in DynamoDB.
```

### Comparing `dynamoclasses-1.0.0a1/README.md` & `dynamoclasses-1.0.0a2/README.md`

 * *Files identical despite different names*

### Comparing `dynamoclasses-1.0.0a1/dynamoclasses/test/test_dynamoclasses.py` & `dynamoclasses-1.0.0a2/dynamoclasses/test/test_dynamoclasses.py`

 * *Files identical despite different names*

### Comparing `dynamoclasses-1.0.0a1/dynamoclasses/__init__.py` & `dynamoclasses-1.0.0a2/dynamoclasses/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 TYPE_MAPPING = {
     str: {"key": "S", "fn": lambda x: str(x)},
     float: {"key": "N", "fn": lambda x: str(x)},
     int: {"key": "N", "fn": lambda x: str(x)},
     bytes: {"key": "B", "fn": lambda x: str(x)},
-    dict: {"key": "M", "fn": lambda x: str(x)},
+    dict: {"key": "M", "fn": lambda x: x},
     bool: {"key": "BOOL", "fn": lambda x: x},
     None: {"key": "NULL", "fn": lambda x: x},
 }
 
 
 def _process_class(
     cls, *, table_name, partition_key_name, sort_key_name, data_class_kwargs
```

### Comparing `dynamoclasses-1.0.0a1/setup.py` & `dynamoclasses-1.0.0a2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 
 # Get the long description from the README file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='dynamoclasses',
-    version='1.0.0a1',
+    version='1.0.0a2',
     description='DynamoDB ORM using dataclasses',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/ewdurbin/dynamoclasses',
-    author='Ernest W. Durbin III',
+    author='Ee Durbin',
     author_email='ewdurbin@gmail.com',
 
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Programming Language :: Python :: 3.7',
     ],
```

