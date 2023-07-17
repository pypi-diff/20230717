# Comparing `tmp/medcase-0.1.0.tar.gz` & `tmp/medcase-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/medcase-0.1.0.tar", last modified: Mon Jul 17 06:08:32 2023, max compression
+gzip compressed data, was "dist/medcase-0.1.1.tar", last modified: Mon Jul 17 06:26:08 2023, max compression
```

## Comparing `medcase-0.1.0.tar` & `medcase-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 leixuechun   (501) staff       (20)        0 2023-07-17 06:08:32.843349 medcase-0.1.0/
--rw-r--r--   0 leixuechun   (501) staff       (20)       51 2023-07-17 06:08:32.843012 medcase-0.1.0/PKG-INFO
-drwxr-xr-x   0 leixuechun   (501) staff       (20)        0 2023-07-17 06:08:32.839859 medcase-0.1.0/common/
--rw-r--r--   0 leixuechun   (501) staff       (20)       95 2023-06-26 11:24:58.000000 medcase-0.1.0/common/__init__.py
--rw-r--r--   0 leixuechun   (501) staff       (20)    20398 2023-07-17 02:51:09.000000 medcase-0.1.0/common/autogui.py
--rw-r--r--   0 leixuechun   (501) staff       (20)      930 2023-07-16 13:34:45.000000 medcase-0.1.0/common/case_data_process.py
--rw-r--r--   0 leixuechun   (501) staff       (20)    10769 2023-07-03 03:06:40.000000 medcase-0.1.0/common/generate_test_code.py
--rw-r--r--   0 leixuechun   (501) staff       (20)     6557 2023-07-04 07:07:29.000000 medcase-0.1.0/common/guitools.py
-drwxr-xr-x   0 leixuechun   (501) staff       (20)        0 2023-07-17 06:08:32.841681 medcase-0.1.0/medcase.egg-info/
--rw-r--r--   0 leixuechun   (501) staff       (20)       51 2023-07-17 06:08:32.000000 medcase-0.1.0/medcase.egg-info/PKG-INFO
--rw-r--r--   0 leixuechun   (501) staff       (20)      356 2023-07-17 06:08:32.000000 medcase-0.1.0/medcase.egg-info/SOURCES.txt
--rw-r--r--   0 leixuechun   (501) staff       (20)        1 2023-07-17 06:08:32.000000 medcase-0.1.0/medcase.egg-info/dependency_links.txt
--rw-r--r--   0 leixuechun   (501) staff       (20)       46 2023-07-17 06:08:32.000000 medcase-0.1.0/medcase.egg-info/entry_points.txt
--rw-r--r--   0 leixuechun   (501) staff       (20)       84 2023-07-17 06:08:32.000000 medcase-0.1.0/medcase.egg-info/requires.txt
--rw-r--r--   0 leixuechun   (501) staff       (20)       16 2023-07-17 06:08:32.000000 medcase-0.1.0/medcase.egg-info/top_level.txt
--rw-r--r--   0 leixuechun   (501) staff       (20)       38 2023-07-17 06:08:32.843437 medcase-0.1.0/setup.cfg
--rw-r--r--   0 leixuechun   (501) staff       (20)      637 2023-07-17 06:08:18.000000 medcase-0.1.0/setup.py
-drwxr-xr-x   0 leixuechun   (501) staff       (20)        0 2023-07-17 06:08:32.842525 medcase-0.1.0/testdata/
--rw-r--r--   0 leixuechun   (501) staff       (20)       95 2023-06-26 12:28:31.000000 medcase-0.1.0/testdata/__init__.py
--rw-r--r--   0 leixuechun   (501) staff       (20)      923 2023-06-26 12:39:18.000000 medcase-0.1.0/testdata/case_template.py
+drwxr-xr-x   0 leixuechun   (501) staff       (20)        0 2023-07-17 06:26:08.287394 medcase-0.1.1/
+-rw-r--r--   0 leixuechun   (501) staff       (20)       51 2023-07-17 06:26:08.286828 medcase-0.1.1/PKG-INFO
+drwxr-xr-x   0 leixuechun   (501) staff       (20)        0 2023-07-17 06:26:08.270760 medcase-0.1.1/common/
+-rw-r--r--   0 leixuechun   (501) staff       (20)       95 2023-06-26 11:24:58.000000 medcase-0.1.1/common/__init__.py
+-rw-r--r--   0 leixuechun   (501) staff       (20)    20398 2023-07-17 02:51:09.000000 medcase-0.1.1/common/autogui.py
+-rw-r--r--   0 leixuechun   (501) staff       (20)      930 2023-07-16 13:34:45.000000 medcase-0.1.1/common/case_data_process.py
+-rw-r--r--   0 leixuechun   (501) staff       (20)    10769 2023-07-03 03:06:40.000000 medcase-0.1.1/common/generate_test_code.py
+-rw-r--r--   0 leixuechun   (501) staff       (20)     6557 2023-07-04 07:07:29.000000 medcase-0.1.1/common/guitools.py
+drwxr-xr-x   0 leixuechun   (501) staff       (20)        0 2023-07-17 06:26:08.272735 medcase-0.1.1/medcase.egg-info/
+-rw-r--r--   0 leixuechun   (501) staff       (20)       51 2023-07-17 06:26:08.000000 medcase-0.1.1/medcase.egg-info/PKG-INFO
+-rw-r--r--   0 leixuechun   (501) staff       (20)      356 2023-07-17 06:26:08.000000 medcase-0.1.1/medcase.egg-info/SOURCES.txt
+-rw-r--r--   0 leixuechun   (501) staff       (20)        1 2023-07-17 06:26:08.000000 medcase-0.1.1/medcase.egg-info/dependency_links.txt
+-rw-r--r--   0 leixuechun   (501) staff       (20)       46 2023-07-17 06:26:08.000000 medcase-0.1.1/medcase.egg-info/entry_points.txt
+-rw-r--r--   0 leixuechun   (501) staff       (20)       49 2023-07-17 06:26:08.000000 medcase-0.1.1/medcase.egg-info/requires.txt
+-rw-r--r--   0 leixuechun   (501) staff       (20)       16 2023-07-17 06:26:08.000000 medcase-0.1.1/medcase.egg-info/top_level.txt
+-rw-r--r--   0 leixuechun   (501) staff       (20)       38 2023-07-17 06:26:08.287557 medcase-0.1.1/setup.cfg
+-rw-r--r--   0 leixuechun   (501) staff       (20)      525 2023-07-17 06:22:20.000000 medcase-0.1.1/setup.py
+drwxr-xr-x   0 leixuechun   (501) staff       (20)        0 2023-07-17 06:26:08.273586 medcase-0.1.1/testdata/
+-rw-r--r--   0 leixuechun   (501) staff       (20)       95 2023-06-26 12:28:31.000000 medcase-0.1.1/testdata/__init__.py
+-rw-r--r--   0 leixuechun   (501) staff       (20)      923 2023-06-26 12:39:18.000000 medcase-0.1.1/testdata/case_template.py
```

### Comparing `medcase-0.1.0/common/autogui.py` & `medcase-0.1.1/common/autogui.py`

 * *Files identical despite different names*

### Comparing `medcase-0.1.0/common/case_data_process.py` & `medcase-0.1.1/common/case_data_process.py`

 * *Files identical despite different names*

### Comparing `medcase-0.1.0/common/generate_test_code.py` & `medcase-0.1.1/common/generate_test_code.py`

 * *Files identical despite different names*

### Comparing `medcase-0.1.0/common/guitools.py` & `medcase-0.1.1/common/guitools.py`

 * *Files identical despite different names*

### Comparing `medcase-0.1.0/setup.py` & `medcase-0.1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,30 +2,23 @@
 # @Author  : jackxclei
 # @Time    : 2023/7/17 11:39 上午
 # @Function:
 from setuptools import setup, find_packages
 
 setup(
     name="medcase",
-    version="0.1.0",
+    version="0.1.1",
     packages=find_packages(),
     install_requires=[
         # 添加项目依赖
         # "tkcalendar",
-        "os",
-        "json",
-        "random",
-        "re",
         "datetime",
         "tkinter",
-        "urllib",
         "requests",
-        "time",
         "hashlib",
-        "json",
         "ast",
         "tkcalendar",
     ],
     entry_points={
         "console_scripts": [
             "medcase=medcase.main:main",
         ],
```

### Comparing `medcase-0.1.0/testdata/case_template.py` & `medcase-0.1.1/testdata/case_template.py`

 * *Files identical despite different names*

