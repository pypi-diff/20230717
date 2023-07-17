# Comparing `tmp/dummy_url_wrapper-0.0.7.tar.gz` & `tmp/dummy_url_wrapper-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dummy_url_wrapper-0.0.7.tar", last modified: Mon Jul 17 10:22:31 2023, max compression
+gzip compressed data, was "dummy_url_wrapper-0.0.8.tar", last modified: Mon Jul 17 10:26:47 2023, max compression
```

## Comparing `dummy_url_wrapper-0.0.7.tar` & `dummy_url_wrapper-0.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 gautampandey  (1001) gautampandey  (1001)        0 2023-07-17 10:22:31.163387 dummy_url_wrapper-0.0.7/
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      714 2023-07-17 10:22:31.163387 dummy_url_wrapper-0.0.7/PKG-INFO
-drwxrwxr-x   0 gautampandey  (1001) gautampandey  (1001)        0 2023-07-17 10:22:31.159387 dummy_url_wrapper-0.0.7/dummy_url_wrapper/
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)       71 2023-07-17 09:13:05.000000 dummy_url_wrapper-0.0.7/dummy_url_wrapper/__init__.py
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)     5320 2023-07-17 09:16:16.000000 dummy_url_wrapper-0.0.7/dummy_url_wrapper/mysdk.py
-drwxrwxr-x   0 gautampandey  (1001) gautampandey  (1001)        0 2023-07-17 10:22:31.163387 dummy_url_wrapper-0.0.7/dummy_url_wrapper.egg-info/
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      714 2023-07-17 10:22:31.000000 dummy_url_wrapper-0.0.7/dummy_url_wrapper.egg-info/PKG-INFO
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      269 2023-07-17 10:22:31.000000 dummy_url_wrapper-0.0.7/dummy_url_wrapper.egg-info/SOURCES.txt
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)        1 2023-07-17 10:22:31.000000 dummy_url_wrapper-0.0.7/dummy_url_wrapper.egg-info/dependency_links.txt
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)       28 2023-07-17 10:22:31.000000 dummy_url_wrapper-0.0.7/dummy_url_wrapper.egg-info/requires.txt
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)       18 2023-07-17 10:22:31.000000 dummy_url_wrapper-0.0.7/dummy_url_wrapper.egg-info/top_level.txt
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)       38 2023-07-17 10:22:31.163387 dummy_url_wrapper-0.0.7/setup.cfg
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      894 2023-07-17 10:21:41.000000 dummy_url_wrapper-0.0.7/setup.py
+drwxrwxr-x   0 gautampandey  (1001) gautampandey  (1001)        0 2023-07-17 10:26:47.078899 dummy_url_wrapper-0.0.8/
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      714 2023-07-17 10:26:47.078899 dummy_url_wrapper-0.0.8/PKG-INFO
+drwxrwxr-x   0 gautampandey  (1001) gautampandey  (1001)        0 2023-07-17 10:26:47.078899 dummy_url_wrapper-0.0.8/dummy_url_wrapper/
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)       71 2023-07-17 09:13:05.000000 dummy_url_wrapper-0.0.8/dummy_url_wrapper/__init__.py
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)     5320 2023-07-17 09:16:16.000000 dummy_url_wrapper-0.0.8/dummy_url_wrapper/mysdk.py
+drwxrwxr-x   0 gautampandey  (1001) gautampandey  (1001)        0 2023-07-17 10:26:47.078899 dummy_url_wrapper-0.0.8/dummy_url_wrapper.egg-info/
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      714 2023-07-17 10:26:47.000000 dummy_url_wrapper-0.0.8/dummy_url_wrapper.egg-info/PKG-INFO
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      269 2023-07-17 10:26:47.000000 dummy_url_wrapper-0.0.8/dummy_url_wrapper.egg-info/SOURCES.txt
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)        1 2023-07-17 10:26:47.000000 dummy_url_wrapper-0.0.8/dummy_url_wrapper.egg-info/dependency_links.txt
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)       23 2023-07-17 10:26:47.000000 dummy_url_wrapper-0.0.8/dummy_url_wrapper.egg-info/requires.txt
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)       18 2023-07-17 10:26:47.000000 dummy_url_wrapper-0.0.8/dummy_url_wrapper.egg-info/top_level.txt
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)       38 2023-07-17 10:26:47.078899 dummy_url_wrapper-0.0.8/setup.cfg
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      886 2023-07-17 10:26:42.000000 dummy_url_wrapper-0.0.8/setup.py
```

### Comparing `dummy_url_wrapper-0.0.7/PKG-INFO` & `dummy_url_wrapper-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dummy_url_wrapper
-Version: 0.0.7
+Version: 0.0.8
 Summary: This package provides the wrapping of URLs for not exposing to clients
 Home-page: https://github.com/nk2909/Python-SDK.git
 Author: Nishant Kabariya
 Author-email: testurl@yopmail.com
 Keywords: python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
```

### Comparing `dummy_url_wrapper-0.0.7/dummy_url_wrapper/mysdk.py` & `dummy_url_wrapper-0.0.8/dummy_url_wrapper/mysdk.py`

 * *Files identical despite different names*

### Comparing `dummy_url_wrapper-0.0.7/dummy_url_wrapper.egg-info/PKG-INFO` & `dummy_url_wrapper-0.0.8/dummy_url_wrapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dummy-url-wrapper
-Version: 0.0.7
+Version: 0.0.8
 Summary: This package provides the wrapping of URLs for not exposing to clients
 Home-page: https://github.com/nk2909/Python-SDK.git
 Author: Nishant Kabariya
 Author-email: testurl@yopmail.com
 Keywords: python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
```

### Comparing `dummy_url_wrapper-0.0.7/setup.py` & `dummy_url_wrapper-0.0.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name="dummy_url_wrapper",
-    version="0.0.7",
+    version="0.0.8",
     description="This package provides the wrapping of URLs for not exposing to clients",
     url="https://github.com/nk2909/Python-SDK.git",
     author="Nishant Kabariya",
     author_email="testurl@yopmail.com",
-    install_requires=["python-dotenv", "requests", "json"],
+    install_requires=["python-dotenv", "requests"],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Education",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.5",
```

