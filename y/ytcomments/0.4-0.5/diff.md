# Comparing `tmp/ytcomments-0.4.tar.gz` & `tmp/ytcomments-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ytcomments-0.4.tar", last modified: Mon Jul 17 01:51:06 2023, max compression
+gzip compressed data, was "ytcomments-0.5.tar", last modified: Mon Jul 17 02:11:05 2023, max compression
```

## Comparing `ytcomments-0.4.tar` & `ytcomments-0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-17 01:51:06.393229 ytcomments-0.4/
--rw-rw-r--   0 dipson    (1000) dipson    (1000)    35149 2023-07-17 00:55:42.000000 ytcomments-0.4/LICENSE
--rw-rw-r--   0 dipson    (1000) dipson    (1000)      544 2023-07-17 01:51:06.393229 ytcomments-0.4/PKG-INFO
--rw-rw-r--   0 dipson    (1000) dipson    (1000)       12 2023-07-17 00:55:06.000000 ytcomments-0.4/README.md
--rw-rw-r--   0 dipson    (1000) dipson    (1000)       38 2023-07-17 01:51:06.393229 ytcomments-0.4/setup.cfg
--rw-rw-r--   0 dipson    (1000) dipson    (1000)     1113 2023-07-17 01:44:43.000000 ytcomments-0.4/setup.py
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-17 01:51:06.389229 ytcomments-0.4/src/
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-17 01:51:06.393229 ytcomments-0.4/src/ytcomments/
--rw-rw-r--   0 dipson    (1000) dipson    (1000)     4254 2023-07-17 01:50:43.000000 ytcomments-0.4/src/ytcomments/__init__.py
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-17 01:51:06.393229 ytcomments-0.4/src/ytcomments.egg-info/
--rw-rw-r--   0 dipson    (1000) dipson    (1000)      544 2023-07-17 01:51:06.000000 ytcomments-0.4/src/ytcomments.egg-info/PKG-INFO
--rw-rw-r--   0 dipson    (1000) dipson    (1000)      283 2023-07-17 01:51:06.000000 ytcomments-0.4/src/ytcomments.egg-info/SOURCES.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)        1 2023-07-17 01:51:06.000000 ytcomments-0.4/src/ytcomments.egg-info/dependency_links.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)       43 2023-07-17 01:51:06.000000 ytcomments-0.4/src/ytcomments.egg-info/entry_points.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)      279 2023-07-17 01:51:06.000000 ytcomments-0.4/src/ytcomments.egg-info/requires.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)       11 2023-07-17 01:51:06.000000 ytcomments-0.4/src/ytcomments.egg-info/top_level.txt
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-17 02:11:05.373895 ytcomments-0.5/
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)    35149 2023-07-17 00:55:42.000000 ytcomments-0.5/LICENSE
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)     1301 2023-07-17 02:11:05.373895 ytcomments-0.5/PKG-INFO
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)      769 2023-07-17 02:08:08.000000 ytcomments-0.5/README.md
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)       38 2023-07-17 02:11:05.373895 ytcomments-0.5/setup.cfg
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)     1113 2023-07-17 02:10:55.000000 ytcomments-0.5/setup.py
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-17 02:11:05.373895 ytcomments-0.5/src/
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-17 02:11:05.373895 ytcomments-0.5/src/ytcomments/
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)     4254 2023-07-17 01:50:43.000000 ytcomments-0.5/src/ytcomments/__init__.py
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-17 02:11:05.373895 ytcomments-0.5/src/ytcomments.egg-info/
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)     1301 2023-07-17 02:11:05.000000 ytcomments-0.5/src/ytcomments.egg-info/PKG-INFO
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)      283 2023-07-17 02:11:05.000000 ytcomments-0.5/src/ytcomments.egg-info/SOURCES.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)        1 2023-07-17 02:11:05.000000 ytcomments-0.5/src/ytcomments.egg-info/dependency_links.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)       43 2023-07-17 02:11:05.000000 ytcomments-0.5/src/ytcomments.egg-info/entry_points.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)      279 2023-07-17 02:11:05.000000 ytcomments-0.5/src/ytcomments.egg-info/requires.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)       11 2023-07-17 02:11:05.000000 ytcomments-0.5/src/ytcomments.egg-info/top_level.txt
```

### Comparing `ytcomments-0.4/LICENSE` & `ytcomments-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ytcomments-0.4/setup.py` & `ytcomments-0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
     
 with open("README.md", "r") as f:
 	long_description = f.read()
 
 setup(
 name="ytcomments",
-version="0.4",
+version="0.5",
 description="python package to retreive youtube comments and translate them",
 package_dir={"": "src"},
 include_package_data=True,
 long_description=long_description,
 long_description_content_type="text/markdown",
 url="https://github.com/dipson94/yt-comments",
 author="Dipson",
```

### Comparing `ytcomments-0.4/src/ytcomments/__init__.py` & `ytcomments-0.5/src/ytcomments/__init__.py`

 * *Files identical despite different names*

