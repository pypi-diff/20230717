# Comparing `tmp/whop-api-wrapper-1.1.1.tar.gz` & `tmp/whop-api-wrapper-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whop-api-wrapper-1.1.1.tar", last modified: Mon Jul 17 20:24:46 2023, max compression
+gzip compressed data, was "whop-api-wrapper-1.1.2.tar", last modified: Mon Jul 17 20:25:25 2023, max compression
```

## Comparing `whop-api-wrapper-1.1.1.tar` & `whop-api-wrapper-1.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 20:24:46.084593 whop-api-wrapper-1.1.1/
--rw-rw-rw-   0        0        0     1089 2023-07-17 07:39:09.000000 whop-api-wrapper-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     2064 2023-07-17 20:24:46.083346 whop-api-wrapper-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1306 2023-07-17 20:23:12.000000 whop-api-wrapper-1.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-17 20:24:46.084593 whop-api-wrapper-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1020 2023-07-17 20:24:38.000000 whop-api-wrapper-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 20:24:46.076861 whop-api-wrapper-1.1.1/whop_api_wrapper/
--rw-rw-rw-   0        0        0    15949 2023-07-17 08:34:16.000000 whop-api-wrapper-1.1.1/whop_api_wrapper/Client.py
--rw-rw-rw-   0        0        0      251 2023-07-16 05:41:49.000000 whop-api-wrapper-1.1.1/whop_api_wrapper/Endpoints.py
--rw-rw-rw-   0        0        0     5957 2023-07-17 07:34:42.000000 whop-api-wrapper-1.1.1/whop_api_wrapper/Objects.py
--rw-rw-rw-   0        0        0      148 2023-07-17 20:11:49.000000 whop-api-wrapper-1.1.1/whop_api_wrapper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 20:24:46.083346 whop-api-wrapper-1.1.1/whop_api_wrapper.egg-info/
--rw-rw-rw-   0        0        0     2064 2023-07-17 20:24:46.000000 whop-api-wrapper-1.1.1/whop_api_wrapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      339 2023-07-17 20:24:46.000000 whop-api-wrapper-1.1.1/whop_api_wrapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 20:24:46.000000 whop-api-wrapper-1.1.1/whop_api_wrapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-17 20:24:46.000000 whop-api-wrapper-1.1.1/whop_api_wrapper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-17 20:24:46.000000 whop-api-wrapper-1.1.1/whop_api_wrapper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 20:25:25.979550 whop-api-wrapper-1.1.2/
+-rw-rw-rw-   0        0        0     1089 2023-07-17 07:39:09.000000 whop-api-wrapper-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0     2064 2023-07-17 20:25:25.979550 whop-api-wrapper-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1306 2023-07-17 20:25:24.000000 whop-api-wrapper-1.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-17 20:25:25.979550 whop-api-wrapper-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1020 2023-07-17 20:25:24.000000 whop-api-wrapper-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 20:25:25.967216 whop-api-wrapper-1.1.2/whop_api_wrapper/
+-rw-rw-rw-   0        0        0    15949 2023-07-17 08:34:16.000000 whop-api-wrapper-1.1.2/whop_api_wrapper/Client.py
+-rw-rw-rw-   0        0        0      251 2023-07-16 05:41:49.000000 whop-api-wrapper-1.1.2/whop_api_wrapper/Endpoints.py
+-rw-rw-rw-   0        0        0     5957 2023-07-17 07:34:42.000000 whop-api-wrapper-1.1.2/whop_api_wrapper/Objects.py
+-rw-rw-rw-   0        0        0      148 2023-07-17 20:11:49.000000 whop-api-wrapper-1.1.2/whop_api_wrapper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 20:25:25.978552 whop-api-wrapper-1.1.2/whop_api_wrapper.egg-info/
+-rw-rw-rw-   0        0        0     2064 2023-07-17 20:25:25.000000 whop-api-wrapper-1.1.2/whop_api_wrapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      339 2023-07-17 20:25:25.000000 whop-api-wrapper-1.1.2/whop_api_wrapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 20:25:25.000000 whop-api-wrapper-1.1.2/whop_api_wrapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-17 20:25:25.000000 whop-api-wrapper-1.1.2/whop_api_wrapper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-17 20:25:25.000000 whop-api-wrapper-1.1.2/whop_api_wrapper.egg-info/top_level.txt
```

### Comparing `whop-api-wrapper-1.1.1/LICENSE` & `whop-api-wrapper-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `whop-api-wrapper-1.1.1/PKG-INFO` & `whop-api-wrapper-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whop-api-wrapper
-Version: 1.1.1
+Version: 1.1.2
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
-pip install whop_api_wrapper
+pip install whop-api-wrapper
 ```
 
 ## Usage
 Initialize the Client class with your token, use any api call as a method of the client.
 
 ```py
 from whop_api_wrapper import Client
```

### Comparing `whop-api-wrapper-1.1.1/README.md` & `whop-api-wrapper-1.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 A simple python API wrapper of Whop's API, documentation can be found at: https://dev.whop.com/reference/home
 
 ## Installation
 
 To install the package, use the following command:
 
 ```shell
-pip install whop_api_wrapper
+pip install whop-api-wrapper
 ```
 
 ## Usage
 Initialize the Client class with your token, use any api call as a method of the client.
 
 ```py
 from whop_api_wrapper import Client
```

### Comparing `whop-api-wrapper-1.1.1/setup.py` & `whop-api-wrapper-1.1.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='whop-api-wrapper',
-    version='1.1.1',
+    version='1.1.2',
     author='Jacobfinn123',
     author_email='jacobfinn@bezosproxy.com',
     description='Simple Python Whop API Wrapper',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/TheSweeet/Whop-API-Wrapper',
     packages=find_packages(),
```

### Comparing `whop-api-wrapper-1.1.1/whop_api_wrapper/Client.py` & `whop-api-wrapper-1.1.2/whop_api_wrapper/Client.py`

 * *Files identical despite different names*

### Comparing `whop-api-wrapper-1.1.1/whop_api_wrapper/Objects.py` & `whop-api-wrapper-1.1.2/whop_api_wrapper/Objects.py`

 * *Files identical despite different names*

### Comparing `whop-api-wrapper-1.1.1/whop_api_wrapper.egg-info/PKG-INFO` & `whop-api-wrapper-1.1.2/whop_api_wrapper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whop-api-wrapper
-Version: 1.1.1
+Version: 1.1.2
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
-pip install whop_api_wrapper
+pip install whop-api-wrapper
 ```
 
 ## Usage
 Initialize the Client class with your token, use any api call as a method of the client.
 
 ```py
 from whop_api_wrapper import Client
```

