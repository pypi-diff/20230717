# Comparing `tmp/mango-framework-0.6.0.tar.gz` & `tmp/mango-framework-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mango-framework-0.6.0.tar", last modified: Mon Jul 17 12:37:01 2023, max compression
+gzip compressed data, was "mango-framework-0.6.1.tar", last modified: Mon Jul 17 12:43:27 2023, max compression
```

## Comparing `mango-framework-0.6.0.tar` & `mango-framework-0.6.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 mohammed   (501) staff       (20)        0 2023-07-17 12:37:01.278573 mango-framework-0.6.0/
--rw-r--r--   0 mohammed   (501) staff       (20)     1023 2023-07-17 05:13:07.000000 mango-framework-0.6.0/LICENSE
--rw-r--r--   0 mohammed   (501) staff       (20)     1920 2023-07-17 12:37:01.278464 mango-framework-0.6.0/PKG-INFO
--rw-r--r--   0 mohammed   (501) staff       (20)     1240 2023-07-17 12:32:59.000000 mango-framework-0.6.0/README.md
--rw-r--r--   0 mohammed   (501) staff       (20)     6050 2023-07-17 12:31:02.000000 mango-framework-0.6.0/mango.py
-drwxr-xr-x   0 mohammed   (501) staff       (20)        0 2023-07-17 12:37:01.278278 mango-framework-0.6.0/mango_framework.egg-info/
--rw-r--r--   0 mohammed   (501) staff       (20)     1920 2023-07-17 12:37:01.000000 mango-framework-0.6.0/mango_framework.egg-info/PKG-INFO
--rw-r--r--   0 mohammed   (501) staff       (20)      191 2023-07-17 12:37:01.000000 mango-framework-0.6.0/mango_framework.egg-info/SOURCES.txt
--rw-r--r--   0 mohammed   (501) staff       (20)        1 2023-07-17 12:37:01.000000 mango-framework-0.6.0/mango_framework.egg-info/dependency_links.txt
--rw-r--r--   0 mohammed   (501) staff       (20)        1 2023-07-17 12:37:01.000000 mango-framework-0.6.0/mango_framework.egg-info/top_level.txt
--rw-r--r--   0 mohammed   (501) staff       (20)       38 2023-07-17 12:37:01.278614 mango-framework-0.6.0/setup.cfg
--rw-r--r--   0 mohammed   (501) staff       (20)      869 2023-07-17 12:33:39.000000 mango-framework-0.6.0/setup.py
+drwxr-xr-x   0 mohammed   (501) staff       (20)        0 2023-07-17 12:43:27.766289 mango-framework-0.6.1/
+-rw-r--r--   0 mohammed   (501) staff       (20)     1023 2023-07-17 05:13:07.000000 mango-framework-0.6.1/LICENSE
+-rw-r--r--   0 mohammed   (501) staff       (20)     1920 2023-07-17 12:43:27.766182 mango-framework-0.6.1/PKG-INFO
+-rw-r--r--   0 mohammed   (501) staff       (20)     1240 2023-07-17 12:32:59.000000 mango-framework-0.6.1/README.md
+-rw-r--r--   0 mohammed   (501) staff       (20)     6046 2023-07-17 12:42:40.000000 mango-framework-0.6.1/mango.py
+drwxr-xr-x   0 mohammed   (501) staff       (20)        0 2023-07-17 12:43:27.766015 mango-framework-0.6.1/mango_framework.egg-info/
+-rw-r--r--   0 mohammed   (501) staff       (20)     1920 2023-07-17 12:43:27.000000 mango-framework-0.6.1/mango_framework.egg-info/PKG-INFO
+-rw-r--r--   0 mohammed   (501) staff       (20)      191 2023-07-17 12:43:27.000000 mango-framework-0.6.1/mango_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 mohammed   (501) staff       (20)        1 2023-07-17 12:43:27.000000 mango-framework-0.6.1/mango_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 mohammed   (501) staff       (20)        1 2023-07-17 12:43:27.000000 mango-framework-0.6.1/mango_framework.egg-info/top_level.txt
+-rw-r--r--   0 mohammed   (501) staff       (20)       38 2023-07-17 12:43:27.766327 mango-framework-0.6.1/setup.cfg
+-rw-r--r--   0 mohammed   (501) staff       (20)      869 2023-07-17 12:42:46.000000 mango-framework-0.6.1/setup.py
```

### Comparing `mango-framework-0.6.0/LICENSE` & `mango-framework-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mango-framework-0.6.0/PKG-INFO` & `mango-framework-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mango-framework
-Version: 0.6.0
+Version: 0.6.1
 Summary: A lightweight and highly customizable Python framework for building web applications
 Home-page: https://github.com/momo-AUX1/mango
 Author: Mohammed
 Author-email: fdlnaal@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `mango-framework-0.6.0/README.md` & `mango-framework-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `mango-framework-0.6.0/mango.py` & `mango-framework-0.6.1/mango.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
       data = parse_qs(body)
       response = routes[path](data)
       start_response(*OK)
 
     else:
       response = "<h1> NOT ALLOWED </h1>"
       start_response(*NOT_ALLOWED)
-      
+
   elif path in routes and method == 'GET':
     try:
       response, content_type, filename = routes[path]()
       start_response(
         '200 OK',
         [('Content-Type', content_type),
          ('content-disposition', f'attachment; filename={filename}')])
@@ -164,15 +164,15 @@
         }
     </style>
 </head>
 <body>
     <h1>Server successfully started, but there are no routes or the "/" route is empty</h1>
     <img class="mango-img" src="https://th.bing.com/th/id/R.54bad49b520690f3858b1f396194779d?rik=QSeITH3EbHg4Vw&pid=ImgRaw&r=0" alt="Mango">
     <footer>
-        Version: 0.5
+        Version: 0.6.1
     </footer>
 </body>
 </html>"""
 
 
 #Native User DB
```

### Comparing `mango-framework-0.6.0/mango_framework.egg-info/PKG-INFO` & `mango-framework-0.6.1/mango_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mango-framework
-Version: 0.6.0
+Version: 0.6.1
 Summary: A lightweight and highly customizable Python framework for building web applications
 Home-page: https://github.com/momo-AUX1/mango
 Author: Mohammed
 Author-email: fdlnaal@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `mango-framework-0.6.0/setup.py` & `mango-framework-0.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='mango-framework',
-    version='0.6.0',
+    version='0.6.1',
     author='Mohammed',
     author_email='fdlnaal@gmail.com',
     description='A lightweight and highly customizable Python framework for building web applications',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/momo-AUX1/mango',
     packages=['.'],
```

