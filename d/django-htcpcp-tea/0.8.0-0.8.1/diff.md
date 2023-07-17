# Comparing `tmp/django_htcpcp_tea-0.8.0.tar.gz` & `tmp/django_htcpcp_tea-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_htcpcp_tea-0.8.0.tar", max compression
+gzip compressed data, was "django_htcpcp_tea-0.8.1.tar", max compression
```

## Comparing `django_htcpcp_tea-0.8.0.tar` & `django_htcpcp_tea-0.8.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     4294 2023-07-17 17:49:14.283743 django_htcpcp_tea-0.8.0/CHANGELOG.rst
--rwxr-xr-x   0        0        0     1071 2019-07-05 01:21:10.480690 django_htcpcp_tea-0.8.0/LICENSE
--rw-r--r--   0        0        0     3031 2019-08-30 02:21:23.636411 django_htcpcp_tea-0.8.0/README.rst
--rw-r--r--   0        0        0      306 2023-07-17 17:49:14.283743 django_htcpcp_tea-0.8.0/django_htcpcp_tea/__init__.py
--rw-r--r--   0        0        0     7598 2023-07-17 17:48:53.536061 django_htcpcp_tea-0.8.0/django_htcpcp_tea/admin.py
--rw-r--r--   0        0        0      361 2023-07-17 17:48:53.536061 django_htcpcp_tea-0.8.0/django_htcpcp_tea/apps.py
--rw-r--r--   0        0        0     1695 2023-07-17 17:48:53.536061 django_htcpcp_tea-0.8.0/django_htcpcp_tea/decorators.py
--rw-r--r--   0        0        0      962 2019-07-05 13:07:23.045128 django_htcpcp_tea-0.8.0/django_htcpcp_tea/fixtures/demo_forbidden_combinations.json
--rw-r--r--   0        0        0      687 2019-07-08 15:32:37.355564 django_htcpcp_tea-0.8.0/django_htcpcp_tea/fixtures/demo_pots.json
--rw-r--r--   0        0        0     1354 2019-07-05 01:29:03.962812 django_htcpcp_tea-0.8.0/django_htcpcp_tea/fixtures/rfc_2324_additions.json
--rw-r--r--   0        0        0      289 2019-07-05 01:29:03.962812 django_htcpcp_tea-0.8.0/django_htcpcp_tea/fixtures/rfc_7168_additions.json
--rw-r--r--   0        0        0      314 2019-07-05 01:29:03.962812 django_htcpcp_tea-0.8.0/django_htcpcp_tea/fixtures/rfc_7168_teas.json
--rw-r--r--   0        0        0     2925 2023-07-17 17:48:53.536061 django_htcpcp_tea-0.8.0/django_htcpcp_tea/middleware.py
--rw-r--r--   0        0        0     1461 2023-07-17 16:59:39.561974 django_htcpcp_tea-0.8.0/django_htcpcp_tea/migrations/0001_initial.py
--rw-r--r--   0        0        0     1429 2023-07-17 16:59:39.561974 django_htcpcp_tea-0.8.0/django_htcpcp_tea/migrations/0002_auto_20190619_1041.py
--rw-r--r--   0        0        0      448 2023-07-17 16:59:39.561974 django_htcpcp_tea-0.8.0/django_htcpcp_tea/migrations/0003_auto_20190620_1205.py
--rw-r--r--   0        0        0      615 2023-07-17 16:59:39.561974 django_htcpcp_tea-0.8.0/django_htcpcp_tea/migrations/0004_addition_type.py
--rw-r--r--   0        0        0      990 2023-07-17 17:02:49.590597 django_htcpcp_tea-0.8.0/django_htcpcp_tea/migrations/0005_forbiddencombination.py
--rw-r--r--   0        0        0        0 2019-07-05 01:21:10.480690 django_htcpcp_tea-0.8.0/django_htcpcp_tea/migrations/__init__.py
--rw-r--r--   0        0        0     5671 2023-07-17 17:48:53.536061 django_htcpcp_tea-0.8.0/django_htcpcp_tea/models.py
--rw-r--r--   0        0        0     1229 2023-07-17 17:48:53.536061 django_htcpcp_tea-0.8.0/django_htcpcp_tea/settings.py
--rw-r--r--   0        0        0      258 2019-07-05 01:29:03.962812 django_htcpcp_tea-0.8.0/django_htcpcp_tea/templates/django_htcpcp_tea/400.html
--rw-r--r--   0        0        0      522 2019-07-05 13:07:23.045128 django_htcpcp_tea-0.8.0/django_htcpcp_tea/templates/django_htcpcp_tea/403.html
--rw-r--r--   0        0        0      497 2019-07-05 01:29:03.962812 django_htcpcp_tea-0.8.0/django_htcpcp_tea/templates/django_htcpcp_tea/406.html
--rw-r--r--   0        0        0      265 2019-07-05 01:29:03.962812 django_htcpcp_tea-0.8.0/django_htcpcp_tea/templates/django_htcpcp_tea/418.html
--rw-r--r--   0        0        0      181 2019-07-05 01:29:03.962812 django_htcpcp_tea-0.8.0/django_htcpcp_tea/templates/django_htcpcp_tea/503.html
--rw-r--r--   0        0        0      176 2019-07-05 01:21:10.480690 django_htcpcp_tea-0.8.0/django_htcpcp_tea/templates/django_htcpcp_tea/base.html
--rw-r--r--   0        0        0       44 2019-07-05 01:29:03.962812 django_htcpcp_tea-0.8.0/django_htcpcp_tea/templates/django_htcpcp_tea/base_beverage.html
--rw-r--r--   0        0        0      179 2019-07-05 01:29:03.962812 django_htcpcp_tea-0.8.0/django_htcpcp_tea/templates/django_htcpcp_tea/base_error.html
--rw-r--r--   0        0        0      584 2019-07-05 01:29:03.962812 django_htcpcp_tea-0.8.0/django_htcpcp_tea/templates/django_htcpcp_tea/brewing.html
--rw-r--r--   0        0        0      375 2019-07-05 01:29:03.962812 django_htcpcp_tea-0.8.0/django_htcpcp_tea/templates/django_htcpcp_tea/finished.html
--rw-r--r--   0        0        0      389 2019-07-05 01:29:03.962812 django_htcpcp_tea-0.8.0/django_htcpcp_tea/templates/django_htcpcp_tea/includes/additions.html
--rw-r--r--   0        0        0      170 2019-07-05 01:29:03.962812 django_htcpcp_tea-0.8.0/django_htcpcp_tea/templates/django_htcpcp_tea/includes/alternatives.html
--rw-r--r--   0        0        0      182 2019-07-05 01:29:03.962812 django_htcpcp_tea-0.8.0/django_htcpcp_tea/templates/django_htcpcp_tea/options.html
--rw-r--r--   0        0        0      148 2019-07-05 01:29:03.962812 django_htcpcp_tea-0.8.0/django_htcpcp_tea/templates/django_htcpcp_tea/pouring.html
--rw-r--r--   0        0        0      498 2023-07-17 17:48:53.536061 django_htcpcp_tea-0.8.0/django_htcpcp_tea/urls.py
--rw-r--r--   0        0        0     2690 2023-07-17 17:48:53.536061 django_htcpcp_tea-0.8.0/django_htcpcp_tea/utils.py
--rw-r--r--   0        0        0    10719 2023-07-17 17:48:53.536061 django_htcpcp_tea-0.8.0/django_htcpcp_tea/views.py
--rw-r--r--   0        0        0      580 2019-07-05 01:29:03.962812 django_htcpcp_tea-0.8.0/docs/Makefile
--rw-r--r--   0        0        0        0 2019-07-05 01:29:03.962812 django_htcpcp_tea-0.8.0/docs/_static/.gitkeep
--rw-r--r--   0        0        0        0 2019-07-05 01:29:03.962812 django_htcpcp_tea-0.8.0/docs/_templates/.gitkeep
--rw-r--r--   0        0        0     2264 2019-08-30 02:21:23.640411 django_htcpcp_tea-0.8.0/docs/api.rst
--rw-r--r--   0        0        0      212 2019-07-14 17:03:10.222453 django_htcpcp_tea-0.8.0/docs/changelog.rst
--rw-r--r--   0        0        0     2120 2023-07-17 17:49:14.283743 django_htcpcp_tea-0.8.0/docs/conf.py
--rw-r--r--   0        0        0    12177 2019-08-30 02:21:23.640411 django_htcpcp_tea-0.8.0/docs/config.rst
--rw-r--r--   0        0        0    12979 2023-07-17 17:48:53.536061 django_htcpcp_tea-0.8.0/docs/examples.rst
--rw-r--r--   0        0        0      596 2019-08-30 02:21:23.640411 django_htcpcp_tea-0.8.0/docs/index.rst
--rw-r--r--   0        0        0     4852 2019-10-06 23:18:06.797581 django_htcpcp_tea-0.8.0/docs/install.rst
--rw-r--r--   0        0        0      752 2019-07-05 01:29:03.962812 django_htcpcp_tea-0.8.0/docs/make.bat
--rw-r--r--   0        0        0       12 2019-07-14 17:03:10.222453 django_htcpcp_tea-0.8.0/docs/requirements.txt
--rw-r--r--   0        0        0     1864 2023-07-17 17:49:14.283743 django_htcpcp_tea-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     8636 1970-01-01 00:00:00.000000 django_htcpcp_tea-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     4362 2023-07-17 18:10:35.325097 django_htcpcp_tea-0.8.1/CHANGELOG.rst
+-rwxr-xr-x   0        0        0     1071 2019-07-05 01:21:10.480690 django_htcpcp_tea-0.8.1/LICENSE
+-rw-r--r--   0        0        0     3031 2019-08-30 02:21:23.636411 django_htcpcp_tea-0.8.1/README.rst
+-rw-r--r--   0        0        0      306 2023-07-17 18:10:35.325097 django_htcpcp_tea-0.8.1/django_htcpcp_tea/__init__.py
+-rw-r--r--   0        0        0     7598 2023-07-17 17:48:53.536061 django_htcpcp_tea-0.8.1/django_htcpcp_tea/admin.py
+-rw-r--r--   0        0        0      361 2023-07-17 17:48:53.536061 django_htcpcp_tea-0.8.1/django_htcpcp_tea/apps.py
+-rw-r--r--   0        0        0     1695 2023-07-17 17:48:53.536061 django_htcpcp_tea-0.8.1/django_htcpcp_tea/decorators.py
+-rw-r--r--   0        0        0      962 2019-07-05 13:07:23.045128 django_htcpcp_tea-0.8.1/django_htcpcp_tea/fixtures/demo_forbidden_combinations.json
+-rw-r--r--   0        0        0      687 2019-07-08 15:32:37.355564 django_htcpcp_tea-0.8.1/django_htcpcp_tea/fixtures/demo_pots.json
+-rw-r--r--   0        0        0     1354 2019-07-05 01:29:03.962812 django_htcpcp_tea-0.8.1/django_htcpcp_tea/fixtures/rfc_2324_additions.json
+-rw-r--r--   0        0        0      289 2019-07-05 01:29:03.962812 django_htcpcp_tea-0.8.1/django_htcpcp_tea/fixtures/rfc_7168_additions.json
+-rw-r--r--   0        0        0      314 2019-07-05 01:29:03.962812 django_htcpcp_tea-0.8.1/django_htcpcp_tea/fixtures/rfc_7168_teas.json
+-rw-r--r--   0        0        0     2925 2023-07-17 17:48:53.536061 django_htcpcp_tea-0.8.1/django_htcpcp_tea/middleware.py
+-rw-r--r--   0        0        0     1461 2023-07-17 16:59:39.561974 django_htcpcp_tea-0.8.1/django_htcpcp_tea/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1429 2023-07-17 16:59:39.561974 django_htcpcp_tea-0.8.1/django_htcpcp_tea/migrations/0002_auto_20190619_1041.py
+-rw-r--r--   0        0        0      448 2023-07-17 16:59:39.561974 django_htcpcp_tea-0.8.1/django_htcpcp_tea/migrations/0003_auto_20190620_1205.py
+-rw-r--r--   0        0        0      615 2023-07-17 16:59:39.561974 django_htcpcp_tea-0.8.1/django_htcpcp_tea/migrations/0004_addition_type.py
+-rw-r--r--   0        0        0      990 2023-07-17 17:02:49.590597 django_htcpcp_tea-0.8.1/django_htcpcp_tea/migrations/0005_forbiddencombination.py
+-rw-r--r--   0        0        0        0 2019-07-05 01:21:10.480690 django_htcpcp_tea-0.8.1/django_htcpcp_tea/migrations/__init__.py
+-rw-r--r--   0        0        0     5671 2023-07-17 17:48:53.536061 django_htcpcp_tea-0.8.1/django_htcpcp_tea/models.py
+-rw-r--r--   0        0        0     1229 2023-07-17 17:48:53.536061 django_htcpcp_tea-0.8.1/django_htcpcp_tea/settings.py
+-rw-r--r--   0        0        0      258 2019-07-05 01:29:03.962812 django_htcpcp_tea-0.8.1/django_htcpcp_tea/templates/django_htcpcp_tea/400.html
+-rw-r--r--   0        0        0      522 2019-07-05 13:07:23.045128 django_htcpcp_tea-0.8.1/django_htcpcp_tea/templates/django_htcpcp_tea/403.html
+-rw-r--r--   0        0        0      497 2019-07-05 01:29:03.962812 django_htcpcp_tea-0.8.1/django_htcpcp_tea/templates/django_htcpcp_tea/406.html
+-rw-r--r--   0        0        0      265 2019-07-05 01:29:03.962812 django_htcpcp_tea-0.8.1/django_htcpcp_tea/templates/django_htcpcp_tea/418.html
+-rw-r--r--   0        0        0      181 2019-07-05 01:29:03.962812 django_htcpcp_tea-0.8.1/django_htcpcp_tea/templates/django_htcpcp_tea/503.html
+-rw-r--r--   0        0        0      176 2019-07-05 01:21:10.480690 django_htcpcp_tea-0.8.1/django_htcpcp_tea/templates/django_htcpcp_tea/base.html
+-rw-r--r--   0        0        0       44 2019-07-05 01:29:03.962812 django_htcpcp_tea-0.8.1/django_htcpcp_tea/templates/django_htcpcp_tea/base_beverage.html
+-rw-r--r--   0        0        0      179 2019-07-05 01:29:03.962812 django_htcpcp_tea-0.8.1/django_htcpcp_tea/templates/django_htcpcp_tea/base_error.html
+-rw-r--r--   0        0        0      584 2019-07-05 01:29:03.962812 django_htcpcp_tea-0.8.1/django_htcpcp_tea/templates/django_htcpcp_tea/brewing.html
+-rw-r--r--   0        0        0      375 2019-07-05 01:29:03.962812 django_htcpcp_tea-0.8.1/django_htcpcp_tea/templates/django_htcpcp_tea/finished.html
+-rw-r--r--   0        0        0      389 2019-07-05 01:29:03.962812 django_htcpcp_tea-0.8.1/django_htcpcp_tea/templates/django_htcpcp_tea/includes/additions.html
+-rw-r--r--   0        0        0      170 2019-07-05 01:29:03.962812 django_htcpcp_tea-0.8.1/django_htcpcp_tea/templates/django_htcpcp_tea/includes/alternatives.html
+-rw-r--r--   0        0        0      182 2019-07-05 01:29:03.962812 django_htcpcp_tea-0.8.1/django_htcpcp_tea/templates/django_htcpcp_tea/options.html
+-rw-r--r--   0        0        0      148 2019-07-05 01:29:03.962812 django_htcpcp_tea-0.8.1/django_htcpcp_tea/templates/django_htcpcp_tea/pouring.html
+-rw-r--r--   0        0        0      498 2023-07-17 17:48:53.536061 django_htcpcp_tea-0.8.1/django_htcpcp_tea/urls.py
+-rw-r--r--   0        0        0     2690 2023-07-17 17:48:53.536061 django_htcpcp_tea-0.8.1/django_htcpcp_tea/utils.py
+-rw-r--r--   0        0        0    10719 2023-07-17 17:48:53.536061 django_htcpcp_tea-0.8.1/django_htcpcp_tea/views.py
+-rw-r--r--   0        0        0      580 2019-07-05 01:29:03.962812 django_htcpcp_tea-0.8.1/docs/Makefile
+-rw-r--r--   0        0        0        0 2019-07-05 01:29:03.962812 django_htcpcp_tea-0.8.1/docs/_static/.gitkeep
+-rw-r--r--   0        0        0        0 2019-07-05 01:29:03.962812 django_htcpcp_tea-0.8.1/docs/_templates/.gitkeep
+-rw-r--r--   0        0        0     2264 2019-08-30 02:21:23.640411 django_htcpcp_tea-0.8.1/docs/api.rst
+-rw-r--r--   0        0        0      212 2019-07-14 17:03:10.222453 django_htcpcp_tea-0.8.1/docs/changelog.rst
+-rw-r--r--   0        0        0     2120 2023-07-17 18:10:35.325097 django_htcpcp_tea-0.8.1/docs/conf.py
+-rw-r--r--   0        0        0    12177 2019-08-30 02:21:23.640411 django_htcpcp_tea-0.8.1/docs/config.rst
+-rw-r--r--   0        0        0    12979 2023-07-17 17:48:53.536061 django_htcpcp_tea-0.8.1/docs/examples.rst
+-rw-r--r--   0        0        0      596 2019-08-30 02:21:23.640411 django_htcpcp_tea-0.8.1/docs/index.rst
+-rw-r--r--   0        0        0     4852 2019-10-06 23:18:06.797581 django_htcpcp_tea-0.8.1/docs/install.rst
+-rw-r--r--   0        0        0      752 2019-07-05 01:29:03.962812 django_htcpcp_tea-0.8.1/docs/make.bat
+-rw-r--r--   0        0        0       12 2019-07-14 17:03:10.222453 django_htcpcp_tea-0.8.1/docs/requirements.txt
+-rw-r--r--   0        0        0     1860 2023-07-17 18:10:35.325097 django_htcpcp_tea-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     8704 1970-01-01 00:00:00.000000 django_htcpcp_tea-0.8.1/PKG-INFO
```

### Comparing `django_htcpcp_tea-0.8.0/CHANGELOG.rst` & `django_htcpcp_tea-0.8.1/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 Changes
 =======
 
 For complete record of changes, see the commit log of the `public git repository`_.
 
 .. _public git repository: https://github.com/blueschu/django-htcpcp-tea
 
+v0.8.1
+-------
+
+- Patch development ``django-debug-toolbar`` version
+
+
 v0.8.0
-----------
+-------
 
 - Migrated build system from ``setuptools`` to ``poetry``.
 - Upgraded supported Python versions from 3.4-3.8 to 3.8+.
 - Development: use black formatting and isort import ordering.
 
 v0.7.0
 ------
```

### Comparing `django_htcpcp_tea-0.8.0/LICENSE` & `django_htcpcp_tea-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_htcpcp_tea-0.8.0/README.rst` & `django_htcpcp_tea-0.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `django_htcpcp_tea-0.8.0/django_htcpcp_tea/admin.py` & `django_htcpcp_tea-0.8.1/django_htcpcp_tea/admin.py`

 * *Files identical despite different names*

### Comparing `django_htcpcp_tea-0.8.0/django_htcpcp_tea/decorators.py` & `django_htcpcp_tea-0.8.1/django_htcpcp_tea/decorators.py`

 * *Files identical despite different names*

### Comparing `django_htcpcp_tea-0.8.0/django_htcpcp_tea/fixtures/demo_forbidden_combinations.json` & `django_htcpcp_tea-0.8.1/django_htcpcp_tea/fixtures/demo_forbidden_combinations.json`

 * *Files identical despite different names*

### Comparing `django_htcpcp_tea-0.8.0/django_htcpcp_tea/fixtures/demo_pots.json` & `django_htcpcp_tea-0.8.1/django_htcpcp_tea/fixtures/demo_pots.json`

 * *Files identical despite different names*

### Comparing `django_htcpcp_tea-0.8.0/django_htcpcp_tea/fixtures/rfc_2324_additions.json` & `django_htcpcp_tea-0.8.1/django_htcpcp_tea/fixtures/rfc_2324_additions.json`

 * *Files identical despite different names*

### Comparing `django_htcpcp_tea-0.8.0/django_htcpcp_tea/middleware.py` & `django_htcpcp_tea-0.8.1/django_htcpcp_tea/middleware.py`

 * *Files identical despite different names*

### Comparing `django_htcpcp_tea-0.8.0/django_htcpcp_tea/migrations/0001_initial.py` & `django_htcpcp_tea-0.8.1/django_htcpcp_tea/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_htcpcp_tea-0.8.0/django_htcpcp_tea/migrations/0002_auto_20190619_1041.py` & `django_htcpcp_tea-0.8.1/django_htcpcp_tea/migrations/0002_auto_20190619_1041.py`

 * *Files identical despite different names*

### Comparing `django_htcpcp_tea-0.8.0/django_htcpcp_tea/migrations/0004_addition_type.py` & `django_htcpcp_tea-0.8.1/django_htcpcp_tea/migrations/0004_addition_type.py`

 * *Files identical despite different names*

### Comparing `django_htcpcp_tea-0.8.0/django_htcpcp_tea/migrations/0005_forbiddencombination.py` & `django_htcpcp_tea-0.8.1/django_htcpcp_tea/migrations/0005_forbiddencombination.py`

 * *Files identical despite different names*

### Comparing `django_htcpcp_tea-0.8.0/django_htcpcp_tea/models.py` & `django_htcpcp_tea-0.8.1/django_htcpcp_tea/models.py`

 * *Files identical despite different names*

### Comparing `django_htcpcp_tea-0.8.0/django_htcpcp_tea/settings.py` & `django_htcpcp_tea-0.8.1/django_htcpcp_tea/settings.py`

 * *Files identical despite different names*

### Comparing `django_htcpcp_tea-0.8.0/django_htcpcp_tea/templates/django_htcpcp_tea/403.html` & `django_htcpcp_tea-0.8.1/django_htcpcp_tea/templates/django_htcpcp_tea/403.html`

 * *Files identical despite different names*

### Comparing `django_htcpcp_tea-0.8.0/django_htcpcp_tea/templates/django_htcpcp_tea/brewing.html` & `django_htcpcp_tea-0.8.1/django_htcpcp_tea/templates/django_htcpcp_tea/brewing.html`

 * *Files identical despite different names*

### Comparing `django_htcpcp_tea-0.8.0/django_htcpcp_tea/utils.py` & `django_htcpcp_tea-0.8.1/django_htcpcp_tea/utils.py`

 * *Files identical despite different names*

### Comparing `django_htcpcp_tea-0.8.0/django_htcpcp_tea/views.py` & `django_htcpcp_tea-0.8.1/django_htcpcp_tea/views.py`

 * *Files identical despite different names*

### Comparing `django_htcpcp_tea-0.8.0/docs/Makefile` & `django_htcpcp_tea-0.8.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django_htcpcp_tea-0.8.0/docs/api.rst` & `django_htcpcp_tea-0.8.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `django_htcpcp_tea-0.8.0/docs/conf.py` & `django_htcpcp_tea-0.8.1/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # -- Project information -----------------------------------------------------
 
 project = 'django-htcpcp-tea'
 copyright = '2019, Brian Schubert'
 author = 'Brian Schubert'
 
 # The full version, including alpha/beta/rc tags
-release = '0.8.0'
+release = '0.8.1'
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `django_htcpcp_tea-0.8.0/docs/config.rst` & `django_htcpcp_tea-0.8.1/docs/config.rst`

 * *Files identical despite different names*

### Comparing `django_htcpcp_tea-0.8.0/docs/examples.rst` & `django_htcpcp_tea-0.8.1/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `django_htcpcp_tea-0.8.0/docs/index.rst` & `django_htcpcp_tea-0.8.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django_htcpcp_tea-0.8.0/docs/install.rst` & `django_htcpcp_tea-0.8.1/docs/install.rst`

 * *Files identical despite different names*

### Comparing `django_htcpcp_tea-0.8.0/docs/make.bat` & `django_htcpcp_tea-0.8.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django_htcpcp_tea-0.8.0/pyproject.toml` & `django_htcpcp_tea-0.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-htcpcp-tea"
-version = "0.8.0"
+version = "0.8.1"
 description = "Django app implementing HTCPCP-TEA as defined in RFC 7168."
 license = "MIT"
 authors = ["Brian Schubert <brianm.schubert@gmail.com>"]
 readme = ["README.rst", "CHANGELOG.rst"]
 repository = "https://github.com/blueschu/django-htcpcp-tea"
 documentation = "https://django-htcpcp-tea.readthedocs.io/en/latest/"
 keywords = ["htcpcp", "django", "rfc-2324", "rfc-7168", "coffee", "tea"]
@@ -32,15 +32,15 @@
 django = "^2.0,<3.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.7.0"
 isort = "^5.12.0"
 
 [tool.poetry.group.sample.dependencies]
-django-debug-toolbar = ">=2,<2.1"
+django-debug-toolbar = "^2.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 # Black config.
 [tool.black]
```

### Comparing `django_htcpcp_tea-0.8.0/PKG-INFO` & `django_htcpcp_tea-0.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-htcpcp-tea
-Version: 0.8.0
+Version: 0.8.1
 Summary: Django app implementing HTCPCP-TEA as defined in RFC 7168.
 Home-page: https://github.com/blueschu/django-htcpcp-tea
 License: MIT
 Keywords: htcpcp,django,rfc-2324,rfc-7168,coffee,tea
 Author: Brian Schubert
 Author-email: brianm.schubert@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -116,16 +116,22 @@
 Changes
 =======
 
 For complete record of changes, see the commit log of the `public git repository`_.
 
 .. _public git repository: https://github.com/blueschu/django-htcpcp-tea
 
+v0.8.1
+-------
+
+- Patch development ``django-debug-toolbar`` version
+
+
 v0.8.0
-----------
+-------
 
 - Migrated build system from ``setuptools`` to ``poetry``.
 - Upgraded supported Python versions from 3.4-3.8 to 3.8+.
 - Development: use black formatting and isort import ordering.
 
 v0.7.0
 ------
```

