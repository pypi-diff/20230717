# Comparing `tmp/liveramp_automation_framework-0.1.8.tar.gz` & `tmp/liveramp_automation_framework-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liveramp_automation_framework-0.1.8.tar", last modified: Mon Jul 17 08:47:46 2023, max compression
+gzip compressed data, was "liveramp_automation_framework-0.1.9.tar", last modified: Mon Jul 17 09:41:17 2023, max compression
```

## Comparing `liveramp_automation_framework-0.1.8.tar` & `liveramp_automation_framework-0.1.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-07-17 08:47:46.204884 liveramp_automation_framework-0.1.8/
--rw-r--r--   0 jasqia     (502) staff       (20)     1881 2023-07-17 08:47:46.204169 liveramp_automation_framework-0.1.8/PKG-INFO
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-07-17 08:47:46.195739 liveramp_automation_framework-0.1.8/liveramp_automation/
--rw-r--r--   0 jasqia     (502) staff       (20)     1705 2023-06-19 09:16:48.000000 liveramp_automation_framework-0.1.8/liveramp_automation/helper_bucket.py
--rw-r--r--   0 jasqia     (502) staff       (20)     3126 2023-07-17 06:23:25.000000 liveramp_automation_framework-0.1.8/liveramp_automation/helper_login.py
--rw-r--r--   0 jasqia     (502) staff       (20)       72 2023-07-17 06:20:26.000000 liveramp_automation_framework-0.1.8/liveramp_automation/helper_notification.py
--rw-r--r--   0 jasqia     (502) staff       (20)     2234 2023-07-17 06:23:25.000000 liveramp_automation_framework-0.1.8/liveramp_automation/helper_report.py
--rw-r--r--   0 jasqia     (502) staff       (20)      713 2023-05-03 08:30:53.000000 liveramp_automation_framework-0.1.8/liveramp_automation/parsers.py
--rw-r--r--   0 jasqia     (502) staff       (20)      670 2023-07-17 02:34:55.000000 liveramp_automation_framework-0.1.8/liveramp_automation/util_allure.py
--rw-r--r--   0 jasqia     (502) staff       (20)     1724 2023-07-17 08:47:40.000000 liveramp_automation_framework-0.1.8/liveramp_automation/util_log.py
--rw-r--r--   0 jasqia     (502) staff       (20)      742 2023-07-17 06:23:25.000000 liveramp_automation_framework-0.1.8/liveramp_automation/util_playwright.py
--rw-r--r--   0 jasqia     (502) staff       (20)     6968 2023-07-17 06:23:25.000000 liveramp_automation_framework-0.1.8/liveramp_automation/util_request.py
--rw-r--r--   0 jasqia     (502) staff       (20)      743 2023-07-17 06:23:25.000000 liveramp_automation_framework-0.1.8/liveramp_automation/util_selenium.py
--rw-r--r--   0 jasqia     (502) staff       (20)      779 2023-07-17 02:34:55.000000 liveramp_automation_framework-0.1.8/liveramp_automation/util_time.py
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-07-17 08:47:46.202793 liveramp_automation_framework-0.1.8/liveramp_automation_framework.egg-info/
--rw-r--r--   0 jasqia     (502) staff       (20)     1881 2023-07-17 08:47:46.000000 liveramp_automation_framework-0.1.8/liveramp_automation_framework.egg-info/PKG-INFO
--rw-r--r--   0 jasqia     (502) staff       (20)      668 2023-07-17 08:47:46.000000 liveramp_automation_framework-0.1.8/liveramp_automation_framework.egg-info/SOURCES.txt
--rw-r--r--   0 jasqia     (502) staff       (20)        1 2023-07-17 08:47:46.000000 liveramp_automation_framework-0.1.8/liveramp_automation_framework.egg-info/dependency_links.txt
--rw-r--r--   0 jasqia     (502) staff       (20)      381 2023-07-17 08:47:46.000000 liveramp_automation_framework-0.1.8/liveramp_automation_framework.egg-info/requires.txt
--rw-r--r--   0 jasqia     (502) staff       (20)       20 2023-07-17 08:47:46.000000 liveramp_automation_framework-0.1.8/liveramp_automation_framework.egg-info/top_level.txt
--rw-r--r--   0 jasqia     (502) staff       (20)       38 2023-07-17 08:47:46.205089 liveramp_automation_framework-0.1.8/setup.cfg
--rw-r--r--   0 jasqia     (502) staff       (20)     1169 2023-07-17 08:47:40.000000 liveramp_automation_framework-0.1.8/setup.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-07-17 09:41:17.097468 liveramp_automation_framework-0.1.9/
+-rw-r--r--   0 jasqia     (502) staff       (20)     1881 2023-07-17 09:41:17.097002 liveramp_automation_framework-0.1.9/PKG-INFO
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-07-17 09:41:17.091094 liveramp_automation_framework-0.1.9/liveramp_automation/
+-rw-r--r--   0 jasqia     (502) staff       (20)     1705 2023-06-19 09:16:48.000000 liveramp_automation_framework-0.1.9/liveramp_automation/helper_bucket.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     2238 2023-07-17 09:37:25.000000 liveramp_automation_framework-0.1.9/liveramp_automation/helper_file.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     3116 2023-07-17 09:39:28.000000 liveramp_automation_framework-0.1.9/liveramp_automation/helper_login.py
+-rw-r--r--   0 jasqia     (502) staff       (20)       72 2023-07-17 06:20:26.000000 liveramp_automation_framework-0.1.9/liveramp_automation/helper_notification.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      713 2023-05-03 08:30:53.000000 liveramp_automation_framework-0.1.9/liveramp_automation/parsers.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      670 2023-07-17 02:34:55.000000 liveramp_automation_framework-0.1.9/liveramp_automation/util_allure.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     1724 2023-07-17 08:47:40.000000 liveramp_automation_framework-0.1.9/liveramp_automation/util_log.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      742 2023-07-17 06:23:25.000000 liveramp_automation_framework-0.1.9/liveramp_automation/util_playwright.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     6968 2023-07-17 06:23:25.000000 liveramp_automation_framework-0.1.9/liveramp_automation/util_request.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      743 2023-07-17 06:23:25.000000 liveramp_automation_framework-0.1.9/liveramp_automation/util_selenium.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      779 2023-07-17 02:34:55.000000 liveramp_automation_framework-0.1.9/liveramp_automation/util_time.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-07-17 09:41:17.096069 liveramp_automation_framework-0.1.9/liveramp_automation_framework.egg-info/
+-rw-r--r--   0 jasqia     (502) staff       (20)     1881 2023-07-17 09:41:16.000000 liveramp_automation_framework-0.1.9/liveramp_automation_framework.egg-info/PKG-INFO
+-rw-r--r--   0 jasqia     (502) staff       (20)      666 2023-07-17 09:41:16.000000 liveramp_automation_framework-0.1.9/liveramp_automation_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)        1 2023-07-17 09:41:16.000000 liveramp_automation_framework-0.1.9/liveramp_automation_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)      381 2023-07-17 09:41:16.000000 liveramp_automation_framework-0.1.9/liveramp_automation_framework.egg-info/requires.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)       20 2023-07-17 09:41:16.000000 liveramp_automation_framework-0.1.9/liveramp_automation_framework.egg-info/top_level.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)       38 2023-07-17 09:41:17.097637 liveramp_automation_framework-0.1.9/setup.cfg
+-rw-r--r--   0 jasqia     (502) staff       (20)     1169 2023-07-17 09:40:28.000000 liveramp_automation_framework-0.1.9/setup.py
```

### Comparing `liveramp_automation_framework-0.1.8/PKG-INFO` & `liveramp_automation_framework-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liveramp_automation_framework
-Version: 0.1.8
+Version: 0.1.9
 Summary: This is the base liveramp_automation_framework
 Home-page: https://github.com/LiveRamp/qe_api_framework
 Author: Jasmine Qian
 Author-email: jasmine.qian@liveramp.com
 Description-Content-Type: text/markdown
 
 ### 1. Descprition of the repository
```

### Comparing `liveramp_automation_framework-0.1.8/liveramp_automation/helper_bucket.py` & `liveramp_automation_framework-0.1.9/liveramp_automation/helper_bucket.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.1.8/liveramp_automation/helper_login.py` & `liveramp_automation_framework-0.1.9/liveramp_automation/helper_login.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import requests
 from selenium.webdriver import Keys
 from selenium.webdriver.common.by import By
-from liveramp_automation.util_log import Logger as Logger
+from liveramp_automation.util_log import Logger
 from liveramp_automation.util_time import fixed_wait
 
 
 class LoginHepler:
 
     @staticmethod
     def liveramp_okta_login_page(page, config, USERNAME, PASSWORD):
```

### Comparing `liveramp_automation_framework-0.1.8/liveramp_automation/helper_report.py` & `liveramp_automation_framework-0.1.9/liveramp_automation/helper_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import yaml
 from liveramp_automation.util_log import Logger
 
 
-class Report:
+class FileHelper:
 
     @staticmethod
     def read_json_report(path) -> dict:
         with open(path, 'r') as file:
             # Read all the content of the file
             json_string = file.read()
             data = json.loads(json_string)
```

### Comparing `liveramp_automation_framework-0.1.8/liveramp_automation/parsers.py` & `liveramp_automation_framework-0.1.9/liveramp_automation/parsers.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.1.8/liveramp_automation/util_allure.py` & `liveramp_automation_framework-0.1.9/liveramp_automation/util_allure.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.1.8/liveramp_automation/util_log.py` & `liveramp_automation_framework-0.1.9/liveramp_automation/util_log.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.1.8/liveramp_automation/util_playwright.py` & `liveramp_automation_framework-0.1.9/liveramp_automation/util_playwright.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.1.8/liveramp_automation/util_request.py` & `liveramp_automation_framework-0.1.9/liveramp_automation/util_request.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.1.8/liveramp_automation/util_selenium.py` & `liveramp_automation_framework-0.1.9/liveramp_automation/util_selenium.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.1.8/liveramp_automation/util_time.py` & `liveramp_automation_framework-0.1.9/liveramp_automation/util_time.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.1.8/liveramp_automation_framework.egg-info/PKG-INFO` & `liveramp_automation_framework-0.1.9/liveramp_automation_framework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liveramp-automation-framework
-Version: 0.1.8
+Version: 0.1.9
 Summary: This is the base liveramp_automation_framework
 Home-page: https://github.com/LiveRamp/qe_api_framework
 Author: Jasmine Qian
 Author-email: jasmine.qian@liveramp.com
 Description-Content-Type: text/markdown
 
 ### 1. Descprition of the repository
```

### Comparing `liveramp_automation_framework-0.1.8/liveramp_automation_framework.egg-info/SOURCES.txt` & `liveramp_automation_framework-0.1.9/liveramp_automation_framework.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 setup.py
 liveramp_automation/helper_bucket.py
+liveramp_automation/helper_file.py
 liveramp_automation/helper_login.py
 liveramp_automation/helper_notification.py
-liveramp_automation/helper_report.py
 liveramp_automation/parsers.py
 liveramp_automation/util_allure.py
 liveramp_automation/util_log.py
 liveramp_automation/util_playwright.py
 liveramp_automation/util_request.py
 liveramp_automation/util_selenium.py
 liveramp_automation/util_time.py
```

### Comparing `liveramp_automation_framework-0.1.8/setup.py` & `liveramp_automation_framework-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("readme.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='liveramp_automation_framework',
-    version='0.1.8',
+    version='0.1.9',
     author='Jasmine Qian',
     author_email='jasmine.qian@liveramp.com',
     description="This is the base liveramp_automation_framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/LiveRamp/qe_api_framework",
     packages=['liveramp_automation'],
```

