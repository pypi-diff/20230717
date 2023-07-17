# Comparing `tmp/lyhapi-0.0.5.tar.gz` & `tmp/lyhapi-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lyhapi-0.0.5.tar", last modified: Tue Mar  9 08:50:11 2021, max compression
+gzip compressed data, was "dist/lyhapi-0.0.6.tar", last modified: Fri Mar 19 08:06:14 2021, max compression
```

## Comparing `lyhapi-0.0.5.tar` & `lyhapi-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,17 @@
-drwxr-xr-x   0 vissy      (502) staff       (20)        0 2021-03-09 08:50:11.000000 lyhapi-0.0.5/
--rw-r--r--   0 vissy      (502) staff       (20)      237 2021-03-09 08:50:11.000000 lyhapi-0.0.5/PKG-INFO
--rw-r--r--   0 vissy      (502) staff       (20)       17 2021-03-09 07:27:39.000000 lyhapi-0.0.5/README.md
-drwxr-xr-x   0 vissy      (502) staff       (20)        0 2021-03-09 08:50:11.000000 lyhapi-0.0.5/commonlib/
--rw-r--r--   0 vissy      (502) staff       (20)       44 2021-03-09 08:04:06.000000 lyhapi-0.0.5/commonlib/__init__.py
--rw-r--r--   0 vissy      (502) staff       (20)     2276 2021-03-09 07:59:36.000000 lyhapi-0.0.5/commonlib/confighttp.py
--rw-r--r--   0 vissy      (502) staff       (20)      476 2021-03-09 08:00:59.000000 lyhapi-0.0.5/commonlib/connectdb.py
--rw-r--r--   0 vissy      (502) staff       (20)      452 2021-03-09 07:27:39.000000 lyhapi-0.0.5/commonlib/htmlresult.py
--rw-r--r--   0 vissy      (502) staff       (20)     1749 2021-03-09 08:00:14.000000 lyhapi-0.0.5/commonlib/sendemail.py
-drwxr-xr-x   0 vissy      (502) staff       (20)        0 2021-03-09 08:50:11.000000 lyhapi-0.0.5/lyhapi.egg-info/
--rw-r--r--   0 vissy      (502) staff       (20)      237 2021-03-09 08:50:11.000000 lyhapi-0.0.5/lyhapi.egg-info/PKG-INFO
--rw-r--r--   0 vissy      (502) staff       (20)      354 2021-03-09 08:50:11.000000 lyhapi-0.0.5/lyhapi.egg-info/SOURCES.txt
--rw-r--r--   0 vissy      (502) staff       (20)        1 2021-03-09 08:50:11.000000 lyhapi-0.0.5/lyhapi.egg-info/dependency_links.txt
--rw-r--r--   0 vissy      (502) staff       (20)        1 2021-03-09 08:39:13.000000 lyhapi-0.0.5/lyhapi.egg-info/not-zip-safe
--rw-r--r--   0 vissy      (502) staff       (20)       19 2021-03-09 08:50:11.000000 lyhapi-0.0.5/lyhapi.egg-info/top_level.txt
--rw-r--r--   0 vissy      (502) staff       (20)       38 2021-03-09 08:50:11.000000 lyhapi-0.0.5/setup.cfg
--rw-r--r--   0 vissy      (502) staff       (20)      391 2021-03-09 08:49:12.000000 lyhapi-0.0.5/setup.py
-drwxr-xr-x   0 vissy      (502) staff       (20)        0 2021-03-09 08:50:11.000000 lyhapi-0.0.5/testdata/
--rw-r--r--   0 vissy      (502) staff       (20)        0 2021-03-09 07:56:04.000000 lyhapi-0.0.5/testdata/__init__.py
--rw-r--r--   0 vissy      (502) staff       (20)       44 2021-03-09 08:01:10.000000 lyhapi-0.0.5/testdata/db.py
--rw-r--r--   0 vissy      (502) staff       (20)       44 2021-03-09 08:01:27.000000 lyhapi-0.0.5/testdata/email.py
--rw-r--r--   0 vissy      (502) staff       (20)       44 2021-03-09 08:01:27.000000 lyhapi-0.0.5/testdata/http.py
+drwxr-xr-x   0 vissy      (502) staff       (20)        0 2021-03-19 08:06:14.000000 lyhapi-0.0.6/
+-rw-r--r--   0 vissy      (502) staff       (20)      237 2021-03-19 08:06:14.000000 lyhapi-0.0.6/PKG-INFO
+-rw-r--r--   0 vissy      (502) staff       (20)       17 2021-03-09 07:27:39.000000 lyhapi-0.0.6/README.md
+drwxr-xr-x   0 vissy      (502) staff       (20)        0 2021-03-19 08:06:14.000000 lyhapi-0.0.6/commonlib/
+-rw-r--r--   0 vissy      (502) staff       (20)       44 2021-03-19 07:03:23.000000 lyhapi-0.0.6/commonlib/__init__.py
+-rw-r--r--   0 vissy      (502) staff       (20)     2228 2021-03-19 07:55:55.000000 lyhapi-0.0.6/commonlib/confighttp.py
+-rw-r--r--   0 vissy      (502) staff       (20)      382 2021-03-19 08:04:11.000000 lyhapi-0.0.6/commonlib/connectdb.py
+-rw-r--r--   0 vissy      (502) staff       (20)      452 2021-03-19 07:03:23.000000 lyhapi-0.0.6/commonlib/htmlresult.py
+-rw-r--r--   0 vissy      (502) staff       (20)     1681 2021-03-19 07:55:41.000000 lyhapi-0.0.6/commonlib/sendemail.py
+drwxr-xr-x   0 vissy      (502) staff       (20)        0 2021-03-19 08:06:14.000000 lyhapi-0.0.6/lyhapi.egg-info/
+-rw-r--r--   0 vissy      (502) staff       (20)      237 2021-03-19 08:06:14.000000 lyhapi-0.0.6/lyhapi.egg-info/PKG-INFO
+-rw-r--r--   0 vissy      (502) staff       (20)      283 2021-03-19 08:06:14.000000 lyhapi-0.0.6/lyhapi.egg-info/SOURCES.txt
+-rw-r--r--   0 vissy      (502) staff       (20)        1 2021-03-19 08:06:14.000000 lyhapi-0.0.6/lyhapi.egg-info/dependency_links.txt
+-rw-r--r--   0 vissy      (502) staff       (20)        1 2021-03-19 08:05:42.000000 lyhapi-0.0.6/lyhapi.egg-info/not-zip-safe
+-rw-r--r--   0 vissy      (502) staff       (20)       10 2021-03-19 08:06:14.000000 lyhapi-0.0.6/lyhapi.egg-info/top_level.txt
+-rw-r--r--   0 vissy      (502) staff       (20)       38 2021-03-19 08:06:14.000000 lyhapi-0.0.6/setup.cfg
+-rw-r--r--   0 vissy      (502) staff       (20)      391 2021-03-19 08:05:55.000000 lyhapi-0.0.6/setup.py
```

