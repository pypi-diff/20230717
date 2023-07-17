# Comparing `tmp/ARIclicker-0.3.6.tar.gz` & `tmp/ARIclicker-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ARIclicker-0.3.6.tar", last modified: Wed Jun 28 11:17:11 2023, max compression
+gzip compressed data, was "ARIclicker-2.0.0.tar", last modified: Mon Jul 17 03:17:48 2023, max compression
```

## Comparing `ARIclicker-0.3.6.tar` & `ARIclicker-2.0.0.tar`

### file list

```diff
@@ -1,14 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-28 11:17:11.766009 ARIclicker-0.3.6/
-drwxrwxrwx   0        0        0        0 2023-06-28 11:17:11.642029 ARIclicker-0.3.6/ARIclicker/
--rw-rw-rw-   0        0        0     4508 2023-06-28 11:13:26.000000 ARIclicker-0.3.6/ARIclicker/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-28 11:17:11.743978 ARIclicker-0.3.6/ARIclicker.egg-info/
--rw-rw-rw-   0        0        0     1891 2023-06-28 11:17:11.000000 ARIclicker-0.3.6/ARIclicker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2023-06-28 11:17:11.000000 ARIclicker-0.3.6/ARIclicker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-28 11:17:11.000000 ARIclicker-0.3.6/ARIclicker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-06-28 11:17:11.000000 ARIclicker-0.3.6/ARIclicker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-28 11:17:11.000000 ARIclicker-0.3.6/ARIclicker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1891 2023-06-28 11:17:11.759017 ARIclicker-0.3.6/PKG-INFO
--rw-rw-rw-   0        0        0     1535 2023-06-24 04:20:24.000000 ARIclicker-0.3.6/README.md
--rw-rw-rw-   0        0        0     1093 2023-06-22 03:55:50.000000 ARIclicker-0.3.6/license.txt
--rw-rw-rw-   0        0        0       42 2023-06-28 11:17:11.766009 ARIclicker-0.3.6/setup.cfg
--rw-rw-rw-   0        0        0      696 2023-06-28 11:16:43.000000 ARIclicker-0.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 03:17:48.475144 ARIclicker-2.0.0/
+drwxrwxrwx   0        0        0        0 2023-07-17 03:17:48.435144 ARIclicker-2.0.0/ARIclicker/
+-rw-rw-rw-   0        0        0     1779 2023-07-16 11:37:39.000000 ARIclicker-2.0.0/ARIclicker/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 03:17:48.465144 ARIclicker-2.0.0/ARIclicker.egg-info/
+-rw-rw-rw-   0        0        0     1021 2023-07-17 03:17:47.000000 ARIclicker-2.0.0/ARIclicker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      177 2023-07-17 03:17:47.000000 ARIclicker-2.0.0/ARIclicker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 03:17:47.000000 ARIclicker-2.0.0/ARIclicker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-07-17 03:17:47.000000 ARIclicker-2.0.0/ARIclicker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1021 2023-07-17 03:17:48.475144 ARIclicker-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2023-07-16 10:49:43.000000 ARIclicker-2.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-17 03:17:48.475144 ARIclicker-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      747 2023-07-17 03:17:17.000000 ARIclicker-2.0.0/setup.py
```

