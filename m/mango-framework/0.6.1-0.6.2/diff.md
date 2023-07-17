# Comparing `tmp/mango-framework-0.6.1.tar.gz` & `tmp/mango-framework-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mango-framework-0.6.1.tar", last modified: Mon Jul 17 12:43:27 2023, max compression
+gzip compressed data, was "mango-framework-0.6.2.tar", last modified: Mon Jul 17 12:53:58 2023, max compression
```

## Comparing `mango-framework-0.6.1.tar` & `mango-framework-0.6.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 mohammed   (501) staff       (20)        0 2023-07-17 12:43:27.766289 mango-framework-0.6.1/
--rw-r--r--   0 mohammed   (501) staff       (20)     1023 2023-07-17 05:13:07.000000 mango-framework-0.6.1/LICENSE
--rw-r--r--   0 mohammed   (501) staff       (20)     1920 2023-07-17 12:43:27.766182 mango-framework-0.6.1/PKG-INFO
--rw-r--r--   0 mohammed   (501) staff       (20)     1240 2023-07-17 12:32:59.000000 mango-framework-0.6.1/README.md
--rw-r--r--   0 mohammed   (501) staff       (20)     6046 2023-07-17 12:42:40.000000 mango-framework-0.6.1/mango.py
-drwxr-xr-x   0 mohammed   (501) staff       (20)        0 2023-07-17 12:43:27.766015 mango-framework-0.6.1/mango_framework.egg-info/
--rw-r--r--   0 mohammed   (501) staff       (20)     1920 2023-07-17 12:43:27.000000 mango-framework-0.6.1/mango_framework.egg-info/PKG-INFO
--rw-r--r--   0 mohammed   (501) staff       (20)      191 2023-07-17 12:43:27.000000 mango-framework-0.6.1/mango_framework.egg-info/SOURCES.txt
--rw-r--r--   0 mohammed   (501) staff       (20)        1 2023-07-17 12:43:27.000000 mango-framework-0.6.1/mango_framework.egg-info/dependency_links.txt
--rw-r--r--   0 mohammed   (501) staff       (20)        1 2023-07-17 12:43:27.000000 mango-framework-0.6.1/mango_framework.egg-info/top_level.txt
--rw-r--r--   0 mohammed   (501) staff       (20)       38 2023-07-17 12:43:27.766327 mango-framework-0.6.1/setup.cfg
--rw-r--r--   0 mohammed   (501) staff       (20)      869 2023-07-17 12:42:46.000000 mango-framework-0.6.1/setup.py
+drwxr-xr-x   0 mohammed   (501) staff       (20)        0 2023-07-17 12:53:58.646586 mango-framework-0.6.2/
+-rw-r--r--   0 mohammed   (501) staff       (20)     1023 2023-07-17 05:13:07.000000 mango-framework-0.6.2/LICENSE
+-rw-r--r--   0 mohammed   (501) staff       (20)     1920 2023-07-17 12:53:58.646475 mango-framework-0.6.2/PKG-INFO
+-rw-r--r--   0 mohammed   (501) staff       (20)     1240 2023-07-17 12:32:59.000000 mango-framework-0.6.2/README.md
+-rw-r--r--   0 mohammed   (501) staff       (20)     6335 2023-07-17 12:53:42.000000 mango-framework-0.6.2/mango.py
+drwxr-xr-x   0 mohammed   (501) staff       (20)        0 2023-07-17 12:53:58.646315 mango-framework-0.6.2/mango_framework.egg-info/
+-rw-r--r--   0 mohammed   (501) staff       (20)     1920 2023-07-17 12:53:58.000000 mango-framework-0.6.2/mango_framework.egg-info/PKG-INFO
+-rw-r--r--   0 mohammed   (501) staff       (20)      191 2023-07-17 12:53:58.000000 mango-framework-0.6.2/mango_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 mohammed   (501) staff       (20)        1 2023-07-17 12:53:58.000000 mango-framework-0.6.2/mango_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 mohammed   (501) staff       (20)        1 2023-07-17 12:53:58.000000 mango-framework-0.6.2/mango_framework.egg-info/top_level.txt
+-rw-r--r--   0 mohammed   (501) staff       (20)       38 2023-07-17 12:53:58.646624 mango-framework-0.6.2/setup.cfg
+-rw-r--r--   0 mohammed   (501) staff       (20)      869 2023-07-17 12:53:53.000000 mango-framework-0.6.2/setup.py
```

### Comparing `mango-framework-0.6.1/LICENSE` & `mango-framework-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mango-framework-0.6.1/PKG-INFO` & `mango-framework-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mango-framework
-Version: 0.6.1
+Version: 0.6.2
 Summary: A lightweight and highly customizable Python framework for building web applications
 Home-page: https://github.com/momo-AUX1/mango
 Author: Mohammed
 Author-email: fdlnaal@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `mango-framework-0.6.1/README.md` & `mango-framework-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `mango-framework-0.6.1/mango.py` & `mango-framework-0.6.2/mango.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from wsgiref.simple_server import make_server
 import json
 from os.path import join
 import sqlite3
 from urllib.parse import parse_qs
+from collections import namedtuple
 
 templates_path = 'templates'
 
 files_path = 'files'
 
 # Default route
 
@@ -164,27 +165,31 @@
         }
     </style>
 </head>
 <body>
     <h1>Server successfully started, but there are no routes or the "/" route is empty</h1>
     <img class="mango-img" src="https://th.bing.com/th/id/R.54bad49b520690f3858b1f396194779d?rik=QSeITH3EbHg4Vw&pid=ImgRaw&r=0" alt="Mango">
     <footer>
-        Version: 0.6.1
+        Version: 0.6.2
     </footer>
 </body>
 </html>"""
 
 
 #Native User DB 
 
 conn = sqlite3.connect('databse.sqlite')
 
 conn.execute('CREATE TABLE IF NOT EXISTS Users (id INTEGER PRIMARY KEY AUTOINCREMENT, username TEXT, firstname TEXT, lastname TEXT, email TEXT, password TEXT)')
 
+from collections import namedtuple
+
 def user():
+    UserFunctions = namedtuple('UserFunctions', ['insert', 'search', 'delete', 'get_user_by_username', 'get_user_by_firstname', 'get_user_by_lastname', 'get_user_by_email', 'get_user_by_password'])
+    
     def insert(username=None, firstname=None, lastname=None, email=None, password=None):
         conn.execute('INSERT INTO Users (username, firstname, lastname, email, password) VALUES (?,?,?,?,?)',
                      (username, firstname, lastname, email, password))
         conn.commit()
 
     def search(search):
         search_term = f"%{search}%"
@@ -214,8 +219,8 @@
         result = conn.execute('SELECT * FROM Users WHERE email = ?', (email,))
         return result.fetchone()
     
     def get_user_by_password(password):
         result = conn.execute('SELECT * FROM Users WHERE password = ?', (password,))
         return result.fetchone()
 
-    return insert, search, delete, get_user_by_username, get_user_by_firstname, get_user_by_lastname, get_user_by_email, get_user_by_password
+    return UserFunctions(insert, search, delete, get_user_by_username, get_user_by_firstname, get_user_by_lastname, get_user_by_email, get_user_by_password)
```

### Comparing `mango-framework-0.6.1/mango_framework.egg-info/PKG-INFO` & `mango-framework-0.6.2/mango_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mango-framework
-Version: 0.6.1
+Version: 0.6.2
 Summary: A lightweight and highly customizable Python framework for building web applications
 Home-page: https://github.com/momo-AUX1/mango
 Author: Mohammed
 Author-email: fdlnaal@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `mango-framework-0.6.1/setup.py` & `mango-framework-0.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='mango-framework',
-    version='0.6.1',
+    version='0.6.2',
     author='Mohammed',
     author_email='fdlnaal@gmail.com',
     description='A lightweight and highly customizable Python framework for building web applications',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/momo-AUX1/mango',
     packages=['.'],
```

