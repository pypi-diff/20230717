# Comparing `tmp/dock-py-selenium-1.0.0.tar.gz` & `tmp/dock-py-selenium-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dock-py-selenium-1.0.0.tar", last modified: Mon Jul 17 04:37:40 2023, max compression
+gzip compressed data, was "dock-py-selenium-1.0.1.tar", last modified: Mon Jul 17 04:47:46 2023, max compression
```

## Comparing `dock-py-selenium-1.0.0.tar` & `dock-py-selenium-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 04:37:40.297470 dock-py-selenium-1.0.0/
--rw-rw-rw-   0        0        0      652 2023-07-17 04:37:40.296474 dock-py-selenium-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1069 2023-07-17 03:34:17.000000 dock-py-selenium-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 04:37:40.250597 dock-py-selenium-1.0.0/dock_py_selenium/
-drwxrwxrwx   0        0        0        0 2023-07-17 04:37:40.294480 dock-py-selenium-1.0.0/dock_py_selenium/dock/
--rw-rw-rw-   0        0        0     5057 2023-07-16 05:50:03.000000 dock-py-selenium-1.0.0/dock_py_selenium/dock/dock.py
-drwxrwxrwx   0        0        0        0 2023-07-17 04:37:40.286501 dock-py-selenium-1.0.0/dock_py_selenium.egg-info/
--rw-rw-rw-   0        0        0      652 2023-07-17 04:37:40.000000 dock-py-selenium-1.0.0/dock_py_selenium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      247 2023-07-17 04:37:40.000000 dock-py-selenium-1.0.0/dock_py_selenium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 04:37:40.000000 dock-py-selenium-1.0.0/dock_py_selenium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-17 04:37:40.000000 dock-py-selenium-1.0.0/dock_py_selenium.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-17 04:37:40.000000 dock-py-selenium-1.0.0/dock_py_selenium.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-17 04:37:40.298469 dock-py-selenium-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      855 2023-07-17 04:37:34.000000 dock-py-selenium-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 04:47:46.087743 dock-py-selenium-1.0.1/
+-rw-rw-rw-   0        0        0      652 2023-07-17 04:47:46.085751 dock-py-selenium-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1069 2023-07-17 03:34:17.000000 dock-py-selenium-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 04:47:46.013795 dock-py-selenium-1.0.1/dock_py_selenium/
+drwxrwxrwx   0        0        0        0 2023-07-17 04:47:46.083755 dock-py-selenium-1.0.1/dock_py_selenium/dock/
+-rw-rw-rw-   0        0        0     5062 2023-07-17 04:47:03.000000 dock-py-selenium-1.0.1/dock_py_selenium/dock/dock.py
+drwxrwxrwx   0        0        0        0 2023-07-17 04:47:46.080763 dock-py-selenium-1.0.1/dock_py_selenium.egg-info/
+-rw-rw-rw-   0        0        0      652 2023-07-17 04:47:45.000000 dock-py-selenium-1.0.1/dock_py_selenium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      247 2023-07-17 04:47:45.000000 dock-py-selenium-1.0.1/dock_py_selenium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 04:47:45.000000 dock-py-selenium-1.0.1/dock_py_selenium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-17 04:47:45.000000 dock-py-selenium-1.0.1/dock_py_selenium.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-17 04:47:45.000000 dock-py-selenium-1.0.1/dock_py_selenium.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 04:47:46.089744 dock-py-selenium-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      855 2023-07-17 04:47:40.000000 dock-py-selenium-1.0.1/setup.py
```

### Comparing `dock-py-selenium-1.0.0/PKG-INFO` & `dock-py-selenium-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dock-py-selenium
-Version: 1.0.0
+Version: 1.0.1
 Summary: A startup / mockup folder for a selenium project with custom methods.
 Home-page: https://github.com/iambstha/dockSelenium
 Author: Bishal Shrestha
 Author-email: iambstha@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dock-py-selenium-1.0.0/README.md` & `dock-py-selenium-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `dock-py-selenium-1.0.0/dock_py_selenium/dock/dock.py` & `dock-py-selenium-1.0.1/dock_py_selenium/dock/dock.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 class Driver:
     # Initialized with driver
     def __init__(self, driver):
         self.driver = driver
 
     # Gets the title of a webpage
     def getTitle(self):
-        print(driver.title)
+        print(self.driver.title)
     
     # Only checks button & input of type submit
     def checkClick(self,element):
         cur_url = driver.current_url
         match element:
             case "button":
                 try:
```

### Comparing `dock-py-selenium-1.0.0/dock_py_selenium.egg-info/PKG-INFO` & `dock-py-selenium-1.0.1/dock_py_selenium.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dock-py-selenium
-Version: 1.0.0
+Version: 1.0.1
 Summary: A startup / mockup folder for a selenium project with custom methods.
 Home-page: https://github.com/iambstha/dockSelenium
 Author: Bishal Shrestha
 Author-email: iambstha@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dock-py-selenium-1.0.0/setup.py` & `dock-py-selenium-1.0.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="dock-py-selenium",
-    version="1.0.0",
+    version="1.0.1",
     author="Bishal Shrestha",
     author_email="iambstha@gmail.com",
     description="A startup / mockup folder for a selenium project with custom methods.",
     long_description="",
     long_description_content_type="text/markdown",
     url="https://github.com/iambstha/dockSelenium",
     packages=["dock_py_selenium.dock"],
```

