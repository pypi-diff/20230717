# Comparing `tmp/External-User-Local-0.0.8.tar.gz` & `tmp/External-user-local-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "External-User-Local-0.0.8.tar", last modified: Mon Jul 10 18:43:22 2023, max compression
+gzip compressed data, was "External-user-local-0.0.9.tar", last modified: Mon Jul 17 10:41:20 2023, max compression
```

## Comparing `External-User-Local-0.0.8.tar` & `External-user-local-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:43:22.512585 External-User-Local-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:43:22.512585 External-User-Local-0.0.8/External_User_Local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-10 18:43:22.000000 External-User-Local-0.0.8/External_User_Local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-10 18:43:22.000000 External-User-Local-0.0.8/External_User_Local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 18:43:22.000000 External-User-Local-0.0.8/External_User_Local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-10 18:43:22.000000 External-User-Local-0.0.8/External_User_Local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-10 18:43:22.512585 External-User-Local-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-10 18:43:07.000000 External-User-Local-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:43:22.512585 External-User-Local-0.0.8/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 18:43:07.000000 External-User-Local-0.0.8/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-10 18:43:07.000000 External-User-Local-0.0.8/db/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-07-10 18:43:07.000000 External-User-Local-0.0.8/db/library_DB.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 18:43:22.512585 External-User-Local-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-10 18:43:07.000000 External-User-Local-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:43:22.512585 External-User-Local-0.0.8/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 18:43:07.000000 External-User-Local-0.0.8/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-07-10 18:43:07.000000 External-User-Local-0.0.8/src/library.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:43:22.512585 External-User-Local-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-10 18:43:07.000000 External-User-Local-0.0.8/tests/test_insertExternal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:41:20.732241 External-user-local-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:41:20.732241 External-user-local-0.0.9/External_user_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-17 10:41:20.000000 External-user-local-0.0.9/External_user_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-17 10:41:20.000000 External-user-local-0.0.9/External_user_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 10:41:20.000000 External-user-local-0.0.9/External_user_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-17 10:41:20.000000 External-user-local-0.0.9/External_user_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-17 10:41:20.732241 External-user-local-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-17 10:41:04.000000 External-user-local-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:41:20.732241 External-user-local-0.0.9/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 10:41:04.000000 External-user-local-0.0.9/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-17 10:41:04.000000 External-user-local-0.0.9/db/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-07-17 10:41:04.000000 External-user-local-0.0.9/db/library_DB.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 10:41:20.732241 External-user-local-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-17 10:41:04.000000 External-user-local-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:41:20.732241 External-user-local-0.0.9/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 10:41:04.000000 External-user-local-0.0.9/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-17 10:41:04.000000 External-user-local-0.0.9/src/library.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:41:20.732241 External-user-local-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-17 10:41:04.000000 External-user-local-0.0.9/tests/test_insertExternal.py
```

### Comparing `External-User-Local-0.0.8/README.md` & `External-user-local-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `External-User-Local-0.0.8/db/library_DB.py` & `External-user-local-0.0.9/db/library_DB.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import os
 import dotenv 
-from LoggerLocalPythonPackage.LoggerServiceSingleton import LoggerServiceSingleton
+from LoggerLocalPythonPackage.LocalLogger import _Local_Logger
 import mysql.connector
 dotenv.load_dotenv()
 from config import db_connection
-logger_serv=LoggerServiceSingleton()
-Local_Logger=logger_serv.get_instance()
+
+Local_Logger=_Local_Logger
 class library_DB:
     def __init__(self):
         self.conn = db_connection()
         self.cursor = self.conn.cursor()
         
     def insert_User_Access_Token(self,user_name,profile_id,access_token):
         try:
-            Local_Logger.info("START insert access token to db "+access_token) 
+            Local_Logger.start("START insert access token to db "+access_token) 
             cursor = self.conn.cursor()
             query_max_id = "SELECT MAX(id) FROM external_user.external_user_table"
             cursor.execute(query_max_id)
             res = cursor.fetchone()
             cursor.close()
             max_id = res[0] + 1
             cursor = self.conn.cursor() 
@@ -37,71 +37,71 @@
                 max_id_new=1
             cursor = self.conn.cursor() 
             values=(max_id_new,max_id,profile_id)
             query_insert_external_user_profile= "INSERT INTO external_user_profile.external_user_profile_table (id,external_user_id,profile_id) VALUES (%s,%s,%s)"
             cursor.execute(query_insert_external_user_profile,values)
             cursor.close()
             self.conn.commit()
-            Local_Logger.info("END insert access token to db")
+            Local_Logger.end("END insert access token to db")
         except mysql.connector.Error as error:
-            Local_Logger.error(error.msg)
+            Local_Logger.exception(error)
             
     def get(self,user_name):
         try:
-            Local_Logger.info("start get access token for "+user_name) 
+            Local_Logger.start("start get access token for "+user_name) 
             cursor = cursor = self.conn.cursor()
             query_get_all = "SELECT token FROM external_user.external_user_table WHERE username=%s"
             cursor.execute(query_get_all,(user_name,))
             res = cursor.fetchone()
-            Local_Logger.info("END get access token from db")
+            Local_Logger.end("END get access token from db")
             return res
         except mysql.connector.Error as error:
-            Local_Logger.error(error.msg)
+            Local_Logger.exception(error)
     
     def select_by_profile_id(self,profile_id):
         try:
-            Local_Logger.info("start get access token") 
+            Local_Logger.start("start get access token") 
             cursor = self.conn.cursor()
 
             # Execute the select query
             select_query = """
                 SELECT * 
                 FROM external_user.external_user_table AS eu 
                 JOIN external_user_profile.external_user_profile_table AS eup ON eu.id = eup.external_user_id 
                 WHERE eup.profile_id = %s
             """
             cursor.execute(select_query, (profile_id,))
             result = cursor.fetchone()
             cursor.close()
-            Local_Logger.info("END get access token from db")
+            Local_Logger.end("END get access token from db")
             return result
         except mysql.connector.Error as error:
-            Local_Logger.error(error.msg)
+            Local_Logger.exception(error)
 
         # Fetch all the rows returned by the query
             
     
     def update_by_user_name(self,user_name,access_token):
         try:
-            Local_Logger.info("start update access token for "+user_name)
+            Local_Logger.start("start update access token for "+user_name)
             cursor = self.conn.cursor()
             update_query = "UPDATE external_user.external_user_table SET token = %s WHERE username = %s"
             values = (access_token, user_name)
             cursor.execute(update_query, values)
             self.conn.commit()
             cursor.close()
-            Local_Logger.info("END update access token in db")
+            Local_Logger.end("END update access token in db")
         except mysql.connector.Error as error:
-            Local_Logger.error(error.msg)
+            Local_Logger.exception(error)
 
 
 
     def update_by_profile_id(self,profile_id, access_token):
         try:
-            Local_Logger.info("start update access token ")
+            Local_Logger.start("start update access token ")
             cursor = self.conn.cursor()
 
             update_query = """
                 UPDATE external_user.external_user_table 
                 SET token = %s 
                 WHERE id IN (
                     SELECT external_user_id 
@@ -109,36 +109,36 @@
                     WHERE profile_id = %s
                 )
             """
             values = (access_token, profile_id)
             cursor.execute(update_query, values)
             self.conn.commit()
             cursor.close()
-            Local_Logger.info("END update access token in db")
+            Local_Logger.end("update access token in db")
         except mysql.connector.Error as error:
-           Local_Logger.error(error.msg)
+           Local_Logger.exception(error)
         
     def delete_by_profile_id(self,profile_id):
         try:
-            Local_Logger.info("start delete user external access token ")
+            Local_Logger.start("delete user external access token ")
             # Create a cursor object to execute queries
             cursor = self.conn.cursor()
             delete_query = """
                 UPDATE external_user.external_user_table AS eu
                 JOIN external_user_profile.external_user_profile_table AS eup ON eu.id = eup.external_user_id
                 SET eu.id = NULL, eu.system_id = NULL, eu.username = NULL, eu.token = NULL, eup.profile_id = NULL
                 WHERE eup.profile_id = %s
             """
             cursor.execute(delete_query, (profile_id,))
 
             self.conn.commit()
 
             cursor.close()
-            Local_Logger.info("END delete access token from db")
+            Local_Logger.end("delete access token from db")
         except mysql.connector.Error as error:
-           Local_Logger.error(error.msg)
+           Local_Logger.exception(error)
```

### Comparing `External-User-Local-0.0.8/setup.py` & `External-user-local-0.0.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import setuptools
 # used by python -m build
 # python -m build needs pyproject.toml or setup.py
 setuptools.setup(
-     # TODO: Please update the name and delete this line i.e. XXX-local or XXX-remote (without the -python-package suffix)
-     name='External-User-Local',  
-     version='0.0.8',
+     name='External-user-local',  
+     version='0.0.9',
      author="Circles",
      author_email="info@circles.life",
      # TODO: Please update the description and delete this line
      description="PyPI Package for Circles access token library Local/Remote Python",
      # TODO: Please update the long description and delete this line    
      long_description="This is a package for sharing common access tokens function used in different repositories",
      long_description_content_type="text/markdown",
```

### Comparing `External-User-Local-0.0.8/src/library.py` & `External-user-local-0.0.9/src/library.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,46 +1,44 @@
 import os
-from LoggerLocalPythonPackage.LoggerServiceSingleton import LoggerServiceSingleton
+from LoggerLocalPythonPackage.LocalLogger import _Local_Logger
 import sys
 import dotenv 
 sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), '..', 'db')))
 from library_DB import library_DB
 
 dotenv.load_dotenv()
-logger_serv=LoggerServiceSingleton()
-Local_Logger=logger_serv.get_instance()
+Local_Logger=_Local_Logger
 class Accsess_Token_Library:
     
     def insert_user_external(self,user_name,profile_id,access_token):
-        Local_Logger.info("START insert access token for "+access_token)
+        Local_Logger.start("START insert access token for "+access_token)
         insert_user_ext=library_DB()
         insert_user_ext.insert_User_Access_Token(user_name,profile_id,access_token)
-        Local_Logger.info("END insert access token "+access_token )
+        Local_Logger.end("END insert access token "+access_token )
         
     def update_user_external(self,profile_id,access_token):
-        Local_Logger.info("START update access token")
+        Local_Logger.start("START update access token")
         insert_user_ext=library_DB()
         insert_user_ext.update_by_profile_id(profile_id,access_token)
-        Local_Logger.info("END update access token "+access_token )
+        Local_Logger.end("END update access token "+access_token )
     def get_access_token(self,profile_id):
-        Local_Logger.info("START get access token")
+        Local_Logger.start("START get access token")
         insert_user_ext=library_DB()
         return insert_user_ext.select_by_profile_id(profile_id)
     def get_access_token_by_user_name(self,user_name):
-        Local_Logger.info("START get access token")
+        Local_Logger.start("START get access token")
         insert_user_ext=library_DB()
         res=insert_user_ext.get(user_name)
-        Local_Logger.info("END get access token")
+        Local_Logger.end("get access token")
         return res
         
     def delete_access_token_by_profile_id(self,profile_id):
-        Local_Logger.info("START get access token")
+        Local_Logger.start("START delete access token")
         insert_user_ext=library_DB()
-        Local_Logger.info("END get access token")
         insert_user_ext.delete_by_profile_id(profile_id)
-        Local_Logger.info("END delete access token")
+        Local_Logger.end("END delete access token")
         
     def update_user_external_by_username(self,user_name,access_token):
-       Local_Logger.info("START update access token")
+       Local_Logger.start("START update access token")
        insert_user_ext=library_DB()
        insert_user_ext.update_by_user_name(user_name,access_token)
-       Local_Logger.info("END update access token "+access_token ) 
+       Local_Logger.end("END update access token "+access_token )
```

### Comparing `External-User-Local-0.0.8/tests/test_insertExternal.py` & `External-user-local-0.0.9/tests/test_insertExternal.py`

 * *Files identical despite different names*

