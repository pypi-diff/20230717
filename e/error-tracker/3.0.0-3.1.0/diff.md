# Comparing `tmp/error-tracker-3.0.0.tar.gz` & `tmp/error-tracker-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "error-tracker-3.0.0.tar", last modified: Thu May 26 09:15:33 2022, max compression
+gzip compressed data, was "error-tracker-3.1.0.tar", last modified: Mon Jul 17 17:15:33 2023, max compression
```

## Comparing `error-tracker-3.0.0.tar` & `error-tracker-3.1.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 sonu       (501) staff       (20)        0 2022-05-26 09:15:33.120334 error-tracker-3.0.0/
--rw-r--r--   0 sonu       (501) staff       (20)     1504 2022-05-24 12:57:32.000000 error-tracker-3.0.0/LICENSE.txt
--rwxr-xr-x   0 sonu       (501) staff       (20)      112 2022-05-24 12:57:32.000000 error-tracker-3.0.0/MANIFEST.in
--rw-r--r--   0 sonu       (501) staff       (20)     7049 2022-05-26 09:15:33.120494 error-tracker-3.0.0/PKG-INFO
--rw-r--r--   0 sonu       (501) staff       (20)     5787 2022-05-24 12:57:32.000000 error-tracker-3.0.0/README.rst
-drwxr-xr-x   0 sonu       (501) staff       (20)        0 2022-05-26 09:15:33.091744 error-tracker-3.0.0/error_tracker/
--rw-r--r--   0 sonu       (501) staff       (20)     1377 2022-05-26 09:14:37.000000 error-tracker-3.0.0/error_tracker/__init__.py
-drwxr-xr-x   0 sonu       (501) staff       (20)        0 2022-05-26 09:15:33.100836 error-tracker-3.0.0/error_tracker/django/
--rw-r--r--   0 sonu       (501) staff       (20)     2741 2022-05-24 12:57:32.000000 error-tracker-3.0.0/error_tracker/django/__init__.py
--rw-r--r--   0 sonu       (501) staff       (20)     1291 2022-05-24 12:57:32.000000 error-tracker-3.0.0/error_tracker/django/admin.py
--rw-r--r--   0 sonu       (501) staff       (20)      384 2022-05-24 12:57:32.000000 error-tracker-3.0.0/error_tracker/django/apps.py
--rw-r--r--   0 sonu       (501) staff       (20)     4794 2022-05-24 12:57:32.000000 error-tracker-3.0.0/error_tracker/django/middleware.py
-drwxr-xr-x   0 sonu       (501) staff       (20)        0 2022-05-26 09:15:33.102332 error-tracker-3.0.0/error_tracker/django/migrations/
--rw-r--r--   0 sonu       (501) staff       (20)     1213 2022-05-24 12:57:32.000000 error-tracker-3.0.0/error_tracker/django/migrations/0001_initial.py
--rw-r--r--   0 sonu       (501) staff       (20)      561 2022-05-24 12:57:32.000000 error-tracker-3.0.0/error_tracker/django/migrations/0002_auto_20201018_1311.py
--rw-r--r--   0 sonu       (501) staff       (20)        0 2022-05-24 12:57:32.000000 error-tracker-3.0.0/error_tracker/django/migrations/__init__.py
--rw-r--r--   0 sonu       (501) staff       (20)     3333 2022-05-24 12:57:32.000000 error-tracker-3.0.0/error_tracker/django/models.py
--rw-r--r--   0 sonu       (501) staff       (20)     2264 2022-05-24 12:57:32.000000 error-tracker-3.0.0/error_tracker/django/settings.py
-drwxr-xr-x   0 sonu       (501) staff       (20)        0 2022-05-26 09:15:33.087482 error-tracker-3.0.0/error_tracker/django/templates/
-drwxr-xr-x   0 sonu       (501) staff       (20)        0 2022-05-26 09:15:33.103528 error-tracker-3.0.0/error_tracker/django/templates/error_tracker/
-drwxr-xr-x   0 sonu       (501) staff       (20)        0 2022-05-26 09:15:33.104176 error-tracker-3.0.0/error_tracker/django/templates/error_tracker/admin/
--rw-r--r--   0 sonu       (501) staff       (20)      117 2022-05-24 12:57:32.000000 error-tracker-3.0.0/error_tracker/django/templates/error_tracker/admin/change_form.html
--rwxr-xr-x   0 sonu       (501) staff       (20)     1428 2022-05-26 09:14:37.000000 error-tracker-3.0.0/error_tracker/django/templates/error_tracker/base.html
--rwxr-xr-x   0 sonu       (501) staff       (20)     1984 2022-05-24 12:57:32.000000 error-tracker-3.0.0/error_tracker/django/templates/error_tracker/detail.html
--rwxr-xr-x   0 sonu       (501) staff       (20)     4150 2022-05-24 12:57:32.000000 error-tracker-3.0.0/error_tracker/django/templates/error_tracker/list.html
-drwxr-xr-x   0 sonu       (501) staff       (20)        0 2022-05-26 09:15:33.105085 error-tracker-3.0.0/error_tracker/django/templates/error_tracker/partials/
--rw-r--r--   0 sonu       (501) staff       (20)      546 2022-05-24 12:57:32.000000 error-tracker-3.0.0/error_tracker/django/templates/error_tracker/partials/navigation.html
--rw-r--r--   0 sonu       (501) staff       (20)      725 2022-05-26 09:14:37.000000 error-tracker-3.0.0/error_tracker/django/templates/error_tracker/partials/partial_table.html
-drwxr-xr-x   0 sonu       (501) staff       (20)        0 2022-05-26 09:15:33.106995 error-tracker-3.0.0/error_tracker/django/templatetags/
--rw-r--r--   0 sonu       (501) staff       (20)        0 2022-05-24 12:57:32.000000 error-tracker-3.0.0/error_tracker/django/templatetags/__init__.py
--rw-r--r--   0 sonu       (501) staff       (20)      818 2022-05-24 12:57:32.000000 error-tracker-3.0.0/error_tracker/django/templatetags/error_tracker.py
--rwxr-xr-x   0 sonu       (501) staff       (20)      421 2022-05-26 09:14:37.000000 error-tracker-3.0.0/error_tracker/django/urls.py
--rw-r--r--   0 sonu       (501) staff       (20)     7648 2022-05-24 12:57:32.000000 error-tracker-3.0.0/error_tracker/django/utils.py
--rw-r--r--   0 sonu       (501) staff       (20)     2911 2022-05-26 09:14:37.000000 error-tracker-3.0.0/error_tracker/django/views.py
-drwxr-xr-x   0 sonu       (501) staff       (20)        0 2022-05-26 09:15:33.114244 error-tracker-3.0.0/error_tracker/flask/
--rwxr-xr-x   0 sonu       (501) staff       (20)      263 2022-05-24 12:57:32.000000 error-tracker-3.0.0/error_tracker/flask/__init__.py
--rwxr-xr-x   0 sonu       (501) staff       (20)      864 2022-05-24 12:57:32.000000 error-tracker-3.0.0/error_tracker/flask/defaults.py
--rwxr-xr-x   0 sonu       (501) staff       (20)    15094 2022-05-24 12:57:32.000000 error-tracker-3.0.0/error_tracker/flask/flask_error.py
-drwxr-xr-x   0 sonu       (501) staff       (20)        0 2022-05-26 09:15:33.088775 error-tracker-3.0.0/error_tracker/flask/templates/
-drwxr-xr-x   0 sonu       (501) staff       (20)        0 2022-05-26 09:15:33.115578 error-tracker-3.0.0/error_tracker/flask/templates/error_tracker/
--rwxr-xr-x   0 sonu       (501) staff       (20)      538 2022-05-24 12:57:32.000000 error-tracker-3.0.0/error_tracker/flask/templates/error_tracker/base.html
--rwxr-xr-x   0 sonu       (501) staff       (20)     1032 2022-05-24 12:57:32.000000 error-tracker-3.0.0/error_tracker/flask/templates/error_tracker/detail.html
--rwxr-xr-x   0 sonu       (501) staff       (20)     2428 2022-05-24 12:57:32.000000 error-tracker-3.0.0/error_tracker/flask/templates/error_tracker/list.html
--rw-r--r--   0 sonu       (501) staff       (20)     2436 2022-05-24 12:57:32.000000 error-tracker-3.0.0/error_tracker/flask/utils.py
--rw-r--r--   0 sonu       (501) staff       (20)     2642 2022-05-24 12:57:32.000000 error-tracker-3.0.0/error_tracker/flask/view.py
-drwxr-xr-x   0 sonu       (501) staff       (20)        0 2022-05-26 09:15:33.119632 error-tracker-3.0.0/error_tracker/libs/
--rw-r--r--   0 sonu       (501) staff       (20)        0 2022-05-24 12:57:32.000000 error-tracker-3.0.0/error_tracker/libs/__init__.py
--rwxr-xr-x   0 sonu       (501) staff       (20)     5953 2022-05-24 12:57:32.000000 error-tracker-3.0.0/error_tracker/libs/exception_formatter.py
--rwxr-xr-x   0 sonu       (501) staff       (20)     4817 2022-05-24 12:57:32.000000 error-tracker-3.0.0/error_tracker/libs/mixins.py
--rw-r--r--   0 sonu       (501) staff       (20)     4976 2022-05-24 12:57:32.000000 error-tracker-3.0.0/error_tracker/libs/utils.py
-drwxr-xr-x   0 sonu       (501) staff       (20)        0 2022-05-26 09:15:33.094822 error-tracker-3.0.0/error_tracker.egg-info/
--rw-r--r--   0 sonu       (501) staff       (20)     7049 2022-05-26 09:15:33.000000 error-tracker-3.0.0/error_tracker.egg-info/PKG-INFO
--rw-r--r--   0 sonu       (501) staff       (20)     1655 2022-05-26 09:15:33.000000 error-tracker-3.0.0/error_tracker.egg-info/SOURCES.txt
--rw-r--r--   0 sonu       (501) staff       (20)        1 2022-05-26 09:15:33.000000 error-tracker-3.0.0/error_tracker.egg-info/dependency_links.txt
--rw-r--r--   0 sonu       (501) staff       (20)        1 2022-05-24 12:57:56.000000 error-tracker-3.0.0/error_tracker.egg-info/not-zip-safe
--rw-r--r--   0 sonu       (501) staff       (20)       80 2022-05-26 09:15:33.000000 error-tracker-3.0.0/error_tracker.egg-info/requires.txt
--rw-r--r--   0 sonu       (501) staff       (20)       14 2022-05-26 09:15:33.000000 error-tracker-3.0.0/error_tracker.egg-info/top_level.txt
--rw-r--r--   0 sonu       (501) staff       (20)       80 2022-05-26 09:15:33.121660 error-tracker-3.0.0/setup.cfg
--rwxr-xr-x   0 sonu       (501) staff       (20)     2165 2022-05-26 09:14:37.000000 error-tracker-3.0.0/setup.py
+drwxr-xr-x   0 sonu       (501) staff       (20)        0 2023-07-17 17:15:33.330353 error-tracker-3.1.0/
+-rw-r--r--   0 sonu       (501) staff       (20)     1504 2023-07-17 17:13:34.000000 error-tracker-3.1.0/LICENSE.txt
+-rwxr-xr-x   0 sonu       (501) staff       (20)      112 2023-07-17 16:11:51.000000 error-tracker-3.1.0/MANIFEST.in
+-rw-r--r--   0 sonu       (501) staff       (20)     7047 2023-07-17 17:15:33.330490 error-tracker-3.1.0/PKG-INFO
+-rw-r--r--   0 sonu       (501) staff       (20)     5787 2023-07-17 16:11:51.000000 error-tracker-3.1.0/README.rst
+drwxr-xr-x   0 sonu       (501) staff       (20)        0 2023-07-17 17:15:33.314295 error-tracker-3.1.0/error_tracker/
+-rw-r--r--   0 sonu       (501) staff       (20)     1377 2023-07-17 17:11:20.000000 error-tracker-3.1.0/error_tracker/__init__.py
+drwxr-xr-x   0 sonu       (501) staff       (20)        0 2023-07-17 17:15:33.320177 error-tracker-3.1.0/error_tracker/django/
+-rw-r--r--   0 sonu       (501) staff       (20)     2741 2023-07-17 17:11:20.000000 error-tracker-3.1.0/error_tracker/django/__init__.py
+-rw-r--r--   0 sonu       (501) staff       (20)     1291 2023-07-17 16:11:51.000000 error-tracker-3.1.0/error_tracker/django/admin.py
+-rw-r--r--   0 sonu       (501) staff       (20)      384 2023-07-17 16:11:51.000000 error-tracker-3.1.0/error_tracker/django/apps.py
+-rw-r--r--   0 sonu       (501) staff       (20)     4794 2023-07-17 17:11:20.000000 error-tracker-3.1.0/error_tracker/django/middleware.py
+drwxr-xr-x   0 sonu       (501) staff       (20)        0 2023-07-17 17:15:33.321416 error-tracker-3.1.0/error_tracker/django/migrations/
+-rw-r--r--   0 sonu       (501) staff       (20)     1213 2023-07-17 16:11:51.000000 error-tracker-3.1.0/error_tracker/django/migrations/0001_initial.py
+-rw-r--r--   0 sonu       (501) staff       (20)      561 2023-07-17 16:11:51.000000 error-tracker-3.1.0/error_tracker/django/migrations/0002_auto_20201018_1311.py
+-rw-r--r--   0 sonu       (501) staff       (20)        0 2023-07-17 16:11:51.000000 error-tracker-3.1.0/error_tracker/django/migrations/__init__.py
+-rw-r--r--   0 sonu       (501) staff       (20)     3333 2023-07-17 17:11:20.000000 error-tracker-3.1.0/error_tracker/django/models.py
+-rw-r--r--   0 sonu       (501) staff       (20)     2264 2023-07-17 16:11:51.000000 error-tracker-3.1.0/error_tracker/django/settings.py
+drwxr-xr-x   0 sonu       (501) staff       (20)        0 2023-07-17 17:15:33.310409 error-tracker-3.1.0/error_tracker/django/templates/
+drwxr-xr-x   0 sonu       (501) staff       (20)        0 2023-07-17 17:15:33.322618 error-tracker-3.1.0/error_tracker/django/templates/error_tracker/
+drwxr-xr-x   0 sonu       (501) staff       (20)        0 2023-07-17 17:15:33.323029 error-tracker-3.1.0/error_tracker/django/templates/error_tracker/admin/
+-rw-r--r--   0 sonu       (501) staff       (20)      117 2023-07-17 16:11:51.000000 error-tracker-3.1.0/error_tracker/django/templates/error_tracker/admin/change_form.html
+-rwxr-xr-x   0 sonu       (501) staff       (20)     1428 2023-07-17 16:11:51.000000 error-tracker-3.1.0/error_tracker/django/templates/error_tracker/base.html
+-rwxr-xr-x   0 sonu       (501) staff       (20)     1984 2023-07-17 16:11:51.000000 error-tracker-3.1.0/error_tracker/django/templates/error_tracker/detail.html
+-rwxr-xr-x   0 sonu       (501) staff       (20)     4150 2023-07-17 16:11:51.000000 error-tracker-3.1.0/error_tracker/django/templates/error_tracker/list.html
+drwxr-xr-x   0 sonu       (501) staff       (20)        0 2023-07-17 17:15:33.323904 error-tracker-3.1.0/error_tracker/django/templates/error_tracker/partials/
+-rw-r--r--   0 sonu       (501) staff       (20)      546 2023-07-17 16:11:51.000000 error-tracker-3.1.0/error_tracker/django/templates/error_tracker/partials/navigation.html
+-rw-r--r--   0 sonu       (501) staff       (20)      725 2023-07-17 16:11:51.000000 error-tracker-3.1.0/error_tracker/django/templates/error_tracker/partials/partial_table.html
+drwxr-xr-x   0 sonu       (501) staff       (20)        0 2023-07-17 17:15:33.324725 error-tracker-3.1.0/error_tracker/django/templatetags/
+-rw-r--r--   0 sonu       (501) staff       (20)        0 2023-07-17 16:11:51.000000 error-tracker-3.1.0/error_tracker/django/templatetags/__init__.py
+-rw-r--r--   0 sonu       (501) staff       (20)      818 2023-07-17 16:11:51.000000 error-tracker-3.1.0/error_tracker/django/templatetags/error_tracker.py
+-rwxr-xr-x   0 sonu       (501) staff       (20)      421 2023-07-17 16:11:51.000000 error-tracker-3.1.0/error_tracker/django/urls.py
+-rw-r--r--   0 sonu       (501) staff       (20)     7648 2023-07-17 17:11:20.000000 error-tracker-3.1.0/error_tracker/django/utils.py
+-rw-r--r--   0 sonu       (501) staff       (20)     2911 2023-07-17 17:11:20.000000 error-tracker-3.1.0/error_tracker/django/views.py
+drwxr-xr-x   0 sonu       (501) staff       (20)        0 2023-07-17 17:15:33.326873 error-tracker-3.1.0/error_tracker/flask/
+-rwxr-xr-x   0 sonu       (501) staff       (20)      263 2023-07-17 16:11:51.000000 error-tracker-3.1.0/error_tracker/flask/__init__.py
+-rwxr-xr-x   0 sonu       (501) staff       (20)      864 2023-07-17 16:11:51.000000 error-tracker-3.1.0/error_tracker/flask/defaults.py
+-rwxr-xr-x   0 sonu       (501) staff       (20)    15094 2023-07-17 17:11:20.000000 error-tracker-3.1.0/error_tracker/flask/flask_error.py
+drwxr-xr-x   0 sonu       (501) staff       (20)        0 2023-07-17 17:15:33.311995 error-tracker-3.1.0/error_tracker/flask/templates/
+drwxr-xr-x   0 sonu       (501) staff       (20)        0 2023-07-17 17:15:33.328294 error-tracker-3.1.0/error_tracker/flask/templates/error_tracker/
+-rwxr-xr-x   0 sonu       (501) staff       (20)      538 2023-07-17 16:11:51.000000 error-tracker-3.1.0/error_tracker/flask/templates/error_tracker/base.html
+-rwxr-xr-x   0 sonu       (501) staff       (20)     1032 2023-07-17 16:11:51.000000 error-tracker-3.1.0/error_tracker/flask/templates/error_tracker/detail.html
+-rwxr-xr-x   0 sonu       (501) staff       (20)     2428 2023-07-17 16:11:51.000000 error-tracker-3.1.0/error_tracker/flask/templates/error_tracker/list.html
+-rw-r--r--   0 sonu       (501) staff       (20)     2436 2023-07-17 17:11:20.000000 error-tracker-3.1.0/error_tracker/flask/utils.py
+-rw-r--r--   0 sonu       (501) staff       (20)     2642 2023-07-17 17:11:20.000000 error-tracker-3.1.0/error_tracker/flask/view.py
+drwxr-xr-x   0 sonu       (501) staff       (20)        0 2023-07-17 17:15:33.330050 error-tracker-3.1.0/error_tracker/libs/
+-rw-r--r--   0 sonu       (501) staff       (20)        0 2023-07-17 16:11:51.000000 error-tracker-3.1.0/error_tracker/libs/__init__.py
+-rwxr-xr-x   0 sonu       (501) staff       (20)     6000 2023-07-17 17:11:20.000000 error-tracker-3.1.0/error_tracker/libs/exception_formatter.py
+-rwxr-xr-x   0 sonu       (501) staff       (20)     4817 2023-07-17 17:11:20.000000 error-tracker-3.1.0/error_tracker/libs/mixins.py
+-rw-r--r--   0 sonu       (501) staff       (20)     4976 2023-07-17 17:11:20.000000 error-tracker-3.1.0/error_tracker/libs/utils.py
+drwxr-xr-x   0 sonu       (501) staff       (20)        0 2023-07-17 17:15:33.316261 error-tracker-3.1.0/error_tracker.egg-info/
+-rw-r--r--   0 sonu       (501) staff       (20)     7047 2023-07-17 17:15:33.000000 error-tracker-3.1.0/error_tracker.egg-info/PKG-INFO
+-rw-r--r--   0 sonu       (501) staff       (20)     1655 2023-07-17 17:15:33.000000 error-tracker-3.1.0/error_tracker.egg-info/SOURCES.txt
+-rw-r--r--   0 sonu       (501) staff       (20)        1 2023-07-17 17:15:33.000000 error-tracker-3.1.0/error_tracker.egg-info/dependency_links.txt
+-rw-r--r--   0 sonu       (501) staff       (20)        1 2023-07-17 16:12:07.000000 error-tracker-3.1.0/error_tracker.egg-info/not-zip-safe
+-rw-r--r--   0 sonu       (501) staff       (20)       80 2023-07-17 17:15:33.000000 error-tracker-3.1.0/error_tracker.egg-info/requires.txt
+-rw-r--r--   0 sonu       (501) staff       (20)       14 2023-07-17 17:15:33.000000 error-tracker-3.1.0/error_tracker.egg-info/top_level.txt
+-rw-r--r--   0 sonu       (501) staff       (20)       80 2023-07-17 17:15:33.330965 error-tracker-3.1.0/setup.cfg
+-rwxr-xr-x   0 sonu       (501) staff       (20)     2165 2023-07-17 16:11:51.000000 error-tracker-3.1.0/setup.py
```

### Comparing `error-tracker-3.0.0/LICENSE.txt` & `error-tracker-3.1.0/LICENSE.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright 2019-2020 Sonu Kumar<sonunitw12@gmail.com>
+Copyright 2019-2023 Sonu Kumar<sonunitw12@gmail.com>
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are
 met:
 
 1.  Redistributions of source code must retain the above copyright
     notice, this list of conditions and the following disclaimer.
```

### Comparing `error-tracker-3.0.0/PKG-INFO` & `error-tracker-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: error-tracker
-Version: 3.0.0
+Version: 3.1.0
 Summary: Simple and Extensible Error Monitoring/Tracking framework for Python
 Home-page: https://github.com/sonus21/error-tracker/
 Author: Sonu Kumar
 Author-email: sonunitw12@gmail.com
 License: BSD-3-Clause
 Keywords: Flask,error-tracker,exception-tracking,exception-monitoring,Django
 Platform: any
@@ -223,9 +223,7 @@
 
     OK
 
 
 Contribution
 -------------
 You're most welcome to raise pull request or fixes.
-
-
```

### Comparing `error-tracker-3.0.0/README.rst` & `error-tracker-3.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `error-tracker-3.0.0/error_tracker/__init__.py` & `error-tracker-3.1.0/error_tracker/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
 #
 #    Error Tracking app
 #
-#    :copyright: 2020 Sonu Kumar
+#    :copyright: 2023 Sonu Kumar
 #    :license: BSD-3-Clause
 #
 
-__version__ = '3.0.0'
+__version__ = '3.1.0'
 __author__ = 'Sonu Kumar'
 __email__ = 'sonunitw12@gmail.com'
 
 from error_tracker.libs.mixins import *
 from error_tracker.libs.exception_formatter import *
 
 flaskInstalled = False
```

### Comparing `error-tracker-3.0.0/error_tracker/django/__init__.py` & `error-tracker-3.1.0/error_tracker/django/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 #    Django components
 #
-#    :copyright: 2020 Sonu Kumar
+#    :copyright: 2023 Sonu Kumar
 #    :license: BSD-3-Clause
 #
 
 
 from .utils import DefaultDjangoContextBuilder, DjangoNotification, DefaultDjangoViewPermission
 from .settings import *
```

### Comparing `error-tracker-3.0.0/error_tracker/django/admin.py` & `error-tracker-3.1.0/error_tracker/django/admin.py`

 * *Files identical despite different names*

### Comparing `error-tracker-3.0.0/error_tracker/django/middleware.py` & `error-tracker-3.1.0/error_tracker/django/middleware.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 #    Django error tracker middleware responsible for recording exception
 #
-#    :copyright: 2020 Sonu Kumar
+#    :copyright: 2023 Sonu Kumar
 #    :license: BSD-3-Clause
 #
 
 from error_tracker.django import get_masking_module, get_context_builder, get_ticketing_module, \
     get_exception_model, get_notification_module, APP_ERROR_SUBJECT_PREFIX, APP_ERROR_EMAIL_SENDER, \
     APP_ERROR_RECIPIENT_EMAIL, TRACK_ALL_EXCEPTIONS, APP_ERROR_NOTIFICATION_ONCE, \
     APP_ERROR_TICKET_ONCE
```

### Comparing `error-tracker-3.0.0/error_tracker/django/migrations/0001_initial.py` & `error-tracker-3.1.0/error_tracker/django/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `error-tracker-3.0.0/error_tracker/django/migrations/0002_auto_20201018_1311.py` & `error-tracker-3.1.0/error_tracker/django/migrations/0002_auto_20201018_1311.py`

 * *Files identical despite different names*

### Comparing `error-tracker-3.0.0/error_tracker/django/models.py` & `error-tracker-3.1.0/error_tracker/django/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 #    Django error tracker default model
 #
-#    :copyright: 2020 Sonu Kumar
+#    :copyright: 2023 Sonu Kumar
 #    :license: BSD-3-Clause
 #
 from django.core.paginator import Paginator, EmptyPage
 from django.db import models
 from error_tracker.libs.mixins import ModelMixin
 from django.utils.timezone import now
 from traceback import print_exc
```

### Comparing `error-tracker-3.0.0/error_tracker/django/settings.py` & `error-tracker-3.1.0/error_tracker/django/settings.py`

 * *Files identical despite different names*

### Comparing `error-tracker-3.0.0/error_tracker/django/templates/error_tracker/base.html` & `error-tracker-3.1.0/error_tracker/django/templates/error_tracker/base.html`

 * *Files identical despite different names*

### Comparing `error-tracker-3.0.0/error_tracker/django/templates/error_tracker/detail.html` & `error-tracker-3.1.0/error_tracker/django/templates/error_tracker/detail.html`

 * *Files identical despite different names*

### Comparing `error-tracker-3.0.0/error_tracker/django/templates/error_tracker/list.html` & `error-tracker-3.1.0/error_tracker/django/templates/error_tracker/list.html`

 * *Files identical despite different names*

### Comparing `error-tracker-3.0.0/error_tracker/django/templates/error_tracker/partials/navigation.html` & `error-tracker-3.1.0/error_tracker/django/templates/error_tracker/partials/navigation.html`

 * *Files identical despite different names*

### Comparing `error-tracker-3.0.0/error_tracker/django/templates/error_tracker/partials/partial_table.html` & `error-tracker-3.1.0/error_tracker/django/templates/error_tracker/partials/partial_table.html`

 * *Files identical despite different names*

### Comparing `error-tracker-3.0.0/error_tracker/django/templatetags/error_tracker.py` & `error-tracker-3.1.0/error_tracker/django/templatetags/error_tracker.py`

 * *Files identical despite different names*

### Comparing `error-tracker-3.0.0/error_tracker/django/utils.py` & `error-tracker-3.1.0/error_tracker/django/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 #    Django error tracker utils classes
 #
-#    :copyright: 2020 Sonu Kumar
+#    :copyright: 2023 Sonu Kumar
 #    :license: BSD-3-Clause
 #
 
 import json
 import re
 
 from error_tracker.libs.mixins import ContextBuilderMixin, NotificationMixin, ViewPermissionMixin
```

### Comparing `error-tracker-3.0.0/error_tracker/django/views.py` & `error-tracker-3.1.0/error_tracker/django/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 #    Django error tracker default value
 #
-#    :copyright: 2020 Sonu Kumar
+#    :copyright: 2023 Sonu Kumar
 #    :license: BSD-3-Clause
 #
 from django.http import Http404, HttpResponse, JsonResponse
 from django.shortcuts import redirect, render
 from django.urls import reverse
 from django.views.decorators.http import require_GET
 from error_tracker.django import get_exception_model, get_view_permission
```

### Comparing `error-tracker-3.0.0/error_tracker/flask/defaults.py` & `error-tracker-3.1.0/error_tracker/flask/defaults.py`

 * *Files identical despite different names*

### Comparing `error-tracker-3.0.0/error_tracker/flask/flask_error.py` & `error-tracker-3.1.0/error_tracker/flask/flask_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 #    Error tracker's flask plugin, this class initialize it's internal state
 #
-#    :copyright: 2020 Sonu Kumar
+#    :copyright: 2023 Sonu Kumar
 #    :license: BSD-3-Clause
 #
 
 
 from warnings import warn
 
 try:
```

### Comparing `error-tracker-3.0.0/error_tracker/flask/templates/error_tracker/base.html` & `error-tracker-3.1.0/error_tracker/flask/templates/error_tracker/base.html`

 * *Files identical despite different names*

### Comparing `error-tracker-3.0.0/error_tracker/flask/templates/error_tracker/detail.html` & `error-tracker-3.1.0/error_tracker/flask/templates/error_tracker/detail.html`

 * *Files identical despite different names*

### Comparing `error-tracker-3.0.0/error_tracker/flask/templates/error_tracker/list.html` & `error-tracker-3.1.0/error_tracker/flask/templates/error_tracker/list.html`

 * *Files identical despite different names*

### Comparing `error-tracker-3.0.0/error_tracker/flask/utils.py` & `error-tracker-3.1.0/error_tracker/flask/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #     Utils modules for flask plugin
 #
-#     :copyright: 2020 Sonu Kumar
+#     :copyright: 2023 Sonu Kumar
 #     :license: BSD-3-Clause
 #
 from error_tracker import ContextBuilderMixin, ViewPermissionMixin
 
 
 class DefaultFlaskContextBuilder(ContextBuilderMixin):
     """
```

### Comparing `error-tracker-3.0.0/error_tracker/flask/view.py` & `error-tracker-3.1.0/error_tracker/flask/view.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #     Exception formatter defaults view for flask app
 #
-#     :copyright: 2020 Sonu Kumar
+#     :copyright: 2023 Sonu Kumar
 #     :license: BSD-3-Clause
 #
 
 import os
 
 from flask import url_for, render_template, abort, redirect, request, blueprints
```

### Comparing `error-tracker-3.0.0/error_tracker/libs/exception_formatter.py` & `error-tracker-3.1.0/error_tracker/libs/exception_formatter.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 #    Exception formatter that captures frame details in string format.
 #
-#    :copyright: 2020 Sonu Kumar
+#    :copyright: 2023 Sonu Kumar
 #    :license: BSD-3-Clause
 #
 
 import six
 import itertools
 import sys
 import traceback
@@ -33,15 +33,15 @@
         pass
     try:
         from django.http import QueryDict
         if type(x) == QueryDict:
             return "QueryDict({%s})", x.dict()
     except ImportError:
         pass
-    return None, None
+    return None, x
 
 
 def format_frame(x, max_elements, max_string, max_recursion, masking=None):
     """
     Return a formatted frame for storing in the database.
     :param x: frame key/value pair
     :param max_elements: Maximum number of elements to be formatted
@@ -164,16 +164,17 @@
             masked = False
             if masking:
                 masked, val = masking(key)
                 if masked:
                     w(val)
             if not masked:
                 try:
-                    w(format_frame(value, max_elements, max_string, max_recursion,
-                                   masking=masking))
+                    formatted_val = format_frame(value, max_elements, max_string, max_recursion,
+                                   masking=masking)
+                    w(formatted_val)
                 except Exception:
                     exc_class = sys.exc_info()[0]
                     w("<%s raised while printing value>" % exc_class)
             w("\n")
     w("\n")
     w(''.join(traceback.format_tb(tb)))
     op = buf.getvalue()
```

### Comparing `error-tracker-3.0.0/error_tracker/libs/mixins.py` & `error-tracker-3.1.0/error_tracker/libs/mixins.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 #    Exception formatter mixin classes
 #
-#    :copyright: 2020 Sonu Kumar
+#    :copyright: 2023 Sonu Kumar
 #    :license: BSD-3-Clause
 #
 
 import abc
 
 
 class MaskingMixin(object):
```

### Comparing `error-tracker-3.0.0/error_tracker/libs/utils.py` & `error-tracker-3.1.0/error_tracker/libs/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 #     Exception formatter utils module
 #
-#     :copyright: 2020 Sonu Kumar
+#     :copyright: 2023 Sonu Kumar
 #     :license: BSD-3-Clause
 #
 import sys
 import traceback
 import warnings
 from hashlib import sha256
 import six
```

### Comparing `error-tracker-3.0.0/error_tracker.egg-info/PKG-INFO` & `error-tracker-3.1.0/error_tracker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: error-tracker
-Version: 3.0.0
+Version: 3.1.0
 Summary: Simple and Extensible Error Monitoring/Tracking framework for Python
 Home-page: https://github.com/sonus21/error-tracker/
 Author: Sonu Kumar
 Author-email: sonunitw12@gmail.com
 License: BSD-3-Clause
 Keywords: Flask,error-tracker,exception-tracking,exception-monitoring,Django
 Platform: any
@@ -223,9 +223,7 @@
 
     OK
 
 
 Contribution
 -------------
 You're most welcome to raise pull request or fixes.
-
-
```

### Comparing `error-tracker-3.0.0/error_tracker.egg-info/SOURCES.txt` & `error-tracker-3.1.0/error_tracker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `error-tracker-3.0.0/setup.py` & `error-tracker-3.1.0/setup.py`

 * *Files identical despite different names*

