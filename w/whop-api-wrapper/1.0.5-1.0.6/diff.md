# Comparing `tmp/whop-api-wrapper-1.0.5.tar.gz` & `tmp/whop-api-wrapper-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whop-api-wrapper-1.0.5.tar", last modified: Mon Jul 17 08:35:22 2023, max compression
+gzip compressed data, was "whop-api-wrapper-1.0.6.tar", last modified: Mon Jul 17 08:48:34 2023, max compression
```

## Comparing `whop-api-wrapper-1.0.5.tar` & `whop-api-wrapper-1.0.6.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 08:35:22.138545 whop-api-wrapper-1.0.5/
--rw-rw-rw-   0        0        0     1089 2023-07-17 07:39:09.000000 whop-api-wrapper-1.0.5/LICENSE
--rw-rw-rw-   0        0        0     2064 2023-07-17 08:35:22.138545 whop-api-wrapper-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1306 2023-07-17 08:12:50.000000 whop-api-wrapper-1.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-07-17 08:35:22.138545 whop-api-wrapper-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1020 2023-07-17 08:35:16.000000 whop-api-wrapper-1.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 08:35:22.137548 whop-api-wrapper-1.0.5/whop_api_wrapper.egg-info/
--rw-rw-rw-   0        0        0     2064 2023-07-17 08:35:22.000000 whop-api-wrapper-1.0.5/whop_api_wrapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-07-17 08:35:22.000000 whop-api-wrapper-1.0.5/whop_api_wrapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 08:35:22.000000 whop-api-wrapper-1.0.5/whop_api_wrapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-17 08:35:22.000000 whop-api-wrapper-1.0.5/whop_api_wrapper.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 08:35:22.000000 whop-api-wrapper-1.0.5/whop_api_wrapper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 08:48:34.028076 whop-api-wrapper-1.0.6/
+-rw-rw-rw-   0        0        0     1089 2023-07-17 07:39:09.000000 whop-api-wrapper-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0     2064 2023-07-17 08:48:34.028076 whop-api-wrapper-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1306 2023-07-17 08:12:50.000000 whop-api-wrapper-1.0.6/README.md
+-rw-rw-rw-   0        0        0      102 2023-07-17 08:41:19.000000 whop-api-wrapper-1.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-17 08:48:34.028076 whop-api-wrapper-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1020 2023-07-17 08:48:32.000000 whop-api-wrapper-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 08:48:34.027079 whop-api-wrapper-1.0.6/whop_api_wrapper.egg-info/
+-rw-rw-rw-   0        0        0     2064 2023-07-17 08:48:33.000000 whop-api-wrapper-1.0.6/whop_api_wrapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2023-07-17 08:48:33.000000 whop-api-wrapper-1.0.6/whop_api_wrapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 08:48:33.000000 whop-api-wrapper-1.0.6/whop_api_wrapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-17 08:48:33.000000 whop-api-wrapper-1.0.6/whop_api_wrapper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 08:48:33.000000 whop-api-wrapper-1.0.6/whop_api_wrapper.egg-info/top_level.txt
```

### Comparing `whop-api-wrapper-1.0.5/LICENSE` & `whop-api-wrapper-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `whop-api-wrapper-1.0.5/PKG-INFO` & `whop-api-wrapper-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whop-api-wrapper
-Version: 1.0.5
+Version: 1.0.6
 Summary: Simple Python Whop API Wrapper
 Home-page: https://github.com/TheSweeet/Whop-API-Wrapper
 Author: Jacobfinn123
 Author-email: jacobfinn@bezosproxy.com
 Keywords: WHOP,API,WRAPPER
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `whop-api-wrapper-1.0.5/README.md` & `whop-api-wrapper-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `whop-api-wrapper-1.0.5/setup.py` & `whop-api-wrapper-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='whop-api-wrapper',
-    version='1.0.5',
+    version='1.0.6',
     author='Jacobfinn123',
     author_email='jacobfinn@bezosproxy.com',
     description='Simple Python Whop API Wrapper',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/TheSweeet/Whop-API-Wrapper',
     packages=find_packages(),
```

### Comparing `whop-api-wrapper-1.0.5/whop_api_wrapper.egg-info/PKG-INFO` & `whop-api-wrapper-1.0.6/whop_api_wrapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whop-api-wrapper
-Version: 1.0.5
+Version: 1.0.6
 Summary: Simple Python Whop API Wrapper
 Home-page: https://github.com/TheSweeet/Whop-API-Wrapper
 Author: Jacobfinn123
 Author-email: jacobfinn@bezosproxy.com
 Keywords: WHOP,API,WRAPPER
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

