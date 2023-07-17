# Comparing `tmp/pythoncryptextensions-1.0.0.tar.gz` & `tmp/pythoncryptextensions-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythoncryptextensions-1.0.0.tar", last modified: Mon Jul 17 15:06:17 2023, max compression
+gzip compressed data, was "pythoncryptextensions-1.1.0.tar", last modified: Mon Jul 17 15:08:22 2023, max compression
```

## Comparing `pythoncryptextensions-1.0.0.tar` & `pythoncryptextensions-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:06:17.634667 pythoncryptextensions-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      354 2023-07-17 15:06:17.634667 pythoncryptextensions-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:06:17.634667 pythoncryptextensions-1.0.0/pythoncryptextensions/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-17 15:06:17.000000 pythoncryptextensions-1.0.0/pythoncryptextensions/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:06:17.634667 pythoncryptextensions-1.0.0/pythoncryptextensions.egg-info/
--rw-r--r--   0 root         (0) root         (0)      354 2023-07-17 15:06:17.000000 pythoncryptextensions-1.0.0/pythoncryptextensions.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      222 2023-07-17 15:06:17.000000 pythoncryptextensions-1.0.0/pythoncryptextensions.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 15:06:17.000000 pythoncryptextensions-1.0.0/pythoncryptextensions.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 15:06:17.000000 pythoncryptextensions-1.0.0/pythoncryptextensions.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-17 15:06:17.638667 pythoncryptextensions-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      567 2023-07-17 15:06:17.000000 pythoncryptextensions-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:08:22.850088 pythoncryptextensions-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      354 2023-07-17 15:08:22.850088 pythoncryptextensions-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:08:22.846088 pythoncryptextensions-1.1.0/pythoncryptextensions/
+-rw-r--r--   0 root         (0) root         (0)    96773 2023-07-17 15:08:22.000000 pythoncryptextensions-1.1.0/pythoncryptextensions/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:08:22.850088 pythoncryptextensions-1.1.0/pythoncryptextensions.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      354 2023-07-17 15:08:22.000000 pythoncryptextensions-1.1.0/pythoncryptextensions.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      222 2023-07-17 15:08:22.000000 pythoncryptextensions-1.1.0/pythoncryptextensions.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 15:08:22.000000 pythoncryptextensions-1.1.0/pythoncryptextensions.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 15:08:22.000000 pythoncryptextensions-1.1.0/pythoncryptextensions.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-17 15:08:22.850088 pythoncryptextensions-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      567 2023-07-17 15:08:22.000000 pythoncryptextensions-1.1.0/setup.py
```

### Comparing `pythoncryptextensions-1.0.0/setup.py` & `pythoncryptextensions-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull utility package"
 LONG_DESCRIPTION = "Usefull utility package"
 
 # Setting up
 setup(
     name="pythoncryptextensions",
     version=VERSION,
```

