# Comparing `tmp/ytcomments-0.1.tar.gz` & `tmp/ytcomments-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ytcomments-0.1.tar", last modified: Mon Jul 17 00:30:29 2023, max compression
+gzip compressed data, was "ytcomments-0.2.tar", last modified: Mon Jul 17 01:17:21 2023, max compression
```

## Comparing `ytcomments-0.1.tar` & `ytcomments-0.2.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-17 00:30:29.166483 ytcomments-0.1/
--rw-rw-r--   0 dipson    (1000) dipson    (1000)      151 2023-07-17 00:30:29.166483 ytcomments-0.1/PKG-INFO
--rw-rw-r--   0 dipson    (1000) dipson    (1000)        0 2023-07-17 00:27:40.000000 ytcomments-0.1/README.md
--rw-rw-r--   0 dipson    (1000) dipson    (1000)       38 2023-07-17 00:30:29.166483 ytcomments-0.1/setup.cfg
--rw-rw-r--   0 dipson    (1000) dipson    (1000)     1126 2023-07-17 00:26:25.000000 ytcomments-0.1/setup.py
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-17 00:30:29.162483 ytcomments-0.1/src/
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-17 00:30:29.166483 ytcomments-0.1/src/ytcomments/
--rw-rw-r--   0 dipson    (1000) dipson    (1000)        0 2023-07-17 00:27:17.000000 ytcomments-0.1/src/ytcomments/__init__.py
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-17 00:30:29.166483 ytcomments-0.1/src/ytcomments.egg-info/
--rw-rw-r--   0 dipson    (1000) dipson    (1000)      151 2023-07-17 00:30:29.000000 ytcomments-0.1/src/ytcomments.egg-info/PKG-INFO
--rw-rw-r--   0 dipson    (1000) dipson    (1000)      238 2023-07-17 00:30:29.000000 ytcomments-0.1/src/ytcomments.egg-info/SOURCES.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)        1 2023-07-17 00:30:29.000000 ytcomments-0.1/src/ytcomments.egg-info/dependency_links.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)       47 2023-07-17 00:30:29.000000 ytcomments-0.1/src/ytcomments.egg-info/entry_points.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)       11 2023-07-17 00:30:29.000000 ytcomments-0.1/src/ytcomments.egg-info/top_level.txt
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-17 01:17:21.951787 ytcomments-0.2/
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)    35149 2023-07-17 00:55:42.000000 ytcomments-0.2/LICENSE
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)      544 2023-07-17 01:17:21.951787 ytcomments-0.2/PKG-INFO
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)       12 2023-07-17 00:55:06.000000 ytcomments-0.2/README.md
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)       38 2023-07-17 01:17:21.951787 ytcomments-0.2/setup.cfg
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)      909 2023-07-17 01:16:47.000000 ytcomments-0.2/setup.py
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-17 01:17:21.947787 ytcomments-0.2/src/
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-17 01:17:21.947787 ytcomments-0.2/src/ytcomments/
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)     3885 2023-07-17 00:54:40.000000 ytcomments-0.2/src/ytcomments/__init__.py
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-17 01:17:21.951787 ytcomments-0.2/src/ytcomments.egg-info/
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)      544 2023-07-17 01:17:21.000000 ytcomments-0.2/src/ytcomments.egg-info/PKG-INFO
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)      283 2023-07-17 01:17:21.000000 ytcomments-0.2/src/ytcomments.egg-info/SOURCES.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)        1 2023-07-17 01:17:21.000000 ytcomments-0.2/src/ytcomments.egg-info/dependency_links.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)       43 2023-07-17 01:17:21.000000 ytcomments-0.2/src/ytcomments.egg-info/entry_points.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)       95 2023-07-17 01:17:21.000000 ytcomments-0.2/src/ytcomments.egg-info/requires.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)       11 2023-07-17 01:17:21.000000 ytcomments-0.2/src/ytcomments.egg-info/top_level.txt
```

