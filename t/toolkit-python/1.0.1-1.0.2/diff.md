# Comparing `tmp/toolkit_python-1.0.1.tar.gz` & `tmp/toolkit_python-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolkit_python-1.0.1.tar", last modified: Mon Jul 17 12:54:34 2023, max compression
+gzip compressed data, was "toolkit_python-1.0.2.tar", last modified: Mon Jul 17 13:04:32 2023, max compression
```

## Comparing `toolkit_python-1.0.1.tar` & `toolkit_python-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:54:34.861045 toolkit_python-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-17 12:54:34.861045 toolkit_python-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-17 12:54:32.000000 toolkit_python-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 12:54:34.861045 toolkit_python-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-17 12:54:34.000000 toolkit_python-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:54:34.861045 toolkit_python-1.0.1/toolkit_python/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-17 12:54:32.000000 toolkit_python-1.0.1/toolkit_python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:54:34.861045 toolkit_python-1.0.1/toolkit_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-17 12:54:34.000000 toolkit_python-1.0.1/toolkit_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-17 12:54:34.000000 toolkit_python-1.0.1/toolkit_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 12:54:34.000000 toolkit_python-1.0.1/toolkit_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-17 12:54:34.000000 toolkit_python-1.0.1/toolkit_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:04:32.751095 toolkit_python-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-17 13:04:32.751095 toolkit_python-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-17 13:04:29.000000 toolkit_python-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 13:04:32.751095 toolkit_python-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-17 13:04:31.000000 toolkit_python-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:04:32.751095 toolkit_python-1.0.2/toolkit_python/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-17 13:04:29.000000 toolkit_python-1.0.2/toolkit_python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:04:32.751095 toolkit_python-1.0.2/toolkit_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-17 13:04:32.000000 toolkit_python-1.0.2/toolkit_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-17 13:04:32.000000 toolkit_python-1.0.2/toolkit_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 13:04:32.000000 toolkit_python-1.0.2/toolkit_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-17 13:04:32.000000 toolkit_python-1.0.2/toolkit_python.egg-info/top_level.txt
```

