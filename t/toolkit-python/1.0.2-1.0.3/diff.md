# Comparing `tmp/toolkit_python-1.0.2.tar.gz` & `tmp/toolkit_python-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolkit_python-1.0.2.tar", last modified: Mon Jul 17 13:04:32 2023, max compression
+gzip compressed data, was "toolkit_python-1.0.3.tar", last modified: Mon Jul 17 13:15:01 2023, max compression
```

## Comparing `toolkit_python-1.0.2.tar` & `toolkit_python-1.0.3.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:04:32.751095 toolkit_python-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-17 13:04:32.751095 toolkit_python-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-17 13:04:29.000000 toolkit_python-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 13:04:32.751095 toolkit_python-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-17 13:04:31.000000 toolkit_python-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:04:32.751095 toolkit_python-1.0.2/toolkit_python/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-17 13:04:29.000000 toolkit_python-1.0.2/toolkit_python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:04:32.751095 toolkit_python-1.0.2/toolkit_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-17 13:04:32.000000 toolkit_python-1.0.2/toolkit_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-17 13:04:32.000000 toolkit_python-1.0.2/toolkit_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 13:04:32.000000 toolkit_python-1.0.2/toolkit_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-17 13:04:32.000000 toolkit_python-1.0.2/toolkit_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:15:01.176873 toolkit_python-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-17 13:15:01.176873 toolkit_python-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-17 13:14:58.000000 toolkit_python-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 13:15:01.176873 toolkit_python-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-17 13:15:00.000000 toolkit_python-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:15:01.176873 toolkit_python-1.0.3/toolkit_python/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 13:14:58.000000 toolkit_python-1.0.3/toolkit_python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:15:01.176873 toolkit_python-1.0.3/toolkit_python/generic_services/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-17 13:14:58.000000 toolkit_python-1.0.3/toolkit_python/generic_services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-17 13:14:58.000000 toolkit_python-1.0.3/toolkit_python/generic_services/app_generic_service_sqlalchemy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:15:01.176873 toolkit_python-1.0.3/toolkit_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-17 13:15:01.000000 toolkit_python-1.0.3/toolkit_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-17 13:15:01.000000 toolkit_python-1.0.3/toolkit_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 13:15:01.000000 toolkit_python-1.0.3/toolkit_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-17 13:15:01.000000 toolkit_python-1.0.3/toolkit_python.egg-info/top_level.txt
```

