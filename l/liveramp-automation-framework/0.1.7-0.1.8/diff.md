# Comparing `tmp/liveramp_automation_framework-0.1.7.tar.gz` & `tmp/liveramp_automation_framework-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liveramp_automation_framework-0.1.7.tar", last modified: Tue Jun 13 08:06:17 2023, max compression
+gzip compressed data, was "liveramp_automation_framework-0.1.8.tar", last modified: Mon Jul 17 08:47:46 2023, max compression
```

## Comparing `liveramp_automation_framework-0.1.7.tar` & `liveramp_automation_framework-0.1.8.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-06-13 08:06:17.625425 liveramp_automation_framework-0.1.7/
--rw-r--r--   0 jasqia     (502) staff       (20)      818 2023-06-13 08:06:17.624921 liveramp_automation_framework-0.1.7/PKG-INFO
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-06-13 08:06:17.618456 liveramp_automation_framework-0.1.7/liveramp_automation/
--rw-r--r--   0 jasqia     (502) staff       (20)      348 2023-06-13 08:06:15.000000 liveramp_automation_framework-0.1.7/liveramp_automation/allure_util.py
--rw-r--r--   0 jasqia     (502) staff       (20)      928 2023-06-08 08:26:48.000000 liveramp_automation_framework-0.1.7/liveramp_automation/logger.py
--rw-r--r--   0 jasqia     (502) staff       (20)     3120 2023-06-12 02:49:19.000000 liveramp_automation_framework-0.1.7/liveramp_automation/login_util.py
--rw-r--r--   0 jasqia     (502) staff       (20)      713 2023-05-03 08:30:53.000000 liveramp_automation_framework-0.1.7/liveramp_automation/parsers.py
--rw-r--r--   0 jasqia     (502) staff       (20)      742 2023-06-13 07:55:12.000000 liveramp_automation_framework-0.1.7/liveramp_automation/playwright_util.py
--rw-r--r--   0 jasqia     (502) staff       (20)     2232 2023-06-13 07:16:27.000000 liveramp_automation_framework-0.1.7/liveramp_automation/read_report.py
--rw-r--r--   0 jasqia     (502) staff       (20)     6966 2023-06-13 07:16:27.000000 liveramp_automation_framework-0.1.7/liveramp_automation/request_util.py
--rw-r--r--   0 jasqia     (502) staff       (20)      743 2023-06-13 07:58:47.000000 liveramp_automation_framework-0.1.7/liveramp_automation/selenium_util.py
--rw-r--r--   0 jasqia     (502) staff       (20)      781 2023-06-08 08:16:59.000000 liveramp_automation_framework-0.1.7/liveramp_automation/time_util.py
--rw-r--r--   0 jasqia     (502) staff       (20)      718 2023-06-13 07:16:27.000000 liveramp_automation_framework-0.1.7/liveramp_automation/upload_util.py
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-06-13 08:06:17.623850 liveramp_automation_framework-0.1.7/liveramp_automation_framework.egg-info/
--rw-r--r--   0 jasqia     (502) staff       (20)      818 2023-06-13 08:06:17.000000 liveramp_automation_framework-0.1.7/liveramp_automation_framework.egg-info/PKG-INFO
--rw-r--r--   0 jasqia     (502) staff       (20)      617 2023-06-13 08:06:17.000000 liveramp_automation_framework-0.1.7/liveramp_automation_framework.egg-info/SOURCES.txt
--rw-r--r--   0 jasqia     (502) staff       (20)        1 2023-06-13 08:06:17.000000 liveramp_automation_framework-0.1.7/liveramp_automation_framework.egg-info/dependency_links.txt
--rw-r--r--   0 jasqia     (502) staff       (20)      381 2023-06-13 08:06:17.000000 liveramp_automation_framework-0.1.7/liveramp_automation_framework.egg-info/requires.txt
--rw-r--r--   0 jasqia     (502) staff       (20)       20 2023-06-13 08:06:17.000000 liveramp_automation_framework-0.1.7/liveramp_automation_framework.egg-info/top_level.txt
--rw-r--r--   0 jasqia     (502) staff       (20)       38 2023-06-13 08:06:17.625598 liveramp_automation_framework-0.1.7/setup.cfg
--rw-r--r--   0 jasqia     (502) staff       (20)     1169 2023-06-13 08:06:15.000000 liveramp_automation_framework-0.1.7/setup.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-07-17 08:47:46.204884 liveramp_automation_framework-0.1.8/
+-rw-r--r--   0 jasqia     (502) staff       (20)     1881 2023-07-17 08:47:46.204169 liveramp_automation_framework-0.1.8/PKG-INFO
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-07-17 08:47:46.195739 liveramp_automation_framework-0.1.8/liveramp_automation/
+-rw-r--r--   0 jasqia     (502) staff       (20)     1705 2023-06-19 09:16:48.000000 liveramp_automation_framework-0.1.8/liveramp_automation/helper_bucket.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     3126 2023-07-17 06:23:25.000000 liveramp_automation_framework-0.1.8/liveramp_automation/helper_login.py
+-rw-r--r--   0 jasqia     (502) staff       (20)       72 2023-07-17 06:20:26.000000 liveramp_automation_framework-0.1.8/liveramp_automation/helper_notification.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     2234 2023-07-17 06:23:25.000000 liveramp_automation_framework-0.1.8/liveramp_automation/helper_report.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      713 2023-05-03 08:30:53.000000 liveramp_automation_framework-0.1.8/liveramp_automation/parsers.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      670 2023-07-17 02:34:55.000000 liveramp_automation_framework-0.1.8/liveramp_automation/util_allure.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     1724 2023-07-17 08:47:40.000000 liveramp_automation_framework-0.1.8/liveramp_automation/util_log.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      742 2023-07-17 06:23:25.000000 liveramp_automation_framework-0.1.8/liveramp_automation/util_playwright.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     6968 2023-07-17 06:23:25.000000 liveramp_automation_framework-0.1.8/liveramp_automation/util_request.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      743 2023-07-17 06:23:25.000000 liveramp_automation_framework-0.1.8/liveramp_automation/util_selenium.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      779 2023-07-17 02:34:55.000000 liveramp_automation_framework-0.1.8/liveramp_automation/util_time.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-07-17 08:47:46.202793 liveramp_automation_framework-0.1.8/liveramp_automation_framework.egg-info/
+-rw-r--r--   0 jasqia     (502) staff       (20)     1881 2023-07-17 08:47:46.000000 liveramp_automation_framework-0.1.8/liveramp_automation_framework.egg-info/PKG-INFO
+-rw-r--r--   0 jasqia     (502) staff       (20)      668 2023-07-17 08:47:46.000000 liveramp_automation_framework-0.1.8/liveramp_automation_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)        1 2023-07-17 08:47:46.000000 liveramp_automation_framework-0.1.8/liveramp_automation_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)      381 2023-07-17 08:47:46.000000 liveramp_automation_framework-0.1.8/liveramp_automation_framework.egg-info/requires.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)       20 2023-07-17 08:47:46.000000 liveramp_automation_framework-0.1.8/liveramp_automation_framework.egg-info/top_level.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)       38 2023-07-17 08:47:46.205089 liveramp_automation_framework-0.1.8/setup.cfg
+-rw-r--r--   0 jasqia     (502) staff       (20)     1169 2023-07-17 08:47:40.000000 liveramp_automation_framework-0.1.8/setup.py
```

### Comparing `liveramp_automation_framework-0.1.7/liveramp_automation/login_util.py` & `liveramp_automation_framework-0.1.8/liveramp_automation/helper_login.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,62 +1,62 @@
 import requests
 from selenium.webdriver import Keys
 from selenium.webdriver.common.by import By
-from liveramp_automation.logger import Logger
-from liveramp_automation.time_util import windows_wait
+from liveramp_automation.util_log import Logger as Logger
+from liveramp_automation.util_time import fixed_wait
 
 
-class Login:
+class LoginHepler:
 
     @staticmethod
     def liveramp_okta_login_page(page, config, USERNAME, PASSWORD):
         # navigate to the Okta login page
         Logger.info("We are going to login to OKTA")
         url = config['login_url']
         Logger.info("The login url is {}".format(url))
         page.goto(url)
-        windows_wait()
+        fixed_wait()
         url_new = page.url
         Logger.info("The current url is {}".format(url_new))
         if url_new.__contains__(url):
             Logger.info("We've already logan to OKTA succefully")
         else:
             page.fill('#idp-discovery-username', USERNAME)
             page.get_by_role("button", name="Next").click()
             page.get_by_role("textbox", name="Password").fill(PASSWORD)
             page.get_by_role("button", name="Sign In").click()
             Logger.info("We could login to OKTA successfully")
             # wait for the login process to complete
-            windows_wait(20)
+            fixed_wait(20)
 
     @staticmethod
     def liveramp_okta_login_driver(driver, config, USERNAME, PASSWORD):
         # navigate to the Okta login page
         Logger.info("We are going to login to OKTA")
         url = config['login_url']
         Logger.info("The login url is {}".format(url))
         driver.get(url)
-        windows_wait()
+        fixed_wait()
         if driver.current_url.__contains__(url):
             Logger.info("We've already logan to OKTA succefully")
         else:
             # username = driver.find_element_by_id('idp-discovery-username')
             username = driver.find_element(by=By.ID, value='idp-discovery-username')
             username.send_keys(USERNAME)
             username.send_keys(Keys.ENTER)
-            windows_wait()
+            fixed_wait()
             # password = driver.find_element_by_id('okta-signin-password')
             password = driver.find_element(by=By.ID, value='okta-signin-password')
             password.send_keys(PASSWORD)
             # driver.find_element_by_id('okta-signin-submit').click()
             submit_button = driver.find_element(by=By.ID, value='okta-signin-submit')
             submit_button.click()
             Logger.info("We could login to OKTA successfully")
             # wait for the login process to complete
-            windows_wait(20)
+            fixed_wait(20)
 
     @staticmethod
     def call_oauth2_get_token(APIUSERNAME, APIPASSWORD):
         params = {
             "grant_type": "password",
             "scope": "openid",
             "client_id": "liveramp-api"
```

### Comparing `liveramp_automation_framework-0.1.7/liveramp_automation/parsers.py` & `liveramp_automation_framework-0.1.8/liveramp_automation/parsers.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.1.7/liveramp_automation/playwright_util.py` & `liveramp_automation_framework-0.1.8/liveramp_automation/util_playwright.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from urllib.parse import urlparse, urlunsplit
-from liveramp_automation.time_util import MACROS
+from liveramp_automation.util_time import MACROS
 
 
 class PlaywrightUtils:
 
     def navigate_url(page, scheme=None, host_name=None, path=None, query=None):
         parsed_uri = urlparse(page.url)
         page.goto(urlunsplit((parsed_uri.scheme if scheme is None else scheme,
```

### Comparing `liveramp_automation_framework-0.1.7/liveramp_automation/read_report.py` & `liveramp_automation_framework-0.1.8/liveramp_automation/helper_report.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 import yaml
-from liveramp_automation.logger import Logger
+from liveramp_automation.util_log import Logger
 
 
 class Report:
 
     @staticmethod
     def read_json_report(path) -> dict:
         with open(path, 'r') as file:
```

### Comparing `liveramp_automation_framework-0.1.7/liveramp_automation/request_util.py` & `liveramp_automation_framework-0.1.8/liveramp_automation/util_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import requests
-from liveramp_automation.allure_util import *
-from liveramp_automation.logger import Logger
+from liveramp_automation.util_allure import *
+from liveramp_automation.util_log import Logger
 
 
 def request_post(url, headers, data=None, json=None):
     Logger.info("The url infomation is {}".format(url))
     Logger.info("The request method is POST")
     allure_attach_text("The url infomation is {}".format(url), "URL")
     allure_attach_text("The request method is POST", "Method")
```

### Comparing `liveramp_automation_framework-0.1.7/liveramp_automation/selenium_util.py` & `liveramp_automation_framework-0.1.8/liveramp_automation/util_selenium.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from urllib.parse import urlparse, urlunsplit
-from liveramp_automation.time_util import MACROS
+from liveramp_automation.util_time import MACROS
 
 
 class SeleniumUtils:
 
     def navigate_url(driver, scheme=None, host_name=None, path=None, query=None):
         parsed_uri = urlparse(driver.url)
         driver.get(urlunsplit((parsed_uri.scheme if scheme is None else scheme,
```

### Comparing `liveramp_automation_framework-0.1.7/liveramp_automation/time_util.py` & `liveramp_automation_framework-0.1.8/liveramp_automation/util_time.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,9 +10,9 @@
     "nowconnect": datetime.now().strftime("%Y%m%d-%H%M%S"),  # data ingestion must be in yyyymmdd-hhmmss format
     "three_days_ago": (date.today() - timedelta(days=0)).strftime("%Y%m%d"),
     "two_hours_from_now": (datetime.now() + timedelta(hours=2)).strftime("%Y%m%d-%H%M%S"),
     "24hours_before_now": (datetime.now() - timedelta(hours=24)).strftime("%Y%m%d%H%M%S")
 }
 
 
-def windows_wait(value=3):
+def fixed_wait(value=3):
     time.sleep(value)
```

### Comparing `liveramp_automation_framework-0.1.7/setup.py` & `liveramp_automation_framework-0.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("readme.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='liveramp_automation_framework',
-    version='0.1.7',
+    version='0.1.8',
     author='Jasmine Qian',
     author_email='jasmine.qian@liveramp.com',
     description="This is the base liveramp_automation_framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/LiveRamp/qe_api_framework",
     packages=['liveramp_automation'],
```

