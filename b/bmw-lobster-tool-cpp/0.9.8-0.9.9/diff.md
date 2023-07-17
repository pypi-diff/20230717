# Comparing `tmp/bmw-lobster-tool-cpp-0.9.8.tar.gz` & `tmp/bmw-lobster-tool-cpp-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmw-lobster-tool-cpp-0.9.8.tar", last modified: Tue Jun 27 13:44:45 2023, max compression
+gzip compressed data, was "bmw-lobster-tool-cpp-0.9.9.tar", last modified: Mon Jul 17 08:49:41 2023, max compression
```

## Comparing `bmw-lobster-tool-cpp-0.9.8.tar` & `bmw-lobster-tool-cpp-0.9.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:45.890413 bmw-lobster-tool-cpp-0.9.8/
--rw-r--r--   0 florian   (1000) florian   (1000)     1984 2023-06-27 13:44:45.890413 bmw-lobster-tool-cpp-0.9.8/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)     1052 2023-06-13 09:17:37.000000 bmw-lobster-tool-cpp-0.9.8/README.md
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:45.890413 bmw-lobster-tool-cpp-0.9.8/bmw_lobster_tool_cpp.egg-info/
--rw-r--r--   0 florian   (1000) florian   (1000)     1984 2023-06-27 13:44:45.000000 bmw-lobster-tool-cpp-0.9.8/bmw_lobster_tool_cpp.egg-info/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)      339 2023-06-27 13:44:45.000000 bmw-lobster-tool-cpp-0.9.8/bmw_lobster_tool_cpp.egg-info/SOURCES.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-06-27 13:44:45.000000 bmw-lobster-tool-cpp-0.9.8/bmw_lobster_tool_cpp.egg-info/dependency_links.txt
--rw-r--r--   0 florian   (1000) florian   (1000)       59 2023-06-27 13:44:45.000000 bmw-lobster-tool-cpp-0.9.8/bmw_lobster_tool_cpp.egg-info/entry_points.txt
--rw-r--r--   0 florian   (1000) florian   (1000)       24 2023-06-27 13:44:45.000000 bmw-lobster-tool-cpp-0.9.8/bmw_lobster_tool_cpp.egg-info/requires.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        8 2023-06-27 13:44:45.000000 bmw-lobster-tool-cpp-0.9.8/bmw_lobster_tool_cpp.egg-info/top_level.txt
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:45.886413 bmw-lobster-tool-cpp-0.9.8/lobster/
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:45.886413 bmw-lobster-tool-cpp-0.9.8/lobster/tools/
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:45.890413 bmw-lobster-tool-cpp-0.9.8/lobster/tools/cpp/
--rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:45.000000 bmw-lobster-tool-cpp-0.9.8/lobster/tools/cpp/__init__.py
--rwxr-xr-x   0 florian   (1000) florian   (1000)     7349 2023-06-27 13:44:45.000000 bmw-lobster-tool-cpp-0.9.8/lobster/tools/cpp/cpp.py
--rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-06-27 13:44:45.890413 bmw-lobster-tool-cpp-0.9.8/setup.cfg
--rw-r--r--   0 florian   (1000) florian   (1000)     2543 2023-06-27 13:44:26.000000 bmw-lobster-tool-cpp-0.9.8/setup.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-17 08:49:41.294614 bmw-lobster-tool-cpp-0.9.9/
+-rw-r--r--   0 florian   (1000) florian   (1000)     1984 2023-07-17 08:49:41.294614 bmw-lobster-tool-cpp-0.9.9/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)     1052 2023-06-13 09:17:37.000000 bmw-lobster-tool-cpp-0.9.9/README.md
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-17 08:49:41.290614 bmw-lobster-tool-cpp-0.9.9/bmw_lobster_tool_cpp.egg-info/
+-rw-r--r--   0 florian   (1000) florian   (1000)     1984 2023-07-17 08:49:41.000000 bmw-lobster-tool-cpp-0.9.9/bmw_lobster_tool_cpp.egg-info/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)      339 2023-07-17 08:49:41.000000 bmw-lobster-tool-cpp-0.9.9/bmw_lobster_tool_cpp.egg-info/SOURCES.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-07-17 08:49:41.000000 bmw-lobster-tool-cpp-0.9.9/bmw_lobster_tool_cpp.egg-info/dependency_links.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)       59 2023-07-17 08:49:41.000000 bmw-lobster-tool-cpp-0.9.9/bmw_lobster_tool_cpp.egg-info/entry_points.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)       24 2023-07-17 08:49:41.000000 bmw-lobster-tool-cpp-0.9.9/bmw_lobster_tool_cpp.egg-info/requires.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        8 2023-07-17 08:49:41.000000 bmw-lobster-tool-cpp-0.9.9/bmw_lobster_tool_cpp.egg-info/top_level.txt
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-17 08:49:41.290614 bmw-lobster-tool-cpp-0.9.9/lobster/
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-17 08:49:41.290614 bmw-lobster-tool-cpp-0.9.9/lobster/tools/
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-17 08:49:41.294614 bmw-lobster-tool-cpp-0.9.9/lobster/tools/cpp/
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-07-17 08:49:41.000000 bmw-lobster-tool-cpp-0.9.9/lobster/tools/cpp/__init__.py
+-rwxr-xr-x   0 florian   (1000) florian   (1000)     7349 2023-07-17 08:49:41.000000 bmw-lobster-tool-cpp-0.9.9/lobster/tools/cpp/cpp.py
+-rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-07-17 08:49:41.294614 bmw-lobster-tool-cpp-0.9.9/setup.cfg
+-rw-r--r--   0 florian   (1000) florian   (1000)     2543 2023-06-27 13:44:26.000000 bmw-lobster-tool-cpp-0.9.9/setup.py
```

### Comparing `bmw-lobster-tool-cpp-0.9.8/PKG-INFO` & `bmw-lobster-tool-cpp-0.9.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmw-lobster-tool-cpp
-Version: 0.9.8
+Version: 0.9.9
 Summary: LOBSTER Tool for ISO C/C++
 Home-page: https://github.com/bmw-software-engineering/lobster
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU Affero General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/lobster/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/lobster/
```

### Comparing `bmw-lobster-tool-cpp-0.9.8/README.md` & `bmw-lobster-tool-cpp-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `bmw-lobster-tool-cpp-0.9.8/bmw_lobster_tool_cpp.egg-info/PKG-INFO` & `bmw-lobster-tool-cpp-0.9.9/bmw_lobster_tool_cpp.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmw-lobster-tool-cpp
-Version: 0.9.8
+Version: 0.9.9
 Summary: LOBSTER Tool for ISO C/C++
 Home-page: https://github.com/bmw-software-engineering/lobster
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU Affero General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/lobster/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/lobster/
```

### Comparing `bmw-lobster-tool-cpp-0.9.8/lobster/tools/cpp/cpp.py` & `bmw-lobster-tool-cpp-0.9.9/lobster/tools/cpp/cpp.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-tool-cpp-0.9.8/setup.py` & `bmw-lobster-tool-cpp-0.9.9/setup.py`

 * *Files identical despite different names*

