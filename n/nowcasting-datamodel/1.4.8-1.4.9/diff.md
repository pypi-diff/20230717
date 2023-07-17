# Comparing `tmp/nowcasting_datamodel-1.4.8.tar.gz` & `tmp/nowcasting_datamodel-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nowcasting_datamodel-1.4.8.tar", last modified: Fri Jun 30 13:13:06 2023, max compression
+gzip compressed data, was "nowcasting_datamodel-1.4.9.tar", last modified: Mon Jul  3 10:33:26 2023, max compression
```

## Comparing `nowcasting_datamodel-1.4.8.tar` & `nowcasting_datamodel-1.4.9.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:13:06.537167 nowcasting_datamodel-1.4.8/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-30 13:12:56.000000 nowcasting_datamodel-1.4.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-06-30 13:13:06.537167 nowcasting_datamodel-1.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-06-30 13:12:56.000000 nowcasting_datamodel-1.4.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   151651 2023-06-30 13:12:56.000000 nowcasting_datamodel-1.4.8/diagram.png
--rw-r--r--   0 runner    (1001) docker     (123)    49887 2023-06-30 13:12:56.000000 nowcasting_datamodel-1.4.8/diagram_pv.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:13:06.533167 nowcasting_datamodel-1.4.8/nowcasting_datamodel/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-30 13:12:56.000000 nowcasting_datamodel-1.4.8/nowcasting_datamodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-06-30 13:12:56.000000 nowcasting_datamodel-1.4.8/nowcasting_datamodel/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9499 2023-06-30 13:12:56.000000 nowcasting_datamodel-1.4.8/nowcasting_datamodel/fake.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:13:06.533167 nowcasting_datamodel-1.4.8/nowcasting_datamodel/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-30 13:12:56.000000 nowcasting_datamodel-1.4.8/nowcasting_datamodel/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-30 13:12:56.000000 nowcasting_datamodel-1.4.8/nowcasting_datamodel/migrations/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:13:06.533167 nowcasting_datamodel-1.4.8/nowcasting_datamodel/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-30 13:12:56.000000 nowcasting_datamodel-1.4.8/nowcasting_datamodel/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-30 13:12:56.000000 nowcasting_datamodel-1.4.8/nowcasting_datamodel/models/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-30 13:12:56.000000 nowcasting_datamodel-1.4.8/nowcasting_datamodel/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-30 13:12:56.000000 nowcasting_datamodel-1.4.8/nowcasting_datamodel/models/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    17820 2023-06-30 13:12:56.000000 nowcasting_datamodel-1.4.8/nowcasting_datamodel/models/forecast.py
--rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-06-30 13:12:56.000000 nowcasting_datamodel-1.4.8/nowcasting_datamodel/models/gsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-06-30 13:12:56.000000 nowcasting_datamodel-1.4.8/nowcasting_datamodel/models/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-06-30 13:12:56.000000 nowcasting_datamodel-1.4.8/nowcasting_datamodel/models/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-06-30 13:12:56.000000 nowcasting_datamodel-1.4.8/nowcasting_datamodel/models/pv.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-30 13:12:56.000000 nowcasting_datamodel-1.4.8/nowcasting_datamodel/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-06-30 13:12:56.000000 nowcasting_datamodel-1.4.8/nowcasting_datamodel/national.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:13:06.533167 nowcasting_datamodel-1.4.8/nowcasting_datamodel/read/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-30 13:12:56.000000 nowcasting_datamodel-1.4.8/nowcasting_datamodel/read/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:13:06.533167 nowcasting_datamodel-1.4.8/nowcasting_datamodel/read/blend/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-30 13:12:56.000000 nowcasting_datamodel-1.4.8/nowcasting_datamodel/read/blend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-06-30 13:12:56.000000 nowcasting_datamodel-1.4.8/nowcasting_datamodel/read/blend/blend.py
--rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-06-30 13:12:56.000000 nowcasting_datamodel-1.4.8/nowcasting_datamodel/read/blend/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-06-30 13:12:56.000000 nowcasting_datamodel-1.4.8/nowcasting_datamodel/read/blend/weights.py
--rw-r--r--   0 runner    (1001) docker     (123)    24247 2023-06-30 13:12:56.000000 nowcasting_datamodel-1.4.8/nowcasting_datamodel/read/read.py
--rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-06-30 13:12:56.000000 nowcasting_datamodel-1.4.8/nowcasting_datamodel/read/read_gsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-06-30 13:12:56.000000 nowcasting_datamodel-1.4.8/nowcasting_datamodel/read/read_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-06-30 13:12:56.000000 nowcasting_datamodel-1.4.8/nowcasting_datamodel/read/read_pv.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-30 13:12:56.000000 nowcasting_datamodel-1.4.8/nowcasting_datamodel/read/read_user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:13:06.533167 nowcasting_datamodel-1.4.8/nowcasting_datamodel/save/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-30 13:12:56.000000 nowcasting_datamodel-1.4.8/nowcasting_datamodel/save/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6373 2023-06-30 13:12:56.000000 nowcasting_datamodel-1.4.8/nowcasting_datamodel/save/adjust.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-06-30 13:12:56.000000 nowcasting_datamodel-1.4.8/nowcasting_datamodel/save/save.py
--rw-r--r--   0 runner    (1001) docker     (123)     9569 2023-06-30 13:12:56.000000 nowcasting_datamodel-1.4.8/nowcasting_datamodel/save/update.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-30 13:12:56.000000 nowcasting_datamodel-1.4.8/nowcasting_datamodel/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:13:06.533167 nowcasting_datamodel-1.4.8/nowcasting_datamodel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-06-30 13:13:06.000000 nowcasting_datamodel-1.4.8/nowcasting_datamodel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-06-30 13:13:06.000000 nowcasting_datamodel-1.4.8/nowcasting_datamodel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 13:13:06.000000 nowcasting_datamodel-1.4.8/nowcasting_datamodel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-30 13:13:06.000000 nowcasting_datamodel-1.4.8/nowcasting_datamodel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-30 13:13:06.000000 nowcasting_datamodel-1.4.8/nowcasting_datamodel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-30 13:12:56.000000 nowcasting_datamodel-1.4.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 13:13:06.537167 nowcasting_datamodel-1.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-30 13:12:56.000000 nowcasting_datamodel-1.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:13:06.537167 nowcasting_datamodel-1.4.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-30 13:12:56.000000 nowcasting_datamodel-1.4.8/tests/test_databaseconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-06-30 13:12:56.000000 nowcasting_datamodel-1.4.8/tests/test_fake.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-30 13:12:56.000000 nowcasting_datamodel-1.4.8/tests/test_fake_pv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-30 13:12:56.000000 nowcasting_datamodel-1.4.8/tests/test_national.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-30 13:12:56.000000 nowcasting_datamodel-1.4.8/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:33:26.246409 nowcasting_datamodel-1.4.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-07-03 10:33:26.246409 nowcasting_datamodel-1.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   151651 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/diagram.png
+-rw-r--r--   0 runner    (1001) docker     (123)    49887 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/diagram_pv.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:33:26.242409 nowcasting_datamodel-1.4.9/nowcasting_datamodel/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9558 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/fake.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:33:26.242409 nowcasting_datamodel-1.4.9/nowcasting_datamodel/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/migrations/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:33:26.242409 nowcasting_datamodel-1.4.9/nowcasting_datamodel/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/models/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/models/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18777 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/models/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/models/gsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/models/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/models/pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/national.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:33:26.242409 nowcasting_datamodel-1.4.9/nowcasting_datamodel/read/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/read/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:33:26.246409 nowcasting_datamodel-1.4.9/nowcasting_datamodel/read/blend/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/read/blend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6529 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/read/blend/blend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8282 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/read/blend/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/read/blend/weights.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24247 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/read/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/read/read_gsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/read/read_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/read/read_pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/read/read_user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:33:26.246409 nowcasting_datamodel-1.4.9/nowcasting_datamodel/save/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/save/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6373 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/save/adjust.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/save/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9583 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/save/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:33:26.242409 nowcasting_datamodel-1.4.9/nowcasting_datamodel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-07-03 10:33:26.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-03 10:33:26.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 10:33:26.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-03 10:33:26.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-03 10:33:26.000000 nowcasting_datamodel-1.4.9/nowcasting_datamodel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 10:33:26.246409 nowcasting_datamodel-1.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:33:26.246409 nowcasting_datamodel-1.4.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/tests/test_databaseconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/tests/test_fake.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/tests/test_fake_pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/tests/test_national.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-03 10:33:16.000000 nowcasting_datamodel-1.4.9/tests/test_utils.py
```

### Comparing `nowcasting_datamodel-1.4.8/PKG-INFO` & `nowcasting_datamodel-1.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nowcasting_datamodel
-Version: 1.4.8
+Version: 1.4.9
 Summary: Data Model for the OCF nowcasting project
 Home-page: https://github.com/openclimatefix/nowcasting_datamodel
 Author: Peter Dudfield
 Author-email: peter@openclimatefix.org
 License: MIT
 Keywords: SQL,Datamodel
 Description-Content-Type: text/markdown
```

### Comparing `nowcasting_datamodel-1.4.8/README.md` & `nowcasting_datamodel-1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.8/diagram.png` & `nowcasting_datamodel-1.4.9/diagram.png`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.8/diagram_pv.png` & `nowcasting_datamodel-1.4.9/diagram_pv.png`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.8/nowcasting_datamodel/connection.py` & `nowcasting_datamodel-1.4.9/nowcasting_datamodel/connection.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.8/nowcasting_datamodel/fake.py` & `nowcasting_datamodel-1.4.9/nowcasting_datamodel/fake.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     intensity = make_fake_intensity(target_time)
     power = forecast_maximum * intensity * random_factor
 
     return ForecastValueSQL(
         target_time=target_time,
         expected_power_generation_megawatts=power,
         adjust_mw=0.0,
+        properties={"10": power * 0.9, "90": power * 1.1},
     )
 
 
 def make_fake_forecast(
     gsp_id: int,
     session: Session,
     t0_datetime_utc: Optional[datetime] = None,
```

### Comparing `nowcasting_datamodel-1.4.8/nowcasting_datamodel/migrations/app.py` & `nowcasting_datamodel-1.4.9/nowcasting_datamodel/migrations/app.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.8/nowcasting_datamodel/models/__init__.py` & `nowcasting_datamodel-1.4.9/nowcasting_datamodel/models/__init__.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.8/nowcasting_datamodel/models/api.py` & `nowcasting_datamodel-1.4.9/nowcasting_datamodel/models/api.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.8/nowcasting_datamodel/models/convert.py` & `nowcasting_datamodel-1.4.9/nowcasting_datamodel/models/convert.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,14 +63,16 @@
 ) -> ForecastSQL:
     """
     Make a ForecastSQL object from a dataframe.
 
     :param forecast_values_df: Dataframe containing
         -- target_datetime_utc
         -- forecast_mw
+        -- (Optional) forecast_mw_plevel_10
+        -- (Optional) forecast_mw_plevel_90
     :param: session: database session
     :param: model_name: the name of the model
     :param: version: the version of the model
     :return: forecast object
     """
 
     logger.debug("Converting dataframe to National Forecast")
@@ -93,14 +95,22 @@
         # add timezone
         target_time = forecast_value.target_datetime_utc.replace(tzinfo=timezone.utc)
         forecast_value_sql = ForecastValue(
             target_time=target_time,
             expected_power_generation_megawatts=forecast_value.forecast_mw,
         ).to_orm()
         forecast_value_sql.adjust_mw = 0.0
+
+        forecast_value_sql.properties = {}
+        if "forecast_mw_plevel_10" in forecast_values_df.columns:
+            forecast_value_sql.properties["10"] = forecast_value.forecast_mw_plevel_10
+
+        if "forecast_mw_plevel_90" in forecast_values_df.columns:
+            forecast_value_sql.properties["90"] = forecast_value.forecast_mw_plevel_90
+
         forecast_values.append(forecast_value_sql)
 
     # make forecast object
     forecast = ForecastSQL(
         model=model,
         forecast_creation_time=datetime.now(tz=timezone.utc),
         location=location,
```

### Comparing `nowcasting_datamodel-1.4.8/nowcasting_datamodel/models/forecast.py` & `nowcasting_datamodel-1.4.9/nowcasting_datamodel/models/forecast.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,26 +8,28 @@
 
 import logging
 from datetime import datetime
 from typing import List
 
 from pydantic import Field, validator
 from sqlalchemy import (
+    JSON,
     Boolean,
     Column,
     DateTime,
     Float,
     ForeignKey,
     Index,
     Integer,
     event,
     func,
 )
 from sqlalchemy.dialects.postgresql import UUID
 from sqlalchemy.ext.declarative import DeclarativeMeta, declared_attr
+from sqlalchemy.ext.mutable import MutableDict
 from sqlalchemy.orm import relationship
 from sqlalchemy.sql.ddl import DDL
 
 from nowcasting_datamodel.models.base import Base_Forecast
 from nowcasting_datamodel.models.gsp import Location
 from nowcasting_datamodel.models.models import InputDataLastUpdated, MLModel
 from nowcasting_datamodel.models.utils import CreatedMixin, EnhancedBaseModel
@@ -108,14 +110,17 @@
     This Mixin is used to create partition tables
     """
 
     uuid = Column(UUID, primary_key=True, server_default=func.gen_random_uuid())
     target_time = Column(DateTime(timezone=True), nullable=False, primary_key=True)
     expected_power_generation_megawatts = Column(Float(precision=6))
     adjust_mw = Column(Float, default=0.0)
+    # this can be used to store any additional information about the forecast, like p_levels.
+    # Want to keep it as json so that we can store different properties for different forecasts
+    properties = Column(MutableDict.as_mutable(JSON), nullable=True)
 
     @declared_attr
     def forecast_id(self):
         """Link with Forecast table"""
         return Column(Integer, ForeignKey("forecast.id"))
 
 
@@ -277,14 +282,17 @@
 
     target_time = Column(DateTime(timezone=True), index=True, primary_key=True)
     expected_power_generation_megawatts = Column(Float(precision=6))
     gsp_id = Column(Integer, index=True, primary_key=True)
     model_id = Column(Integer, index=True, primary_key=True, default=-1)
     is_primary = Column(Boolean, default=True)
     adjust_mw = Column(Float, default=0.0)
+    # this can be used to store any additional information about the forecast, like p_levels.
+    # Want to keep it as json so that we can store different properties for different forecasts
+    properties = Column(MutableDict.as_mutable(JSON), nullable=True)
 
     forecast_id = Column(Integer, ForeignKey("forecast.id"), index=True)
     forecast_latest = relationship("ForecastSQL", back_populates="forecast_values_latest")
 
     Index("index_forecast_value_latest", CreatedMixin.created_utc.desc())
 
 
@@ -306,14 +314,22 @@
     _adjust_mw: float = Field(
         0.0,
         description="The amount that the forecast should be adjusted by, "
         "due to persistence errors. This way we keep the original ML prediction. "
         "The _ at the start means it is not expose in the API",
     )
 
+    # This its better to keep this out of the current pydantic models used by the API.
+    # A new pydantic mode can be made that includes the forecast plevels, perhaps in the API.
+    _properties: dict = Field(
+        None,
+        description="Dictionary to hold properties of the forecast, like p_levels. "
+        "The _ at the start means it is not expose in the API",
+    )
+
     _normalize_target_time = validator("target_time", allow_reuse=True)(datetime_must_have_timezone)
 
     def to_orm(self) -> ForecastValueSQL:
         """Change model to ForecastValueSQL"""
         return ForecastValueSQL(
             target_time=self.target_time,
             expected_power_generation_megawatts=self.expected_power_generation_megawatts,
```

### Comparing `nowcasting_datamodel-1.4.8/nowcasting_datamodel/models/gsp.py` & `nowcasting_datamodel-1.4.9/nowcasting_datamodel/models/gsp.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,16 +49,14 @@
     gsp_name: Optional[str] = Field(None, description="The GSP name")
     gsp_group: Optional[str] = Field(None, description="The GSP group name")
     region_name: Optional[str] = Field(None, description="The GSP region name")
     installed_capacity_mw: Optional[float] = Field(
         None, description="The installed capacity of the GSP in MW"
     )
 
-    rm_mode = True
-
     def to_orm(self) -> LocationSQL:
         """Change model to LocationSQL"""
 
         if isinstance(self, LocationSQL):
             return self
 
         return LocationSQL(
```

### Comparing `nowcasting_datamodel-1.4.8/nowcasting_datamodel/models/metric.py` & `nowcasting_datamodel-1.4.9/nowcasting_datamodel/models/metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,16 +37,14 @@
 
 class Metric(EnhancedBaseModel):
     """Metric metadata"""
 
     name: str = Field(..., description="The name of the metric")
     description: str = Field(..., description="The description of the metric")
 
-    rm_mode = True
-
     def to_orm(self) -> MetricSQL:
         """Change model to LocationSQL"""
 
         if isinstance(self, MetricSQL):
             return self
 
         return MetricSQL(
@@ -166,16 +164,14 @@
     time_of_day: time = Field(None, description="the time of tday for this metric")
     metric: Metric = Field(..., description="The metric this value is about")
     datetime_interval: DatetimeInterval = Field(
         ..., description="The datetime interval this value is about"
     )
     location: Location = Field(..., description="The location object for this metric value")
 
-    rm_mode = True
-
     def to_orm(self) -> MetricValueSQL:
         """Change model to MetricValueSQL"""
 
         if isinstance(self, MetricValueSQL):
             return self
 
         return MetricValueSQL(
```

### Comparing `nowcasting_datamodel-1.4.8/nowcasting_datamodel/models/models.py` & `nowcasting_datamodel-1.4.9/nowcasting_datamodel/models/models.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.8/nowcasting_datamodel/models/pv.py` & `nowcasting_datamodel-1.4.9/nowcasting_datamodel/models/pv.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.8/nowcasting_datamodel/models/utils.py` & `nowcasting_datamodel-1.4.9/nowcasting_datamodel/models/utils.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.8/nowcasting_datamodel/national.py` & `nowcasting_datamodel-1.4.9/nowcasting_datamodel/national.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.8/nowcasting_datamodel/read/blend/utils.py` & `nowcasting_datamodel-1.4.9/nowcasting_datamodel/read/blend/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         logger.debug("using all forecasts as all are older than 2 hours")
         forecast_values_all_model_valid = forecast_values_all_model
     return forecast_values_all_model_valid
 
 
 def convert_list_forecast_values_to_df(forecast_values_all_model_valid):
     """
-    Conert list of forecast values to a pandas dataframe
+    Convert list of forecast values to a pandas dataframe
 
     :param forecast_values_all_model_valid:
     :return: merged into pandas dataframe with columns
      - "expected_power_generation_megawatts",
      - "adjust_mw",
      - "created_utc",
      - "model_name",
@@ -62,58 +62,61 @@
 
         values_list = [
             [
                 value.target_time,
                 value.expected_power_generation_megawatts,
                 value.adjust_mw,
                 value.created_utc,
+                value.properties,
                 model_name,
             ]
             for value in forecast_values_one_model
         ]
         value_df = pd.DataFrame(
             values_list,
             columns=[
                 "target_time",
                 "expected_power_generation_megawatts",
                 "adjust_mw",
                 "created_utc",
+                "properties",
                 "model_name",
             ],
         )
         value_df.reset_index(inplace=True, drop=False)
         forecast_values_all_model_df.append(value_df)
     # join into one dataframe
     forecast_values_all_model = pd.concat(forecast_values_all_model_df, axis=0)
     forecast_values_all_model.reset_index(inplace=True)
+
     return forecast_values_all_model
 
 
 def convert_df_to_list_forecast_values(forecast_values_blended):
     """
     Convert the blended dataframe to a list of ForecastValue objects
 
     :param forecast_values_blended: Needs to have the columns 'target_time'
         and 'expected_power_generation_megawatts
     :return:
     """
-    # change in to list of ForecastValue objects
     forecast_values = []
     logger.debug(forecast_values_blended)
     for i, row in forecast_values_blended.iterrows():
         # make sure we don't have negative values
         expected_power_generation_megawatts = row.expected_power_generation_megawatts
         if expected_power_generation_megawatts < 0:
             expected_power_generation_megawatts = 0
 
         forecast_value = ForecastValue(
             target_time=row.target_time,
             expected_power_generation_megawatts=expected_power_generation_megawatts,
         )
         forecast_value._adjust_mw = row.adjust_mw
+        forecast_value._properties = row.properties
         forecast_values.append(forecast_value)
     return forecast_values
 
 
 def blend_forecasts_together(forecast_values_all_model, weights_df):
     """
     Blend the forecasts together using the weights_df
@@ -122,39 +125,49 @@
         'expected_power_generation_megawatts', 'adjust_mw', 'model_name'
     :param weights_df: Dataframe of weights with columns 'model_name' and 'weight'
     :return: Dataframe with the columns
         'target_time',
         'expected_power_generation_megawatts',
         'adjust_mw'
     """
+
+    # drop of the "properties" column
+    if "properties" in forecast_values_all_model.columns:
+        forecast_values_all_model = forecast_values_all_model.drop(columns=["properties"]).copy()
+
     # blend together
     # lets deal with unique target times first
     logger.debug(forecast_values_all_model["target_time"])
     # get all unique target times
     all_target_times = forecast_values_all_model["target_time"].unique()
     logger.debug(f"Found in total {len(all_target_times)} target times")
+
     # get the duplicated target times
     duplicated_target_times = forecast_values_all_model[
         forecast_values_all_model["target_time"].duplicated()
     ]["target_time"].tolist()
     logger.debug(f"Found {len(duplicated_target_times)} duplicated target times")
     unique_target_times = [x for x in all_target_times if x not in duplicated_target_times]
     logger.debug(f"Found in {len(unique_target_times)} unique target times")
+
     # get the index of the duplicated and unique target times
     duplicated_target_times_idx = forecast_values_all_model[
         forecast_values_all_model["target_time"].isin(duplicated_target_times)
     ].index
     unique_target_times_idx = forecast_values_all_model[
         forecast_values_all_model["target_time"].isin(unique_target_times)
     ].index
+
     # get the unique forecast values
     forecast_values_blended = forecast_values_all_model.loc[unique_target_times_idx]
+
     # now lets deal with the weights
     duplicated = forecast_values_all_model.loc[duplicated_target_times_idx]
     duplicated = duplicated.drop_duplicates()
+
     # only do this if there are duplicated
     if len(duplicated) > 0:
         logger.debug(f"Now blending the duplicated target times using {weights_df}")
 
         pd.DataFrame()
         # unstack the weights
         weights_one_df = weights_df.stack()
@@ -169,30 +182,28 @@
             weights_one_df,
             how="left",
             left_on=["model_name", "target_time"],
             right_on=["model_name", "target_time"],
         )
 
         # multiply the expected power generation by the weight
-        duplicated["expected_power_generation_megawatts"] = (
-            duplicated["expected_power_generation_megawatts"] * duplicated["weight"]
-        )
-        duplicated["adjust_mw"] = duplicated["adjust_mw"] * duplicated["weight"]
+        for col in ["expected_power_generation_megawatts", "adjust_mw"]:
+            duplicated[col] = duplicated[col] * duplicated["weight"]
         duplicated.drop(columns=["created_utc"], inplace=True)
 
         # sum the weights
         duplicated = duplicated.groupby(["target_time"]).sum()
 
         # make sure target_time is a columns
         duplicated["target_time"] = duplicated.index
         duplicated.reset_index(inplace=True, drop=True)
 
         # divide by the sum of the weights, # TODO should we be worried about dividing by zero?
-        duplicated["expected_power_generation_megawatts"] /= duplicated["weight"]
-        duplicated["adjust_mw"] /= duplicated["weight"]
+        for col in ["expected_power_generation_megawatts", "adjust_mw"]:
+            duplicated[col] /= duplicated["weight"]
 
         logger.debug(duplicated)
     # join unique and duplicates together
     forecast_values_blended = pd.concat([forecast_values_blended, duplicated], axis=0)
     # sort by target time
     forecast_values_blended.sort_values(by="target_time", inplace=True)
     return forecast_values_blended
```

### Comparing `nowcasting_datamodel-1.4.8/nowcasting_datamodel/read/blend/weights.py` & `nowcasting_datamodel-1.4.9/nowcasting_datamodel/read/blend/weights.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.8/nowcasting_datamodel/read/read.py` & `nowcasting_datamodel-1.4.9/nowcasting_datamodel/read/read.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.8/nowcasting_datamodel/read/read_gsp.py` & `nowcasting_datamodel-1.4.9/nowcasting_datamodel/read/read_gsp.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.8/nowcasting_datamodel/read/read_metric.py` & `nowcasting_datamodel-1.4.9/nowcasting_datamodel/read/read_metric.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.8/nowcasting_datamodel/read/read_pv.py` & `nowcasting_datamodel-1.4.9/nowcasting_datamodel/read/read_pv.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.8/nowcasting_datamodel/read/read_user.py` & `nowcasting_datamodel-1.4.9/nowcasting_datamodel/read/read_user.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.8/nowcasting_datamodel/save/adjust.py` & `nowcasting_datamodel-1.4.9/nowcasting_datamodel/save/adjust.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.8/nowcasting_datamodel/save/save.py` & `nowcasting_datamodel-1.4.9/nowcasting_datamodel/save/save.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.8/nowcasting_datamodel/save/update.py` & `nowcasting_datamodel-1.4.9/nowcasting_datamodel/save/update.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,15 @@
     :param gsp_id: gsp id
     :param forecast_id: forecast joining id
     :param model_id: model joining id
     :return: forecast value latest object
     """
 
     forecast_value_dict = {}
-    for v in ["target_time", "expected_power_generation_megawatts", "adjust_mw"]:
+    for v in ["target_time", "expected_power_generation_megawatts", "adjust_mw", "properties"]:
         forecast_value_dict[v] = getattr(forecast_value, v)
 
     forecast_value_dict["gsp_id"] = gsp_id
     if forecast_id is not None:
         forecast_value_dict["forecast_id"] = forecast_id
 
     if model_id is not None:
```

### Comparing `nowcasting_datamodel-1.4.8/nowcasting_datamodel/utils.py` & `nowcasting_datamodel-1.4.9/nowcasting_datamodel/utils.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.8/nowcasting_datamodel.egg-info/PKG-INFO` & `nowcasting_datamodel-1.4.9/nowcasting_datamodel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nowcasting-datamodel
-Version: 1.4.8
+Version: 1.4.9
 Summary: Data Model for the OCF nowcasting project
 Home-page: https://github.com/openclimatefix/nowcasting_datamodel
 Author: Peter Dudfield
 Author-email: peter@openclimatefix.org
 License: MIT
 Keywords: SQL,Datamodel
 Description-Content-Type: text/markdown
```

### Comparing `nowcasting_datamodel-1.4.8/nowcasting_datamodel.egg-info/SOURCES.txt` & `nowcasting_datamodel-1.4.9/nowcasting_datamodel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.8/setup.py` & `nowcasting_datamodel-1.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.8/tests/test_databaseconnection.py` & `nowcasting_datamodel-1.4.9/tests/test_databaseconnection.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.8/tests/test_fake.py` & `nowcasting_datamodel-1.4.9/tests/test_fake.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.8/tests/test_fake_pv.py` & `nowcasting_datamodel-1.4.9/tests/test_fake_pv.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.8/tests/test_national.py` & `nowcasting_datamodel-1.4.9/tests/test_national.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.8/tests/test_utils.py` & `nowcasting_datamodel-1.4.9/tests/test_utils.py`

 * *Files identical despite different names*

