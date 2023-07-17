# Comparing `tmp/pdfsBlankDetection-0.1.4.tar.gz` & `tmp/pdfsBlankDetection-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdfsBlankDetection-0.1.4.tar", last modified: Fri Jul 14 02:02:38 2023, max compression
+gzip compressed data, was "pdfsBlankDetection-0.1.5.tar", last modified: Mon Jul 17 06:12:11 2023, max compression
```

## Comparing `pdfsBlankDetection-0.1.4.tar` & `pdfsBlankDetection-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 02:02:38.145462 pdfsBlankDetection-0.1.4/
--rw-rw-rw-   0        0        0       19 2023-07-05 02:27:45.000000 pdfsBlankDetection-0.1.4/LICENSE.txt
--rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 pdfsBlankDetection-0.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0      410 2023-07-14 02:02:38.145462 pdfsBlankDetection-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0       30 2023-07-05 02:45:05.000000 pdfsBlankDetection-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 02:02:38.122460 pdfsBlankDetection-0.1.4/pdfsBlankDetection/
--rw-rw-rw-   0        0        0        0 2023-06-25 05:47:26.000000 pdfsBlankDetection-0.1.4/pdfsBlankDetection/__init__.py
--rw-rw-rw-   0        0        0   110080 2023-07-14 01:34:39.000000 pdfsBlankDetection-0.1.4/pdfsBlankDetection/pdf_blank_detection_f.pyd
--rw-rw-rw-   0        0        0    79360 2023-07-14 01:34:43.000000 pdfsBlankDetection-0.1.4/pdfsBlankDetection/pdf_blank_detection_ui_v2.pyd
--rw-rw-rw-   0        0        0    44032 2023-07-14 01:34:47.000000 pdfsBlankDetection-0.1.4/pdfsBlankDetection/pdf_blank_detection_ui_v2_result_windows2.pyd
--rw-rw-rw-   0        0        0   115200 2023-07-14 01:34:34.000000 pdfsBlankDetection-0.1.4/pdfsBlankDetection/pdfsBlankDetection.pyd
-drwxrwxrwx   0        0        0        0 2023-07-14 02:02:38.141460 pdfsBlankDetection-0.1.4/pdfsBlankDetection.egg-info/
--rw-rw-rw-   0        0        0      410 2023-07-14 02:02:38.000000 pdfsBlankDetection-0.1.4/pdfsBlankDetection.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      452 2023-07-14 02:02:38.000000 pdfsBlankDetection-0.1.4/pdfsBlankDetection.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 02:02:38.000000 pdfsBlankDetection-0.1.4/pdfsBlankDetection.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-14 02:02:38.000000 pdfsBlankDetection-0.1.4/pdfsBlankDetection.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      136 2023-07-14 02:02:38.147462 pdfsBlankDetection-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1028 2023-07-14 02:01:07.000000 pdfsBlankDetection-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:12:11.254835 pdfsBlankDetection-0.1.5/
+-rw-rw-rw-   0        0        0       19 2023-07-05 02:27:45.000000 pdfsBlankDetection-0.1.5/LICENSE.txt
+-rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 pdfsBlankDetection-0.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      410 2023-07-17 06:12:11.254835 pdfsBlankDetection-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2023-07-05 02:45:05.000000 pdfsBlankDetection-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 06:12:11.238610 pdfsBlankDetection-0.1.5/pdfsBlankDetection/
+-rw-rw-rw-   0        0        0        0 2023-06-25 05:47:26.000000 pdfsBlankDetection-0.1.5/pdfsBlankDetection/__init__.py
+-rw-rw-rw-   0        0        0   110080 2023-07-14 01:34:39.000000 pdfsBlankDetection-0.1.5/pdfsBlankDetection/pdf_blank_detection_f.pyd
+-rw-rw-rw-   0        0        0    79360 2023-07-14 01:34:43.000000 pdfsBlankDetection-0.1.5/pdfsBlankDetection/pdf_blank_detection_ui_v2.pyd
+-rw-rw-rw-   0        0        0    44032 2023-07-14 01:34:47.000000 pdfsBlankDetection-0.1.5/pdfsBlankDetection/pdf_blank_detection_ui_v2_result_windows2.pyd
+-rw-rw-rw-   0        0        0   115200 2023-07-17 06:09:05.000000 pdfsBlankDetection-0.1.5/pdfsBlankDetection/pdfsBlankDetection.pyd
+drwxrwxrwx   0        0        0        0 2023-07-17 06:12:11.251836 pdfsBlankDetection-0.1.5/pdfsBlankDetection.egg-info/
+-rw-rw-rw-   0        0        0      410 2023-07-17 06:12:11.000000 pdfsBlankDetection-0.1.5/pdfsBlankDetection.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      452 2023-07-17 06:12:11.000000 pdfsBlankDetection-0.1.5/pdfsBlankDetection.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 06:12:11.000000 pdfsBlankDetection-0.1.5/pdfsBlankDetection.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-17 06:12:11.000000 pdfsBlankDetection-0.1.5/pdfsBlankDetection.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      136 2023-07-17 06:12:11.256836 pdfsBlankDetection-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1028 2023-07-17 06:11:42.000000 pdfsBlankDetection-0.1.5/setup.py
```

### Comparing `pdfsBlankDetection-0.1.4/setup.py` & `pdfsBlankDetection-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 #-*- coding:utf-8 -*-
 import os 
 from setuptools import setup, find_packages
 
 MAJOR = 0
 MINOR = 1
-PATCH = 4
+PATCH = 5
 VERSION = f"{MAJOR}.{MINOR}.{PATCH}"
 
 def get_install_requires():
     reqs = []
     return reqs
 setup(
 	name = "pdfsBlankDetection",
```

