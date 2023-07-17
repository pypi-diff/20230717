# Comparing `tmp/mango-framework-0.6.5.tar.gz` & `tmp/mango-framework-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mango-framework-0.6.5.tar", last modified: Mon Jul 17 13:27:56 2023, max compression
+gzip compressed data, was "mango-framework-0.6.7.tar", last modified: Mon Jul 17 13:52:55 2023, max compression
```

## Comparing `mango-framework-0.6.5.tar` & `mango-framework-0.6.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 mohammed   (501) staff       (20)        0 2023-07-17 13:27:56.223357 mango-framework-0.6.5/
--rw-r--r--   0 mohammed   (501) staff       (20)     1023 2023-07-17 05:13:07.000000 mango-framework-0.6.5/LICENSE
--rw-r--r--   0 mohammed   (501) staff       (20)     1920 2023-07-17 13:27:56.223245 mango-framework-0.6.5/PKG-INFO
--rw-r--r--   0 mohammed   (501) staff       (20)     1240 2023-07-17 12:32:59.000000 mango-framework-0.6.5/README.md
--rw-r--r--   0 mohammed   (501) staff       (20)     6285 2023-07-17 13:25:38.000000 mango-framework-0.6.5/mango.py
-drwxr-xr-x   0 mohammed   (501) staff       (20)        0 2023-07-17 13:27:56.223071 mango-framework-0.6.5/mango_framework.egg-info/
--rw-r--r--   0 mohammed   (501) staff       (20)     1920 2023-07-17 13:27:56.000000 mango-framework-0.6.5/mango_framework.egg-info/PKG-INFO
--rw-r--r--   0 mohammed   (501) staff       (20)      191 2023-07-17 13:27:56.000000 mango-framework-0.6.5/mango_framework.egg-info/SOURCES.txt
--rw-r--r--   0 mohammed   (501) staff       (20)        1 2023-07-17 13:27:56.000000 mango-framework-0.6.5/mango_framework.egg-info/dependency_links.txt
--rw-r--r--   0 mohammed   (501) staff       (20)        1 2023-07-17 13:27:56.000000 mango-framework-0.6.5/mango_framework.egg-info/top_level.txt
--rw-r--r--   0 mohammed   (501) staff       (20)       38 2023-07-17 13:27:56.223401 mango-framework-0.6.5/setup.cfg
--rw-r--r--   0 mohammed   (501) staff       (20)      869 2023-07-17 13:27:12.000000 mango-framework-0.6.5/setup.py
+drwxr-xr-x   0 mohammed   (501) staff       (20)        0 2023-07-17 13:52:55.037893 mango-framework-0.6.7/
+-rw-r--r--   0 mohammed   (501) staff       (20)     1023 2023-07-17 05:13:07.000000 mango-framework-0.6.7/LICENSE
+-rw-r--r--   0 mohammed   (501) staff       (20)     1920 2023-07-17 13:52:55.037776 mango-framework-0.6.7/PKG-INFO
+-rw-r--r--   0 mohammed   (501) staff       (20)     1240 2023-07-17 12:32:59.000000 mango-framework-0.6.7/README.md
+-rw-r--r--   0 mohammed   (501) staff       (20)     6351 2023-07-17 13:49:28.000000 mango-framework-0.6.7/mango.py
+drwxr-xr-x   0 mohammed   (501) staff       (20)        0 2023-07-17 13:52:55.037612 mango-framework-0.6.7/mango_framework.egg-info/
+-rw-r--r--   0 mohammed   (501) staff       (20)     1920 2023-07-17 13:52:55.000000 mango-framework-0.6.7/mango_framework.egg-info/PKG-INFO
+-rw-r--r--   0 mohammed   (501) staff       (20)      191 2023-07-17 13:52:55.000000 mango-framework-0.6.7/mango_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 mohammed   (501) staff       (20)        1 2023-07-17 13:52:55.000000 mango-framework-0.6.7/mango_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 mohammed   (501) staff       (20)        1 2023-07-17 13:52:55.000000 mango-framework-0.6.7/mango_framework.egg-info/top_level.txt
+-rw-r--r--   0 mohammed   (501) staff       (20)       38 2023-07-17 13:52:55.037933 mango-framework-0.6.7/setup.cfg
+-rw-r--r--   0 mohammed   (501) staff       (20)      869 2023-07-17 13:52:22.000000 mango-framework-0.6.7/setup.py
```

### Comparing `mango-framework-0.6.5/LICENSE` & `mango-framework-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mango-framework-0.6.5/PKG-INFO` & `mango-framework-0.6.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mango-framework
-Version: 0.6.5
+Version: 0.6.7
 Summary: A lightweight and highly customizable Python framework for building web applications
 Home-page: https://github.com/momo-AUX1/mango
 Author: Mohammed
 Author-email: fdlnaal@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `mango-framework-0.6.5/README.md` & `mango-framework-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `mango-framework-0.6.5/mango.py` & `mango-framework-0.6.7/mango.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,14 +111,19 @@
   return json.loads(data)
 
 
 def send_json(data):
   return json.dumps(data), 'application/json'
 
 
+def get_data(info,query):
+  data = info[query][0]
+  return data
+
+
 def send_file(path):
   try:
     with open(join(files_path, path), 'rb') as f:
       response = f.read()
   except:
     with open(path, 'rb') as f:
       response = f.read()
@@ -172,15 +177,15 @@
         }
     </style>
 </head>
 <body>
     <h1>Server successfully started, but there are no routes or the "/" route is empty</h1>
     <img class="mango-img" src="https://th.bing.com/th/id/R.54bad49b520690f3858b1f396194779d?rik=QSeITH3EbHg4Vw&pid=ImgRaw&r=0" alt="Mango">
     <footer>
-        Version: 0.6.5
+        Version: 0.6.7
         <br>
         <a class="link" href="https://pypi.org/project/mango-framework/">Check out the development!</a>
     </footer>
 </body>
 </html>
 """
```

### Comparing `mango-framework-0.6.5/mango_framework.egg-info/PKG-INFO` & `mango-framework-0.6.7/mango_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mango-framework
-Version: 0.6.5
+Version: 0.6.7
 Summary: A lightweight and highly customizable Python framework for building web applications
 Home-page: https://github.com/momo-AUX1/mango
 Author: Mohammed
 Author-email: fdlnaal@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `mango-framework-0.6.5/setup.py` & `mango-framework-0.6.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='mango-framework',
-    version='0.6.5',
+    version='0.6.7',
     author='Mohammed',
     author_email='fdlnaal@gmail.com',
     description='A lightweight and highly customizable Python framework for building web applications',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/momo-AUX1/mango',
     packages=['.'],
```

