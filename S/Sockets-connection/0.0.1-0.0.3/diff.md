# Comparing `tmp/Sockets_connection-0.0.1.tar.gz` & `tmp/Sockets_connection-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Sockets_connection-0.0.1.tar", last modified: Mon Jul 17 13:14:41 2023, max compression
+gzip compressed data, was "Sockets_connection-0.0.3.tar", last modified: Mon Jul 17 13:18:30 2023, max compression
```

## Comparing `Sockets_connection-0.0.1.tar` & `Sockets_connection-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,11 @@
-drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-07-17 13:14:41.149843 Sockets_connection-0.0.1/
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      552 2023-07-17 13:14:41.149843 Sockets_connection-0.0.1/PKG-INFO
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-07-17 12:49:20.000000 Sockets_connection-0.0.1/README.md
-drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-07-17 13:14:41.149843 Sockets_connection-0.0.1/Sockets_connection.egg-info/
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      552 2023-07-17 13:14:41.000000 Sockets_connection-0.0.1/Sockets_connection.egg-info/PKG-INFO
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      272 2023-07-17 13:14:41.000000 Sockets_connection-0.0.1/Sockets_connection.egg-info/SOURCES.txt
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        1 2023-07-17 13:14:41.000000 Sockets_connection-0.0.1/Sockets_connection.egg-info/dependency_links.txt
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       57 2023-07-17 13:14:41.000000 Sockets_connection-0.0.1/Sockets_connection.egg-info/entry_points.txt
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        8 2023-07-17 13:14:41.000000 Sockets_connection-0.0.1/Sockets_connection.egg-info/requires.txt
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        1 2023-07-17 13:14:41.000000 Sockets_connection-0.0.1/Sockets_connection.egg-info/top_level.txt
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       38 2023-07-17 13:14:41.149843 Sockets_connection-0.0.1/setup.cfg
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      880 2023-07-17 13:06:20.000000 Sockets_connection-0.0.1/setup.py
+drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-07-17 13:18:30.847346 Sockets_connection-0.0.3/
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      552 2023-07-17 13:18:30.847346 Sockets_connection-0.0.3/PKG-INFO
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-07-17 12:49:20.000000 Sockets_connection-0.0.3/README.md
+drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-07-17 13:18:30.847346 Sockets_connection-0.0.3/Sockets_connection.egg-info/
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      552 2023-07-17 13:18:30.000000 Sockets_connection-0.0.3/Sockets_connection.egg-info/PKG-INFO
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      227 2023-07-17 13:18:30.000000 Sockets_connection-0.0.3/Sockets_connection.egg-info/SOURCES.txt
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        1 2023-07-17 13:18:30.000000 Sockets_connection-0.0.3/Sockets_connection.egg-info/dependency_links.txt
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        8 2023-07-17 13:18:30.000000 Sockets_connection-0.0.3/Sockets_connection.egg-info/requires.txt
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        1 2023-07-17 13:18:30.000000 Sockets_connection-0.0.3/Sockets_connection.egg-info/top_level.txt
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       38 2023-07-17 13:18:30.847346 Sockets_connection-0.0.3/setup.cfg
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      762 2023-07-17 13:18:28.000000 Sockets_connection-0.0.3/setup.py
```

### Comparing `Sockets_connection-0.0.1/PKG-INFO` & `Sockets_connection-0.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Sockets_connection
-Version: 0.0.1
+Version: 0.0.3
 Summary: Connect the Multiple devices using Python Sockets with simple ways
 Home-page: https://git.selfmade.ninja/SRIDHARDSCV/sockets-python
 Author: Sridhar
 Author-email: sridhardscv@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Sockets_connection-0.0.1/Sockets_connection.egg-info/PKG-INFO` & `Sockets_connection-0.0.3/Sockets_connection.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Sockets-connection
-Version: 0.0.1
+Version: 0.0.3
 Summary: Connect the Multiple devices using Python Sockets with simple ways
 Home-page: https://git.selfmade.ninja/SRIDHARDSCV/sockets-python
 Author: Sridhar
 Author-email: sridhardscv@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Sockets_connection-0.0.1/setup.py` & `Sockets_connection-0.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,26 @@
 from setuptools import setup
 
 with open("README.md", "r") as readme:
     long_description = readme.read()
 
 setup (
     name="Sockets_connection",
-    version='0.0.1',
+    version='0.0.3',
     author="Sridhar",
     url="https://git.selfmade.ninja/SRIDHARDSCV/sockets-python",
     author_email="sridhardscv@gmail.com",
     description="Connect the Multiple devices using Python Sockets with simple ways",
     long_description=long_description,
     long_description_content_type="text/markdown",
+    install_requires = [
+        "sockets"
+    ],
+    python_requires=">=3.6",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Development Status :: 4 - Beta"
-    ],
-    install_requires = [
-        "sockets"
-    ],
-    python_requires=">=3.6",
-    entry_points={
-        'console_scripts': [
-            'Sockets_connection=main.main:Socket',
-        ],
-    }
-
+    ]
 )
```

