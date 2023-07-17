# Comparing `tmp/ContactApi-0.0.3.tar.gz` & `tmp/ContactApi-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ContactApi-0.0.3.tar", last modified: Sat Jul 15 15:12:12 2023, max compression
+gzip compressed data, was "ContactApi-0.0.4.tar", last modified: Mon Jul 17 13:49:00 2023, max compression
```

## Comparing `ContactApi-0.0.3.tar` & `ContactApi-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:12:12.273049 ContactApi-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-15 15:12:12.269049 ContactApi-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-15 15:11:56.000000 ContactApi-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-15 15:11:57.000000 ContactApi-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 15:12:12.273049 ContactApi-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:12:12.269049 ContactApi-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:12:12.269049 ContactApi-0.0.3/src/ContactApi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-15 15:12:12.000000 ContactApi-0.0.3/src/ContactApi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-15 15:12:12.000000 ContactApi-0.0.3/src/ContactApi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 15:12:12.000000 ContactApi-0.0.3/src/ContactApi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-15 15:12:12.000000 ContactApi-0.0.3/src/ContactApi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-15 15:12:12.000000 ContactApi-0.0.3/src/ContactApi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-15 15:12:12.000000 ContactApi-0.0.3/src/ContactApi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 15:11:56.000000 ContactApi-0.0.3/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-15 15:11:56.000000 ContactApi-0.0.3/src/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-15 15:11:56.000000 ContactApi-0.0.3/src/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-15 15:11:56.000000 ContactApi-0.0.3/src/crud.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-15 15:11:56.000000 ContactApi-0.0.3/src/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-15 15:11:56.000000 ContactApi-0.0.3/src/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-15 15:11:56.000000 ContactApi-0.0.3/src/router.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-15 15:11:56.000000 ContactApi-0.0.3/src/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:49:00.638869 ContactApi-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-17 13:49:00.638869 ContactApi-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-17 13:48:47.000000 ContactApi-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-17 13:48:47.000000 ContactApi-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 13:49:00.638869 ContactApi-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:49:00.634869 ContactApi-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:49:00.638869 ContactApi-0.0.4/src/ContactApi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-17 13:49:00.000000 ContactApi-0.0.4/src/ContactApi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-17 13:49:00.000000 ContactApi-0.0.4/src/ContactApi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 13:49:00.000000 ContactApi-0.0.4/src/ContactApi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-17 13:49:00.000000 ContactApi-0.0.4/src/ContactApi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-17 13:49:00.000000 ContactApi-0.0.4/src/ContactApi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-17 13:49:00.000000 ContactApi-0.0.4/src/ContactApi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 13:48:47.000000 ContactApi-0.0.4/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-17 13:48:47.000000 ContactApi-0.0.4/src/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-17 13:48:47.000000 ContactApi-0.0.4/src/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-17 13:48:47.000000 ContactApi-0.0.4/src/crud.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-17 13:48:47.000000 ContactApi-0.0.4/src/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-17 13:48:47.000000 ContactApi-0.0.4/src/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-17 13:48:47.000000 ContactApi-0.0.4/src/router.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-17 13:48:47.000000 ContactApi-0.0.4/src/schemas.py
```

### Comparing `ContactApi-0.0.3/PKG-INFO` & `ContactApi-0.0.4/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,23 @@
-Metadata-Version: 2.1
-Name: ContactApi
-Version: 0.0.3
-Summary: Just a demo project
-Keywords: flask,project
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-
 # fastapi
 
 # Runing app with docker
 
+export POSTGRES_CONTAINER="postgresdb"
+
 export DB_PASS="password"
 
-export DATABASE_URL="postgresql://postgres:$DB_PASS@localhost:5432"
+export DATABASE_URL="postgresql://postgres:$DB_PASS@$POSTGRES_CONTAINER:5432"
 
-podman create network contactapi
+podman network create contactapi
 
 podman pull docker.io/library/postgres
 
 podman pull ghcr.io/yulai202020/contactapi
 
 podman images
 
-podman run --network contactapi -e POSTGRES_PASSWORD=$DB_PASS -d --name postgresdb docker.io/library/postgres
+podman run --network contactapi -e POSTGRES_PASSWORD=$DB_PASS -d --name $POSTGRES_CONTAINER docker.io/library/postgres
 
 podman run --network contactapi -e DATABASE_URL=$DATABASE_URL -p 8000:8000 -d ghcr.io/yulai202020/contactapi 
 
-podman ps
+podman ps
```

### Comparing `ContactApi-0.0.3/src/config.py` & `ContactApi-0.0.4/src/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,17 @@
 import os
 from sqlalchemy.orm import sessionmaker
 from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy import MetaData, create_engine, Table, Column, Integer, String
-from dotenv import load_dotenv
 
-load_dotenv()
 database_url = os.environ.get("DATABASE_URL")
 
 base = declarative_base()
 engine = create_engine(database_url)
-
-try:
-    engine = create_engine(database_url)
-except:
-    print("DATABASE_URL does not exists.")
-    print('(Example DATABASE_URL=postgresql://postgres:P*ss*ord@localhost:5432")')
-    exit(1)
+engine = create_engine(database_url)
 
 SessionLocal = sessionmaker(autocommit=False, autoflush=False, bind=engine)
 
 meta = MetaData()
 
 person = Table(
     "person",
```

### Comparing `ContactApi-0.0.3/src/crud.py` & `ContactApi-0.0.4/src/crud.py`

 * *Files identical despite different names*

### Comparing `ContactApi-0.0.3/src/router.py` & `ContactApi-0.0.4/src/router.py`

 * *Files identical despite different names*

