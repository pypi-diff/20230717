# Comparing `tmp/bmw-lobster-0.9.8.tar.gz` & `tmp/bmw-lobster-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmw-lobster-0.9.8.tar", last modified: Tue Jun 27 13:44:47 2023, max compression
+gzip compressed data, was "bmw-lobster-0.9.9.tar", last modified: Mon Jul 17 08:49:42 2023, max compression
```

## Comparing `bmw-lobster-0.9.8.tar` & `bmw-lobster-0.9.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:47.062434 bmw-lobster-0.9.8/
--rw-r--r--   0 florian   (1000) florian   (1000)     2316 2023-06-27 13:44:47.062434 bmw-lobster-0.9.8/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)     1379 2023-06-27 13:44:26.000000 bmw-lobster-0.9.8/README.md
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:47.062434 bmw-lobster-0.9.8/bmw_lobster.egg-info/
--rw-r--r--   0 florian   (1000) florian   (1000)     2316 2023-06-27 13:44:47.000000 bmw-lobster-0.9.8/bmw_lobster.egg-info/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)      192 2023-06-27 13:44:47.000000 bmw-lobster-0.9.8/bmw_lobster.egg-info/SOURCES.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-06-27 13:44:47.000000 bmw-lobster-0.9.8/bmw_lobster.egg-info/dependency_links.txt
--rw-r--r--   0 florian   (1000) florian   (1000)      223 2023-06-27 13:44:47.000000 bmw-lobster-0.9.8/bmw_lobster.egg-info/requires.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-06-27 13:44:47.000000 bmw-lobster-0.9.8/bmw_lobster.egg-info/top_level.txt
--rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-06-27 13:44:47.062434 bmw-lobster-0.9.8/setup.cfg
--rw-r--r--   0 florian   (1000) florian   (1000)     2511 2023-06-27 13:44:26.000000 bmw-lobster-0.9.8/setup.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-17 08:49:42.530627 bmw-lobster-0.9.9/
+-rw-r--r--   0 florian   (1000) florian   (1000)     2316 2023-07-17 08:49:42.530627 bmw-lobster-0.9.9/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)     1379 2023-06-27 13:44:26.000000 bmw-lobster-0.9.9/README.md
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-17 08:49:42.530627 bmw-lobster-0.9.9/bmw_lobster.egg-info/
+-rw-r--r--   0 florian   (1000) florian   (1000)     2316 2023-07-17 08:49:42.000000 bmw-lobster-0.9.9/bmw_lobster.egg-info/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)      192 2023-07-17 08:49:42.000000 bmw-lobster-0.9.9/bmw_lobster.egg-info/SOURCES.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-07-17 08:49:42.000000 bmw-lobster-0.9.9/bmw_lobster.egg-info/dependency_links.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)      223 2023-07-17 08:49:42.000000 bmw-lobster-0.9.9/bmw_lobster.egg-info/requires.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-07-17 08:49:42.000000 bmw-lobster-0.9.9/bmw_lobster.egg-info/top_level.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-07-17 08:49:42.530627 bmw-lobster-0.9.9/setup.cfg
+-rw-r--r--   0 florian   (1000) florian   (1000)     2511 2023-06-27 13:44:26.000000 bmw-lobster-0.9.9/setup.py
```

### Comparing `bmw-lobster-0.9.8/PKG-INFO` & `bmw-lobster-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmw-lobster
-Version: 0.9.8
+Version: 0.9.9
 Summary: Metapackage to install all LOBSTER Tools
 Home-page: https://github.com/bmw-software-engineering/lobster
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU Affero General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/lobster/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/lobster/
```

### Comparing `bmw-lobster-0.9.8/README.md` & `bmw-lobster-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `bmw-lobster-0.9.8/bmw_lobster.egg-info/PKG-INFO` & `bmw-lobster-0.9.9/bmw_lobster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmw-lobster
-Version: 0.9.8
+Version: 0.9.9
 Summary: Metapackage to install all LOBSTER Tools
 Home-page: https://github.com/bmw-software-engineering/lobster
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU Affero General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/lobster/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/lobster/
```

### Comparing `bmw-lobster-0.9.8/setup.py` & `bmw-lobster-0.9.9/setup.py`

 * *Files identical despite different names*

