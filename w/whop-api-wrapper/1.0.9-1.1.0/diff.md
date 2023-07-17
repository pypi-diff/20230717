# Comparing `tmp/whop_api_wrapper-1.0.9.tar.gz` & `tmp/whop_api_wrapper-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whop_api_wrapper-1.0.9.tar", last modified: Mon Jul 17 20:22:29 2023, max compression
+gzip compressed data, was "whop_api_wrapper-1.1.0.tar", last modified: Mon Jul 17 20:23:51 2023, max compression
```

## Comparing `whop_api_wrapper-1.0.9.tar` & `whop_api_wrapper-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 20:22:29.384718 whop_api_wrapper-1.0.9/
--rw-rw-rw-   0        0        0     1089 2023-07-17 07:39:09.000000 whop_api_wrapper-1.0.9/LICENSE
--rw-rw-rw-   0        0        0     2064 2023-07-17 20:22:29.384718 whop_api_wrapper-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     1306 2023-07-17 20:22:21.000000 whop_api_wrapper-1.0.9/README.md
--rw-rw-rw-   0        0        0       42 2023-07-17 20:22:29.385716 whop_api_wrapper-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1020 2023-07-17 20:22:26.000000 whop_api_wrapper-1.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 20:22:29.368491 whop_api_wrapper-1.0.9/whop_api_wrapper/
--rw-rw-rw-   0        0        0    15949 2023-07-17 08:34:16.000000 whop_api_wrapper-1.0.9/whop_api_wrapper/Client.py
--rw-rw-rw-   0        0        0      251 2023-07-16 05:41:49.000000 whop_api_wrapper-1.0.9/whop_api_wrapper/Endpoints.py
--rw-rw-rw-   0        0        0     5957 2023-07-17 07:34:42.000000 whop_api_wrapper-1.0.9/whop_api_wrapper/Objects.py
--rw-rw-rw-   0        0        0      148 2023-07-17 20:11:49.000000 whop_api_wrapper-1.0.9/whop_api_wrapper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 20:22:29.384718 whop_api_wrapper-1.0.9/whop_api_wrapper.egg-info/
--rw-rw-rw-   0        0        0     2064 2023-07-17 20:22:29.000000 whop_api_wrapper-1.0.9/whop_api_wrapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      339 2023-07-17 20:22:29.000000 whop_api_wrapper-1.0.9/whop_api_wrapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 20:22:29.000000 whop_api_wrapper-1.0.9/whop_api_wrapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-17 20:22:29.000000 whop_api_wrapper-1.0.9/whop_api_wrapper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-17 20:22:29.000000 whop_api_wrapper-1.0.9/whop_api_wrapper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 20:23:51.411208 whop_api_wrapper-1.1.0/
+-rw-rw-rw-   0        0        0     1089 2023-07-17 07:39:09.000000 whop_api_wrapper-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     2064 2023-07-17 20:23:51.411208 whop_api_wrapper-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1306 2023-07-17 20:23:12.000000 whop_api_wrapper-1.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-17 20:23:51.411208 whop_api_wrapper-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1020 2023-07-17 20:23:49.000000 whop_api_wrapper-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 20:23:51.401724 whop_api_wrapper-1.1.0/whop_api_wrapper/
+-rw-rw-rw-   0        0        0    15949 2023-07-17 08:34:16.000000 whop_api_wrapper-1.1.0/whop_api_wrapper/Client.py
+-rw-rw-rw-   0        0        0      251 2023-07-16 05:41:49.000000 whop_api_wrapper-1.1.0/whop_api_wrapper/Endpoints.py
+-rw-rw-rw-   0        0        0     5957 2023-07-17 07:34:42.000000 whop_api_wrapper-1.1.0/whop_api_wrapper/Objects.py
+-rw-rw-rw-   0        0        0      148 2023-07-17 20:11:49.000000 whop_api_wrapper-1.1.0/whop_api_wrapper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 20:23:51.410211 whop_api_wrapper-1.1.0/whop_api_wrapper.egg-info/
+-rw-rw-rw-   0        0        0     2064 2023-07-17 20:23:51.000000 whop_api_wrapper-1.1.0/whop_api_wrapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      339 2023-07-17 20:23:51.000000 whop_api_wrapper-1.1.0/whop_api_wrapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 20:23:51.000000 whop_api_wrapper-1.1.0/whop_api_wrapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-17 20:23:51.000000 whop_api_wrapper-1.1.0/whop_api_wrapper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-17 20:23:51.000000 whop_api_wrapper-1.1.0/whop_api_wrapper.egg-info/top_level.txt
```

### Comparing `whop_api_wrapper-1.0.9/LICENSE` & `whop_api_wrapper-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `whop_api_wrapper-1.0.9/PKG-INFO` & `whop_api_wrapper-1.1.0/whop_api_wrapper.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: whop_api_wrapper
-Version: 1.0.9
+Name: whop-api-wrapper
+Version: 1.1.0
 Summary: Simple Python Whop API Wrapper
 Home-page: https://github.com/TheSweeet/Whop-API-Wrapper
 Author: Jacobfinn123
 Author-email: jacobfinn@bezosproxy.com
 Keywords: WHOP,API,WRAPPER
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -29,15 +29,15 @@
 pip install whop_api_wrapper
 ```
 
 ## Usage
 Initialize the Client class with your token, use any api call as a method of the client.
 
 ```py
-from Resources.Client import Client
+from whop_api_wrapper import Client
 
 client = Client("input_token_here")
 
 products = client.list_all_products()
 for product in products:
     print(product)  # Product(id=product_id, name=product_name, visibility=visible, created_at=123, experiences=[], plans=[])
```

### Comparing `whop_api_wrapper-1.0.9/README.md` & `whop_api_wrapper-1.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 pip install whop_api_wrapper
 ```
 
 ## Usage
 Initialize the Client class with your token, use any api call as a method of the client.
 
 ```py
-from Resources.Client import Client
+from whop_api_wrapper import Client
 
 client = Client("input_token_here")
 
 products = client.list_all_products()
 for product in products:
     print(product)  # Product(id=product_id, name=product_name, visibility=visible, created_at=123, experiences=[], plans=[])
```

### Comparing `whop_api_wrapper-1.0.9/setup.py` & `whop_api_wrapper-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='whop_api_wrapper',
-    version='1.0.9',
+    version='1.1.0',
     author='Jacobfinn123',
     author_email='jacobfinn@bezosproxy.com',
     description='Simple Python Whop API Wrapper',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/TheSweeet/Whop-API-Wrapper',
     packages=find_packages(),
```

### Comparing `whop_api_wrapper-1.0.9/whop_api_wrapper/Client.py` & `whop_api_wrapper-1.1.0/whop_api_wrapper/Client.py`

 * *Files identical despite different names*

### Comparing `whop_api_wrapper-1.0.9/whop_api_wrapper/Objects.py` & `whop_api_wrapper-1.1.0/whop_api_wrapper/Objects.py`

 * *Files identical despite different names*

### Comparing `whop_api_wrapper-1.0.9/whop_api_wrapper.egg-info/PKG-INFO` & `whop_api_wrapper-1.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: whop-api-wrapper
-Version: 1.0.9
+Name: whop_api_wrapper
+Version: 1.1.0
 Summary: Simple Python Whop API Wrapper
 Home-page: https://github.com/TheSweeet/Whop-API-Wrapper
 Author: Jacobfinn123
 Author-email: jacobfinn@bezosproxy.com
 Keywords: WHOP,API,WRAPPER
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -29,15 +29,15 @@
 pip install whop_api_wrapper
 ```
 
 ## Usage
 Initialize the Client class with your token, use any api call as a method of the client.
 
 ```py
-from Resources.Client import Client
+from whop_api_wrapper import Client
 
 client = Client("input_token_here")
 
 products = client.list_all_products()
 for product in products:
     print(product)  # Product(id=product_id, name=product_name, visibility=visible, created_at=123, experiences=[], plans=[])
```

