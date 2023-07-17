# Comparing `tmp/ContactApi-0.0.6.tar.gz` & `tmp/ContactApi-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ContactApi-0.0.6.tar", last modified: Mon Jul 17 14:26:36 2023, max compression
+gzip compressed data, was "ContactApi-0.0.7.tar", last modified: Mon Jul 17 14:28:56 2023, max compression
```

## Comparing `ContactApi-0.0.6.tar` & `ContactApi-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:26:36.631811 ContactApi-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-17 14:26:36.631811 ContactApi-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-17 14:26:24.000000 ContactApi-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-17 14:26:24.000000 ContactApi-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 14:26:36.631811 ContactApi-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:26:36.631811 ContactApi-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:26:36.631811 ContactApi-0.0.6/src/ContactApi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-17 14:26:36.000000 ContactApi-0.0.6/src/ContactApi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-17 14:26:36.000000 ContactApi-0.0.6/src/ContactApi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 14:26:36.000000 ContactApi-0.0.6/src/ContactApi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-17 14:26:36.000000 ContactApi-0.0.6/src/ContactApi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-17 14:26:36.000000 ContactApi-0.0.6/src/ContactApi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-17 14:26:36.000000 ContactApi-0.0.6/src/ContactApi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:26:24.000000 ContactApi-0.0.6/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-17 14:26:24.000000 ContactApi-0.0.6/src/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-17 14:26:24.000000 ContactApi-0.0.6/src/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-17 14:26:24.000000 ContactApi-0.0.6/src/crud.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-17 14:26:24.000000 ContactApi-0.0.6/src/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-17 14:26:24.000000 ContactApi-0.0.6/src/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-17 14:26:24.000000 ContactApi-0.0.6/src/router.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-17 14:26:24.000000 ContactApi-0.0.6/src/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:28:56.420920 ContactApi-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-17 14:28:56.420920 ContactApi-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-17 14:28:43.000000 ContactApi-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-17 14:28:44.000000 ContactApi-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 14:28:56.420920 ContactApi-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:28:56.416920 ContactApi-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:28:56.420920 ContactApi-0.0.7/src/ContactApi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-17 14:28:56.000000 ContactApi-0.0.7/src/ContactApi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-17 14:28:56.000000 ContactApi-0.0.7/src/ContactApi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 14:28:56.000000 ContactApi-0.0.7/src/ContactApi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-17 14:28:56.000000 ContactApi-0.0.7/src/ContactApi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-17 14:28:56.000000 ContactApi-0.0.7/src/ContactApi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-17 14:28:56.000000 ContactApi-0.0.7/src/ContactApi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:28:43.000000 ContactApi-0.0.7/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-17 14:28:43.000000 ContactApi-0.0.7/src/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-17 14:28:43.000000 ContactApi-0.0.7/src/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-17 14:28:43.000000 ContactApi-0.0.7/src/crud.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-17 14:28:43.000000 ContactApi-0.0.7/src/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-17 14:28:43.000000 ContactApi-0.0.7/src/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-17 14:28:43.000000 ContactApi-0.0.7/src/router.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-17 14:28:43.000000 ContactApi-0.0.7/src/schemas.py
```

### Comparing `ContactApi-0.0.6/PKG-INFO` & `ContactApi-0.0.7/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ContactApi
-Version: 0.0.6
+Version: 0.0.7
 Summary: Just a demo project
 Keywords: flask,project
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # fastapi
```

### Comparing `ContactApi-0.0.6/README.md` & `ContactApi-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ContactApi-0.0.6/src/ContactApi.egg-info/PKG-INFO` & `ContactApi-0.0.7/src/ContactApi.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ContactApi
-Version: 0.0.6
+Version: 0.0.7
 Summary: Just a demo project
 Keywords: flask,project
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # fastapi
```

### Comparing `ContactApi-0.0.6/src/config.py` & `ContactApi-0.0.7/src/config.py`

 * *Files identical despite different names*

### Comparing `ContactApi-0.0.6/src/crud.py` & `ContactApi-0.0.7/src/crud.py`

 * *Files identical despite different names*

### Comparing `ContactApi-0.0.6/src/router.py` & `ContactApi-0.0.7/src/router.py`

 * *Files identical despite different names*

