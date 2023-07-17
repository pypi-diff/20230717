# Comparing `tmp/RdQxbAPI-0.1.1.tar.gz` & `tmp/RdQxbAPI-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RdQxbAPI-0.1.1.tar", last modified: Wed Jul  5 02:32:33 2023, max compression
+gzip compressed data, was "RdQxbAPI-0.1.2.tar", last modified: Mon Jul 17 05:50:09 2023, max compression
```

## Comparing `RdQxbAPI-0.1.1.tar` & `RdQxbAPI-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 02:32:33.844096 RdQxbAPI-0.1.1/
--rw-rw-rw-   0        0        0       19 2023-07-05 02:27:45.000000 RdQxbAPI-0.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 RdQxbAPI-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0      374 2023-07-05 02:32:33.845096 RdQxbAPI-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       17 2023-07-05 02:28:57.000000 RdQxbAPI-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-05 02:32:33.804109 RdQxbAPI-0.1.1/RdQxbAPI/
-drwxrwxrwx   0        0        0        0 2023-07-05 02:32:33.836099 RdQxbAPI-0.1.1/RdQxbAPI/Function/
--rw-rw-rw-   0        0        0    83456 2023-07-05 02:09:39.000000 RdQxbAPI-0.1.1/RdQxbAPI/Function/QxbAPIgsgd.pyd
--rw-rw-rw-   0        0        0   113152 2023-07-05 02:09:45.000000 RdQxbAPI-0.1.1/RdQxbAPI/Function/QxbAPIphone.pyd
--rw-rw-rw-   0        0        0   177152 2023-07-05 02:09:53.000000 RdQxbAPI-0.1.1/RdQxbAPI/Function/QxbAPIqylt.pyd
--rw-rw-rw-   0        0        0   115200 2023-07-05 02:09:59.000000 RdQxbAPI-0.1.1/RdQxbAPI/Function/QxbAPIysglf.pyd
--rw-rw-rw-   0        0        0   139264 2023-07-05 02:10:06.000000 RdQxbAPI-0.1.1/RdQxbAPI/Function/QxbAPIzyrytz.pyd
--rw-rw-rw-   0        0        0        0 2023-06-25 08:05:06.000000 RdQxbAPI-0.1.1/RdQxbAPI/Function/__init__.py
--rw-rw-rw-   0        0        0   154624 2023-07-04 10:01:44.000000 RdQxbAPI-0.1.1/RdQxbAPI/RdqxbAPI.pyd
-drwxrwxrwx   0        0        0        0 2023-07-05 02:32:33.842097 RdQxbAPI-0.1.1/RdQxbAPI/UI/
--rw-rw-rw-   0        0        0        0 2023-06-25 08:04:41.000000 RdQxbAPI-0.1.1/RdQxbAPI/UI/__init__.py
--rw-rw-rw-   0        0        0    80384 2023-07-05 02:10:12.000000 RdQxbAPI-0.1.1/RdQxbAPI/UI/qxbUI.pyd
--rw-rw-rw-   0        0        0        0 2023-06-25 09:28:39.000000 RdQxbAPI-0.1.1/RdQxbAPI/__init__.py
--rw-rw-rw-   0        0        0    69632 2023-07-05 02:09:33.000000 RdQxbAPI-0.1.1/RdQxbAPI/optionDb.pyd
-drwxrwxrwx   0        0        0        0 2023-07-05 02:32:33.816139 RdQxbAPI-0.1.1/RdQxbAPI.egg-info/
--rw-rw-rw-   0        0        0      374 2023-07-05 02:32:33.000000 RdQxbAPI-0.1.1/RdQxbAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      490 2023-07-05 02:32:33.000000 RdQxbAPI-0.1.1/RdQxbAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 02:32:33.000000 RdQxbAPI-0.1.1/RdQxbAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-05 02:32:33.000000 RdQxbAPI-0.1.1/RdQxbAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      136 2023-07-05 02:32:33.846096 RdQxbAPI-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1005 2023-07-05 02:30:09.000000 RdQxbAPI-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 05:50:09.381457 RdQxbAPI-0.1.2/
+-rw-rw-rw-   0        0        0       19 2023-07-05 02:27:45.000000 RdQxbAPI-0.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 RdQxbAPI-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      374 2023-07-17 05:50:09.381457 RdQxbAPI-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       17 2023-07-05 02:28:57.000000 RdQxbAPI-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 05:50:09.332258 RdQxbAPI-0.1.2/RdQxbAPI/
+drwxrwxrwx   0        0        0        0 2023-07-17 05:50:09.372005 RdQxbAPI-0.1.2/RdQxbAPI/Function/
+-rw-rw-rw-   0        0        0    83456 2023-07-05 02:09:39.000000 RdQxbAPI-0.1.2/RdQxbAPI/Function/QxbAPIgsgd.pyd
+-rw-rw-rw-   0        0        0   113152 2023-07-05 02:09:45.000000 RdQxbAPI-0.1.2/RdQxbAPI/Function/QxbAPIphone.pyd
+-rw-rw-rw-   0        0        0   177152 2023-07-05 02:09:53.000000 RdQxbAPI-0.1.2/RdQxbAPI/Function/QxbAPIqylt.pyd
+-rw-rw-rw-   0        0        0   115200 2023-07-05 02:09:59.000000 RdQxbAPI-0.1.2/RdQxbAPI/Function/QxbAPIysglf.pyd
+-rw-rw-rw-   0        0        0   139264 2023-07-05 02:10:06.000000 RdQxbAPI-0.1.2/RdQxbAPI/Function/QxbAPIzyrytz.pyd
+-rw-rw-rw-   0        0        0        0 2023-06-25 08:05:06.000000 RdQxbAPI-0.1.2/RdQxbAPI/Function/__init__.py
+-rw-rw-rw-   0        0        0   155136 2023-07-17 05:46:51.000000 RdQxbAPI-0.1.2/RdQxbAPI/RdqxbAPI.pyd
+drwxrwxrwx   0        0        0        0 2023-07-17 05:50:09.377005 RdQxbAPI-0.1.2/RdQxbAPI/UI/
+-rw-rw-rw-   0        0        0        0 2023-06-25 08:04:41.000000 RdQxbAPI-0.1.2/RdQxbAPI/UI/__init__.py
+-rw-rw-rw-   0        0        0    80384 2023-07-05 02:10:12.000000 RdQxbAPI-0.1.2/RdQxbAPI/UI/qxbUI.pyd
+-rw-rw-rw-   0        0        0        0 2023-06-25 09:28:39.000000 RdQxbAPI-0.1.2/RdQxbAPI/__init__.py
+-rw-rw-rw-   0        0        0    69632 2023-07-05 02:09:33.000000 RdQxbAPI-0.1.2/RdQxbAPI/optionDb.pyd
+drwxrwxrwx   0        0        0        0 2023-07-17 05:50:09.346004 RdQxbAPI-0.1.2/RdQxbAPI.egg-info/
+-rw-rw-rw-   0        0        0      374 2023-07-17 05:50:09.000000 RdQxbAPI-0.1.2/RdQxbAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      490 2023-07-17 05:50:09.000000 RdQxbAPI-0.1.2/RdQxbAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 05:50:09.000000 RdQxbAPI-0.1.2/RdQxbAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-17 05:50:09.000000 RdQxbAPI-0.1.2/RdQxbAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      136 2023-07-17 05:50:09.383453 RdQxbAPI-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1005 2023-07-17 05:50:03.000000 RdQxbAPI-0.1.2/setup.py
```

### Comparing `RdQxbAPI-0.1.1/setup.py` & `RdQxbAPI-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 #-*- coding:utf-8 -*-
 import os 
 from setuptools import setup, find_packages
 
 MAJOR = 0
 MINOR = 1
-PATCH = 1
+PATCH = 2
 VERSION = f"{MAJOR}.{MINOR}.{PATCH}"
 
 def get_install_requires():
     reqs = []
     return reqs
 setup(
 	name = "RdQxbAPI",
```

