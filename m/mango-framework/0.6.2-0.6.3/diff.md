# Comparing `tmp/mango-framework-0.6.2.tar.gz` & `tmp/mango-framework-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mango-framework-0.6.2.tar", last modified: Mon Jul 17 12:53:58 2023, max compression
+gzip compressed data, was "mango-framework-0.6.3.tar", last modified: Mon Jul 17 13:02:08 2023, max compression
```

## Comparing `mango-framework-0.6.2.tar` & `mango-framework-0.6.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 mohammed   (501) staff       (20)        0 2023-07-17 12:53:58.646586 mango-framework-0.6.2/
--rw-r--r--   0 mohammed   (501) staff       (20)     1023 2023-07-17 05:13:07.000000 mango-framework-0.6.2/LICENSE
--rw-r--r--   0 mohammed   (501) staff       (20)     1920 2023-07-17 12:53:58.646475 mango-framework-0.6.2/PKG-INFO
--rw-r--r--   0 mohammed   (501) staff       (20)     1240 2023-07-17 12:32:59.000000 mango-framework-0.6.2/README.md
--rw-r--r--   0 mohammed   (501) staff       (20)     6335 2023-07-17 12:53:42.000000 mango-framework-0.6.2/mango.py
-drwxr-xr-x   0 mohammed   (501) staff       (20)        0 2023-07-17 12:53:58.646315 mango-framework-0.6.2/mango_framework.egg-info/
--rw-r--r--   0 mohammed   (501) staff       (20)     1920 2023-07-17 12:53:58.000000 mango-framework-0.6.2/mango_framework.egg-info/PKG-INFO
--rw-r--r--   0 mohammed   (501) staff       (20)      191 2023-07-17 12:53:58.000000 mango-framework-0.6.2/mango_framework.egg-info/SOURCES.txt
--rw-r--r--   0 mohammed   (501) staff       (20)        1 2023-07-17 12:53:58.000000 mango-framework-0.6.2/mango_framework.egg-info/dependency_links.txt
--rw-r--r--   0 mohammed   (501) staff       (20)        1 2023-07-17 12:53:58.000000 mango-framework-0.6.2/mango_framework.egg-info/top_level.txt
--rw-r--r--   0 mohammed   (501) staff       (20)       38 2023-07-17 12:53:58.646624 mango-framework-0.6.2/setup.cfg
--rw-r--r--   0 mohammed   (501) staff       (20)      869 2023-07-17 12:53:53.000000 mango-framework-0.6.2/setup.py
+drwxr-xr-x   0 mohammed   (501) staff       (20)        0 2023-07-17 13:02:08.744080 mango-framework-0.6.3/
+-rw-r--r--   0 mohammed   (501) staff       (20)     1023 2023-07-17 05:13:07.000000 mango-framework-0.6.3/LICENSE
+-rw-r--r--   0 mohammed   (501) staff       (20)     1920 2023-07-17 13:02:08.743955 mango-framework-0.6.3/PKG-INFO
+-rw-r--r--   0 mohammed   (501) staff       (20)     1240 2023-07-17 12:32:59.000000 mango-framework-0.6.3/README.md
+-rw-r--r--   0 mohammed   (501) staff       (20)     6046 2023-07-17 13:01:56.000000 mango-framework-0.6.3/mango.py
+drwxr-xr-x   0 mohammed   (501) staff       (20)        0 2023-07-17 13:02:08.743740 mango-framework-0.6.3/mango_framework.egg-info/
+-rw-r--r--   0 mohammed   (501) staff       (20)     1920 2023-07-17 13:02:08.000000 mango-framework-0.6.3/mango_framework.egg-info/PKG-INFO
+-rw-r--r--   0 mohammed   (501) staff       (20)      191 2023-07-17 13:02:08.000000 mango-framework-0.6.3/mango_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 mohammed   (501) staff       (20)        1 2023-07-17 13:02:08.000000 mango-framework-0.6.3/mango_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 mohammed   (501) staff       (20)        1 2023-07-17 13:02:08.000000 mango-framework-0.6.3/mango_framework.egg-info/top_level.txt
+-rw-r--r--   0 mohammed   (501) staff       (20)       38 2023-07-17 13:02:08.744123 mango-framework-0.6.3/setup.cfg
+-rw-r--r--   0 mohammed   (501) staff       (20)      869 2023-07-17 13:01:59.000000 mango-framework-0.6.3/setup.py
```

### Comparing `mango-framework-0.6.2/LICENSE` & `mango-framework-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mango-framework-0.6.2/PKG-INFO` & `mango-framework-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mango-framework
-Version: 0.6.2
+Version: 0.6.3
 Summary: A lightweight and highly customizable Python framework for building web applications
 Home-page: https://github.com/momo-AUX1/mango
 Author: Mohammed
 Author-email: fdlnaal@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `mango-framework-0.6.2/README.md` & `mango-framework-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `mango-framework-0.6.2/mango.py` & `mango-framework-0.6.3/mango.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from wsgiref.simple_server import make_server
 import json
 from os.path import join
 import sqlite3
 from urllib.parse import parse_qs
-from collections import namedtuple
 
 templates_path = 'templates'
 
 files_path = 'files'
 
 # Default route
 
@@ -165,62 +164,56 @@
         }
     </style>
 </head>
 <body>
     <h1>Server successfully started, but there are no routes or the "/" route is empty</h1>
     <img class="mango-img" src="https://th.bing.com/th/id/R.54bad49b520690f3858b1f396194779d?rik=QSeITH3EbHg4Vw&pid=ImgRaw&r=0" alt="Mango">
     <footer>
-        Version: 0.6.2
+        Version: 0.6.3
     </footer>
 </body>
 </html>"""
 
 
 #Native User DB 
 
-conn = sqlite3.connect('databse.sqlite')
+class User:
+    def __init__(self):
+      self.conn = sqlite3.connect('databse.sqlite')
+      self.conn.execute('CREATE TABLE IF NOT EXISTS Users (id INTEGER PRIMARY KEY AUTOINCREMENT, username TEXT, firstname TEXT, lastname TEXT, email TEXT, password TEXT)')
 
-conn.execute('CREATE TABLE IF NOT EXISTS Users (id INTEGER PRIMARY KEY AUTOINCREMENT, username TEXT, firstname TEXT, lastname TEXT, email TEXT, password TEXT)')
-
-from collections import namedtuple
-
-def user():
-    UserFunctions = namedtuple('UserFunctions', ['insert', 'search', 'delete', 'get_user_by_username', 'get_user_by_firstname', 'get_user_by_lastname', 'get_user_by_email', 'get_user_by_password'])
-    
-    def insert(username=None, firstname=None, lastname=None, email=None, password=None):
-        conn.execute('INSERT INTO Users (username, firstname, lastname, email, password) VALUES (?,?,?,?,?)',
+    def insert(self, username=None, firstname=None, lastname=None, email=None, password=None):
+        self.conn.execute('INSERT INTO Users (username, firstname, lastname, email, password) VALUES (?,?,?,?,?)',
                      (username, firstname, lastname, email, password))
-        conn.commit()
+        self.conn.commit()
 
-    def search(search):
+    def search(self, search):
         search_term = f"%{search}%"
-        result = conn.execute('SELECT * FROM Users WHERE username LIKE ? OR firstname LIKE ? OR lastname LIKE ? OR email LIKE ? OR password LIKE ?',
+        result = self.conn.execute('SELECT * FROM Users WHERE username LIKE ? OR firstname LIKE ? OR lastname LIKE ? OR email LIKE ? OR password LIKE ?',
                               (search_term, search_term, search_term, search_term, search_term))
         return result.fetchall()
 
-    def delete(search):
+    def delete(self, search):
         search_term = f"%{search}%"
-        conn.execute('DELETE FROM Users WHERE username LIKE ? OR firstname LIKE ? OR lastname LIKE ? OR email LIKE ? OR password LIKE ?',
+        self.conn.execute('DELETE FROM Users WHERE username LIKE ? OR firstname LIKE ? OR lastname LIKE ? OR email LIKE ? OR password LIKE ?',
                      (search_term, search_term, search_term, search_term, search_term))
-        conn.commit()
+        self.conn.commit()
 
-    def get_user_by_username(username):
-        result = conn.execute('SELECT * FROM Users WHERE username = ?', (username,))
+    def get_user_by_username(self, username):
+        result = self.conn.execute('SELECT * FROM Users WHERE username = ?', (username,))
         return result.fetchone()
     
-    def get_user_by_firstname(firstname):
-        result = conn.execute('SELECT * FROM Users WHERE firstname = ?', (firstname,))
+    def get_user_by_firstname(self, firstname):
+        result = self.conn.execute('SELECT * FROM Users WHERE firstname = ?', (firstname,))
         return result.fetchone()
     
-    def get_user_by_lastname(lastname):
-        result = conn.execute('SELECT * FROM Users WHERE lastname = ?', (lastname,))
+    def get_user_by_lastname(self, lastname):
+        result = self.conn.execute('SELECT * FROM Users WHERE lastname = ?', (lastname,))
         return result.fetchone()
     
-    def get_user_by_email(email):
-        result = conn.execute('SELECT * FROM Users WHERE email = ?', (email,))
+    def get_user_by_email(self, email):
+        result = self.conn.execute('SELECT * FROM Users WHERE email = ?', (email,))
         return result.fetchone()
     
-    def get_user_by_password(password):
-        result = conn.execute('SELECT * FROM Users WHERE password = ?', (password,))
+    def get_user_by_password(self, password):
+        result = self.conn.execute('SELECT * FROM Users WHERE password = ?', (password,))
         return result.fetchone()
-
-    return UserFunctions(insert, search, delete, get_user_by_username, get_user_by_firstname, get_user_by_lastname, get_user_by_email, get_user_by_password)
```

### Comparing `mango-framework-0.6.2/mango_framework.egg-info/PKG-INFO` & `mango-framework-0.6.3/mango_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mango-framework
-Version: 0.6.2
+Version: 0.6.3
 Summary: A lightweight and highly customizable Python framework for building web applications
 Home-page: https://github.com/momo-AUX1/mango
 Author: Mohammed
 Author-email: fdlnaal@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `mango-framework-0.6.2/setup.py` & `mango-framework-0.6.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='mango-framework',
-    version='0.6.2',
+    version='0.6.3',
     author='Mohammed',
     author_email='fdlnaal@gmail.com',
     description='A lightweight and highly customizable Python framework for building web applications',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/momo-AUX1/mango',
     packages=['.'],
```

