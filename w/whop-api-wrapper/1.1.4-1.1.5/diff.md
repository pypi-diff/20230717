# Comparing `tmp/whop-api-wrapper-1.1.4.tar.gz` & `tmp/whop-api-wrapper-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whop-api-wrapper-1.1.4.tar", last modified: Mon Jul 17 21:09:12 2023, max compression
+gzip compressed data, was "whop-api-wrapper-1.1.5.tar", last modified: Mon Jul 17 21:10:02 2023, max compression
```

## Comparing `whop-api-wrapper-1.1.4.tar` & `whop-api-wrapper-1.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 21:09:12.827865 whop-api-wrapper-1.1.4/
--rw-rw-rw-   0        0        0     1089 2023-07-17 07:39:09.000000 whop-api-wrapper-1.1.4/LICENSE
--rw-rw-rw-   0        0        0     2064 2023-07-17 21:09:12.827865 whop-api-wrapper-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1306 2023-07-17 20:25:24.000000 whop-api-wrapper-1.1.4/README.md
--rw-rw-rw-   0        0        0       42 2023-07-17 21:09:12.827865 whop-api-wrapper-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1020 2023-07-17 21:08:38.000000 whop-api-wrapper-1.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 21:09:12.823879 whop-api-wrapper-1.1.4/whop_api_wrapper/
--rw-rw-rw-   0        0        0    15951 2023-07-17 21:08:38.000000 whop-api-wrapper-1.1.4/whop_api_wrapper/Client.py
--rw-rw-rw-   0        0        0      251 2023-07-17 21:02:55.000000 whop-api-wrapper-1.1.4/whop_api_wrapper/Endpoints.py
--rw-rw-rw-   0        0        0     5957 2023-07-17 21:02:55.000000 whop-api-wrapper-1.1.4/whop_api_wrapper/Objects.py
--rw-rw-rw-   0        0        0      308 2023-07-17 21:06:17.000000 whop-api-wrapper-1.1.4/whop_api_wrapper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 21:09:12.826869 whop-api-wrapper-1.1.4/whop_api_wrapper.egg-info/
--rw-rw-rw-   0        0        0     2064 2023-07-17 21:09:12.000000 whop-api-wrapper-1.1.4/whop_api_wrapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      339 2023-07-17 21:09:12.000000 whop-api-wrapper-1.1.4/whop_api_wrapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 21:09:12.000000 whop-api-wrapper-1.1.4/whop_api_wrapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-17 21:09:12.000000 whop-api-wrapper-1.1.4/whop_api_wrapper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-17 21:09:12.000000 whop-api-wrapper-1.1.4/whop_api_wrapper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 21:10:02.728153 whop-api-wrapper-1.1.5/
+-rw-rw-rw-   0        0        0     1089 2023-07-17 07:39:09.000000 whop-api-wrapper-1.1.5/LICENSE
+-rw-rw-rw-   0        0        0     2064 2023-07-17 21:10:02.727156 whop-api-wrapper-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1306 2023-07-17 20:25:24.000000 whop-api-wrapper-1.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-17 21:10:02.728153 whop-api-wrapper-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1020 2023-07-17 21:09:51.000000 whop-api-wrapper-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 21:10:02.724166 whop-api-wrapper-1.1.5/whop_api_wrapper/
+-rw-rw-rw-   0        0        0    15951 2023-07-17 21:08:38.000000 whop-api-wrapper-1.1.5/whop_api_wrapper/Client.py
+-rw-rw-rw-   0        0        0      251 2023-07-17 21:02:55.000000 whop-api-wrapper-1.1.5/whop_api_wrapper/Endpoints.py
+-rw-rw-rw-   0        0        0     5957 2023-07-17 21:02:55.000000 whop-api-wrapper-1.1.5/whop_api_wrapper/Objects.py
+-rw-rw-rw-   0        0        0        0 2023-07-17 21:09:46.000000 whop-api-wrapper-1.1.5/whop_api_wrapper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 21:10:02.727156 whop-api-wrapper-1.1.5/whop_api_wrapper.egg-info/
+-rw-rw-rw-   0        0        0     2064 2023-07-17 21:10:02.000000 whop-api-wrapper-1.1.5/whop_api_wrapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      339 2023-07-17 21:10:02.000000 whop-api-wrapper-1.1.5/whop_api_wrapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 21:10:02.000000 whop-api-wrapper-1.1.5/whop_api_wrapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-17 21:10:02.000000 whop-api-wrapper-1.1.5/whop_api_wrapper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-17 21:10:02.000000 whop-api-wrapper-1.1.5/whop_api_wrapper.egg-info/top_level.txt
```

### Comparing `whop-api-wrapper-1.1.4/LICENSE` & `whop-api-wrapper-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `whop-api-wrapper-1.1.4/PKG-INFO` & `whop-api-wrapper-1.1.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whop-api-wrapper
-Version: 1.1.4
+Version: 1.1.5
 Summary: Simple Python Whop API Wrapper
 Home-page: https://github.com/TheSweeet/Whop-API-Wrapper
 Author: Jacobfinn123
 Author-email: jacobfinn@bezosproxy.com
 Keywords: WHOP,API,WRAPPER
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `whop-api-wrapper-1.1.4/README.md` & `whop-api-wrapper-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `whop-api-wrapper-1.1.4/setup.py` & `whop-api-wrapper-1.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='whop-api-wrapper',
-    version='1.1.4',
+    version='1.1.5',
     author='Jacobfinn123',
     author_email='jacobfinn@bezosproxy.com',
     description='Simple Python Whop API Wrapper',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/TheSweeet/Whop-API-Wrapper',
     packages=find_packages(),
```

### Comparing `whop-api-wrapper-1.1.4/whop_api_wrapper/Client.py` & `whop-api-wrapper-1.1.5/whop_api_wrapper/Client.py`

 * *Files identical despite different names*

### Comparing `whop-api-wrapper-1.1.4/whop_api_wrapper/Objects.py` & `whop-api-wrapper-1.1.5/whop_api_wrapper/Objects.py`

 * *Files identical despite different names*

### Comparing `whop-api-wrapper-1.1.4/whop_api_wrapper.egg-info/PKG-INFO` & `whop-api-wrapper-1.1.5/whop_api_wrapper.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whop-api-wrapper
-Version: 1.1.4
+Version: 1.1.5
 Summary: Simple Python Whop API Wrapper
 Home-page: https://github.com/TheSweeet/Whop-API-Wrapper
 Author: Jacobfinn123
 Author-email: jacobfinn@bezosproxy.com
 Keywords: WHOP,API,WRAPPER
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

