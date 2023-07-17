# Comparing `tmp/PVNet-2.1.8.tar.gz` & `tmp/PVNet-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PVNet-2.1.8.tar", last modified: Mon Jul 10 10:20:34 2023, max compression
+gzip compressed data, was "PVNet-2.1.9.tar", last modified: Tue Jul 11 13:02:14 2023, max compression
```

## Comparing `PVNet-2.1.8.tar` & `PVNet-2.1.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:20:34.405094 PVNet-2.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-10 10:20:24.000000 PVNet-2.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-10 10:20:24.000000 PVNet-2.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-10 10:20:34.405094 PVNet-2.1.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:20:34.405094 PVNet-2.1.8/PVNet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-10 10:20:34.000000 PVNet-2.1.8/PVNet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-10 10:20:34.000000 PVNet-2.1.8/PVNet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 10:20:34.000000 PVNet-2.1.8/PVNet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-10 10:20:34.000000 PVNet-2.1.8/PVNet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-10 10:20:34.000000 PVNet-2.1.8/PVNet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-10 10:20:24.000000 PVNet-2.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:20:34.405094 PVNet-2.1.8/pvnet/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-10 10:20:24.000000 PVNet-2.1.8/pvnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13611 2023-07-10 10:20:24.000000 PVNet-2.1.8/pvnet/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-07-10 10:20:24.000000 PVNet-2.1.8/pvnet/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-10 10:20:24.000000 PVNet-2.1.8/pvnet/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-07-10 10:20:24.000000 PVNet-2.1.8/pvnet/training.py
--rw-r--r--   0 runner    (1001) docker     (123)    10158 2023-07-10 10:20:24.000000 PVNet-2.1.8/pvnet/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-10 10:20:24.000000 PVNet-2.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-10 10:20:24.000000 PVNet-2.1.8/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-10 10:20:24.000000 PVNet-2.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 10:20:34.405094 PVNet-2.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-10 10:20:24.000000 PVNet-2.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:20:34.405094 PVNet-2.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 10:20:24.000000 PVNet-2.1.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-07-10 10:20:24.000000 PVNet-2.1.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-10 10:20:24.000000 PVNet-2.1.8/tests/test_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:02:14.228193 PVNet-2.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-11 13:02:01.000000 PVNet-2.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-11 13:02:01.000000 PVNet-2.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-11 13:02:14.228193 PVNet-2.1.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:02:14.228193 PVNet-2.1.9/PVNet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-11 13:02:14.000000 PVNet-2.1.9/PVNet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-11 13:02:14.000000 PVNet-2.1.9/PVNet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 13:02:14.000000 PVNet-2.1.9/PVNet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-11 13:02:14.000000 PVNet-2.1.9/PVNet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-11 13:02:14.000000 PVNet-2.1.9/PVNet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-11 13:02:01.000000 PVNet-2.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:02:14.228193 PVNet-2.1.9/pvnet/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-11 13:02:01.000000 PVNet-2.1.9/pvnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13611 2023-07-11 13:02:01.000000 PVNet-2.1.9/pvnet/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-07-11 13:02:01.000000 PVNet-2.1.9/pvnet/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-11 13:02:01.000000 PVNet-2.1.9/pvnet/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-07-11 13:02:01.000000 PVNet-2.1.9/pvnet/training.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10158 2023-07-11 13:02:01.000000 PVNet-2.1.9/pvnet/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-11 13:02:01.000000 PVNet-2.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-11 13:02:01.000000 PVNet-2.1.9/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-11 13:02:01.000000 PVNet-2.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 13:02:14.228193 PVNet-2.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-11 13:02:01.000000 PVNet-2.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:02:14.228193 PVNet-2.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 13:02:01.000000 PVNet-2.1.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-07-11 13:02:01.000000 PVNet-2.1.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-11 13:02:02.000000 PVNet-2.1.9/tests/test_app.py
```

### Comparing `PVNet-2.1.8/LICENSE` & `PVNet-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `PVNet-2.1.8/PKG-INFO` & `PVNet-2.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PVNet
-Version: 2.1.8
+Version: 2.1.9
 Summary: PVNet
 Author: Peter Dudfield
 Author-email: info@openclimatefix.org
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: all_models
 License-File: LICENSE
```

### Comparing `PVNet-2.1.8/PVNet.egg-info/PKG-INFO` & `PVNet-2.1.9/PVNet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PVNet
-Version: 2.1.8
+Version: 2.1.9
 Summary: PVNet
 Author: Peter Dudfield
 Author-email: info@openclimatefix.org
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: all_models
 License-File: LICENSE
```

### Comparing `PVNet-2.1.8/README.md` & `PVNet-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `PVNet-2.1.8/pvnet/app.py` & `PVNet-2.1.9/pvnet/app.py`

 * *Files identical despite different names*

### Comparing `PVNet-2.1.8/pvnet/callbacks.py` & `PVNet-2.1.9/pvnet/callbacks.py`

 * *Files identical despite different names*

### Comparing `PVNet-2.1.8/pvnet/optimizers.py` & `PVNet-2.1.9/pvnet/optimizers.py`

 * *Files identical despite different names*

### Comparing `PVNet-2.1.8/pvnet/training.py` & `PVNet-2.1.9/pvnet/training.py`

 * *Files identical despite different names*

### Comparing `PVNet-2.1.8/pvnet/utils.py` & `PVNet-2.1.9/pvnet/utils.py`

 * *Files identical despite different names*

### Comparing `PVNet-2.1.8/setup.py` & `PVNet-2.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `PVNet-2.1.8/tests/conftest.py` & `PVNet-2.1.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `PVNet-2.1.8/tests/test_app.py` & `PVNet-2.1.9/tests/test_app.py`

 * *Files identical despite different names*

