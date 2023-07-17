# Comparing `tmp/wizlib-0.5.1.tar.gz` & `tmp/wizlib-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wizlib-0.5.1.tar", last modified: Wed Jul 12 03:03:58 2023, max compression
+gzip compressed data, was "wizlib-0.6.0.tar", last modified: Mon Jul 17 06:32:00 2023, max compression
```

## Comparing `wizlib-0.5.1.tar` & `wizlib-0.6.0.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 03:03:58.147327 wizlib-0.5.1/
--rw-rw-rw-   0 root         (0) root         (0)        5 2023-07-12 03:03:04.000000 wizlib-0.5.1/.version
--rw-r--r--   0 root         (0) root         (0)     1771 2023-07-12 03:03:58.147327 wizlib-0.5.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1506 2023-07-12 03:03:48.000000 wizlib-0.5.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      541 2023-07-12 03:03:48.000000 wizlib-0.5.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 03:03:58.147327 wizlib-0.5.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 03:03:58.145327 wizlib-0.5.1/test/
--rw-rw-rw-   0 root         (0) root         (0)      232 2023-07-12 03:03:48.000000 wizlib-0.5.1/test/test_class_family.py
--rw-rw-rw-   0 root         (0) root         (0)     1406 2023-07-12 03:03:48.000000 wizlib-0.5.1/test/test_super_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 03:03:58.145327 wizlib-0.5.1/wizlib/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-12 03:03:48.000000 wizlib-0.5.1/wizlib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5935 2023-07-12 03:03:48.000000 wizlib-0.5.1/wizlib/class_family.py
--rw-rw-rw-   0 root         (0) root         (0)     1647 2023-07-12 03:03:48.000000 wizlib-0.5.1/wizlib/rlinput.py
--rw-rw-rw-   0 root         (0) root         (0)      973 2023-07-12 03:03:48.000000 wizlib-0.5.1/wizlib/super_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 03:03:58.146327 wizlib-0.5.1/wizlib.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1771 2023-07-12 03:03:58.000000 wizlib-0.5.1/wizlib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      319 2023-07-12 03:03:58.000000 wizlib-0.5.1/wizlib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 03:03:58.000000 wizlib-0.5.1/wizlib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       89 2023-07-12 03:03:58.000000 wizlib-0.5.1/wizlib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-12 03:03:58.000000 wizlib-0.5.1/wizlib.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 06:32:00.828410 wizlib-0.6.0/
+-rw-rw-rw-   0 root         (0) root         (0)        5 2023-07-17 06:31:10.000000 wizlib-0.6.0/.version
+-rw-r--r--   0 root         (0) root         (0)     3319 2023-07-17 06:32:00.828410 wizlib-0.6.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3054 2023-07-17 06:31:52.000000 wizlib-0.6.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      541 2023-07-17 06:31:52.000000 wizlib-0.6.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-17 06:32:00.829409 wizlib-0.6.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 06:32:00.826409 wizlib-0.6.0/test/
+-rw-rw-rw-   0 root         (0) root         (0)      232 2023-07-17 06:31:52.000000 wizlib-0.6.0/test/test_class_family.py
+-rw-rw-rw-   0 root         (0) root         (0)      391 2023-07-17 06:31:52.000000 wizlib-0.6.0/test/test_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     1406 2023-07-17 06:31:52.000000 wizlib-0.6.0/test/test_super_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 06:32:00.827409 wizlib-0.6.0/wizlib/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-17 06:31:52.000000 wizlib-0.6.0/wizlib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4413 2023-07-17 06:31:52.000000 wizlib-0.6.0/wizlib/class_family.py
+-rw-rw-rw-   0 root         (0) root         (0)     2155 2023-07-17 06:31:52.000000 wizlib-0.6.0/wizlib/command_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     1647 2023-07-17 06:31:52.000000 wizlib-0.6.0/wizlib/rlinput.py
+-rw-rw-rw-   0 root         (0) root         (0)      973 2023-07-17 06:31:52.000000 wizlib-0.6.0/wizlib/super_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 06:32:00.828410 wizlib-0.6.0/wizlib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3319 2023-07-17 06:32:00.000000 wizlib-0.6.0/wizlib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      366 2023-07-17 06:32:00.000000 wizlib-0.6.0/wizlib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 06:32:00.000000 wizlib-0.6.0/wizlib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       89 2023-07-17 06:32:00.000000 wizlib-0.6.0/wizlib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-17 06:32:00.000000 wizlib-0.6.0/wizlib.egg-info/top_level.txt
```

### Comparing `wizlib-0.5.1/pyproject.toml` & `wizlib-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wizlib-0.5.1/test/test_super_wrapper.py` & `wizlib-0.6.0/test/test_super_wrapper.py`

 * *Files identical despite different names*

### Comparing `wizlib-0.5.1/wizlib/class_family.py` & `wizlib-0.6.0/wizlib/class_family.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,7 @@
-# A class family is a set of class definitions that use single inheritance
-# (each subclass inherits from only one parent) and often multiple inheritance
-# (subclasses can inherit from subclasses). So it's a hierarchy of classes,
-# with one super-parent at the top.
-#
-# We offer a way for members of the family to declare themselves simply by
-# living in the right package location. Then those classes can be instantiated
-# using keys or names, without having to be specifically called. The members
-# act independently of each other.
-#
-# What we get, after importing everything and loading it all, is essentially a
-# little database of classes, where class-level properties become keys for
-# looking up member classes. So, for example, we can have a family of commands,
-# and use a command string to look up the right command.
-#
-# Ultimately, the super-parent of the family -- the class at the top of the
-# hierarchy -- holds the database, actually a list, in the property called
-# "family". So that class can be queried to find appropriate family member
-# classes or instances thereof.
-#
-# This utility provides functions for importing family members, loading the
-# "families" property of the super-parent, and querying the family.
-#
-# In the process of loading and querying the class family, we need to *avoid*
-# inheritance of attributes. There might be abstract intermediary classes that
-# don't want to play. So we use __dict__ to ensure we're only seeing the
-# atttributes that are defined on that specific class.
-
-
 from importlib import import_module
 from inspect import getmodule
 from pathlib import Path
 from re import match
 
 
 class ClassFamily:
```

### Comparing `wizlib-0.5.1/wizlib/rlinput.py` & `wizlib-0.6.0/wizlib/rlinput.py`

 * *Files identical despite different names*

### Comparing `wizlib-0.5.1/wizlib/super_wrapper.py` & `wizlib-0.6.0/wizlib/super_wrapper.py`

 * *Files identical despite different names*

