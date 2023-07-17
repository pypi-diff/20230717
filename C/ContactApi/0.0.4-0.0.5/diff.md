# Comparing `tmp/ContactApi-0.0.4.tar.gz` & `tmp/ContactApi-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ContactApi-0.0.4.tar", last modified: Mon Jul 17 13:49:00 2023, max compression
+gzip compressed data, was "ContactApi-0.0.5.tar", last modified: Mon Jul 17 13:59:39 2023, max compression
```

## Comparing `ContactApi-0.0.4.tar` & `ContactApi-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:49:00.638869 ContactApi-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-17 13:49:00.638869 ContactApi-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-17 13:48:47.000000 ContactApi-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-17 13:48:47.000000 ContactApi-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 13:49:00.638869 ContactApi-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:49:00.634869 ContactApi-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:49:00.638869 ContactApi-0.0.4/src/ContactApi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-17 13:49:00.000000 ContactApi-0.0.4/src/ContactApi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-17 13:49:00.000000 ContactApi-0.0.4/src/ContactApi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 13:49:00.000000 ContactApi-0.0.4/src/ContactApi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-17 13:49:00.000000 ContactApi-0.0.4/src/ContactApi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-17 13:49:00.000000 ContactApi-0.0.4/src/ContactApi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-17 13:49:00.000000 ContactApi-0.0.4/src/ContactApi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 13:48:47.000000 ContactApi-0.0.4/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-17 13:48:47.000000 ContactApi-0.0.4/src/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-17 13:48:47.000000 ContactApi-0.0.4/src/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-17 13:48:47.000000 ContactApi-0.0.4/src/crud.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-17 13:48:47.000000 ContactApi-0.0.4/src/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-17 13:48:47.000000 ContactApi-0.0.4/src/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-17 13:48:47.000000 ContactApi-0.0.4/src/router.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-17 13:48:47.000000 ContactApi-0.0.4/src/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:59:39.612844 ContactApi-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-17 13:59:39.612844 ContactApi-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-17 13:59:26.000000 ContactApi-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-17 13:59:26.000000 ContactApi-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 13:59:39.612844 ContactApi-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:59:39.612844 ContactApi-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:59:39.612844 ContactApi-0.0.5/src/ContactApi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-17 13:59:39.000000 ContactApi-0.0.5/src/ContactApi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-17 13:59:39.000000 ContactApi-0.0.5/src/ContactApi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 13:59:39.000000 ContactApi-0.0.5/src/ContactApi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-17 13:59:39.000000 ContactApi-0.0.5/src/ContactApi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-17 13:59:39.000000 ContactApi-0.0.5/src/ContactApi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-17 13:59:39.000000 ContactApi-0.0.5/src/ContactApi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 13:59:26.000000 ContactApi-0.0.5/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-17 13:59:26.000000 ContactApi-0.0.5/src/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-17 13:59:26.000000 ContactApi-0.0.5/src/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-17 13:59:26.000000 ContactApi-0.0.5/src/crud.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-17 13:59:26.000000 ContactApi-0.0.5/src/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-17 13:59:26.000000 ContactApi-0.0.5/src/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-17 13:59:26.000000 ContactApi-0.0.5/src/router.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-17 13:59:26.000000 ContactApi-0.0.5/src/schemas.py
```

### Comparing `ContactApi-0.0.4/PKG-INFO` & `ContactApi-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ContactApi
-Version: 0.0.4
+Version: 0.0.5
 Summary: Just a demo project
 Keywords: flask,project
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # fastapi
```

### Comparing `ContactApi-0.0.4/README.md` & `ContactApi-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ContactApi-0.0.4/src/ContactApi.egg-info/PKG-INFO` & `ContactApi-0.0.5/src/ContactApi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ContactApi
-Version: 0.0.4
+Version: 0.0.5
 Summary: Just a demo project
 Keywords: flask,project
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # fastapi
```

### Comparing `ContactApi-0.0.4/src/config.py` & `ContactApi-0.0.5/src/config.py`

 * *Files identical despite different names*

### Comparing `ContactApi-0.0.4/src/crud.py` & `ContactApi-0.0.5/src/crud.py`

 * *Files identical despite different names*

### Comparing `ContactApi-0.0.4/src/router.py` & `ContactApi-0.0.5/src/router.py`

 * *Files identical despite different names*

