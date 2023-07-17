# Comparing `tmp/bmw-lobster-monolithic-0.9.8.tar.gz` & `tmp/bmw-lobster-monolithic-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmw-lobster-monolithic-0.9.8.tar", last modified: Tue Jun 27 13:44:47 2023, max compression
+gzip compressed data, was "bmw-lobster-monolithic-0.9.9.tar", last modified: Mon Jul 17 08:49:42 2023, max compression
```

## Comparing `bmw-lobster-monolithic-0.9.8.tar` & `bmw-lobster-monolithic-0.9.9.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:47.362439 bmw-lobster-monolithic-0.9.8/
--rw-r--r--   0 florian   (1000) florian   (1000)     1710 2023-06-27 13:44:47.362439 bmw-lobster-monolithic-0.9.8/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)      762 2023-06-27 13:44:26.000000 bmw-lobster-monolithic-0.9.8/README.md
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:47.358439 bmw-lobster-monolithic-0.9.8/bmw_lobster_monolithic.egg-info/
--rw-r--r--   0 florian   (1000) florian   (1000)     1710 2023-06-27 13:44:47.000000 bmw-lobster-monolithic-0.9.8/bmw_lobster_monolithic.egg-info/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)     1152 2023-06-27 13:44:47.000000 bmw-lobster-monolithic-0.9.8/bmw_lobster_monolithic.egg-info/SOURCES.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-06-27 13:44:47.000000 bmw-lobster-monolithic-0.9.8/bmw_lobster_monolithic.egg-info/dependency_links.txt
--rw-r--r--   0 florian   (1000) florian   (1000)      528 2023-06-27 13:44:47.000000 bmw-lobster-monolithic-0.9.8/bmw_lobster_monolithic.egg-info/entry_points.txt
--rw-r--r--   0 florian   (1000) florian   (1000)       58 2023-06-27 13:44:47.000000 bmw-lobster-monolithic-0.9.8/bmw_lobster_monolithic.egg-info/requires.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        8 2023-06-27 13:44:47.000000 bmw-lobster-monolithic-0.9.8/bmw_lobster_monolithic.egg-info/top_level.txt
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:47.362439 bmw-lobster-monolithic-0.9.8/lobster/
--rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:47.000000 bmw-lobster-monolithic-0.9.8/lobster/__init__.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:47.362439 bmw-lobster-monolithic-0.9.8/lobster/config/
--rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:47.000000 bmw-lobster-monolithic-0.9.8/lobster/config/__init__.py
--rw-r--r--   0 florian   (1000) florian   (1000)     4161 2023-06-27 13:44:47.000000 bmw-lobster-monolithic-0.9.8/lobster/config/lexer.py
--rw-r--r--   0 florian   (1000) florian   (1000)     9087 2023-06-27 13:44:47.000000 bmw-lobster-monolithic-0.9.8/lobster/config/parser.py
--rw-r--r--   0 florian   (1000) florian   (1000)     2501 2023-06-27 13:44:47.000000 bmw-lobster-monolithic-0.9.8/lobster/errors.py
--rw-r--r--   0 florian   (1000) florian   (1000)     1244 2023-06-27 13:44:47.000000 bmw-lobster-monolithic-0.9.8/lobster/exceptions.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:47.362439 bmw-lobster-monolithic-0.9.8/lobster/html/
--rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:47.000000 bmw-lobster-monolithic-0.9.8/lobster/html/__init__.py
--rw-r--r--   0 florian   (1000) florian   (1000)     2682 2023-06-27 13:44:47.000000 bmw-lobster-monolithic-0.9.8/lobster/html/assets.py
--rw-r--r--   0 florian   (1000) florian   (1000)     9667 2023-06-27 13:44:47.000000 bmw-lobster-monolithic-0.9.8/lobster/html/htmldoc.py
--rw-r--r--   0 florian   (1000) florian   (1000)     4448 2023-06-27 13:44:47.000000 bmw-lobster-monolithic-0.9.8/lobster/io.py
--rw-r--r--   0 florian   (1000) florian   (1000)    11205 2023-06-27 13:44:47.000000 bmw-lobster-monolithic-0.9.8/lobster/items.py
--rw-r--r--   0 florian   (1000) florian   (1000)     7684 2023-06-27 13:44:47.000000 bmw-lobster-monolithic-0.9.8/lobster/location.py
--rw-r--r--   0 florian   (1000) florian   (1000)     8158 2023-06-27 13:44:47.000000 bmw-lobster-monolithic-0.9.8/lobster/report.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:47.362439 bmw-lobster-monolithic-0.9.8/lobster/tools/
--rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:47.000000 bmw-lobster-monolithic-0.9.8/lobster/tools/__init__.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:47.362439 bmw-lobster-monolithic-0.9.8/lobster/tools/codebeamer/
--rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:47.000000 bmw-lobster-monolithic-0.9.8/lobster/tools/codebeamer/__init__.py
--rwxr-xr-x   0 florian   (1000) florian   (1000)    10398 2023-06-27 13:44:47.000000 bmw-lobster-monolithic-0.9.8/lobster/tools/codebeamer/codebeamer.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:47.362439 bmw-lobster-monolithic-0.9.8/lobster/tools/core/
--rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:47.000000 bmw-lobster-monolithic-0.9.8/lobster/tools/core/__init__.py
--rwxr-xr-x   0 florian   (1000) florian   (1000)     1917 2023-06-27 13:44:47.000000 bmw-lobster-monolithic-0.9.8/lobster/tools/core/ci_report.py
--rwxr-xr-x   0 florian   (1000) florian   (1000)    15951 2023-06-27 13:44:47.000000 bmw-lobster-monolithic-0.9.8/lobster/tools/core/html_report.py
--rwxr-xr-x   0 florian   (1000) florian   (1000)     3707 2023-06-27 13:44:47.000000 bmw-lobster-monolithic-0.9.8/lobster/tools/core/online_report.py
--rwxr-xr-x   0 florian   (1000) florian   (1000)     2142 2023-06-27 13:44:47.000000 bmw-lobster-monolithic-0.9.8/lobster/tools/core/report.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:47.362439 bmw-lobster-monolithic-0.9.8/lobster/tools/cpp/
--rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:47.000000 bmw-lobster-monolithic-0.9.8/lobster/tools/cpp/__init__.py
--rwxr-xr-x   0 florian   (1000) florian   (1000)     7349 2023-06-27 13:44:47.000000 bmw-lobster-monolithic-0.9.8/lobster/tools/cpp/cpp.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:47.362439 bmw-lobster-monolithic-0.9.8/lobster/tools/gtest/
--rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:47.000000 bmw-lobster-monolithic-0.9.8/lobster/tools/gtest/__init__.py
--rwxr-xr-x   0 florian   (1000) florian   (1000)     5739 2023-06-27 13:44:47.000000 bmw-lobster-monolithic-0.9.8/lobster/tools/gtest/gtest.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:47.362439 bmw-lobster-monolithic-0.9.8/lobster/tools/json/
--rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:47.000000 bmw-lobster-monolithic-0.9.8/lobster/tools/json/__init__.py
--rwxr-xr-x   0 florian   (1000) florian   (1000)     6914 2023-06-27 13:44:47.000000 bmw-lobster-monolithic-0.9.8/lobster/tools/json/json.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:47.362439 bmw-lobster-monolithic-0.9.8/lobster/tools/python/
--rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:47.000000 bmw-lobster-monolithic-0.9.8/lobster/tools/python/__init__.py
--rwxr-xr-x   0 florian   (1000) florian   (1000)    12276 2023-06-27 13:44:47.000000 bmw-lobster-monolithic-0.9.8/lobster/tools/python/python.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:47.362439 bmw-lobster-monolithic-0.9.8/lobster/tools/trlc/
--rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:47.000000 bmw-lobster-monolithic-0.9.8/lobster/tools/trlc/__init__.py
--rw-r--r--   0 florian   (1000) florian   (1000)    15533 2023-06-27 13:44:47.000000 bmw-lobster-monolithic-0.9.8/lobster/tools/trlc/trlc.py
--rw-r--r--   0 florian   (1000) florian   (1000)     1026 2023-06-27 13:44:47.000000 bmw-lobster-monolithic-0.9.8/lobster/version.py
--rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-06-27 13:44:47.362439 bmw-lobster-monolithic-0.9.8/setup.cfg
--rw-r--r--   0 florian   (1000) florian   (1000)     2824 2023-06-27 13:44:26.000000 bmw-lobster-monolithic-0.9.8/setup.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-17 08:49:42.850631 bmw-lobster-monolithic-0.9.9/
+-rw-r--r--   0 florian   (1000) florian   (1000)     1710 2023-07-17 08:49:42.850631 bmw-lobster-monolithic-0.9.9/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)      762 2023-06-27 13:44:26.000000 bmw-lobster-monolithic-0.9.9/README.md
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-17 08:49:42.846631 bmw-lobster-monolithic-0.9.9/bmw_lobster_monolithic.egg-info/
+-rw-r--r--   0 florian   (1000) florian   (1000)     1710 2023-07-17 08:49:42.000000 bmw-lobster-monolithic-0.9.9/bmw_lobster_monolithic.egg-info/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)     1152 2023-07-17 08:49:42.000000 bmw-lobster-monolithic-0.9.9/bmw_lobster_monolithic.egg-info/SOURCES.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-07-17 08:49:42.000000 bmw-lobster-monolithic-0.9.9/bmw_lobster_monolithic.egg-info/dependency_links.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)      528 2023-07-17 08:49:42.000000 bmw-lobster-monolithic-0.9.9/bmw_lobster_monolithic.egg-info/entry_points.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)       58 2023-07-17 08:49:42.000000 bmw-lobster-monolithic-0.9.9/bmw_lobster_monolithic.egg-info/requires.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        8 2023-07-17 08:49:42.000000 bmw-lobster-monolithic-0.9.9/bmw_lobster_monolithic.egg-info/top_level.txt
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-17 08:49:42.846631 bmw-lobster-monolithic-0.9.9/lobster/
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-07-17 08:49:42.000000 bmw-lobster-monolithic-0.9.9/lobster/__init__.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-17 08:49:42.846631 bmw-lobster-monolithic-0.9.9/lobster/config/
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-07-17 08:49:42.000000 bmw-lobster-monolithic-0.9.9/lobster/config/__init__.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     4161 2023-07-17 08:49:42.000000 bmw-lobster-monolithic-0.9.9/lobster/config/lexer.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     9087 2023-07-17 08:49:42.000000 bmw-lobster-monolithic-0.9.9/lobster/config/parser.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     2501 2023-07-17 08:49:42.000000 bmw-lobster-monolithic-0.9.9/lobster/errors.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     1244 2023-07-17 08:49:42.000000 bmw-lobster-monolithic-0.9.9/lobster/exceptions.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-17 08:49:42.846631 bmw-lobster-monolithic-0.9.9/lobster/html/
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-07-17 08:49:42.000000 bmw-lobster-monolithic-0.9.9/lobster/html/__init__.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     2682 2023-07-17 08:49:42.000000 bmw-lobster-monolithic-0.9.9/lobster/html/assets.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     9667 2023-07-17 08:49:42.000000 bmw-lobster-monolithic-0.9.9/lobster/html/htmldoc.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     4448 2023-07-17 08:49:42.000000 bmw-lobster-monolithic-0.9.9/lobster/io.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    11375 2023-07-17 08:49:42.000000 bmw-lobster-monolithic-0.9.9/lobster/items.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     8320 2023-07-17 08:49:42.000000 bmw-lobster-monolithic-0.9.9/lobster/location.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     8158 2023-07-17 08:49:42.000000 bmw-lobster-monolithic-0.9.9/lobster/report.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-17 08:49:42.846631 bmw-lobster-monolithic-0.9.9/lobster/tools/
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-07-17 08:49:42.000000 bmw-lobster-monolithic-0.9.9/lobster/tools/__init__.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-17 08:49:42.846631 bmw-lobster-monolithic-0.9.9/lobster/tools/codebeamer/
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-07-17 08:49:42.000000 bmw-lobster-monolithic-0.9.9/lobster/tools/codebeamer/__init__.py
+-rwxr-xr-x   0 florian   (1000) florian   (1000)    10398 2023-07-17 08:49:42.000000 bmw-lobster-monolithic-0.9.9/lobster/tools/codebeamer/codebeamer.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-17 08:49:42.846631 bmw-lobster-monolithic-0.9.9/lobster/tools/core/
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-07-17 08:49:42.000000 bmw-lobster-monolithic-0.9.9/lobster/tools/core/__init__.py
+-rwxr-xr-x   0 florian   (1000) florian   (1000)     1917 2023-07-17 08:49:42.000000 bmw-lobster-monolithic-0.9.9/lobster/tools/core/ci_report.py
+-rwxr-xr-x   0 florian   (1000) florian   (1000)    17169 2023-07-17 08:49:42.000000 bmw-lobster-monolithic-0.9.9/lobster/tools/core/html_report.py
+-rwxr-xr-x   0 florian   (1000) florian   (1000)     3707 2023-07-17 08:49:42.000000 bmw-lobster-monolithic-0.9.9/lobster/tools/core/online_report.py
+-rwxr-xr-x   0 florian   (1000) florian   (1000)     2141 2023-07-17 08:49:42.000000 bmw-lobster-monolithic-0.9.9/lobster/tools/core/report.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-17 08:49:42.846631 bmw-lobster-monolithic-0.9.9/lobster/tools/cpp/
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-07-17 08:49:42.000000 bmw-lobster-monolithic-0.9.9/lobster/tools/cpp/__init__.py
+-rwxr-xr-x   0 florian   (1000) florian   (1000)     7349 2023-07-17 08:49:42.000000 bmw-lobster-monolithic-0.9.9/lobster/tools/cpp/cpp.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-17 08:49:42.846631 bmw-lobster-monolithic-0.9.9/lobster/tools/gtest/
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-07-17 08:49:42.000000 bmw-lobster-monolithic-0.9.9/lobster/tools/gtest/__init__.py
+-rwxr-xr-x   0 florian   (1000) florian   (1000)     5739 2023-07-17 08:49:42.000000 bmw-lobster-monolithic-0.9.9/lobster/tools/gtest/gtest.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-17 08:49:42.846631 bmw-lobster-monolithic-0.9.9/lobster/tools/json/
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-07-17 08:49:42.000000 bmw-lobster-monolithic-0.9.9/lobster/tools/json/__init__.py
+-rwxr-xr-x   0 florian   (1000) florian   (1000)     6914 2023-07-17 08:49:42.000000 bmw-lobster-monolithic-0.9.9/lobster/tools/json/json.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-17 08:49:42.846631 bmw-lobster-monolithic-0.9.9/lobster/tools/python/
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-07-17 08:49:42.000000 bmw-lobster-monolithic-0.9.9/lobster/tools/python/__init__.py
+-rwxr-xr-x   0 florian   (1000) florian   (1000)    12276 2023-07-17 08:49:42.000000 bmw-lobster-monolithic-0.9.9/lobster/tools/python/python.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-17 08:49:42.850631 bmw-lobster-monolithic-0.9.9/lobster/tools/trlc/
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-07-17 08:49:42.000000 bmw-lobster-monolithic-0.9.9/lobster/tools/trlc/__init__.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    15533 2023-07-17 08:49:42.000000 bmw-lobster-monolithic-0.9.9/lobster/tools/trlc/trlc.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     1026 2023-07-17 08:49:42.000000 bmw-lobster-monolithic-0.9.9/lobster/version.py
+-rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-07-17 08:49:42.850631 bmw-lobster-monolithic-0.9.9/setup.cfg
+-rw-r--r--   0 florian   (1000) florian   (1000)     2824 2023-06-27 13:44:26.000000 bmw-lobster-monolithic-0.9.9/setup.py
```

### Comparing `bmw-lobster-monolithic-0.9.8/PKG-INFO` & `bmw-lobster-monolithic-0.9.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmw-lobster-monolithic
-Version: 0.9.8
+Version: 0.9.9
 Summary: Monolithic package for all LOBSTER Tools
 Home-page: https://github.com/bmw-software-engineering/lobster
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU Affero General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/lobster/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/lobster/
```

### Comparing `bmw-lobster-monolithic-0.9.8/README.md` & `bmw-lobster-monolithic-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `bmw-lobster-monolithic-0.9.8/bmw_lobster_monolithic.egg-info/PKG-INFO` & `bmw-lobster-monolithic-0.9.9/bmw_lobster_monolithic.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmw-lobster-monolithic
-Version: 0.9.8
+Version: 0.9.9
 Summary: Monolithic package for all LOBSTER Tools
 Home-page: https://github.com/bmw-software-engineering/lobster
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU Affero General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/lobster/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/lobster/
```

### Comparing `bmw-lobster-monolithic-0.9.8/bmw_lobster_monolithic.egg-info/SOURCES.txt` & `bmw-lobster-monolithic-0.9.9/bmw_lobster_monolithic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bmw-lobster-monolithic-0.9.8/bmw_lobster_monolithic.egg-info/entry_points.txt` & `bmw-lobster-monolithic-0.9.9/bmw_lobster_monolithic.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `bmw-lobster-monolithic-0.9.8/lobster/config/lexer.py` & `bmw-lobster-monolithic-0.9.9/lobster/config/lexer.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-monolithic-0.9.8/lobster/config/parser.py` & `bmw-lobster-monolithic-0.9.9/lobster/config/parser.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-monolithic-0.9.8/lobster/errors.py` & `bmw-lobster-monolithic-0.9.9/lobster/errors.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-monolithic-0.9.8/lobster/exceptions.py` & `bmw-lobster-monolithic-0.9.9/lobster/exceptions.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-monolithic-0.9.8/lobster/html/assets.py` & `bmw-lobster-monolithic-0.9.9/lobster/html/assets.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-monolithic-0.9.8/lobster/html/htmldoc.py` & `bmw-lobster-monolithic-0.9.9/lobster/html/htmldoc.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-monolithic-0.9.8/lobster/io.py` & `bmw-lobster-monolithic-0.9.9/lobster/io.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-monolithic-0.9.8/lobster/items.py` & `bmw-lobster-monolithic-0.9.9/lobster/items.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 from lobster.location import Location
 
 
 class Tracing_Tag:
     def __init__(self, namespace, tag, version=None):
         assert isinstance(namespace, str) and " " not in namespace
-        assert isinstance(tag, str) and " " not in tag
+        assert isinstance(tag, str)
         assert version is None or isinstance(version, (str, int))
         assert not isinstance(version, str) or version != "None"
 
         self.namespace = namespace
         self.tag       = tag
         self.version   = version
         self.hash_val  = None
@@ -92,14 +92,15 @@
         self.tag       = tag
         self.location  = location
         self.name      = tag.tag
 
         self.ref_up   = []
         self.ref_down = []
 
+        self.unresolved_references_cache = set()
         self.unresolved_references = []
 
         self.messages    = []
         self.just_up     = []
         self.just_down   = []
         self.just_global = []
 
@@ -113,15 +114,19 @@
     def error(self, message):
         assert isinstance(message, str)
         self.messages.append(message)
         self.has_error = True
 
     def add_tracing_target(self, target):
         assert isinstance(target, Tracing_Tag)
+        if target.key() in self.unresolved_references_cache:
+            return
+
         self.unresolved_references.append(target)
+        self.unresolved_references_cache.add(target.key())
 
     def perform_source_checks(self, source_info):
         assert isinstance(source_info, dict)
 
     def determine_status(self, config, stab):
         assert self.level in config
         assert self.tag.key() in stab
```

### Comparing `bmw-lobster-monolithic-0.9.8/lobster/location.py` & `bmw-lobster-monolithic-0.9.9/lobster/location.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,18 @@
 import html
 
 from lobster.exceptions import LOBSTER_Exception
 
 
 class Location(metaclass=ABCMeta):
     @abstractmethod
+    def sorting_key(self):
+        pass
+
+    @abstractmethod
     def to_string(self):
         pass
 
     @abstractmethod
     def to_html(self):
         pass
 
@@ -68,14 +72,17 @@
                 json) from err
 
 
 class Void_Reference(Location):
     def __init__(self):
         pass
 
+    def sorting_key(self):
+        return tuple()
+
     def to_string(self):
         return "<unknown location>"
 
     def to_html(self):
         return html.escape(self.to_string())
 
     def to_json(self):
@@ -96,14 +103,23 @@
         assert column is None or (line is not None and
                                   isinstance(column, int) and
                                   column >= 1)
         self.filename = filename
         self.line     = line
         self.column   = column
 
+    def sorting_key(self):
+        if self.line is not None:
+            if self.column is not None:
+                return (self.filename, self.line, self.column)
+            else:
+                return (self.filename, self.line)
+        else:
+            return (self.filename,)
+
     def to_string(self):
         rv = self.filename
         if self.line:
             rv += ":%u" % self.line
         if self.column:
             rv += ":%u" % self.column
         return rv
@@ -143,14 +159,20 @@
 
         self.gh_root  = gh_root.rstrip("/")
         self.gh_repo  = self.gh_root.split("/")[-1]
         self.commit   = commit
         self.filename = filename
         self.line     = line
 
+    def sorting_key(self):
+        if self.line is not None:
+            return (self.filename, self.line)
+        else:
+            return (self.filename,)
+
     def to_string(self):
         if self.line:
             return "%s:%u" % (self.filename,
                               self.line)
         else:
             return self.filename
 
@@ -196,14 +218,17 @@
 
         self.cb_root  = cb_root
         self.tracker  = tracker
         self.item     = item
         self.version  = version
         self.name     = name
 
+    def sorting_key(self):
+        return (self.cb_root, self.tracker, self.item)
+
     def to_string(self):
         if self.name:
             return "cb item %u '%s'" % (self.item, self.name)
         else:
             return "cb item %u" % self.item
 
     def to_html(self):
```

### Comparing `bmw-lobster-monolithic-0.9.8/lobster/report.py` & `bmw-lobster-monolithic-0.9.9/lobster/report.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-monolithic-0.9.8/lobster/tools/codebeamer/codebeamer.py` & `bmw-lobster-monolithic-0.9.9/lobster/tools/codebeamer/codebeamer.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-monolithic-0.9.8/lobster/tools/core/ci_report.py` & `bmw-lobster-monolithic-0.9.9/lobster/tools/core/ci_report.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-monolithic-0.9.8/lobster/tools/core/html_report.py` & `bmw-lobster-monolithic-0.9.9/lobster/tools/core/html_report.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,18 @@
 import html
 import subprocess
 import hashlib
 import tempfile
 
 from lobster.html import htmldoc, assets
 from lobster.report import Report
+from lobster.location import (Void_Reference,
+                              File_Reference,
+                              Github_Reference,
+                              Codebeamer_Reference)
 from lobster.items import (Tracing_Status, Item,
                            Requirement, Implementation, Activity)
 
 LOBSTER_GH = "https://github.com/bmw-software-engineering/lobster"
 
 
 def is_dot_available():
@@ -383,15 +387,16 @@
               "include the tracing policy visualisation")
         print("> please install Graphviz (https://graphviz.org)")
     doc.add_line('</div>')
 
     ### Issues
     doc.add_heading(2, "Issues", "issues")
     has_issues = False
-    for item in report.items.values():
+    for item in sorted(report.items.values(),
+                       key = lambda x: x.location.sorting_key()):
         if item.tracing_status not in (Tracing_Status.OK,
                                        Tracing_Status.JUSTIFIED):
             for message in item.messages:
                 if not has_issues:
                     has_issues = True
                     doc.add_line("<ul>")
                 doc.add_line("<li>%s: %s</li>" %
@@ -399,14 +404,15 @@
                               message))
     if has_issues:
         doc.add_line("</ul>")
     else:
         doc.add_line("<div>No traceability issues found.</div>")
 
     ### Report
+    file_heading = None
     doc.add_heading(2, "Detailed report", "detailed-report")
     items_by_level = {}
     for level in report.config:
         items_by_level[level] = [item
                                  for item in report.items.values()
                                  if item.level == level]
     for kind, title in [("requirements",
@@ -418,17 +424,32 @@
         doc.add_heading(3, title)
         for level in report.config.values():
             if level["kind"] != kind:
                 continue
             doc.add_heading(4,
                             html.escape(level["name"]),
                             name_hash(level["name"]))
-
             if items_by_level[level["name"]]:
-                for item in items_by_level[level["name"]]:
+                for item in sorted(items_by_level[level["name"]],
+                                   key = lambda x: x.location.sorting_key()):
+                    if isinstance(item.location, Void_Reference):
+                        new_file_heading = "Unknown"
+                    elif isinstance(item.location, (File_Reference,
+                                                    Github_Reference)):
+                        new_file_heading = item.location.filename
+                    elif isinstance(item.location, Codebeamer_Reference):
+                        new_file_heading = "Codebeamer %s, tracker %u" % \
+                            (item.location.cb_root,
+                             item.location.tracker)
+                    else:  # pragma: no cover
+                        assert False
+                    if new_file_heading != file_heading:
+                        file_heading = new_file_heading
+                        doc.add_heading(5, html.escape(file_heading))
+
                     write_item_box_begin(doc, item)
                     if isinstance(item, Requirement) and item.status:
                         doc.add_line('<div class="attribute">')
                         doc.add_line("Status: %s" % html.escape(item.status))
                         doc.add_line('</div>')
                     if isinstance(item, Requirement) and item.text:
                         doc.add_line('<div class="attribute">')
```

### Comparing `bmw-lobster-monolithic-0.9.8/lobster/tools/core/online_report.py` & `bmw-lobster-monolithic-0.9.9/lobster/tools/core/online_report.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-monolithic-0.9.8/lobster/tools/core/report.py` & `bmw-lobster-monolithic-0.9.9/lobster/tools/core/report.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,14 @@
         return 1
 
     if os.path.exists(options.out) and not os.path.isfile(options.out):
         print("error: cannot write to '%s'" % options.out)
         print("error: '%s' exists and is not a file" % options.out)
         return 1
 
-
     report = Report()
 
     try:
         report.parse_config(options.lobster_config)
     except LOBSTER_Error:
         print("lobster: aborting due to earlier errors.")
         return 1
```

### Comparing `bmw-lobster-monolithic-0.9.8/lobster/tools/cpp/cpp.py` & `bmw-lobster-monolithic-0.9.9/lobster/tools/cpp/cpp.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-monolithic-0.9.8/lobster/tools/gtest/gtest.py` & `bmw-lobster-monolithic-0.9.9/lobster/tools/gtest/gtest.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-monolithic-0.9.8/lobster/tools/json/json.py` & `bmw-lobster-monolithic-0.9.9/lobster/tools/json/json.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-monolithic-0.9.8/lobster/tools/python/python.py` & `bmw-lobster-monolithic-0.9.9/lobster/tools/python/python.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-monolithic-0.9.8/lobster/tools/trlc/trlc.py` & `bmw-lobster-monolithic-0.9.9/lobster/tools/trlc/trlc.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-monolithic-0.9.8/lobster/version.py` & `bmw-lobster-monolithic-0.9.9/lobster/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,14 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
 # Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public
 # License along with this program. If not, see
 # <https://www.gnu.org/licenses/>.
 
-VERSION_TUPLE = (0, 9, 8)
+VERSION_TUPLE = (0, 9, 9)
 VERSION_SUFFIX = ""
 
 LOBSTER_VERSION = ("%u.%u.%u" % VERSION_TUPLE) + \
     ("-%s" % VERSION_SUFFIX if VERSION_SUFFIX else "")
 
 FULL_NAME = "LOBSTER %s" % LOBSTER_VERSION
```

### Comparing `bmw-lobster-monolithic-0.9.8/setup.py` & `bmw-lobster-monolithic-0.9.9/setup.py`

 * *Files identical despite different names*

