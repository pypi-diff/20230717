# Comparing `tmp/lqq_tool_weekreport-1.0.0.tar.gz` & `tmp/lqq_tool_weekreport-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lqq_tool_weekreport-1.0.0.tar", last modified: Wed Jul 12 07:48:49 2023, max compression
+gzip compressed data, was "lqq_tool_weekreport-1.0.1.tar", last modified: Mon Jul 17 09:21:47 2023, max compression
```

## Comparing `lqq_tool_weekreport-1.0.0.tar` & `lqq_tool_weekreport-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 07:48:49.950132 lqq_tool_weekreport-1.0.0/
--rw-rw-rw-   0        0        0      205 2023-07-12 07:48:49.948800 lqq_tool_weekreport-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-12 07:48:49.931313 lqq_tool_weekreport-1.0.0/com/
-drwxrwxrwx   0        0        0        0 2023-07-12 07:48:49.932347 lqq_tool_weekreport-1.0.0/com/lqq/
-drwxrwxrwx   0        0        0        0 2023-07-12 07:48:49.933392 lqq_tool_weekreport-1.0.0/com/lqq/tool/
-drwxrwxrwx   0        0        0        0 2023-07-12 07:48:49.937972 lqq_tool_weekreport-1.0.0/com/lqq/tool/report/
--rw-rw-rw-   0        0        0        0 2023-07-12 06:29:17.000000 lqq_tool_weekreport-1.0.0/com/lqq/tool/report/__init__.py
--rw-rw-rw-   0        0        0     8728 2023-07-07 08:15:38.000000 lqq_tool_weekreport-1.0.0/com/lqq/tool/report/tool_build_report.py
-drwxrwxrwx   0        0        0        0 2023-07-12 07:48:49.947404 lqq_tool_weekreport-1.0.0/lqq_tool_weekreport.egg-info/
--rw-rw-rw-   0        0        0      205 2023-07-12 07:48:49.000000 lqq_tool_weekreport-1.0.0/lqq_tool_weekreport.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      295 2023-07-12 07:48:49.000000 lqq_tool_weekreport-1.0.0/lqq_tool_weekreport.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 07:48:49.000000 lqq_tool_weekreport-1.0.0/lqq_tool_weekreport.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-07-12 07:48:49.000000 lqq_tool_weekreport-1.0.0/lqq_tool_weekreport.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-12 07:48:49.000000 lqq_tool_weekreport-1.0.0/lqq_tool_weekreport.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 07:48:49.950132 lqq_tool_weekreport-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      384 2023-07-12 07:48:17.000000 lqq_tool_weekreport-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:21:47.342900 lqq_tool_weekreport-1.0.1/
+-rw-rw-rw-   0        0        0      205 2023-07-17 09:21:47.341891 lqq_tool_weekreport-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-17 09:21:47.325291 lqq_tool_weekreport-1.0.1/com/
+drwxrwxrwx   0        0        0        0 2023-07-17 09:21:47.326288 lqq_tool_weekreport-1.0.1/com/lqq/
+drwxrwxrwx   0        0        0        0 2023-07-17 09:21:47.326288 lqq_tool_weekreport-1.0.1/com/lqq/tool/
+drwxrwxrwx   0        0        0        0 2023-07-17 09:21:47.331271 lqq_tool_weekreport-1.0.1/com/lqq/tool/report/
+-rw-rw-rw-   0        0        0        0 2023-07-17 09:16:53.000000 lqq_tool_weekreport-1.0.1/com/lqq/tool/report/__init__.py
+-rw-rw-rw-   0        0        0     8728 2023-07-17 09:16:53.000000 lqq_tool_weekreport-1.0.1/com/lqq/tool/report/tool_build_report.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:21:47.340014 lqq_tool_weekreport-1.0.1/lqq_tool_weekreport.egg-info/
+-rw-rw-rw-   0        0        0      205 2023-07-17 09:21:47.000000 lqq_tool_weekreport-1.0.1/lqq_tool_weekreport.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      295 2023-07-17 09:21:47.000000 lqq_tool_weekreport-1.0.1/lqq_tool_weekreport.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 09:21:47.000000 lqq_tool_weekreport-1.0.1/lqq_tool_weekreport.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-07-17 09:21:47.000000 lqq_tool_weekreport-1.0.1/lqq_tool_weekreport.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-17 09:21:47.000000 lqq_tool_weekreport-1.0.1/lqq_tool_weekreport.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 09:21:47.342900 lqq_tool_weekreport-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      384 2023-07-17 09:21:03.000000 lqq_tool_weekreport-1.0.1/setup.py
```

### Comparing `lqq_tool_weekreport-1.0.0/com/lqq/tool/report/tool_build_report.py` & `lqq_tool_weekreport-1.0.1/com/lqq/tool/report/tool_build_report.py`

 * *Files identical despite different names*

