# Comparing `tmp/noelmode-1.0.2.tar.gz` & `tmp/noelmode-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noelmode-1.0.2.tar", last modified: Mon Jul 17 00:09:26 2023, max compression
+gzip compressed data, was "noelmode-1.0.3.tar", last modified: Mon Jul 17 00:21:40 2023, max compression
```

## Comparing `noelmode-1.0.2.tar` & `noelmode-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:09:26.368594 noelmode-1.0.2/
--rw-r--r--   0 root         (0) root         (0)    35148 2023-07-16 10:33:54.000000 noelmode-1.0.2/COPYING
--rw-r--r--   0 root         (0) root         (0)     7651 2023-07-16 10:33:54.000000 noelmode-1.0.2/COPYING.lesser
--rw-r--r--   0 root         (0) root         (0)      738 2023-07-16 23:40:28.000000 noelmode-1.0.2/NOTICE
--rw-r--r--   0 root         (0) root         (0)     7892 2023-07-17 00:09:26.368594 noelmode-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7063 2023-07-16 23:40:28.000000 noelmode-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:09:26.364593 noelmode-1.0.2/noelmode/
--rw-r--r--   0 root         (0) root         (0)      803 2023-07-16 23:40:28.000000 noelmode-1.0.2/noelmode/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:09:26.368594 noelmode-1.0.2/noelmode.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7892 2023-07-17 00:09:26.000000 noelmode-1.0.2/noelmode.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      228 2023-07-17 00:09:26.000000 noelmode-1.0.2/noelmode.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 00:09:26.000000 noelmode-1.0.2/noelmode.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-17 00:09:26.000000 noelmode-1.0.2/noelmode.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-17 00:09:26.000000 noelmode-1.0.2/noelmode.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-17 00:09:26.368594 noelmode-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1157 2023-07-17 00:09:22.000000 noelmode-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:21:40.823463 noelmode-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)    35148 2023-07-17 00:21:07.000000 noelmode-1.0.3/COPYING
+-rw-r--r--   0 root         (0) root         (0)     7651 2023-07-17 00:21:07.000000 noelmode-1.0.3/COPYING.lesser
+-rw-r--r--   0 root         (0) root         (0)      738 2023-07-17 00:21:07.000000 noelmode-1.0.3/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     7892 2023-07-17 00:21:40.823463 noelmode-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7063 2023-07-17 00:21:07.000000 noelmode-1.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:21:40.823463 noelmode-1.0.3/noelmode/
+-rw-r--r--   0 root         (0) root         (0)      803 2023-07-17 00:21:07.000000 noelmode-1.0.3/noelmode/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:21:40.823463 noelmode-1.0.3/noelmode.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7892 2023-07-17 00:21:40.000000 noelmode-1.0.3/noelmode.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      228 2023-07-17 00:21:40.000000 noelmode-1.0.3/noelmode.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 00:21:40.000000 noelmode-1.0.3/noelmode.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-17 00:21:40.000000 noelmode-1.0.3/noelmode.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-17 00:21:40.000000 noelmode-1.0.3/noelmode.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-17 00:21:40.823463 noelmode-1.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1157 2023-07-17 00:21:07.000000 noelmode-1.0.3/setup.py
```

### Comparing `noelmode-1.0.2/COPYING` & `noelmode-1.0.3/COPYING`

 * *Files identical despite different names*

### Comparing `noelmode-1.0.2/COPYING.lesser` & `noelmode-1.0.3/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `noelmode-1.0.2/NOTICE` & `noelmode-1.0.3/NOTICE`

 * *Files identical despite different names*

### Comparing `noelmode-1.0.2/PKG-INFO` & `noelmode-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: noelmode
-Version: 1.0.2
+Version: 1.0.3
 Summary: pyromod custom
 Home-page: https://github.com/jokokendi/xmode
 Author: jokokendi
 Author-email: ajual7832@gmail.com
 License: MIT
-Download-URL: https://github.com/jokokendi/xmode/archive/v1.0.2.zip
+Download-URL: https://github.com/jokokendi/xmode/archive/v1.0.3.zip
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `noelmode-1.0.2/README.md` & `noelmode-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `noelmode-1.0.2/noelmode/__init__.py` & `noelmode-1.0.3/noelmode/__init__.py`

 * *Files identical despite different names*

### Comparing `noelmode-1.0.2/noelmode.egg-info/PKG-INFO` & `noelmode-1.0.3/noelmode.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: noelmode
-Version: 1.0.2
+Version: 1.0.3
 Summary: pyromod custom
 Home-page: https://github.com/jokokendi/xmode
 Author: jokokendi
 Author-email: ajual7832@gmail.com
 License: MIT
-Download-URL: https://github.com/jokokendi/xmode/archive/v1.0.2.zip
+Download-URL: https://github.com/jokokendi/xmode/archive/v1.0.3.zip
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `noelmode-1.0.2/setup.py` & `noelmode-1.0.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 
 try:
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
 
-version = '1.0.2'
+version = '1.0.3'
 
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name='noelmode',
```

