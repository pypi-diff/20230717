# Comparing `tmp/liveramp_automation_framework-0.1.9.tar.gz` & `tmp/liveramp_automation_framework-0.1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liveramp_automation_framework-0.1.9.tar", last modified: Mon Jul 17 09:41:17 2023, max compression
+gzip compressed data, was "liveramp_automation_framework-0.1.9.1.tar", last modified: Mon Jul 17 10:04:42 2023, max compression
```

## Comparing `liveramp_automation_framework-0.1.9.tar` & `liveramp_automation_framework-0.1.9.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-07-17 09:41:17.097468 liveramp_automation_framework-0.1.9/
--rw-r--r--   0 jasqia     (502) staff       (20)     1881 2023-07-17 09:41:17.097002 liveramp_automation_framework-0.1.9/PKG-INFO
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-07-17 09:41:17.091094 liveramp_automation_framework-0.1.9/liveramp_automation/
--rw-r--r--   0 jasqia     (502) staff       (20)     1705 2023-06-19 09:16:48.000000 liveramp_automation_framework-0.1.9/liveramp_automation/helper_bucket.py
--rw-r--r--   0 jasqia     (502) staff       (20)     2238 2023-07-17 09:37:25.000000 liveramp_automation_framework-0.1.9/liveramp_automation/helper_file.py
--rw-r--r--   0 jasqia     (502) staff       (20)     3116 2023-07-17 09:39:28.000000 liveramp_automation_framework-0.1.9/liveramp_automation/helper_login.py
--rw-r--r--   0 jasqia     (502) staff       (20)       72 2023-07-17 06:20:26.000000 liveramp_automation_framework-0.1.9/liveramp_automation/helper_notification.py
--rw-r--r--   0 jasqia     (502) staff       (20)      713 2023-05-03 08:30:53.000000 liveramp_automation_framework-0.1.9/liveramp_automation/parsers.py
--rw-r--r--   0 jasqia     (502) staff       (20)      670 2023-07-17 02:34:55.000000 liveramp_automation_framework-0.1.9/liveramp_automation/util_allure.py
--rw-r--r--   0 jasqia     (502) staff       (20)     1724 2023-07-17 08:47:40.000000 liveramp_automation_framework-0.1.9/liveramp_automation/util_log.py
--rw-r--r--   0 jasqia     (502) staff       (20)      742 2023-07-17 06:23:25.000000 liveramp_automation_framework-0.1.9/liveramp_automation/util_playwright.py
--rw-r--r--   0 jasqia     (502) staff       (20)     6968 2023-07-17 06:23:25.000000 liveramp_automation_framework-0.1.9/liveramp_automation/util_request.py
--rw-r--r--   0 jasqia     (502) staff       (20)      743 2023-07-17 06:23:25.000000 liveramp_automation_framework-0.1.9/liveramp_automation/util_selenium.py
--rw-r--r--   0 jasqia     (502) staff       (20)      779 2023-07-17 02:34:55.000000 liveramp_automation_framework-0.1.9/liveramp_automation/util_time.py
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-07-17 09:41:17.096069 liveramp_automation_framework-0.1.9/liveramp_automation_framework.egg-info/
--rw-r--r--   0 jasqia     (502) staff       (20)     1881 2023-07-17 09:41:16.000000 liveramp_automation_framework-0.1.9/liveramp_automation_framework.egg-info/PKG-INFO
--rw-r--r--   0 jasqia     (502) staff       (20)      666 2023-07-17 09:41:16.000000 liveramp_automation_framework-0.1.9/liveramp_automation_framework.egg-info/SOURCES.txt
--rw-r--r--   0 jasqia     (502) staff       (20)        1 2023-07-17 09:41:16.000000 liveramp_automation_framework-0.1.9/liveramp_automation_framework.egg-info/dependency_links.txt
--rw-r--r--   0 jasqia     (502) staff       (20)      381 2023-07-17 09:41:16.000000 liveramp_automation_framework-0.1.9/liveramp_automation_framework.egg-info/requires.txt
--rw-r--r--   0 jasqia     (502) staff       (20)       20 2023-07-17 09:41:16.000000 liveramp_automation_framework-0.1.9/liveramp_automation_framework.egg-info/top_level.txt
--rw-r--r--   0 jasqia     (502) staff       (20)       38 2023-07-17 09:41:17.097637 liveramp_automation_framework-0.1.9/setup.cfg
--rw-r--r--   0 jasqia     (502) staff       (20)     1169 2023-07-17 09:40:28.000000 liveramp_automation_framework-0.1.9/setup.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-07-17 10:04:42.657450 liveramp_automation_framework-0.1.9.1/
+-rw-r--r--   0 jasqia     (502) staff       (20)     1883 2023-07-17 10:04:42.656982 liveramp_automation_framework-0.1.9.1/PKG-INFO
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-07-17 10:04:42.650204 liveramp_automation_framework-0.1.9.1/liveramp_automation/
+-rw-r--r--   0 jasqia     (502) staff       (20)     1705 2023-06-19 09:16:48.000000 liveramp_automation_framework-0.1.9.1/liveramp_automation/helper_bucket.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     2238 2023-07-17 09:37:25.000000 liveramp_automation_framework-0.1.9.1/liveramp_automation/helper_file.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     3116 2023-07-17 09:39:28.000000 liveramp_automation_framework-0.1.9.1/liveramp_automation/helper_login.py
+-rw-r--r--   0 jasqia     (502) staff       (20)       72 2023-07-17 06:20:26.000000 liveramp_automation_framework-0.1.9.1/liveramp_automation/helper_notification.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      713 2023-05-03 08:30:53.000000 liveramp_automation_framework-0.1.9.1/liveramp_automation/parsers.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      670 2023-07-17 02:34:55.000000 liveramp_automation_framework-0.1.9.1/liveramp_automation/util_allure.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     1726 2023-07-17 09:48:01.000000 liveramp_automation_framework-0.1.9.1/liveramp_automation/util_log.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      742 2023-07-17 06:23:25.000000 liveramp_automation_framework-0.1.9.1/liveramp_automation/util_playwright.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     6968 2023-07-17 06:23:25.000000 liveramp_automation_framework-0.1.9.1/liveramp_automation/util_request.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      743 2023-07-17 06:23:25.000000 liveramp_automation_framework-0.1.9.1/liveramp_automation/util_selenium.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      779 2023-07-17 02:34:55.000000 liveramp_automation_framework-0.1.9.1/liveramp_automation/util_time.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-07-17 10:04:42.655757 liveramp_automation_framework-0.1.9.1/liveramp_automation_framework.egg-info/
+-rw-r--r--   0 jasqia     (502) staff       (20)     1883 2023-07-17 10:04:42.000000 liveramp_automation_framework-0.1.9.1/liveramp_automation_framework.egg-info/PKG-INFO
+-rw-r--r--   0 jasqia     (502) staff       (20)      666 2023-07-17 10:04:42.000000 liveramp_automation_framework-0.1.9.1/liveramp_automation_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)        1 2023-07-17 10:04:42.000000 liveramp_automation_framework-0.1.9.1/liveramp_automation_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)      381 2023-07-17 10:04:42.000000 liveramp_automation_framework-0.1.9.1/liveramp_automation_framework.egg-info/requires.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)       20 2023-07-17 10:04:42.000000 liveramp_automation_framework-0.1.9.1/liveramp_automation_framework.egg-info/top_level.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)       38 2023-07-17 10:04:42.657624 liveramp_automation_framework-0.1.9.1/setup.cfg
+-rw-r--r--   0 jasqia     (502) staff       (20)     1171 2023-07-17 10:04:38.000000 liveramp_automation_framework-0.1.9.1/setup.py
```

### Comparing `liveramp_automation_framework-0.1.9/PKG-INFO` & `liveramp_automation_framework-0.1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liveramp_automation_framework
-Version: 0.1.9
+Version: 0.1.9.1
 Summary: This is the base liveramp_automation_framework
 Home-page: https://github.com/LiveRamp/qe_api_framework
 Author: Jasmine Qian
 Author-email: jasmine.qian@liveramp.com
 Description-Content-Type: text/markdown
 
 ### 1. Descprition of the repository
```

### Comparing `liveramp_automation_framework-0.1.9/liveramp_automation/helper_bucket.py` & `liveramp_automation_framework-0.1.9.1/liveramp_automation/helper_bucket.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.1.9/liveramp_automation/helper_file.py` & `liveramp_automation_framework-0.1.9.1/liveramp_automation/helper_file.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.1.9/liveramp_automation/helper_login.py` & `liveramp_automation_framework-0.1.9.1/liveramp_automation/helper_login.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.1.9/liveramp_automation/parsers.py` & `liveramp_automation_framework-0.1.9.1/liveramp_automation/parsers.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.1.9/liveramp_automation/util_allure.py` & `liveramp_automation_framework-0.1.9.1/liveramp_automation/util_allure.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.1.9/liveramp_automation/util_log.py` & `liveramp_automation_framework-0.1.9.1/liveramp_automation/util_log.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 class LoggerUtils:
     _instance = None
     _lock = Lock()
 
     @classmethod
-    def __inti__(cls):
+    def get_logger(cls):
         if not cls._instance:
             with cls._lock:
                 if not cls._instance:
                     cls._instance = cls._configure_logging()
         return cls._instance
 
     @staticmethod
```

### Comparing `liveramp_automation_framework-0.1.9/liveramp_automation/util_playwright.py` & `liveramp_automation_framework-0.1.9.1/liveramp_automation/util_playwright.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.1.9/liveramp_automation/util_request.py` & `liveramp_automation_framework-0.1.9.1/liveramp_automation/util_request.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.1.9/liveramp_automation/util_selenium.py` & `liveramp_automation_framework-0.1.9.1/liveramp_automation/util_selenium.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.1.9/liveramp_automation/util_time.py` & `liveramp_automation_framework-0.1.9.1/liveramp_automation/util_time.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.1.9/liveramp_automation_framework.egg-info/PKG-INFO` & `liveramp_automation_framework-0.1.9.1/liveramp_automation_framework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liveramp-automation-framework
-Version: 0.1.9
+Version: 0.1.9.1
 Summary: This is the base liveramp_automation_framework
 Home-page: https://github.com/LiveRamp/qe_api_framework
 Author: Jasmine Qian
 Author-email: jasmine.qian@liveramp.com
 Description-Content-Type: text/markdown
 
 ### 1. Descprition of the repository
```

### Comparing `liveramp_automation_framework-0.1.9/liveramp_automation_framework.egg-info/SOURCES.txt` & `liveramp_automation_framework-0.1.9.1/liveramp_automation_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.1.9/setup.py` & `liveramp_automation_framework-0.1.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("readme.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='liveramp_automation_framework',
-    version='0.1.9',
+    version='0.1.9.1',
     author='Jasmine Qian',
     author_email='jasmine.qian@liveramp.com',
     description="This is the base liveramp_automation_framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/LiveRamp/qe_api_framework",
     packages=['liveramp_automation'],
```

