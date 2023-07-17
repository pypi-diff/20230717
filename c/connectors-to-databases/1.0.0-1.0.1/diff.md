# Comparing `tmp/connectors_to_databases-1.0.0.tar.gz` & `tmp/connectors_to_databases-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connectors_to_databases-1.0.0.tar", last modified: Sun Feb 19 06:48:00 2023, max compression
+gzip compressed data, was "connectors_to_databases-1.0.1.tar", last modified: Mon Jul 17 07:15:57 2023, max compression
```

## Comparing `connectors_to_databases-1.0.0.tar` & `connectors_to_databases-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 ivankorsakov   (501) staff       (20)        0 2023-02-19 06:48:00.386144 connectors_to_databases-1.0.0/
--rw-r--r--   0 ivankorsakov   (501) staff       (20)    11347 2023-02-18 06:59:30.000000 connectors_to_databases-1.0.0/LICENSE.MD
--rw-r--r--   0 ivankorsakov   (501) staff       (20)     4192 2023-02-19 06:48:00.385914 connectors_to_databases-1.0.0/PKG-INFO
--rw-r--r--   0 ivankorsakov   (501) staff       (20)     2987 2023-02-18 07:09:33.000000 connectors_to_databases-1.0.0/README.md
-drwxr-xr-x   0 ivankorsakov   (501) staff       (20)        0 2023-02-19 06:48:00.383785 connectors_to_databases-1.0.0/connectors_to_databases/
--rw-r--r--   0 ivankorsakov   (501) staff       (20)     3616 2023-02-18 05:45:48.000000 connectors_to_databases-1.0.0/connectors_to_databases/BaseOperator.py
--rw-r--r--   0 ivankorsakov   (501) staff       (20)     1108 2023-02-18 07:09:33.000000 connectors_to_databases-1.0.0/connectors_to_databases/ClickHouse.py
--rw-r--r--   0 ivankorsakov   (501) staff       (20)     2801 2023-02-18 05:51:36.000000 connectors_to_databases-1.0.0/connectors_to_databases/PostgreSQL.py
--rw-r--r--   0 ivankorsakov   (501) staff       (20)       41 2022-11-15 09:41:17.000000 connectors_to_databases-1.0.0/connectors_to_databases/TypeHinting.py
--rw-r--r--   0 ivankorsakov   (501) staff       (20)      301 2023-02-19 06:37:50.000000 connectors_to_databases-1.0.0/connectors_to_databases/__init__.py
-drwxr-xr-x   0 ivankorsakov   (501) staff       (20)        0 2023-02-19 06:48:00.384864 connectors_to_databases-1.0.0/connectors_to_databases.egg-info/
--rw-r--r--   0 ivankorsakov   (501) staff       (20)     4192 2023-02-19 06:48:00.000000 connectors_to_databases-1.0.0/connectors_to_databases.egg-info/PKG-INFO
--rw-r--r--   0 ivankorsakov   (501) staff       (20)      454 2023-02-19 06:48:00.000000 connectors_to_databases-1.0.0/connectors_to_databases.egg-info/SOURCES.txt
--rw-r--r--   0 ivankorsakov   (501) staff       (20)        1 2023-02-19 06:48:00.000000 connectors_to_databases-1.0.0/connectors_to_databases.egg-info/dependency_links.txt
--rw-r--r--   0 ivankorsakov   (501) staff       (20)       73 2023-02-19 06:48:00.000000 connectors_to_databases-1.0.0/connectors_to_databases.egg-info/requires.txt
--rw-r--r--   0 ivankorsakov   (501) staff       (20)       24 2023-02-19 06:48:00.000000 connectors_to_databases-1.0.0/connectors_to_databases.egg-info/top_level.txt
--rw-r--r--   0 ivankorsakov   (501) staff       (20)       38 2023-02-19 06:48:00.386224 connectors_to_databases-1.0.0/setup.cfg
--rw-r--r--   0 ivankorsakov   (501) staff       (20)     1714 2023-02-19 06:42:24.000000 connectors_to_databases-1.0.0/setup.py
+drwxr-xr-x   0 ivankorsakov   (501) staff       (20)        0 2023-07-17 07:15:57.678553 connectors_to_databases-1.0.1/
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)    11347 2023-02-18 06:59:30.000000 connectors_to_databases-1.0.1/LICENSE.MD
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)     4166 2023-07-17 07:15:57.678401 connectors_to_databases-1.0.1/PKG-INFO
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)     3033 2023-07-17 07:08:57.000000 connectors_to_databases-1.0.1/README.md
+drwxr-xr-x   0 ivankorsakov   (501) staff       (20)        0 2023-07-17 07:15:57.677496 connectors_to_databases-1.0.1/connectors_to_databases/
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)     3984 2023-07-17 06:50:16.000000 connectors_to_databases-1.0.1/connectors_to_databases/BaseOperator.py
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)     1161 2023-06-03 06:35:40.000000 connectors_to_databases-1.0.1/connectors_to_databases/ClickHouse.py
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)     7957 2023-07-17 06:50:16.000000 connectors_to_databases-1.0.1/connectors_to_databases/PostgreSQL.py
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)       41 2022-11-15 09:41:17.000000 connectors_to_databases-1.0.1/connectors_to_databases/TypeHinting.py
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)      313 2023-07-17 06:46:10.000000 connectors_to_databases-1.0.1/connectors_to_databases/__init__.py
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)      480 2023-07-17 06:04:07.000000 connectors_to_databases-1.0.1/connectors_to_databases/class_use.py
+drwxr-xr-x   0 ivankorsakov   (501) staff       (20)        0 2023-07-17 07:15:57.678204 connectors_to_databases-1.0.1/connectors_to_databases.egg-info/
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)     4166 2023-07-17 07:15:57.000000 connectors_to_databases-1.0.1/connectors_to_databases.egg-info/PKG-INFO
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)      506 2023-07-17 07:15:57.000000 connectors_to_databases-1.0.1/connectors_to_databases.egg-info/SOURCES.txt
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)        1 2023-07-17 07:15:57.000000 connectors_to_databases-1.0.1/connectors_to_databases.egg-info/dependency_links.txt
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)       81 2023-07-17 07:15:57.000000 connectors_to_databases-1.0.1/connectors_to_databases.egg-info/requires.txt
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)       24 2023-07-17 07:15:57.000000 connectors_to_databases-1.0.1/connectors_to_databases.egg-info/top_level.txt
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)     1076 2023-07-17 06:54:10.000000 connectors_to_databases-1.0.1/pyproject.toml
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)       38 2023-07-17 07:15:57.678601 connectors_to_databases-1.0.1/setup.cfg
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)     1689 2023-07-17 06:52:13.000000 connectors_to_databases-1.0.1/setup.py
```

### Comparing `connectors_to_databases-1.0.0/LICENSE.MD` & `connectors_to_databases-1.0.1/LICENSE.MD`

 * *Files identical despite different names*

### Comparing `connectors_to_databases-1.0.0/PKG-INFO` & `connectors_to_databases-1.0.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 Metadata-Version: 2.1
 Name: connectors_to_databases
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python module for connect with PostgreSQL and ClickHouse 
 Home-page: https://github.com/k0rsakov/connectors_to_databases
 Download-URL: https://github.com/k0rsakov/connectors_to_databases/archive/refs/heads/main.zip
 Author: k0rsakov
 Author-email: korsakov.iyu@gmail.com
 License: Apache License, Version 2.0, see LICENSE file
+Keywords: database,SQL,PostgreSQL,ClickHouse,dataframe
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python :: Implementation :: CPython
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.MD
 
 # Connector to databases
 
 ![PyPI](https://img.shields.io/pypi/v/connectors-to-databases?color=blueviolet) 
-![Python 3.6, 3.7, 3.8, 3.9, 3.10, 3.11](https://img.shields.io/pypi/pyversions/clubhouse?color=blueviolet)
+![Python 3, 3.10, 3.11](https://img.shields.io/pypi/pyversions/clubhouse?color=blueviolet)
 ![License](https://img.shields.io/pypi/l/connectors-to-databases?color=blueviolet) 
 
 **Connector to databases** – easy package for connect with database 
 [PostgreSQL](https://github.com/postgres/postgres) and 
 [ClickHouse](https://github.com/ClickHouse/ClickHouse)
 
 ## Installation
@@ -65,27 +64,33 @@
     port=0,
     database='main',
     login='admin',
     password='admin',
 )
 ```
 
+### Check connection to database
+
+```python
+pg.check_connection()
+```
+
 ### Creating a table for examples
 
 ```python
 pg.execute_script('CREATE TABLE simple_ (id int4)')
 ```
 
 ### Filling the table with data
 
 ```python
 # simple pd.DataFrame
 df = pd.DataFrame(data={'id':[1]})
 
-pg.into_pg_table(
+pg.insert_df(
     df=df,
     pg_table_name='simple_'
 )
 ```
 
 ### Getting data from a table
 
@@ -151,15 +156,15 @@
 
 ### Filling the table with data
 
 ```python
 # simple pd.DataFrame
 df = ch.DataFrame(data={'value':[1]})
 
-ch.into_pg_table(
+ch.insert_df(
     df=df,
     pg_table_name='test'
 )
 ```
 
 ### Getting data from a table
```

### Comparing `connectors_to_databases-1.0.0/README.md` & `connectors_to_databases-1.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Connector to databases
 
 ![PyPI](https://img.shields.io/pypi/v/connectors-to-databases?color=blueviolet) 
-![Python 3.6, 3.7, 3.8, 3.9, 3.10, 3.11](https://img.shields.io/pypi/pyversions/clubhouse?color=blueviolet)
+![Python 3, 3.10, 3.11](https://img.shields.io/pypi/pyversions/clubhouse?color=blueviolet)
 ![License](https://img.shields.io/pypi/l/connectors-to-databases?color=blueviolet) 
 
 **Connector to databases** – easy package for connect with database 
 [PostgreSQL](https://github.com/postgres/postgres) and 
 [ClickHouse](https://github.com/ClickHouse/ClickHouse)
 
 ## Installation
@@ -39,27 +39,33 @@
     port=0,
     database='main',
     login='admin',
     password='admin',
 )
 ```
 
+### Check connection to database
+
+```python
+pg.check_connection()
+```
+
 ### Creating a table for examples
 
 ```python
 pg.execute_script('CREATE TABLE simple_ (id int4)')
 ```
 
 ### Filling the table with data
 
 ```python
 # simple pd.DataFrame
 df = pd.DataFrame(data={'id':[1]})
 
-pg.into_pg_table(
+pg.insert_df(
     df=df,
     pg_table_name='simple_'
 )
 ```
 
 ### Getting data from a table
 
@@ -125,15 +131,15 @@
 
 ### Filling the table with data
 
 ```python
 # simple pd.DataFrame
 df = ch.DataFrame(data={'value':[1]})
 
-ch.into_pg_table(
+ch.insert_df(
     df=df,
     pg_table_name='test'
 )
 ```
 
 ### Getting data from a table
```

### Comparing `connectors_to_databases-1.0.0/connectors_to_databases/BaseOperator.py` & `connectors_to_databases-1.0.1/connectors_to_databases/BaseOperator.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,84 +28,100 @@
         """
         self._host = host
         self._database = database
         self._login = login
         self._password = password
         self._port = port
 
-    def _authorization_pg(self) -> engine.base.Engine:
+    def _authorization_database(self) -> engine.base.Engine:
         """
         Creating connector engine to database PostgreSQL.
         """
 
         engine_str = f'base://' \
-                     f'{self._login}:%s@{self._host}:{self._port}/' \
-                     f'{self._database}' % quote(self._password)
+                     f'{self._login}:{quote(self._password)}@{self._host}:{self._port}/' \
+                     f'{self._database}'
 
         return create_engine(engine_str)
 
-    def insert_df(self,
-                  df: pd.DataFrame = None,
-                  pg_table_name: str = None,
-                  pg_table_schema: str = None,
-                  chunksize: Union[int, None] = 10024,
-                  index: bool = False,
-                  if_exists: str = 'append',
-                  ) -> Union[None, Exception]:
+    def insert_df(
+            self,
+            df: pd.DataFrame = None,
+            table_name: str = None,
+            table_schema: str = None,
+            chunksize: Union[int, None] = 10024,
+            index: bool = False,
+            if_exists: str = 'append',
+    ) -> Union[None, Exception]:
         """
         Inserting data from dataframe to database.
 
         :param df: dataframe with data; default None.
-        :param pg_table_name: name of table; default None.
-        :param pg_table_schema: name of schema; default None.
+        :param table_name: name of table; default None.
+        :param table_schema: name of schema; default None.
         :param chunksize: Specify the number of rows in each batch to be written at a time.
-            By default, all rows will be written at once.
+            By default, all rows will be written at once; default `10024`.
         :param if_exists: {'fail', 'replace', 'append'}, default 'append'
             How to behave if the table already exists.
 
             * fail: Raise a ValueError.
             * replace: Drop the table before inserting new values.
             * append: Insert new values to the existing table.
         :param index: Write DataFrame index as a column. Uses `index_label` as the column
             name in the table.
         """
 
         df.to_sql(
-            name=pg_table_name,
-            schema=pg_table_schema,
-            con=self._authorization_pg(),
+            name=table_name,
+            schema=table_schema,
+            con=self._authorization_database(),
             chunksize=chunksize,
             index=index,
             if_exists=if_exists,
         )
 
     def execute_to_df(
             self,
             sql_query: str = SQLQuery,
     ) -> Union[pd.DataFrame, Exception]:
         """
         Getting data from database with SQL-query.
 
-        :param sql_query:str: SQL-query; default ''.
-        :return:pd.DataFrame: dataframe with data from database
+        :param sql_query; default `''`.
+        :return: DataFrame with data from database.
         """
 
-        return pd.read_sql(sql_query, self._authorization_pg())
+        return pd.read_sql(
+            sql=sql_query,
+            con=self._authorization_database(),
+        )
 
-    def execute_script(self,
-                       manual_sql_script: SQLQuery):
+    def execute_script(
+            self,
+            manual_sql_script: SQLQuery
+    ) -> None:
         """
         Execute manual scripts (INSERT, TRUNCATE, DROP, CREATE, etc). Other than SELECT
 
-        :param manual_sql_script:SQLQuery: `str` query with manual script
-        :return:
+        :param manual_sql_script: query with manual script; default `''`.
+        :return: None.
         """
-        self._authorization_pg().execute(manual_sql_script)
+        self._authorization_database().execute(manual_sql_script)
 
     def get_uri(self) -> engine.base.Engine:
         """
-        Get connector for manual manipulation with connect to database
+        Get connector for manual manipulation with connect to database.
 
         :return engine.base.Engine:
         """
 
-        return self._authorization_pg()
+        return self._authorization_database()
+
+    def check_connection_to_database(self) -> Union[bool, Exception]:
+        """
+        Method to check connection to database.
+
+        :return: boolean True, if connection to database is successful, Exception otherwise.
+        """
+        df = self.execute_to_df('SELECT 1 AS ONE')
+
+        return bool(isinstance(df, pd.DataFrame))
```

### Comparing `connectors_to_databases-1.0.0/connectors_to_databases/ClickHouse.py` & `connectors_to_databases-1.0.1/connectors_to_databases/ClickHouse.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from urllib.parse import quote
 
 from sqlalchemy import create_engine, engine
 
 from .BaseOperator import BaseOperator
 
+# TODO: Change sqlalchemy to clickhouse-driver
 
 class ClickHouse(BaseOperator):
     """
     Connector to PostgreSQL database
     """
     def __init__(
             self,
@@ -24,15 +25,15 @@
         """
         super().__init__(host, port, login, password)
         self._host = host
         self._login = login
         self._password = password
         self._port = port
 
-    def _authorization_pg(self) -> engine.base.Engine:
+    def _authorization_database(self) -> engine.base.Engine:
         """
         Creating connector engine to database ClickHouse.
         """
 
         engine_str = f'clickhouse://{self._login}:{quote(self._password)}@{self._host}:{self._port}/default'
 
         return create_engine(engine_str)
```

### Comparing `connectors_to_databases-1.0.0/connectors_to_databases.egg-info/PKG-INFO` & `connectors_to_databases-1.0.1/connectors_to_databases.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 Metadata-Version: 2.1
 Name: connectors-to-databases
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python module for connect with PostgreSQL and ClickHouse 
 Home-page: https://github.com/k0rsakov/connectors_to_databases
 Download-URL: https://github.com/k0rsakov/connectors_to_databases/archive/refs/heads/main.zip
 Author: k0rsakov
 Author-email: korsakov.iyu@gmail.com
 License: Apache License, Version 2.0, see LICENSE file
+Keywords: database,SQL,PostgreSQL,ClickHouse,dataframe
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python :: Implementation :: CPython
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.MD
 
 # Connector to databases
 
 ![PyPI](https://img.shields.io/pypi/v/connectors-to-databases?color=blueviolet) 
-![Python 3.6, 3.7, 3.8, 3.9, 3.10, 3.11](https://img.shields.io/pypi/pyversions/clubhouse?color=blueviolet)
+![Python 3, 3.10, 3.11](https://img.shields.io/pypi/pyversions/clubhouse?color=blueviolet)
 ![License](https://img.shields.io/pypi/l/connectors-to-databases?color=blueviolet) 
 
 **Connector to databases** – easy package for connect with database 
 [PostgreSQL](https://github.com/postgres/postgres) and 
 [ClickHouse](https://github.com/ClickHouse/ClickHouse)
 
 ## Installation
@@ -65,27 +64,33 @@
     port=0,
     database='main',
     login='admin',
     password='admin',
 )
 ```
 
+### Check connection to database
+
+```python
+pg.check_connection()
+```
+
 ### Creating a table for examples
 
 ```python
 pg.execute_script('CREATE TABLE simple_ (id int4)')
 ```
 
 ### Filling the table with data
 
 ```python
 # simple pd.DataFrame
 df = pd.DataFrame(data={'id':[1]})
 
-pg.into_pg_table(
+pg.insert_df(
     df=df,
     pg_table_name='simple_'
 )
 ```
 
 ### Getting data from a table
 
@@ -151,15 +156,15 @@
 
 ### Filling the table with data
 
 ```python
 # simple pd.DataFrame
 df = ch.DataFrame(data={'value':[1]})
 
-ch.into_pg_table(
+ch.insert_df(
     df=df,
     pg_table_name='test'
 )
 ```
 
 ### Getting data from a table
```

