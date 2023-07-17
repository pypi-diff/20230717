# Comparing `tmp/connectors_to_databases-1.0.2.tar.gz` & `tmp/connectors_to_databases-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connectors_to_databases-1.0.2.tar", last modified: Mon Jul 17 07:23:18 2023, max compression
+gzip compressed data, was "connectors_to_databases-1.0.3.tar", last modified: Mon Jul 17 07:27:56 2023, max compression
```

## Comparing `connectors_to_databases-1.0.2.tar` & `connectors_to_databases-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 ivankorsakov   (501) staff       (20)        0 2023-07-17 07:23:18.357943 connectors_to_databases-1.0.2/
--rw-r--r--   0 ivankorsakov   (501) staff       (20)    11347 2023-02-18 06:59:30.000000 connectors_to_databases-1.0.2/LICENSE.MD
--rw-r--r--   0 ivankorsakov   (501) staff       (20)     4166 2023-07-17 07:23:18.357787 connectors_to_databases-1.0.2/PKG-INFO
--rw-r--r--   0 ivankorsakov   (501) staff       (20)     3033 2023-07-17 07:08:57.000000 connectors_to_databases-1.0.2/README.md
-drwxr-xr-x   0 ivankorsakov   (501) staff       (20)        0 2023-07-17 07:23:18.356756 connectors_to_databases-1.0.2/connectors_to_databases/
--rw-r--r--   0 ivankorsakov   (501) staff       (20)     3984 2023-07-17 06:50:16.000000 connectors_to_databases-1.0.2/connectors_to_databases/BaseOperator.py
--rw-r--r--   0 ivankorsakov   (501) staff       (20)     1161 2023-06-03 06:35:40.000000 connectors_to_databases-1.0.2/connectors_to_databases/ClickHouse.py
--rw-r--r--   0 ivankorsakov   (501) staff       (20)     7957 2023-07-17 06:50:16.000000 connectors_to_databases-1.0.2/connectors_to_databases/PostgreSQL.py
--rw-r--r--   0 ivankorsakov   (501) staff       (20)       41 2022-11-15 09:41:17.000000 connectors_to_databases-1.0.2/connectors_to_databases/TypeHinting.py
--rw-r--r--   0 ivankorsakov   (501) staff       (20)      307 2023-07-17 07:23:12.000000 connectors_to_databases-1.0.2/connectors_to_databases/__init__.py
--rw-r--r--   0 ivankorsakov   (501) staff       (20)      480 2023-07-17 06:04:07.000000 connectors_to_databases-1.0.2/connectors_to_databases/class_use.py
-drwxr-xr-x   0 ivankorsakov   (501) staff       (20)        0 2023-07-17 07:23:18.357559 connectors_to_databases-1.0.2/connectors_to_databases.egg-info/
--rw-r--r--   0 ivankorsakov   (501) staff       (20)     4166 2023-07-17 07:23:18.000000 connectors_to_databases-1.0.2/connectors_to_databases.egg-info/PKG-INFO
--rw-r--r--   0 ivankorsakov   (501) staff       (20)      506 2023-07-17 07:23:18.000000 connectors_to_databases-1.0.2/connectors_to_databases.egg-info/SOURCES.txt
--rw-r--r--   0 ivankorsakov   (501) staff       (20)        1 2023-07-17 07:23:18.000000 connectors_to_databases-1.0.2/connectors_to_databases.egg-info/dependency_links.txt
--rw-r--r--   0 ivankorsakov   (501) staff       (20)       81 2023-07-17 07:23:18.000000 connectors_to_databases-1.0.2/connectors_to_databases.egg-info/requires.txt
--rw-r--r--   0 ivankorsakov   (501) staff       (20)       24 2023-07-17 07:23:18.000000 connectors_to_databases-1.0.2/connectors_to_databases.egg-info/top_level.txt
--rw-r--r--   0 ivankorsakov   (501) staff       (20)     1076 2023-07-17 06:54:10.000000 connectors_to_databases-1.0.2/pyproject.toml
--rw-r--r--   0 ivankorsakov   (501) staff       (20)       38 2023-07-17 07:23:18.357984 connectors_to_databases-1.0.2/setup.cfg
--rw-r--r--   0 ivankorsakov   (501) staff       (20)     1689 2023-07-17 07:23:12.000000 connectors_to_databases-1.0.2/setup.py
+drwxr-xr-x   0 ivankorsakov   (501) staff       (20)        0 2023-07-17 07:27:56.232088 connectors_to_databases-1.0.3/
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)    11347 2023-02-18 06:59:30.000000 connectors_to_databases-1.0.3/LICENSE.MD
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)     4166 2023-07-17 07:27:56.231919 connectors_to_databases-1.0.3/PKG-INFO
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)     3033 2023-07-17 07:08:57.000000 connectors_to_databases-1.0.3/README.md
+drwxr-xr-x   0 ivankorsakov   (501) staff       (20)        0 2023-07-17 07:27:56.230916 connectors_to_databases-1.0.3/connectors_to_databases/
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)     3984 2023-07-17 06:50:16.000000 connectors_to_databases-1.0.3/connectors_to_databases/BaseOperator.py
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)     1161 2023-06-03 06:35:40.000000 connectors_to_databases-1.0.3/connectors_to_databases/ClickHouse.py
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)     7957 2023-07-17 07:27:31.000000 connectors_to_databases-1.0.3/connectors_to_databases/PostgreSQL.py
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)       41 2022-11-15 09:41:17.000000 connectors_to_databases-1.0.3/connectors_to_databases/TypeHinting.py
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)      307 2023-07-17 07:27:31.000000 connectors_to_databases-1.0.3/connectors_to_databases/__init__.py
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)      480 2023-07-17 06:04:07.000000 connectors_to_databases-1.0.3/connectors_to_databases/class_use.py
+drwxr-xr-x   0 ivankorsakov   (501) staff       (20)        0 2023-07-17 07:27:56.231693 connectors_to_databases-1.0.3/connectors_to_databases.egg-info/
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)     4166 2023-07-17 07:27:56.000000 connectors_to_databases-1.0.3/connectors_to_databases.egg-info/PKG-INFO
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)      506 2023-07-17 07:27:56.000000 connectors_to_databases-1.0.3/connectors_to_databases.egg-info/SOURCES.txt
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)        1 2023-07-17 07:27:56.000000 connectors_to_databases-1.0.3/connectors_to_databases.egg-info/dependency_links.txt
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)       81 2023-07-17 07:27:56.000000 connectors_to_databases-1.0.3/connectors_to_databases.egg-info/requires.txt
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)       24 2023-07-17 07:27:56.000000 connectors_to_databases-1.0.3/connectors_to_databases.egg-info/top_level.txt
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)     1076 2023-07-17 06:54:10.000000 connectors_to_databases-1.0.3/pyproject.toml
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)       38 2023-07-17 07:27:56.232131 connectors_to_databases-1.0.3/setup.cfg
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)     1689 2023-07-17 07:27:31.000000 connectors_to_databases-1.0.3/setup.py
```

### Comparing `connectors_to_databases-1.0.2/LICENSE.MD` & `connectors_to_databases-1.0.3/LICENSE.MD`

 * *Files identical despite different names*

### Comparing `connectors_to_databases-1.0.2/PKG-INFO` & `connectors_to_databases-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connectors_to_databases
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python module for connect with PostgreSQL and ClickHouse 
 Home-page: https://github.com/k0rsakov/connectors_to_databases
 Download-URL: https://github.com/k0rsakov/connectors_to_databases/archive/refs/heads/main.zip
 Author: k0rsakov
 Author-email: korsakov.iyu@gmail.com
 License: Apache License, Version 2.0, see LICENSE file
 Keywords: database,SQL,PostgreSQL,ClickHouse,dataframe
```

### Comparing `connectors_to_databases-1.0.2/README.md` & `connectors_to_databases-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `connectors_to_databases-1.0.2/connectors_to_databases/BaseOperator.py` & `connectors_to_databases-1.0.3/connectors_to_databases/BaseOperator.py`

 * *Files identical despite different names*

### Comparing `connectors_to_databases-1.0.2/connectors_to_databases/ClickHouse.py` & `connectors_to_databases-1.0.3/connectors_to_databases/ClickHouse.py`

 * *Files identical despite different names*

### Comparing `connectors_to_databases-1.0.2/connectors_to_databases/PostgreSQL.py` & `connectors_to_databases-1.0.3/connectors_to_databases/PostgreSQL.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# from .BaseOperator import BaseOperator
-from connectors_to_databases.BaseOperator import BaseOperator
+from .BaseOperator import BaseOperator
+# from connectors_to_databases.BaseOperator import BaseOperator
 from urllib.parse import quote
 from typing import Union, Iterable
 
 from sqlalchemy import create_engine, engine
 
 
 class PostgreSQL(BaseOperator):
```

### Comparing `connectors_to_databases-1.0.2/connectors_to_databases.egg-info/PKG-INFO` & `connectors_to_databases-1.0.3/connectors_to_databases.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connectors-to-databases
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python module for connect with PostgreSQL and ClickHouse 
 Home-page: https://github.com/k0rsakov/connectors_to_databases
 Download-URL: https://github.com/k0rsakov/connectors_to_databases/archive/refs/heads/main.zip
 Author: k0rsakov
 Author-email: korsakov.iyu@gmail.com
 License: Apache License, Version 2.0, see LICENSE file
 Keywords: database,SQL,PostgreSQL,ClickHouse,dataframe
```

### Comparing `connectors_to_databases-1.0.2/pyproject.toml` & `connectors_to_databases-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `connectors_to_databases-1.0.2/setup.py` & `connectors_to_databases-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from io import open
 from setuptools import setup
 
 
-version = '1.0.2'
+version = '1.0.3'
 
 with open('README.md', encoding='utf-8-sig') as f:
     long_description = f.read()
 
 setup(
     name='connectors_to_databases',
     version=version,
```

