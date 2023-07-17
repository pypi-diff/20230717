# Comparing `tmp/selenium_profiles_brand-2.2.7.3.tar.gz` & `tmp/selenium_profiles_brand-2.2.7.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium_profiles_brand-2.2.7.3.tar", last modified: Mon Jul 17 10:03:57 2023, max compression
+gzip compressed data, was "selenium_profiles_brand-2.2.7.3.1.tar", last modified: Mon Jul 17 10:57:29 2023, max compression
```

## Comparing `selenium_profiles_brand-2.2.7.3.tar` & `selenium_profiles_brand-2.2.7.3.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 10:03:57.667827 selenium_profiles_brand-2.2.7.3/
--rw-rw-rw-   0        0        0      661 2023-07-17 03:46:10.000000 selenium_profiles_brand-2.2.7.3/LICENSE.md
--rw-rw-rw-   0        0        0      294 2023-07-17 09:58:05.000000 selenium_profiles_brand-2.2.7.3/MANIFEST.in
--rw-rw-rw-   0        0        0    14465 2023-07-17 10:03:57.667827 selenium_profiles_brand-2.2.7.3/PKG-INFO
--rw-rw-rw-   0        0        0    13111 2023-07-17 09:54:29.000000 selenium_profiles_brand-2.2.7.3/README.md
--rw-rw-rw-   0        0        0      101 2023-07-17 03:46:10.000000 selenium_profiles_brand-2.2.7.3/pyproject.toml
--rw-rw-rw-   0        0        0      137 2023-07-17 10:03:57.668823 selenium_profiles_brand-2.2.7.3/setup.cfg
--rw-rw-rw-   0        0        0     2144 2023-07-17 09:53:44.000000 selenium_profiles_brand-2.2.7.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 10:03:57.626573 selenium_profiles_brand-2.2.7.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-17 10:03:57.638034 selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand/
--rw-rw-rw-   0        0        0       25 2023-07-17 04:23:29.000000 selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 10:03:57.643028 selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand/files/
--rw-rw-rw-   0        0        0       21 2023-07-17 03:46:10.000000 selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand/files/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 10:03:57.645020 selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand/files/proxy_extension/
--rw-rw-rw-   0        0        0      615 2023-07-17 03:46:10.000000 selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand/files/proxy_extension/background.js
--rw-rw-rw-   0        0        0      347 2023-07-17 03:46:10.000000 selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand/files/proxy_extension/manifest.json
-drwxrwxrwx   0        0        0        0 2023-07-17 10:03:57.646017 selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand/files/tmp/
--rw-rw-rw-   0        0        0        0 2023-07-17 03:46:10.000000 selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand/files/tmp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 10:03:57.646017 selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand/files/tmp/proxy_extension/
--rw-rw-rw-   0        0        0      347 2023-07-17 03:46:10.000000 selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand/files/tmp/proxy_extension/manifest.json
-drwxrwxrwx   0        0        0        0 2023-07-17 10:03:57.649007 selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand/js/
--rw-rw-rw-   0        0        0       21 2023-07-17 03:46:10.000000 selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand/js/__init__.py
--rw-rw-rw-   0        0        0     3098 2023-07-17 03:46:10.000000 selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand/js/export_profile.js
--rw-rw-rw-   0        0        0     1243 2023-07-17 03:46:10.000000 selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand/js/fetch.js
-drwxrwxrwx   0        0        0        0 2023-07-17 10:03:57.652358 selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand/js/undetected/
--rw-rw-rw-   0        0        0        0 2023-07-17 03:46:10.000000 selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand/js/undetected/__init.py
--rw-rw-rw-   0        0        0      291 2023-07-17 03:46:10.000000 selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand/js/undetected/get_cdc_props.js
--rw-rw-rw-   0        0        0      392 2023-07-17 03:46:10.000000 selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand/js/undetected/navigator_webdriver.js
--rw-rw-rw-   0        0        0      357 2023-07-17 03:46:10.000000 selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand/js/undetected/remove_cdc_props.js
-drwxrwxrwx   0        0        0        0 2023-07-17 10:03:57.659335 selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand/profiles/
--rw-rw-rw-   0        0        0       91 2023-07-17 09:54:29.000000 selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand/profiles/__init__.py
--rw-rw-rw-   0        0        0     3080 2023-07-17 03:46:10.000000 selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand/profiles/default.json
--rw-rw-rw-   0        0        0     1856 2023-07-17 03:46:10.000000 selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand/profiles/example.json
--rw-rw-rw-   0        0        0      849 2023-07-17 09:54:29.000000 selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand/profiles/profiles.py
--rw-rw-rw-   0        0        0     1891 2023-07-17 03:46:10.000000 selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand/profiles/scratch.json
-drwxrwxrwx   0        0        0        0 2023-07-17 10:03:57.663835 selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand/scripts/
--rw-rw-rw-   0        0        0        0 2023-07-17 03:46:10.000000 selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand/scripts/__init__.py
--rw-rw-rw-   0        0        0    10729 2023-07-17 09:54:29.000000 selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand/scripts/driver_utils.py
--rw-rw-rw-   0        0        0    24928 2023-07-17 09:54:29.000000 selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand/scripts/profiles.py
--rw-rw-rw-   0        0        0     4687 2023-07-17 03:46:10.000000 selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand/scripts/proxy.py
--rw-rw-rw-   0        0        0     1667 2023-07-17 09:54:29.000000 selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand/scripts/undetected.py
-drwxrwxrwx   0        0        0        0 2023-07-17 10:03:57.665834 selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand/utils/
--rw-rw-rw-   0        0        0        0 2023-07-17 03:46:10.000000 selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand/utils/__init__.py
--rw-rw-rw-   0        0        0     1887 2023-07-17 03:46:10.000000 selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand/utils/colab_utils.py
--rw-rw-rw-   0        0        0     1773 2023-07-17 09:54:29.000000 selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand/utils/utils.py
--rw-rw-rw-   0        0        0    10300 2023-07-17 09:54:29.000000 selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand/webdriver.py
-drwxrwxrwx   0        0        0        0 2023-07-17 10:03:57.642032 selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand.egg-info/
--rw-rw-rw-   0        0        0    14465 2023-07-17 10:03:57.000000 selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1713 2023-07-17 10:03:57.000000 selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 10:03:57.000000 selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      140 2023-07-17 10:03:57.000000 selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-07-17 10:03:57.000000 selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-17 10:03:57.666833 selenium_profiles_brand-2.2.7.3/tests/
--rw-rw-rw-   0        0        0     1629 2023-07-17 09:54:29.000000 selenium_profiles_brand-2.2.7.3/tests/test_driver.py
+drwxrwxrwx   0        0        0        0 2023-07-17 10:57:29.789646 selenium_profiles_brand-2.2.7.3.1/
+-rw-rw-rw-   0        0        0      661 2023-07-17 03:46:10.000000 selenium_profiles_brand-2.2.7.3.1/LICENSE.md
+-rw-rw-rw-   0        0        0      294 2023-07-17 09:58:05.000000 selenium_profiles_brand-2.2.7.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    14467 2023-07-17 10:57:29.790642 selenium_profiles_brand-2.2.7.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0    13111 2023-07-17 09:54:29.000000 selenium_profiles_brand-2.2.7.3.1/README.md
+-rw-rw-rw-   0        0        0      101 2023-07-17 03:46:10.000000 selenium_profiles_brand-2.2.7.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0      187 2023-07-17 10:57:29.790642 selenium_profiles_brand-2.2.7.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     2144 2023-07-17 09:53:44.000000 selenium_profiles_brand-2.2.7.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 10:57:29.742511 selenium_profiles_brand-2.2.7.3.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-17 10:57:29.757468 selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand/
+-rw-rw-rw-   0        0        0       27 2023-07-17 10:56:57.000000 selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 10:57:29.763976 selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand/files/
+-rw-rw-rw-   0        0        0       21 2023-07-17 03:46:10.000000 selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand/files/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 10:57:29.766967 selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand/files/proxy_extension/
+-rw-rw-rw-   0        0        0      615 2023-07-17 03:46:10.000000 selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand/files/proxy_extension/background.js
+-rw-rw-rw-   0        0        0      347 2023-07-17 03:46:10.000000 selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand/files/proxy_extension/manifest.json
+drwxrwxrwx   0        0        0        0 2023-07-17 10:57:29.767962 selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand/files/tmp/
+-rw-rw-rw-   0        0        0        0 2023-07-17 03:46:10.000000 selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand/files/tmp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 10:57:29.768958 selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand/files/tmp/proxy_extension/
+-rw-rw-rw-   0        0        0      347 2023-07-17 03:46:10.000000 selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand/files/tmp/proxy_extension/manifest.json
+drwxrwxrwx   0        0        0        0 2023-07-17 10:57:29.770952 selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand/js/
+-rw-rw-rw-   0        0        0       21 2023-07-17 03:46:10.000000 selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand/js/__init__.py
+-rw-rw-rw-   0        0        0     3098 2023-07-17 03:46:10.000000 selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand/js/export_profile.js
+-rw-rw-rw-   0        0        0     1243 2023-07-17 03:46:10.000000 selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand/js/fetch.js
+drwxrwxrwx   0        0        0        0 2023-07-17 10:57:29.774941 selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand/js/undetected/
+-rw-rw-rw-   0        0        0        0 2023-07-17 03:46:10.000000 selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand/js/undetected/__init.py
+-rw-rw-rw-   0        0        0      291 2023-07-17 03:46:10.000000 selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand/js/undetected/get_cdc_props.js
+-rw-rw-rw-   0        0        0      392 2023-07-17 03:46:10.000000 selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand/js/undetected/navigator_webdriver.js
+-rw-rw-rw-   0        0        0      357 2023-07-17 03:46:10.000000 selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand/js/undetected/remove_cdc_props.js
+drwxrwxrwx   0        0        0        0 2023-07-17 10:57:29.781479 selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand/profiles/
+-rw-rw-rw-   0        0        0       91 2023-07-17 09:54:29.000000 selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand/profiles/__init__.py
+-rw-rw-rw-   0        0        0     3080 2023-07-17 03:46:10.000000 selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand/profiles/default.json
+-rw-rw-rw-   0        0        0     1856 2023-07-17 03:46:10.000000 selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand/profiles/example.json
+-rw-rw-rw-   0        0        0      849 2023-07-17 09:54:29.000000 selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand/profiles/profiles.py
+-rw-rw-rw-   0        0        0     1891 2023-07-17 03:46:10.000000 selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand/profiles/scratch.json
+drwxrwxrwx   0        0        0        0 2023-07-17 10:57:29.785469 selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand/scripts/
+-rw-rw-rw-   0        0        0        0 2023-07-17 03:46:10.000000 selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand/scripts/__init__.py
+-rw-rw-rw-   0        0        0    10729 2023-07-17 09:54:29.000000 selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand/scripts/driver_utils.py
+-rw-rw-rw-   0        0        0    24930 2023-07-17 10:56:57.000000 selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand/scripts/profiles.py
+-rw-rw-rw-   0        0        0     4687 2023-07-17 03:46:10.000000 selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand/scripts/proxy.py
+-rw-rw-rw-   0        0        0     1667 2023-07-17 09:54:29.000000 selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand/scripts/undetected.py
+drwxrwxrwx   0        0        0        0 2023-07-17 10:57:29.788650 selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-17 03:46:10.000000 selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand/utils/__init__.py
+-rw-rw-rw-   0        0        0     1887 2023-07-17 03:46:10.000000 selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand/utils/colab_utils.py
+-rw-rw-rw-   0        0        0     1773 2023-07-17 09:54:29.000000 selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand/utils/utils.py
+-rw-rw-rw-   0        0        0    10300 2023-07-17 09:54:29.000000 selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand/webdriver.py
+drwxrwxrwx   0        0        0        0 2023-07-17 10:57:29.762981 selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand.egg-info/
+-rw-rw-rw-   0        0        0    14467 2023-07-17 10:57:29.000000 selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1713 2023-07-17 10:57:29.000000 selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 10:57:29.000000 selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      140 2023-07-17 10:57:29.000000 selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-07-17 10:57:29.000000 selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 10:57:29.789646 selenium_profiles_brand-2.2.7.3.1/tests/
+-rw-rw-rw-   0        0        0     1629 2023-07-17 09:54:29.000000 selenium_profiles_brand-2.2.7.3.1/tests/test_driver.py
```

### Comparing `selenium_profiles_brand-2.2.7.3/LICENSE.md` & `selenium_profiles_brand-2.2.7.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `selenium_profiles_brand-2.2.7.3/PKG-INFO` & `selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: selenium_profiles_brand
-Version: 2.2.7.3
+Name: selenium-profiles-brand
+Version: 2.2.7.3.1
 Summary: Emulate and Automate Chrome using Profiles and Selenium
 Home-page: https://github.com/kaliiiiiiiiii/Selenium_Profiles
 Author: Aurin Aegerter
 Author-email: aurinliun@gmx.ch
 Project-URL: Documentation, https://github.com/kaliiiiiiiiii/Selenium_Profiles
 Project-URL: Bug Reports, https://github.com/kaliiiiiiiiii/Selenium_Profiles/issues
 Project-URL: Source Code, https://github.com/kaliiiiiiiiii/Selenium_Profiles
```

### Comparing `selenium_profiles_brand-2.2.7.3/README.md` & `selenium_profiles_brand-2.2.7.3.1/README.md`

 * *Files identical despite different names*

### Comparing `selenium_profiles_brand-2.2.7.3/setup.py` & `selenium_profiles_brand-2.2.7.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand/files/proxy_extension/background.js` & `selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand/files/proxy_extension/background.js`

 * *Files identical despite different names*

### Comparing `selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand/js/export_profile.js` & `selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand/js/export_profile.js`

 * *Files identical despite different names*

### Comparing `selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand/js/fetch.js` & `selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand/js/fetch.js`

 * *Files identical despite different names*

### Comparing `selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand/profiles/default.json` & `selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand/profiles/default.json`

 * *Files identical despite different names*

### Comparing `selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand/profiles/example.json` & `selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand/profiles/example.json`

 * *Files identical despite different names*

### Comparing `selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand/profiles/profiles.py` & `selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand/profiles/profiles.py`

 * *Files identical despite different names*

### Comparing `selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand/profiles/scratch.json` & `selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand/profiles/scratch.json`

 * *Files identical despite different names*

### Comparing `selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand/scripts/driver_utils.py` & `selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand/scripts/driver_utils.py`

 * *Files identical despite different names*

### Comparing `selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand/scripts/profiles.py` & `selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand/scripts/profiles.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
                                               version.split(".")[0] + ".0.0.0", profile["userAgent"])
 
             if profile["userAgentMetadata"]:
                 metadata = defaultdict(lambda: None)
                 # noinspection PyTypeChecker
                 metadata.update(profile["userAgentMetadata"])
 
-                brans_pattern = r'^Not[ (:-./);=?_]A[ (:-./);=?_]Brand$'
+                brans_pattern = r'^Not[ (:\-./);=?_]A[ (:\-./);=?_]Brand$'
                 if metadata["brands"]:
                     brands = []
                     # noinspection PyTypeChecker
                     for brand in metadata["brands"]:
                         if not re.match(brans_pattern, brand["brand"]):
                             brand["version"] = version.split(".")[0]
                         brands.append(brand)
```

### Comparing `selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand/scripts/proxy.py` & `selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand/scripts/proxy.py`

 * *Files identical despite different names*

### Comparing `selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand/scripts/undetected.py` & `selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand/scripts/undetected.py`

 * *Files identical despite different names*

### Comparing `selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand/utils/colab_utils.py` & `selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand/utils/colab_utils.py`

 * *Files identical despite different names*

### Comparing `selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand/utils/utils.py` & `selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand/utils/utils.py`

 * *Files identical despite different names*

### Comparing `selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand/webdriver.py` & `selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand/webdriver.py`

 * *Files identical despite different names*

### Comparing `selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand.egg-info/PKG-INFO` & `selenium_profiles_brand-2.2.7.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: selenium-profiles-brand
-Version: 2.2.7.3
+Name: selenium_profiles_brand
+Version: 2.2.7.3.1
 Summary: Emulate and Automate Chrome using Profiles and Selenium
 Home-page: https://github.com/kaliiiiiiiiii/Selenium_Profiles
 Author: Aurin Aegerter
 Author-email: aurinliun@gmx.ch
 Project-URL: Documentation, https://github.com/kaliiiiiiiiii/Selenium_Profiles
 Project-URL: Bug Reports, https://github.com/kaliiiiiiiiii/Selenium_Profiles/issues
 Project-URL: Source Code, https://github.com/kaliiiiiiiiii/Selenium_Profiles
```

### Comparing `selenium_profiles_brand-2.2.7.3/src/selenium_profiles_brand.egg-info/SOURCES.txt` & `selenium_profiles_brand-2.2.7.3.1/src/selenium_profiles_brand.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `selenium_profiles_brand-2.2.7.3/tests/test_driver.py` & `selenium_profiles_brand-2.2.7.3.1/tests/test_driver.py`

 * *Files identical despite different names*

