# Comparing `tmp/whop-api-wrapper-1.0.1.tar.gz` & `tmp/whop-api-wrapper-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whop-api-wrapper-1.0.1.tar", last modified: Mon Jul 17 08:04:18 2023, max compression
+gzip compressed data, was "whop-api-wrapper-1.0.2.tar", last modified: Mon Jul 17 08:05:53 2023, max compression
```

## Comparing `whop-api-wrapper-1.0.1.tar` & `whop-api-wrapper-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 08:04:18.057497 whop-api-wrapper-1.0.1/
--rw-rw-rw-   0        0        0     1089 2023-07-17 07:39:09.000000 whop-api-wrapper-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     1419 2023-07-17 08:04:18.057497 whop-api-wrapper-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      641 2023-07-17 07:53:44.000000 whop-api-wrapper-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-17 08:04:18.057497 whop-api-wrapper-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1046 2023-07-17 08:02:04.000000 whop-api-wrapper-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 08:04:18.056499 whop-api-wrapper-1.0.1/whop_api_wrapper.egg-info/
--rw-rw-rw-   0        0        0     1419 2023-07-17 08:04:18.000000 whop-api-wrapper-1.0.1/whop_api_wrapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-07-17 08:04:18.000000 whop-api-wrapper-1.0.1/whop_api_wrapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 08:04:18.000000 whop-api-wrapper-1.0.1/whop_api_wrapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-17 08:04:18.000000 whop-api-wrapper-1.0.1/whop_api_wrapper.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 08:04:18.000000 whop-api-wrapper-1.0.1/whop_api_wrapper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 08:05:53.259072 whop-api-wrapper-1.0.2/
+-rw-rw-rw-   0        0        0     1089 2023-07-17 07:39:09.000000 whop-api-wrapper-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1391 2023-07-17 08:05:53.259072 whop-api-wrapper-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      641 2023-07-17 07:53:44.000000 whop-api-wrapper-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-17 08:05:53.259072 whop-api-wrapper-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1018 2023-07-17 08:05:51.000000 whop-api-wrapper-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 08:05:53.258075 whop-api-wrapper-1.0.2/whop_api_wrapper.egg-info/
+-rw-rw-rw-   0        0        0     1391 2023-07-17 08:05:53.000000 whop-api-wrapper-1.0.2/whop_api_wrapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2023-07-17 08:05:53.000000 whop-api-wrapper-1.0.2/whop_api_wrapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 08:05:53.000000 whop-api-wrapper-1.0.2/whop_api_wrapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-17 08:05:53.000000 whop-api-wrapper-1.0.2/whop_api_wrapper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 08:05:53.000000 whop-api-wrapper-1.0.2/whop_api_wrapper.egg-info/top_level.txt
```

### Comparing `whop-api-wrapper-1.0.1/LICENSE` & `whop-api-wrapper-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `whop-api-wrapper-1.0.1/PKG-INFO` & `whop-api-wrapper-1.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: whop-api-wrapper
-Version: 1.0.1
+Version: 1.0.2
 Summary: Simple Python Whop API Wrapper
 Home-page: https://github.com/TheSweeet/Whop-API-Wrapper
 Author: Jacobfinn123
 Author-email: jacobfinn@bezosproxy.com
 Keywords: WHOP,API,WRAPPER
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: # Whop-API-Wrapper
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Whop-API-Wrapper
 
 A simple python API wrapper of Whop's API, documentation can be found at: https://dev.whop.com/reference/home
 
 ## Installation
 
 To install the package, use the following command:
 
@@ -34,10 +37,7 @@
 
 client.list_all_products()
 client.retrieve_membership("membership_id_here")
 client.create_promo_code(amount_off=25, base_currency="usd", code="25off", promo_type="flat_amount")
 ```
 
 Feel free open any issues or report them to me on discord, `jacobfinn`.
-License-File: LICENSE
-
-Makes use of the Whop API easy in python.
```

### Comparing `whop-api-wrapper-1.0.1/README.md` & `whop-api-wrapper-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `whop-api-wrapper-1.0.1/setup.py` & `whop-api-wrapper-1.0.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='whop-api-wrapper',
-    version='1.0.1',
+    version='1.0.2',
     author='Jacobfinn123',
     author_email='jacobfinn@bezosproxy.com',
     description='Simple Python Whop API Wrapper',
-    long_description='Makes use of the Whop API easy in python.',
-    long_description_content_type=long_description,
+    long_description=long_description,
+    long_description_content_type='text/markdown',
     url='https://github.com/TheSweeet/Whop-API-Wrapper',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
```

### Comparing `whop-api-wrapper-1.0.1/whop_api_wrapper.egg-info/PKG-INFO` & `whop-api-wrapper-1.0.2/whop_api_wrapper.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: whop-api-wrapper
-Version: 1.0.1
+Version: 1.0.2
 Summary: Simple Python Whop API Wrapper
 Home-page: https://github.com/TheSweeet/Whop-API-Wrapper
 Author: Jacobfinn123
 Author-email: jacobfinn@bezosproxy.com
 Keywords: WHOP,API,WRAPPER
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: # Whop-API-Wrapper
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Whop-API-Wrapper
 
 A simple python API wrapper of Whop's API, documentation can be found at: https://dev.whop.com/reference/home
 
 ## Installation
 
 To install the package, use the following command:
 
@@ -34,10 +37,7 @@
 
 client.list_all_products()
 client.retrieve_membership("membership_id_here")
 client.create_promo_code(amount_off=25, base_currency="usd", code="25off", promo_type="flat_amount")
 ```
 
 Feel free open any issues or report them to me on discord, `jacobfinn`.
-License-File: LICENSE
-
-Makes use of the Whop API easy in python.
```

