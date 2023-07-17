# Comparing `tmp/dj-veryfi-0.1.8.tar.gz` & `tmp/dj-veryfi-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dj-veryfi-0.1.8.tar", last modified: Mon Jul 17 14:44:23 2023, max compression
+gzip compressed data, was "dist/dj-veryfi-0.1.9.tar", last modified: Mon Jul 17 14:52:09 2023, max compression
```

## Comparing `dj-veryfi-0.1.8.tar` & `dj-veryfi-0.1.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 tony      (1000) tony      (1000)        0 2023-07-17 14:44:23.000000 dj-veryfi-0.1.8/
--rw-r--r--   0 tony      (1000) tony      (1000)     1139 2023-07-15 23:02:53.000000 dj-veryfi-0.1.8/LICENSE
--rw-r--r--   0 tony      (1000) tony      (1000)     3501 2023-07-17 14:44:23.000000 dj-veryfi-0.1.8/PKG-INFO
--rw-r--r--   0 tony      (1000) tony      (1000)     2883 2023-07-17 14:07:47.000000 dj-veryfi-0.1.8/README.md
-drwxr-xr-x   0 tony      (1000) tony      (1000)        0 2023-07-17 14:44:23.000000 dj-veryfi-0.1.8/dj_veryfi/
--rw-r--r--   0 tony      (1000) tony      (1000)      149 2023-07-15 18:29:43.000000 dj-veryfi-0.1.8/dj_veryfi/apps.py
-drwxr-xr-x   0 tony      (1000) tony      (1000)        0 2023-07-17 14:44:23.000000 dj-veryfi-0.1.8/dj_veryfi/dj_veryfi.egg-info/
--rw-r--r--   0 tony      (1000) tony      (1000)     3501 2023-07-17 14:44:23.000000 dj-veryfi-0.1.8/dj_veryfi/dj_veryfi.egg-info/PKG-INFO
--rw-r--r--   0 tony      (1000) tony      (1000)      432 2023-07-17 14:44:23.000000 dj-veryfi-0.1.8/dj_veryfi/dj_veryfi.egg-info/SOURCES.txt
--rw-r--r--   0 tony      (1000) tony      (1000)        1 2023-07-17 14:44:23.000000 dj-veryfi-0.1.8/dj_veryfi/dj_veryfi.egg-info/dependency_links.txt
--rw-r--r--   0 tony      (1000) tony      (1000)       50 2023-07-17 14:44:23.000000 dj-veryfi-0.1.8/dj_veryfi/dj_veryfi.egg-info/requires.txt
--rw-r--r--   0 tony      (1000) tony      (1000)       43 2023-07-17 14:44:23.000000 dj-veryfi-0.1.8/dj_veryfi/dj_veryfi.egg-info/top_level.txt
--rw-r--r--   0 tony      (1000) tony      (1000)     1758 2023-07-15 22:01:27.000000 dj-veryfi-0.1.8/dj_veryfi/fields.py
-drwxr-xr-x   0 tony      (1000) tony      (1000)        0 2023-07-17 14:44:23.000000 dj-veryfi-0.1.8/dj_veryfi/migrations/
--rw-r--r--   0 tony      (1000) tony      (1000)      615 2023-07-15 22:04:41.000000 dj-veryfi-0.1.8/dj_veryfi/migrations/0001_initial.py
--rw-r--r--   0 tony      (1000) tony      (1000)        0 2023-07-15 18:29:43.000000 dj-veryfi-0.1.8/dj_veryfi/migrations/__init__.py
--rw-r--r--   0 tony      (1000) tony      (1000)      235 2023-07-15 22:01:46.000000 dj-veryfi-0.1.8/dj_veryfi/models.py
--rw-r--r--   0 tony      (1000) tony      (1000)     2063 2023-07-15 22:03:59.000000 dj-veryfi-0.1.8/dj_veryfi/tests.py
--rw-r--r--   0 tony      (1000) tony      (1000)      398 2023-07-15 18:33:52.000000 dj-veryfi-0.1.8/dj_veryfi/veryfi.py
--rw-r--r--   0 tony      (1000) tony      (1000)       86 2023-07-16 00:47:58.000000 dj-veryfi-0.1.8/pyproject.toml
--rw-r--r--   0 tony      (1000) tony      (1000)      767 2023-07-17 14:44:23.000000 dj-veryfi-0.1.8/setup.cfg
--rw-r--r--   0 tony      (1000) tony      (1000)      154 2023-07-17 14:17:27.000000 dj-veryfi-0.1.8/setup.py
+drwxr-xr-x   0 tony      (1000) tony      (1000)        0 2023-07-17 14:52:09.000000 dj-veryfi-0.1.9/
+-rw-r--r--   0 tony      (1000) tony      (1000)     1139 2023-07-15 23:02:53.000000 dj-veryfi-0.1.9/LICENSE
+-rw-r--r--   0 tony      (1000) tony      (1000)     3501 2023-07-17 14:52:09.000000 dj-veryfi-0.1.9/PKG-INFO
+-rw-r--r--   0 tony      (1000) tony      (1000)     2883 2023-07-17 14:07:47.000000 dj-veryfi-0.1.9/README.md
+drwxr-xr-x   0 tony      (1000) tony      (1000)        0 2023-07-17 14:52:09.000000 dj-veryfi-0.1.9/dj_veryfi/
+-rw-r--r--   0 tony      (1000) tony      (1000)        0 2023-07-15 18:29:43.000000 dj-veryfi-0.1.9/dj_veryfi/__init__.py
+-rw-r--r--   0 tony      (1000) tony      (1000)       63 2023-07-15 18:29:43.000000 dj-veryfi-0.1.9/dj_veryfi/admin.py
+-rw-r--r--   0 tony      (1000) tony      (1000)      149 2023-07-15 18:29:43.000000 dj-veryfi-0.1.9/dj_veryfi/apps.py
+-rw-r--r--   0 tony      (1000) tony      (1000)     1758 2023-07-15 22:01:27.000000 dj-veryfi-0.1.9/dj_veryfi/fields.py
+-rw-r--r--   0 tony      (1000) tony      (1000)      235 2023-07-15 22:01:46.000000 dj-veryfi-0.1.9/dj_veryfi/models.py
+-rw-r--r--   0 tony      (1000) tony      (1000)     2063 2023-07-15 22:03:59.000000 dj-veryfi-0.1.9/dj_veryfi/tests.py
+-rw-r--r--   0 tony      (1000) tony      (1000)      398 2023-07-15 18:33:52.000000 dj-veryfi-0.1.9/dj_veryfi/veryfi.py
+-rw-r--r--   0 tony      (1000) tony      (1000)       63 2023-07-15 18:29:43.000000 dj-veryfi-0.1.9/dj_veryfi/views.py
+drwxr-xr-x   0 tony      (1000) tony      (1000)        0 2023-07-17 14:52:09.000000 dj-veryfi-0.1.9/dj_veryfi.egg-info/
+-rw-r--r--   0 tony      (1000) tony      (1000)     3501 2023-07-17 14:52:09.000000 dj-veryfi-0.1.9/dj_veryfi.egg-info/PKG-INFO
+-rw-r--r--   0 tony      (1000) tony      (1000)      372 2023-07-17 14:52:09.000000 dj-veryfi-0.1.9/dj_veryfi.egg-info/SOURCES.txt
+-rw-r--r--   0 tony      (1000) tony      (1000)        1 2023-07-17 14:52:09.000000 dj-veryfi-0.1.9/dj_veryfi.egg-info/dependency_links.txt
+-rw-r--r--   0 tony      (1000) tony      (1000)       50 2023-07-17 14:52:09.000000 dj-veryfi-0.1.9/dj_veryfi.egg-info/requires.txt
+-rw-r--r--   0 tony      (1000) tony      (1000)       10 2023-07-17 14:52:09.000000 dj-veryfi-0.1.9/dj_veryfi.egg-info/top_level.txt
+-rw-r--r--   0 tony      (1000) tony      (1000)       86 2023-07-16 00:47:58.000000 dj-veryfi-0.1.9/pyproject.toml
+-rw-r--r--   0 tony      (1000) tony      (1000)      680 2023-07-17 14:52:09.000000 dj-veryfi-0.1.9/setup.cfg
+-rw-r--r--   0 tony      (1000) tony      (1000)      156 2023-07-17 14:50:05.000000 dj-veryfi-0.1.9/setup.py
```

### Comparing `dj-veryfi-0.1.8/LICENSE` & `dj-veryfi-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dj-veryfi-0.1.8/PKG-INFO` & `dj-veryfi-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-veryfi
-Version: 0.1.8
+Version: 0.1.9
 Summary: Django integration for Veryfi OCR API.
 Home-page: https://github.com/tonykamillo/dj-veryfi
 Author: Tony Kamillo
 Author-email: tonykamillo@gmail.com
 License: DBAD
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `dj-veryfi-0.1.8/README.md` & `dj-veryfi-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `dj-veryfi-0.1.8/dj_veryfi/dj_veryfi.egg-info/PKG-INFO` & `dj-veryfi-0.1.9/dj_veryfi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-veryfi
-Version: 0.1.8
+Version: 0.1.9
 Summary: Django integration for Veryfi OCR API.
 Home-page: https://github.com/tonykamillo/dj-veryfi
 Author: Tony Kamillo
 Author-email: tonykamillo@gmail.com
 License: DBAD
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `dj-veryfi-0.1.8/dj_veryfi/fields.py` & `dj-veryfi-0.1.9/dj_veryfi/fields.py`

 * *Files identical despite different names*

### Comparing `dj-veryfi-0.1.8/dj_veryfi/tests.py` & `dj-veryfi-0.1.9/dj_veryfi/tests.py`

 * *Files identical despite different names*

