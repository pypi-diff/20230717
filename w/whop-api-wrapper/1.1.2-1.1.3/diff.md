# Comparing `tmp/whop-api-wrapper-1.1.2.tar.gz` & `tmp/whop-api-wrapper-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whop-api-wrapper-1.1.2.tar", last modified: Mon Jul 17 20:25:25 2023, max compression
+gzip compressed data, was "whop-api-wrapper-1.1.3.tar", last modified: Mon Jul 17 21:03:35 2023, max compression
```

## Comparing `whop-api-wrapper-1.1.2.tar` & `whop-api-wrapper-1.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 20:25:25.979550 whop-api-wrapper-1.1.2/
--rw-rw-rw-   0        0        0     1089 2023-07-17 07:39:09.000000 whop-api-wrapper-1.1.2/LICENSE
--rw-rw-rw-   0        0        0     2064 2023-07-17 20:25:25.979550 whop-api-wrapper-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1306 2023-07-17 20:25:24.000000 whop-api-wrapper-1.1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-17 20:25:25.979550 whop-api-wrapper-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1020 2023-07-17 20:25:24.000000 whop-api-wrapper-1.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 20:25:25.967216 whop-api-wrapper-1.1.2/whop_api_wrapper/
--rw-rw-rw-   0        0        0    15949 2023-07-17 08:34:16.000000 whop-api-wrapper-1.1.2/whop_api_wrapper/Client.py
--rw-rw-rw-   0        0        0      251 2023-07-16 05:41:49.000000 whop-api-wrapper-1.1.2/whop_api_wrapper/Endpoints.py
--rw-rw-rw-   0        0        0     5957 2023-07-17 07:34:42.000000 whop-api-wrapper-1.1.2/whop_api_wrapper/Objects.py
--rw-rw-rw-   0        0        0      148 2023-07-17 20:11:49.000000 whop-api-wrapper-1.1.2/whop_api_wrapper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 20:25:25.978552 whop-api-wrapper-1.1.2/whop_api_wrapper.egg-info/
--rw-rw-rw-   0        0        0     2064 2023-07-17 20:25:25.000000 whop-api-wrapper-1.1.2/whop_api_wrapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      339 2023-07-17 20:25:25.000000 whop-api-wrapper-1.1.2/whop_api_wrapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 20:25:25.000000 whop-api-wrapper-1.1.2/whop_api_wrapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-17 20:25:25.000000 whop-api-wrapper-1.1.2/whop_api_wrapper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-17 20:25:25.000000 whop-api-wrapper-1.1.2/whop_api_wrapper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 21:03:35.842508 whop-api-wrapper-1.1.3/
+-rw-rw-rw-   0        0        0     1089 2023-07-17 07:39:09.000000 whop-api-wrapper-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0     2064 2023-07-17 21:03:35.842508 whop-api-wrapper-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1306 2023-07-17 20:25:24.000000 whop-api-wrapper-1.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-17 21:03:35.842508 whop-api-wrapper-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1020 2023-07-17 21:03:33.000000 whop-api-wrapper-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 21:03:35.833021 whop-api-wrapper-1.1.3/whop_api_wrapper/
+-rw-rw-rw-   0        0        0    15949 2023-07-17 21:02:55.000000 whop-api-wrapper-1.1.3/whop_api_wrapper/Client.py
+-rw-rw-rw-   0        0        0      251 2023-07-17 21:02:55.000000 whop-api-wrapper-1.1.3/whop_api_wrapper/Endpoints.py
+-rw-rw-rw-   0        0        0     5957 2023-07-17 21:02:55.000000 whop-api-wrapper-1.1.3/whop_api_wrapper/Objects.py
+-rw-rw-rw-   0        0        0        0 2023-07-17 21:03:04.000000 whop-api-wrapper-1.1.3/whop_api_wrapper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 21:03:35.841500 whop-api-wrapper-1.1.3/whop_api_wrapper.egg-info/
+-rw-rw-rw-   0        0        0     2064 2023-07-17 21:03:35.000000 whop-api-wrapper-1.1.3/whop_api_wrapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      339 2023-07-17 21:03:35.000000 whop-api-wrapper-1.1.3/whop_api_wrapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 21:03:35.000000 whop-api-wrapper-1.1.3/whop_api_wrapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-17 21:03:35.000000 whop-api-wrapper-1.1.3/whop_api_wrapper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-17 21:03:35.000000 whop-api-wrapper-1.1.3/whop_api_wrapper.egg-info/top_level.txt
```

### Comparing `whop-api-wrapper-1.1.2/LICENSE` & `whop-api-wrapper-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `whop-api-wrapper-1.1.2/PKG-INFO` & `whop-api-wrapper-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whop-api-wrapper
-Version: 1.1.2
+Version: 1.1.3
 Summary: Simple Python Whop API Wrapper
 Home-page: https://github.com/TheSweeet/Whop-API-Wrapper
 Author: Jacobfinn123
 Author-email: jacobfinn@bezosproxy.com
 Keywords: WHOP,API,WRAPPER
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `whop-api-wrapper-1.1.2/README.md` & `whop-api-wrapper-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `whop-api-wrapper-1.1.2/setup.py` & `whop-api-wrapper-1.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='whop-api-wrapper',
-    version='1.1.2',
+    version='1.1.3',
     author='Jacobfinn123',
     author_email='jacobfinn@bezosproxy.com',
     description='Simple Python Whop API Wrapper',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/TheSweeet/Whop-API-Wrapper',
     packages=find_packages(),
```

### Comparing `whop-api-wrapper-1.1.2/whop_api_wrapper/Client.py` & `whop-api-wrapper-1.1.3/whop_api_wrapper/Client.py`

 * *Files identical despite different names*

### Comparing `whop-api-wrapper-1.1.2/whop_api_wrapper/Objects.py` & `whop-api-wrapper-1.1.3/whop_api_wrapper/Objects.py`

 * *Files identical despite different names*

### Comparing `whop-api-wrapper-1.1.2/whop_api_wrapper.egg-info/PKG-INFO` & `whop-api-wrapper-1.1.3/whop_api_wrapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whop-api-wrapper
-Version: 1.1.2
+Version: 1.1.3
 Summary: Simple Python Whop API Wrapper
 Home-page: https://github.com/TheSweeet/Whop-API-Wrapper
 Author: Jacobfinn123
 Author-email: jacobfinn@bezosproxy.com
 Keywords: WHOP,API,WRAPPER
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

