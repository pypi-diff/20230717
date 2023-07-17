# Comparing `tmp/error-tracker-3.1.0.tar.gz` & `tmp/error-tracker-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "error-tracker-3.1.0.tar", last modified: Mon Jul 17 17:15:33 2023, max compression
+gzip compressed data, was "error-tracker-3.1.1.tar", last modified: Mon Jul 17 17:52:02 2023, max compression
```

## Comparing `error-tracker-3.1.0.tar` & `error-tracker-3.1.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 sonu       (501) staff       (20)        0 2023-07-17 17:15:33.330353 error-tracker-3.1.0/
--rw-r--r--   0 sonu       (501) staff       (20)     1504 2023-07-17 17:13:34.000000 error-tracker-3.1.0/LICENSE.txt
--rwxr-xr-x   0 sonu       (501) staff       (20)      112 2023-07-17 16:11:51.000000 error-tracker-3.1.0/MANIFEST.in
--rw-r--r--   0 sonu       (501) staff       (20)     7047 2023-07-17 17:15:33.330490 error-tracker-3.1.0/PKG-INFO
--rw-r--r--   0 sonu       (501) staff       (20)     5787 2023-07-17 16:11:51.000000 error-tracker-3.1.0/README.rst
-drwxr-xr-x   0 sonu       (501) staff       (20)        0 2023-07-17 17:15:33.314295 error-tracker-3.1.0/error_tracker/
--rw-r--r--   0 sonu       (501) staff       (20)     1377 2023-07-17 17:11:20.000000 error-tracker-3.1.0/error_tracker/__init__.py
-drwxr-xr-x   0 sonu       (501) staff       (20)        0 2023-07-17 17:15:33.320177 error-tracker-3.1.0/error_tracker/django/
--rw-r--r--   0 sonu       (501) staff       (20)     2741 2023-07-17 17:11:20.000000 error-tracker-3.1.0/error_tracker/django/__init__.py
--rw-r--r--   0 sonu       (501) staff       (20)     1291 2023-07-17 16:11:51.000000 error-tracker-3.1.0/error_tracker/django/admin.py
--rw-r--r--   0 sonu       (501) staff       (20)      384 2023-07-17 16:11:51.000000 error-tracker-3.1.0/error_tracker/django/apps.py
--rw-r--r--   0 sonu       (501) staff       (20)     4794 2023-07-17 17:11:20.000000 error-tracker-3.1.0/error_tracker/django/middleware.py
-drwxr-xr-x   0 sonu       (501) staff       (20)        0 2023-07-17 17:15:33.321416 error-tracker-3.1.0/error_tracker/django/migrations/
--rw-r--r--   0 sonu       (501) staff       (20)     1213 2023-07-17 16:11:51.000000 error-tracker-3.1.0/error_tracker/django/migrations/0001_initial.py
--rw-r--r--   0 sonu       (501) staff       (20)      561 2023-07-17 16:11:51.000000 error-tracker-3.1.0/error_tracker/django/migrations/0002_auto_20201018_1311.py
--rw-r--r--   0 sonu       (501) staff       (20)        0 2023-07-17 16:11:51.000000 error-tracker-3.1.0/error_tracker/django/migrations/__init__.py
--rw-r--r--   0 sonu       (501) staff       (20)     3333 2023-07-17 17:11:20.000000 error-tracker-3.1.0/error_tracker/django/models.py
--rw-r--r--   0 sonu       (501) staff       (20)     2264 2023-07-17 16:11:51.000000 error-tracker-3.1.0/error_tracker/django/settings.py
-drwxr-xr-x   0 sonu       (501) staff       (20)        0 2023-07-17 17:15:33.310409 error-tracker-3.1.0/error_tracker/django/templates/
-drwxr-xr-x   0 sonu       (501) staff       (20)        0 2023-07-17 17:15:33.322618 error-tracker-3.1.0/error_tracker/django/templates/error_tracker/
-drwxr-xr-x   0 sonu       (501) staff       (20)        0 2023-07-17 17:15:33.323029 error-tracker-3.1.0/error_tracker/django/templates/error_tracker/admin/
--rw-r--r--   0 sonu       (501) staff       (20)      117 2023-07-17 16:11:51.000000 error-tracker-3.1.0/error_tracker/django/templates/error_tracker/admin/change_form.html
--rwxr-xr-x   0 sonu       (501) staff       (20)     1428 2023-07-17 16:11:51.000000 error-tracker-3.1.0/error_tracker/django/templates/error_tracker/base.html
--rwxr-xr-x   0 sonu       (501) staff       (20)     1984 2023-07-17 16:11:51.000000 error-tracker-3.1.0/error_tracker/django/templates/error_tracker/detail.html
--rwxr-xr-x   0 sonu       (501) staff       (20)     4150 2023-07-17 16:11:51.000000 error-tracker-3.1.0/error_tracker/django/templates/error_tracker/list.html
-drwxr-xr-x   0 sonu       (501) staff       (20)        0 2023-07-17 17:15:33.323904 error-tracker-3.1.0/error_tracker/django/templates/error_tracker/partials/
--rw-r--r--   0 sonu       (501) staff       (20)      546 2023-07-17 16:11:51.000000 error-tracker-3.1.0/error_tracker/django/templates/error_tracker/partials/navigation.html
--rw-r--r--   0 sonu       (501) staff       (20)      725 2023-07-17 16:11:51.000000 error-tracker-3.1.0/error_tracker/django/templates/error_tracker/partials/partial_table.html
-drwxr-xr-x   0 sonu       (501) staff       (20)        0 2023-07-17 17:15:33.324725 error-tracker-3.1.0/error_tracker/django/templatetags/
--rw-r--r--   0 sonu       (501) staff       (20)        0 2023-07-17 16:11:51.000000 error-tracker-3.1.0/error_tracker/django/templatetags/__init__.py
--rw-r--r--   0 sonu       (501) staff       (20)      818 2023-07-17 16:11:51.000000 error-tracker-3.1.0/error_tracker/django/templatetags/error_tracker.py
--rwxr-xr-x   0 sonu       (501) staff       (20)      421 2023-07-17 16:11:51.000000 error-tracker-3.1.0/error_tracker/django/urls.py
--rw-r--r--   0 sonu       (501) staff       (20)     7648 2023-07-17 17:11:20.000000 error-tracker-3.1.0/error_tracker/django/utils.py
--rw-r--r--   0 sonu       (501) staff       (20)     2911 2023-07-17 17:11:20.000000 error-tracker-3.1.0/error_tracker/django/views.py
-drwxr-xr-x   0 sonu       (501) staff       (20)        0 2023-07-17 17:15:33.326873 error-tracker-3.1.0/error_tracker/flask/
--rwxr-xr-x   0 sonu       (501) staff       (20)      263 2023-07-17 16:11:51.000000 error-tracker-3.1.0/error_tracker/flask/__init__.py
--rwxr-xr-x   0 sonu       (501) staff       (20)      864 2023-07-17 16:11:51.000000 error-tracker-3.1.0/error_tracker/flask/defaults.py
--rwxr-xr-x   0 sonu       (501) staff       (20)    15094 2023-07-17 17:11:20.000000 error-tracker-3.1.0/error_tracker/flask/flask_error.py
-drwxr-xr-x   0 sonu       (501) staff       (20)        0 2023-07-17 17:15:33.311995 error-tracker-3.1.0/error_tracker/flask/templates/
-drwxr-xr-x   0 sonu       (501) staff       (20)        0 2023-07-17 17:15:33.328294 error-tracker-3.1.0/error_tracker/flask/templates/error_tracker/
--rwxr-xr-x   0 sonu       (501) staff       (20)      538 2023-07-17 16:11:51.000000 error-tracker-3.1.0/error_tracker/flask/templates/error_tracker/base.html
--rwxr-xr-x   0 sonu       (501) staff       (20)     1032 2023-07-17 16:11:51.000000 error-tracker-3.1.0/error_tracker/flask/templates/error_tracker/detail.html
--rwxr-xr-x   0 sonu       (501) staff       (20)     2428 2023-07-17 16:11:51.000000 error-tracker-3.1.0/error_tracker/flask/templates/error_tracker/list.html
--rw-r--r--   0 sonu       (501) staff       (20)     2436 2023-07-17 17:11:20.000000 error-tracker-3.1.0/error_tracker/flask/utils.py
--rw-r--r--   0 sonu       (501) staff       (20)     2642 2023-07-17 17:11:20.000000 error-tracker-3.1.0/error_tracker/flask/view.py
-drwxr-xr-x   0 sonu       (501) staff       (20)        0 2023-07-17 17:15:33.330050 error-tracker-3.1.0/error_tracker/libs/
--rw-r--r--   0 sonu       (501) staff       (20)        0 2023-07-17 16:11:51.000000 error-tracker-3.1.0/error_tracker/libs/__init__.py
--rwxr-xr-x   0 sonu       (501) staff       (20)     6000 2023-07-17 17:11:20.000000 error-tracker-3.1.0/error_tracker/libs/exception_formatter.py
--rwxr-xr-x   0 sonu       (501) staff       (20)     4817 2023-07-17 17:11:20.000000 error-tracker-3.1.0/error_tracker/libs/mixins.py
--rw-r--r--   0 sonu       (501) staff       (20)     4976 2023-07-17 17:11:20.000000 error-tracker-3.1.0/error_tracker/libs/utils.py
-drwxr-xr-x   0 sonu       (501) staff       (20)        0 2023-07-17 17:15:33.316261 error-tracker-3.1.0/error_tracker.egg-info/
--rw-r--r--   0 sonu       (501) staff       (20)     7047 2023-07-17 17:15:33.000000 error-tracker-3.1.0/error_tracker.egg-info/PKG-INFO
--rw-r--r--   0 sonu       (501) staff       (20)     1655 2023-07-17 17:15:33.000000 error-tracker-3.1.0/error_tracker.egg-info/SOURCES.txt
--rw-r--r--   0 sonu       (501) staff       (20)        1 2023-07-17 17:15:33.000000 error-tracker-3.1.0/error_tracker.egg-info/dependency_links.txt
--rw-r--r--   0 sonu       (501) staff       (20)        1 2023-07-17 16:12:07.000000 error-tracker-3.1.0/error_tracker.egg-info/not-zip-safe
--rw-r--r--   0 sonu       (501) staff       (20)       80 2023-07-17 17:15:33.000000 error-tracker-3.1.0/error_tracker.egg-info/requires.txt
--rw-r--r--   0 sonu       (501) staff       (20)       14 2023-07-17 17:15:33.000000 error-tracker-3.1.0/error_tracker.egg-info/top_level.txt
--rw-r--r--   0 sonu       (501) staff       (20)       80 2023-07-17 17:15:33.330965 error-tracker-3.1.0/setup.cfg
--rwxr-xr-x   0 sonu       (501) staff       (20)     2165 2023-07-17 16:11:51.000000 error-tracker-3.1.0/setup.py
+drwxr-xr-x   0 sonu       (501) staff       (20)        0 2023-07-17 17:52:02.499821 error-tracker-3.1.1/
+-rw-r--r--   0 sonu       (501) staff       (20)     1504 2023-07-17 17:13:34.000000 error-tracker-3.1.1/LICENSE.txt
+-rwxr-xr-x   0 sonu       (501) staff       (20)      112 2023-07-17 16:11:51.000000 error-tracker-3.1.1/MANIFEST.in
+-rw-r--r--   0 sonu       (501) staff       (20)     7047 2023-07-17 17:52:02.499930 error-tracker-3.1.1/PKG-INFO
+-rw-r--r--   0 sonu       (501) staff       (20)     5787 2023-07-17 16:11:51.000000 error-tracker-3.1.1/README.rst
+drwxr-xr-x   0 sonu       (501) staff       (20)        0 2023-07-17 17:52:02.476387 error-tracker-3.1.1/error_tracker/
+-rw-r--r--   0 sonu       (501) staff       (20)     1377 2023-07-17 17:51:36.000000 error-tracker-3.1.1/error_tracker/__init__.py
+drwxr-xr-x   0 sonu       (501) staff       (20)        0 2023-07-17 17:52:02.489998 error-tracker-3.1.1/error_tracker/django/
+-rw-r--r--   0 sonu       (501) staff       (20)     2741 2023-07-17 17:11:20.000000 error-tracker-3.1.1/error_tracker/django/__init__.py
+-rw-r--r--   0 sonu       (501) staff       (20)     1291 2023-07-17 16:11:51.000000 error-tracker-3.1.1/error_tracker/django/admin.py
+-rw-r--r--   0 sonu       (501) staff       (20)      384 2023-07-17 16:11:51.000000 error-tracker-3.1.1/error_tracker/django/apps.py
+-rw-r--r--   0 sonu       (501) staff       (20)     4794 2023-07-17 17:11:20.000000 error-tracker-3.1.1/error_tracker/django/middleware.py
+drwxr-xr-x   0 sonu       (501) staff       (20)        0 2023-07-17 17:52:02.491930 error-tracker-3.1.1/error_tracker/django/migrations/
+-rw-r--r--   0 sonu       (501) staff       (20)     1213 2023-07-17 16:11:51.000000 error-tracker-3.1.1/error_tracker/django/migrations/0001_initial.py
+-rw-r--r--   0 sonu       (501) staff       (20)      561 2023-07-17 16:11:51.000000 error-tracker-3.1.1/error_tracker/django/migrations/0002_auto_20201018_1311.py
+-rw-r--r--   0 sonu       (501) staff       (20)        0 2023-07-17 16:11:51.000000 error-tracker-3.1.1/error_tracker/django/migrations/__init__.py
+-rw-r--r--   0 sonu       (501) staff       (20)     3333 2023-07-17 17:11:20.000000 error-tracker-3.1.1/error_tracker/django/models.py
+-rw-r--r--   0 sonu       (501) staff       (20)     2264 2023-07-17 16:11:51.000000 error-tracker-3.1.1/error_tracker/django/settings.py
+drwxr-xr-x   0 sonu       (501) staff       (20)        0 2023-07-17 17:52:02.471018 error-tracker-3.1.1/error_tracker/django/templates/
+drwxr-xr-x   0 sonu       (501) staff       (20)        0 2023-07-17 17:52:02.493060 error-tracker-3.1.1/error_tracker/django/templates/error_tracker/
+drwxr-xr-x   0 sonu       (501) staff       (20)        0 2023-07-17 17:52:02.493452 error-tracker-3.1.1/error_tracker/django/templates/error_tracker/admin/
+-rw-r--r--   0 sonu       (501) staff       (20)      117 2023-07-17 16:11:51.000000 error-tracker-3.1.1/error_tracker/django/templates/error_tracker/admin/change_form.html
+-rwxr-xr-x   0 sonu       (501) staff       (20)     1428 2023-07-17 16:11:51.000000 error-tracker-3.1.1/error_tracker/django/templates/error_tracker/base.html
+-rwxr-xr-x   0 sonu       (501) staff       (20)     1984 2023-07-17 16:11:51.000000 error-tracker-3.1.1/error_tracker/django/templates/error_tracker/detail.html
+-rwxr-xr-x   0 sonu       (501) staff       (20)     4150 2023-07-17 16:11:51.000000 error-tracker-3.1.1/error_tracker/django/templates/error_tracker/list.html
+drwxr-xr-x   0 sonu       (501) staff       (20)        0 2023-07-17 17:52:02.494216 error-tracker-3.1.1/error_tracker/django/templates/error_tracker/partials/
+-rw-r--r--   0 sonu       (501) staff       (20)      546 2023-07-17 16:11:51.000000 error-tracker-3.1.1/error_tracker/django/templates/error_tracker/partials/navigation.html
+-rw-r--r--   0 sonu       (501) staff       (20)      725 2023-07-17 16:11:51.000000 error-tracker-3.1.1/error_tracker/django/templates/error_tracker/partials/partial_table.html
+drwxr-xr-x   0 sonu       (501) staff       (20)        0 2023-07-17 17:52:02.494857 error-tracker-3.1.1/error_tracker/django/templatetags/
+-rw-r--r--   0 sonu       (501) staff       (20)        0 2023-07-17 16:11:51.000000 error-tracker-3.1.1/error_tracker/django/templatetags/__init__.py
+-rw-r--r--   0 sonu       (501) staff       (20)      818 2023-07-17 16:11:51.000000 error-tracker-3.1.1/error_tracker/django/templatetags/error_tracker.py
+-rwxr-xr-x   0 sonu       (501) staff       (20)      421 2023-07-17 16:11:51.000000 error-tracker-3.1.1/error_tracker/django/urls.py
+-rw-r--r--   0 sonu       (501) staff       (20)     7648 2023-07-17 17:11:20.000000 error-tracker-3.1.1/error_tracker/django/utils.py
+-rw-r--r--   0 sonu       (501) staff       (20)     2911 2023-07-17 17:11:20.000000 error-tracker-3.1.1/error_tracker/django/views.py
+drwxr-xr-x   0 sonu       (501) staff       (20)        0 2023-07-17 17:52:02.496735 error-tracker-3.1.1/error_tracker/flask/
+-rwxr-xr-x   0 sonu       (501) staff       (20)      263 2023-07-17 16:11:51.000000 error-tracker-3.1.1/error_tracker/flask/__init__.py
+-rwxr-xr-x   0 sonu       (501) staff       (20)      864 2023-07-17 16:11:51.000000 error-tracker-3.1.1/error_tracker/flask/defaults.py
+-rwxr-xr-x   0 sonu       (501) staff       (20)    15355 2023-07-17 17:50:27.000000 error-tracker-3.1.1/error_tracker/flask/flask_error.py
+drwxr-xr-x   0 sonu       (501) staff       (20)        0 2023-07-17 17:52:02.473056 error-tracker-3.1.1/error_tracker/flask/templates/
+drwxr-xr-x   0 sonu       (501) staff       (20)        0 2023-07-17 17:52:02.497811 error-tracker-3.1.1/error_tracker/flask/templates/error_tracker/
+-rwxr-xr-x   0 sonu       (501) staff       (20)      538 2023-07-17 16:11:51.000000 error-tracker-3.1.1/error_tracker/flask/templates/error_tracker/base.html
+-rwxr-xr-x   0 sonu       (501) staff       (20)     1032 2023-07-17 16:11:51.000000 error-tracker-3.1.1/error_tracker/flask/templates/error_tracker/detail.html
+-rwxr-xr-x   0 sonu       (501) staff       (20)     2428 2023-07-17 16:11:51.000000 error-tracker-3.1.1/error_tracker/flask/templates/error_tracker/list.html
+-rw-r--r--   0 sonu       (501) staff       (20)     2436 2023-07-17 17:11:20.000000 error-tracker-3.1.1/error_tracker/flask/utils.py
+-rw-r--r--   0 sonu       (501) staff       (20)     2642 2023-07-17 17:11:20.000000 error-tracker-3.1.1/error_tracker/flask/view.py
+drwxr-xr-x   0 sonu       (501) staff       (20)        0 2023-07-17 17:52:02.499413 error-tracker-3.1.1/error_tracker/libs/
+-rw-r--r--   0 sonu       (501) staff       (20)        0 2023-07-17 16:11:51.000000 error-tracker-3.1.1/error_tracker/libs/__init__.py
+-rwxr-xr-x   0 sonu       (501) staff       (20)     6000 2023-07-17 17:11:20.000000 error-tracker-3.1.1/error_tracker/libs/exception_formatter.py
+-rwxr-xr-x   0 sonu       (501) staff       (20)     4817 2023-07-17 17:11:20.000000 error-tracker-3.1.1/error_tracker/libs/mixins.py
+-rw-r--r--   0 sonu       (501) staff       (20)     4976 2023-07-17 17:11:20.000000 error-tracker-3.1.1/error_tracker/libs/utils.py
+drwxr-xr-x   0 sonu       (501) staff       (20)        0 2023-07-17 17:52:02.479471 error-tracker-3.1.1/error_tracker.egg-info/
+-rw-r--r--   0 sonu       (501) staff       (20)     7047 2023-07-17 17:52:02.000000 error-tracker-3.1.1/error_tracker.egg-info/PKG-INFO
+-rw-r--r--   0 sonu       (501) staff       (20)     1655 2023-07-17 17:52:02.000000 error-tracker-3.1.1/error_tracker.egg-info/SOURCES.txt
+-rw-r--r--   0 sonu       (501) staff       (20)        1 2023-07-17 17:52:02.000000 error-tracker-3.1.1/error_tracker.egg-info/dependency_links.txt
+-rw-r--r--   0 sonu       (501) staff       (20)        1 2023-07-17 17:52:02.000000 error-tracker-3.1.1/error_tracker.egg-info/not-zip-safe
+-rw-r--r--   0 sonu       (501) staff       (20)       80 2023-07-17 17:52:02.000000 error-tracker-3.1.1/error_tracker.egg-info/requires.txt
+-rw-r--r--   0 sonu       (501) staff       (20)       14 2023-07-17 17:52:02.000000 error-tracker-3.1.1/error_tracker.egg-info/top_level.txt
+-rw-r--r--   0 sonu       (501) staff       (20)       80 2023-07-17 17:52:02.500404 error-tracker-3.1.1/setup.cfg
+-rwxr-xr-x   0 sonu       (501) staff       (20)     2165 2023-07-17 16:11:51.000000 error-tracker-3.1.1/setup.py
```

### Comparing `error-tracker-3.1.0/LICENSE.txt` & `error-tracker-3.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `error-tracker-3.1.0/PKG-INFO` & `error-tracker-3.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: error-tracker
-Version: 3.1.0
+Version: 3.1.1
 Summary: Simple and Extensible Error Monitoring/Tracking framework for Python
 Home-page: https://github.com/sonus21/error-tracker/
 Author: Sonu Kumar
 Author-email: sonunitw12@gmail.com
 License: BSD-3-Clause
 Keywords: Flask,error-tracker,exception-tracking,exception-monitoring,Django
 Platform: any
```

### Comparing `error-tracker-3.1.0/README.rst` & `error-tracker-3.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `error-tracker-3.1.0/error_tracker/__init__.py` & `error-tracker-3.1.1/error_tracker/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 #    Error Tracking app
 #
 #    :copyright: 2023 Sonu Kumar
 #    :license: BSD-3-Clause
 #
 
-__version__ = '3.1.0'
+__version__ = '3.1.1'
 __author__ = 'Sonu Kumar'
 __email__ = 'sonunitw12@gmail.com'
 
 from error_tracker.libs.mixins import *
 from error_tracker.libs.exception_formatter import *
 
 flaskInstalled = False
```

### Comparing `error-tracker-3.1.0/error_tracker/django/__init__.py` & `error-tracker-3.1.1/error_tracker/django/__init__.py`

 * *Files identical despite different names*

### Comparing `error-tracker-3.1.0/error_tracker/django/admin.py` & `error-tracker-3.1.1/error_tracker/django/admin.py`

 * *Files identical despite different names*

### Comparing `error-tracker-3.1.0/error_tracker/django/middleware.py` & `error-tracker-3.1.1/error_tracker/django/middleware.py`

 * *Files identical despite different names*

### Comparing `error-tracker-3.1.0/error_tracker/django/migrations/0001_initial.py` & `error-tracker-3.1.1/error_tracker/django/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `error-tracker-3.1.0/error_tracker/django/migrations/0002_auto_20201018_1311.py` & `error-tracker-3.1.1/error_tracker/django/migrations/0002_auto_20201018_1311.py`

 * *Files identical despite different names*

### Comparing `error-tracker-3.1.0/error_tracker/django/models.py` & `error-tracker-3.1.1/error_tracker/django/models.py`

 * *Files identical despite different names*

### Comparing `error-tracker-3.1.0/error_tracker/django/settings.py` & `error-tracker-3.1.1/error_tracker/django/settings.py`

 * *Files identical despite different names*

### Comparing `error-tracker-3.1.0/error_tracker/django/templates/error_tracker/base.html` & `error-tracker-3.1.1/error_tracker/django/templates/error_tracker/base.html`

 * *Files identical despite different names*

### Comparing `error-tracker-3.1.0/error_tracker/django/templates/error_tracker/detail.html` & `error-tracker-3.1.1/error_tracker/django/templates/error_tracker/detail.html`

 * *Files identical despite different names*

### Comparing `error-tracker-3.1.0/error_tracker/django/templates/error_tracker/list.html` & `error-tracker-3.1.1/error_tracker/django/templates/error_tracker/list.html`

 * *Files identical despite different names*

### Comparing `error-tracker-3.1.0/error_tracker/django/templates/error_tracker/partials/navigation.html` & `error-tracker-3.1.1/error_tracker/django/templates/error_tracker/partials/navigation.html`

 * *Files identical despite different names*

### Comparing `error-tracker-3.1.0/error_tracker/django/templates/error_tracker/partials/partial_table.html` & `error-tracker-3.1.1/error_tracker/django/templates/error_tracker/partials/partial_table.html`

 * *Files identical despite different names*

### Comparing `error-tracker-3.1.0/error_tracker/django/templatetags/error_tracker.py` & `error-tracker-3.1.1/error_tracker/django/templatetags/error_tracker.py`

 * *Files identical despite different names*

### Comparing `error-tracker-3.1.0/error_tracker/django/utils.py` & `error-tracker-3.1.1/error_tracker/django/utils.py`

 * *Files identical despite different names*

### Comparing `error-tracker-3.1.0/error_tracker/django/views.py` & `error-tracker-3.1.1/error_tracker/django/views.py`

 * *Files identical despite different names*

### Comparing `error-tracker-3.1.0/error_tracker/flask/defaults.py` & `error-tracker-3.1.1/error_tracker/flask/defaults.py`

 * *Files identical despite different names*

### Comparing `error-tracker-3.1.0/error_tracker/flask/flask_error.py` & `error-tracker-3.1.1/error_tracker/flask/flask_error.py`

 * *Files 3% similar despite different names*

```diff
@@ -211,15 +211,15 @@
                     cls.db.session.add(error)
                     cls.db.session.commit()
                 return error
 
             @classmethod
             def get_exceptions_per_page(cls, page_number=1):
                 return cls.query.order_by(desc(cls.last_seen)).paginate(
-                    page_number, page_size, False)
+                    page=page_number, per_page=page_size, error_out=False)
 
             @classmethod
             def get_entity(cls, rhash):
                 """
                 :param rhash: key for lookup
                 :return: Single entry of this class
                 """
@@ -281,18 +281,19 @@
             rq = None
             path = ""
             host = ""
             method = ""
 
         ty, frames, frame_str, traceback_str, rhash, request_data = \
             get_context_detail(rq, self.masking, self.context_builder, additional_context)
-        error = self.model.create_or_update_entity(rhash, host, path, method,
-                                                   str(request_data),
-                                                   get_exception_name(ty),
-                                                   traceback_str)
+        with self.app.app_context():
+            error = self.model.create_or_update_entity(rhash, host, path, method,
+                                                       str(request_data),
+                                                       get_exception_name(ty),
+                                                       traceback_str)
         self._post_process(rq, frame_str, frames, error)
 
     def auto_track_exception(self, func, additional_context=None, silent=False):
         """
         Decorator to be used for automatic exception capture, where exception can occur
         :param func:
         :param additional_context:  any additional context
@@ -325,36 +326,40 @@
     def get_exceptions(self, page_number=1):
         """
         Get list of exception objects from persistence store
         :param page_number: documents of a specific page
         :return: list of exception objects
         """
         if self.model:
-            return self.model.get_exceptions_per_page(page_number=page_number).items
+            with self.app.app_context():
+                return self.model.get_exceptions_per_page(page_number=page_number).items
         raise ConfigError
 
     def get_exception(self, rhash):
         """
         Get a specific exception, can be used for some customization etc
         :param rhash:  hash of the exception
         :return:  exception object
         """
         if self.model:
-            return self.model.get_entity(rhash)
+            with self.app.app_context():
+                return self.model.get_entity(rhash)
         raise ConfigError
 
     def delete_exception(self, rhash):
         """
         Delete a specific exception from database
         :param rhash: hash of the exception
         :return:   whatever model returns
         """
         if self.model:
-            return self.model.delete_entity(rhash)
+            with self.app.app_context():
+                return self.model.delete_entity(rhash)
         raise ConfigError
 
     def create_or_update_exception(self, rhash, host, path, method, request_data,
                                    exception_name, traceback):
         if self.model:
-            return self.model.create_or_update_entity(rhash, host, path, method, request_data,
-                                                      exception_name, traceback)
+            with self.app.app_context():
+                return self.model.create_or_update_entity(rhash, host, path, method, request_data,
+                                                          exception_name, traceback)
         raise ConfigError
```

### Comparing `error-tracker-3.1.0/error_tracker/flask/templates/error_tracker/base.html` & `error-tracker-3.1.1/error_tracker/flask/templates/error_tracker/base.html`

 * *Files identical despite different names*

### Comparing `error-tracker-3.1.0/error_tracker/flask/templates/error_tracker/detail.html` & `error-tracker-3.1.1/error_tracker/flask/templates/error_tracker/detail.html`

 * *Files identical despite different names*

### Comparing `error-tracker-3.1.0/error_tracker/flask/templates/error_tracker/list.html` & `error-tracker-3.1.1/error_tracker/flask/templates/error_tracker/list.html`

 * *Files identical despite different names*

### Comparing `error-tracker-3.1.0/error_tracker/flask/utils.py` & `error-tracker-3.1.1/error_tracker/flask/utils.py`

 * *Files identical despite different names*

### Comparing `error-tracker-3.1.0/error_tracker/flask/view.py` & `error-tracker-3.1.1/error_tracker/flask/view.py`

 * *Files identical despite different names*

### Comparing `error-tracker-3.1.0/error_tracker/libs/exception_formatter.py` & `error-tracker-3.1.1/error_tracker/libs/exception_formatter.py`

 * *Files identical despite different names*

### Comparing `error-tracker-3.1.0/error_tracker/libs/mixins.py` & `error-tracker-3.1.1/error_tracker/libs/mixins.py`

 * *Files identical despite different names*

### Comparing `error-tracker-3.1.0/error_tracker/libs/utils.py` & `error-tracker-3.1.1/error_tracker/libs/utils.py`

 * *Files identical despite different names*

### Comparing `error-tracker-3.1.0/error_tracker.egg-info/PKG-INFO` & `error-tracker-3.1.1/error_tracker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: error-tracker
-Version: 3.1.0
+Version: 3.1.1
 Summary: Simple and Extensible Error Monitoring/Tracking framework for Python
 Home-page: https://github.com/sonus21/error-tracker/
 Author: Sonu Kumar
 Author-email: sonunitw12@gmail.com
 License: BSD-3-Clause
 Keywords: Flask,error-tracker,exception-tracking,exception-monitoring,Django
 Platform: any
```

### Comparing `error-tracker-3.1.0/error_tracker.egg-info/SOURCES.txt` & `error-tracker-3.1.1/error_tracker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `error-tracker-3.1.0/setup.py` & `error-tracker-3.1.1/setup.py`

 * *Files identical despite different names*

