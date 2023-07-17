# Comparing `tmp/mango-framework-0.6.3.tar.gz` & `tmp/mango-framework-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mango-framework-0.6.3.tar", last modified: Mon Jul 17 13:02:08 2023, max compression
+gzip compressed data, was "mango-framework-0.6.5.tar", last modified: Mon Jul 17 13:27:56 2023, max compression
```

## Comparing `mango-framework-0.6.3.tar` & `mango-framework-0.6.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 mohammed   (501) staff       (20)        0 2023-07-17 13:02:08.744080 mango-framework-0.6.3/
--rw-r--r--   0 mohammed   (501) staff       (20)     1023 2023-07-17 05:13:07.000000 mango-framework-0.6.3/LICENSE
--rw-r--r--   0 mohammed   (501) staff       (20)     1920 2023-07-17 13:02:08.743955 mango-framework-0.6.3/PKG-INFO
--rw-r--r--   0 mohammed   (501) staff       (20)     1240 2023-07-17 12:32:59.000000 mango-framework-0.6.3/README.md
--rw-r--r--   0 mohammed   (501) staff       (20)     6046 2023-07-17 13:01:56.000000 mango-framework-0.6.3/mango.py
-drwxr-xr-x   0 mohammed   (501) staff       (20)        0 2023-07-17 13:02:08.743740 mango-framework-0.6.3/mango_framework.egg-info/
--rw-r--r--   0 mohammed   (501) staff       (20)     1920 2023-07-17 13:02:08.000000 mango-framework-0.6.3/mango_framework.egg-info/PKG-INFO
--rw-r--r--   0 mohammed   (501) staff       (20)      191 2023-07-17 13:02:08.000000 mango-framework-0.6.3/mango_framework.egg-info/SOURCES.txt
--rw-r--r--   0 mohammed   (501) staff       (20)        1 2023-07-17 13:02:08.000000 mango-framework-0.6.3/mango_framework.egg-info/dependency_links.txt
--rw-r--r--   0 mohammed   (501) staff       (20)        1 2023-07-17 13:02:08.000000 mango-framework-0.6.3/mango_framework.egg-info/top_level.txt
--rw-r--r--   0 mohammed   (501) staff       (20)       38 2023-07-17 13:02:08.744123 mango-framework-0.6.3/setup.cfg
--rw-r--r--   0 mohammed   (501) staff       (20)      869 2023-07-17 13:01:59.000000 mango-framework-0.6.3/setup.py
+drwxr-xr-x   0 mohammed   (501) staff       (20)        0 2023-07-17 13:27:56.223357 mango-framework-0.6.5/
+-rw-r--r--   0 mohammed   (501) staff       (20)     1023 2023-07-17 05:13:07.000000 mango-framework-0.6.5/LICENSE
+-rw-r--r--   0 mohammed   (501) staff       (20)     1920 2023-07-17 13:27:56.223245 mango-framework-0.6.5/PKG-INFO
+-rw-r--r--   0 mohammed   (501) staff       (20)     1240 2023-07-17 12:32:59.000000 mango-framework-0.6.5/README.md
+-rw-r--r--   0 mohammed   (501) staff       (20)     6285 2023-07-17 13:25:38.000000 mango-framework-0.6.5/mango.py
+drwxr-xr-x   0 mohammed   (501) staff       (20)        0 2023-07-17 13:27:56.223071 mango-framework-0.6.5/mango_framework.egg-info/
+-rw-r--r--   0 mohammed   (501) staff       (20)     1920 2023-07-17 13:27:56.000000 mango-framework-0.6.5/mango_framework.egg-info/PKG-INFO
+-rw-r--r--   0 mohammed   (501) staff       (20)      191 2023-07-17 13:27:56.000000 mango-framework-0.6.5/mango_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 mohammed   (501) staff       (20)        1 2023-07-17 13:27:56.000000 mango-framework-0.6.5/mango_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 mohammed   (501) staff       (20)        1 2023-07-17 13:27:56.000000 mango-framework-0.6.5/mango_framework.egg-info/top_level.txt
+-rw-r--r--   0 mohammed   (501) staff       (20)       38 2023-07-17 13:27:56.223401 mango-framework-0.6.5/setup.cfg
+-rw-r--r--   0 mohammed   (501) staff       (20)      869 2023-07-17 13:27:12.000000 mango-framework-0.6.5/setup.py
```

### Comparing `mango-framework-0.6.3/LICENSE` & `mango-framework-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mango-framework-0.6.3/PKG-INFO` & `mango-framework-0.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mango-framework
-Version: 0.6.3
+Version: 0.6.5
 Summary: A lightweight and highly customizable Python framework for building web applications
 Home-page: https://github.com/momo-AUX1/mango
 Author: Mohammed
 Author-email: fdlnaal@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `mango-framework-0.6.3/README.md` & `mango-framework-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `mango-framework-0.6.3/mango.py` & `mango-framework-0.6.5/mango.py`

 * *Files 6% similar despite different names*

```diff
@@ -74,14 +74,15 @@
     except:
       try:
         response, content_type = routes[path]()
         start_response('200 OK', [('Content-Type', content_type)])
       except:
         response = routes[path]()
         start_response(*OK)
+
   else:
     response = "<h1>404 NOT FOUND</h1>"
     start_response(*NOT_FOUND)
 
   try:
     return [response.encode()]
   except:
@@ -125,15 +126,16 @@
 
 
 def redirect(link):
   return f"<script>window.location.href = '{link}'</script>"
 
 # Default page
 
-html = """<!DOCTYPE html>
+html = """
+<!DOCTYPE html>
 <html>
 <head>
     <title>Mango Server</title>
     <style>
         body {
             background-color: white;
             color: orange;
@@ -158,31 +160,40 @@
             color: #888;
         }
 
         .mango-img {
             width: 150px;
             margin: 0 auto;
         }
+
+        .link {
+            color: orange;
+            text-decoration: underline;
+            margin-top: 10px;
+        }
     </style>
 </head>
 <body>
     <h1>Server successfully started, but there are no routes or the "/" route is empty</h1>
     <img class="mango-img" src="https://th.bing.com/th/id/R.54bad49b520690f3858b1f396194779d?rik=QSeITH3EbHg4Vw&pid=ImgRaw&r=0" alt="Mango">
     <footer>
-        Version: 0.6.3
+        Version: 0.6.5
+        <br>
+        <a class="link" href="https://pypi.org/project/mango-framework/">Check out the development!</a>
     </footer>
 </body>
-</html>"""
+</html>
+"""
 
 
 #Native User DB 
 
 class User:
     def __init__(self):
-      self.conn = sqlite3.connect('databse.sqlite')
+      self.conn = sqlite3.connect('DB.sqlite')
       self.conn.execute('CREATE TABLE IF NOT EXISTS Users (id INTEGER PRIMARY KEY AUTOINCREMENT, username TEXT, firstname TEXT, lastname TEXT, email TEXT, password TEXT)')
 
     def insert(self, username=None, firstname=None, lastname=None, email=None, password=None):
         self.conn.execute('INSERT INTO Users (username, firstname, lastname, email, password) VALUES (?,?,?,?,?)',
                      (username, firstname, lastname, email, password))
         self.conn.commit()
```

### Comparing `mango-framework-0.6.3/mango_framework.egg-info/PKG-INFO` & `mango-framework-0.6.5/mango_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mango-framework
-Version: 0.6.3
+Version: 0.6.5
 Summary: A lightweight and highly customizable Python framework for building web applications
 Home-page: https://github.com/momo-AUX1/mango
 Author: Mohammed
 Author-email: fdlnaal@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `mango-framework-0.6.3/setup.py` & `mango-framework-0.6.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='mango-framework',
-    version='0.6.3',
+    version='0.6.5',
     author='Mohammed',
     author_email='fdlnaal@gmail.com',
     description='A lightweight and highly customizable Python framework for building web applications',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/momo-AUX1/mango',
     packages=['.'],
```

