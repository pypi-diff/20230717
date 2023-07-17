# Comparing `tmp/tigersyn-0.0.2b0.tar.gz` & `tmp/tigersyn-0.0.2rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tigersyn-0.0.2b0.tar", last modified: Mon Jul 17 09:50:36 2023, max compression
+gzip compressed data, was "tigersyn-0.0.2rc0.tar", last modified: Mon Jul 17 09:53:53 2023, max compression
```

## Comparing `tigersyn-0.0.2b0.tar` & `tigersyn-0.0.2rc0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 09:50:36.324725 tigersyn-0.0.2b0/
--rw-rw-rw-   0        0        0     1088 2023-07-17 07:49:07.000000 tigersyn-0.0.2b0/LICENSE
--rw-rw-rw-   0        0        0      757 2023-07-17 09:50:36.323683 tigersyn-0.0.2b0/PKG-INFO
--rw-rw-rw-   0        0        0      261 2023-07-17 07:50:52.000000 tigersyn-0.0.2b0/README.md
--rw-rw-rw-   0        0        0       88 2023-07-17 06:43:23.000000 tigersyn-0.0.2b0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-17 09:50:36.325684 tigersyn-0.0.2b0/setup.cfg
--rw-rw-rw-   0        0        0      908 2023-07-17 09:49:35.000000 tigersyn-0.0.2b0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:50:36.281678 tigersyn-0.0.2b0/tigersyn/
--rw-rw-rw-   0        0        0       28 2023-07-17 09:40:04.000000 tigersyn-0.0.2b0/tigersyn/__init__.py
--rw-rw-rw-   0        0        0     2252 2023-07-17 09:43:55.000000 tigersyn-0.0.2b0/tigersyn/syn.py
--rw-rw-rw-   0        0        0     4006 2023-07-17 08:49:05.000000 tigersyn-0.0.2b0/tigersyn/syn_tool.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:50:36.321685 tigersyn-0.0.2b0/tigersyn.egg-info/
--rw-rw-rw-   0        0        0      757 2023-07-17 09:50:36.000000 tigersyn-0.0.2b0/tigersyn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-07-17 09:50:36.000000 tigersyn-0.0.2b0/tigersyn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 09:50:36.000000 tigersyn-0.0.2b0/tigersyn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-07-17 09:50:36.000000 tigersyn-0.0.2b0/tigersyn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-17 09:50:36.000000 tigersyn-0.0.2b0/tigersyn.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 09:53:53.261006 tigersyn-0.0.2rc0/
+-rw-rw-rw-   0        0        0     1088 2023-07-17 07:49:07.000000 tigersyn-0.0.2rc0/LICENSE
+-rw-rw-rw-   0        0        0      758 2023-07-17 09:53:53.260011 tigersyn-0.0.2rc0/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2023-07-17 07:50:52.000000 tigersyn-0.0.2rc0/README.md
+-rw-rw-rw-   0        0        0       88 2023-07-17 06:43:23.000000 tigersyn-0.0.2rc0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-17 09:53:53.261006 tigersyn-0.0.2rc0/setup.cfg
+-rw-rw-rw-   0        0        0      908 2023-07-17 09:53:44.000000 tigersyn-0.0.2rc0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:53:53.235012 tigersyn-0.0.2rc0/tigersyn/
+-rw-rw-rw-   0        0        0       28 2023-07-17 09:40:04.000000 tigersyn-0.0.2rc0/tigersyn/__init__.py
+-rw-rw-rw-   0        0        0     2252 2023-07-17 09:43:55.000000 tigersyn-0.0.2rc0/tigersyn/syn.py
+-rw-rw-rw-   0        0        0     3948 2023-07-17 09:52:58.000000 tigersyn-0.0.2rc0/tigersyn/syn_tool.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:53:53.258015 tigersyn-0.0.2rc0/tigersyn.egg-info/
+-rw-rw-rw-   0        0        0      758 2023-07-17 09:53:53.000000 tigersyn-0.0.2rc0/tigersyn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-07-17 09:53:53.000000 tigersyn-0.0.2rc0/tigersyn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 09:53:53.000000 tigersyn-0.0.2rc0/tigersyn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-07-17 09:53:53.000000 tigersyn-0.0.2rc0/tigersyn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-17 09:53:53.000000 tigersyn-0.0.2rc0/tigersyn.egg-info/top_level.txt
```

### Comparing `tigersyn-0.0.2b0/LICENSE` & `tigersyn-0.0.2rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `tigersyn-0.0.2b0/PKG-INFO` & `tigersyn-0.0.2rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tigersyn
-Version: 0.0.2b0
+Version: 0.0.2rc0
 Summary: Processing MRI images based on deep-learning
 Home-page: https://github.com/StanleyWangTW/tigersyn
 Author: X. S. Wang
 Author-email: 
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tigersyn-0.0.2b0/setup.py` & `tigersyn-0.0.2rc0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-VESION = '0.0.2b'
+VESION = '0.0.2c'
 DESCRIPTION = 'Processing MRI images based on deep-learning'
 CLASSIFIERS = [
     'Intended Audience :: Developers',
     'Programming Language :: Python :: 3.9',
     'License :: OSI Approved :: MIT License',
     "Operating System :: Microsoft :: Windows"
 ]
```

### Comparing `tigersyn-0.0.2b0/tigersyn/syn.py` & `tigersyn-0.0.2rc0/tigersyn/syn.py`

 * *Files identical despite different names*

### Comparing `tigersyn-0.0.2b0/tigersyn/syn_tool.py` & `tigersyn-0.0.2rc0/tigersyn/syn_tool.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,15 +43,14 @@
 
 def download(url, file_name):
     import urllib.request
     import certifi
     import shutil
     import ssl
     context = ssl.create_default_context(cafile=certifi.where())
-    #urllib.request.urlopen(url, cafile=certifi.where())
     with urllib.request.urlopen(url,
                                 context=context) as response, open(file_name, 'wb') as out_file:
         shutil.copyfileobj(response, out_file)
 
 def get_model(f):
     if isfile(f):
         return f
```

### Comparing `tigersyn-0.0.2b0/tigersyn.egg-info/PKG-INFO` & `tigersyn-0.0.2rc0/tigersyn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tigersyn
-Version: 0.0.2b0
+Version: 0.0.2rc0
 Summary: Processing MRI images based on deep-learning
 Home-page: https://github.com/StanleyWangTW/tigersyn
 Author: X. S. Wang
 Author-email: 
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

