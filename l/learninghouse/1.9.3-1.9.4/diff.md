# Comparing `tmp/learninghouse-1.9.3.tar.gz` & `tmp/learninghouse-1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "learninghouse-1.9.3.tar", last modified: Mon Jul 17 12:43:01 2023, max compression
+gzip compressed data, was "learninghouse-1.9.4.tar", last modified: Mon Jul 17 14:43:54 2023, max compression
```

## Comparing `learninghouse-1.9.3.tar` & `learninghouse-1.9.4.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:43:01.162748 learninghouse-1.9.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-17 12:42:49.000000 learninghouse-1.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-17 12:42:47.000000 learninghouse-1.9.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15815 2023-07-17 12:43:01.162748 learninghouse-1.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15012 2023-07-17 12:42:49.000000 learninghouse-1.9.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-07-17 12:42:49.000000 learninghouse-1.9.3/THIRD-PARTY-NOTICES
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:43:01.162748 learninghouse-1.9.3/learninghouse/
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-17 12:42:47.000000 learninghouse-1.9.3/learninghouse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-17 12:42:47.000000 learninghouse-1.9.3/learninghouse/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-17 12:43:01.162748 learninghouse-1.9.3/learninghouse/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:43:01.146748 learninghouse-1.9.3/learninghouse/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-17 12:42:47.000000 learninghouse-1.9.3/learninghouse/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-07-17 12:42:47.000000 learninghouse-1.9.3/learninghouse/api/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-07-17 12:42:47.000000 learninghouse-1.9.3/learninghouse/api/brain.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-17 12:42:47.000000 learninghouse-1.9.3/learninghouse/api/docs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:43:01.146748 learninghouse-1.9.3/learninghouse/api/errors/
--rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-07-17 12:42:47.000000 learninghouse-1.9.3/learninghouse/api/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-07-17 12:42:47.000000 learninghouse-1.9.3/learninghouse/api/errors/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-07-17 12:42:47.000000 learninghouse-1.9.3/learninghouse/api/errors/brain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-17 12:42:47.000000 learninghouse-1.9.3/learninghouse/api/errors/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-07-17 12:42:47.000000 learninghouse-1.9.3/learninghouse/api/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-07-17 12:42:47.000000 learninghouse-1.9.3/learninghouse/api/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-17 12:42:47.000000 learninghouse-1.9.3/learninghouse/api/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:43:01.146748 learninghouse-1.9.3/learninghouse/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 12:42:47.000000 learninghouse-1.9.3/learninghouse/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-07-17 12:42:47.000000 learninghouse-1.9.3/learninghouse/core/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-07-17 12:42:47.000000 learninghouse-1.9.3/learninghouse/core/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:43:01.150748 learninghouse-1.9.3/learninghouse/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-17 12:42:47.000000 learninghouse-1.9.3/learninghouse/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-07-17 12:42:47.000000 learninghouse-1.9.3/learninghouse/models/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-07-17 12:42:47.000000 learninghouse-1.9.3/learninghouse/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13029 2023-07-17 12:42:47.000000 learninghouse-1.9.3/learninghouse/models/brain.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-17 12:42:47.000000 learninghouse-1.9.3/learninghouse/models/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-07-17 12:42:47.000000 learninghouse-1.9.3/learninghouse/models/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-07-17 12:42:47.000000 learninghouse-1.9.3/learninghouse/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:43:01.150748 learninghouse-1.9.3/learninghouse/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 12:42:47.000000 learninghouse-1.9.3/learninghouse/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8901 2023-07-17 12:42:47.000000 learninghouse-1.9.3/learninghouse/services/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-07-17 12:42:47.000000 learninghouse-1.9.3/learninghouse/services/brain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5838 2023-07-17 12:42:47.000000 learninghouse-1.9.3/learninghouse/services/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-17 12:42:47.000000 learninghouse-1.9.3/learninghouse/services/sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:43:01.150748 learninghouse-1.9.3/learninghouse/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:43:01.154748 learninghouse-1.9.3/learninghouse/static/docs/
--rw-r--r--   0 runner    (1001) docker     (123)  1435746 2023-07-17 12:42:47.000000 learninghouse-1.9.3/learninghouse/static/docs/swagger-ui-bundle.js
--rw-r--r--   0 runner    (1001) docker     (123)  2066928 2023-07-17 12:42:47.000000 learninghouse-1.9.3/learninghouse/static/docs/swagger-ui-bundle.js.map
--rw-r--r--   0 runner    (1001) docker     (123)   150945 2023-07-17 12:42:47.000000 learninghouse-1.9.3/learninghouse/static/docs/swagger-ui.css
--rw-r--r--   0 runner    (1001) docker     (123)   260491 2023-07-17 12:42:47.000000 learninghouse-1.9.3/learninghouse/static/docs/swagger-ui.css.map
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-07-17 12:42:47.000000 learninghouse-1.9.3/learninghouse/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:43:01.158748 learninghouse-1.9.3/learninghouse/ui/
--rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-07-17 12:42:47.000000 learninghouse-1.9.3/learninghouse/ui/357.4043c05452966edd.js
--rw-r--r--   0 runner    (1001) docker     (123)    16338 2023-07-17 12:42:47.000000 learninghouse-1.9.3/learninghouse/ui/3rdpartylicenses.txt
--rw-r--r--   0 runner    (1001) docker     (123)    13960 2023-07-17 12:42:47.000000 learninghouse-1.9.3/learninghouse/ui/603.bd786a543fc56b9a.js
--rw-r--r--   0 runner    (1001) docker     (123)    11837 2023-07-17 12:42:47.000000 learninghouse-1.9.3/learninghouse/ui/779.1f2d344d5b166c65.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:43:01.158748 learninghouse-1.9.3/learninghouse/ui/assets/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-17 12:42:48.000000 learninghouse-1.9.3/learninghouse/ui/assets/env.js
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-17 12:42:48.000000 learninghouse-1.9.3/learninghouse/ui/assets/env.template.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:43:01.162748 learninghouse-1.9.3/learninghouse/ui/assets/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   128504 2023-07-17 12:42:48.000000 learninghouse-1.9.3/learninghouse/ui/assets/fonts/material-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    20416 2023-07-17 12:42:48.000000 learninghouse-1.9.3/learninghouse/ui/assets/fonts/roboto-v30-latin-300.woff
--rw-r--r--   0 runner    (1001) docker     (123)    15740 2023-07-17 12:42:49.000000 learninghouse-1.9.3/learninghouse/ui/assets/fonts/roboto-v30-latin-300.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    22292 2023-07-17 12:42:49.000000 learninghouse-1.9.3/learninghouse/ui/assets/fonts/roboto-v30-latin-300italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    17508 2023-07-17 12:42:49.000000 learninghouse-1.9.3/learninghouse/ui/assets/fonts/roboto-v30-latin-300italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    20544 2023-07-17 12:42:49.000000 learninghouse-1.9.3/learninghouse/ui/assets/fonts/roboto-v30-latin-500.woff
--rw-r--r--   0 runner    (1001) docker     (123)    15920 2023-07-17 12:42:49.000000 learninghouse-1.9.3/learninghouse/ui/assets/fonts/roboto-v30-latin-500.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    22092 2023-07-17 12:42:49.000000 learninghouse-1.9.3/learninghouse/ui/assets/fonts/roboto-v30-latin-500italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    17336 2023-07-17 12:42:49.000000 learninghouse-1.9.3/learninghouse/ui/assets/fonts/roboto-v30-latin-500italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    22048 2023-07-17 12:42:49.000000 learninghouse-1.9.3/learninghouse/ui/assets/fonts/roboto-v30-latin-italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    17368 2023-07-17 12:42:49.000000 learninghouse-1.9.3/learninghouse/ui/assets/fonts/roboto-v30-latin-italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    20344 2023-07-17 12:42:49.000000 learninghouse-1.9.3/learninghouse/ui/assets/fonts/roboto-v30-latin-regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    15744 2023-07-17 12:42:49.000000 learninghouse-1.9.3/learninghouse/ui/assets/fonts/roboto-v30-latin-regular.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:43:01.162748 learninghouse-1.9.3/learninghouse/ui/assets/i18n/
--rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-07-17 12:42:49.000000 learninghouse-1.9.3/learninghouse/ui/assets/i18n/de.json
--rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-07-17 12:42:49.000000 learninghouse-1.9.3/learninghouse/ui/assets/i18n/en.json
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-07-17 12:42:48.000000 learninghouse-1.9.3/learninghouse/ui/assets/learninghouse_icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-17 12:42:47.000000 learninghouse-1.9.3/learninghouse/ui/common.b01a0b50178d7f2a.js
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-07-17 12:42:47.000000 learninghouse-1.9.3/learninghouse/ui/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     9649 2023-07-17 12:42:47.000000 learninghouse-1.9.3/learninghouse/ui/index.html
--rw-r--r--   0 runner    (1001) docker     (123)   991126 2023-07-17 12:42:47.000000 learninghouse-1.9.3/learninghouse/ui/main.e32b94e23641097a.js
--rw-r--r--   0 runner    (1001) docker     (123)   128504 2023-07-17 12:42:47.000000 learninghouse-1.9.3/learninghouse/ui/material-icons.3705a31196184f2e.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    33845 2023-07-17 12:42:48.000000 learninghouse-1.9.3/learninghouse/ui/polyfills.50674f5957a13a5d.js
--rw-r--r--   0 runner    (1001) docker     (123)    20416 2023-07-17 12:42:48.000000 learninghouse-1.9.3/learninghouse/ui/roboto-v30-latin-300.006981bf6ff6087f.woff
--rw-r--r--   0 runner    (1001) docker     (123)    15740 2023-07-17 12:42:48.000000 learninghouse-1.9.3/learninghouse/ui/roboto-v30-latin-300.a4eae32d320f45e6.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    17508 2023-07-17 12:42:48.000000 learninghouse-1.9.3/learninghouse/ui/roboto-v30-latin-300italic.43a343143e72a1ca.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    22292 2023-07-17 12:42:48.000000 learninghouse-1.9.3/learninghouse/ui/roboto-v30-latin-300italic.9d3ffcc3b116eed0.woff
--rw-r--r--   0 runner    (1001) docker     (123)    15920 2023-07-17 12:42:48.000000 learninghouse-1.9.3/learninghouse/ui/roboto-v30-latin-500.3170fd9aa9258fe0.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    20544 2023-07-17 12:42:48.000000 learninghouse-1.9.3/learninghouse/ui/roboto-v30-latin-500.e5748c3b7acf0d45.woff
--rw-r--r--   0 runner    (1001) docker     (123)    17336 2023-07-17 12:42:48.000000 learninghouse-1.9.3/learninghouse/ui/roboto-v30-latin-500italic.04452ce88d6a3c12.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    22092 2023-07-17 12:42:48.000000 learninghouse-1.9.3/learninghouse/ui/roboto-v30-latin-500italic.b575d1cc3fe2787f.woff
--rw-r--r--   0 runner    (1001) docker     (123)    17368 2023-07-17 12:42:48.000000 learninghouse-1.9.3/learninghouse/ui/roboto-v30-latin-italic.8ed3d75f3892762e.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    22048 2023-07-17 12:42:48.000000 learninghouse-1.9.3/learninghouse/ui/roboto-v30-latin-italic.cf6e4911a0d1cade.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20344 2023-07-17 12:42:48.000000 learninghouse-1.9.3/learninghouse/ui/roboto-v30-latin-regular.224e95b0e84110d8.woff
--rw-r--r--   0 runner    (1001) docker     (123)    15744 2023-07-17 12:42:48.000000 learninghouse-1.9.3/learninghouse/ui/roboto-v30-latin-regular.f2894edcf7d09d36.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-07-17 12:42:48.000000 learninghouse-1.9.3/learninghouse/ui/runtime.4daf7c4bacaafab6.js
--rw-r--r--   0 runner    (1001) docker     (123)   111809 2023-07-17 12:42:48.000000 learninghouse-1.9.3/learninghouse/ui/styles.9ca034c6b6ad1aec.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:43:01.146748 learninghouse-1.9.3/learninghouse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15815 2023-07-17 12:43:01.000000 learninghouse-1.9.3/learninghouse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-07-17 12:43:01.000000 learninghouse-1.9.3/learninghouse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 12:43:01.000000 learninghouse-1.9.3/learninghouse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-17 12:43:01.000000 learninghouse-1.9.3/learninghouse.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-17 12:43:01.000000 learninghouse-1.9.3/learninghouse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-17 12:43:01.000000 learninghouse-1.9.3/learninghouse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-17 12:42:47.000000 learninghouse-1.9.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-17 12:43:01.162748 learninghouse-1.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-17 12:42:47.000000 learninghouse-1.9.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-07-17 12:42:47.000000 learninghouse-1.9.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:43:54.974553 learninghouse-1.9.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-17 14:43:41.000000 learninghouse-1.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-17 14:43:39.000000 learninghouse-1.9.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15815 2023-07-17 14:43:54.974553 learninghouse-1.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15012 2023-07-17 14:43:41.000000 learninghouse-1.9.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-07-17 14:43:41.000000 learninghouse-1.9.4/THIRD-PARTY-NOTICES
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:43:54.974553 learninghouse-1.9.4/learninghouse/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-17 14:43:39.000000 learninghouse-1.9.4/learninghouse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-17 14:43:39.000000 learninghouse-1.9.4/learninghouse/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-17 14:43:54.974553 learninghouse-1.9.4/learninghouse/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:43:54.958553 learninghouse-1.9.4/learninghouse/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-17 14:43:39.000000 learninghouse-1.9.4/learninghouse/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-07-17 14:43:39.000000 learninghouse-1.9.4/learninghouse/api/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-07-17 14:43:39.000000 learninghouse-1.9.4/learninghouse/api/brain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-17 14:43:39.000000 learninghouse-1.9.4/learninghouse/api/docs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:43:54.958553 learninghouse-1.9.4/learninghouse/api/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-07-17 14:43:39.000000 learninghouse-1.9.4/learninghouse/api/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-07-17 14:43:39.000000 learninghouse-1.9.4/learninghouse/api/errors/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-07-17 14:43:39.000000 learninghouse-1.9.4/learninghouse/api/errors/brain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-17 14:43:39.000000 learninghouse-1.9.4/learninghouse/api/errors/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-07-17 14:43:39.000000 learninghouse-1.9.4/learninghouse/api/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-07-17 14:43:39.000000 learninghouse-1.9.4/learninghouse/api/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-17 14:43:39.000000 learninghouse-1.9.4/learninghouse/api/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:43:54.958553 learninghouse-1.9.4/learninghouse/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:43:39.000000 learninghouse-1.9.4/learninghouse/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-07-17 14:43:39.000000 learninghouse-1.9.4/learninghouse/core/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-07-17 14:43:39.000000 learninghouse-1.9.4/learninghouse/core/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:43:54.962553 learninghouse-1.9.4/learninghouse/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-17 14:43:39.000000 learninghouse-1.9.4/learninghouse/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-07-17 14:43:39.000000 learninghouse-1.9.4/learninghouse/models/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-07-17 14:43:39.000000 learninghouse-1.9.4/learninghouse/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13029 2023-07-17 14:43:39.000000 learninghouse-1.9.4/learninghouse/models/brain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-17 14:43:39.000000 learninghouse-1.9.4/learninghouse/models/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-07-17 14:43:39.000000 learninghouse-1.9.4/learninghouse/models/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-07-17 14:43:39.000000 learninghouse-1.9.4/learninghouse/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:43:54.962553 learninghouse-1.9.4/learninghouse/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:43:39.000000 learninghouse-1.9.4/learninghouse/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8901 2023-07-17 14:43:39.000000 learninghouse-1.9.4/learninghouse/services/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-07-17 14:43:39.000000 learninghouse-1.9.4/learninghouse/services/brain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5838 2023-07-17 14:43:39.000000 learninghouse-1.9.4/learninghouse/services/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-17 14:43:39.000000 learninghouse-1.9.4/learninghouse/services/sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:43:54.962553 learninghouse-1.9.4/learninghouse/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:43:54.966553 learninghouse-1.9.4/learninghouse/static/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)  1435746 2023-07-17 14:43:39.000000 learninghouse-1.9.4/learninghouse/static/docs/swagger-ui-bundle.js
+-rw-r--r--   0 runner    (1001) docker     (123)  2066928 2023-07-17 14:43:39.000000 learninghouse-1.9.4/learninghouse/static/docs/swagger-ui-bundle.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)   150945 2023-07-17 14:43:39.000000 learninghouse-1.9.4/learninghouse/static/docs/swagger-ui.css
+-rw-r--r--   0 runner    (1001) docker     (123)   260491 2023-07-17 14:43:39.000000 learninghouse-1.9.4/learninghouse/static/docs/swagger-ui.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-07-17 14:43:39.000000 learninghouse-1.9.4/learninghouse/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:43:54.970553 learninghouse-1.9.4/learninghouse/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-07-17 14:43:40.000000 learninghouse-1.9.4/learninghouse/ui/357.4043c05452966edd.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16338 2023-07-17 14:43:40.000000 learninghouse-1.9.4/learninghouse/ui/3rdpartylicenses.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13960 2023-07-17 14:43:40.000000 learninghouse-1.9.4/learninghouse/ui/603.bd786a543fc56b9a.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11837 2023-07-17 14:43:40.000000 learninghouse-1.9.4/learninghouse/ui/779.1f2d344d5b166c65.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:43:54.970553 learninghouse-1.9.4/learninghouse/ui/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-17 14:43:40.000000 learninghouse-1.9.4/learninghouse/ui/assets/env.js
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-17 14:43:40.000000 learninghouse-1.9.4/learninghouse/ui/assets/env.template.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:43:54.974553 learninghouse-1.9.4/learninghouse/ui/assets/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   128504 2023-07-17 14:43:40.000000 learninghouse-1.9.4/learninghouse/ui/assets/fonts/material-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    20416 2023-07-17 14:43:40.000000 learninghouse-1.9.4/learninghouse/ui/assets/fonts/roboto-v30-latin-300.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    15740 2023-07-17 14:43:40.000000 learninghouse-1.9.4/learninghouse/ui/assets/fonts/roboto-v30-latin-300.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    22292 2023-07-17 14:43:40.000000 learninghouse-1.9.4/learninghouse/ui/assets/fonts/roboto-v30-latin-300italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    17508 2023-07-17 14:43:40.000000 learninghouse-1.9.4/learninghouse/ui/assets/fonts/roboto-v30-latin-300italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    20544 2023-07-17 14:43:40.000000 learninghouse-1.9.4/learninghouse/ui/assets/fonts/roboto-v30-latin-500.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    15920 2023-07-17 14:43:40.000000 learninghouse-1.9.4/learninghouse/ui/assets/fonts/roboto-v30-latin-500.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    22092 2023-07-17 14:43:40.000000 learninghouse-1.9.4/learninghouse/ui/assets/fonts/roboto-v30-latin-500italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    17336 2023-07-17 14:43:40.000000 learninghouse-1.9.4/learninghouse/ui/assets/fonts/roboto-v30-latin-500italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    22048 2023-07-17 14:43:40.000000 learninghouse-1.9.4/learninghouse/ui/assets/fonts/roboto-v30-latin-italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    17368 2023-07-17 14:43:40.000000 learninghouse-1.9.4/learninghouse/ui/assets/fonts/roboto-v30-latin-italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    20344 2023-07-17 14:43:40.000000 learninghouse-1.9.4/learninghouse/ui/assets/fonts/roboto-v30-latin-regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    15744 2023-07-17 14:43:40.000000 learninghouse-1.9.4/learninghouse/ui/assets/fonts/roboto-v30-latin-regular.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:43:54.974553 learninghouse-1.9.4/learninghouse/ui/assets/i18n/
+-rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-07-17 14:43:40.000000 learninghouse-1.9.4/learninghouse/ui/assets/i18n/de.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-07-17 14:43:40.000000 learninghouse-1.9.4/learninghouse/ui/assets/i18n/en.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-07-17 14:43:40.000000 learninghouse-1.9.4/learninghouse/ui/assets/learninghouse_icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-17 14:43:40.000000 learninghouse-1.9.4/learninghouse/ui/common.b01a0b50178d7f2a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-07-17 14:43:40.000000 learninghouse-1.9.4/learninghouse/ui/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     9649 2023-07-17 14:43:40.000000 learninghouse-1.9.4/learninghouse/ui/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)   991126 2023-07-17 14:43:40.000000 learninghouse-1.9.4/learninghouse/ui/main.f783603f82a9309f.js
+-rw-r--r--   0 runner    (1001) docker     (123)   128504 2023-07-17 14:43:40.000000 learninghouse-1.9.4/learninghouse/ui/material-icons.3705a31196184f2e.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    33845 2023-07-17 14:43:40.000000 learninghouse-1.9.4/learninghouse/ui/polyfills.50674f5957a13a5d.js
+-rw-r--r--   0 runner    (1001) docker     (123)    20416 2023-07-17 14:43:40.000000 learninghouse-1.9.4/learninghouse/ui/roboto-v30-latin-300.006981bf6ff6087f.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    15740 2023-07-17 14:43:40.000000 learninghouse-1.9.4/learninghouse/ui/roboto-v30-latin-300.a4eae32d320f45e6.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    17508 2023-07-17 14:43:40.000000 learninghouse-1.9.4/learninghouse/ui/roboto-v30-latin-300italic.43a343143e72a1ca.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    22292 2023-07-17 14:43:40.000000 learninghouse-1.9.4/learninghouse/ui/roboto-v30-latin-300italic.9d3ffcc3b116eed0.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    15920 2023-07-17 14:43:40.000000 learninghouse-1.9.4/learninghouse/ui/roboto-v30-latin-500.3170fd9aa9258fe0.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    20544 2023-07-17 14:43:40.000000 learninghouse-1.9.4/learninghouse/ui/roboto-v30-latin-500.e5748c3b7acf0d45.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    17336 2023-07-17 14:43:40.000000 learninghouse-1.9.4/learninghouse/ui/roboto-v30-latin-500italic.04452ce88d6a3c12.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    22092 2023-07-17 14:43:40.000000 learninghouse-1.9.4/learninghouse/ui/roboto-v30-latin-500italic.b575d1cc3fe2787f.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    17368 2023-07-17 14:43:40.000000 learninghouse-1.9.4/learninghouse/ui/roboto-v30-latin-italic.8ed3d75f3892762e.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    22048 2023-07-17 14:43:40.000000 learninghouse-1.9.4/learninghouse/ui/roboto-v30-latin-italic.cf6e4911a0d1cade.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20344 2023-07-17 14:43:40.000000 learninghouse-1.9.4/learninghouse/ui/roboto-v30-latin-regular.224e95b0e84110d8.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    15744 2023-07-17 14:43:40.000000 learninghouse-1.9.4/learninghouse/ui/roboto-v30-latin-regular.f2894edcf7d09d36.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-07-17 14:43:40.000000 learninghouse-1.9.4/learninghouse/ui/runtime.4daf7c4bacaafab6.js
+-rw-r--r--   0 runner    (1001) docker     (123)   111809 2023-07-17 14:43:40.000000 learninghouse-1.9.4/learninghouse/ui/styles.9ca034c6b6ad1aec.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:43:54.958553 learninghouse-1.9.4/learninghouse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15815 2023-07-17 14:43:54.000000 learninghouse-1.9.4/learninghouse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-07-17 14:43:54.000000 learninghouse-1.9.4/learninghouse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 14:43:54.000000 learninghouse-1.9.4/learninghouse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-17 14:43:54.000000 learninghouse-1.9.4/learninghouse.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-17 14:43:54.000000 learninghouse-1.9.4/learninghouse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-17 14:43:54.000000 learninghouse-1.9.4/learninghouse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-17 14:43:39.000000 learninghouse-1.9.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-17 14:43:54.974553 learninghouse-1.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-17 14:43:39.000000 learninghouse-1.9.4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-07-17 14:43:39.000000 learninghouse-1.9.4/versioneer.py
```

### Comparing `learninghouse-1.9.3/LICENSE` & `learninghouse-1.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/PKG-INFO` & `learninghouse-1.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: learninghouse
-Version: 1.9.3
+Version: 1.9.4
 Summary: learningHouse - Teach your smart home everything
 Home-page: https://github.com/LearningHouseService/learninghouse-monorepo
 Author: Johannes Ott
 Author-email: info@johannes-ott.net
 Project-URL: Bug Reports, https://github.com/LearningHouseService/learninghouse/issues
 Keywords: smart home,machine learning,house automation
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `learninghouse-1.9.3/README.md` & `learninghouse-1.9.4/README.md`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/THIRD-PARTY-NOTICES` & `learninghouse-1.9.4/THIRD-PARTY-NOTICES`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/__init__.py` & `learninghouse-1.9.4/learninghouse/__init__.py`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/api/__init__.py` & `learninghouse-1.9.4/learninghouse/api/__init__.py`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/api/auth.py` & `learninghouse-1.9.4/learninghouse/api/auth.py`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/api/brain.py` & `learninghouse-1.9.4/learninghouse/api/brain.py`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/api/docs.py` & `learninghouse-1.9.4/learninghouse/api/docs.py`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/api/errors/__init__.py` & `learninghouse-1.9.4/learninghouse/api/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/api/errors/auth.py` & `learninghouse-1.9.4/learninghouse/api/errors/auth.py`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/api/errors/brain.py` & `learninghouse-1.9.4/learninghouse/api/errors/brain.py`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/api/errors/sensor.py` & `learninghouse-1.9.4/learninghouse/api/errors/sensor.py`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/api/middleware.py` & `learninghouse-1.9.4/learninghouse/api/middleware.py`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/api/sensor.py` & `learninghouse-1.9.4/learninghouse/api/sensor.py`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/api/ui.py` & `learninghouse-1.9.4/learninghouse/api/ui.py`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/core/logging.py` & `learninghouse-1.9.4/learninghouse/core/logging.py`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/core/settings.py` & `learninghouse-1.9.4/learninghouse/core/settings.py`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/models/__init__.py` & `learninghouse-1.9.4/learninghouse/models/__init__.py`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/models/auth.py` & `learninghouse-1.9.4/learninghouse/models/auth.py`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/models/base.py` & `learninghouse-1.9.4/learninghouse/models/base.py`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/models/brain.py` & `learninghouse-1.9.4/learninghouse/models/brain.py`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/models/preprocessing.py` & `learninghouse-1.9.4/learninghouse/models/preprocessing.py`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/models/sensor.py` & `learninghouse-1.9.4/learninghouse/models/sensor.py`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/service.py` & `learninghouse-1.9.4/learninghouse/service.py`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/services/auth.py` & `learninghouse-1.9.4/learninghouse/services/auth.py`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/services/brain.py` & `learninghouse-1.9.4/learninghouse/services/brain.py`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/services/preprocessing.py` & `learninghouse-1.9.4/learninghouse/services/preprocessing.py`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/services/sensor.py` & `learninghouse-1.9.4/learninghouse/services/sensor.py`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/static/docs/swagger-ui-bundle.js` & `learninghouse-1.9.4/learninghouse/static/docs/swagger-ui-bundle.js`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/static/docs/swagger-ui-bundle.js.map` & `learninghouse-1.9.4/learninghouse/static/docs/swagger-ui-bundle.js.map`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/static/docs/swagger-ui.css` & `learninghouse-1.9.4/learninghouse/static/docs/swagger-ui.css`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/static/docs/swagger-ui.css.map` & `learninghouse-1.9.4/learninghouse/static/docs/swagger-ui.css.map`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/static/favicon.ico` & `learninghouse-1.9.4/learninghouse/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/ui/357.4043c05452966edd.js` & `learninghouse-1.9.4/learninghouse/ui/357.4043c05452966edd.js`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/ui/3rdpartylicenses.txt` & `learninghouse-1.9.4/learninghouse/ui/3rdpartylicenses.txt`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/ui/603.bd786a543fc56b9a.js` & `learninghouse-1.9.4/learninghouse/ui/603.bd786a543fc56b9a.js`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/ui/779.1f2d344d5b166c65.js` & `learninghouse-1.9.4/learninghouse/ui/779.1f2d344d5b166c65.js`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/ui/assets/fonts/material-icons.woff2` & `learninghouse-1.9.4/learninghouse/ui/assets/fonts/material-icons.woff2`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/ui/assets/fonts/roboto-v30-latin-300.woff` & `learninghouse-1.9.4/learninghouse/ui/assets/fonts/roboto-v30-latin-300.woff`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/ui/assets/fonts/roboto-v30-latin-300.woff2` & `learninghouse-1.9.4/learninghouse/ui/assets/fonts/roboto-v30-latin-300.woff2`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/ui/assets/fonts/roboto-v30-latin-300italic.woff` & `learninghouse-1.9.4/learninghouse/ui/assets/fonts/roboto-v30-latin-300italic.woff`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/ui/assets/fonts/roboto-v30-latin-300italic.woff2` & `learninghouse-1.9.4/learninghouse/ui/assets/fonts/roboto-v30-latin-300italic.woff2`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/ui/assets/fonts/roboto-v30-latin-500.woff` & `learninghouse-1.9.4/learninghouse/ui/assets/fonts/roboto-v30-latin-500.woff`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/ui/assets/fonts/roboto-v30-latin-500.woff2` & `learninghouse-1.9.4/learninghouse/ui/assets/fonts/roboto-v30-latin-500.woff2`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/ui/assets/fonts/roboto-v30-latin-500italic.woff` & `learninghouse-1.9.4/learninghouse/ui/assets/fonts/roboto-v30-latin-500italic.woff`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/ui/assets/fonts/roboto-v30-latin-500italic.woff2` & `learninghouse-1.9.4/learninghouse/ui/assets/fonts/roboto-v30-latin-500italic.woff2`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/ui/assets/fonts/roboto-v30-latin-italic.woff` & `learninghouse-1.9.4/learninghouse/ui/assets/fonts/roboto-v30-latin-italic.woff`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/ui/assets/fonts/roboto-v30-latin-italic.woff2` & `learninghouse-1.9.4/learninghouse/ui/assets/fonts/roboto-v30-latin-italic.woff2`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/ui/assets/fonts/roboto-v30-latin-regular.woff` & `learninghouse-1.9.4/learninghouse/ui/assets/fonts/roboto-v30-latin-regular.woff`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/ui/assets/fonts/roboto-v30-latin-regular.woff2` & `learninghouse-1.9.4/learninghouse/ui/assets/fonts/roboto-v30-latin-regular.woff2`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/ui/assets/i18n/de.json` & `learninghouse-1.9.4/learninghouse/ui/assets/i18n/de.json`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/ui/assets/i18n/en.json` & `learninghouse-1.9.4/learninghouse/ui/assets/i18n/en.json`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/ui/assets/learninghouse_icon.svg` & `learninghouse-1.9.4/learninghouse/ui/assets/learninghouse_icon.svg`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/ui/common.b01a0b50178d7f2a.js` & `learninghouse-1.9.4/learninghouse/ui/common.b01a0b50178d7f2a.js`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/ui/favicon.ico` & `learninghouse-1.9.4/learninghouse/ui/favicon.ico`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/ui/index.html` & `learninghouse-1.9.4/learninghouse/ui/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -8,10 +8,10 @@
   <meta name="viewport" content="width=device-width, initial-scale=1">
   <link rel="icon" type="image/x-icon" href="favicon.ico">
   <script src="assets/env.js"></script>
 <style>html{--mat-option-selected-state-label-text-color:green;--mat-option-label-text-color:rgba(0, 0, 0, .87);--mat-option-hover-state-layer-color:rgba(0, 0, 0, .04);--mat-option-focus-state-layer-color:rgba(0, 0, 0, .04);--mat-option-selected-state-layer-color:rgba(0, 0, 0, .04)}html{--mat-optgroup-label-text-color:rgba(0, 0, 0, .87)}html{--mat-option-label-text-font:Roboto, sans-serif;--mat-option-label-text-line-height:24px;--mat-option-label-text-size:16px;--mat-option-label-text-tracking:.03125em;--mat-option-label-text-weight:400;--mat-optgroup-label-text-font:Roboto, sans-serif;--mat-optgroup-label-text-line-height:24px;--mat-optgroup-label-text-size:16px;--mat-optgroup-label-text-tracking:.03125em;--mat-optgroup-label-text-weight:400}html{--mat-select-panel-background-color:white;--mat-select-enabled-trigger-text-color:rgba(0, 0, 0, .87);--mat-select-disabled-trigger-text-color:rgba(0, 0, 0, .38);--mat-select-placeholder-text-color:rgba(0, 0, 0, .6);--mat-select-enabled-arrow-color:rgba(0, 0, 0, .54);--mat-select-disabled-arrow-color:rgba(0, 0, 0, .38);--mat-select-focused-arrow-color:rgba(0, 128, 0, .87);--mat-select-invalid-arrow-color:rgba(204, 0, 0, .87)}html{--mat-select-trigger-text-font:Roboto, sans-serif;--mat-select-trigger-text-line-height:24px;--mat-select-trigger-text-size:16px;--mat-select-trigger-text-tracking:.03125em;--mat-select-trigger-text-weight:400;--mat-autocomplete-background-color:white}html{--mat-menu-item-label-text-color:rgba(0, 0, 0, .87);--mat-menu-item-icon-color:rgba(0, 0, 0, .87);--mat-menu-item-hover-state-layer-color:rgba(0, 0, 0, .04);--mat-menu-item-focus-state-layer-color:rgba(0, 0, 0, .04);--mat-menu-container-color:white;--mat-menu-item-label-text-font:Roboto, sans-serif;--mat-menu-item-label-text-size:16px;--mat-menu-item-label-text-tracking:.03125em;--mat-menu-item-label-text-line-height:24px;--mat-menu-item-label-text-weight:400}html{--mat-paginator-container-text-color:rgba(0, 0, 0, .87);--mat-paginator-container-background-color:white;--mat-paginator-enabled-icon-color:rgba(0, 0, 0, .54);--mat-paginator-disabled-icon-color:rgba(0, 0, 0, .12);--mat-paginator-container-size:56px}html{--mat-paginator-container-text-font:Roboto, sans-serif;--mat-paginator-container-text-line-height:20px;--mat-paginator-container-text-size:12px;--mat-paginator-container-text-tracking:.0333333333em;--mat-paginator-container-text-weight:400;--mat-paginator-select-trigger-text-size:12px}html{--mdc-checkbox-disabled-selected-icon-color:rgba(0, 0, 0, .38);--mdc-checkbox-disabled-unselected-icon-color:rgba(0, 0, 0, .38);--mdc-checkbox-selected-checkmark-color:#000;--mdc-checkbox-selected-focus-icon-color:#83ff83;--mdc-checkbox-selected-hover-icon-color:#83ff83;--mdc-checkbox-selected-icon-color:#83ff83;--mdc-checkbox-selected-pressed-icon-color:#83ff83;--mdc-checkbox-unselected-focus-icon-color:#212121;--mdc-checkbox-unselected-hover-icon-color:#212121;--mdc-checkbox-unselected-icon-color:rgba(0, 0, 0, .54);--mdc-checkbox-unselected-pressed-icon-color:rgba(0, 0, 0, .54);--mdc-checkbox-selected-focus-state-layer-color:#83ff83;--mdc-checkbox-selected-hover-state-layer-color:#83ff83;--mdc-checkbox-selected-pressed-state-layer-color:#83ff83;--mdc-checkbox-unselected-focus-state-layer-color:black;--mdc-checkbox-unselected-hover-state-layer-color:black;--mdc-checkbox-unselected-pressed-state-layer-color:black}html{--mdc-checkbox-state-layer-size:40px}html{--mat-expansion-container-background-color:white;--mat-expansion-container-text-color:rgba(0, 0, 0, .87);--mat-expansion-actions-divider-color:rgba(0, 0, 0, .12);--mat-expansion-header-hover-state-layer-color:rgba(0, 0, 0, .04);--mat-expansion-header-focus-state-layer-color:rgba(0, 0, 0, .04);--mat-expansion-header-disabled-state-text-color:rgba(0, 0, 0, .26);--mat-expansion-header-text-color:rgba(0, 0, 0, .87);--mat-expansion-header-description-color:rgba(0, 0, 0, .54);--mat-expansion-header-indicator-color:rgba(0, 0, 0, .54);--mat-expansion-header-collapsed-state-height:48px;--mat-expansion-header-expanded-state-height:64px;--mat-expansion-header-text-font:Roboto, sans-serif;--mat-expansion-header-text-size:14px;--mat-expansion-header-text-weight:500;--mat-expansion-header-text-line-height:inherit;--mat-expansion-header-text-tracking:inherit;--mat-expansion-container-text-font:Roboto, sans-serif;--mat-expansion-container-text-line-height:20px;--mat-expansion-container-text-size:14px;--mat-expansion-container-text-tracking:.0178571429em;--mat-expansion-container-text-weight:400}html{--mat-stepper-header-icon-foreground-color:white;--mat-stepper-header-selected-state-icon-background-color:green;--mat-stepper-header-selected-state-icon-foreground-color:white;--mat-stepper-header-done-state-icon-background-color:green;--mat-stepper-header-done-state-icon-foreground-color:white;--mat-stepper-header-edit-state-icon-background-color:green;--mat-stepper-header-edit-state-icon-foreground-color:white;--mat-stepper-container-color:white;--mat-stepper-line-color:rgba(0, 0, 0, .12);--mat-stepper-header-hover-state-layer-color:rgba(0, 0, 0, .04);--mat-stepper-header-focus-state-layer-color:rgba(0, 0, 0, .04);--mat-stepper-header-label-text-color:rgba(0, 0, 0, .54);--mat-stepper-header-optional-label-text-color:rgba(0, 0, 0, .54);--mat-stepper-header-selected-state-label-text-color:rgba(0, 0, 0, .87);--mat-stepper-header-error-state-label-text-color:#cc0000;--mat-stepper-header-icon-background-color:rgba(0, 0, 0, .54);--mat-stepper-header-error-state-icon-foreground-color:#cc0000;--mat-stepper-header-error-state-icon-background-color:transparent}html{--mat-stepper-header-height:72px;--mat-stepper-container-text-font:Roboto, sans-serif;--mat-stepper-header-label-text-font:Roboto, sans-serif;--mat-stepper-header-label-text-size:14px;--mat-stepper-header-label-text-weight:400;--mat-stepper-header-error-state-label-text-size:16px;--mat-stepper-header-selected-state-label-text-size:16px;--mat-stepper-header-selected-state-label-text-weight:400}*,:before,:after{box-sizing:border-box;border-width:0;border-style:solid;border-color:#e5e7eb}:before,:after{--tw-content:""}html{line-height:1.5;-webkit-text-size-adjust:100%;tab-size:4;font-family:ui-sans-serif,system-ui,-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica Neue,Arial,Noto Sans,sans-serif,"Apple Color Emoji","Segoe UI Emoji",Segoe UI Symbol,"Noto Color Emoji";font-feature-settings:normal;font-variation-settings:normal}body{margin:0;line-height:inherit}*,:before,:after{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-gradient-from-position: ;--tw-gradient-via-position: ;--tw-gradient-to-position: ;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:rgb(59 130 246 / .5);--tw-ring-offset-shadow:0 0 #0000;--tw-ring-shadow:0 0 #0000;--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: }@font-face{font-family:Roboto;font-style:normal;font-weight:300;src:local(""),url(roboto-v30-latin-300.a4eae32d320f45e6.woff2) format("woff2"),url(roboto-v30-latin-300.006981bf6ff6087f.woff) format("woff")}@font-face{font-family:Roboto;font-style:italic;font-weight:300;src:local(""),url(roboto-v30-latin-300italic.43a343143e72a1ca.woff2) format("woff2"),url(roboto-v30-latin-300italic.9d3ffcc3b116eed0.woff) format("woff")}@font-face{font-family:Roboto;font-style:normal;font-weight:400;src:local(""),url(roboto-v30-latin-regular.f2894edcf7d09d36.woff2) format("woff2"),url(roboto-v30-latin-regular.224e95b0e84110d8.woff) format("woff")}@font-face{font-family:Roboto;font-style:italic;font-weight:400;src:local(""),url(roboto-v30-latin-italic.8ed3d75f3892762e.woff2) format("woff2"),url(roboto-v30-latin-italic.cf6e4911a0d1cade.woff) format("woff")}@font-face{font-family:Roboto;font-style:normal;font-weight:500;src:local(""),url(roboto-v30-latin-500.3170fd9aa9258fe0.woff2) format("woff2"),url(roboto-v30-latin-500.e5748c3b7acf0d45.woff) format("woff")}@font-face{font-family:Roboto;font-style:italic;font-weight:500;src:local(""),url(roboto-v30-latin-500italic.04452ce88d6a3c12.woff2) format("woff2"),url(roboto-v30-latin-500italic.b575d1cc3fe2787f.woff) format("woff")}html,body{height:100%}body{margin:0;font-family:Roboto,Helvetica Neue,sans-serif}</style><link rel="stylesheet" href="styles.9ca034c6b6ad1aec.css" media="print" onload="this.media='all'"><noscript><link rel="stylesheet" href="styles.9ca034c6b6ad1aec.css"></noscript></head>
 
 <body class="mat-typography">
   <app-root></app-root>
-<script src="runtime.4daf7c4bacaafab6.js" type="module"></script><script src="polyfills.50674f5957a13a5d.js" type="module"></script><script src="main.e32b94e23641097a.js" type="module"></script></body>
+<script src="runtime.4daf7c4bacaafab6.js" type="module"></script><script src="polyfills.50674f5957a13a5d.js" type="module"></script><script src="main.f783603f82a9309f.js" type="module"></script></body>
 
 </html>
```

### Comparing `learninghouse-1.9.3/learninghouse/ui/main.e32b94e23641097a.js` & `learninghouse-1.9.4/learninghouse/ui/main.f783603f82a9309f.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -4729,15 +4729,15 @@
             var v = d(7398),
                 k = d(6306),
                 x = d(2096),
                 K = d(9209);
             let ut = (() => {
                 class M {
                     get_app_version() {
-                        return "1.9.3"
+                        return "1.9.4"
                     }
                     get_angular_version() {
                         return s.q4F.full
                     }
                 }
                 return M.\u0275fac = function(u) {
                     return new(u || M)
```

### Comparing `learninghouse-1.9.3/learninghouse/ui/material-icons.3705a31196184f2e.woff2` & `learninghouse-1.9.4/learninghouse/ui/material-icons.3705a31196184f2e.woff2`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/ui/polyfills.50674f5957a13a5d.js` & `learninghouse-1.9.4/learninghouse/ui/polyfills.50674f5957a13a5d.js`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/ui/roboto-v30-latin-300.006981bf6ff6087f.woff` & `learninghouse-1.9.4/learninghouse/ui/roboto-v30-latin-300.006981bf6ff6087f.woff`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/ui/roboto-v30-latin-300.a4eae32d320f45e6.woff2` & `learninghouse-1.9.4/learninghouse/ui/roboto-v30-latin-300.a4eae32d320f45e6.woff2`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/ui/roboto-v30-latin-300italic.43a343143e72a1ca.woff2` & `learninghouse-1.9.4/learninghouse/ui/roboto-v30-latin-300italic.43a343143e72a1ca.woff2`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/ui/roboto-v30-latin-300italic.9d3ffcc3b116eed0.woff` & `learninghouse-1.9.4/learninghouse/ui/roboto-v30-latin-300italic.9d3ffcc3b116eed0.woff`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/ui/roboto-v30-latin-500.3170fd9aa9258fe0.woff2` & `learninghouse-1.9.4/learninghouse/ui/roboto-v30-latin-500.3170fd9aa9258fe0.woff2`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/ui/roboto-v30-latin-500.e5748c3b7acf0d45.woff` & `learninghouse-1.9.4/learninghouse/ui/roboto-v30-latin-500.e5748c3b7acf0d45.woff`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/ui/roboto-v30-latin-500italic.04452ce88d6a3c12.woff2` & `learninghouse-1.9.4/learninghouse/ui/roboto-v30-latin-500italic.04452ce88d6a3c12.woff2`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/ui/roboto-v30-latin-500italic.b575d1cc3fe2787f.woff` & `learninghouse-1.9.4/learninghouse/ui/roboto-v30-latin-500italic.b575d1cc3fe2787f.woff`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/ui/roboto-v30-latin-italic.8ed3d75f3892762e.woff2` & `learninghouse-1.9.4/learninghouse/ui/roboto-v30-latin-italic.8ed3d75f3892762e.woff2`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/ui/roboto-v30-latin-italic.cf6e4911a0d1cade.woff` & `learninghouse-1.9.4/learninghouse/ui/roboto-v30-latin-italic.cf6e4911a0d1cade.woff`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/ui/roboto-v30-latin-regular.224e95b0e84110d8.woff` & `learninghouse-1.9.4/learninghouse/ui/roboto-v30-latin-regular.224e95b0e84110d8.woff`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/ui/roboto-v30-latin-regular.f2894edcf7d09d36.woff2` & `learninghouse-1.9.4/learninghouse/ui/roboto-v30-latin-regular.f2894edcf7d09d36.woff2`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/ui/runtime.4daf7c4bacaafab6.js` & `learninghouse-1.9.4/learninghouse/ui/runtime.4daf7c4bacaafab6.js`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse/ui/styles.9ca034c6b6ad1aec.css` & `learninghouse-1.9.4/learninghouse/ui/styles.9ca034c6b6ad1aec.css`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/learninghouse.egg-info/PKG-INFO` & `learninghouse-1.9.4/learninghouse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: learninghouse
-Version: 1.9.3
+Version: 1.9.4
 Summary: learningHouse - Teach your smart home everything
 Home-page: https://github.com/LearningHouseService/learninghouse-monorepo
 Author: Johannes Ott
 Author-email: info@johannes-ott.net
 Project-URL: Bug Reports, https://github.com/LearningHouseService/learninghouse/issues
 Keywords: smart home,machine learning,house automation
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `learninghouse-1.9.3/learninghouse.egg-info/SOURCES.txt` & `learninghouse-1.9.4/learninghouse.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 learninghouse/ui/357.4043c05452966edd.js
 learninghouse/ui/3rdpartylicenses.txt
 learninghouse/ui/603.bd786a543fc56b9a.js
 learninghouse/ui/779.1f2d344d5b166c65.js
 learninghouse/ui/common.b01a0b50178d7f2a.js
 learninghouse/ui/favicon.ico
 learninghouse/ui/index.html
-learninghouse/ui/main.e32b94e23641097a.js
+learninghouse/ui/main.f783603f82a9309f.js
 learninghouse/ui/material-icons.3705a31196184f2e.woff2
 learninghouse/ui/polyfills.50674f5957a13a5d.js
 learninghouse/ui/roboto-v30-latin-300.006981bf6ff6087f.woff
 learninghouse/ui/roboto-v30-latin-300.a4eae32d320f45e6.woff2
 learninghouse/ui/roboto-v30-latin-300italic.43a343143e72a1ca.woff2
 learninghouse/ui/roboto-v30-latin-300italic.9d3ffcc3b116eed0.woff
 learninghouse/ui/roboto-v30-latin-500.3170fd9aa9258fe0.woff2
```

### Comparing `learninghouse-1.9.3/setup.py` & `learninghouse-1.9.4/setup.py`

 * *Files identical despite different names*

### Comparing `learninghouse-1.9.3/versioneer.py` & `learninghouse-1.9.4/versioneer.py`

 * *Files identical despite different names*

