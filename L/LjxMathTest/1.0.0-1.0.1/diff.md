# Comparing `tmp/LjxMathTest-1.0.0.tar.gz` & `tmp/LjxMathTest-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\LjxMathTest-1.0.0.tar", last modified: Mon Jul 17 08:51:32 2023, max compression
+gzip compressed data, was "dist\LjxMathTest-1.0.1.tar", last modified: Mon Jul 17 09:24:10 2023, max compression
```

## Comparing `LjxMathTest-1.0.0.tar` & `LjxMathTest-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 08:51:32.000000 LjxMathTest-1.0.0/
-drwxrwxrwx   0        0        0        0 2023-07-17 08:51:32.000000 LjxMathTest-1.0.0/LjxMathTest.egg-info/
--rw-rw-rw-   0        0        0      197 2023-07-17 08:51:32.000000 LjxMathTest-1.0.0/LjxMathTest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-07-17 08:51:32.000000 LjxMathTest-1.0.0/LjxMathTest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 08:51:32.000000 LjxMathTest-1.0.0/LjxMathTest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-07-17 08:51:32.000000 LjxMathTest-1.0.0/LjxMathTest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      197 2023-07-17 08:51:32.000000 LjxMathTest-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-17 08:51:32.000000 LjxMathTest-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      241 2023-07-17 08:50:28.000000 LjxMathTest-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 08:51:32.000000 LjxMathTest-1.0.0/src/
--rw-rw-rw-   0        0        0      101 2023-07-17 08:17:23.000000 LjxMathTest-1.0.0/src/__init__.py
--rw-rw-rw-   0        0        0      135 2023-07-17 08:17:32.000000 LjxMathTest-1.0.0/src/addition.py
--rw-rw-rw-   0        0        0      221 2023-07-17 08:18:08.000000 LjxMathTest-1.0.0/src/division.py
--rw-rw-rw-   0        0        0      140 2023-07-17 08:17:54.000000 LjxMathTest-1.0.0/src/multiplication.py
--rw-rw-rw-   0        0        0      140 2023-07-17 08:17:43.000000 LjxMathTest-1.0.0/src/subtraction.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:24:10.000000 LjxMathTest-1.0.1/
+drwxrwxrwx   0        0        0        0 2023-07-17 09:24:10.000000 LjxMathTest-1.0.1/LjxMathTest/
+-rw-rw-rw-   0        0        0      101 2023-07-17 08:17:23.000000 LjxMathTest-1.0.1/LjxMathTest/__init__.py
+-rw-rw-rw-   0        0        0      135 2023-07-17 08:17:32.000000 LjxMathTest-1.0.1/LjxMathTest/addition.py
+-rw-rw-rw-   0        0        0      221 2023-07-17 08:18:08.000000 LjxMathTest-1.0.1/LjxMathTest/division.py
+-rw-rw-rw-   0        0        0      140 2023-07-17 08:17:54.000000 LjxMathTest-1.0.1/LjxMathTest/multiplication.py
+-rw-rw-rw-   0        0        0      140 2023-07-17 08:17:43.000000 LjxMathTest-1.0.1/LjxMathTest/subtraction.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:24:10.000000 LjxMathTest-1.0.1/LjxMathTest.egg-info/
+-rw-rw-rw-   0        0        0      197 2023-07-17 09:24:10.000000 LjxMathTest-1.0.1/LjxMathTest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2023-07-17 09:24:10.000000 LjxMathTest-1.0.1/LjxMathTest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 09:24:10.000000 LjxMathTest-1.0.1/LjxMathTest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-17 09:24:10.000000 LjxMathTest-1.0.1/LjxMathTest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      197 2023-07-17 09:24:10.000000 LjxMathTest-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-17 09:24:10.000000 LjxMathTest-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      241 2023-07-17 09:23:58.000000 LjxMathTest-1.0.1/setup.py
```

