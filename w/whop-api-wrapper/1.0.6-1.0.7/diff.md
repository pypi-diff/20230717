# Comparing `tmp/whop-api-wrapper-1.0.6.tar.gz` & `tmp/whop-api-wrapper-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whop-api-wrapper-1.0.6.tar", last modified: Mon Jul 17 08:48:34 2023, max compression
+gzip compressed data, was "whop-api-wrapper-1.0.7.tar", last modified: Mon Jul 17 20:12:31 2023, max compression
```

## Comparing `whop-api-wrapper-1.0.6.tar` & `whop-api-wrapper-1.0.7.tar`

### file list

```diff
@@ -1,13 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 08:48:34.028076 whop-api-wrapper-1.0.6/
--rw-rw-rw-   0        0        0     1089 2023-07-17 07:39:09.000000 whop-api-wrapper-1.0.6/LICENSE
--rw-rw-rw-   0        0        0     2064 2023-07-17 08:48:34.028076 whop-api-wrapper-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1306 2023-07-17 08:12:50.000000 whop-api-wrapper-1.0.6/README.md
--rw-rw-rw-   0        0        0      102 2023-07-17 08:41:19.000000 whop-api-wrapper-1.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-17 08:48:34.028076 whop-api-wrapper-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1020 2023-07-17 08:48:32.000000 whop-api-wrapper-1.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 08:48:34.027079 whop-api-wrapper-1.0.6/whop_api_wrapper.egg-info/
--rw-rw-rw-   0        0        0     2064 2023-07-17 08:48:33.000000 whop-api-wrapper-1.0.6/whop_api_wrapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2023-07-17 08:48:33.000000 whop-api-wrapper-1.0.6/whop_api_wrapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 08:48:33.000000 whop-api-wrapper-1.0.6/whop_api_wrapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-17 08:48:33.000000 whop-api-wrapper-1.0.6/whop_api_wrapper.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 08:48:33.000000 whop-api-wrapper-1.0.6/whop_api_wrapper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 20:12:31.495284 whop-api-wrapper-1.0.7/
+-rw-rw-rw-   0        0        0     1089 2023-07-17 07:39:09.000000 whop-api-wrapper-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0     2064 2023-07-17 20:12:31.494285 whop-api-wrapper-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1306 2023-07-17 08:12:50.000000 whop-api-wrapper-1.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-17 20:12:31.495284 whop-api-wrapper-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1020 2023-07-17 20:12:29.000000 whop-api-wrapper-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 20:12:31.485810 whop-api-wrapper-1.0.7/whop-api-wrapper/
+-rw-rw-rw-   0        0        0    15949 2023-07-17 08:34:16.000000 whop-api-wrapper-1.0.7/whop-api-wrapper/Client.py
+-rw-rw-rw-   0        0        0      251 2023-07-16 05:41:49.000000 whop-api-wrapper-1.0.7/whop-api-wrapper/Endpoints.py
+-rw-rw-rw-   0        0        0     5957 2023-07-17 07:34:42.000000 whop-api-wrapper-1.0.7/whop-api-wrapper/Objects.py
+-rw-rw-rw-   0        0        0      148 2023-07-17 20:11:49.000000 whop-api-wrapper-1.0.7/whop-api-wrapper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 20:12:31.494285 whop-api-wrapper-1.0.7/whop_api_wrapper.egg-info/
+-rw-rw-rw-   0        0        0     2064 2023-07-17 20:12:31.000000 whop-api-wrapper-1.0.7/whop_api_wrapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      339 2023-07-17 20:12:31.000000 whop-api-wrapper-1.0.7/whop_api_wrapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 20:12:31.000000 whop-api-wrapper-1.0.7/whop_api_wrapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-17 20:12:31.000000 whop-api-wrapper-1.0.7/whop_api_wrapper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-17 20:12:31.000000 whop-api-wrapper-1.0.7/whop_api_wrapper.egg-info/top_level.txt
```

### Comparing `whop-api-wrapper-1.0.6/LICENSE` & `whop-api-wrapper-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `whop-api-wrapper-1.0.6/PKG-INFO` & `whop-api-wrapper-1.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whop-api-wrapper
-Version: 1.0.6
+Version: 1.0.7
 Summary: Simple Python Whop API Wrapper
 Home-page: https://github.com/TheSweeet/Whop-API-Wrapper
 Author: Jacobfinn123
 Author-email: jacobfinn@bezosproxy.com
 Keywords: WHOP,API,WRAPPER
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `whop-api-wrapper-1.0.6/README.md` & `whop-api-wrapper-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `whop-api-wrapper-1.0.6/setup.py` & `whop-api-wrapper-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='whop-api-wrapper',
-    version='1.0.6',
+    version='1.0.7',
     author='Jacobfinn123',
     author_email='jacobfinn@bezosproxy.com',
     description='Simple Python Whop API Wrapper',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/TheSweeet/Whop-API-Wrapper',
     packages=find_packages(),
```

### Comparing `whop-api-wrapper-1.0.6/whop_api_wrapper.egg-info/PKG-INFO` & `whop-api-wrapper-1.0.7/whop_api_wrapper.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whop-api-wrapper
-Version: 1.0.6
+Version: 1.0.7
 Summary: Simple Python Whop API Wrapper
 Home-page: https://github.com/TheSweeet/Whop-API-Wrapper
 Author: Jacobfinn123
 Author-email: jacobfinn@bezosproxy.com
 Keywords: WHOP,API,WRAPPER
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

