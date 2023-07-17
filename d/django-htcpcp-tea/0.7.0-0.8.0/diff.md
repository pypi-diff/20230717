# Comparing `tmp/django-htcpcp-tea-0.7.0.tar.gz` & `tmp/django_htcpcp_tea-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-htcpcp-tea-0.7.0.tar", last modified: Fri Aug 30 02:25:03 2019, max compression
+gzip compressed data, was "django_htcpcp_tea-0.8.0.tar", max compression
```

## Comparing `django-htcpcp-tea-0.7.0.tar` & `django_htcpcp_tea-0.8.0.tar`

### file list

```diff
@@ -1,69 +1,52 @@
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2019-08-30 02:25:03.000000 django-htcpcp-tea-0.7.0/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2019-08-30 02:25:03.000000 django-htcpcp-tea-0.7.0/docs/
--rw-rw-r--   0 brian     (1000) brian     (1000)       12 2019-07-14 17:03:10.000000 django-htcpcp-tea-0.7.0/docs/requirements.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)    12908 2019-08-30 02:21:23.000000 django-htcpcp-tea-0.7.0/docs/examples.rst
--rw-rw-r--   0 brian     (1000) brian     (1000)    12177 2019-08-30 02:21:23.000000 django-htcpcp-tea-0.7.0/docs/config.rst
--rw-rw-r--   0 brian     (1000) brian     (1000)     2120 2019-08-30 02:22:46.000000 django-htcpcp-tea-0.7.0/docs/conf.py
--rw-rw-r--   0 brian     (1000) brian     (1000)      596 2019-08-30 02:21:23.000000 django-htcpcp-tea-0.7.0/docs/index.rst
--rw-rw-r--   0 brian     (1000) brian     (1000)      752 2019-07-05 01:29:03.000000 django-htcpcp-tea-0.7.0/docs/make.bat
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2019-08-30 02:25:03.000000 django-htcpcp-tea-0.7.0/docs/_static/
--rw-rw-r--   0 brian     (1000) brian     (1000)        0 2019-07-05 01:29:03.000000 django-htcpcp-tea-0.7.0/docs/_static/.gitkeep
--rw-rw-r--   0 brian     (1000) brian     (1000)     2264 2019-08-30 02:21:23.000000 django-htcpcp-tea-0.7.0/docs/api.rst
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2019-08-30 02:25:03.000000 django-htcpcp-tea-0.7.0/docs/_templates/
--rw-rw-r--   0 brian     (1000) brian     (1000)        0 2019-07-05 01:29:03.000000 django-htcpcp-tea-0.7.0/docs/_templates/.gitkeep
--rw-rw-r--   0 brian     (1000) brian     (1000)      212 2019-07-14 17:03:10.000000 django-htcpcp-tea-0.7.0/docs/changelog.rst
--rw-rw-r--   0 brian     (1000) brian     (1000)      580 2019-07-05 01:29:03.000000 django-htcpcp-tea-0.7.0/docs/Makefile
--rw-rw-r--   0 brian     (1000) brian     (1000)     4852 2019-08-30 02:21:23.000000 django-htcpcp-tea-0.7.0/docs/install.rst
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2019-08-30 02:25:03.000000 django-htcpcp-tea-0.7.0/django_htcpcp_tea/
--rw-rw-r--   0 brian     (1000) brian     (1000)     7375 2019-07-05 13:07:23.000000 django-htcpcp-tea-0.7.0/django_htcpcp_tea/admin.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     9900 2019-07-14 17:03:10.000000 django-htcpcp-tea-0.7.0/django_htcpcp_tea/views.py
--rw-rw-r--   0 brian     (1000) brian     (1000)      361 2019-07-11 15:44:49.000000 django-htcpcp-tea-0.7.0/django_htcpcp_tea/apps.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     1170 2019-08-30 02:21:23.000000 django-htcpcp-tea-0.7.0/django_htcpcp_tea/settings.py
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2019-08-30 02:25:03.000000 django-htcpcp-tea-0.7.0/django_htcpcp_tea/fixtures/
--rw-rw-r--   0 brian     (1000) brian     (1000)      687 2019-07-08 15:32:37.000000 django-htcpcp-tea-0.7.0/django_htcpcp_tea/fixtures/demo_pots.json
--rw-rw-r--   0 brian     (1000) brian     (1000)      314 2019-07-05 01:29:03.000000 django-htcpcp-tea-0.7.0/django_htcpcp_tea/fixtures/rfc_7168_teas.json
--rw-rw-r--   0 brian     (1000) brian     (1000)      962 2019-07-05 13:07:23.000000 django-htcpcp-tea-0.7.0/django_htcpcp_tea/fixtures/demo_forbidden_combinations.json
--rw-rw-r--   0 brian     (1000) brian     (1000)      289 2019-07-05 01:29:03.000000 django-htcpcp-tea-0.7.0/django_htcpcp_tea/fixtures/rfc_7168_additions.json
--rw-rw-r--   0 brian     (1000) brian     (1000)     1354 2019-07-05 01:29:03.000000 django-htcpcp-tea-0.7.0/django_htcpcp_tea/fixtures/rfc_2324_additions.json
--rw-rw-r--   0 brian     (1000) brian     (1000)     2865 2019-08-30 02:21:23.000000 django-htcpcp-tea-0.7.0/django_htcpcp_tea/middleware.py
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2019-08-30 02:25:03.000000 django-htcpcp-tea-0.7.0/django_htcpcp_tea/templates/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2019-08-30 02:25:03.000000 django-htcpcp-tea-0.7.0/django_htcpcp_tea/templates/django_htcpcp_tea/
--rw-rw-r--   0 brian     (1000) brian     (1000)      179 2019-07-05 01:29:03.000000 django-htcpcp-tea-0.7.0/django_htcpcp_tea/templates/django_htcpcp_tea/base_error.html
--rw-rw-r--   0 brian     (1000) brian     (1000)      497 2019-07-05 01:29:03.000000 django-htcpcp-tea-0.7.0/django_htcpcp_tea/templates/django_htcpcp_tea/406.html
--rw-rw-r--   0 brian     (1000) brian     (1000)      522 2019-07-05 13:07:23.000000 django-htcpcp-tea-0.7.0/django_htcpcp_tea/templates/django_htcpcp_tea/403.html
--rw-rw-r--   0 brian     (1000) brian     (1000)      258 2019-07-05 01:29:03.000000 django-htcpcp-tea-0.7.0/django_htcpcp_tea/templates/django_htcpcp_tea/400.html
--rw-rw-r--   0 brian     (1000) brian     (1000)      181 2019-07-05 01:29:03.000000 django-htcpcp-tea-0.7.0/django_htcpcp_tea/templates/django_htcpcp_tea/503.html
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2019-08-30 02:25:03.000000 django-htcpcp-tea-0.7.0/django_htcpcp_tea/templates/django_htcpcp_tea/includes/
--rw-rw-r--   0 brian     (1000) brian     (1000)      389 2019-07-05 01:29:03.000000 django-htcpcp-tea-0.7.0/django_htcpcp_tea/templates/django_htcpcp_tea/includes/additions.html
--rw-rw-r--   0 brian     (1000) brian     (1000)      170 2019-07-05 01:29:03.000000 django-htcpcp-tea-0.7.0/django_htcpcp_tea/templates/django_htcpcp_tea/includes/alternatives.html
--rw-rw-r--   0 brian     (1000) brian     (1000)      182 2019-07-05 01:29:03.000000 django-htcpcp-tea-0.7.0/django_htcpcp_tea/templates/django_htcpcp_tea/options.html
--rw-rw-r--   0 brian     (1000) brian     (1000)      148 2019-07-05 01:29:03.000000 django-htcpcp-tea-0.7.0/django_htcpcp_tea/templates/django_htcpcp_tea/pouring.html
--rw-rw-r--   0 brian     (1000) brian     (1000)      584 2019-07-05 01:29:03.000000 django-htcpcp-tea-0.7.0/django_htcpcp_tea/templates/django_htcpcp_tea/brewing.html
--rw-rw-r--   0 brian     (1000) brian     (1000)       44 2019-07-05 01:29:03.000000 django-htcpcp-tea-0.7.0/django_htcpcp_tea/templates/django_htcpcp_tea/base_beverage.html
--rw-rw-r--   0 brian     (1000) brian     (1000)      265 2019-07-05 01:29:03.000000 django-htcpcp-tea-0.7.0/django_htcpcp_tea/templates/django_htcpcp_tea/418.html
--rw-rw-r--   0 brian     (1000) brian     (1000)      176 2019-07-05 01:21:10.000000 django-htcpcp-tea-0.7.0/django_htcpcp_tea/templates/django_htcpcp_tea/base.html
--rw-rw-r--   0 brian     (1000) brian     (1000)      375 2019-07-05 01:29:03.000000 django-htcpcp-tea-0.7.0/django_htcpcp_tea/templates/django_htcpcp_tea/finished.html
--rw-rw-r--   0 brian     (1000) brian     (1000)      306 2019-08-30 02:21:37.000000 django-htcpcp-tea-0.7.0/django_htcpcp_tea/__init__.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     2708 2019-07-14 17:03:10.000000 django-htcpcp-tea-0.7.0/django_htcpcp_tea/utils.py
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2019-08-30 02:25:03.000000 django-htcpcp-tea-0.7.0/django_htcpcp_tea/migrations/
--rw-rw-r--   0 brian     (1000) brian     (1000)     1429 2019-07-05 01:21:10.000000 django-htcpcp-tea-0.7.0/django_htcpcp_tea/migrations/0002_auto_20190619_1041.py
--rw-rw-r--   0 brian     (1000) brian     (1000)      448 2019-07-05 01:21:10.000000 django-htcpcp-tea-0.7.0/django_htcpcp_tea/migrations/0003_auto_20190620_1205.py
--rw-rw-r--   0 brian     (1000) brian     (1000)      990 2019-07-05 13:07:23.000000 django-htcpcp-tea-0.7.0/django_htcpcp_tea/migrations/0005_forbiddencombination.py
--rw-rw-r--   0 brian     (1000) brian     (1000)      615 2019-07-05 01:21:10.000000 django-htcpcp-tea-0.7.0/django_htcpcp_tea/migrations/0004_addition_type.py
--rw-rw-r--   0 brian     (1000) brian     (1000)        0 2019-07-05 01:21:10.000000 django-htcpcp-tea-0.7.0/django_htcpcp_tea/migrations/__init__.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     1461 2019-07-05 01:21:10.000000 django-htcpcp-tea-0.7.0/django_htcpcp_tea/migrations/0001_initial.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     1695 2019-07-14 17:03:10.000000 django-htcpcp-tea-0.7.0/django_htcpcp_tea/decorators.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     5735 2019-07-08 15:32:37.000000 django-htcpcp-tea-0.7.0/django_htcpcp_tea/models.py
--rw-rw-r--   0 brian     (1000) brian     (1000)      498 2019-07-11 23:07:09.000000 django-htcpcp-tea-0.7.0/django_htcpcp_tea/urls.py
--rw-rw-r--   0 brian     (1000) brian     (1000)       38 2019-08-30 02:25:03.000000 django-htcpcp-tea-0.7.0/setup.cfg
--rw-rw-r--   0 brian     (1000) brian     (1000)    10445 2019-08-30 02:25:03.000000 django-htcpcp-tea-0.7.0/PKG-INFO
--rw-rw-r--   0 brian     (1000) brian     (1000)      230 2019-07-05 01:29:03.000000 django-htcpcp-tea-0.7.0/MANIFEST.in
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2019-08-30 02:25:03.000000 django-htcpcp-tea-0.7.0/django_htcpcp_tea.egg-info/
--rw-rw-r--   0 brian     (1000) brian     (1000)       12 2019-08-30 02:25:03.000000 django-htcpcp-tea-0.7.0/django_htcpcp_tea.egg-info/requires.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)    10445 2019-08-30 02:25:03.000000 django-htcpcp-tea-0.7.0/django_htcpcp_tea.egg-info/PKG-INFO
--rw-rw-r--   0 brian     (1000) brian     (1000)     2131 2019-08-30 02:25:03.000000 django-htcpcp-tea-0.7.0/django_htcpcp_tea.egg-info/SOURCES.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)        1 2019-08-30 02:25:03.000000 django-htcpcp-tea-0.7.0/django_htcpcp_tea.egg-info/dependency_links.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)       18 2019-08-30 02:25:03.000000 django-htcpcp-tea-0.7.0/django_htcpcp_tea.egg-info/top_level.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)     2061 2019-08-30 02:22:48.000000 django-htcpcp-tea-0.7.0/setup.py
--rwxrwxr-x   0 brian     (1000) brian     (1000)     1071 2019-07-05 01:21:10.000000 django-htcpcp-tea-0.7.0/LICENSE
--rw-rw-r--   0 brian     (1000) brian     (1000)     3031 2019-08-30 02:21:23.000000 django-htcpcp-tea-0.7.0/README.rst
+-rw-r--r--   0        0        0     4294 2023-07-17 17:49:14.283743 django_htcpcp_tea-0.8.0/CHANGELOG.rst
+-rwxr-xr-x   0        0        0     1071 2019-07-05 01:21:10.480690 django_htcpcp_tea-0.8.0/LICENSE
+-rw-r--r--   0        0        0     3031 2019-08-30 02:21:23.636411 django_htcpcp_tea-0.8.0/README.rst
+-rw-r--r--   0        0        0      306 2023-07-17 17:49:14.283743 django_htcpcp_tea-0.8.0/django_htcpcp_tea/__init__.py
+-rw-r--r--   0        0        0     7598 2023-07-17 17:48:53.536061 django_htcpcp_tea-0.8.0/django_htcpcp_tea/admin.py
+-rw-r--r--   0        0        0      361 2023-07-17 17:48:53.536061 django_htcpcp_tea-0.8.0/django_htcpcp_tea/apps.py
+-rw-r--r--   0        0        0     1695 2023-07-17 17:48:53.536061 django_htcpcp_tea-0.8.0/django_htcpcp_tea/decorators.py
+-rw-r--r--   0        0        0      962 2019-07-05 13:07:23.045128 django_htcpcp_tea-0.8.0/django_htcpcp_tea/fixtures/demo_forbidden_combinations.json
+-rw-r--r--   0        0        0      687 2019-07-08 15:32:37.355564 django_htcpcp_tea-0.8.0/django_htcpcp_tea/fixtures/demo_pots.json
+-rw-r--r--   0        0        0     1354 2019-07-05 01:29:03.962812 django_htcpcp_tea-0.8.0/django_htcpcp_tea/fixtures/rfc_2324_additions.json
+-rw-r--r--   0        0        0      289 2019-07-05 01:29:03.962812 django_htcpcp_tea-0.8.0/django_htcpcp_tea/fixtures/rfc_7168_additions.json
+-rw-r--r--   0        0        0      314 2019-07-05 01:29:03.962812 django_htcpcp_tea-0.8.0/django_htcpcp_tea/fixtures/rfc_7168_teas.json
+-rw-r--r--   0        0        0     2925 2023-07-17 17:48:53.536061 django_htcpcp_tea-0.8.0/django_htcpcp_tea/middleware.py
+-rw-r--r--   0        0        0     1461 2023-07-17 16:59:39.561974 django_htcpcp_tea-0.8.0/django_htcpcp_tea/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1429 2023-07-17 16:59:39.561974 django_htcpcp_tea-0.8.0/django_htcpcp_tea/migrations/0002_auto_20190619_1041.py
+-rw-r--r--   0        0        0      448 2023-07-17 16:59:39.561974 django_htcpcp_tea-0.8.0/django_htcpcp_tea/migrations/0003_auto_20190620_1205.py
+-rw-r--r--   0        0        0      615 2023-07-17 16:59:39.561974 django_htcpcp_tea-0.8.0/django_htcpcp_tea/migrations/0004_addition_type.py
+-rw-r--r--   0        0        0      990 2023-07-17 17:02:49.590597 django_htcpcp_tea-0.8.0/django_htcpcp_tea/migrations/0005_forbiddencombination.py
+-rw-r--r--   0        0        0        0 2019-07-05 01:21:10.480690 django_htcpcp_tea-0.8.0/django_htcpcp_tea/migrations/__init__.py
+-rw-r--r--   0        0        0     5671 2023-07-17 17:48:53.536061 django_htcpcp_tea-0.8.0/django_htcpcp_tea/models.py
+-rw-r--r--   0        0        0     1229 2023-07-17 17:48:53.536061 django_htcpcp_tea-0.8.0/django_htcpcp_tea/settings.py
+-rw-r--r--   0        0        0      258 2019-07-05 01:29:03.962812 django_htcpcp_tea-0.8.0/django_htcpcp_tea/templates/django_htcpcp_tea/400.html
+-rw-r--r--   0        0        0      522 2019-07-05 13:07:23.045128 django_htcpcp_tea-0.8.0/django_htcpcp_tea/templates/django_htcpcp_tea/403.html
+-rw-r--r--   0        0        0      497 2019-07-05 01:29:03.962812 django_htcpcp_tea-0.8.0/django_htcpcp_tea/templates/django_htcpcp_tea/406.html
+-rw-r--r--   0        0        0      265 2019-07-05 01:29:03.962812 django_htcpcp_tea-0.8.0/django_htcpcp_tea/templates/django_htcpcp_tea/418.html
+-rw-r--r--   0        0        0      181 2019-07-05 01:29:03.962812 django_htcpcp_tea-0.8.0/django_htcpcp_tea/templates/django_htcpcp_tea/503.html
+-rw-r--r--   0        0        0      176 2019-07-05 01:21:10.480690 django_htcpcp_tea-0.8.0/django_htcpcp_tea/templates/django_htcpcp_tea/base.html
+-rw-r--r--   0        0        0       44 2019-07-05 01:29:03.962812 django_htcpcp_tea-0.8.0/django_htcpcp_tea/templates/django_htcpcp_tea/base_beverage.html
+-rw-r--r--   0        0        0      179 2019-07-05 01:29:03.962812 django_htcpcp_tea-0.8.0/django_htcpcp_tea/templates/django_htcpcp_tea/base_error.html
+-rw-r--r--   0        0        0      584 2019-07-05 01:29:03.962812 django_htcpcp_tea-0.8.0/django_htcpcp_tea/templates/django_htcpcp_tea/brewing.html
+-rw-r--r--   0        0        0      375 2019-07-05 01:29:03.962812 django_htcpcp_tea-0.8.0/django_htcpcp_tea/templates/django_htcpcp_tea/finished.html
+-rw-r--r--   0        0        0      389 2019-07-05 01:29:03.962812 django_htcpcp_tea-0.8.0/django_htcpcp_tea/templates/django_htcpcp_tea/includes/additions.html
+-rw-r--r--   0        0        0      170 2019-07-05 01:29:03.962812 django_htcpcp_tea-0.8.0/django_htcpcp_tea/templates/django_htcpcp_tea/includes/alternatives.html
+-rw-r--r--   0        0        0      182 2019-07-05 01:29:03.962812 django_htcpcp_tea-0.8.0/django_htcpcp_tea/templates/django_htcpcp_tea/options.html
+-rw-r--r--   0        0        0      148 2019-07-05 01:29:03.962812 django_htcpcp_tea-0.8.0/django_htcpcp_tea/templates/django_htcpcp_tea/pouring.html
+-rw-r--r--   0        0        0      498 2023-07-17 17:48:53.536061 django_htcpcp_tea-0.8.0/django_htcpcp_tea/urls.py
+-rw-r--r--   0        0        0     2690 2023-07-17 17:48:53.536061 django_htcpcp_tea-0.8.0/django_htcpcp_tea/utils.py
+-rw-r--r--   0        0        0    10719 2023-07-17 17:48:53.536061 django_htcpcp_tea-0.8.0/django_htcpcp_tea/views.py
+-rw-r--r--   0        0        0      580 2019-07-05 01:29:03.962812 django_htcpcp_tea-0.8.0/docs/Makefile
+-rw-r--r--   0        0        0        0 2019-07-05 01:29:03.962812 django_htcpcp_tea-0.8.0/docs/_static/.gitkeep
+-rw-r--r--   0        0        0        0 2019-07-05 01:29:03.962812 django_htcpcp_tea-0.8.0/docs/_templates/.gitkeep
+-rw-r--r--   0        0        0     2264 2019-08-30 02:21:23.640411 django_htcpcp_tea-0.8.0/docs/api.rst
+-rw-r--r--   0        0        0      212 2019-07-14 17:03:10.222453 django_htcpcp_tea-0.8.0/docs/changelog.rst
+-rw-r--r--   0        0        0     2120 2023-07-17 17:49:14.283743 django_htcpcp_tea-0.8.0/docs/conf.py
+-rw-r--r--   0        0        0    12177 2019-08-30 02:21:23.640411 django_htcpcp_tea-0.8.0/docs/config.rst
+-rw-r--r--   0        0        0    12979 2023-07-17 17:48:53.536061 django_htcpcp_tea-0.8.0/docs/examples.rst
+-rw-r--r--   0        0        0      596 2019-08-30 02:21:23.640411 django_htcpcp_tea-0.8.0/docs/index.rst
+-rw-r--r--   0        0        0     4852 2019-10-06 23:18:06.797581 django_htcpcp_tea-0.8.0/docs/install.rst
+-rw-r--r--   0        0        0      752 2019-07-05 01:29:03.962812 django_htcpcp_tea-0.8.0/docs/make.bat
+-rw-r--r--   0        0        0       12 2019-07-14 17:03:10.222453 django_htcpcp_tea-0.8.0/docs/requirements.txt
+-rw-r--r--   0        0        0     1864 2023-07-17 17:49:14.283743 django_htcpcp_tea-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     8636 1970-01-01 00:00:00.000000 django_htcpcp_tea-0.8.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-htcpcp-tea-0.7.0/docs/examples.rst` & `django_htcpcp_tea-0.8.0/docs/examples.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 .. This file is distributed under the MIT License. If a copy of the
 .. MIT License was not distributed with this file, you can obtain one
 .. at https://opensource.org/licenses/MIT.
 
 Examples
 ========
 
+.. warning::
+
+    This documentation has not been updated since 2019.
+
 This document highlights the basic usage of Django HTCPCP-TEA by interacting with it over a command line interface. It is worth noting that since Django HTCPCP-TEA simulates an HTTP extension, there are many other ways to use it beyond a CLI.
 
 In these examples, I will be using the GNU `netcat`_ utility to transmit HTTP requests. Netcat is available for most Unix systems, including MacOS and Linux. Similar utilities are also available for Windows systems.
 
 .. _netcat: http://netcat.sourceforge.net/
 
 For the sake of brevity, this document assumes that you have already installed Django HTCPCP-TEA will the "Schema Compliant" URL configuration (see :ref:`install-schema-compliant`). If you want to follow these examples for with "Standard" installation, add the appropriate prefix to the request line's URI in each HTCPCP request.
```

#### html2text {}

```diff
@@ -1,38 +1,39 @@
 .. This file is distributed under the MIT License. If a copy of the .. MIT
 License was not distributed with this file, you can obtain one .. at https://
-opensource.org/licenses/MIT. Examples ======== This document highlights the
-basic usage of Django HTCPCP-TEA by interacting with it over a command line
-interface. It is worth noting that since Django HTCPCP-TEA simulates an HTTP
-extension, there are many other ways to use it beyond a CLI. In these examples,
-I will be using the GNU `netcat`_ utility to transmit HTTP requests. Netcat is
-available for most Unix systems, including MacOS and Linux. Similar utilities
-are also available for Windows systems. .. _netcat: http://
-netcat.sourceforge.net/ For the sake of brevity, this document assumes that you
-have already installed Django HTCPCP-TEA will the "Schema Compliant" URL
-configuration (see :ref:`install-schema-compliant`). If you want to follow
-these examples for with "Standard" installation, add the appropriate prefix to
-the request line's URI in each HTCPCP request. .. note:: These examples
-interact with a locally run instance of the `Django testing server`_ located at
-``example.localhost:8080``. To duplicate this setup, add ``example.localhost``
-as a loopback address on your system. On Unix systems, this can be accomplished
-by adding:: 127.0.0.1 example.localhost to your ``/etc/hosts`` file. Then, run
-the following command from your Django project's root: .. code-block:: console
-$ ./manage.py runserver example.localhost:8080 .. _Django testing server:
-https://docs.djangoproject.com/en/2.2/ref/django-admin/#runserver Basic HTCPCP
------------- The simplest way to use Django HTCPCP-TEA is with pot sessions
-disabled. If you have set the ``HTCPCP_POT_SESSION`` setting to ``False``,
-Django HTCPCP-TEA will not try to keep track of your transaction history with
-the servers pots, so you do not have to worry about keeping track of a session
-id. Let's begin using Django HTCPCP-TEA in this capacity by creating a file
-named ``request.http`` with the following contents: .. code-block:: http BREW /
-HTTP/1.1 Host: example.localhost Content-Type: message/coffeepot Content-
-Length: 5 start .. note:: The HTCPCP request listed above uses the ``BREW``
-request method from the HTCPCP standard. If this method is not available to you
-in your HTTP client, the ``POST`` method can be used in place with no loss of
+opensource.org/licenses/MIT. Examples ======== .. warning:: This documentation
+has not been updated since 2019. This document highlights the basic usage of
+Django HTCPCP-TEA by interacting with it over a command line interface. It is
+worth noting that since Django HTCPCP-TEA simulates an HTTP extension, there
+are many other ways to use it beyond a CLI. In these examples, I will be using
+the GNU `netcat`_ utility to transmit HTTP requests. Netcat is available for
+most Unix systems, including MacOS and Linux. Similar utilities are also
+available for Windows systems. .. _netcat: http://netcat.sourceforge.net/ For
+the sake of brevity, this document assumes that you have already installed
+Django HTCPCP-TEA will the "Schema Compliant" URL configuration (see :ref:
+`install-schema-compliant`). If you want to follow these examples for with
+"Standard" installation, add the appropriate prefix to the request line's URI
+in each HTCPCP request. .. note:: These examples interact with a locally run
+instance of the `Django testing server`_ located at ``example.localhost:8080``.
+To duplicate this setup, add ``example.localhost`` as a loopback address on
+your system. On Unix systems, this can be accomplished by adding:: 127.0.0.1
+example.localhost to your ``/etc/hosts`` file. Then, run the following command
+from your Django project's root: .. code-block:: console $ ./manage.py
+runserver example.localhost:8080 .. _Django testing server: https://
+docs.djangoproject.com/en/2.2/ref/django-admin/#runserver Basic HTCPCP --------
+---- The simplest way to use Django HTCPCP-TEA is with pot sessions disabled.
+If you have set the ``HTCPCP_POT_SESSION`` setting to ``False``, Django HTCPCP-
+TEA will not try to keep track of your transaction history with the servers
+pots, so you do not have to worry about keeping track of a session id. Let's
+begin using Django HTCPCP-TEA in this capacity by creating a file named
+``request.http`` with the following contents: .. code-block:: http BREW / HTTP/
+1.1 Host: example.localhost Content-Type: message/coffeepot Content-Length: 5
+start .. note:: The HTCPCP request listed above uses the ``BREW`` request
+method from the HTCPCP standard. If this method is not available to you in your
+HTTP client, the ``POST`` method can be used in place with no loss of
 functionality. This is a simple HTCPCP request that will prompt the server to
 return a list of available beverages. To the untrained eye, this file will look
 like an ordinary HTTP request: it has a well-formed request line, a Host
 header, and some entity body. A closer look, however, makes it clear that this
 request makes us of some unconventional HTTP. Most notably, the request method,
 found at the beginning of the request line, is ``BREW`` (not a particular
 common HTTP verb). Moreover, the content type is the HTCPCP specialize
```

### Comparing `django-htcpcp-tea-0.7.0/docs/config.rst` & `django_htcpcp_tea-0.8.0/docs/config.rst`

 * *Files identical despite different names*

### Comparing `django-htcpcp-tea-0.7.0/docs/conf.py` & `django_htcpcp_tea-0.8.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # -- Project information -----------------------------------------------------
 
 project = 'django-htcpcp-tea'
 copyright = '2019, Brian Schubert'
 author = 'Brian Schubert'
 
 # The full version, including alpha/beta/rc tags
-release = '0.7.0'
+release = '0.8.0'
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `django-htcpcp-tea-0.7.0/docs/index.rst` & `django_htcpcp_tea-0.8.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django-htcpcp-tea-0.7.0/docs/make.bat` & `django_htcpcp_tea-0.8.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-htcpcp-tea-0.7.0/docs/api.rst` & `django_htcpcp_tea-0.8.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `django-htcpcp-tea-0.7.0/docs/Makefile` & `django_htcpcp_tea-0.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-htcpcp-tea-0.7.0/docs/install.rst` & `django_htcpcp_tea-0.8.0/docs/install.rst`

 * *Files identical despite different names*

### Comparing `django-htcpcp-tea-0.7.0/django_htcpcp_tea/admin.py` & `django_htcpcp_tea-0.8.0/django_htcpcp_tea/admin.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,107 +9,121 @@
 from django.db import models
 
 from .models import Addition, ForbiddenCombination, Pot, TeaType
 
 
 class RelatedItemsExistsListFilter(admin.SimpleListFilter):
     """Admin list filter for whether an object has a ManyToMany related item."""
+
     related_item_field = None
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         if not self.related_item_field:
-            error_msg = 'The list filter {} does not specify a related_item_field'
+            error_msg = "The list filter {} does not specify a related_item_field"
             raise ImproperlyConfigured(error_msg.format(self.__class__.__name__))
 
     def lookups(self, request, model_admin):
         return (
-            ('y', 'Yes'),
-            ('n', 'No'),
+            ("y", "Yes"),
+            ("n", "No"),
         )
 
     def queryset(self, request, queryset):
         value = self.value()
-        lookup_param = '{}__isnull'.format(self.related_item_field)
+        lookup_param = "{}__isnull".format(self.related_item_field)
 
-        if value == 'y':
+        if value == "y":
             return queryset.filter(**{lookup_param: False})
 
-        if value == 'n':
+        if value == "n":
             return queryset.filter(**{lookup_param: True})
 
 
 class BrewTeaListFilter(RelatedItemsExistsListFilter):
     """Admin list filter for whether a pots serves any teas."""
-    title = 'able to brew tea'
 
-    parameter_name = 'brew_tea'
+    title = "able to brew tea"
+
+    parameter_name = "brew_tea"
 
-    related_item_field = 'supported_teas'
+    related_item_field = "supported_teas"
 
 
 class ServedByAPotListFilter(RelatedItemsExistsListFilter):
     """Admin list filter for whether an object is served by a pot."""
-    title = 'served by a pot'
 
-    parameter_name = 'is_served'
+    title = "served by a pot"
 
-    related_item_field = 'pot_list'
+    parameter_name = "is_served"
+
+    related_item_field = "pot_list"
 
 
 class SomeCombinationsForbiddenListFilter(RelatedItemsExistsListFilter):
-    title = 'has forbidden combinations'
+    title = "has forbidden combinations"
 
-    parameter_name = 'has_restrictions'
+    parameter_name = "has_restrictions"
 
-    related_item_field = 'forbidden_combinations'
+    related_item_field = "forbidden_combinations"
 
 
 @admin.register(Pot)
 class PotAdmin(admin.ModelAdmin):
-    search_fields = ('supported_teas__name', 'supported_additions__name')
+    search_fields = ("supported_teas__name", "supported_additions__name")
 
-    fields = (('name', 'brew_coffee'), 'supported_teas', 'supported_additions')
+    fields = (("name", "brew_coffee"), "supported_teas", "supported_additions")
 
-    list_display = ('id', 'name', 'brew_coffee', 'tea_capable_view', 'tea_count_view', 'addition_count_view')
+    list_display = (
+        "id",
+        "name",
+        "brew_coffee",
+        "tea_capable_view",
+        "tea_count_view",
+        "addition_count_view",
+    )
 
-    list_display_links = ('id', 'name')
+    list_display_links = ("id", "name")
 
-    filter_horizontal = ('supported_teas', 'supported_additions')
+    filter_horizontal = ("supported_teas", "supported_additions")
 
-    list_filter = ('brew_coffee', BrewTeaListFilter, ('supported_teas', admin.RelatedOnlyFieldListFilter))
+    list_filter = (
+        "brew_coffee",
+        BrewTeaListFilter,
+        ("supported_teas", admin.RelatedOnlyFieldListFilter),
+    )
 
     save_as = True
 
     def tea_capable_view(self, obj):
         """Display whether the given pot can brew tea."""
         return obj.tea_capable
 
     tea_capable_view.boolean = True
     tea_capable_view.short_description = "able to brew tea"
-    tea_capable_view.admin_order_field = 'supported_teas'
+    tea_capable_view.admin_order_field = "supported_teas"
 
     def tea_count_view(self, obj):
         "Display the number of tea types that the given pot supports."
         return obj.tea_count
 
-    tea_count_view.admin_order_field = 'tea_count'
-    tea_count_view.short_description = 'supported teas'
+    tea_count_view.admin_order_field = "tea_count"
+    tea_count_view.short_description = "supported teas"
 
     def addition_count_view(self, obj):
         "Display the number of addition types that the given pot supports."
         return obj.addition_count
 
-    addition_count_view.admin_order_field = 'addition_count'
-    addition_count_view.short_description = 'supported additions'
+    addition_count_view.admin_order_field = "addition_count"
+    addition_count_view.short_description = "supported additions"
 
     def get_queryset(self, request):
         queryset = super().get_queryset(request)
-        queryset = queryset.prefetch_related('supported_teas')
-        queryset = queryset.prefetch_related('supported_additions')
+        queryset = queryset.prefetch_related("supported_teas")
+        queryset = queryset.prefetch_related("supported_additions")
         return queryset.with_tea_count().with_addition_count()
 
 
 class PotsServingMixin:
     """
     Mixin to add a 'pots serving' item to a model admin's list_display
     and list_filter
@@ -125,20 +139,22 @@
     def get_list_filter(self, request):
         return (ServedByAPotListFilter,) + super().get_list_filter(request)
 
     def pots_serving_count_view(self, obj):
         """Display the number of pots that serve the given object."""
         return obj.pot_count
 
-    pots_serving_count_view.admin_order_field = 'pot_count'
-    pots_serving_count_view.short_description = 'pots serving'
+    pots_serving_count_view.admin_order_field = "pot_count"
+    pots_serving_count_view.short_description = "pots serving"
 
     def get_queryset(self, request):
-        return super().get_queryset(request).annotate(
-            pot_count=models.Count('pot_list', distinct=True)
+        return (
+            super()
+            .get_queryset(request)
+            .annotate(pot_count=models.Count("pot_list", distinct=True))
         )
 
 
 class HasForbiddenCombinationsMixin:
     """
     Mixin to add a 'forbidden combinations' item to a model admin's
     list_display and list_filter.
@@ -157,81 +173,89 @@
     def forbidden_combination_count_view(self, obj):
         """
         Display the number of forbidden combinations that include the
         given object.
         """
         return obj.forbidden_count
 
-    forbidden_combination_count_view.admin_order_field = 'forbidden_count'
-    forbidden_combination_count_view.short_description = 'forbidden combinations'
+    forbidden_combination_count_view.admin_order_field = "forbidden_count"
+    forbidden_combination_count_view.short_description = "forbidden combinations"
 
     def get_queryset(self, request):
-        return super().get_queryset(request).annotate(
-            forbidden_count=models.Count('forbidden_combinations', distinct=True)
+        return (
+            super()
+            .get_queryset(request)
+            .annotate(
+                forbidden_count=models.Count("forbidden_combinations", distinct=True)
+            )
         )
 
 
 class ForbiddenCombinationInline(admin.TabularInline):
     model = ForbiddenCombination
 
-    fields = ('reason', 'additions')
+    fields = ("reason", "additions")
 
     extra = 0
 
-    filter_horizontal = ('additions',)
+    filter_horizontal = ("additions",)
 
-    classes = ('collapse',)
+    classes = ("collapse",)
 
     def get_queryset(self, request):
         queryset = super().get_queryset(request)
-        return queryset.select_related('tea').prefetch_related('additions')
+        return queryset.select_related("tea").prefetch_related("additions")
 
 
 @admin.register(TeaType)
 class TeaTypeAdmin(PotsServingMixin, HasForbiddenCombinationsMixin, admin.ModelAdmin):
     inlines = (ForbiddenCombinationInline,)
 
-    search_fields = ('name',)
+    search_fields = ("name",)
 
-    prepopulated_fields = {'slug': ('name',)}
+    prepopulated_fields = {"slug": ("name",)}
 
     fieldsets = (
-        (None, {
-            'fields': ('name',)
-        }),
-        ('Advanced', {
-            'classes': ('collapse',),
-            'fields': ('slug',),
-        }),
+        (None, {"fields": ("name",)}),
+        (
+            "Advanced",
+            {
+                "classes": ("collapse",),
+                "fields": ("slug",),
+            },
+        ),
     )
 
 
 @admin.register(Addition)
 class AdditionAdmin(PotsServingMixin, HasForbiddenCombinationsMixin, admin.ModelAdmin):
-    search_fields = ('name',)
+    search_fields = ("name",)
 
-    list_display = ('name', 'type')
+    list_display = ("name", "type")
 
-    list_filter = ('type',)
+    list_filter = ("type",)
 
-    radio_fields = {'type': admin.HORIZONTAL}
+    radio_fields = {"type": admin.HORIZONTAL}
 
 
 @admin.register(ForbiddenCombination)
 class ForbiddenCombinationAdmin(admin.ModelAdmin):
-    list_display = ('__str__', 'reason')
+    list_display = ("__str__", "reason")
 
-    search_fields = ('additions__name', 'tea__name')
+    search_fields = ("additions__name", "tea__name")
 
-    list_filter = (('tea', admin.RelatedOnlyFieldListFilter), ('additions', admin.RelatedOnlyFieldListFilter))
+    list_filter = (
+        ("tea", admin.RelatedOnlyFieldListFilter),
+        ("additions", admin.RelatedOnlyFieldListFilter),
+    )
 
-    filter_horizontal = ('additions',)
+    filter_horizontal = ("additions",)
 
     save_as = True
 
     formfield_overrides = {
-        models.ForeignKey: {'empty_label': '------ All ------'},
+        models.ForeignKey: {"empty_label": "------ All ------"},
     }
 
     def get_queryset(self, request):
         queryset = super().get_queryset(request)
-        return queryset.select_related('tea').prefetch_related('additions')
+        return queryset.select_related("tea").prefetch_related("additions")
```

### Comparing `django-htcpcp-tea-0.7.0/django_htcpcp_tea/views.py` & `django_htcpcp_tea-0.8.0/django_htcpcp_tea/views.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,64 +8,72 @@
 
 from django.shortcuts import get_object_or_404, render
 
 from .decorators import require_htcpcp
 from .models import Addition, Pot
 from .settings import htcpcp_settings
 from .utils import (
-    build_alternates, find_forbidden_combinations, resolve_requested_additions,
+    build_alternates,
+    find_forbidden_combinations,
+    resolve_requested_additions,
 )
 
 
 @require_htcpcp
 def brew_pot(request, pot_designator=None, tea_type=None):
     if not pot_designator:
         alternates = list(build_alternates())
-        context = {'alternatives': alternates}
-        response = render(request, 'django_htcpcp_tea/options.html', context, status=300)
+        context = {"alternatives": alternates}
+        response = render(
+            request, "django_htcpcp_tea/options.html", context, status=300
+        )
         response.htcpcp_alternates = alternates
         return response
 
-    if request.method == 'WHEN' and request.htcpcp_message_type == 'start':
+    if request.method == "WHEN" and request.htcpcp_message_type == "start":
         return render(
             request,
-            'django_htcpcp_tea/400.html',
-            {'error_reason': 'Cannot start a beverage with a WHEN request.'},
-            status=400
+            "django_htcpcp_tea/400.html",
+            {"error_reason": "Cannot start a beverage with a WHEN request."},
+            status=400,
         )
 
     pot = get_object_or_404(Pot, id=pot_designator)
 
     if _request_for_tea(request, tea_type):
         response = _precheck_teapot(request, pot, tea_type)
         # Beverage name only required when starting a new beverage
-        beverage_name = '{} Tea'.format(tea_type.capitalize) if tea_type else None
+        beverage_name = "{} Tea".format(tea_type.capitalize) if tea_type else None
     else:
         response = _precheck_coffee(request, pot)
-        beverage_name = 'coffee'
+        beverage_name = "coffee"
 
     if response is None:
         addition_names = resolve_requested_additions(request)
         try:
             additions = list(pot.fetch_additions(addition_names))
         except Addition.DoesNotExist:
             # Fetch all supported additions for the requested pot.
             # Note that this will result in an additional query.
-            context = {'supported_additions': pot.supported_additions.all()}
-            return render(request, 'django_htcpcp_tea/406.html', context, status=406)
+            context = {"supported_additions": pot.supported_additions.all()}
+            return render(request, "django_htcpcp_tea/406.html", context, status=406)
 
         if htcpcp_settings.CHECK_FORBIDDEN:
             forbidden = find_forbidden_combinations(additions, tea_type)
 
             if forbidden:
-                context = {'matched_combinations': forbidden}
-                return render(request, "django_htcpcp_tea/403.html", context, status=403)
+                context = {"matched_combinations": forbidden}
+                return render(
+                    request, "django_htcpcp_tea/403.html", context, status=403
+                )
 
         if htcpcp_settings.POT_SESSIONS:
-            response = _finalize_beverage_with_session(request, pot, beverage_name, additions)
+            response = _finalize_beverage_with_session(
+                request, pot, beverage_name, additions
+            )
         else:
             response = _finalize_beverage(request, pot, beverage_name, additions)
 
     return response
 
 
 def _request_for_tea(request, tea_type):
@@ -75,162 +83,202 @@
     If the ``STRICT_MIME_TYPE`` settings is enabled, then the MIME type of the
     request is used to unambiguously categorize it as a tea or coffee request.
 
     If strict MIME types are not enforced, the requested beverage type is
     inferred from the existence of a tea type in the request URI and the HTCPCP
     MIME type, if one is provided.
     """
-    if request.content_type == 'message/teapot':
+    if request.content_type == "message/teapot":
         return True
     elif not htcpcp_settings.STRICT_MIME_TYPE:
         return tea_type
     else:
         return False
 
 
 def _precheck_coffee(request, pot):
     """
     Return a response if a precondition for coffee requests is not satisfied,
     else None.
     """
     if pot.is_teapot:
-        return render(request, 'django_htcpcp_tea/418.html', status=418)
+        return render(request, "django_htcpcp_tea/418.html", status=418)
 
     if not pot.brew_coffee:
         return render(
             request,
-            'django_htcpcp_tea/503.html',
-            {'error_reason': 'Pot out of service. No coffee or tea available.'},
+            "django_htcpcp_tea/503.html",
+            {"error_reason": "Pot out of service. No coffee or tea available."},
             status=503,
         )
 
     return None
 
 
 def _precheck_teapot(request, pot, tea):
     """
     Return a response if a precondition for tea requests is not satisfied, else
     None.
     """
-    if request.htcpcp_message_type == 'start':
+    if request.htcpcp_message_type == "start":
         if not tea:  # Require tea type only when starting a new beverage
             alternatives = list(build_alternates(index_pot=pot))
-            context = {'alternatives': alternatives}
-            response = render(request, 'django_htcpcp_tea/options.html', context, status=300)
+            context = {"alternatives": alternatives}
+            response = render(
+                request, "django_htcpcp_tea/options.html", context, status=300
+            )
             response.htcpcp_alternates = alternatives
             return response
-        elif tea not in pot.supported_teas.values_list('slug', flat=True):
+        elif tea not in pot.supported_teas.values_list("slug", flat=True):
             return render(
                 request,
-                'django_htcpcp_tea/503.html',
-                {'error_reason': '{} is not available for this pot'.format(tea.capitalize)},
+                "django_htcpcp_tea/503.html",
+                {
+                    "error_reason": "{} is not available for this pot".format(
+                        tea.capitalize
+                    )
+                },
                 status=503,
             )
     return None
 
 
 def _finalize_beverage(request, pot, beverage_name, additions):
     """
     Return a response to the beverage request according to the HTCPCP standard
     without referencing the user's session.
     """
     context = {
-        'pot': pot,
-        'beverage': beverage_name,
-        'additions': additions,
+        "pot": pot,
+        "beverage": beverage_name,
+        "additions": additions,
     }
 
-    if request.htcpcp_message_type == 'start':
-        if beverage_name == 'coffee':
+    if request.htcpcp_message_type == "start":
+        if beverage_name == "coffee":
             # Display alternatives when brewing coffee per RFC 7168 section 2.1.1
             alternates = list(build_alternates())
-            context['alternatives'] = alternates
-            response = render(request, 'django_htcpcp_tea/brewing.html', context, status=202)  # Accepted
+            context["alternatives"] = alternates
+            response = render(
+                request, "django_htcpcp_tea/brewing.html", context, status=202
+            )  # Accepted
             response.htcpcp_alternates = alternates
         else:
-            response = render(request, 'django_htcpcp_tea/brewing.html', context, status=202)  # Accepted
+            response = render(
+                request, "django_htcpcp_tea/brewing.html", context, status=202
+            )  # Accepted
     else:  # request.htcpcp_message_type == 'stop':
         if any(addition.is_milk for addition in additions):
-            response = render(request, 'django_htcpcp_tea/pouring.html', context, status=200)  # Ok
+            response = render(
+                request, "django_htcpcp_tea/pouring.html", context, status=200
+            )  # Ok
         else:
-            response = render(request, 'django_htcpcp_tea/finished.html', context, status=201)  # Created
+            response = render(
+                request, "django_htcpcp_tea/finished.html", context, status=201
+            )  # Created
 
     return response
 
 
 def _finalize_beverage_with_session(request, pot, beverage_name, additions):
     """
     Return a response to the beverage request according to the HTCPCP standard
     by referencing the current state of the user's session.
     """
-    session_key = 'htcpcp_pot_{}'.format(pot.id)
+    session_key = "htcpcp_pot_{}".format(pot.id)
     pot_status = request.session.get(session_key)
 
     context = {
-        'pot': pot,
-        'beverage': beverage_name,
-        'additions': additions,
+        "pot": pot,
+        "beverage": beverage_name,
+        "additions": additions,
     }
 
     # TODO add brew time and additions display to finished template
 
     if pot_status:
         # 'stop' requests may not be able to reproduce the name of a beverage
         # or the additions that were requested, so override these values in the
         # context with the ones stored in the user's session.
-        context['beverage'] = pot_status['beverage']
-        context['additions'] = pot_status['additions']
+        context["beverage"] = pot_status["beverage"]
+        context["additions"] = pot_status["additions"]
 
-        if request.htcpcp_message_type == 'start':
-            context['error_reason'] = 'Pot is busy and cannot start a new beverage.'
-            response = render(request, 'django_htcpcp_tea/503.html', context, status=503)
+        if request.htcpcp_message_type == "start":
+            context["error_reason"] = "Pot is busy and cannot start a new beverage."
+            response = render(
+                request, "django_htcpcp_tea/503.html", context, status=503
+            )
         else:  # htcpcp_message_type == 'stop'
-            if request.method == 'WHEN':
-                if pot_status['currently_pouring']:
-                    response = render(request, 'django_htcpcp_tea/finished.html', context, status=201)
+            if request.method == "WHEN":
+                if pot_status["currently_pouring"]:
+                    response = render(
+                        request, "django_htcpcp_tea/finished.html", context, status=201
+                    )
                     del request.session[session_key]
                 else:
-                    context['error_reason'] = 'No milk is being poured. Please stop shouting "WHEN!"'
-                    return render(request, 'django_htcpcp_tea/400.html', context, status=400)
+                    context[
+                        "error_reason"
+                    ] = 'No milk is being poured. Please stop shouting "WHEN!"'
+                    return render(
+                        request, "django_htcpcp_tea/400.html", context, status=400
+                    )
             else:
-                if pot_status['currently_pouring']:
-                    context['error_reason'] = 'Milk is currently being poured. Please say "WHEN"'
+                if pot_status["currently_pouring"]:
+                    context[
+                        "error_reason"
+                    ] = 'Milk is currently being poured. Please say "WHEN"'
                     response = render(
-                        request, 'django_htcpcp_tea/400.html', context, status=400)
-                elif pot_status['needs_milk']:  # Stop brewing and begin pouring milk
-                    response = render(request, 'django_htcpcp_tea/pouring.html', context, status=200)
-                    request.session[session_key].update({
-                        'needs_milk': False,
-                        'currently_pouring': True,
-                    })
+                        request, "django_htcpcp_tea/400.html", context, status=400
+                    )
+                elif pot_status["needs_milk"]:  # Stop brewing and begin pouring milk
+                    response = render(
+                        request, "django_htcpcp_tea/pouring.html", context, status=200
+                    )
+                    request.session[session_key].update(
+                        {
+                            "needs_milk": False,
+                            "currently_pouring": True,
+                        }
+                    )
                     request.session.modified = True
                 else:  # Stop brewing. No milk required.
-                    response = render(request, 'django_htcpcp_tea/finished.html', context, status=201)
+                    response = render(
+                        request, "django_htcpcp_tea/finished.html", context, status=201
+                    )
                     del request.session[session_key]
-    elif request.htcpcp_message_type == 'start':
+    elif request.htcpcp_message_type == "start":
         # New session, and the client requested a new beverage
-        if beverage_name == 'coffee':
+        if beverage_name == "coffee":
             # Display alternatives when brewing coffee per RFC 7168 section 2.1.1
-            context['alternatives'] = build_alternates(index_pot=pot)
-        response = render(request, 'django_htcpcp_tea/brewing.html', context, status=202)  # Accepted
+            context["alternatives"] = build_alternates(index_pot=pot)
+        response = render(
+            request, "django_htcpcp_tea/brewing.html", context, status=202
+        )  # Accepted
         request.session[session_key] = {
-            'beverage': beverage_name,
+            "beverage": beverage_name,
             # Serialize the requested additions to as dictionaries for storage
             # in the user's session since we do not need actual Addition objects
             # to display the additions during future requests.
-            'additions': [{'name': a.name, 'get_type_display': a.get_type_display()} for a in additions],
-            'needs_milk': any(addition.is_milk for addition in additions),
-            'currently_pouring': False,
-            'start_time': datetime.utcnow().timestamp()
+            "additions": [
+                {"name": a.name, "get_type_display": a.get_type_display()}
+                for a in additions
+            ],
+            "needs_milk": any(addition.is_milk for addition in additions),
+            "currently_pouring": False,
+            "start_time": datetime.utcnow().timestamp(),
         }
     else:
-        reason = ("No beverage is being brewed by this pot, but the "
-                  "request did not indicate that a new beverage should be "
-                  "brewed")
-        response = render(request, 'django_htcpcp_tea/400.html', {'error_reason': reason}, status=400)
+        reason = (
+            "No beverage is being brewed by this pot, but the "
+            "request did not indicate that a new beverage should be "
+            "brewed"
+        )
+        response = render(
+            request, "django_htcpcp_tea/400.html", {"error_reason": reason}, status=400
+        )
 
     return response
 
 
 if htcpcp_settings.DISABLE_CSRF:
     # Mark the HTCPCP view function as being exempt from the CSRF view
     # protection. This is the same as using the csrf_exempt decorator
```

### Comparing `django-htcpcp-tea-0.7.0/django_htcpcp_tea/settings.py` & `django_htcpcp_tea-0.8.0/django_htcpcp_tea/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,16 +36,19 @@
     USE_SAFE_HEADER_EXT = True
 
     def __init__(self, settings_prefix):
         self.prefix = settings_prefix
 
     def __getattribute__(self, item):
         try:
-            return getattr(django_settings, '{}_{}'.format(
-                object.__getattribute__(self, 'prefix'),
-                item,
-            ))
+            return getattr(
+                django_settings,
+                "{}_{}".format(
+                    object.__getattribute__(self, "prefix"),
+                    item,
+                ),
+            )
         except AttributeError:
             return object.__getattribute__(self, item)
 
 
-htcpcp_settings = _HTCPCPTeaSettings('HTCPCP')
+htcpcp_settings = _HTCPCPTeaSettings("HTCPCP")
```

### Comparing `django-htcpcp-tea-0.7.0/django_htcpcp_tea/fixtures/demo_pots.json` & `django_htcpcp_tea-0.8.0/django_htcpcp_tea/fixtures/demo_pots.json`

 * *Files identical despite different names*

### Comparing `django-htcpcp-tea-0.7.0/django_htcpcp_tea/fixtures/demo_forbidden_combinations.json` & `django_htcpcp_tea-0.8.0/django_htcpcp_tea/fixtures/demo_forbidden_combinations.json`

 * *Files identical despite different names*

### Comparing `django-htcpcp-tea-0.7.0/django_htcpcp_tea/fixtures/rfc_2324_additions.json` & `django_htcpcp_tea-0.8.0/django_htcpcp_tea/fixtures/rfc_2324_additions.json`

 * *Files identical despite different names*

### Comparing `django-htcpcp-tea-0.7.0/django_htcpcp_tea/middleware.py` & `django_htcpcp_tea-0.8.0/django_htcpcp_tea/middleware.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,70 +6,76 @@
 
 from .settings import htcpcp_settings
 from .utils import render_alternates_header
 from .views import brew_pot
 
 
 class HTCPCPTeaMiddleware:
-    HTCPCP_MESSAGE_KEYWORDS = (b'start', b'stop')
+    HTCPCP_MESSAGE_KEYWORDS = (b"start", b"stop")
 
-    HTCPCP_MIME_TYPES = ('message/teapot', 'message/coffeepot')
+    HTCPCP_MIME_TYPES = ("message/teapot", "message/coffeepot")
 
     def __init__(self, get_response):
         self.get_response = get_response
-        self.valid_methods = ('BREW', 'WHEN')
+        self.valid_methods = ("BREW", "WHEN")
         if htcpcp_settings.ALLOW_DEPRECATED_POST:
-            self.valid_methods += ('POST',)
+            self.valid_methods += ("POST",)
 
     def __call__(self, request):
         htcpcp_valid = True
 
         if request.method not in self.valid_methods:
             htcpcp_valid = False
 
         # Resolve HTCPCP message type (start or stop)
         if htcpcp_settings.STRICT_REQUEST_BODY:
             if request.body not in self.HTCPCP_MESSAGE_KEYWORDS:
                 htcpcp_valid = False
             else:
-                request.htcpcp_message_type = request.body.decode(encoding='utf-8')
+                request.htcpcp_message_type = request.body.decode(encoding="utf-8")
         else:
             for keyword in self.HTCPCP_MESSAGE_KEYWORDS:
                 if keyword in request.body:
-                    request.htcpcp_message_type = keyword.decode(encoding='utf-8')
+                    request.htcpcp_message_type = keyword.decode(encoding="utf-8")
                     break  # Trigger else branch if no keyword is found
             else:
                 htcpcp_valid = False
 
-        if (htcpcp_settings.STRICT_MIME_TYPE and
-                request.content_type not in self.HTCPCP_MIME_TYPES):
+        if (
+            htcpcp_settings.STRICT_MIME_TYPE
+            and request.content_type not in self.HTCPCP_MIME_TYPES
+        ):
             htcpcp_valid = False
 
         request.htcpcp_valid = htcpcp_valid
 
-        if (htcpcp_valid and request.path == '/' and
-                htcpcp_settings.OVERRIDE_ROOT_URI and htcpcp_settings.STRICT_MIME_TYPE):
+        if (
+            htcpcp_valid
+            and request.path == "/"
+            and htcpcp_settings.OVERRIDE_ROOT_URI
+            and htcpcp_settings.STRICT_MIME_TYPE
+        ):
             response = brew_pot(request)
         else:
             response = self.get_response(request)
 
         try:
             alternates_pairs = response.htcpcp_alternates
-            response['Alternates'] = render_alternates_header(alternates_pairs)
+            response["Alternates"] = render_alternates_header(alternates_pairs)
         except AttributeError:
             pass
 
         update_server_name = htcpcp_settings.OVERRIDE_SERVER_NAME
         if htcpcp_valid and update_server_name:
             if update_server_name is True:
-                server = request.META.get('SERVER_SOFTWARE')
-                response['Server'] = 'HTCPCP-TEA ' + (server if server else 'Python')
+                server = request.META.get("SERVER_SOFTWARE")
+                response["Server"] = "HTCPCP-TEA " + (server if server else "Python")
             elif callable(update_server_name):
-                response['Server'] = update_server_name(request, response)
+                response["Server"] = update_server_name(request, response)
             else:
-                response['Server'] = update_server_name.format(**request.META)
+                response["Server"] = update_server_name.format(**request.META)
 
         content_type_override = htcpcp_settings.RESPONSE_CONTENT_TYPE
         if htcpcp_valid and content_type_override is not None:
-            response['Content-Type'] = content_type_override
+            response["Content-Type"] = content_type_override
 
         return response
```

### Comparing `django-htcpcp-tea-0.7.0/django_htcpcp_tea/templates/django_htcpcp_tea/403.html` & `django_htcpcp_tea-0.8.0/django_htcpcp_tea/templates/django_htcpcp_tea/403.html`

 * *Files identical despite different names*

### Comparing `django-htcpcp-tea-0.7.0/django_htcpcp_tea/templates/django_htcpcp_tea/brewing.html` & `django_htcpcp_tea-0.8.0/django_htcpcp_tea/templates/django_htcpcp_tea/brewing.html`

 * *Files identical despite different names*

### Comparing `django-htcpcp-tea-0.7.0/django_htcpcp_tea/utils.py` & `django_htcpcp_tea-0.8.0/django_htcpcp_tea/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,46 +15,44 @@
     """
     Generate the Alternates pairs for available beverages, optionally
     for a specific pot.
     """
     if index_pot:
         pots = (index_pot,)
     else:
-        pots = Pot.objects.prefetch_related('supported_teas').all()
+        pots = Pot.objects.prefetch_related("supported_teas").all()
     for pot in pots:
         if pot.brew_coffee:
-            yield (reverse('pot-detail', args=[pot.id]), 'message/coffeepot')
+            yield reverse("pot-detail", args=[pot.id]), "message/coffeepot"
         for tea in pot.supported_teas.all():
-            yield (reverse('pot-detail-tea', args=[pot.id, tea.slug]), 'message/teapot')
+            yield reverse("pot-detail-tea", args=[pot.id, tea.slug]), "message/teapot"
 
 
 def render_alternates_header(alternates_pairs):
     """
     Render (uri, content-type) pairs into an RFC 2295 Alternates header value.
     """
     fmt = '{{"{}" {{type {}}}}}'
-    return ','.join(
-        fmt.format(*pair) for pair in alternates_pairs
-    )
+    return ",".join(fmt.format(*pair) for pair in alternates_pairs)
 
 
 def resolve_requested_additions(request):
     """
     Return the requested additions for the provided request.
 
     Additions may be requested in the ``Accept-Additions`` header field, or
     (if the ``HTCPCP_GET_ADDITIONS`` settings is enabled) in the query string
     of a uri.
 
     Note that the returned additions are not guaranteed to be valid additions
     that are supported by any pot.
     """
     try:
-        header = request.META['HTTP_ACCEPT_ADDITIONS']
-        additions = [addition.strip() for addition in header.split(',')]
+        header = request.META["HTTP_ACCEPT_ADDITIONS"]
+        additions = [addition.strip() for addition in header.split(",")]
     except KeyError:
         additions = []
 
     if htcpcp_settings.GET_ADDITIONS:
         additions += request.GET.dict().keys()
 
     return additions
@@ -66,15 +64,15 @@
     requested additions.
     """
 
     requested_additions = set(requested_additions)
 
     # Calls to ForbiddenCombination.forbids_additions will need the full
     # list of forbidden additions for each retrieved objects.
-    forbidden = ForbiddenCombination.objects.prefetch_related('additions')
+    forbidden = ForbiddenCombination.objects.prefetch_related("additions")
 
     if tea_slug:
         forbidden = forbidden.filter(Q(tea__slug=tea_slug) | Q(tea__isnull=True))
     else:
         forbidden = forbidden.filter(tea__isnull=True)
 
     # Filter ForbiddenCombinations by what additions they forbid in Python
```

### Comparing `django-htcpcp-tea-0.7.0/django_htcpcp_tea/migrations/0002_auto_20190619_1041.py` & `django_htcpcp_tea-0.8.0/django_htcpcp_tea/migrations/0002_auto_20190619_1041.py`

 * *Files identical despite different names*

### Comparing `django-htcpcp-tea-0.7.0/django_htcpcp_tea/migrations/0005_forbiddencombination.py` & `django_htcpcp_tea-0.8.0/django_htcpcp_tea/migrations/0005_forbiddencombination.py`

 * *Files identical despite different names*

### Comparing `django-htcpcp-tea-0.7.0/django_htcpcp_tea/migrations/0004_addition_type.py` & `django_htcpcp_tea-0.8.0/django_htcpcp_tea/migrations/0004_addition_type.py`

 * *Files identical despite different names*

### Comparing `django-htcpcp-tea-0.7.0/django_htcpcp_tea/migrations/0001_initial.py` & `django_htcpcp_tea-0.8.0/django_htcpcp_tea/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-htcpcp-tea-0.7.0/django_htcpcp_tea/decorators.py` & `django_htcpcp_tea-0.8.0/django_htcpcp_tea/decorators.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,30 +30,30 @@
     The decorator will only have effect if the HTCPCP Safe header extension
     option is enabled.
 
     See `RFC 2324 section 2.2.1.1`_ for further details.
 
     .. _RFC 2324 section 2.2.1.1: https://tools.ietf.org/html/rfc2324#section-2.2.1.1
     """
+
     def decorator(func):
         @wraps(func)
         def _wrapped_view(request, *args, **kwargs):
             response = func(request, *args, **kwargs)
             if htcpcp_settings.USE_SAFE_HEADER_EXT:
-                response['Safe'] = 'if-{}'.format(token)
+                response["Safe"] = "if-{}".format(token)
             return response
 
         return _wrapped_view
 
     return decorator
 
 
-safe_require_user_awake = safe_condition('user-awake')
+safe_require_user_awake = safe_condition("user-awake")
 """
 Decorator for adding an "if-user-awake" safe condition to the Safe header
 field.
 
 See `RFC 2324 section 2.2.1.1`_ for further details.
 
 .. _RFC 2324 section 2.2.1.1: https://tools.ietf.org/html/rfc2324#section-2.2.1.1
 """
-
```

### Comparing `django-htcpcp-tea-0.7.0/django_htcpcp_tea/models.py` & `django_htcpcp_tea-0.8.0/django_htcpcp_tea/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,59 +9,54 @@
 from django.db.models import Count
 from django.urls import reverse
 from django.utils.functional import cached_property
 
 
 class PotQuerySet(models.QuerySet):
     def _count_relation(self, field, annotation_name):
-        return self.annotate(**{
-            annotation_name: Count(field, distinct=True)
-        })
+        return self.annotate(**{annotation_name: Count(field, distinct=True)})
 
     def with_tea_count(self):
-        return self._count_relation('supported_teas', 'tea_count')
+        return self._count_relation("supported_teas", "tea_count")
 
     def with_addition_count(self):
-        return self._count_relation('supported_additions', 'addition_count')
+        return self._count_relation("supported_additions", "addition_count")
 
 
 class Pot(models.Model):
     """A Tea- or Coffee Pot capable of brewing a choice beverage."""
+
     name = models.CharField(
         max_length=35,
         unique=True,
         help_text='The name of this pot, e.g. "Joe\'s Joe Jar" or "Breville (R)'
-                  ' BTM800XL"',
+        ' BTM800XL"',
     )
 
     brew_coffee = models.BooleanField(
-        verbose_name='able to brew coffee',
+        verbose_name="able to brew coffee",
         default=True,
         help_text="Can this pot brew coffee?",
     )
 
     supported_teas = models.ManyToManyField(
-        'TeaType',
-        blank=True,
-        related_name='pot_list'
+        "TeaType", blank=True, related_name="pot_list"
     )
 
     supported_additions = models.ManyToManyField(
-        'Addition',
-        blank=True,
-        related_name='pot_list'
+        "Addition", blank=True, related_name="pot_list"
     )
 
     objects = PotQuerySet.as_manager()
 
     def __str__(self):
-        return '{} - {}'.format(self.id, self.name)
+        return "{} - {}".format(self.id, self.name)
 
     def get_absolute_url(self):
-        return reverse('pot-detail', args=(self.pk,))
+        return reverse("pot-detail", args=(self.pk,))
 
     @cached_property
     def tea_capable(self):
         """Return True if this pot can serve tea."""
         return self.supported_teas.exists()
 
     @property
@@ -88,16 +83,17 @@
 
 class TeaType(models.Model):
     """
     A variety of tea that can be brewed by a pot.
 
     Per the HTCPCP standard, tea may be available as tea bags or tea leaves.
     """
+
     name = models.CharField(
-        verbose_name='Tea name',
+        verbose_name="Tea name",
         max_length=35,
         unique=True,
         db_index=True,
     )
 
     slug = models.SlugField(unique=True)
 
@@ -107,27 +103,27 @@
 
 class Addition(models.Model):
     """
     A beverage addition that may be specified in the Accept-Additions header
     field of an HTCPCP request.
     """
 
-    MILK = 'MLK'
+    MILK = "MLK"
 
-    SYRUP = 'SYP'
+    SYRUP = "SYP"
 
-    SWEETENER = 'SWT'
+    SWEETENER = "SWT"
 
-    SPICE = 'SPC'
+    SPICE = "SPC"
 
-    ALCOHOL = 'ACL'
+    ALCOHOL = "ACL"
 
-    SUGAR = 'SUG'
+    SUGAR = "SUG"
 
-    OTHER = 'OTR'
+    OTHER = "OTR"
 
     TYPE_CHOICES = (
         (MILK, "Milk"),
         (SYRUP, "Syrup"),
         (SWEETENER, "Sweetener"),
         (SPICE, "Spice"),
         (ALCOHOL, "Alcohol"),
@@ -135,32 +131,34 @@
         (OTHER, "Other"),
     )
 
     name = models.CharField(
         max_length=35,
         unique=True,
         help_text="The name of this beverage addition as it would appear in the"
-                  " HTCPCP Accept-Additions header field.",
+        " HTCPCP Accept-Additions header field.",
     )
 
     type = models.CharField(
         max_length=3,
         choices=TYPE_CHOICES,
-        verbose_name='Addition type',
+        verbose_name="Addition type",
     )
 
     def clean(self):
         # Calling parent in case it is given a non-empty body in the
         # future (currently it is empty).
         super().clean()
 
-        error_msg = ("Decaffeinated addition not allowed. RFC 2324 specifies "
-                     "no option for decaffeinated coffee. What's the point? ")
+        error_msg = (
+            "Decaffeinated addition not allowed. RFC 2324 specifies "
+            "no option for decaffeinated coffee. What's the point? "
+        )
 
-        if 'decaffeinated' in self.name.lower():
+        if "decaffeinated" in self.name.lower():
             raise ValidationError(error_msg)
 
     def __str__(self):
         return "{} / {}".format(self.get_type_display(), self.name)
 
     @property
     def is_milk(self):
@@ -169,35 +167,35 @@
 
 class ForbiddenCombination(models.Model):
     """
     A combination of additions that is "contrary to the sensibilities of a
     consensus of drinkers", either for a specific variety of tea or for all
     beverages.
     """
+
     tea = models.ForeignKey(
         TeaType,
         null=True,
         blank=True,
         on_delete=models.CASCADE,
-        related_name='forbidden_combinations',
-        help_text=("The type of tea that this forbidden combination applies to."
-                   " Leave blank to apply to all beverages."),
+        related_name="forbidden_combinations",
+        help_text=(
+            "The type of tea that this forbidden combination applies to."
+            " Leave blank to apply to all beverages."
+        ),
     )
 
-    additions = models.ManyToManyField(
-        Addition,
-        related_name='forbidden_combinations'
-    )
+    additions = models.ManyToManyField(Addition, related_name="forbidden_combinations")
 
     reason = models.CharField(max_length=180)
 
     def __str__(self):
-        return '{} / {}'.format(
-            'All' if not self.tea else self.tea.name,
-            ', '.join(a.name for a in self.additions.all())
+        return "{} / {}".format(
+            "All" if not self.tea else self.tea.name,
+            ", ".join(a.name for a in self.additions.all()),
         )
 
     def forbids_additions(self, requested_additions):
         """
         Return True if the combination of additions that this
         ForbiddenCombination prohibits is contained in the specified sequence
         of additions.
```

### Comparing `django-htcpcp-tea-0.7.0/LICENSE` & `django_htcpcp_tea-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-htcpcp-tea-0.7.0/README.rst` & `django_htcpcp_tea-0.8.0/README.rst`

 * *Files identical despite different names*

