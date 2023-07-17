# Comparing `tmp/django_celery_tracker-2.0.0.tar.gz` & `tmp/django_celery_tracker-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_celery_tracker-2.0.0.tar", last modified: Fri Jun  3 14:04:03 2022, max compression
+gzip compressed data, was "django_celery_tracker-2.1.0.tar", last modified: Mon Jul 17 16:21:20 2023, max compression
```

## Comparing `django_celery_tracker-2.0.0.tar` & `django_celery_tracker-2.1.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 chris     (1000) wheel      (998)        0 2022-06-03 14:04:03.679716 django_celery_tracker-2.0.0/
--rw-r--r--   0 chris     (1000) wheel      (998)      120 2022-06-03 13:36:46.000000 django_celery_tracker-2.0.0/.coveragerc
--rw-r--r--   0 chris     (1000) wheel      (998)     1501 2022-06-03 13:59:51.000000 django_celery_tracker-2.0.0/CHANGELOG.md
--rw-r--r--   0 chris     (1000) wheel      (998)     1077 2020-05-27 18:41:50.000000 django_celery_tracker-2.0.0/LICENSE
--rw-r--r--   0 chris     (1000) wheel      (998)      420 2020-05-27 18:41:50.000000 django_celery_tracker-2.0.0/MANIFEST.in
--rw-r--r--   0 chris     (1000) wheel      (998)     4551 2022-06-03 14:04:03.679716 django_celery_tracker-2.0.0/PKG-INFO
--rw-r--r--   0 chris     (1000) wheel      (998)     3470 2022-06-03 13:36:46.000000 django_celery_tracker-2.0.0/README.rst
-drwxr-xr-x   0 chris     (1000) wheel      (998)        0 2022-06-03 14:04:03.676383 django_celery_tracker-2.0.0/django_celery_tracker/
--rw-r--r--   0 chris     (1000) wheel      (998)      908 2022-06-03 13:58:45.000000 django_celery_tracker-2.0.0/django_celery_tracker/__init__.py
--rw-r--r--   0 chris     (1000) wheel      (998)      518 2022-06-03 13:36:46.000000 django_celery_tracker-2.0.0/django_celery_tracker/apps.py
--rw-r--r--   0 chris     (1000) wheel      (998)      428 2020-05-27 18:41:50.000000 django_celery_tracker-2.0.0/django_celery_tracker/decorators.py
--rw-r--r--   0 chris     (1000) wheel      (998)      941 2020-05-27 18:41:50.000000 django_celery_tracker-2.0.0/django_celery_tracker/helpers.py
-drwxr-xr-x   0 chris     (1000) wheel      (998)        0 2022-06-03 14:04:03.000000 django_celery_tracker-2.0.0/django_celery_tracker/migrations/
--rw-r--r--   0 chris     (1000) wheel      (998)     1317 2020-05-27 18:41:50.000000 django_celery_tracker-2.0.0/django_celery_tracker/migrations/0001_initial.py
--rw-r--r--   0 chris     (1000) wheel      (998)      397 2020-05-27 18:41:50.000000 django_celery_tracker-2.0.0/django_celery_tracker/migrations/0002_celerytask_args.py
--rw-r--r--   0 chris     (1000) wheel      (998)        0 2020-05-27 18:41:50.000000 django_celery_tracker-2.0.0/django_celery_tracker/migrations/__init__.py
--rw-r--r--   0 chris     (1000) wheel      (998)      864 2020-05-27 18:41:50.000000 django_celery_tracker-2.0.0/django_celery_tracker/models.py
--rw-r--r--   0 chris     (1000) wheel      (998)     1165 2020-05-27 18:41:50.000000 django_celery_tracker-2.0.0/django_celery_tracker/signals.py
-drwxr-xr-x   0 chris     (1000) wheel      (998)        0 2022-06-03 14:04:03.000000 django_celery_tracker-2.0.0/django_celery_tracker/static/
-drwxr-xr-x   0 chris     (1000) wheel      (998)        0 2022-06-03 14:04:03.000000 django_celery_tracker-2.0.0/django_celery_tracker/static/celery_tracker/
-drwxr-xr-x   0 chris     (1000) wheel      (998)        0 2022-06-03 14:04:03.000000 django_celery_tracker-2.0.0/django_celery_tracker/static/celery_tracker/css/
--rw-r--r--   0 chris     (1000) wheel      (998)     1920 2022-06-03 13:58:15.000000 django_celery_tracker-2.0.0/django_celery_tracker/static/celery_tracker/css/dashboard.css
-drwxr-xr-x   0 chris     (1000) wheel      (998)        0 2022-06-03 14:04:03.000000 django_celery_tracker-2.0.0/django_celery_tracker/static/celery_tracker/fonts/
--rw-r--r--   0 chris     (1000) wheel      (998)     1408 2020-05-27 18:41:50.000000 django_celery_tracker-2.0.0/django_celery_tracker/static/celery_tracker/fonts/icomoon.ttf
-drwxr-xr-x   0 chris     (1000) wheel      (998)        0 2022-06-03 14:04:03.000000 django_celery_tracker-2.0.0/django_celery_tracker/static/celery_tracker/js/
--rw-r--r--   0 chris     (1000) wheel      (998)     4926 2020-05-27 18:41:50.000000 django_celery_tracker-2.0.0/django_celery_tracker/static/celery_tracker/js/dashboard.js
-drwxr-xr-x   0 chris     (1000) wheel      (998)        0 2022-06-03 14:04:03.000000 django_celery_tracker-2.0.0/django_celery_tracker/templates/
-drwxr-xr-x   0 chris     (1000) wheel      (998)        0 2022-06-03 14:04:03.000000 django_celery_tracker-2.0.0/django_celery_tracker/templates/celery_tracker/
--rw-r--r--   0 chris     (1000) wheel      (998)     2453 2020-05-27 18:41:50.000000 django_celery_tracker-2.0.0/django_celery_tracker/templates/celery_tracker/timeline_dashboard.html
--rw-r--r--   0 chris     (1000) wheel      (998)     1006 2022-06-03 13:36:46.000000 django_celery_tracker-2.0.0/django_celery_tracker/urls.py
--rw-r--r--   0 chris     (1000) wheel      (998)     2871 2022-06-03 13:47:05.000000 django_celery_tracker-2.0.0/django_celery_tracker/views.py
-drwxr-xr-x   0 chris     (1000) wheel      (998)        0 2022-06-03 14:04:03.679716 django_celery_tracker-2.0.0/django_celery_tracker.egg-info/
--rw-r--r--   0 chris     (1000) wheel      (998)     4551 2022-06-03 14:04:03.000000 django_celery_tracker-2.0.0/django_celery_tracker.egg-info/PKG-INFO
--rw-r--r--   0 chris     (1000) wheel      (998)     1341 2022-06-03 14:04:03.000000 django_celery_tracker-2.0.0/django_celery_tracker.egg-info/SOURCES.txt
--rw-r--r--   0 chris     (1000) wheel      (998)        1 2022-06-03 14:04:03.000000 django_celery_tracker-2.0.0/django_celery_tracker.egg-info/dependency_links.txt
--rw-r--r--   0 chris     (1000) wheel      (998)        1 2022-06-03 14:04:03.000000 django_celery_tracker-2.0.0/django_celery_tracker.egg-info/not-zip-safe
--rw-r--r--   0 chris     (1000) wheel      (998)       12 2022-06-03 14:04:03.000000 django_celery_tracker-2.0.0/django_celery_tracker.egg-info/requires.txt
--rw-r--r--   0 chris     (1000) wheel      (998)       22 2022-06-03 14:04:03.000000 django_celery_tracker-2.0.0/django_celery_tracker.egg-info/top_level.txt
--rwxr-xr-x   0 chris     (1000) wheel      (998)      545 2022-06-03 14:04:03.000000 django_celery_tracker-2.0.0/manage.py
-drwxr-xr-x   0 chris     (1000) wheel      (998)        0 2022-06-03 14:04:03.000000 django_celery_tracker-2.0.0/requirements/
--rw-r--r--   0 chris     (1000) wheel      (998)       11 2022-06-03 13:58:15.000000 django_celery_tracker-2.0.0/requirements/install.txt
--rw-r--r--   0 chris     (1000) wheel      (998)      190 2022-06-03 13:36:46.000000 django_celery_tracker-2.0.0/requirements/pkgutils.txt
--rw-r--r--   0 chris     (1000) wheel      (998)       91 2022-06-03 13:36:46.000000 django_celery_tracker-2.0.0/requirements/test.txt
--rw-r--r--   0 chris     (1000) wheel      (998)      353 2022-06-03 14:04:03.000000 django_celery_tracker-2.0.0/setup.cfg
--rw-r--r--   0 chris     (1000) wheel      (998)     3993 2022-06-03 14:04:03.000000 django_celery_tracker-2.0.0/setup.py
-drwxr-xr-x   0 chris     (1000) wheel      (998)        0 2022-06-03 14:04:03.000000 django_celery_tracker-2.0.0/tests/
--rw-r--r--   0 chris     (1000) wheel      (998)        0 2020-05-27 18:41:50.000000 django_celery_tracker-2.0.0/tests/__init__.py
-drwxr-xr-x   0 chris     (1000) wheel      (998)        0 2022-06-03 14:04:03.679716 django_celery_tracker-2.0.0/tests/testapp/
--rw-r--r--   0 chris     (1000) wheel      (998)       45 2020-05-27 18:41:50.000000 django_celery_tracker-2.0.0/tests/testapp/__init__.py
--rw-r--r--   0 chris     (1000) wheel      (998)      373 2020-05-27 18:41:50.000000 django_celery_tracker-2.0.0/tests/testapp/celery.py
--rw-r--r--   0 chris     (1000) wheel      (998)     2659 2020-05-27 18:41:50.000000 django_celery_tracker-2.0.0/tests/testapp/settings.py
--rw-r--r--   0 chris     (1000) wheel      (998)      208 2022-06-03 13:36:46.000000 django_celery_tracker-2.0.0/tests/testapp/urls.py
--rw-r--r--   0 chris     (1000) wheel      (998)      391 2020-05-27 18:41:50.000000 django_celery_tracker-2.0.0/tests/testapp/wsgi.py
-drwxr-xr-x   0 chris     (1000) wheel      (998)        0 2022-06-03 14:04:03.679716 django_celery_tracker-2.0.0/tests/unit/
--rw-r--r--   0 chris     (1000) wheel      (998)        0 2020-05-27 18:41:50.000000 django_celery_tracker-2.0.0/tests/unit/__init__.py
--rw-r--r--   0 chris     (1000) wheel      (998)     3850 2022-05-05 15:48:18.000000 django_celery_tracker-2.0.0/tests/unit/conftest.py
--rw-r--r--   0 chris     (1000) wheel      (998)     2848 2020-05-27 18:41:50.000000 django_celery_tracker-2.0.0/tests/unit/test_celerytask.py
--rw-r--r--   0 chris     (1000) wheel      (998)     5534 2020-05-27 18:41:50.000000 django_celery_tracker-2.0.0/tests/unit/test_dashboard.py
--rw-r--r--   0 chris     (1000) wheel      (998)      733 2022-06-03 14:04:03.000000 django_celery_tracker-2.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:21:20.374076 django_celery_tracker-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-17 16:21:09.000000 django_celery_tracker-2.1.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-17 16:21:09.000000 django_celery_tracker-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-17 16:21:09.000000 django_celery_tracker-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-07-17 16:21:20.374076 django_celery_tracker-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-17 16:21:09.000000 django_celery_tracker-2.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:21:20.370076 django_celery_tracker-2.1.0/django_celery_tracker/
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-17 16:21:09.000000 django_celery_tracker-2.1.0/django_celery_tracker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-17 16:21:09.000000 django_celery_tracker-2.1.0/django_celery_tracker/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-17 16:21:09.000000 django_celery_tracker-2.1.0/django_celery_tracker/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-17 16:21:09.000000 django_celery_tracker-2.1.0/django_celery_tracker/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:21:20.370076 django_celery_tracker-2.1.0/django_celery_tracker/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-07-17 16:21:09.000000 django_celery_tracker-2.1.0/django_celery_tracker/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-17 16:21:09.000000 django_celery_tracker-2.1.0/django_celery_tracker/migrations/0002_celerytask_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-17 16:21:09.000000 django_celery_tracker-2.1.0/django_celery_tracker/migrations/0003_alter_celerytask_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 16:21:09.000000 django_celery_tracker-2.1.0/django_celery_tracker/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-17 16:21:09.000000 django_celery_tracker-2.1.0/django_celery_tracker/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-17 16:21:09.000000 django_celery_tracker-2.1.0/django_celery_tracker/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:21:20.366076 django_celery_tracker-2.1.0/django_celery_tracker/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:21:20.366076 django_celery_tracker-2.1.0/django_celery_tracker/static/celery_tracker/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:21:20.374076 django_celery_tracker-2.1.0/django_celery_tracker/static/celery_tracker/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-17 16:21:09.000000 django_celery_tracker-2.1.0/django_celery_tracker/static/celery_tracker/css/dashboard.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:21:20.374076 django_celery_tracker-2.1.0/django_celery_tracker/static/celery_tracker/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-17 16:21:09.000000 django_celery_tracker-2.1.0/django_celery_tracker/static/celery_tracker/fonts/icomoon.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:21:20.374076 django_celery_tracker-2.1.0/django_celery_tracker/static/celery_tracker/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-07-17 16:21:09.000000 django_celery_tracker-2.1.0/django_celery_tracker/static/celery_tracker/js/dashboard.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:21:20.366076 django_celery_tracker-2.1.0/django_celery_tracker/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:21:20.374076 django_celery_tracker-2.1.0/django_celery_tracker/templates/celery_tracker/
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-17 16:21:09.000000 django_celery_tracker-2.1.0/django_celery_tracker/templates/celery_tracker/timeline_dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-17 16:21:09.000000 django_celery_tracker-2.1.0/django_celery_tracker/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-07-17 16:21:09.000000 django_celery_tracker-2.1.0/django_celery_tracker/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:21:20.370076 django_celery_tracker-2.1.0/django_celery_tracker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-07-17 16:21:20.000000 django_celery_tracker-2.1.0/django_celery_tracker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-17 16:21:20.000000 django_celery_tracker-2.1.0/django_celery_tracker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 16:21:20.000000 django_celery_tracker-2.1.0/django_celery_tracker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 16:21:20.000000 django_celery_tracker-2.1.0/django_celery_tracker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-17 16:21:20.000000 django_celery_tracker-2.1.0/django_celery_tracker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 16:21:20.000000 django_celery_tracker-2.1.0/django_celery_tracker.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      545 2023-07-17 16:21:09.000000 django_celery_tracker-2.1.0/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:21:20.374076 django_celery_tracker-2.1.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-17 16:21:09.000000 django_celery_tracker-2.1.0/requirements/install.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-17 16:21:09.000000 django_celery_tracker-2.1.0/requirements/pkgutils.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-17 16:21:09.000000 django_celery_tracker-2.1.0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-17 16:21:20.378076 django_celery_tracker-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-07-17 16:21:09.000000 django_celery_tracker-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:21:20.374076 django_celery_tracker-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 16:21:09.000000 django_celery_tracker-2.1.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:21:20.374076 django_celery_tracker-2.1.0/tests/testapp/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-17 16:21:09.000000 django_celery_tracker-2.1.0/tests/testapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-17 16:21:09.000000 django_celery_tracker-2.1.0/tests/testapp/celery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-07-17 16:21:09.000000 django_celery_tracker-2.1.0/tests/testapp/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-17 16:21:09.000000 django_celery_tracker-2.1.0/tests/testapp/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-17 16:21:09.000000 django_celery_tracker-2.1.0/tests/testapp/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:21:20.374076 django_celery_tracker-2.1.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 16:21:09.000000 django_celery_tracker-2.1.0/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-07-17 16:21:09.000000 django_celery_tracker-2.1.0/tests/unit/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-07-17 16:21:09.000000 django_celery_tracker-2.1.0/tests/unit/test_celerytask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-07-17 16:21:09.000000 django_celery_tracker-2.1.0/tests/unit/test_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-17 16:21:09.000000 django_celery_tracker-2.1.0/tox.ini
```

### Comparing `django_celery_tracker-2.0.0/LICENSE` & `django_celery_tracker-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_celery_tracker-2.0.0/django_celery_tracker/__init__.py` & `django_celery_tracker-2.1.0/django_celery_tracker/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from __future__ import absolute_import, unicode_literals
 
 import re
 
 from collections import namedtuple
 
-__version__ = '2.0.0'
+__version__ = '2.1.0'
 __author__ = 'Chris Allen'
 __contact__ = 'chris@apaxsoftware.com'
 __homepage__ = 'https://github.com/chris-allen/django-celery-tracker'
 __docformat__ = 'restructuredtext'
 
 # -eof meta-
 
@@ -24,11 +24,11 @@
 
 # bumpversion can only search for {current_version}
 # so we have to parse the version here.
 _temp = re.match(
     r'(\d+)\.(\d+).(\d+)(.+)?', __version__).groups()
 VERSION = version_info = version_info_t(
     int(_temp[0]), int(_temp[1]), int(_temp[2]), _temp[3] or '', '')
-del(_temp)
-del(re)
+del _temp
+del re
 
 __all__ = []
```

### Comparing `django_celery_tracker-2.0.0/django_celery_tracker/apps.py` & `django_celery_tracker-2.1.0/django_celery_tracker/apps.py`

 * *Files identical despite different names*

### Comparing `django_celery_tracker-2.0.0/django_celery_tracker/helpers.py` & `django_celery_tracker-2.1.0/django_celery_tracker/helpers.py`

 * *Files identical despite different names*

### Comparing `django_celery_tracker-2.0.0/django_celery_tracker/migrations/0001_initial.py` & `django_celery_tracker-2.1.0/django_celery_tracker/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_celery_tracker-2.0.0/django_celery_tracker/models.py` & `django_celery_tracker-2.1.0/django_celery_tracker/models.py`

 * *Files identical despite different names*

### Comparing `django_celery_tracker-2.0.0/django_celery_tracker/signals.py` & `django_celery_tracker-2.1.0/django_celery_tracker/signals.py`

 * *Files identical despite different names*

### Comparing `django_celery_tracker-2.0.0/django_celery_tracker/static/celery_tracker/css/dashboard.css` & `django_celery_tracker-2.1.0/django_celery_tracker/static/celery_tracker/css/dashboard.css`

 * *Files identical despite different names*

### Comparing `django_celery_tracker-2.0.0/django_celery_tracker/static/celery_tracker/fonts/icomoon.ttf` & `django_celery_tracker-2.1.0/django_celery_tracker/static/celery_tracker/fonts/icomoon.ttf`

 * *Files identical despite different names*

### Comparing `django_celery_tracker-2.0.0/django_celery_tracker/static/celery_tracker/js/dashboard.js` & `django_celery_tracker-2.1.0/django_celery_tracker/static/celery_tracker/js/dashboard.js`

 * *Files identical despite different names*

### Comparing `django_celery_tracker-2.0.0/django_celery_tracker/templates/celery_tracker/timeline_dashboard.html` & `django_celery_tracker-2.1.0/django_celery_tracker/templates/celery_tracker/timeline_dashboard.html`

 * *Files identical despite different names*

### Comparing `django_celery_tracker-2.0.0/django_celery_tracker/urls.py` & `django_celery_tracker-2.1.0/django_celery_tracker/urls.py`

 * *Files identical despite different names*

### Comparing `django_celery_tracker-2.0.0/django_celery_tracker/views.py` & `django_celery_tracker-2.1.0/django_celery_tracker/views.py`

 * *Files identical despite different names*

### Comparing `django_celery_tracker-2.0.0/django_celery_tracker.egg-info/SOURCES.txt` & `django_celery_tracker-2.1.0/django_celery_tracker.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 .coveragerc
-CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.rst
 manage.py
 setup.cfg
 setup.py
 tox.ini
@@ -19,14 +18,15 @@
 django_celery_tracker.egg-info/SOURCES.txt
 django_celery_tracker.egg-info/dependency_links.txt
 django_celery_tracker.egg-info/not-zip-safe
 django_celery_tracker.egg-info/requires.txt
 django_celery_tracker.egg-info/top_level.txt
 django_celery_tracker/migrations/0001_initial.py
 django_celery_tracker/migrations/0002_celerytask_args.py
+django_celery_tracker/migrations/0003_alter_celerytask_id.py
 django_celery_tracker/migrations/__init__.py
 django_celery_tracker/static/celery_tracker/css/dashboard.css
 django_celery_tracker/static/celery_tracker/fonts/icomoon.ttf
 django_celery_tracker/static/celery_tracker/js/dashboard.js
 django_celery_tracker/templates/celery_tracker/timeline_dashboard.html
 requirements/install.txt
 requirements/pkgutils.txt
```

### Comparing `django_celery_tracker-2.0.0/manage.py` & `django_celery_tracker-2.1.0/manage.py`

 * *Files identical despite different names*

### Comparing `django_celery_tracker-2.0.0/setup.py` & `django_celery_tracker-2.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     Programming Language :: Python :: 3
     Programming Language :: Python :: 3.8
     Programming Language :: Python :: 3.10
     Programming Language :: Python :: Implementation :: CPython
     Programming Language :: Python :: Implementation :: PyPy
     Framework :: Django
     Framework :: Django :: 3.2
-    Framework :: Django :: 4.0
+    Framework :: Django :: 4.2
     Operating System :: OS Independent
     Topic :: Communications
     Topic :: System :: Distributed Computing
     Topic :: Software Development :: Libraries :: Python Modules
 """
 classifiers = [s.strip() for s in classes.split('\n') if s]
```

### Comparing `django_celery_tracker-2.0.0/tests/testapp/settings.py` & `django_celery_tracker-2.1.0/tests/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `django_celery_tracker-2.0.0/tests/unit/conftest.py` & `django_celery_tracker-2.1.0/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `django_celery_tracker-2.0.0/tests/unit/test_celerytask.py` & `django_celery_tracker-2.1.0/tests/unit/test_celerytask.py`

 * *Files identical despite different names*

### Comparing `django_celery_tracker-2.0.0/tests/unit/test_dashboard.py` & `django_celery_tracker-2.1.0/tests/unit/test_dashboard.py`

 * *Files identical despite different names*

### Comparing `django_celery_tracker-2.0.0/tox.ini` & `django_celery_tracker-2.1.0/tox.ini`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 
 [tox]
 envlist =
     tests-py{38,310}-dj3-celery{4,5},
-    tests-py{38,310}-dj4-celery5
+    tests-py{38,310}-dj4-celery5,
     flake8,manifest,readme
 
-; [travis]
-; python =
-;   2.7: py27, apicheck, builddocs, flake8
-
-; [travis:after]
-; travis = python: 3.5
+[gh-actions]
+python =
+    3.8: py38
+    3.10: py310, flake8, manifest, readme
 
 [testenv]
 sitepackages = False
 deps=
     -r{toxinidir}/requirements/test.txt
 
     dj3: django>=3.2,<4
```

