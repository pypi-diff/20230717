# Comparing `tmp/ytcomments-0.3.tar.gz` & `tmp/ytcomments-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ytcomments-0.3.tar", last modified: Mon Jul 17 01:25:56 2023, max compression
+gzip compressed data, was "ytcomments-0.4.tar", last modified: Mon Jul 17 01:51:06 2023, max compression
```

## Comparing `ytcomments-0.3.tar` & `ytcomments-0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-17 01:25:56.390415 ytcomments-0.3/
--rw-rw-r--   0 dipson    (1000) dipson    (1000)    35149 2023-07-17 00:55:42.000000 ytcomments-0.3/LICENSE
--rw-rw-r--   0 dipson    (1000) dipson    (1000)      544 2023-07-17 01:25:56.390415 ytcomments-0.3/PKG-INFO
--rw-rw-r--   0 dipson    (1000) dipson    (1000)       12 2023-07-17 00:55:06.000000 ytcomments-0.3/README.md
--rw-rw-r--   0 dipson    (1000) dipson    (1000)       38 2023-07-17 01:25:56.390415 ytcomments-0.3/setup.cfg
--rw-rw-r--   0 dipson    (1000) dipson    (1000)     1113 2023-07-17 01:25:47.000000 ytcomments-0.3/setup.py
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-17 01:25:56.386415 ytcomments-0.3/src/
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-17 01:25:56.386415 ytcomments-0.3/src/ytcomments/
--rw-rw-r--   0 dipson    (1000) dipson    (1000)     3894 2023-07-17 01:23:04.000000 ytcomments-0.3/src/ytcomments/__init__.py
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-17 01:25:56.390415 ytcomments-0.3/src/ytcomments.egg-info/
--rw-rw-r--   0 dipson    (1000) dipson    (1000)      544 2023-07-17 01:25:56.000000 ytcomments-0.3/src/ytcomments.egg-info/PKG-INFO
--rw-rw-r--   0 dipson    (1000) dipson    (1000)      283 2023-07-17 01:25:56.000000 ytcomments-0.3/src/ytcomments.egg-info/SOURCES.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)        1 2023-07-17 01:25:56.000000 ytcomments-0.3/src/ytcomments.egg-info/dependency_links.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)       43 2023-07-17 01:25:56.000000 ytcomments-0.3/src/ytcomments.egg-info/entry_points.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)      279 2023-07-17 01:25:56.000000 ytcomments-0.3/src/ytcomments.egg-info/requires.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)       11 2023-07-17 01:25:56.000000 ytcomments-0.3/src/ytcomments.egg-info/top_level.txt
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-17 01:51:06.393229 ytcomments-0.4/
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)    35149 2023-07-17 00:55:42.000000 ytcomments-0.4/LICENSE
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)      544 2023-07-17 01:51:06.393229 ytcomments-0.4/PKG-INFO
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)       12 2023-07-17 00:55:06.000000 ytcomments-0.4/README.md
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)       38 2023-07-17 01:51:06.393229 ytcomments-0.4/setup.cfg
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)     1113 2023-07-17 01:44:43.000000 ytcomments-0.4/setup.py
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-17 01:51:06.389229 ytcomments-0.4/src/
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-17 01:51:06.393229 ytcomments-0.4/src/ytcomments/
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)     4254 2023-07-17 01:50:43.000000 ytcomments-0.4/src/ytcomments/__init__.py
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-17 01:51:06.393229 ytcomments-0.4/src/ytcomments.egg-info/
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)      544 2023-07-17 01:51:06.000000 ytcomments-0.4/src/ytcomments.egg-info/PKG-INFO
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)      283 2023-07-17 01:51:06.000000 ytcomments-0.4/src/ytcomments.egg-info/SOURCES.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)        1 2023-07-17 01:51:06.000000 ytcomments-0.4/src/ytcomments.egg-info/dependency_links.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)       43 2023-07-17 01:51:06.000000 ytcomments-0.4/src/ytcomments.egg-info/entry_points.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)      279 2023-07-17 01:51:06.000000 ytcomments-0.4/src/ytcomments.egg-info/requires.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)       11 2023-07-17 01:51:06.000000 ytcomments-0.4/src/ytcomments.egg-info/top_level.txt
```

### Comparing `ytcomments-0.3/LICENSE` & `ytcomments-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ytcomments-0.3/PKG-INFO` & `ytcomments-0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytcomments
-Version: 0.3
+Version: 0.4
 Summary: python package to retreive youtube comments and translate them
 Home-page: https://github.com/dipson94/yt-comments
 Author: Dipson
 Author-email: dipson94.coding@gmail.com
 License: GNU GPL V3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `ytcomments-0.3/setup.py` & `ytcomments-0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
     
 with open("README.md", "r") as f:
 	long_description = f.read()
 
 setup(
 name="ytcomments",
-version="0.3",
+version="0.4",
 description="python package to retreive youtube comments and translate them",
 package_dir={"": "src"},
 include_package_data=True,
 long_description=long_description,
 long_description_content_type="text/markdown",
 url="https://github.com/dipson94/yt-comments",
 author="Dipson",
```

### Comparing `ytcomments-0.3/src/ytcomments/__init__.py` & `ytcomments-0.4/src/ytcomments/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -32,15 +32,27 @@
 def main():
     global iso_639
     import getch
     import youtube_comment_downloader as downloader
     from itertools import islice
     import pyperclip as pc
     d=downloader.YoutubeCommentDownloader()
-    print("\n Youtube Comments downloader \n")
+    print("""
+                        _________
+                    ________________
+                  _____________________
+               __________________________           
+               
+    ---------> Youtube Comments downloader <---------
+               ___________________________
+                  _____________________
+                     _______________
+                        _________
+    
+    ")
     url=str(input("\nEnter youtube video url : "))
     print("""
     Sort by :
              1 : Popular
              2 : Recent
              
     """)
@@ -105,8 +117,7 @@
         pr=getch.getch()
         if pr=="y":
             for r in tr:
                 print(r)
             print("\n Results copied to clipboard\n")
         else:
             print("\n Results copied to clipboard\n")
-main()
```

### Comparing `ytcomments-0.3/src/ytcomments.egg-info/PKG-INFO` & `ytcomments-0.4/src/ytcomments.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytcomments
-Version: 0.3
+Version: 0.4
 Summary: python package to retreive youtube comments and translate them
 Home-page: https://github.com/dipson94/yt-comments
 Author: Dipson
 Author-email: dipson94.coding@gmail.com
 License: GNU GPL V3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.10
```

