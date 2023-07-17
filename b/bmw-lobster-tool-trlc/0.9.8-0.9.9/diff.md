# Comparing `tmp/bmw-lobster-tool-trlc-0.9.8.tar.gz` & `tmp/bmw-lobster-tool-trlc-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmw-lobster-tool-trlc-0.9.8.tar", last modified: Tue Jun 27 13:44:45 2023, max compression
+gzip compressed data, was "bmw-lobster-tool-trlc-0.9.9.tar", last modified: Mon Jul 17 08:49:40 2023, max compression
```

## Comparing `bmw-lobster-tool-trlc-0.9.8.tar` & `bmw-lobster-tool-trlc-0.9.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:45.294403 bmw-lobster-tool-trlc-0.9.8/
--rw-r--r--   0 florian   (1000) florian   (1000)     3210 2023-06-27 13:44:45.294403 bmw-lobster-tool-trlc-0.9.8/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)     2282 2023-06-13 09:17:37.000000 bmw-lobster-tool-trlc-0.9.8/README.md
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:45.294403 bmw-lobster-tool-trlc-0.9.8/bmw_lobster_tool_trlc.egg-info/
--rw-r--r--   0 florian   (1000) florian   (1000)     3210 2023-06-27 13:44:45.000000 bmw-lobster-tool-trlc-0.9.8/bmw_lobster_tool_trlc.egg-info/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)      348 2023-06-27 13:44:45.000000 bmw-lobster-tool-trlc-0.9.8/bmw_lobster_tool_trlc.egg-info/SOURCES.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-06-27 13:44:45.000000 bmw-lobster-tool-trlc-0.9.8/bmw_lobster_tool_trlc.egg-info/dependency_links.txt
--rw-r--r--   0 florian   (1000) florian   (1000)       62 2023-06-27 13:44:45.000000 bmw-lobster-tool-trlc-0.9.8/bmw_lobster_tool_trlc.egg-info/entry_points.txt
--rw-r--r--   0 florian   (1000) florian   (1000)       36 2023-06-27 13:44:45.000000 bmw-lobster-tool-trlc-0.9.8/bmw_lobster_tool_trlc.egg-info/requires.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        8 2023-06-27 13:44:45.000000 bmw-lobster-tool-trlc-0.9.8/bmw_lobster_tool_trlc.egg-info/top_level.txt
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:45.290403 bmw-lobster-tool-trlc-0.9.8/lobster/
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:45.290403 bmw-lobster-tool-trlc-0.9.8/lobster/tools/
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:45.294403 bmw-lobster-tool-trlc-0.9.8/lobster/tools/trlc/
--rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:45.000000 bmw-lobster-tool-trlc-0.9.8/lobster/tools/trlc/__init__.py
--rw-r--r--   0 florian   (1000) florian   (1000)    15533 2023-06-27 13:44:45.000000 bmw-lobster-tool-trlc-0.9.8/lobster/tools/trlc/trlc.py
--rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-06-27 13:44:45.294403 bmw-lobster-tool-trlc-0.9.8/setup.cfg
--rw-r--r--   0 florian   (1000) florian   (1000)     2540 2023-06-27 13:44:26.000000 bmw-lobster-tool-trlc-0.9.8/setup.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-17 08:49:40.662608 bmw-lobster-tool-trlc-0.9.9/
+-rw-r--r--   0 florian   (1000) florian   (1000)     3210 2023-07-17 08:49:40.662608 bmw-lobster-tool-trlc-0.9.9/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)     2282 2023-06-13 09:17:37.000000 bmw-lobster-tool-trlc-0.9.9/README.md
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-17 08:49:40.662608 bmw-lobster-tool-trlc-0.9.9/bmw_lobster_tool_trlc.egg-info/
+-rw-r--r--   0 florian   (1000) florian   (1000)     3210 2023-07-17 08:49:40.000000 bmw-lobster-tool-trlc-0.9.9/bmw_lobster_tool_trlc.egg-info/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)      348 2023-07-17 08:49:40.000000 bmw-lobster-tool-trlc-0.9.9/bmw_lobster_tool_trlc.egg-info/SOURCES.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-07-17 08:49:40.000000 bmw-lobster-tool-trlc-0.9.9/bmw_lobster_tool_trlc.egg-info/dependency_links.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)       62 2023-07-17 08:49:40.000000 bmw-lobster-tool-trlc-0.9.9/bmw_lobster_tool_trlc.egg-info/entry_points.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)       36 2023-07-17 08:49:40.000000 bmw-lobster-tool-trlc-0.9.9/bmw_lobster_tool_trlc.egg-info/requires.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        8 2023-07-17 08:49:40.000000 bmw-lobster-tool-trlc-0.9.9/bmw_lobster_tool_trlc.egg-info/top_level.txt
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-17 08:49:40.658608 bmw-lobster-tool-trlc-0.9.9/lobster/
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-17 08:49:40.658608 bmw-lobster-tool-trlc-0.9.9/lobster/tools/
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-17 08:49:40.662608 bmw-lobster-tool-trlc-0.9.9/lobster/tools/trlc/
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-07-17 08:49:40.000000 bmw-lobster-tool-trlc-0.9.9/lobster/tools/trlc/__init__.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    15533 2023-07-17 08:49:40.000000 bmw-lobster-tool-trlc-0.9.9/lobster/tools/trlc/trlc.py
+-rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-07-17 08:49:40.662608 bmw-lobster-tool-trlc-0.9.9/setup.cfg
+-rw-r--r--   0 florian   (1000) florian   (1000)     2540 2023-06-27 13:44:26.000000 bmw-lobster-tool-trlc-0.9.9/setup.py
```

### Comparing `bmw-lobster-tool-trlc-0.9.8/PKG-INFO` & `bmw-lobster-tool-trlc-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmw-lobster-tool-trlc
-Version: 0.9.8
+Version: 0.9.9
 Summary: LOBSTER Tool for TRLC
 Home-page: https://github.com/bmw-software-engineering/lobster
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU Affero General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/lobster/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/lobster/
```

### Comparing `bmw-lobster-tool-trlc-0.9.8/README.md` & `bmw-lobster-tool-trlc-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `bmw-lobster-tool-trlc-0.9.8/bmw_lobster_tool_trlc.egg-info/PKG-INFO` & `bmw-lobster-tool-trlc-0.9.9/bmw_lobster_tool_trlc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmw-lobster-tool-trlc
-Version: 0.9.8
+Version: 0.9.9
 Summary: LOBSTER Tool for TRLC
 Home-page: https://github.com/bmw-software-engineering/lobster
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU Affero General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/lobster/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/lobster/
```

### Comparing `bmw-lobster-tool-trlc-0.9.8/lobster/tools/trlc/trlc.py` & `bmw-lobster-tool-trlc-0.9.9/lobster/tools/trlc/trlc.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-tool-trlc-0.9.8/setup.py` & `bmw-lobster-tool-trlc-0.9.9/setup.py`

 * *Files identical despite different names*

