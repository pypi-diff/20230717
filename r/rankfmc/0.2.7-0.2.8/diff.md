# Comparing `tmp/rankfmc-0.2.7.tar.gz` & `tmp/rankfmc-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rankfmc-0.2.7.tar", last modified: Wed Jul 12 09:14:34 2023, max compression
+gzip compressed data, was "dist/rankfmc-0.2.8.tar", last modified: Mon Jul 17 01:21:33 2023, max compression
```

## Comparing `rankfmc-0.2.7.tar` & `rankfmc-0.2.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 09:14:34.031236 rankfmc-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-07-12 09:14:17.000000 rankfmc-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       98 2023-07-12 09:14:17.000000 rankfmc-0.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    10339 2023-07-12 09:14:34.031236 rankfmc-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     9746 2023-07-12 09:14:17.000000 rankfmc-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 09:14:34.031236 rankfmc-0.2.7/rankfmc/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 09:14:17.000000 rankfmc-0.2.7/rankfmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)  1052362 2023-07-12 09:14:33.000000 rankfmc-0.2.7/rankfmc/_rankfm.c
--rw-r--r--   0 runner    (1001) docker     (122)     9296 2023-07-12 09:14:17.000000 rankfmc-0.2.7/rankfmc/evaluation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 09:14:34.031236 rankfmc-0.2.7/rankfmc/mt19937ar/
--rw-r--r--   0 runner    (1001) docker     (122)     5923 2023-07-12 09:14:17.000000 rankfmc-0.2.7/rankfmc/mt19937ar/mt19937ar.c
--rw-r--r--   0 runner    (1001) docker     (122)    21516 2023-07-12 09:14:17.000000 rankfmc-0.2.7/rankfmc/rankfm.py
--rw-r--r--   0 runner    (1001) docker     (122)      511 2023-07-12 09:14:17.000000 rankfmc-0.2.7/rankfmc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 09:14:34.031236 rankfmc-0.2.7/rankfmc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    10339 2023-07-12 09:14:33.000000 rankfmc-0.2.7/rankfmc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      347 2023-07-12 09:14:34.000000 rankfmc-0.2.7/rankfmc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-12 09:14:33.000000 rankfmc-0.2.7/rankfmc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-12 09:14:33.000000 rankfmc-0.2.7/rankfmc.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       24 2023-07-12 09:14:33.000000 rankfmc-0.2.7/rankfmc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-07-12 09:14:33.000000 rankfmc-0.2.7/rankfmc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-12 09:14:34.031236 rankfmc-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2263 2023-07-12 09:14:17.000000 rankfmc-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 01:21:33.000000 rankfmc-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-07-17 01:21:18.000000 rankfmc-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       98 2023-07-17 01:21:18.000000 rankfmc-0.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    10339 2023-07-17 01:21:33.000000 rankfmc-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     9746 2023-07-17 01:21:18.000000 rankfmc-0.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 01:21:33.000000 rankfmc-0.2.8/rankfmc/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 01:21:18.000000 rankfmc-0.2.8/rankfmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)  1052362 2023-07-17 01:21:33.000000 rankfmc-0.2.8/rankfmc/_rankfm.c
+-rw-r--r--   0 runner    (1001) docker     (122)     9296 2023-07-17 01:21:18.000000 rankfmc-0.2.8/rankfmc/evaluation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 01:21:33.000000 rankfmc-0.2.8/rankfmc/mt19937ar/
+-rw-r--r--   0 runner    (1001) docker     (122)     5923 2023-07-17 01:21:18.000000 rankfmc-0.2.8/rankfmc/mt19937ar/mt19937ar.c
+-rw-r--r--   0 runner    (1001) docker     (122)    21516 2023-07-17 01:21:18.000000 rankfmc-0.2.8/rankfmc/rankfm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      511 2023-07-17 01:21:18.000000 rankfmc-0.2.8/rankfmc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 01:21:33.000000 rankfmc-0.2.8/rankfmc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    10339 2023-07-17 01:21:33.000000 rankfmc-0.2.8/rankfmc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      347 2023-07-17 01:21:33.000000 rankfmc-0.2.8/rankfmc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-17 01:21:33.000000 rankfmc-0.2.8/rankfmc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-17 01:21:33.000000 rankfmc-0.2.8/rankfmc.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-07-17 01:21:33.000000 rankfmc-0.2.8/rankfmc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-07-17 01:21:33.000000 rankfmc-0.2.8/rankfmc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-17 01:21:33.000000 rankfmc-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2263 2023-07-17 01:21:18.000000 rankfmc-0.2.8/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `rankfmc-0.2.7/LICENSE` & `rankfmc-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `rankfmc-0.2.7/PKG-INFO` & `rankfmc-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: rankfmc
-Version: 0.2.7
+Version: 0.2.8
 Summary: a python implementation of the generic factorization machines model class adapted for collaborative filtering recommendation problems with implicit feedback user-item interaction data and (optionally) additional user/item side features
 Home-page: https://github.com/ErraticO/rankfmc
 Author: ErraticO
 Author-email: wyh123132@163.com
 License: GNU General Public License v3.0
 Keywords: machine,learning,recommendation,factorization,machines,implicit
-Requires-Python: >=3.9
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # RankFM
 
 [![PyPI version](https://badge.fury.io/py/rankfm.svg)](https://badge.fury.io/py/rankfm)
 [![CircleCI](https://circleci.com/gh/etlundquist/rankfm.svg?style=shield)](https://circleci.com/gh/etlundquist/rankfm)
```

### Comparing `rankfmc-0.2.7/README.md` & `rankfmc-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `rankfmc-0.2.7/rankfmc/_rankfm.c` & `rankfmc-0.2.8/rankfmc/_rankfm.c`

 * *Files identical despite different names*

### Comparing `rankfmc-0.2.7/rankfmc/evaluation.py` & `rankfmc-0.2.8/rankfmc/evaluation.py`

 * *Files identical despite different names*

### Comparing `rankfmc-0.2.7/rankfmc/mt19937ar/mt19937ar.c` & `rankfmc-0.2.8/rankfmc/mt19937ar/mt19937ar.c`

 * *Files identical despite different names*

### Comparing `rankfmc-0.2.7/rankfmc/rankfm.py` & `rankfmc-0.2.8/rankfmc/rankfm.py`

 * *Files identical despite different names*

### Comparing `rankfmc-0.2.7/rankfmc.egg-info/PKG-INFO` & `rankfmc-0.2.8/rankfmc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: rankfmc
-Version: 0.2.7
+Version: 0.2.8
 Summary: a python implementation of the generic factorization machines model class adapted for collaborative filtering recommendation problems with implicit feedback user-item interaction data and (optionally) additional user/item side features
 Home-page: https://github.com/ErraticO/rankfmc
 Author: ErraticO
 Author-email: wyh123132@163.com
 License: GNU General Public License v3.0
 Keywords: machine,learning,recommendation,factorization,machines,implicit
-Requires-Python: >=3.9
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # RankFM
 
 [![PyPI version](https://badge.fury.io/py/rankfm.svg)](https://badge.fury.io/py/rankfm)
 [![CircleCI](https://circleci.com/gh/etlundquist/rankfm.svg?style=shield)](https://circleci.com/gh/etlundquist/rankfm)
```

### Comparing `rankfmc-0.2.7/setup.py` & `rankfmc-0.2.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import sys
 import glob
 from setuptools import Extension, setup
 
 NAME = 'rankfmc'
-VERSION = '0.2.7'
+VERSION = '0.2.8'
 
 # define the extension packages to include
 # ----------------------------------------
 
 # prefer the generated C extensions when building
 if glob.glob('rankfmc/_rankfm.c'):
     print("building extensions with pre-generated C source...")
@@ -59,13 +59,13 @@
     author_email='wyh123132@163.com',
     url='https://github.com/ErraticO/rankfmc',
     keywords=['machine', 'learning', 'recommendation', 'factorization', 'machines', 'implicit'],
     license='GNU General Public License v3.0',
     packages=['rankfmc'],
     ext_modules=extensions,
     zip_safe=False,
-    python_requires='>=3.9',
+    python_requires='>=3.6',
     install_requires=['numpy>=1.15', 'pandas>=1.5'],
     long_description=long_description,
     long_description_content_type="text/markdown",
 )
```

