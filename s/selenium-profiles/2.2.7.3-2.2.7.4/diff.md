# Comparing `tmp/selenium_profiles-2.2.7.3.tar.gz` & `tmp/selenium_profiles-2.2.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\selenium_profiles-2.2.7.3.tar", last modified: Fri Jul 14 14:03:50 2023, max compression
+gzip compressed data, was "dist\selenium_profiles-2.2.7.4.tar", last modified: Mon Jul 17 11:12:08 2023, max compression
```

## Comparing `selenium_profiles-2.2.7.3.tar` & `selenium_profiles-2.2.7.4.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 14:03:50.000000 selenium_profiles-2.2.7.3/
--rw-rw-rw-   0        0        0      641 2022-11-24 08:41:11.000000 selenium_profiles-2.2.7.3/LICENSE.md
--rw-rw-rw-   0        0        0      261 2023-01-17 17:45:34.000000 selenium_profiles-2.2.7.3/MANIFEST.in
--rw-rw-rw-   0        0        0    14374 2023-07-14 14:03:50.000000 selenium_profiles-2.2.7.3/PKG-INFO
--rw-rw-rw-   0        0        0    13026 2023-07-14 13:59:58.000000 selenium_profiles-2.2.7.3/README.md
--rw-rw-rw-   0        0        0     1740 2023-07-03 16:17:23.000000 selenium_profiles-2.2.7.3/build_upload.md
--rw-rw-rw-   0        0        0      101 2022-11-24 08:05:09.000000 selenium_profiles-2.2.7.3/pyproject.toml
--rw-rw-rw-   0        0        0      131 2023-07-14 14:03:50.000000 selenium_profiles-2.2.7.3/setup.cfg
--rw-rw-rw-   0        0        0     2083 2023-07-14 14:01:27.000000 selenium_profiles-2.2.7.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-14 14:03:50.000000 selenium_profiles-2.2.7.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-14 14:03:50.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/
--rw-rw-rw-   0        0        0       25 2023-07-14 14:01:02.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 14:03:50.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/files/
--rw-rw-rw-   0        0        0       21 2022-11-24 09:43:39.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/files/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 14:03:50.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/files/proxy_extension/
--rw-rw-rw-   0        0        0      615 2023-01-17 17:37:32.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/files/proxy_extension/background.js
--rw-rw-rw-   0        0        0      347 2023-01-17 07:03:50.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/files/proxy_extension/manifest.json
-drwxrwxrwx   0        0        0        0 2023-07-14 14:03:50.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/files/tmp/
--rw-rw-rw-   0        0        0        0 2023-01-17 07:50:51.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/files/tmp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 14:03:50.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/files/tmp/proxy_extension/
--rw-rw-rw-   0        0        0      652 2023-04-12 17:20:07.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/files/tmp/proxy_extension/background.js
--rw-rw-rw-   0        0        0      347 2023-04-12 17:20:07.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/files/tmp/proxy_extension/manifest.json
-drwxrwxrwx   0        0        0        0 2023-07-14 14:03:50.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/js/
--rw-rw-rw-   0        0        0       21 2022-11-24 09:43:39.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/js/__init__.py
--rw-rw-rw-   0        0        0     3098 2023-04-09 15:39:08.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/js/export_profile.js
--rw-rw-rw-   0        0        0     1243 2023-04-09 15:50:01.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/js/fetch.js
-drwxrwxrwx   0        0        0        0 2023-07-14 14:03:50.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/js/undetected/
--rw-rw-rw-   0        0        0        0 2022-11-30 15:39:00.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/js/undetected/__init.py
--rw-rw-rw-   0        0        0      291 2022-11-30 15:48:11.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/js/undetected/get_cdc_props.js
--rw-rw-rw-   0        0        0      392 2022-11-30 15:43:54.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/js/undetected/navigator_webdriver.js
--rw-rw-rw-   0        0        0      357 2022-11-30 15:51:50.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/js/undetected/remove_cdc_props.js
-drwxrwxrwx   0        0        0        0 2023-07-14 14:03:50.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/profiles/
--rw-rw-rw-   0        0        0       85 2022-11-24 12:02:54.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/profiles/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 14:03:50.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/profiles/__pycache__/
--rw-rw-rw-   0        0        0      293 2023-04-10 19:28:24.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/profiles/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      287 2023-04-09 11:28:56.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/profiles/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0     1419 2023-04-10 19:28:24.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/profiles/__pycache__/profiles.cpython-310.pyc
--rw-rw-rw-   0        0        0     1418 2023-06-20 17:12:11.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/profiles/__pycache__/profiles.cpython-37.pyc
--rw-rw-rw-   0        0        0     3080 2023-04-10 20:03:55.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/profiles/default.json
--rw-rw-rw-   0        0        0     1856 2023-04-10 20:31:32.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/profiles/example.json
--rw-rw-rw-   0        0        0      837 2023-06-20 17:12:01.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/profiles/profiles.py
--rw-rw-rw-   0        0        0     1891 2022-12-17 00:01:23.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/profiles/scratch.json
-drwxrwxrwx   0        0        0        0 2023-07-14 14:03:50.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/scripts/
--rw-rw-rw-   0        0        0        0 2022-11-29 13:10:11.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/scripts/__init__.py
--rw-rw-rw-   0        0        0    10723 2023-06-20 19:25:57.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/scripts/driver_utils.py
--rw-rw-rw-   0        0        0    24902 2023-06-27 09:54:03.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/scripts/profiles.py
--rw-rw-rw-   0        0        0     4687 2023-06-27 07:04:38.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/scripts/proxy.py
--rw-rw-rw-   0        0        0     1649 2023-06-26 05:06:24.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/scripts/undetected.py
-drwxrwxrwx   0        0        0        0 2023-07-14 14:03:50.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/utils/
--rw-rw-rw-   0        0        0        0 2023-01-13 13:06:48.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/utils/__init__.py
--rw-rw-rw-   0        0        0     1887 2023-03-16 14:15:27.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/utils/colab_utils.py
--rw-rw-rw-   0        0        0     1755 2023-06-26 05:36:03.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/utils/utils.py
--rw-rw-rw-   0        0        0    10234 2023-07-14 13:57:17.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/webdriver.py
-drwxrwxrwx   0        0        0        0 2023-07-14 14:03:50.000000 selenium_profiles-2.2.7.3/src/selenium_profiles.egg-info/
--rw-rw-rw-   0        0        0    14374 2023-07-14 14:03:50.000000 selenium_profiles-2.2.7.3/src/selenium_profiles.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1869 2023-07-14 14:03:50.000000 selenium_profiles-2.2.7.3/src/selenium_profiles.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 14:03:50.000000 selenium_profiles-2.2.7.3/src/selenium_profiles.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      140 2023-07-14 14:03:50.000000 selenium_profiles-2.2.7.3/src/selenium_profiles.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-07-14 14:03:50.000000 selenium_profiles-2.2.7.3/src/selenium_profiles.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-14 14:03:50.000000 selenium_profiles-2.2.7.3/tests/
--rw-rw-rw-   0        0        0     1617 2023-06-27 16:34:45.000000 selenium_profiles-2.2.7.3/tests/test_driver.py
+drwxrwxrwx   0        0        0        0 2023-07-17 11:12:08.000000 selenium_profiles-2.2.7.4/
+-rw-rw-rw-   0        0        0      641 2022-11-24 08:41:11.000000 selenium_profiles-2.2.7.4/LICENSE.md
+-rw-rw-rw-   0        0        0      261 2023-01-17 17:45:34.000000 selenium_profiles-2.2.7.4/MANIFEST.in
+-rw-rw-rw-   0        0        0    14332 2023-07-17 11:12:08.000000 selenium_profiles-2.2.7.4/PKG-INFO
+-rw-rw-rw-   0        0        0    12984 2023-07-16 17:28:04.000000 selenium_profiles-2.2.7.4/README.md
+-rw-rw-rw-   0        0        0     1740 2023-07-03 16:17:23.000000 selenium_profiles-2.2.7.4/build_upload.md
+-rw-rw-rw-   0        0        0      101 2022-11-24 08:05:09.000000 selenium_profiles-2.2.7.4/pyproject.toml
+-rw-rw-rw-   0        0        0      131 2023-07-17 11:12:08.000000 selenium_profiles-2.2.7.4/setup.cfg
+-rw-rw-rw-   0        0        0     2083 2023-07-14 14:01:27.000000 selenium_profiles-2.2.7.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 11:12:08.000000 selenium_profiles-2.2.7.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-17 11:12:08.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/
+-rw-rw-rw-   0        0        0       25 2023-07-17 11:12:07.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 11:12:08.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/files/
+-rw-rw-rw-   0        0        0       21 2022-11-24 09:43:39.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/files/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 11:12:08.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/files/proxy_extension/
+-rw-rw-rw-   0        0        0      615 2023-01-17 17:37:32.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/files/proxy_extension/background.js
+-rw-rw-rw-   0        0        0      347 2023-01-17 07:03:50.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/files/proxy_extension/manifest.json
+drwxrwxrwx   0        0        0        0 2023-07-17 11:12:08.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/files/tmp/
+-rw-rw-rw-   0        0        0        0 2023-01-17 07:50:51.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/files/tmp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 11:12:08.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/files/tmp/proxy_extension/
+-rw-rw-rw-   0        0        0      652 2023-04-12 17:20:07.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/files/tmp/proxy_extension/background.js
+-rw-rw-rw-   0        0        0      347 2023-04-12 17:20:07.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/files/tmp/proxy_extension/manifest.json
+drwxrwxrwx   0        0        0        0 2023-07-17 11:12:08.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/js/
+-rw-rw-rw-   0        0        0       21 2022-11-24 09:43:39.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/js/__init__.py
+-rw-rw-rw-   0        0        0     3098 2023-04-09 15:39:08.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/js/export_profile.js
+-rw-rw-rw-   0        0        0     1243 2023-04-09 15:50:01.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/js/fetch.js
+drwxrwxrwx   0        0        0        0 2023-07-17 11:12:08.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/js/undetected/
+-rw-rw-rw-   0        0        0        0 2022-11-30 15:39:00.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/js/undetected/__init.py
+-rw-rw-rw-   0        0        0      291 2022-11-30 15:48:11.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/js/undetected/get_cdc_props.js
+-rw-rw-rw-   0        0        0      392 2022-11-30 15:43:54.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/js/undetected/navigator_webdriver.js
+-rw-rw-rw-   0        0        0      357 2022-11-30 15:51:50.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/js/undetected/remove_cdc_props.js
+drwxrwxrwx   0        0        0        0 2023-07-17 11:12:08.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/profiles/
+-rw-rw-rw-   0        0        0       85 2022-11-24 12:02:54.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/profiles/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 11:12:08.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/profiles/__pycache__/
+-rw-rw-rw-   0        0        0      293 2023-04-10 19:28:24.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/profiles/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      287 2023-04-09 11:28:56.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/profiles/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1419 2023-04-10 19:28:24.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/profiles/__pycache__/profiles.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1418 2023-06-20 17:12:11.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/profiles/__pycache__/profiles.cpython-37.pyc
+-rw-rw-rw-   0        0        0     2997 2023-07-16 17:33:38.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/profiles/default.json
+-rw-rw-rw-   0        0        0     1816 2023-07-16 17:28:04.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/profiles/example.json
+-rw-rw-rw-   0        0        0      837 2023-06-20 17:12:01.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/profiles/profiles.py
+-rw-rw-rw-   0        0        0     1891 2022-12-17 00:01:23.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/profiles/scratch.json
+drwxrwxrwx   0        0        0        0 2023-07-17 11:12:08.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/scripts/
+-rw-rw-rw-   0        0        0        0 2022-11-29 13:10:11.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/scripts/__init__.py
+-rw-rw-rw-   0        0        0    10723 2023-06-20 19:25:57.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/scripts/driver_utils.py
+-rw-rw-rw-   0        0        0    24206 2023-07-17 11:06:31.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/scripts/profiles.py
+-rw-rw-rw-   0        0        0     4687 2023-06-27 07:04:38.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/scripts/proxy.py
+-rw-rw-rw-   0        0        0     1649 2023-06-26 05:06:24.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/scripts/undetected.py
+drwxrwxrwx   0        0        0        0 2023-07-17 11:12:08.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/utils/
+-rw-rw-rw-   0        0        0        0 2023-01-13 13:06:48.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/utils/__init__.py
+-rw-rw-rw-   0        0        0     1887 2023-03-16 14:15:27.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/utils/colab_utils.py
+-rw-rw-rw-   0        0        0     1755 2023-06-26 05:36:03.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/utils/utils.py
+-rw-rw-rw-   0        0        0    10234 2023-07-14 13:57:17.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/webdriver.py
+drwxrwxrwx   0        0        0        0 2023-07-17 11:12:08.000000 selenium_profiles-2.2.7.4/src/selenium_profiles.egg-info/
+-rw-rw-rw-   0        0        0    14332 2023-07-17 11:12:07.000000 selenium_profiles-2.2.7.4/src/selenium_profiles.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1869 2023-07-17 11:12:07.000000 selenium_profiles-2.2.7.4/src/selenium_profiles.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 11:12:07.000000 selenium_profiles-2.2.7.4/src/selenium_profiles.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      140 2023-07-17 11:12:07.000000 selenium_profiles-2.2.7.4/src/selenium_profiles.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-07-17 11:12:07.000000 selenium_profiles-2.2.7.4/src/selenium_profiles.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 11:12:08.000000 selenium_profiles-2.2.7.4/tests/
+-rw-rw-rw-   0        0        0     1617 2023-06-27 16:34:45.000000 selenium_profiles-2.2.7.4/tests/test_driver.py
```

### Comparing `selenium_profiles-2.2.7.3/LICENSE.md` & `selenium_profiles-2.2.7.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7.3/PKG-INFO` & `selenium_profiles-2.2.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium_profiles
-Version: 2.2.7.3
+Version: 2.2.7.4
 Summary: Emulate and Automate Chrome using Profiles and Selenium
 Home-page: https://github.com/kaliiiiiiiiii/Selenium_Profiles
 Author: Aurin Aegerter
 Author-email: aurinliun@gmx.ch
 Project-URL: Documentation, https://github.com/kaliiiiiiiiii/Selenium_Profiles
 Project-URL: Bug Reports, https://github.com/kaliiiiiiiiii/Selenium_Profiles/issues
 Project-URL: Source Code, https://github.com/kaliiiiiiiiii/Selenium_Profiles
@@ -93,15 +93,14 @@
 
 Example Profile: 
 ```python
 profile = \
 {
   "options": {
       "sandbox": True,
-      "window_size": {"x":1024,"y":648},
       "headless": False,
       "load_images": True,
       "incognito": True,
       "touch": True,
       "app": False,
       "gpu": False,
       "proxy": "http://example-proxy.com:9000", # note: auth not supported,
```

### Comparing `selenium_profiles-2.2.7.3/README.md` & `selenium_profiles-2.2.7.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,14 @@
 
 Example Profile: 
 ```python
 profile = \
 {
   "options": {
       "sandbox": True,
-      "window_size": {"x":1024,"y":648},
       "headless": False,
       "load_images": True,
       "incognito": True,
       "touch": True,
       "app": False,
       "gpu": False,
       "proxy": "http://example-proxy.com:9000", # note: auth not supported,
```

### Comparing `selenium_profiles-2.2.7.3/build_upload.md` & `selenium_profiles-2.2.7.4/build_upload.md`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7.3/setup.py` & `selenium_profiles-2.2.7.4/setup.py`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7.3/src/selenium_profiles/files/proxy_extension/background.js` & `selenium_profiles-2.2.7.4/src/selenium_profiles/files/proxy_extension/background.js`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7.3/src/selenium_profiles/files/tmp/proxy_extension/background.js` & `selenium_profiles-2.2.7.4/src/selenium_profiles/files/tmp/proxy_extension/background.js`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7.3/src/selenium_profiles/js/export_profile.js` & `selenium_profiles-2.2.7.4/src/selenium_profiles/js/export_profile.js`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7.3/src/selenium_profiles/js/fetch.js` & `selenium_profiles-2.2.7.4/src/selenium_profiles/js/fetch.js`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7.3/src/selenium_profiles/profiles/__pycache__/profiles.cpython-310.pyc` & `selenium_profiles-2.2.7.4/src/selenium_profiles/profiles/__pycache__/profiles.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7.3/src/selenium_profiles/profiles/__pycache__/profiles.cpython-37.pyc` & `selenium_profiles-2.2.7.4/src/selenium_profiles/profiles/__pycache__/profiles.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7.3/src/selenium_profiles/profiles/default.json` & `selenium_profiles-2.2.7.4/src/selenium_profiles/profiles/default.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'Android'": "{'options': {delete: ['window_size']}}",*

 * * "'Windows'": "{'options': {delete: ['window_size']}}"}*

```diff
@@ -56,19 +56,15 @@
                     "platform": "Android",
                     "platformVersion": "11.0.0",
                     "wow64": false
                 }
             }
         },
         "options": {
-            "gpu": false,
-            "window_size": {
-                "x": 384,
-                "y": 700
-            }
+            "gpu": false
         }
     },
     "IOS": {},
     "Linux": {},
     "Tablet": {},
     "Windows": {
         "cdp": {
@@ -127,15 +123,11 @@
                     "platform": "Windows",
                     "platformVersion": "10.0.0",
                     "wow64": false
                 }
             }
         },
         "options": {
-            "gpu": false,
-            "window_size": {
-                "x": 1024,
-                "y": 648
-            }
+            "gpu": false
         }
     }
 }
```

### Comparing `selenium_profiles-2.2.7.3/src/selenium_profiles/profiles/example.json` & `selenium_profiles-2.2.7.4/src/selenium_profiles/profiles/example.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9821428571428572%*

 * *Differences: {"'options'": "{delete: ['window_size']}"}*

```diff
@@ -73,14 +73,10 @@
         "capabilities": [],
         "extension_paths": [],
         "gpu": false,
         "headless": false,
         "incognito": true,
         "load_images": true,
         "proxy": null,
-        "sandbox": true,
-        "window_size": {
-            "x": 1024,
-            "y": 648
-        }
+        "sandbox": true
     }
 }
```

### Comparing `selenium_profiles-2.2.7.3/src/selenium_profiles/profiles/profiles.py` & `selenium_profiles-2.2.7.4/src/selenium_profiles/profiles/profiles.py`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7.3/src/selenium_profiles/profiles/scratch.json` & `selenium_profiles-2.2.7.4/src/selenium_profiles/profiles/scratch.json`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7.3/src/selenium_profiles/scripts/driver_utils.py` & `selenium_profiles-2.2.7.4/src/selenium_profiles/scripts/driver_utils.py`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7.3/src/selenium_profiles/scripts/profiles.py` & `selenium_profiles-2.2.7.4/src/selenium_profiles/scripts/profiles.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,40 +94,41 @@
                 import re
                 version = re.findall(r'(?<=Chrome/)\d+(?:\.\d+)+|(?<=Chromium/)\d+(?:\.\d+)+', useragent)
                 version = version[0]
             else:
                 raise ValueError("driver or version needs to be specified")
 
         if type(version) == str:
+            import re
             if profile["userAgent"]:
-                import re
                 # noinspection PyTypeChecker
                 profile["userAgent"] = re.sub(r"(?<=Chrome/)\d+(?:\.\d+)+|(?<=Chromium/)\d+(?:\.\d+)+",
                                               version.split(".")[0] + ".0.0.0", profile["userAgent"])
 
             if profile["userAgentMetadata"]:
                 metadata = defaultdict(lambda: None)
                 # noinspection PyTypeChecker
                 metadata.update(profile["userAgentMetadata"])
 
+                brands_pattern = r'^Not[ (:\-./);=?]A[ (:\-./);=?]Brand$'
                 if metadata["brands"]:
                     brands = []
                     # noinspection PyTypeChecker
                     for brand in metadata["brands"]:
-                        if not (brand["brand"] == "Not=A?Brand" or brand["brand"] == "Not)A;Brand"):
+                        if not re.match(brands_pattern, brand["brand"]):
                             brand["version"] = version.split(".")[0]
                         brands.append(brand)
                     # noinspection PyTypeChecker
                     metadata["brands"] = brands
 
                 if metadata["fullVersionList"]:
                     version_list = []
                     # noinspection PyTypeChecker
                     for i in metadata["fullVersionList"]:
-                        if not (i["brand"] == "Not=A?Brand" or i["brand"] == "Not)A;Brand"):
+                        if not re.match(brands_pattern, i["brand"]):
                             i["version"] = version
                         version_list.append(i)
                     # noinspection PyTypeChecker
                     metadata["fullVersionList"] = version_list
 
                 if metadata["fullVersion"]:
                     metadata["fullVersion"] = version
@@ -145,14 +146,15 @@
         if emulation:
 
             # fix for https://github.com/kaliiiiiiiiii/Selenium-Profiles/issues/29
             if not "screenWidth" in emulation.keys():
                 emulation.update({"screenWidth": emulation["width"]})
             if not "screenHeight" in emulation.keys():
                 emulation.update({"screenHeight": emulation["height"]})
+            self._driver.set_window_rect(0,0,emulation["width"], emulation["height"])
 
             return self._driver.execute_cdp_cmd('Emulation.setDeviceMetricsOverride', emulation)
 
     def clear_emulation(self, enabled:bool or None):
         if enabled or (enabled is None):
             self._driver.execute_cdp_cmd("Emulation.clearDeviceMetricsOverride", {})
 
@@ -205,34 +207,36 @@
     def remove_evaluate_on_document(self, identifier: int):
         del self.evaluate_on_document_identifiers[identifier]
         return self._driver.execute_cdp_cmd("Page.removeScriptToEvaluateOnNewDocument", {"identifier": str(identifier)})
 
 class options:  # webdriver.Chrome or uc.Chrome options
     # noinspection PyDefaultArgument,PyShadowingNames
     def __init__(self, options, options_profile: dict or None = None, duplicate_policy: str = "warn-add",
-                 safe_duplicates: list = ["--add-extension"]):
+                 safe_duplicates: list = None):
         """
         :param options:  for example ChromeOptions()
         :param options_profile: # profile["options"] for a Selenium-Profiles profile
         :param duplicate_policy: for args | "raise" or "replace" or "warn-replace" or "skip" or "warn-skip" or "add" or "warn-add"
         exact duplicates always get removed with a warning
         """
         if not options_profile:
             options_profile = {}
         self.profile = defaultdict(lambda: None)
         self.profile.update(options_profile)
 
         self.duplicate_policy = duplicate_policy
         self.duplicates = defaultdict(lambda: set())
+        if not safe_duplicates:
+            safe_duplicates = []
         self.safe_duplicates = safe_duplicates
 
         self.Options = options
         self.to_capabilities = self.Options.to_capabilities
 
-        self._profile_keys = ["sandbox", "window_size", "headless", "load_images", "incognito", "touch", "app", "gpu",
+        self._profile_keys = ["sandbox", "headless", "load_images", "incognito", "touch", "app", "gpu",
                               "proxy", "args", "capabilities", "experimental_options", "adb", "adb_package",
                               "use_running_app",
                               "extension_paths",
                               ]
         self._supported_duplicate_policies = ["raise", "replace", "warn-replace",
                                               "skip", "warn-skip", "add", "warn-add"]
 
@@ -241,15 +245,14 @@
     def apply(self, options_profile):
         profile = defaultdict(lambda: None)
         profile.update(options_profile)
 
         valid_key(profile.keys(), self._profile_keys, "options_profile => profile['options']")
         # libs
         self.sandbox(enabled=profile["sandbox"], adb=profile["adb"])
-        self.window_size(profile["window_size"], adb=profile["adb"])
         self.headless(profile["headless"], profile["load_images"])
         self.incognito(profile["incognito"], profile["extensions"])
         self.touch(profile["touch"])
         self.app(profile["app"], adb=profile["adb"])
         self.gpu(profile["gpu"], adb=profile["adb"])
         self.proxy(profile["proxy"])
         self.extend_arguments(profile["args"])
@@ -264,29 +267,14 @@
         """
         :param enabled: defaults to True
         """
         if enabled is False:
             self.warn_adb_unsupported(adb, "disabling sandbox")
             self.extend_arguments(["--no-sandbox", "--test-type"])
 
-    # noinspection PyDefaultArgument
-    def window_size(self, size: Dict[str, str] or None = None, adb: bool or None = None):
-        """
-        :param size: defaults to default
-        :param adb: warning
-        """
-        if size:
-            self.warn_adb_unsupported(adb, "setting window_size")
-            if "x" not in size.keys():
-                raise ValueError("value 'x' is required for specifying window_size")
-            if "y" not in size.keys():
-                raise ValueError("value 'y' is required for specifying window_size")
-            valid_key(size.keys(), ["x", "y"], 'profile_options window_size => profile["options"]["window_size]')
-            self.add_argument("--window-size=" + str(size['x']) + "," + str(size['y']))
-
     # noinspection PyIncorrectDocstring
     def headless(self, headless: bool or None = None, load_images: bool or None = None, adb: bool or None = None):
         """
         :param headless: defaults to False
         :param load_images: defaults to True
         """
```

### Comparing `selenium_profiles-2.2.7.3/src/selenium_profiles/scripts/proxy.py` & `selenium_profiles-2.2.7.4/src/selenium_profiles/scripts/proxy.py`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7.3/src/selenium_profiles/scripts/undetected.py` & `selenium_profiles-2.2.7.4/src/selenium_profiles/scripts/undetected.py`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7.3/src/selenium_profiles/utils/colab_utils.py` & `selenium_profiles-2.2.7.4/src/selenium_profiles/utils/colab_utils.py`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7.3/src/selenium_profiles/utils/utils.py` & `selenium_profiles-2.2.7.4/src/selenium_profiles/utils/utils.py`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7.3/src/selenium_profiles/webdriver.py` & `selenium_profiles-2.2.7.4/src/selenium_profiles/webdriver.py`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7.3/src/selenium_profiles.egg-info/PKG-INFO` & `selenium_profiles-2.2.7.4/src/selenium_profiles.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium-profiles
-Version: 2.2.7.3
+Version: 2.2.7.4
 Summary: Emulate and Automate Chrome using Profiles and Selenium
 Home-page: https://github.com/kaliiiiiiiiii/Selenium_Profiles
 Author: Aurin Aegerter
 Author-email: aurinliun@gmx.ch
 Project-URL: Documentation, https://github.com/kaliiiiiiiiii/Selenium_Profiles
 Project-URL: Bug Reports, https://github.com/kaliiiiiiiiii/Selenium_Profiles/issues
 Project-URL: Source Code, https://github.com/kaliiiiiiiiii/Selenium_Profiles
@@ -93,15 +93,14 @@
 
 Example Profile: 
 ```python
 profile = \
 {
   "options": {
       "sandbox": True,
-      "window_size": {"x":1024,"y":648},
       "headless": False,
       "load_images": True,
       "incognito": True,
       "touch": True,
       "app": False,
       "gpu": False,
       "proxy": "http://example-proxy.com:9000", # note: auth not supported,
```

### Comparing `selenium_profiles-2.2.7.3/src/selenium_profiles.egg-info/SOURCES.txt` & `selenium_profiles-2.2.7.4/src/selenium_profiles.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7.3/tests/test_driver.py` & `selenium_profiles-2.2.7.4/tests/test_driver.py`

 * *Files identical despite different names*

