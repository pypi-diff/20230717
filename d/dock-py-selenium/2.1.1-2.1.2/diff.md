# Comparing `tmp/dock-py-selenium-2.1.1.tar.gz` & `tmp/dock-py-selenium-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dock-py-selenium-2.1.1.tar", last modified: Mon Jul 17 09:56:56 2023, max compression
+gzip compressed data, was "dock-py-selenium-2.1.2.tar", last modified: Mon Jul 17 10:40:43 2023, max compression
```

## Comparing `dock-py-selenium-2.1.1.tar` & `dock-py-selenium-2.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 09:56:56.060380 dock-py-selenium-2.1.1/
-drwxrwxrwx   0        0        0        0 2023-07-17 09:56:56.050380 dock-py-selenium-2.1.1/Dock_Py_Selenium.egg-info/
--rw-rw-rw-   0        0        0      572 2023-07-17 09:56:55.000000 dock-py-selenium-2.1.1/Dock_Py_Selenium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      446 2023-07-17 09:56:55.000000 dock-py-selenium-2.1.1/Dock_Py_Selenium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 09:56:55.000000 dock-py-selenium-2.1.1/Dock_Py_Selenium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-17 09:56:55.000000 dock-py-selenium-2.1.1/Dock_Py_Selenium.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-17 09:56:55.000000 dock-py-selenium-2.1.1/Dock_Py_Selenium.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      572 2023-07-17 09:56:56.057377 dock-py-selenium-2.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      971 2023-07-17 05:59:50.000000 dock-py-selenium-2.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 09:56:55.984414 dock-py-selenium-2.1.1/dock_py_selenium/
-drwxrwxrwx   0        0        0        0 2023-07-17 09:56:56.055378 dock-py-selenium-2.1.1/dock_py_selenium/dock/
--rw-rw-rw-   0        0        0     6828 2023-07-17 09:46:10.000000 dock-py-selenium-2.1.1/dock_py_selenium/dock/dock.py
--rw-rw-rw-   0        0        0       42 2023-07-17 09:56:56.061380 dock-py-selenium-2.1.1/setup.cfg
--rw-rw-rw-   0        0        0      774 2023-07-17 09:56:22.000000 dock-py-selenium-2.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 10:40:43.444467 dock-py-selenium-2.1.2/
+drwxrwxrwx   0        0        0        0 2023-07-17 10:40:43.435459 dock-py-selenium-2.1.2/Dock_Py_Selenium.egg-info/
+-rw-rw-rw-   0        0        0      572 2023-07-17 10:40:43.000000 dock-py-selenium-2.1.2/Dock_Py_Selenium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      446 2023-07-17 10:40:43.000000 dock-py-selenium-2.1.2/Dock_Py_Selenium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 10:40:43.000000 dock-py-selenium-2.1.2/Dock_Py_Selenium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-17 10:40:43.000000 dock-py-selenium-2.1.2/Dock_Py_Selenium.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-17 10:40:43.000000 dock-py-selenium-2.1.2/Dock_Py_Selenium.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      572 2023-07-17 10:40:43.442464 dock-py-selenium-2.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1807 2023-07-17 10:10:05.000000 dock-py-selenium-2.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 10:40:43.387462 dock-py-selenium-2.1.2/dock_py_selenium/
+drwxrwxrwx   0        0        0        0 2023-07-17 10:40:43.439463 dock-py-selenium-2.1.2/dock_py_selenium/dock/
+-rw-rw-rw-   0        0        0     7817 2023-07-17 10:32:37.000000 dock-py-selenium-2.1.2/dock_py_selenium/dock/dock.py
+-rw-rw-rw-   0        0        0       42 2023-07-17 10:40:43.445466 dock-py-selenium-2.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      774 2023-07-17 10:40:16.000000 dock-py-selenium-2.1.2/setup.py
```

### Comparing `dock-py-selenium-2.1.1/Dock_Py_Selenium.egg-info/PKG-INFO` & `dock-py-selenium-2.1.2/Dock_Py_Selenium.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dock-py-selenium
-Version: 2.1.1
+Version: 2.1.2
 Summary: A startup / mockup folder for a selenium project with custom methods.
 Home-page: https://github.com/iambstha/dock-py-selenium
 Author: Bishal Shrestha
 Author-email: iambstha@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dock-py-selenium-2.1.1/PKG-INFO` & `dock-py-selenium-2.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dock-py-selenium
-Version: 2.1.1
+Version: 2.1.2
 Summary: A startup / mockup folder for a selenium project with custom methods.
 Home-page: https://github.com/iambstha/dock-py-selenium
 Author: Bishal Shrestha
 Author-email: iambstha@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dock-py-selenium-2.1.1/dock_py_selenium/dock/dock.py` & `dock-py-selenium-2.1.2/dock_py_selenium/dock/dock.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import time
 from selenium import webdriver
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.common.by import By
 from selenium.common.exceptions import NoSuchElementException
 from selenium.webdriver.chrome.options import Options as ChromeOptions
+from selenium.webdriver.common.keys import Keys
 
 # Set options
 options = ChromeOptions()
 # options.add_argument("--headless")
 
 #driver settings
 driver = webdriver.Chrome(options=options)
@@ -68,103 +69,111 @@
         match elem:
             case "id":
                 try:
                     e = self.driver.find_element(By.ID, i)
                     print("The element with ID '" + i + "' is available.")
                     return e
                 except NoSuchElementException as err:
-                    print("Exception: " + err.msg)
+                    print("Exception: The element with ID '" + i + "' is not available.")
             
             case "name":
                 try:
                     e = self.driver.find_element(By.NAME, i)
                     print("The element with name '" + i + "' is available.")
                     return e
                 except NoSuchElementException as err:
-                    print("Exception: " + err.msg)
+                    print("Exception: The element with name '" + i + "' is not available.")
             
-            case "pname":
+            case "name_many":
                 try:
                     e = self.driver.find_elements(By.NAME, i)
                     print("The elements with name '" + i + "' is available.")
                     return e
                 except NoSuchElementException as err:
-                    print("Exception: " + err.msg)
+                    print("Exception: The elements with name '" + i + "' is not available.")
             
             case "class":
                 try:
                     e = self.driver.find_element(By.CLASS_NAME, i)
                     print("The element with class name '" + i + "' is available.")
                     return e
                 except NoSuchElementException as err:
-                    print("Exception: " + err.msg)
+                    print("Exception: The element with ID '" + i + "' is not available.")
 
-            case "pclass":
+            case "class_many":
                 try:
                     e = self.driver.find_elements(By.CLASS_NAME, i)
                     print("The elements with class name '" + i + "' is available.")
                     return e
                 except NoSuchElementException as err:
-                    print("Exception: " + err.msg)
+                    print("Exception: The elements with class name '" + i + "' is not available.")
             
             case "tag":
                 try:
                     e = self.driver.find_elements(By.TAG_NAME, i)
                     print("The elements with tag name '" + i + "' is available.")
                     return e
                 except NoSuchElementException as err:
-                    print("Exception: " + err.msg)
+                    print("Exception: The element with tag '" + i + "' is not available.")
+
+            case "tag_many":
+                try:
+                    e = self.driver.find_elements(By.TAG_NAME, i)
+                    print("The elements with tag name '" + i + "' is available.")
+                    return e
+                except NoSuchElementException as err:
+                    print("Exception: The elements with tag '" + i + "' is not available.")
             
             case "link_text":
                 try:
                     e = self.driver.find_element(By.LINK_TEXT, i)
                     print("The element with link text '" + i + "' is available.")
                     return e
                 except NoSuchElementException as err:
-                    print("Exception: " + err.msg)
+                    print("Exception: The element with link text '" + i + "' is not available.")
             
             case "partial_link_text":
                 try:
                     e = self.driver.find_element(By.PARTIAL_LINK_TEXT, i)
                     print("The element with partial link text '" + i + "' is available.")
                     return e
                 except NoSuchElementException as err:
-                    print("Exception: " + err.msg)
+                    print("Exception: The element with partial link text '" + i + "' is not available.")
             
-            case "selector":
+            case "css_selector":
                 try:
                     e = self.driver.find_element(By.CSS_SELECTOR, i)
                     print("The element with CSS selector '" + i + "' is available.")
                     return e
                 except NoSuchElementException as err:
-                    print("Exception: " + err.msg)
+                    print("Exception: The element with CSS Selector '" + i + "' is not available.")
             
-            case "pselector":
+            case "css_selector_many":
                 try:
                     e = self.driver.find_elements(By.CSS_SELECTOR, i)
                     print("The elements with CSS selector '" + i + "' is available.")
                     return e
                 except NoSuchElementException as err:
-                    print("Exception: " + err.msg)
+                    print("Exception: The elements with CSS Selector '" + i + "' is not available.")
             
             case "xpath":
                 try:
                     e = self.driver.find_element(By.XPATH, i)
                     print("The element with XPath '" + i + "' is available.")
                     return e
                 except NoSuchElementException as err:
-                    print("Exception: " + err.msg)
+                    print("Exception: The element with XPATH '" + i + "' is not available.")
 
-            case "pxpath":
+            case "xpath_many":
                 try:
                     e = self.driver.find_elements(By.XPATH, i)
-                    print("The element with XPath '" + i + "' is available.")
+                    print("The elements with XPath '" + i + "' is available.")
                     return e
                 except NoSuchElementException as err:
-                    print("Exception: " + err.msg)
+                    print("Exception: The elements with xpath '" + i + "' is not available.")
             
             case _:
                 print("Invalid element.")
 
    
 
     # Rerun in dock for 'x' times
```

### Comparing `dock-py-selenium-2.1.1/setup.py` & `dock-py-selenium-2.1.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="dock-py-selenium",
-    version="2.1.1",
+    version="2.1.2",
     author="Bishal Shrestha",
     author_email="iambstha@gmail.com",
     description="A startup / mockup folder for a selenium project with custom methods.",
     long_description="# A startup / mockup folder for a selenium project with custom methods.",
     long_description_content_type="text/markdown",
     url="https://github.com/iambstha/dock-py-selenium",
     packages=["dock_py_selenium.dock"],
```

