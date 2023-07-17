# Comparing `tmp/spdb-1.0.4.tar.gz` & `tmp/spdb-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spdb-1.0.4.tar", last modified: Mon Jul 17 13:00:18 2023, max compression
+gzip compressed data, was "spdb-1.0.5.tar", last modified: Mon Jul 17 13:02:08 2023, max compression
```

## Comparing `spdb-1.0.4.tar` & `spdb-1.0.5.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-17 13:00:18.320133 spdb-1.0.4/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     1052 2023-07-17 12:15:45.000000 spdb-1.0.4/LICENSE
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      139 2023-07-17 13:00:18.320133 spdb-1.0.4/PKG-INFO
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     1655 2023-07-17 12:50:32.000000 spdb-1.0.4/README.md
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       38 2023-07-17 13:00:18.320133 spdb-1.0.4/setup.cfg
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      269 2023-07-17 13:00:13.000000 spdb-1.0.4/setup.py
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-17 13:00:18.320133 spdb-1.0.4/spdb/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      170 2023-07-17 10:29:25.000000 spdb-1.0.4/spdb/__init__.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     1596 2023-07-17 12:41:12.000000 spdb-1.0.4/spdb/db.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      596 2023-07-17 12:49:27.000000 spdb-1.0.4/spdb/generator_utils.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     1047 2023-07-17 12:49:07.000000 spdb-1.0.4/spdb/otp.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      325 2023-07-17 12:10:08.000000 spdb-1.0.4/spdb/text_validator.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      654 2023-07-17 12:46:37.000000 spdb-1.0.4/spdb/token_generator.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       34 2023-07-17 10:29:15.000000 spdb-1.0.4/spdb/utils.py
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-17 13:00:18.320133 spdb-1.0.4/spdb.egg-info/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      139 2023-07-17 13:00:18.000000 spdb-1.0.4/spdb.egg-info/PKG-INFO
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      317 2023-07-17 13:00:18.000000 spdb-1.0.4/spdb.egg-info/SOURCES.txt
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2023-07-17 13:00:18.000000 spdb-1.0.4/spdb.egg-info/dependency_links.txt
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2023-07-17 10:51:25.000000 spdb-1.0.4/spdb.egg-info/not-zip-safe
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       13 2023-07-17 13:00:18.000000 spdb-1.0.4/spdb.egg-info/requires.txt
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)        5 2023-07-17 13:00:18.000000 spdb-1.0.4/spdb.egg-info/top_level.txt
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-17 13:02:08.005794 spdb-1.0.5/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     1052 2023-07-17 12:15:45.000000 spdb-1.0.5/LICENSE
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     2139 2023-07-17 13:02:08.005794 spdb-1.0.5/PKG-INFO
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     1655 2023-07-17 12:50:32.000000 spdb-1.0.5/README.md
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      468 2023-07-17 13:02:03.000000 spdb-1.0.5/pyproject.toml
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       38 2023-07-17 13:02:08.005794 spdb-1.0.5/setup.cfg
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      246 2023-07-17 13:02:00.000000 spdb-1.0.5/setup.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-17 13:02:08.002460 spdb-1.0.5/spdb/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      170 2023-07-17 10:29:25.000000 spdb-1.0.5/spdb/__init__.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     1596 2023-07-17 12:41:12.000000 spdb-1.0.5/spdb/db.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      596 2023-07-17 12:49:27.000000 spdb-1.0.5/spdb/generator_utils.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     1047 2023-07-17 12:49:07.000000 spdb-1.0.5/spdb/otp.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      325 2023-07-17 12:10:08.000000 spdb-1.0.5/spdb/text_validator.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      654 2023-07-17 12:46:37.000000 spdb-1.0.5/spdb/token_generator.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       34 2023-07-17 10:29:15.000000 spdb-1.0.5/spdb/utils.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-17 13:02:08.002460 spdb-1.0.5/spdb.egg-info/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     2139 2023-07-17 13:02:07.000000 spdb-1.0.5/spdb.egg-info/PKG-INFO
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      332 2023-07-17 13:02:07.000000 spdb-1.0.5/spdb.egg-info/SOURCES.txt
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2023-07-17 13:02:07.000000 spdb-1.0.5/spdb.egg-info/dependency_links.txt
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2023-07-17 10:51:25.000000 spdb-1.0.5/spdb.egg-info/not-zip-safe
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       13 2023-07-17 13:02:07.000000 spdb-1.0.5/spdb.egg-info/requires.txt
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)        5 2023-07-17 13:02:07.000000 spdb-1.0.5/spdb.egg-info/top_level.txt
```

### Comparing `spdb-1.0.4/LICENSE` & `spdb-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `spdb-1.0.4/README.md` & `spdb-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `spdb-1.0.4/spdb/db.py` & `spdb-1.0.5/spdb/db.py`

 * *Files identical despite different names*

### Comparing `spdb-1.0.4/spdb/generator_utils.py` & `spdb-1.0.5/spdb/generator_utils.py`

 * *Files identical despite different names*

### Comparing `spdb-1.0.4/spdb/otp.py` & `spdb-1.0.5/spdb/otp.py`

 * *Files identical despite different names*

### Comparing `spdb-1.0.4/spdb/token_generator.py` & `spdb-1.0.5/spdb/token_generator.py`

 * *Files identical despite different names*

