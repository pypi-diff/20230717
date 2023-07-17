# Comparing `tmp/nowcasting_datamodel-1.4.9.tar.gz` & `tmp/nowcasting_datamodel-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nowcasting_datamodel-1.4.9.tar", last modified: Mon Jul  3 10:33:26 2023, max compression
+gzip compressed data, was "nowcasting_datamodel-1.5.0.tar", last modified: Mon Jul 17 19:50:51 2023, max compression
```

## Comparing `nowcasting_datamodel-1.4.9.tar` & `nowcasting_datamodel-1.5.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:33:26.246409 nowcasting_datamodel-1.4.9/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-07-03 10:33:26.246409 nowcasting_datamodel-1.4.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   151651 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/diagram.png
--rw-r--r--   0 runner    (1001) docker     (123)    49887 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/diagram_pv.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:33:26.242409 nowcasting_datamodel-1.4.9/nowcasting_datamodel/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9558 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/fake.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:33:26.242409 nowcasting_datamodel-1.4.9/nowcasting_datamodel/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/migrations/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:33:26.242409 nowcasting_datamodel-1.4.9/nowcasting_datamodel/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/models/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/models/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    18777 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/models/forecast.py
--rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/models/gsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/models/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/models/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/models/pv.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/national.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:33:26.242409 nowcasting_datamodel-1.4.9/nowcasting_datamodel/read/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/read/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:33:26.246409 nowcasting_datamodel-1.4.9/nowcasting_datamodel/read/blend/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/read/blend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6529 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/read/blend/blend.py
--rw-r--r--   0 runner    (1001) docker     (123)     8282 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/read/blend/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/read/blend/weights.py
--rw-r--r--   0 runner    (1001) docker     (123)    24247 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/read/read.py
--rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/read/read_gsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/read/read_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/read/read_pv.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/read/read_user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:33:26.246409 nowcasting_datamodel-1.4.9/nowcasting_datamodel/save/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/save/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6373 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/save/adjust.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/save/save.py
--rw-r--r--   0 runner    (1001) docker     (123)     9583 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/save/update.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:33:26.242409 nowcasting_datamodel-1.4.9/nowcasting_datamodel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-07-03 10:33:26.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-03 10:33:26.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 10:33:26.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-03 10:33:26.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-03 10:33:26.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 10:33:26.246409 nowcasting_datamodel-1.4.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:33:26.246409 nowcasting_datamodel-1.4.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/tests/test_databaseconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/tests/test_fake.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/tests/test_fake_pv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/tests/test_national.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:50:51.070671 nowcasting_datamodel-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-17 19:50:39.000000 nowcasting_datamodel-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-07-17 19:50:51.070671 nowcasting_datamodel-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-07-17 19:50:39.000000 nowcasting_datamodel-1.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   151651 2023-07-17 19:50:39.000000 nowcasting_datamodel-1.5.0/diagram.png
+-rw-r--r--   0 runner    (1001) docker     (123)    49887 2023-07-17 19:50:39.000000 nowcasting_datamodel-1.5.0/diagram_pv.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:50:51.062671 nowcasting_datamodel-1.5.0/nowcasting_datamodel/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-17 19:50:39.000000 nowcasting_datamodel-1.5.0/nowcasting_datamodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-17 19:50:39.000000 nowcasting_datamodel-1.5.0/nowcasting_datamodel/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-07-17 19:50:39.000000 nowcasting_datamodel-1.5.0/nowcasting_datamodel/fake.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:50:51.062671 nowcasting_datamodel-1.5.0/nowcasting_datamodel/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-17 19:50:39.000000 nowcasting_datamodel-1.5.0/nowcasting_datamodel/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-17 19:50:39.000000 nowcasting_datamodel-1.5.0/nowcasting_datamodel/migrations/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:50:51.066671 nowcasting_datamodel-1.5.0/nowcasting_datamodel/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-17 19:50:39.000000 nowcasting_datamodel-1.5.0/nowcasting_datamodel/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-17 19:50:39.000000 nowcasting_datamodel-1.5.0/nowcasting_datamodel/models/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-17 19:50:39.000000 nowcasting_datamodel-1.5.0/nowcasting_datamodel/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-07-17 19:50:39.000000 nowcasting_datamodel-1.5.0/nowcasting_datamodel/models/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19379 2023-07-17 19:50:39.000000 nowcasting_datamodel-1.5.0/nowcasting_datamodel/models/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-07-17 19:50:39.000000 nowcasting_datamodel-1.5.0/nowcasting_datamodel/models/gsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-07-17 19:50:39.000000 nowcasting_datamodel-1.5.0/nowcasting_datamodel/models/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-07-17 19:50:39.000000 nowcasting_datamodel-1.5.0/nowcasting_datamodel/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-07-17 19:50:39.000000 nowcasting_datamodel-1.5.0/nowcasting_datamodel/models/pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-17 19:50:39.000000 nowcasting_datamodel-1.5.0/nowcasting_datamodel/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-07-17 19:50:39.000000 nowcasting_datamodel-1.5.0/nowcasting_datamodel/national.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:50:51.066671 nowcasting_datamodel-1.5.0/nowcasting_datamodel/read/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-17 19:50:39.000000 nowcasting_datamodel-1.5.0/nowcasting_datamodel/read/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:50:51.070671 nowcasting_datamodel-1.5.0/nowcasting_datamodel/read/blend/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-17 19:50:39.000000 nowcasting_datamodel-1.5.0/nowcasting_datamodel/read/blend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-07-17 19:50:39.000000 nowcasting_datamodel-1.5.0/nowcasting_datamodel/read/blend/blend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8394 2023-07-17 19:50:39.000000 nowcasting_datamodel-1.5.0/nowcasting_datamodel/read/blend/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-07-17 19:50:39.000000 nowcasting_datamodel-1.5.0/nowcasting_datamodel/read/blend/weights.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24306 2023-07-17 19:50:39.000000 nowcasting_datamodel-1.5.0/nowcasting_datamodel/read/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9274 2023-07-17 19:50:39.000000 nowcasting_datamodel-1.5.0/nowcasting_datamodel/read/read_gsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-07-17 19:50:39.000000 nowcasting_datamodel-1.5.0/nowcasting_datamodel/read/read_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-07-17 19:50:39.000000 nowcasting_datamodel-1.5.0/nowcasting_datamodel/read/read_pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-17 19:50:39.000000 nowcasting_datamodel-1.5.0/nowcasting_datamodel/read/read_user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:50:51.070671 nowcasting_datamodel-1.5.0/nowcasting_datamodel/save/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-17 19:50:39.000000 nowcasting_datamodel-1.5.0/nowcasting_datamodel/save/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6373 2023-07-17 19:50:39.000000 nowcasting_datamodel-1.5.0/nowcasting_datamodel/save/adjust.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-07-17 19:50:39.000000 nowcasting_datamodel-1.5.0/nowcasting_datamodel/save/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9583 2023-07-17 19:50:39.000000 nowcasting_datamodel-1.5.0/nowcasting_datamodel/save/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-17 19:50:39.000000 nowcasting_datamodel-1.5.0/nowcasting_datamodel/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:50:51.062671 nowcasting_datamodel-1.5.0/nowcasting_datamodel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-07-17 19:50:51.000000 nowcasting_datamodel-1.5.0/nowcasting_datamodel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-17 19:50:51.000000 nowcasting_datamodel-1.5.0/nowcasting_datamodel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 19:50:51.000000 nowcasting_datamodel-1.5.0/nowcasting_datamodel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-17 19:50:51.000000 nowcasting_datamodel-1.5.0/nowcasting_datamodel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-17 19:50:51.000000 nowcasting_datamodel-1.5.0/nowcasting_datamodel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-17 19:50:39.000000 nowcasting_datamodel-1.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 19:50:51.070671 nowcasting_datamodel-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-17 19:50:39.000000 nowcasting_datamodel-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:50:51.070671 nowcasting_datamodel-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-17 19:50:39.000000 nowcasting_datamodel-1.5.0/tests/test_databaseconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-07-17 19:50:39.000000 nowcasting_datamodel-1.5.0/tests/test_fake.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-17 19:50:39.000000 nowcasting_datamodel-1.5.0/tests/test_fake_pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-17 19:50:39.000000 nowcasting_datamodel-1.5.0/tests/test_national.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-17 19:50:39.000000 nowcasting_datamodel-1.5.0/tests/test_utils.py
```

### Comparing `nowcasting_datamodel-1.4.9/PKG-INFO` & `nowcasting_datamodel-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nowcasting_datamodel
-Version: 1.4.9
+Version: 1.5.0
 Summary: Data Model for the OCF nowcasting project
 Home-page: https://github.com/openclimatefix/nowcasting_datamodel
 Author: Peter Dudfield
 Author-email: peter@openclimatefix.org
 License: MIT
 Keywords: SQL,Datamodel
 Description-Content-Type: text/markdown
```

### Comparing `nowcasting_datamodel-1.4.9/README.md` & `nowcasting_datamodel-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.9/diagram.png` & `nowcasting_datamodel-1.5.0/diagram.png`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.9/diagram_pv.png` & `nowcasting_datamodel-1.5.0/diagram_pv.png`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.9/nowcasting_datamodel/connection.py` & `nowcasting_datamodel-1.5.0/nowcasting_datamodel/connection.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.9/nowcasting_datamodel/fake.py` & `nowcasting_datamodel-1.5.0/nowcasting_datamodel/fake.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,16 +58,16 @@
     )
 
 
 def make_fake_forecast(
     gsp_id: int,
     session: Session,
     t0_datetime_utc: Optional[datetime] = None,
-    forecast_values: Optional = None,
-    forecast_values_latest: Optional = None,
+    forecast_values: Optional[List[ForecastValueSQL]] = None,
+    forecast_values_latest: Optional[List[ForecastValueSQL]] = None,
     add_latest: Optional[bool] = False,
     historic: Optional[bool] = False,
 ) -> ForecastSQL:
     """Make one fake forecast"""
 
     if gsp_id == 0:
         # national capacity
@@ -123,15 +123,15 @@
     return forecast
 
 
 def make_fake_forecasts(
     gsp_ids: List[int],
     session: Session,
     t0_datetime_utc: Optional[datetime] = None,
-    forecast_values: Optional = None,
+    forecast_values: Optional[List[ForecastValueSQL]] = None,
     add_latest: Optional[bool] = False,
     historic: Optional[bool] = False,
 ) -> List[ForecastSQL]:
     """Make many fake forecast"""
     forecasts = []
     for gsp_id in gsp_ids:
         forecasts.append(
```

### Comparing `nowcasting_datamodel-1.4.9/nowcasting_datamodel/migrations/app.py` & `nowcasting_datamodel-1.5.0/nowcasting_datamodel/migrations/app.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.9/nowcasting_datamodel/models/__init__.py` & `nowcasting_datamodel-1.5.0/nowcasting_datamodel/models/__init__.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.9/nowcasting_datamodel/models/api.py` & `nowcasting_datamodel-1.5.0/nowcasting_datamodel/models/api.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.9/nowcasting_datamodel/models/convert.py` & `nowcasting_datamodel-1.5.0/nowcasting_datamodel/models/convert.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.9/nowcasting_datamodel/models/forecast.py` & `nowcasting_datamodel-1.5.0/nowcasting_datamodel/models/forecast.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 """
 
 import logging
 from datetime import datetime
 from typing import List
 
+import numpy as np
 from pydantic import Field, validator
 from sqlalchemy import (
     JSON,
     Boolean,
     Column,
     DateTime,
     Float,
@@ -40,15 +41,15 @@
 """
 Tried to follow the example here
 https://stackoverflow.com/questions/61545680/postgresql-partition-and-sqlalchemy
 """
 
 
 class PartitionByMeta(DeclarativeMeta):
-    """Parition table meta object"""
+    """Partition table meta object"""
 
     def __new__(cls, clsname, bases, attrs, *, partition_by, partition_type: str = "RANGE"):
         """Make new partition"""
 
         @classmethod
         def get_partition_name(cls_, suffix):
             """Get the name of the partition table"""
@@ -339,18 +340,22 @@
     @classmethod
     def from_orm(cls, obj: ForecastValueSQL):
         """Make sure _adjust_mw is transfered also"""
         m = super().from_orm(obj=obj)
 
         # this is because from orm doesnt copy over '_' variables.
         # But we don't want to expose this in the API
+        default_value = 0.0
         if hasattr(obj, "adjust_mw"):
-            m._adjust_mw = obj.adjust_mw
+            adjust_mw = obj.adjust_mw
+            if not adjust_mw or np.isnan(adjust_mw):
+                adjust_mw = default_value
+            m._adjust_mw = adjust_mw
         else:
-            m._adjust_mw = 0.0
+            m._adjust_mw = default_value
 
         return m
 
     def normalize(self, installed_capacity_mw):
         """Normalize forecasts by installed capacity mw"""
         if installed_capacity_mw in [0, None]:
             self.expected_power_generation_normalized = 0
@@ -373,14 +378,22 @@
             self.expected_power_generation_megawatts = (
                 self.expected_power_generation_megawatts - adjust_mw
             )
 
             if self.expected_power_generation_megawatts < 0:
                 self.expected_power_generation_megawatts = 0.0
 
+            if isinstance(self._properties, dict):
+                for p_level in ["10", "90"]:
+                    if p_level in self._properties.keys():
+                        if self._properties[p_level] is not None:
+                            self._properties[p_level] -= adjust_mw
+                            if self._properties[p_level] < 0:
+                                self._properties[p_level] = 0.0
+
         return self
 
 
 class ForecastSQL(Base_Forecast, CreatedMixin):
     """Forecast SQL model"""
 
     __tablename__ = "forecast"
```

### Comparing `nowcasting_datamodel-1.4.9/nowcasting_datamodel/models/gsp.py` & `nowcasting_datamodel-1.5.0/nowcasting_datamodel/models/gsp.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 2. Location objects, where the forecast is for
 8. GSP yield for storing GSP yield data
 
 """
 import logging
 from datetime import datetime
-from typing import List, Optional
+from typing import ClassVar, List, Optional
 
 from pydantic import Field, validator
 from sqlalchemy import Column, DateTime, Float, ForeignKey, Index, Integer, String
 from sqlalchemy.orm import relationship
 
 from nowcasting_datamodel.models.base import Base_Forecast
 from nowcasting_datamodel.models.utils import CreatedMixin, EnhancedBaseModel
@@ -49,14 +49,16 @@
     gsp_name: Optional[str] = Field(None, description="The GSP name")
     gsp_group: Optional[str] = Field(None, description="The GSP group name")
     region_name: Optional[str] = Field(None, description="The GSP region name")
     installed_capacity_mw: Optional[float] = Field(
         None, description="The installed capacity of the GSP in MW"
     )
 
+    rm_mode: ClassVar[bool] = True
+
     def to_orm(self) -> LocationSQL:
         """Change model to LocationSQL"""
 
         if isinstance(self, LocationSQL):
             return self
 
         return LocationSQL(
```

### Comparing `nowcasting_datamodel-1.4.9/nowcasting_datamodel/models/metric.py` & `nowcasting_datamodel-1.5.0/nowcasting_datamodel/models/metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 1. metric, stores the metric metadata
 2. datetime_interval - The datetime interval that the metric is for
 3. metric_value, the actual value of this metric
 
 """
 
 from datetime import datetime, time
+from typing import ClassVar
 
 from pydantic import Field, validator
 from sqlalchemy import Boolean, Column, DateTime, Float, ForeignKey, Index, Integer, String, Time
 from sqlalchemy.orm import relationship
 
 from nowcasting_datamodel.models.base import Base_Forecast
 from nowcasting_datamodel.models.gsp import Location
@@ -37,14 +38,16 @@
 
 class Metric(EnhancedBaseModel):
     """Metric metadata"""
 
     name: str = Field(..., description="The name of the metric")
     description: str = Field(..., description="The description of the metric")
 
+    rm_mode: ClassVar[bool] = True
+
     def to_orm(self) -> MetricSQL:
         """Change model to LocationSQL"""
 
         if isinstance(self, MetricSQL):
             return self
 
         return MetricSQL(
@@ -162,15 +165,17 @@
         "60 minutes means the forecast made 60 mintues before the target time",
     )
     time_of_day: time = Field(None, description="the time of tday for this metric")
     metric: Metric = Field(..., description="The metric this value is about")
     datetime_interval: DatetimeInterval = Field(
         ..., description="The datetime interval this value is about"
     )
-    location: Location = Field(..., description="The location object for this metric value")
+    location: Location = Field(None, description="The location object for this metric value")
+
+    rm_mode: ClassVar[bool] = True
 
     def to_orm(self) -> MetricValueSQL:
         """Change model to MetricValueSQL"""
 
         if isinstance(self, MetricValueSQL):
             return self
```

### Comparing `nowcasting_datamodel-1.4.9/nowcasting_datamodel/models/models.py` & `nowcasting_datamodel-1.5.0/nowcasting_datamodel/models/models.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.9/nowcasting_datamodel/models/pv.py` & `nowcasting_datamodel-1.5.0/nowcasting_datamodel/models/pv.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.9/nowcasting_datamodel/models/utils.py` & `nowcasting_datamodel-1.5.0/nowcasting_datamodel/models/utils.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.9/nowcasting_datamodel/national.py` & `nowcasting_datamodel-1.5.0/nowcasting_datamodel/national.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.9/nowcasting_datamodel/read/blend/blend.py` & `nowcasting_datamodel-1.5.0/nowcasting_datamodel/read/blend/blend.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,14 +145,15 @@
     if properties_model is None:
         blended_df["properties"] = None
         return blended_df
 
     # get properties
 
     properties_df = all_model_df[all_model_df["model_name"] == properties_model]
+    properties_df.reset_index(inplace=True, drop=True)
 
     # adjust "properties" to be relative to the expected_power_generation_megawatts
     # this is a bit tricky becasue the "properties" column is a list of dictionaries
     # below we add "expected_power_generation_megawatts" value back to this.
     # We do this so that plevels are relative to the blended values.
     properties_only_df = pd.json_normalize(properties_df["properties"])
     for c in properties_only_df.columns:
```

### Comparing `nowcasting_datamodel-1.4.9/nowcasting_datamodel/read/blend/utils.py` & `nowcasting_datamodel-1.5.0/nowcasting_datamodel/read/blend/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Utils for blending forecasts together"""
 from datetime import datetime, timedelta, timezone
 from typing import List, Union
 
+import numpy as np
 import pandas as pd
 import structlog
 
 from nowcasting_datamodel.models import ForecastValue
 
 logger = structlog.stdlib.get_logger()
 
@@ -87,27 +88,29 @@
     # join into one dataframe
     forecast_values_all_model = pd.concat(forecast_values_all_model_df, axis=0)
     forecast_values_all_model.reset_index(inplace=True)
 
     return forecast_values_all_model
 
 
-def convert_df_to_list_forecast_values(forecast_values_blended):
+def convert_df_to_list_forecast_values(forecast_values_blended: pd.DataFrame):
     """
     Convert the blended dataframe to a list of ForecastValue objects
 
     :param forecast_values_blended: Needs to have the columns 'target_time'
         and 'expected_power_generation_megawatts
     :return:
     """
     forecast_values = []
     logger.debug(forecast_values_blended)
     for i, row in forecast_values_blended.iterrows():
         # make sure we don't have negative values
         expected_power_generation_megawatts = row.expected_power_generation_megawatts
+        if np.isnan(expected_power_generation_megawatts):
+            continue
         if expected_power_generation_megawatts < 0:
             expected_power_generation_megawatts = 0
 
         forecast_value = ForecastValue(
             target_time=row.target_time,
             expected_power_generation_megawatts=expected_power_generation_megawatts,
         )
```

### Comparing `nowcasting_datamodel-1.4.9/nowcasting_datamodel/read/blend/weights.py` & `nowcasting_datamodel-1.5.0/nowcasting_datamodel/read/blend/weights.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.9/nowcasting_datamodel/read/read.py` & `nowcasting_datamodel-1.5.0/nowcasting_datamodel/read/read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """ Read database functions
 
 1. Get the latest forecast
 2. get the latest forecasts for all gsp ids
 3. get all forecast values
 """
 from datetime import datetime, timedelta, timezone
-from typing import List, Optional
+from typing import List, Optional, Union
 
 import structlog
 from sqlalchemy import desc, text
 from sqlalchemy.orm import contains_eager, joinedload
 from sqlalchemy.orm.session import Session
 
 from nowcasting_datamodel import N_GSP
@@ -81,15 +81,15 @@
     return input_data
 
 
 def update_latest_input_data_last_updated(
     session: Session, component: str, update_datetime: Optional[datetime] = None
 ):
     """
-    Update the table InputDataLastUpdatedSQL with a new valye
+    Update the table InputDataLastUpdatedSQL with a new value
 
     :param session:
     :param component: This should be gsp, pv, nwp or satellite
     :param update_datetime: the datetime is should be updated.
         Default is None, so will be set to now
     :return:
     """
@@ -403,15 +403,15 @@
     session: Session,
     gsp_id: Optional[int] = None,
     gsp_ids: Optional[List[int]] = None,
     start_datetime: Optional[datetime] = None,
     end_datetime: Optional[datetime] = None,
     forecast_horizon_minutes: Optional[int] = None,
     only_return_latest: Optional[bool] = False,
-    model: Optional = ForecastValueSQL,
+    model: Optional[Union[ForecastValueSQL, ForecastValueSevenDaysSQL]] = ForecastValueSQL,
     model_name: Optional[str] = None,
     created_utc_limit: Optional[datetime] = None,
 ) -> List[ForecastValueSQL]:
     """
     Get forecast values
 
     :param session: database session
```

### Comparing `nowcasting_datamodel-1.4.9/nowcasting_datamodel/read/read_gsp.py` & `nowcasting_datamodel-1.5.0/nowcasting_datamodel/read/read_gsp.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,15 +50,17 @@
 
     if datetime_utc is not None:
         # filter on datetime
         query = query.where(GSPYieldSQL.datetime_utc >= datetime_utc)
 
     # order by 'created_utc' desc, so we get the latest one
     query = query.order_by(
-        LocationSQL.gsp_id, desc(GSPYieldSQL.datetime_utc), desc(GSPYieldSQL.created_utc)
+        LocationSQL.gsp_id,
+        desc(GSPYieldSQL.datetime_utc),
+        desc(GSPYieldSQL.created_utc),
     )
 
     # get all results
     gsp_yields: List[GSPYieldSQL] = query.all()
 
     logger.debug(f"Found {len(gsp_yields)}  latest gsp yields")
 
@@ -141,15 +143,17 @@
     query = query.distinct(*[LocationSQL.gsp_id, GSPYieldSQL.datetime_utc])
 
     # select only the gsp systems we want
     query = query.where(LocationSQL.gsp_id.in_(gsp_ids))
 
     # order by 'created_utc' desc, so we get the latest one
     query = query.order_by(
-        LocationSQL.gsp_id, desc(GSPYieldSQL.datetime_utc), desc(GSPYieldSQL.created_utc)
+        LocationSQL.gsp_id,
+        desc(GSPYieldSQL.datetime_utc),
+        desc(GSPYieldSQL.created_utc),
     )
 
     # get all results
     gsp_yields: List[GSPYieldSQL] = query.all()
 
     for gsp_yield in gsp_yields:
         gsp_yield.datetime_utc = gsp_yield.datetime_utc.replace(tzinfo=timezone.utc)
@@ -202,15 +206,17 @@
     query = query.where(LocationSQL.gsp_id.in_(gsp_ids))
 
     # load only once
     query = query.options(contains_eager(LocationSQL.gsp_yields))
 
     # order by 'created_utc' desc, so we get the latest one
     query = query.order_by(
-        LocationSQL.gsp_id, desc(GSPYieldSQL.datetime_utc), desc(GSPYieldSQL.created_utc)
+        LocationSQL.gsp_id,
+        desc(GSPYieldSQL.datetime_utc),
+        desc(GSPYieldSQL.created_utc),
     )
 
     # get all results
     locations: List[LocationSQL] = query.all()
 
     for location in locations:
         for gsp_yield in location.gsp_yields:
@@ -260,14 +266,17 @@
     query = query.where(GSPYieldSQL.regime == regime)
 
     # filter on datetime
     query = query.where(GSPYieldSQL.datetime_utc >= start_datetime_utc)
     if end_datetime_utc is not None:
         query = query.where(GSPYieldSQL.datetime_utc <= end_datetime_utc)
 
+    # filter out nans
+    query = query.where(GSPYieldSQL.solar_generation_kw + 1 > GSPYieldSQL.solar_generation_kw)
+
     # group and order by datetime
     query = query.group_by(GSPYieldSQL.datetime_utc)
     query = query.order_by(GSPYieldSQL.datetime_utc)
 
     results = query.all()
 
     # format results
```

### Comparing `nowcasting_datamodel-1.4.9/nowcasting_datamodel/read/read_metric.py` & `nowcasting_datamodel-1.5.0/nowcasting_datamodel/read/read_metric.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.9/nowcasting_datamodel/read/read_pv.py` & `nowcasting_datamodel-1.5.0/nowcasting_datamodel/read/read_pv.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.9/nowcasting_datamodel/read/read_user.py` & `nowcasting_datamodel-1.5.0/nowcasting_datamodel/read/read_user.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.9/nowcasting_datamodel/save/adjust.py` & `nowcasting_datamodel-1.5.0/nowcasting_datamodel/save/adjust.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.9/nowcasting_datamodel/save/save.py` & `nowcasting_datamodel-1.5.0/nowcasting_datamodel/save/save.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.9/nowcasting_datamodel/save/update.py` & `nowcasting_datamodel-1.5.0/nowcasting_datamodel/save/update.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.9/nowcasting_datamodel/utils.py` & `nowcasting_datamodel-1.5.0/nowcasting_datamodel/utils.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.9/nowcasting_datamodel.egg-info/PKG-INFO` & `nowcasting_datamodel-1.5.0/nowcasting_datamodel.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nowcasting-datamodel
-Version: 1.4.9
+Version: 1.5.0
 Summary: Data Model for the OCF nowcasting project
 Home-page: https://github.com/openclimatefix/nowcasting_datamodel
 Author: Peter Dudfield
 Author-email: peter@openclimatefix.org
 License: MIT
 Keywords: SQL,Datamodel
 Description-Content-Type: text/markdown
```

### Comparing `nowcasting_datamodel-1.4.9/nowcasting_datamodel.egg-info/SOURCES.txt` & `nowcasting_datamodel-1.5.0/nowcasting_datamodel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.9/setup.py` & `nowcasting_datamodel-1.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.9/tests/test_databaseconnection.py` & `nowcasting_datamodel-1.5.0/tests/test_databaseconnection.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.9/tests/test_fake.py` & `nowcasting_datamodel-1.5.0/tests/test_fake.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     _ = Forecast.from_orm(forecast_sql)
 
     from sqlalchemy import text
 
     f = ForecastValueSQL(target_time="2023-01-01 12:00:00", expected_power_generation_megawatts=3)
     db_session.add(f)
     db_session.commit()
-    tables = db_session.execute(text("SELECT * FROM forecast_value_2023_01")).all()
+    _ = db_session.execute(text("SELECT * FROM forecast_value_2023_01")).all()
 
 
 def test_make_fake_forecasts(db_session):
     make_fake_forecasts(session=db_session, gsp_ids=[0, 1, 2, 3], add_latest=True)
 
     assert len(db_session.query(ForecastSQL).all()) > 0
     assert len(db_session.query(ForecastValueLatestSQL).all()) > 0
```

### Comparing `nowcasting_datamodel-1.4.9/tests/test_fake_pv.py` & `nowcasting_datamodel-1.5.0/tests/test_fake_pv.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from datetime import datetime, timezone
+from datetime import datetime
 
 import pytest
 
 from nowcasting_datamodel.fake import make_fake_pv_system
-from nowcasting_datamodel.models import PVSystem, PVSystemSQL, PVYield, PVYieldSQL
+from nowcasting_datamodel.models import PVSystem, PVSystemSQL, PVYield
 
 
 def test_make_fake_pv_system():
     pv_system_sql: PVSystemSQL = make_fake_pv_system()
     pv_system = PVSystem.from_orm(pv_system_sql)
     _ = PVSystem.to_orm(pv_system)
```

### Comparing `nowcasting_datamodel-1.4.9/tests/test_national.py` & `nowcasting_datamodel-1.5.0/tests/test_national.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.9/tests/test_utils.py` & `nowcasting_datamodel-1.5.0/tests/test_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 """ Utils functions for test """
 from datetime import datetime, timezone
 
-import pytest
-
 # Used constants
 from nowcasting_datamodel.utils import convert_to_camelcase, datetime_must_have_timezone
 
 
 def test_datetime_must_have_timezone():
     """Test function datetime_must_have_timezone"""
```

