# Comparing `tmp/dock-py-selenium-1.0.2.tar.gz` & `tmp/dock-py-selenium-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dock-py-selenium-1.0.2.tar", last modified: Mon Jul 17 04:57:16 2023, max compression
+gzip compressed data, was "dock-py-selenium-1.0.3.tar", last modified: Mon Jul 17 05:05:13 2023, max compression
```

## Comparing `dock-py-selenium-1.0.2.tar` & `dock-py-selenium-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 04:57:16.252317 dock-py-selenium-1.0.2/
--rw-rw-rw-   0        0        0      652 2023-07-17 04:57:16.249321 dock-py-selenium-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1069 2023-07-17 03:34:17.000000 dock-py-selenium-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 04:57:16.199455 dock-py-selenium-1.0.2/dock_py_selenium/
-drwxrwxrwx   0        0        0        0 2023-07-17 04:57:16.247325 dock-py-selenium-1.0.2/dock_py_selenium/dock/
--rw-rw-rw-   0        0        0     5138 2023-07-17 04:56:58.000000 dock-py-selenium-1.0.2/dock_py_selenium/dock/dock.py
-drwxrwxrwx   0        0        0        0 2023-07-17 04:57:16.243342 dock-py-selenium-1.0.2/dock_py_selenium.egg-info/
--rw-rw-rw-   0        0        0      652 2023-07-17 04:57:15.000000 dock-py-selenium-1.0.2/dock_py_selenium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      247 2023-07-17 04:57:16.000000 dock-py-selenium-1.0.2/dock_py_selenium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 04:57:15.000000 dock-py-selenium-1.0.2/dock_py_selenium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-17 04:57:15.000000 dock-py-selenium-1.0.2/dock_py_selenium.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-17 04:57:15.000000 dock-py-selenium-1.0.2/dock_py_selenium.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-17 04:57:16.253311 dock-py-selenium-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      855 2023-07-17 04:57:09.000000 dock-py-selenium-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 05:05:13.724522 dock-py-selenium-1.0.3/
+-rw-rw-rw-   0        0        0      652 2023-07-17 05:05:13.723528 dock-py-selenium-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1069 2023-07-17 03:34:17.000000 dock-py-selenium-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 05:05:13.649721 dock-py-selenium-1.0.3/dock_py_selenium/
+drwxrwxrwx   0        0        0        0 2023-07-17 05:05:13.720532 dock-py-selenium-1.0.3/dock_py_selenium/dock/
+-rw-rw-rw-   0        0        0     5138 2023-07-17 05:04:43.000000 dock-py-selenium-1.0.3/dock_py_selenium/dock/dock.py
+drwxrwxrwx   0        0        0        0 2023-07-17 05:05:13.709562 dock-py-selenium-1.0.3/dock_py_selenium.egg-info/
+-rw-rw-rw-   0        0        0      652 2023-07-17 05:05:13.000000 dock-py-selenium-1.0.3/dock_py_selenium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      247 2023-07-17 05:05:13.000000 dock-py-selenium-1.0.3/dock_py_selenium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 05:05:13.000000 dock-py-selenium-1.0.3/dock_py_selenium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-17 05:05:13.000000 dock-py-selenium-1.0.3/dock_py_selenium.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-17 05:05:13.000000 dock-py-selenium-1.0.3/dock_py_selenium.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 05:05:13.725519 dock-py-selenium-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      855 2023-07-17 05:05:07.000000 dock-py-selenium-1.0.3/setup.py
```

### Comparing `dock-py-selenium-1.0.2/PKG-INFO` & `dock-py-selenium-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dock-py-selenium
-Version: 1.0.2
+Version: 1.0.3
 Summary: A startup / mockup folder for a selenium project with custom methods.
 Home-page: https://github.com/iambstha/dockSelenium
 Author: Bishal Shrestha
 Author-email: iambstha@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dock-py-selenium-1.0.2/README.md` & `dock-py-selenium-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `dock-py-selenium-1.0.2/dock_py_selenium/dock/dock.py` & `dock-py-selenium-1.0.3/dock_py_selenium/dock/dock.py`

 * *Files identical despite different names*

### Comparing `dock-py-selenium-1.0.2/dock_py_selenium.egg-info/PKG-INFO` & `dock-py-selenium-1.0.3/dock_py_selenium.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dock-py-selenium
-Version: 1.0.2
+Version: 1.0.3
 Summary: A startup / mockup folder for a selenium project with custom methods.
 Home-page: https://github.com/iambstha/dockSelenium
 Author: Bishal Shrestha
 Author-email: iambstha@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dock-py-selenium-1.0.2/setup.py` & `dock-py-selenium-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="dock-py-selenium",
-    version="1.0.2",
+    version="1.0.3",
     author="Bishal Shrestha",
     author_email="iambstha@gmail.com",
     description="A startup / mockup folder for a selenium project with custom methods.",
     long_description="",
     long_description_content_type="text/markdown",
     url="https://github.com/iambstha/dockSelenium",
     packages=["dock_py_selenium.dock"],
```

