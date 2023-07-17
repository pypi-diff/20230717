# Comparing `tmp/ytcomments-0.5.tar.gz` & `tmp/ytcomments-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ytcomments-0.5.tar", last modified: Mon Jul 17 02:11:05 2023, max compression
+gzip compressed data, was "ytcomments-0.6.tar", last modified: Mon Jul 17 05:33:27 2023, max compression
```

## Comparing `ytcomments-0.5.tar` & `ytcomments-0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-17 02:11:05.373895 ytcomments-0.5/
--rw-rw-r--   0 dipson    (1000) dipson    (1000)    35149 2023-07-17 00:55:42.000000 ytcomments-0.5/LICENSE
--rw-rw-r--   0 dipson    (1000) dipson    (1000)     1301 2023-07-17 02:11:05.373895 ytcomments-0.5/PKG-INFO
--rw-rw-r--   0 dipson    (1000) dipson    (1000)      769 2023-07-17 02:08:08.000000 ytcomments-0.5/README.md
--rw-rw-r--   0 dipson    (1000) dipson    (1000)       38 2023-07-17 02:11:05.373895 ytcomments-0.5/setup.cfg
--rw-rw-r--   0 dipson    (1000) dipson    (1000)     1113 2023-07-17 02:10:55.000000 ytcomments-0.5/setup.py
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-17 02:11:05.373895 ytcomments-0.5/src/
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-17 02:11:05.373895 ytcomments-0.5/src/ytcomments/
--rw-rw-r--   0 dipson    (1000) dipson    (1000)     4254 2023-07-17 01:50:43.000000 ytcomments-0.5/src/ytcomments/__init__.py
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-17 02:11:05.373895 ytcomments-0.5/src/ytcomments.egg-info/
--rw-rw-r--   0 dipson    (1000) dipson    (1000)     1301 2023-07-17 02:11:05.000000 ytcomments-0.5/src/ytcomments.egg-info/PKG-INFO
--rw-rw-r--   0 dipson    (1000) dipson    (1000)      283 2023-07-17 02:11:05.000000 ytcomments-0.5/src/ytcomments.egg-info/SOURCES.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)        1 2023-07-17 02:11:05.000000 ytcomments-0.5/src/ytcomments.egg-info/dependency_links.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)       43 2023-07-17 02:11:05.000000 ytcomments-0.5/src/ytcomments.egg-info/entry_points.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)      279 2023-07-17 02:11:05.000000 ytcomments-0.5/src/ytcomments.egg-info/requires.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)       11 2023-07-17 02:11:05.000000 ytcomments-0.5/src/ytcomments.egg-info/top_level.txt
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-17 05:33:27.177654 ytcomments-0.6/
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)    35149 2023-07-17 00:55:42.000000 ytcomments-0.6/LICENSE
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)     1301 2023-07-17 05:33:27.177654 ytcomments-0.6/PKG-INFO
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)      769 2023-07-17 02:08:08.000000 ytcomments-0.6/README.md
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)       38 2023-07-17 05:33:27.177654 ytcomments-0.6/setup.cfg
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)     1113 2023-07-17 05:33:05.000000 ytcomments-0.6/setup.py
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-17 05:33:27.177654 ytcomments-0.6/src/
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-17 05:33:27.177654 ytcomments-0.6/src/ytcomments/
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)     4256 2023-07-17 05:32:31.000000 ytcomments-0.6/src/ytcomments/__init__.py
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-17 05:33:27.177654 ytcomments-0.6/src/ytcomments.egg-info/
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)     1301 2023-07-17 05:33:27.000000 ytcomments-0.6/src/ytcomments.egg-info/PKG-INFO
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)      283 2023-07-17 05:33:27.000000 ytcomments-0.6/src/ytcomments.egg-info/SOURCES.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)        1 2023-07-17 05:33:27.000000 ytcomments-0.6/src/ytcomments.egg-info/dependency_links.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)       43 2023-07-17 05:33:27.000000 ytcomments-0.6/src/ytcomments.egg-info/entry_points.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)      279 2023-07-17 05:33:27.000000 ytcomments-0.6/src/ytcomments.egg-info/requires.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)       11 2023-07-17 05:33:27.000000 ytcomments-0.6/src/ytcomments.egg-info/top_level.txt
```

### Comparing `ytcomments-0.5/LICENSE` & `ytcomments-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ytcomments-0.5/PKG-INFO` & `ytcomments-0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytcomments
-Version: 0.5
+Version: 0.6
 Summary: python package to retreive youtube comments and translate them
 Home-page: https://github.com/dipson94/yt-comments
 Author: Dipson
 Author-email: dipson94.coding@gmail.com
 License: GNU GPL V3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `ytcomments-0.5/README.md` & `ytcomments-0.6/README.md`

 * *Files identical despite different names*

### Comparing `ytcomments-0.5/setup.py` & `ytcomments-0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
     
 with open("README.md", "r") as f:
 	long_description = f.read()
 
 setup(
 name="ytcomments",
-version="0.5",
+version="0.6",
 description="python package to retreive youtube comments and translate them",
 package_dir={"": "src"},
 include_package_data=True,
 long_description=long_description,
 long_description_content_type="text/markdown",
 url="https://github.com/dipson94/yt-comments",
 author="Dipson",
```

### Comparing `ytcomments-0.5/src/ytcomments/__init__.py` & `ytcomments-0.6/src/ytcomments/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
                
     ---------> Youtube Comments downloader <---------
                ___________________________
                   _____________________
                      _______________
                         _________
     
-    ")
+    """)
     url=str(input("\nEnter youtube video url : "))
     print("""
     Sort by :
              1 : Popular
              2 : Recent
              
     """)
```

### Comparing `ytcomments-0.5/src/ytcomments.egg-info/PKG-INFO` & `ytcomments-0.6/src/ytcomments.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytcomments
-Version: 0.5
+Version: 0.6
 Summary: python package to retreive youtube comments and translate them
 Home-page: https://github.com/dipson94/yt-comments
 Author: Dipson
 Author-email: dipson94.coding@gmail.com
 License: GNU GPL V3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.10
```

