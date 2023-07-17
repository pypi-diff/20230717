# Comparing `tmp/toolkit_python-1.0.3.tar.gz` & `tmp/toolkit_python-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolkit_python-1.0.3.tar", last modified: Mon Jul 17 13:15:01 2023, max compression
+gzip compressed data, was "toolkit_python-1.0.4.tar", last modified: Mon Jul 17 13:19:31 2023, max compression
```

## Comparing `toolkit_python-1.0.3.tar` & `toolkit_python-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:15:01.176873 toolkit_python-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-17 13:15:01.176873 toolkit_python-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-17 13:14:58.000000 toolkit_python-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 13:15:01.176873 toolkit_python-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-17 13:15:00.000000 toolkit_python-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:15:01.176873 toolkit_python-1.0.3/toolkit_python/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 13:14:58.000000 toolkit_python-1.0.3/toolkit_python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:15:01.176873 toolkit_python-1.0.3/toolkit_python/generic_services/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-17 13:14:58.000000 toolkit_python-1.0.3/toolkit_python/generic_services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-17 13:14:58.000000 toolkit_python-1.0.3/toolkit_python/generic_services/app_generic_service_sqlalchemy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:15:01.176873 toolkit_python-1.0.3/toolkit_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-17 13:15:01.000000 toolkit_python-1.0.3/toolkit_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-17 13:15:01.000000 toolkit_python-1.0.3/toolkit_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 13:15:01.000000 toolkit_python-1.0.3/toolkit_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-17 13:15:01.000000 toolkit_python-1.0.3/toolkit_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:19:31.611101 toolkit_python-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-17 13:19:31.611101 toolkit_python-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-17 13:19:28.000000 toolkit_python-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 13:19:31.611101 toolkit_python-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-17 13:19:30.000000 toolkit_python-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:19:31.607102 toolkit_python-1.0.4/toolkit_python/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 13:19:28.000000 toolkit_python-1.0.4/toolkit_python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:19:31.611101 toolkit_python-1.0.4/toolkit_python/generic_services/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-17 13:19:28.000000 toolkit_python-1.0.4/toolkit_python/generic_services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-17 13:19:28.000000 toolkit_python-1.0.4/toolkit_python/generic_services/app_generic_service_sqlalchemy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:19:31.611101 toolkit_python-1.0.4/toolkit_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-17 13:19:31.000000 toolkit_python-1.0.4/toolkit_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-17 13:19:31.000000 toolkit_python-1.0.4/toolkit_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 13:19:31.000000 toolkit_python-1.0.4/toolkit_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-17 13:19:31.000000 toolkit_python-1.0.4/toolkit_python.egg-info/top_level.txt
```

