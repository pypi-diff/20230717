# Comparing `tmp/whop-api-wrapper-1.0.3.tar.gz` & `tmp/whop-api-wrapper-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whop-api-wrapper-1.0.3.tar", last modified: Mon Jul 17 08:20:49 2023, max compression
+gzip compressed data, was "whop-api-wrapper-1.0.4.tar", last modified: Mon Jul 17 08:26:16 2023, max compression
```

## Comparing `whop-api-wrapper-1.0.3.tar` & `whop-api-wrapper-1.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 08:20:49.638229 whop-api-wrapper-1.0.3/
--rw-rw-rw-   0        0        0     1089 2023-07-17 07:39:09.000000 whop-api-wrapper-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     2064 2023-07-17 08:20:49.637232 whop-api-wrapper-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1306 2023-07-17 08:12:50.000000 whop-api-wrapper-1.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-07-17 08:20:49.638229 whop-api-wrapper-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1018 2023-07-17 08:20:48.000000 whop-api-wrapper-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 08:20:49.637232 whop-api-wrapper-1.0.3/whop_api_wrapper.egg-info/
--rw-rw-rw-   0        0        0     2064 2023-07-17 08:20:49.000000 whop-api-wrapper-1.0.3/whop_api_wrapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-07-17 08:20:49.000000 whop-api-wrapper-1.0.3/whop_api_wrapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 08:20:49.000000 whop-api-wrapper-1.0.3/whop_api_wrapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-17 08:20:49.000000 whop-api-wrapper-1.0.3/whop_api_wrapper.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 08:20:49.000000 whop-api-wrapper-1.0.3/whop_api_wrapper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 08:26:16.046806 whop-api-wrapper-1.0.4/
+-rw-rw-rw-   0        0        0     1089 2023-07-17 07:39:09.000000 whop-api-wrapper-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     2064 2023-07-17 08:26:16.046806 whop-api-wrapper-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1306 2023-07-17 08:12:50.000000 whop-api-wrapper-1.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-17 08:26:16.046806 whop-api-wrapper-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1018 2023-07-17 08:26:13.000000 whop-api-wrapper-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 08:26:16.046806 whop-api-wrapper-1.0.4/whop_api_wrapper.egg-info/
+-rw-rw-rw-   0        0        0     2064 2023-07-17 08:26:15.000000 whop-api-wrapper-1.0.4/whop_api_wrapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2023-07-17 08:26:16.000000 whop-api-wrapper-1.0.4/whop_api_wrapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 08:26:15.000000 whop-api-wrapper-1.0.4/whop_api_wrapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-17 08:26:15.000000 whop-api-wrapper-1.0.4/whop_api_wrapper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 08:26:15.000000 whop-api-wrapper-1.0.4/whop_api_wrapper.egg-info/top_level.txt
```

### Comparing `whop-api-wrapper-1.0.3/LICENSE` & `whop-api-wrapper-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `whop-api-wrapper-1.0.3/PKG-INFO` & `whop-api-wrapper-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whop-api-wrapper
-Version: 1.0.3
+Version: 1.0.4
 Summary: Simple Python Whop API Wrapper
 Home-page: https://github.com/TheSweeet/Whop-API-Wrapper
 Author: Jacobfinn123
 Author-email: jacobfinn@bezosproxy.com
 Keywords: WHOP,API,WRAPPER
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `whop-api-wrapper-1.0.3/README.md` & `whop-api-wrapper-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `whop-api-wrapper-1.0.3/setup.py` & `whop-api-wrapper-1.0.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='whop-api-wrapper',
-    version='1.0.3',
+    version='1.0.4',
     author='Jacobfinn123',
     author_email='jacobfinn@bezosproxy.com',
     description='Simple Python Whop API Wrapper',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/TheSweeet/Whop-API-Wrapper',
     packages=find_packages(),
```

### Comparing `whop-api-wrapper-1.0.3/whop_api_wrapper.egg-info/PKG-INFO` & `whop-api-wrapper-1.0.4/whop_api_wrapper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whop-api-wrapper
-Version: 1.0.3
+Version: 1.0.4
 Summary: Simple Python Whop API Wrapper
 Home-page: https://github.com/TheSweeet/Whop-API-Wrapper
 Author: Jacobfinn123
 Author-email: jacobfinn@bezosproxy.com
 Keywords: WHOP,API,WRAPPER
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

