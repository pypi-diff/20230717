# Comparing `tmp/dock-py-selenium-2.1.2.tar.gz` & `tmp/dock-py-selenium-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dock-py-selenium-2.1.2.tar", last modified: Mon Jul 17 10:40:43 2023, max compression
+gzip compressed data, was "dock-py-selenium-2.1.3.tar", last modified: Mon Jul 17 11:08:23 2023, max compression
```

## Comparing `dock-py-selenium-2.1.2.tar` & `dock-py-selenium-2.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 10:40:43.444467 dock-py-selenium-2.1.2/
-drwxrwxrwx   0        0        0        0 2023-07-17 10:40:43.435459 dock-py-selenium-2.1.2/Dock_Py_Selenium.egg-info/
--rw-rw-rw-   0        0        0      572 2023-07-17 10:40:43.000000 dock-py-selenium-2.1.2/Dock_Py_Selenium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      446 2023-07-17 10:40:43.000000 dock-py-selenium-2.1.2/Dock_Py_Selenium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 10:40:43.000000 dock-py-selenium-2.1.2/Dock_Py_Selenium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-17 10:40:43.000000 dock-py-selenium-2.1.2/Dock_Py_Selenium.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-17 10:40:43.000000 dock-py-selenium-2.1.2/Dock_Py_Selenium.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      572 2023-07-17 10:40:43.442464 dock-py-selenium-2.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1807 2023-07-17 10:10:05.000000 dock-py-selenium-2.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 10:40:43.387462 dock-py-selenium-2.1.2/dock_py_selenium/
-drwxrwxrwx   0        0        0        0 2023-07-17 10:40:43.439463 dock-py-selenium-2.1.2/dock_py_selenium/dock/
--rw-rw-rw-   0        0        0     7817 2023-07-17 10:32:37.000000 dock-py-selenium-2.1.2/dock_py_selenium/dock/dock.py
--rw-rw-rw-   0        0        0       42 2023-07-17 10:40:43.445466 dock-py-selenium-2.1.2/setup.cfg
--rw-rw-rw-   0        0        0      774 2023-07-17 10:40:16.000000 dock-py-selenium-2.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 11:08:23.013614 dock-py-selenium-2.1.3/
+drwxrwxrwx   0        0        0        0 2023-07-17 11:08:23.002618 dock-py-selenium-2.1.3/Dock_Py_Selenium.egg-info/
+-rw-rw-rw-   0        0        0      572 2023-07-17 11:08:22.000000 dock-py-selenium-2.1.3/Dock_Py_Selenium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      446 2023-07-17 11:08:22.000000 dock-py-selenium-2.1.3/Dock_Py_Selenium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 11:08:22.000000 dock-py-selenium-2.1.3/Dock_Py_Selenium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-17 11:08:22.000000 dock-py-selenium-2.1.3/Dock_Py_Selenium.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-17 11:08:22.000000 dock-py-selenium-2.1.3/Dock_Py_Selenium.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      572 2023-07-17 11:08:23.010610 dock-py-selenium-2.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1807 2023-07-17 10:10:05.000000 dock-py-selenium-2.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 11:08:22.924614 dock-py-selenium-2.1.3/dock_py_selenium/
+drwxrwxrwx   0        0        0        0 2023-07-17 11:08:23.008618 dock-py-selenium-2.1.3/dock_py_selenium/dock/
+-rw-rw-rw-   0        0        0     8412 2023-07-17 11:05:44.000000 dock-py-selenium-2.1.3/dock_py_selenium/dock/dock.py
+-rw-rw-rw-   0        0        0       42 2023-07-17 11:08:23.013614 dock-py-selenium-2.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      774 2023-07-17 11:08:05.000000 dock-py-selenium-2.1.3/setup.py
```

### Comparing `dock-py-selenium-2.1.2/Dock_Py_Selenium.egg-info/PKG-INFO` & `dock-py-selenium-2.1.3/Dock_Py_Selenium.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dock-py-selenium
-Version: 2.1.2
+Version: 2.1.3
 Summary: A startup / mockup folder for a selenium project with custom methods.
 Home-page: https://github.com/iambstha/dock-py-selenium
 Author: Bishal Shrestha
 Author-email: iambstha@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dock-py-selenium-2.1.2/PKG-INFO` & `dock-py-selenium-2.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dock-py-selenium
-Version: 2.1.2
+Version: 2.1.3
 Summary: A startup / mockup folder for a selenium project with custom methods.
 Home-page: https://github.com/iambstha/dock-py-selenium
 Author: Bishal Shrestha
 Author-email: iambstha@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dock-py-selenium-2.1.2/README.md` & `dock-py-selenium-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `dock-py-selenium-2.1.2/dock_py_selenium/dock/dock.py` & `dock-py-selenium-2.1.3/dock_py_selenium/dock/dock.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from selenium.webdriver.common.by import By
 from selenium.common.exceptions import NoSuchElementException
 from selenium.webdriver.chrome.options import Options as ChromeOptions
 from selenium.webdriver.common.keys import Keys
 
 # Set options
 options = ChromeOptions()
-# options.add_argument("--headless")
+options.add_argument("--headless")
 
 #driver settings
 driver = webdriver.Chrome(options=options)
 driver.maximize_window
 
 class Driver:
     # Initialized with driver
@@ -29,14 +29,27 @@
         print(self.driver.title)
 
     def checkTitle(self,title):
         if title == self.driver.title:
             print("Yes! The correct title is " + title)
         else:
             print("The title " + title + " is incorrect.")
+
+    # Get the height and width of the window
+    def dimension(self,param):
+        height = self.driver.execute_script("return window.innerHeight;")
+        width = self.driver.execute_script("return window.innerWidth;")
+        if param == "h":
+            print("Window's Height: " + str(height) + "px")
+        elif param == "w":
+            print("Window's Width: " + str(width) + "px")
+        elif param == "hw":
+            print("Window's Height: " + str(height) + "px & Window's Width : " + str(width) + "px")
+        else:
+            print("Invalid dimension property.")
     
     # Only checks button & input of type submit
     def checkClick(self, element):
         cur_url = self.driver.current_url
 
         if element == "button":
             try:
```

### Comparing `dock-py-selenium-2.1.2/setup.py` & `dock-py-selenium-2.1.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="dock-py-selenium",
-    version="2.1.2",
+    version="2.1.3",
     author="Bishal Shrestha",
     author_email="iambstha@gmail.com",
     description="A startup / mockup folder for a selenium project with custom methods.",
     long_description="# A startup / mockup folder for a selenium project with custom methods.",
     long_description_content_type="text/markdown",
     url="https://github.com/iambstha/dock-py-selenium",
     packages=["dock_py_selenium.dock"],
```

