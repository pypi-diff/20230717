# Comparing `tmp/whop-api-wrapper-1.0.2.tar.gz` & `tmp/whop-api-wrapper-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whop-api-wrapper-1.0.2.tar", last modified: Mon Jul 17 08:05:53 2023, max compression
+gzip compressed data, was "whop-api-wrapper-1.0.3.tar", last modified: Mon Jul 17 08:20:49 2023, max compression
```

## Comparing `whop-api-wrapper-1.0.2.tar` & `whop-api-wrapper-1.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 08:05:53.259072 whop-api-wrapper-1.0.2/
--rw-rw-rw-   0        0        0     1089 2023-07-17 07:39:09.000000 whop-api-wrapper-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     1391 2023-07-17 08:05:53.259072 whop-api-wrapper-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      641 2023-07-17 07:53:44.000000 whop-api-wrapper-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-17 08:05:53.259072 whop-api-wrapper-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1018 2023-07-17 08:05:51.000000 whop-api-wrapper-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 08:05:53.258075 whop-api-wrapper-1.0.2/whop_api_wrapper.egg-info/
--rw-rw-rw-   0        0        0     1391 2023-07-17 08:05:53.000000 whop-api-wrapper-1.0.2/whop_api_wrapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-07-17 08:05:53.000000 whop-api-wrapper-1.0.2/whop_api_wrapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 08:05:53.000000 whop-api-wrapper-1.0.2/whop_api_wrapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-17 08:05:53.000000 whop-api-wrapper-1.0.2/whop_api_wrapper.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 08:05:53.000000 whop-api-wrapper-1.0.2/whop_api_wrapper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 08:20:49.638229 whop-api-wrapper-1.0.3/
+-rw-rw-rw-   0        0        0     1089 2023-07-17 07:39:09.000000 whop-api-wrapper-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     2064 2023-07-17 08:20:49.637232 whop-api-wrapper-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1306 2023-07-17 08:12:50.000000 whop-api-wrapper-1.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-17 08:20:49.638229 whop-api-wrapper-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1018 2023-07-17 08:20:48.000000 whop-api-wrapper-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 08:20:49.637232 whop-api-wrapper-1.0.3/whop_api_wrapper.egg-info/
+-rw-rw-rw-   0        0        0     2064 2023-07-17 08:20:49.000000 whop-api-wrapper-1.0.3/whop_api_wrapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2023-07-17 08:20:49.000000 whop-api-wrapper-1.0.3/whop_api_wrapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 08:20:49.000000 whop-api-wrapper-1.0.3/whop_api_wrapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-17 08:20:49.000000 whop-api-wrapper-1.0.3/whop_api_wrapper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 08:20:49.000000 whop-api-wrapper-1.0.3/whop_api_wrapper.egg-info/top_level.txt
```

### Comparing `whop-api-wrapper-1.0.2/LICENSE` & `whop-api-wrapper-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `whop-api-wrapper-1.0.2/setup.py` & `whop-api-wrapper-1.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='whop-api-wrapper',
-    version='1.0.2',
+    version='1.0.3',
     author='Jacobfinn123',
     author_email='jacobfinn@bezosproxy.com',
     description='Simple Python Whop API Wrapper',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/TheSweeet/Whop-API-Wrapper',
     packages=find_packages(),
```

