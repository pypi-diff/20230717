# Comparing `tmp/whop_api_wrapper-1.0.8.tar.gz` & `tmp/whop_api_wrapper-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whop_api_wrapper-1.0.8.tar", last modified: Mon Jul 17 20:19:18 2023, max compression
+gzip compressed data, was "whop_api_wrapper-1.0.9.tar", last modified: Mon Jul 17 20:22:29 2023, max compression
```

## Comparing `whop_api_wrapper-1.0.8.tar` & `whop_api_wrapper-1.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 20:19:18.420085 whop_api_wrapper-1.0.8/
--rw-rw-rw-   0        0        0     1089 2023-07-17 07:39:09.000000 whop_api_wrapper-1.0.8/LICENSE
--rw-rw-rw-   0        0        0     2064 2023-07-17 20:19:18.420085 whop_api_wrapper-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1306 2023-07-17 08:12:50.000000 whop_api_wrapper-1.0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-07-17 20:19:18.420085 whop_api_wrapper-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1020 2023-07-17 20:19:12.000000 whop_api_wrapper-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 20:19:18.407366 whop_api_wrapper-1.0.8/whop-api-wrapper/
--rw-rw-rw-   0        0        0    15949 2023-07-17 08:34:16.000000 whop_api_wrapper-1.0.8/whop-api-wrapper/Client.py
--rw-rw-rw-   0        0        0      251 2023-07-16 05:41:49.000000 whop_api_wrapper-1.0.8/whop-api-wrapper/Endpoints.py
--rw-rw-rw-   0        0        0     5957 2023-07-17 07:34:42.000000 whop_api_wrapper-1.0.8/whop-api-wrapper/Objects.py
--rw-rw-rw-   0        0        0      148 2023-07-17 20:11:49.000000 whop_api_wrapper-1.0.8/whop-api-wrapper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 20:19:18.419088 whop_api_wrapper-1.0.8/whop_api_wrapper.egg-info/
--rw-rw-rw-   0        0        0     2064 2023-07-17 20:19:18.000000 whop_api_wrapper-1.0.8/whop_api_wrapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      339 2023-07-17 20:19:18.000000 whop_api_wrapper-1.0.8/whop_api_wrapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 20:19:18.000000 whop_api_wrapper-1.0.8/whop_api_wrapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-17 20:19:18.000000 whop_api_wrapper-1.0.8/whop_api_wrapper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-17 20:19:18.000000 whop_api_wrapper-1.0.8/whop_api_wrapper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 20:22:29.384718 whop_api_wrapper-1.0.9/
+-rw-rw-rw-   0        0        0     1089 2023-07-17 07:39:09.000000 whop_api_wrapper-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0     2064 2023-07-17 20:22:29.384718 whop_api_wrapper-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1306 2023-07-17 20:22:21.000000 whop_api_wrapper-1.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-17 20:22:29.385716 whop_api_wrapper-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1020 2023-07-17 20:22:26.000000 whop_api_wrapper-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 20:22:29.368491 whop_api_wrapper-1.0.9/whop_api_wrapper/
+-rw-rw-rw-   0        0        0    15949 2023-07-17 08:34:16.000000 whop_api_wrapper-1.0.9/whop_api_wrapper/Client.py
+-rw-rw-rw-   0        0        0      251 2023-07-16 05:41:49.000000 whop_api_wrapper-1.0.9/whop_api_wrapper/Endpoints.py
+-rw-rw-rw-   0        0        0     5957 2023-07-17 07:34:42.000000 whop_api_wrapper-1.0.9/whop_api_wrapper/Objects.py
+-rw-rw-rw-   0        0        0      148 2023-07-17 20:11:49.000000 whop_api_wrapper-1.0.9/whop_api_wrapper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 20:22:29.384718 whop_api_wrapper-1.0.9/whop_api_wrapper.egg-info/
+-rw-rw-rw-   0        0        0     2064 2023-07-17 20:22:29.000000 whop_api_wrapper-1.0.9/whop_api_wrapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      339 2023-07-17 20:22:29.000000 whop_api_wrapper-1.0.9/whop_api_wrapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 20:22:29.000000 whop_api_wrapper-1.0.9/whop_api_wrapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-17 20:22:29.000000 whop_api_wrapper-1.0.9/whop_api_wrapper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-17 20:22:29.000000 whop_api_wrapper-1.0.9/whop_api_wrapper.egg-info/top_level.txt
```

### Comparing `whop_api_wrapper-1.0.8/LICENSE` & `whop_api_wrapper-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `whop_api_wrapper-1.0.8/PKG-INFO` & `whop_api_wrapper-1.0.9/whop_api_wrapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: whop_api_wrapper
-Version: 1.0.8
+Name: whop-api-wrapper
+Version: 1.0.9
 Summary: Simple Python Whop API Wrapper
 Home-page: https://github.com/TheSweeet/Whop-API-Wrapper
 Author: Jacobfinn123
 Author-email: jacobfinn@bezosproxy.com
 Keywords: WHOP,API,WRAPPER
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -22,15 +22,15 @@
 A simple python API wrapper of Whop's API, documentation can be found at: https://dev.whop.com/reference/home
 
 ## Installation
 
 To install the package, use the following command:
 
 ```shell
-pip install whop-api-wrapper
+pip install whop_api_wrapper
 ```
 
 ## Usage
 Initialize the Client class with your token, use any api call as a method of the client.
 
 ```py
 from Resources.Client import Client
```

### Comparing `whop_api_wrapper-1.0.8/README.md` & `whop_api_wrapper-1.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 A simple python API wrapper of Whop's API, documentation can be found at: https://dev.whop.com/reference/home
 
 ## Installation
 
 To install the package, use the following command:
 
 ```shell
-pip install whop-api-wrapper
+pip install whop_api_wrapper
 ```
 
 ## Usage
 Initialize the Client class with your token, use any api call as a method of the client.
 
 ```py
 from Resources.Client import Client
```

### Comparing `whop_api_wrapper-1.0.8/setup.py` & `whop_api_wrapper-1.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='whop_api_wrapper',
-    version='1.0.8',
+    version='1.0.9',
     author='Jacobfinn123',
     author_email='jacobfinn@bezosproxy.com',
     description='Simple Python Whop API Wrapper',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/TheSweeet/Whop-API-Wrapper',
     packages=find_packages(),
```

### Comparing `whop_api_wrapper-1.0.8/whop-api-wrapper/Client.py` & `whop_api_wrapper-1.0.9/whop_api_wrapper/Client.py`

 * *Files identical despite different names*

### Comparing `whop_api_wrapper-1.0.8/whop-api-wrapper/Objects.py` & `whop_api_wrapper-1.0.9/whop_api_wrapper/Objects.py`

 * *Files identical despite different names*

### Comparing `whop_api_wrapper-1.0.8/whop_api_wrapper.egg-info/PKG-INFO` & `whop_api_wrapper-1.0.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: whop-api-wrapper
-Version: 1.0.8
+Name: whop_api_wrapper
+Version: 1.0.9
 Summary: Simple Python Whop API Wrapper
 Home-page: https://github.com/TheSweeet/Whop-API-Wrapper
 Author: Jacobfinn123
 Author-email: jacobfinn@bezosproxy.com
 Keywords: WHOP,API,WRAPPER
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -22,15 +22,15 @@
 A simple python API wrapper of Whop's API, documentation can be found at: https://dev.whop.com/reference/home
 
 ## Installation
 
 To install the package, use the following command:
 
 ```shell
-pip install whop-api-wrapper
+pip install whop_api_wrapper
 ```
 
 ## Usage
 Initialize the Client class with your token, use any api call as a method of the client.
 
 ```py
 from Resources.Client import Client
```

