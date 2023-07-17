# Comparing `tmp/pipcoloringstools-1.0.0.tar.gz` & `tmp/pipcoloringstools-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipcoloringstools-1.0.0.tar", last modified: Mon Jul 17 15:05:10 2023, max compression
+gzip compressed data, was "pipcoloringstools-1.1.0.tar", last modified: Mon Jul 17 15:07:14 2023, max compression
```

## Comparing `pipcoloringstools-1.0.0.tar` & `pipcoloringstools-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:05:10.130995 pipcoloringstools-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      350 2023-07-17 15:05:10.130995 pipcoloringstools-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:05:10.130995 pipcoloringstools-1.0.0/pipcoloringstools/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-17 15:05:09.000000 pipcoloringstools-1.0.0/pipcoloringstools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:05:10.130995 pipcoloringstools-1.0.0/pipcoloringstools.egg-info/
--rw-r--r--   0 root         (0) root         (0)      350 2023-07-17 15:05:09.000000 pipcoloringstools-1.0.0/pipcoloringstools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      202 2023-07-17 15:05:10.000000 pipcoloringstools-1.0.0/pipcoloringstools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 15:05:09.000000 pipcoloringstools-1.0.0/pipcoloringstools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-17 15:05:09.000000 pipcoloringstools-1.0.0/pipcoloringstools.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-17 15:05:10.130995 pipcoloringstools-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      563 2023-07-17 15:05:09.000000 pipcoloringstools-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:07:14.970398 pipcoloringstools-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      350 2023-07-17 15:07:14.970398 pipcoloringstools-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:07:14.966398 pipcoloringstools-1.1.0/pipcoloringstools/
+-rw-r--r--   0 root         (0) root         (0)    96773 2023-07-17 15:07:14.000000 pipcoloringstools-1.1.0/pipcoloringstools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:07:14.966398 pipcoloringstools-1.1.0/pipcoloringstools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      350 2023-07-17 15:07:14.000000 pipcoloringstools-1.1.0/pipcoloringstools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      202 2023-07-17 15:07:14.000000 pipcoloringstools-1.1.0/pipcoloringstools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 15:07:14.000000 pipcoloringstools-1.1.0/pipcoloringstools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-17 15:07:14.000000 pipcoloringstools-1.1.0/pipcoloringstools.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-17 15:07:14.970398 pipcoloringstools-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      563 2023-07-17 15:07:14.000000 pipcoloringstools-1.1.0/setup.py
```

### Comparing `pipcoloringstools-1.0.0/setup.py` & `pipcoloringstools-1.1.0/setup.py`

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
     name="pipcoloringstools",
     version=VERSION,
```

