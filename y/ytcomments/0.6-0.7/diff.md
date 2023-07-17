# Comparing `tmp/ytcomments-0.6.tar.gz` & `tmp/ytcomments-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ytcomments-0.6.tar", last modified: Mon Jul 17 05:33:27 2023, max compression
+gzip compressed data, was "ytcomments-0.7.tar", last modified: Mon Jul 17 05:41:05 2023, max compression
```

## Comparing `ytcomments-0.6.tar` & `ytcomments-0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-17 05:33:27.177654 ytcomments-0.6/
--rw-rw-r--   0 dipson    (1000) dipson    (1000)    35149 2023-07-17 00:55:42.000000 ytcomments-0.6/LICENSE
--rw-rw-r--   0 dipson    (1000) dipson    (1000)     1301 2023-07-17 05:33:27.177654 ytcomments-0.6/PKG-INFO
--rw-rw-r--   0 dipson    (1000) dipson    (1000)      769 2023-07-17 02:08:08.000000 ytcomments-0.6/README.md
--rw-rw-r--   0 dipson    (1000) dipson    (1000)       38 2023-07-17 05:33:27.177654 ytcomments-0.6/setup.cfg
--rw-rw-r--   0 dipson    (1000) dipson    (1000)     1113 2023-07-17 05:33:05.000000 ytcomments-0.6/setup.py
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-17 05:33:27.177654 ytcomments-0.6/src/
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-17 05:33:27.177654 ytcomments-0.6/src/ytcomments/
--rw-rw-r--   0 dipson    (1000) dipson    (1000)     4256 2023-07-17 05:32:31.000000 ytcomments-0.6/src/ytcomments/__init__.py
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-17 05:33:27.177654 ytcomments-0.6/src/ytcomments.egg-info/
--rw-rw-r--   0 dipson    (1000) dipson    (1000)     1301 2023-07-17 05:33:27.000000 ytcomments-0.6/src/ytcomments.egg-info/PKG-INFO
--rw-rw-r--   0 dipson    (1000) dipson    (1000)      283 2023-07-17 05:33:27.000000 ytcomments-0.6/src/ytcomments.egg-info/SOURCES.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)        1 2023-07-17 05:33:27.000000 ytcomments-0.6/src/ytcomments.egg-info/dependency_links.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)       43 2023-07-17 05:33:27.000000 ytcomments-0.6/src/ytcomments.egg-info/entry_points.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)      279 2023-07-17 05:33:27.000000 ytcomments-0.6/src/ytcomments.egg-info/requires.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)       11 2023-07-17 05:33:27.000000 ytcomments-0.6/src/ytcomments.egg-info/top_level.txt
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-17 05:41:05.579056 ytcomments-0.7/
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)    35149 2023-07-17 00:55:42.000000 ytcomments-0.7/LICENSE
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)     1301 2023-07-17 05:41:05.579056 ytcomments-0.7/PKG-INFO
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)      769 2023-07-17 02:08:08.000000 ytcomments-0.7/README.md
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)       38 2023-07-17 05:41:05.579056 ytcomments-0.7/setup.cfg
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)     1132 2023-07-17 05:40:06.000000 ytcomments-0.7/setup.py
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-17 05:41:05.575056 ytcomments-0.7/src/
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-17 05:41:05.579056 ytcomments-0.7/src/ytcomments/
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)     4256 2023-07-17 05:32:31.000000 ytcomments-0.7/src/ytcomments/__init__.py
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-17 05:41:05.579056 ytcomments-0.7/src/ytcomments.egg-info/
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)     1301 2023-07-17 05:41:05.000000 ytcomments-0.7/src/ytcomments.egg-info/PKG-INFO
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)      283 2023-07-17 05:41:05.000000 ytcomments-0.7/src/ytcomments.egg-info/SOURCES.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)        1 2023-07-17 05:41:05.000000 ytcomments-0.7/src/ytcomments.egg-info/dependency_links.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)       43 2023-07-17 05:41:05.000000 ytcomments-0.7/src/ytcomments.egg-info/entry_points.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)      296 2023-07-17 05:41:05.000000 ytcomments-0.7/src/ytcomments.egg-info/requires.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)       11 2023-07-17 05:41:05.000000 ytcomments-0.7/src/ytcomments.egg-info/top_level.txt
```

### Comparing `ytcomments-0.6/LICENSE` & `ytcomments-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ytcomments-0.6/PKG-INFO` & `ytcomments-0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytcomments
-Version: 0.6
+Version: 0.7
 Summary: python package to retreive youtube comments and translate them
 Home-page: https://github.com/dipson94/yt-comments
 Author: Dipson
 Author-email: dipson94.coding@gmail.com
 License: GNU GPL V3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `ytcomments-0.6/README.md` & `ytcomments-0.7/README.md`

 * *Files identical despite different names*

### Comparing `ytcomments-0.6/setup.py` & `ytcomments-0.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup
     
 with open("README.md", "r") as f:
 	long_description = f.read()
 
 setup(
 name="ytcomments",
-version="0.6",
+version="0.7",
 description="python package to retreive youtube comments and translate them",
 package_dir={"": "src"},
 include_package_data=True,
 long_description=long_description,
 long_description_content_type="text/markdown",
 url="https://github.com/dipson94/yt-comments",
 author="Dipson",
 author_email="dipson94.coding@gmail.com",
 license="GNU GPL V3",
 classifiers=["License :: OSI Approved :: GNU General Public License v3 (GPLv3)","Programming Language :: Python :: 3.10","Operating System :: OS Independent"],
-install_requires=["pyperclip >= 1.8.2","tqdm >= 4.65.0","getch >= 1.0","youtube_comment_downloader >= 0.1.68","beautifulsoup4","webencodings","packaging>=21.3","numpy>=1.4","scipy!=1.9.2,>=1.4","importlib-metadata>=3.6","keyring>=15.1","requests-toolbelt!=0.9.0,>=0.8.0","ipython>=7.23.1","matplotlib-inline>=0.1"],
+install_requires=["pyperclip >= 1.8.2","tqdm >= 4.65.0","getch >= 1.0","youtube_comment_downloader >= 0.1.68","beautifulsoup4","webencodings","packaging>=21.3","numpy>=1.4","scipy!=1.9.2,>=1.4","importlib-metadata>=3.6","keyring>=15.1","requests-toolbelt!=0.9.0,>=0.8.0","ipython>=7.23.1","matplotlib-inline>=0.1","translatepy==2.3"],
 extras_require={
         "dev": ["pytest >= 7.0"]
         },
 entry_points={
 'console_scripts': ['ytcmts=ytcomments:main',],},
 python_requires=">=3.10",    
 )
```

### Comparing `ytcomments-0.6/src/ytcomments/__init__.py` & `ytcomments-0.7/src/ytcomments/__init__.py`

 * *Files identical despite different names*

### Comparing `ytcomments-0.6/src/ytcomments.egg-info/PKG-INFO` & `ytcomments-0.7/src/ytcomments.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytcomments
-Version: 0.6
+Version: 0.7
 Summary: python package to retreive youtube comments and translate them
 Home-page: https://github.com/dipson94/yt-comments
 Author: Dipson
 Author-email: dipson94.coding@gmail.com
 License: GNU GPL V3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.10
```

