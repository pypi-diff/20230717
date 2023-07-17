# Comparing `tmp/pgsqlx-1.0.2.tar.gz` & `tmp/pgsqlx-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pgsqlx-1.0.2.tar", last modified: Mon Jul 17 10:13:26 2023, max compression
+gzip compressed data, was "dist\pgsqlx-1.0.3.tar", last modified: Mon Jul 17 14:35:37 2023, max compression
```

## Comparing `pgsqlx-1.0.2.tar` & `pgsqlx-1.0.3.tar`

### file list

```diff
@@ -1,23 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 10:13:26.000000 pgsqlx-1.0.2/
--rw-rw-rw-   0        0        0    11558 2023-07-14 14:50:12.000000 pgsqlx-1.0.2/LICENSE
-drwxrwxrwx   0        0        0        0 2023-07-17 10:13:26.000000 pgsqlx-1.0.2/pgsqlx/
--rw-rw-rw-   0        0        0      678 2023-07-15 12:19:37.000000 pgsqlx-1.0.2/pgsqlx/constant.py
--rw-rw-rw-   0        0        0    19259 2023-07-17 09:29:32.000000 pgsqlx-1.0.2/pgsqlx/db.py
--rw-rw-rw-   0        0        0    13886 2023-07-17 09:29:32.000000 pgsqlx-1.0.2/pgsqlx/dbx.py
--rw-rw-rw-   0        0        0     3984 2023-07-13 13:31:18.000000 pgsqlx-1.0.2/pgsqlx/log_support.py
--rw-rw-rw-   0        0        0    37747 2023-07-17 09:02:03.000000 pgsqlx-1.0.2/pgsqlx/orm.py
--rw-rw-rw-   0        0        0     2392 2023-06-26 14:23:12.000000 pgsqlx-1.0.2/pgsqlx/snowflake.py
--rw-rw-rw-   0        0        0     5119 2023-07-14 23:31:12.000000 pgsqlx-1.0.2/pgsqlx/sql_mapper.py
--rw-rw-rw-   0        0        0     6487 2023-07-17 09:30:08.000000 pgsqlx-1.0.2/pgsqlx/support.py
--rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 pgsqlx-1.0.2/pgsqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 10:13:26.000000 pgsqlx-1.0.2/pgsqlx.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-17 10:13:26.000000 pgsqlx-1.0.2/pgsqlx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-15 04:29:07.000000 pgsqlx-1.0.2/pgsqlx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     4292 2023-07-17 10:13:26.000000 pgsqlx-1.0.2/pgsqlx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       30 2023-07-17 10:13:26.000000 pgsqlx-1.0.2/pgsqlx.egg-info/requires.txt
--rw-rw-rw-   0        0        0      365 2023-07-17 10:13:26.000000 pgsqlx-1.0.2/pgsqlx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-07-17 10:13:26.000000 pgsqlx-1.0.2/pgsqlx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4292 2023-07-17 10:13:26.000000 pgsqlx-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3758 2023-07-16 02:24:38.000000 pgsqlx-1.0.2/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-17 10:13:26.000000 pgsqlx-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1204 2023-07-17 10:12:52.000000 pgsqlx-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 14:35:37.000000 pgsqlx-1.0.3/
+drwxrwxrwx   0        0        0        0 2023-07-17 14:35:37.000000 pgsqlx-1.0.3/pgsqlx/
+-rw-rw-rw-   0        0        0      678 2023-07-15 12:19:37.000000 pgsqlx-1.0.3/pgsqlx/constant.py
+-rw-rw-rw-   0        0        0    19259 2023-07-17 09:29:32.000000 pgsqlx-1.0.3/pgsqlx/db.py
+-rw-rw-rw-   0        0        0    13886 2023-07-17 09:29:32.000000 pgsqlx-1.0.3/pgsqlx/dbx.py
+-rw-rw-rw-   0        0        0     3984 2023-07-13 13:31:18.000000 pgsqlx-1.0.3/pgsqlx/log_support.py
+-rw-rw-rw-   0        0        0    37747 2023-07-17 09:02:03.000000 pgsqlx-1.0.3/pgsqlx/orm.py
+-rw-rw-rw-   0        0        0     2392 2023-06-26 14:23:12.000000 pgsqlx-1.0.3/pgsqlx/snowflake.py
+-rw-rw-rw-   0        0        0     5119 2023-07-14 23:31:12.000000 pgsqlx-1.0.3/pgsqlx/sql_mapper.py
+-rw-rw-rw-   0        0        0     6487 2023-07-17 09:30:08.000000 pgsqlx-1.0.3/pgsqlx/support.py
+-rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 pgsqlx-1.0.3/pgsqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 14:35:37.000000 pgsqlx-1.0.3/pgsqlx.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-17 14:35:37.000000 pgsqlx-1.0.3/pgsqlx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-17 14:35:37.000000 pgsqlx-1.0.3/pgsqlx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     4268 2023-07-17 14:35:37.000000 pgsqlx-1.0.3/pgsqlx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2023-07-17 14:35:37.000000 pgsqlx-1.0.3/pgsqlx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      357 2023-07-17 14:35:37.000000 pgsqlx-1.0.3/pgsqlx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-07-17 14:35:37.000000 pgsqlx-1.0.3/pgsqlx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4268 2023-07-17 14:35:37.000000 pgsqlx-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3758 2023-07-16 02:24:38.000000 pgsqlx-1.0.3/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-17 14:35:37.000000 pgsqlx-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1203 2023-07-17 14:35:33.000000 pgsqlx-1.0.3/setup.py
```

### Comparing `pgsqlx-1.0.2/pgsqlx/constant.py` & `pgsqlx-1.0.3/pgsqlx/constant.py`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.0.2/pgsqlx/db.py` & `pgsqlx-1.0.3/pgsqlx/db.py`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.0.2/pgsqlx/dbx.py` & `pgsqlx-1.0.3/pgsqlx/dbx.py`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.0.2/pgsqlx/log_support.py` & `pgsqlx-1.0.3/pgsqlx/log_support.py`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.0.2/pgsqlx/orm.py` & `pgsqlx-1.0.3/pgsqlx/orm.py`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.0.2/pgsqlx/snowflake.py` & `pgsqlx-1.0.3/pgsqlx/snowflake.py`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.0.2/pgsqlx/sql_mapper.py` & `pgsqlx-1.0.3/pgsqlx/sql_mapper.py`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.0.2/pgsqlx/support.py` & `pgsqlx-1.0.3/pgsqlx/support.py`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.0.2/pgsqlx.egg-info/PKG-INFO` & `pgsqlx-1.0.3/pgsqlx.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: pgsqlx
-Version: 1.0.2
+Version: 1.0.3
 Summary: PgSqlx is a simple python sql executor for PostgreSQL like MyBatis.
 Home-page: https://gitee.com/summry/pgsqlx
-Author: summry
+Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 Mapper file
 '''''''''''
 
 Create a mapper file in 'mapper' folder, you can named
 'person_mapper.xml', like follow:
```

### Comparing `pgsqlx-1.0.2/PKG-INFO` & `pgsqlx-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: pgsqlx
-Version: 1.0.2
+Version: 1.0.3
 Summary: PgSqlx is a simple python sql executor for PostgreSQL like MyBatis.
 Home-page: https://gitee.com/summry/pgsqlx
-Author: summry
+Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 Mapper file
 '''''''''''
 
 Create a mapper file in 'mapper' folder, you can named
 'person_mapper.xml', like follow:
```

### Comparing `pgsqlx-1.0.2/README.rst` & `pgsqlx-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.0.2/setup.py` & `pgsqlx-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,17 @@
     description="PgSqlx is a simple python sql executor for PostgreSQL like MyBatis.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'Jinja2>=2.7.0',
         'psycopg2>=2.7.4',
     ],
-    version='1.0.2',
+    version='1.0.3',
     url='https://gitee.com/summry/pgsqlx',
-    author='summry',
+    author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'PostgreSQL', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
     },
     include_package_data=True,
```

