# Comparing `tmp/spdb-1.0.1.tar.gz` & `tmp/spdb-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spdb-1.0.1.tar", last modified: Mon Jul 17 10:44:44 2023, max compression
+gzip compressed data, was "spdb-1.0.2.tar", last modified: Mon Jul 17 10:52:26 2023, max compression
```

## Comparing `spdb-1.0.1.tar` & `spdb-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-17 10:44:44.579023 spdb-1.0.1/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      117 2023-07-17 10:44:44.579023 spdb-1.0.1/PKG-INFO
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       38 2023-07-17 10:44:44.579023 spdb-1.0.1/setup.cfg
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-17 10:44:44.575690 spdb-1.0.1/spdb/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      170 2023-07-17 10:29:25.000000 spdb-1.0.1/spdb/__init__.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     1448 2023-07-17 10:26:37.000000 spdb-1.0.1/spdb/db.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      584 2023-07-17 10:26:50.000000 spdb-1.0.1/spdb/generator_utils.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      974 2023-07-17 10:26:29.000000 spdb-1.0.1/spdb/otp.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      246 2023-07-17 10:44:15.000000 spdb-1.0.1/spdb/setup.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      316 2023-07-17 10:26:46.000000 spdb-1.0.1/spdb/text_validator.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      633 2023-07-17 10:26:40.000000 spdb-1.0.1/spdb/token_generator.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       34 2023-07-17 10:29:15.000000 spdb-1.0.1/spdb/utils.py
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-17 10:44:44.575690 spdb-1.0.1/spdb.egg-info/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      117 2023-07-17 10:44:44.000000 spdb-1.0.1/spdb.egg-info/PKG-INFO
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      304 2023-07-17 10:44:44.000000 spdb-1.0.1/spdb.egg-info/SOURCES.txt
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2023-07-17 10:44:44.000000 spdb-1.0.1/spdb.egg-info/dependency_links.txt
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2023-07-17 10:44:44.000000 spdb-1.0.1/spdb.egg-info/not-zip-safe
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       13 2023-07-17 10:44:44.000000 spdb-1.0.1/spdb.egg-info/requires.txt
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)        5 2023-07-17 10:44:44.000000 spdb-1.0.1/spdb.egg-info/top_level.txt
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-17 10:52:26.712073 spdb-1.0.2/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      117 2023-07-17 10:52:26.712073 spdb-1.0.2/PKG-INFO
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       38 2023-07-17 10:52:26.712073 spdb-1.0.2/setup.cfg
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      246 2023-07-17 10:52:20.000000 spdb-1.0.2/setup.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-17 10:52:26.708740 spdb-1.0.2/spdb/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      170 2023-07-17 10:29:25.000000 spdb-1.0.2/spdb/__init__.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     1448 2023-07-17 10:26:37.000000 spdb-1.0.2/spdb/db.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      584 2023-07-17 10:26:50.000000 spdb-1.0.2/spdb/generator_utils.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      974 2023-07-17 10:26:29.000000 spdb-1.0.2/spdb/otp.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      316 2023-07-17 10:26:46.000000 spdb-1.0.2/spdb/text_validator.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      633 2023-07-17 10:26:40.000000 spdb-1.0.2/spdb/token_generator.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       34 2023-07-17 10:29:15.000000 spdb-1.0.2/spdb/utils.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-17 10:52:26.712073 spdb-1.0.2/spdb.egg-info/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      117 2023-07-17 10:52:26.000000 spdb-1.0.2/spdb.egg-info/PKG-INFO
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      299 2023-07-17 10:52:26.000000 spdb-1.0.2/spdb.egg-info/SOURCES.txt
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2023-07-17 10:52:26.000000 spdb-1.0.2/spdb.egg-info/dependency_links.txt
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2023-07-17 10:51:25.000000 spdb-1.0.2/spdb.egg-info/not-zip-safe
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       13 2023-07-17 10:52:26.000000 spdb-1.0.2/spdb.egg-info/requires.txt
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)        5 2023-07-17 10:52:26.000000 spdb-1.0.2/spdb.egg-info/top_level.txt
```

### Comparing `spdb-1.0.1/spdb/db.py` & `spdb-1.0.2/spdb/db.py`

 * *Files identical despite different names*

### Comparing `spdb-1.0.1/spdb/generator_utils.py` & `spdb-1.0.2/spdb/generator_utils.py`

 * *Files identical despite different names*

### Comparing `spdb-1.0.1/spdb/otp.py` & `spdb-1.0.2/spdb/otp.py`

 * *Files identical despite different names*

### Comparing `spdb-1.0.1/spdb/token_generator.py` & `spdb-1.0.2/spdb/token_generator.py`

 * *Files identical despite different names*

