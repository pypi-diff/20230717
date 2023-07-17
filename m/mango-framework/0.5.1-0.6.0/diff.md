# Comparing `tmp/mango-framework-0.5.1.tar.gz` & `tmp/mango-framework-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mango-framework-0.5.1.tar", last modified: Mon Jul 17 12:11:46 2023, max compression
+gzip compressed data, was "mango-framework-0.6.0.tar", last modified: Mon Jul 17 12:37:01 2023, max compression
```

## Comparing `mango-framework-0.5.1.tar` & `mango-framework-0.6.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 mohammed   (501) staff       (20)        0 2023-07-17 12:11:46.175012 mango-framework-0.5.1/
--rw-r--r--   0 mohammed   (501) staff       (20)     1023 2023-07-17 05:13:07.000000 mango-framework-0.5.1/LICENSE
--rw-r--r--   0 mohammed   (501) staff       (20)     1890 2023-07-17 12:11:46.174902 mango-framework-0.5.1/PKG-INFO
--rw-r--r--   0 mohammed   (501) staff       (20)     1210 2023-07-17 11:58:46.000000 mango-framework-0.5.1/README.md
--rw-r--r--   0 mohammed   (501) staff       (20)     5747 2023-07-17 05:04:24.000000 mango-framework-0.5.1/mango.py
-drwxr-xr-x   0 mohammed   (501) staff       (20)        0 2023-07-17 12:11:46.174740 mango-framework-0.5.1/mango_framework.egg-info/
--rw-r--r--   0 mohammed   (501) staff       (20)     1890 2023-07-17 12:11:46.000000 mango-framework-0.5.1/mango_framework.egg-info/PKG-INFO
--rw-r--r--   0 mohammed   (501) staff       (20)      191 2023-07-17 12:11:46.000000 mango-framework-0.5.1/mango_framework.egg-info/SOURCES.txt
--rw-r--r--   0 mohammed   (501) staff       (20)        1 2023-07-17 12:11:46.000000 mango-framework-0.5.1/mango_framework.egg-info/dependency_links.txt
--rw-r--r--   0 mohammed   (501) staff       (20)        1 2023-07-17 12:11:46.000000 mango-framework-0.5.1/mango_framework.egg-info/top_level.txt
--rw-r--r--   0 mohammed   (501) staff       (20)       38 2023-07-17 12:11:46.175058 mango-framework-0.5.1/setup.cfg
--rw-r--r--   0 mohammed   (501) staff       (20)      869 2023-07-17 12:11:42.000000 mango-framework-0.5.1/setup.py
+drwxr-xr-x   0 mohammed   (501) staff       (20)        0 2023-07-17 12:37:01.278573 mango-framework-0.6.0/
+-rw-r--r--   0 mohammed   (501) staff       (20)     1023 2023-07-17 05:13:07.000000 mango-framework-0.6.0/LICENSE
+-rw-r--r--   0 mohammed   (501) staff       (20)     1920 2023-07-17 12:37:01.278464 mango-framework-0.6.0/PKG-INFO
+-rw-r--r--   0 mohammed   (501) staff       (20)     1240 2023-07-17 12:32:59.000000 mango-framework-0.6.0/README.md
+-rw-r--r--   0 mohammed   (501) staff       (20)     6050 2023-07-17 12:31:02.000000 mango-framework-0.6.0/mango.py
+drwxr-xr-x   0 mohammed   (501) staff       (20)        0 2023-07-17 12:37:01.278278 mango-framework-0.6.0/mango_framework.egg-info/
+-rw-r--r--   0 mohammed   (501) staff       (20)     1920 2023-07-17 12:37:01.000000 mango-framework-0.6.0/mango_framework.egg-info/PKG-INFO
+-rw-r--r--   0 mohammed   (501) staff       (20)      191 2023-07-17 12:37:01.000000 mango-framework-0.6.0/mango_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 mohammed   (501) staff       (20)        1 2023-07-17 12:37:01.000000 mango-framework-0.6.0/mango_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 mohammed   (501) staff       (20)        1 2023-07-17 12:37:01.000000 mango-framework-0.6.0/mango_framework.egg-info/top_level.txt
+-rw-r--r--   0 mohammed   (501) staff       (20)       38 2023-07-17 12:37:01.278614 mango-framework-0.6.0/setup.cfg
+-rw-r--r--   0 mohammed   (501) staff       (20)      869 2023-07-17 12:33:39.000000 mango-framework-0.6.0/setup.py
```

### Comparing `mango-framework-0.5.1/LICENSE` & `mango-framework-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mango-framework-0.5.1/PKG-INFO` & `mango-framework-0.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mango-framework
-Version: 0.5.1
+Version: 0.6.0
 Summary: A lightweight and highly customizable Python framework for building web applications
 Home-page: https://github.com/momo-AUX1/mango
 Author: Mohammed
 Author-email: fdlnaal@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -26,14 +26,15 @@
 
 ## Features
 
 - Easy routing configuration
 - Rendering HTML templates
 - Serving static files
 - Handling JSON data
+- Handling of basic form data
 - Lightweight and minimal dependencies
 - Suitable for small to medium-sized web applications
 - Human readible code even beginners could modify 
 - Integrated basic ORM for DB functions
 
 ## Installation
```

### Comparing `mango-framework-0.5.1/README.md` & `mango-framework-0.6.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 ## Features
 
 - Easy routing configuration
 - Rendering HTML templates
 - Serving static files
 - Handling JSON data
+- Handling of basic form data
 - Lightweight and minimal dependencies
 - Suitable for small to medium-sized web applications
 - Human readible code even beginners could modify 
 - Integrated basic ORM for DB functions
 
 ## Installation
```

### Comparing `mango-framework-0.5.1/mango.py` & `mango-framework-0.6.0/mango.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from wsgiref.simple_server import make_server
 import json
 from os.path import join
 import sqlite3
+from urllib.parse import parse_qs
 
 templates_path = 'templates'
 
 files_path = 'files'
 
 # Default route
 
@@ -47,17 +48,26 @@
 
   if path in routes and method == 'POST':
     if req == 'application/json':
       length = int(environ.get('CONTENT_LENGTH', 0))
       body = environ['wsgi.input'].read(length).decode('utf-8')
       response = routes[path](body)
       start_response(*OK)
+
+    elif req == 'application/x-www-form-urlencoded':
+      length = int(environ.get('CONTENT_LENGTH', 0))
+      body = environ['wsgi.input'].read(length).decode('utf-8')
+      data = parse_qs(body)
+      response = routes[path](data)
+      start_response(*OK)
+
     else:
       response = "<h1> NOT ALLOWED </h1>"
       start_response(*NOT_ALLOWED)
+      
   elif path in routes and method == 'GET':
     try:
       response, content_type, filename = routes[path]()
       start_response(
         '200 OK',
         [('Content-Type', content_type),
          ('content-disposition', f'attachment; filename={filename}')])
```

### Comparing `mango-framework-0.5.1/mango_framework.egg-info/PKG-INFO` & `mango-framework-0.6.0/mango_framework.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mango-framework
-Version: 0.5.1
+Version: 0.6.0
 Summary: A lightweight and highly customizable Python framework for building web applications
 Home-page: https://github.com/momo-AUX1/mango
 Author: Mohammed
 Author-email: fdlnaal@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -26,14 +26,15 @@
 
 ## Features
 
 - Easy routing configuration
 - Rendering HTML templates
 - Serving static files
 - Handling JSON data
+- Handling of basic form data
 - Lightweight and minimal dependencies
 - Suitable for small to medium-sized web applications
 - Human readible code even beginners could modify 
 - Integrated basic ORM for DB functions
 
 ## Installation
```

### Comparing `mango-framework-0.5.1/setup.py` & `mango-framework-0.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='mango-framework',
-    version='0.5.1',
+    version='0.6.0',
     author='Mohammed',
     author_email='fdlnaal@gmail.com',
     description='A lightweight and highly customizable Python framework for building web applications',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/momo-AUX1/mango',
     packages=['.'],
```

