# Comparing `tmp/bbva2pandas-1.1.1.tar.gz` & `tmp/bbva2pandas-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbva2pandas-1.1.1.tar", last modified: Sun Jul  3 20:35:50 2022, max compression
+gzip compressed data, was "bbva2pandas-1.1.2.tar", last modified: Mon Jul 17 06:50:41 2023, max compression
```

## Comparing `bbva2pandas-1.1.1.tar` & `bbva2pandas-1.1.2.tar`

### file list

```diff
@@ -1,24 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-03 20:35:50.266202 bbva2pandas-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (121)      912 2022-07-03 20:35:29.000000 bbva2pandas-1.1.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-07-03 20:35:29.000000 bbva2pandas-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-07-03 20:35:29.000000 bbva2pandas-1.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2162 2022-07-03 20:35:50.266202 bbva2pandas-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1213 2022-07-03 20:35:29.000000 bbva2pandas-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-03 20:35:50.266202 bbva2pandas-1.1.1/bbva2pandas/
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-03 20:35:29.000000 bbva2pandas-1.1.1/bbva2pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1168 2022-07-03 20:35:29.000000 bbva2pandas-1.1.1/bbva2pandas/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (121)      767 2022-07-03 20:35:29.000000 bbva2pandas-1.1.1/bbva2pandas/extractor.py
--rw-r--r--   0 runner    (1001) docker     (121)      352 2022-07-03 20:35:29.000000 bbva2pandas-1.1.1/bbva2pandas/pdf.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      589 2022-07-03 20:35:29.000000 bbva2pandas-1.1.1/bbva2pandas/report.py
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-07-03 20:35:29.000000 bbva2pandas-1.1.1/bbva2pandas/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-03 20:35:50.266202 bbva2pandas-1.1.1/bbva2pandas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2162 2022-07-03 20:35:49.000000 bbva2pandas-1.1.1/bbva2pandas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      395 2022-07-03 20:35:50.000000 bbva2pandas-1.1.1/bbva2pandas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-03 20:35:49.000000 bbva2pandas-1.1.1/bbva2pandas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-07-03 20:35:50.000000 bbva2pandas-1.1.1/bbva2pandas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-07-03 20:35:50.000000 bbva2pandas-1.1.1/bbva2pandas.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-03 20:35:50.266202 bbva2pandas-1.1.1/bin/
--rwxr-xr-x   0 runner    (1001) docker     (121)     1530 2022-07-03 20:35:29.000000 bbva2pandas-1.1.1/bin/bbva2pandas
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-07-03 20:35:29.000000 bbva2pandas-1.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-03 20:35:50.266202 bbva2pandas-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1510 2022-07-03 20:35:29.000000 bbva2pandas-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:50:41.189893 bbva2pandas-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-17 06:50:15.000000 bbva2pandas-1.1.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-17 06:50:15.000000 bbva2pandas-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-17 06:50:15.000000 bbva2pandas-1.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-17 06:50:41.189893 bbva2pandas-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-17 06:50:15.000000 bbva2pandas-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:50:41.185893 bbva2pandas-1.1.2/bbva2pandas/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 06:50:15.000000 bbva2pandas-1.1.2/bbva2pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-17 06:50:15.000000 bbva2pandas-1.1.2/bbva2pandas/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-17 06:50:15.000000 bbva2pandas-1.1.2/bbva2pandas/extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-17 06:50:15.000000 bbva2pandas-1.1.2/bbva2pandas/pdf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      589 2023-07-17 06:50:15.000000 bbva2pandas-1.1.2/bbva2pandas/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-17 06:50:15.000000 bbva2pandas-1.1.2/bbva2pandas/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:50:41.185893 bbva2pandas-1.1.2/bbva2pandas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-17 06:50:41.000000 bbva2pandas-1.1.2/bbva2pandas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-17 06:50:41.000000 bbva2pandas-1.1.2/bbva2pandas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 06:50:41.000000 bbva2pandas-1.1.2/bbva2pandas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-17 06:50:41.000000 bbva2pandas-1.1.2/bbva2pandas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-17 06:50:41.000000 bbva2pandas-1.1.2/bbva2pandas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:50:41.189893 bbva2pandas-1.1.2/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1530 2023-07-17 06:50:15.000000 bbva2pandas-1.1.2/bin/bbva2pandas
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-17 06:50:15.000000 bbva2pandas-1.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 06:50:41.189893 bbva2pandas-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-17 06:50:15.000000 bbva2pandas-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:50:41.189893 bbva2pandas-1.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-17 06:50:15.000000 bbva2pandas-1.1.2/tests/test_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-17 06:50:15.000000 bbva2pandas-1.1.2/tests/test_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-17 06:50:15.000000 bbva2pandas-1.1.2/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-17 06:50:15.000000 bbva2pandas-1.1.2/tests/test_pdf.py
```

### Comparing `bbva2pandas-1.1.1/CHANGELOG.md` & `bbva2pandas-1.1.2/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 # Change Log
 All notable changes to this project will be documented in this file.
 This project adheres to [Semantic Versioning](http://semver.org/) and [Keep a changelog](https://github.com/olivierlacan/keep-a-changelog).
 
 ## [Unreleased](https://github.com/blalop/bbva2pandas/tree/main)
 
+## [1.1.2](https://github.com/idealista/bbva2pandas/tree/1.1.2)
+### Fixed
+- [#8](https://github.com/blalop/bbva2pandas/pull/8) Fixing issue with empty sub-concepts @neugartf
+
 ## [1.1.1](https://github.com/idealista/bbva2pandas/tree/1.1.1)
 ### Changed
-- Physical flag for pdftotext
+- [#6](https://github.com/blalop/bbva2pandas/pull/6) Physical flag for pdftotext
 
 ## [1.1.0](https://github.com/idealista/bbva2pandas/tree/1.1.0)
 ### Added
 - Python 3.10 support
 ### Fixed
-- Fixing an issue with regex recognizing certain characters @neugartf
+- [#3](https://github.com/blalop/bbva2pandas/pull/3) Fixing an issue with regex recognizing certain characters @neugartf
 ### Removed
 - Python 3.7 support
 - Remove Grafana dashboard - use [blalop/bbva2pandas-notebook](https://github.com/blalop/bbva2pandas-notebook) instead
 
 ## [1.0.0](https://github.com/idealista/bbva2pandas/tree/1.0.0)
 ### Changed
 - API refactoring
```

### Comparing `bbva2pandas-1.1.1/LICENSE` & `bbva2pandas-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bbva2pandas-1.1.1/PKG-INFO` & `bbva2pandas-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbva2pandas
-Version: 1.1.1
+Version: 1.1.2
 Summary: Parse BBVA monthly reports directly to a Dataframe
 Home-page: https://github.com/blalop/bbva2pandas
 Author: Alejandro Blanco López
 Author-email: alexbl1996@gmail.com
 License: GPLv3+
 Keywords: bbva pdf bank regex
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `bbva2pandas-1.1.1/README.md` & `bbva2pandas-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `bbva2pandas-1.1.1/bbva2pandas/dataframe.py` & `bbva2pandas-1.1.2/bbva2pandas/dataframe.py`

 * *Files identical despite different names*

### Comparing `bbva2pandas-1.1.1/bbva2pandas/report.py` & `bbva2pandas-1.1.2/bbva2pandas/report.py`

 * *Files identical despite different names*

### Comparing `bbva2pandas-1.1.1/bbva2pandas.egg-info/PKG-INFO` & `bbva2pandas-1.1.2/bbva2pandas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbva2pandas
-Version: 1.1.1
+Version: 1.1.2
 Summary: Parse BBVA monthly reports directly to a Dataframe
 Home-page: https://github.com/blalop/bbva2pandas
 Author: Alejandro Blanco López
 Author-email: alexbl1996@gmail.com
 License: GPLv3+
 Keywords: bbva pdf bank regex
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `bbva2pandas-1.1.1/bin/bbva2pandas` & `bbva2pandas-1.1.2/bin/bbva2pandas`

 * *Files identical despite different names*

### Comparing `bbva2pandas-1.1.1/setup.py` & `bbva2pandas-1.1.2/setup.py`

 * *Files identical despite different names*

