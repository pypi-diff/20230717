# Comparing `tmp/ContactApi-0.0.8.tar.gz` & `tmp/ContactApi-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ContactApi-0.0.8.tar", last modified: Mon Jul 17 14:58:32 2023, max compression
+gzip compressed data, was "ContactApi-0.0.9.tar", last modified: Mon Jul 17 15:00:45 2023, max compression
```

## Comparing `ContactApi-0.0.8.tar` & `ContactApi-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:58:32.983294 ContactApi-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-17 14:58:32.983294 ContactApi-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-17 14:58:22.000000 ContactApi-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-17 14:58:22.000000 ContactApi-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 14:58:32.983294 ContactApi-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:58:32.983294 ContactApi-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:58:32.983294 ContactApi-0.0.8/src/ContactApi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-17 14:58:32.000000 ContactApi-0.0.8/src/ContactApi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-17 14:58:32.000000 ContactApi-0.0.8/src/ContactApi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 14:58:32.000000 ContactApi-0.0.8/src/ContactApi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-17 14:58:32.000000 ContactApi-0.0.8/src/ContactApi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-17 14:58:32.000000 ContactApi-0.0.8/src/ContactApi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-17 14:58:32.000000 ContactApi-0.0.8/src/ContactApi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:58:22.000000 ContactApi-0.0.8/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-17 14:58:22.000000 ContactApi-0.0.8/src/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-17 14:58:22.000000 ContactApi-0.0.8/src/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-17 14:58:22.000000 ContactApi-0.0.8/src/crud.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-17 14:58:22.000000 ContactApi-0.0.8/src/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-17 14:58:22.000000 ContactApi-0.0.8/src/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-17 14:58:22.000000 ContactApi-0.0.8/src/router.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-17 14:58:22.000000 ContactApi-0.0.8/src/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:00:45.361878 ContactApi-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-17 15:00:45.361878 ContactApi-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-17 15:00:28.000000 ContactApi-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-17 15:00:28.000000 ContactApi-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 15:00:45.361878 ContactApi-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:00:45.357878 ContactApi-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:00:45.361878 ContactApi-0.0.9/src/ContactApi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-17 15:00:45.000000 ContactApi-0.0.9/src/ContactApi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-17 15:00:45.000000 ContactApi-0.0.9/src/ContactApi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 15:00:45.000000 ContactApi-0.0.9/src/ContactApi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-17 15:00:45.000000 ContactApi-0.0.9/src/ContactApi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-17 15:00:45.000000 ContactApi-0.0.9/src/ContactApi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-17 15:00:45.000000 ContactApi-0.0.9/src/ContactApi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:00:28.000000 ContactApi-0.0.9/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-17 15:00:28.000000 ContactApi-0.0.9/src/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-17 15:00:28.000000 ContactApi-0.0.9/src/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-17 15:00:28.000000 ContactApi-0.0.9/src/crud.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-17 15:00:28.000000 ContactApi-0.0.9/src/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-17 15:00:28.000000 ContactApi-0.0.9/src/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-17 15:00:28.000000 ContactApi-0.0.9/src/router.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-17 15:00:28.000000 ContactApi-0.0.9/src/schemas.py
```

### Comparing `ContactApi-0.0.8/PKG-INFO` & `ContactApi-0.0.9/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-Metadata-Version: 2.1
-Name: ContactApi
-Version: 0.0.8
-Summary: Just a demo project
-Keywords: flask,project
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-
 # fastapi
 
 # Runing app with docker
 
 export POSTGRES_CONTAINER="postgresdb"
 
 export DB_PASS="password"
@@ -24,8 +16,8 @@
 
 podman images
 
 podman run --network contactapi -e POSTGRES_PASSWORD=$DB_PASS -d --name $POSTGRES_CONTAINER docker.io/library/postgres
 
 podman run --network contactapi -e DATABASE_URL=$DATABASE_URL -p 8000:8000 -d ghcr.io/yulai202020/contactapi 
 
-podman ps
+podman ps
```

### Comparing `ContactApi-0.0.8/src/config.py` & `ContactApi-0.0.9/src/config.py`

 * *Files identical despite different names*

### Comparing `ContactApi-0.0.8/src/crud.py` & `ContactApi-0.0.9/src/crud.py`

 * *Files identical despite different names*

### Comparing `ContactApi-0.0.8/src/router.py` & `ContactApi-0.0.9/src/router.py`

 * *Files identical despite different names*

