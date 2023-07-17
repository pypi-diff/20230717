# Comparing `tmp/dock-py-selenium-2.0.1.tar.gz` & `tmp/dock-py-selenium-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dock-py-selenium-2.0.1.tar", last modified: Mon Jul 17 06:56:48 2023, max compression
+gzip compressed data, was "dock-py-selenium-2.1.1.tar", last modified: Mon Jul 17 09:56:56 2023, max compression
```

## Comparing `dock-py-selenium-2.0.1.tar` & `dock-py-selenium-2.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 06:56:48.209811 dock-py-selenium-2.0.1/
-drwxrwxrwx   0        0        0        0 2023-07-17 06:56:48.198835 dock-py-selenium-2.0.1/Dock_Py_Selenium.egg-info/
--rw-rw-rw-   0        0        0      572 2023-07-17 06:56:47.000000 dock-py-selenium-2.0.1/Dock_Py_Selenium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      446 2023-07-17 06:56:47.000000 dock-py-selenium-2.0.1/Dock_Py_Selenium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 06:56:47.000000 dock-py-selenium-2.0.1/Dock_Py_Selenium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-17 06:56:47.000000 dock-py-selenium-2.0.1/Dock_Py_Selenium.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-17 06:56:47.000000 dock-py-selenium-2.0.1/Dock_Py_Selenium.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      572 2023-07-17 06:56:48.206820 dock-py-selenium-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      971 2023-07-17 05:59:50.000000 dock-py-selenium-2.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 06:56:48.146218 dock-py-selenium-2.0.1/dock_py_selenium/
-drwxrwxrwx   0        0        0        0 2023-07-17 06:56:48.203834 dock-py-selenium-2.0.1/dock_py_selenium/dock/
--rw-rw-rw-   0        0        0     5252 2023-07-17 06:56:27.000000 dock-py-selenium-2.0.1/dock_py_selenium/dock/dock.py
--rw-rw-rw-   0        0        0       42 2023-07-17 06:56:48.210808 dock-py-selenium-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0      774 2023-07-17 05:51:06.000000 dock-py-selenium-2.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:56:56.060380 dock-py-selenium-2.1.1/
+drwxrwxrwx   0        0        0        0 2023-07-17 09:56:56.050380 dock-py-selenium-2.1.1/Dock_Py_Selenium.egg-info/
+-rw-rw-rw-   0        0        0      572 2023-07-17 09:56:55.000000 dock-py-selenium-2.1.1/Dock_Py_Selenium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      446 2023-07-17 09:56:55.000000 dock-py-selenium-2.1.1/Dock_Py_Selenium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 09:56:55.000000 dock-py-selenium-2.1.1/Dock_Py_Selenium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-17 09:56:55.000000 dock-py-selenium-2.1.1/Dock_Py_Selenium.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-17 09:56:55.000000 dock-py-selenium-2.1.1/Dock_Py_Selenium.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      572 2023-07-17 09:56:56.057377 dock-py-selenium-2.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      971 2023-07-17 05:59:50.000000 dock-py-selenium-2.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 09:56:55.984414 dock-py-selenium-2.1.1/dock_py_selenium/
+drwxrwxrwx   0        0        0        0 2023-07-17 09:56:56.055378 dock-py-selenium-2.1.1/dock_py_selenium/dock/
+-rw-rw-rw-   0        0        0     6828 2023-07-17 09:46:10.000000 dock-py-selenium-2.1.1/dock_py_selenium/dock/dock.py
+-rw-rw-rw-   0        0        0       42 2023-07-17 09:56:56.061380 dock-py-selenium-2.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      774 2023-07-17 09:56:22.000000 dock-py-selenium-2.1.1/setup.py
```

### Comparing `dock-py-selenium-2.0.1/Dock_Py_Selenium.egg-info/PKG-INFO` & `dock-py-selenium-2.1.1/Dock_Py_Selenium.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dock-py-selenium
-Version: 2.0.1
+Version: 2.1.1
 Summary: A startup / mockup folder for a selenium project with custom methods.
 Home-page: https://github.com/iambstha/dock-py-selenium
 Author: Bishal Shrestha
 Author-email: iambstha@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dock-py-selenium-2.0.1/PKG-INFO` & `dock-py-selenium-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dock-py-selenium
-Version: 2.0.1
+Version: 2.1.1
 Summary: A startup / mockup folder for a selenium project with custom methods.
 Home-page: https://github.com/iambstha/dock-py-selenium
 Author: Bishal Shrestha
 Author-email: iambstha@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dock-py-selenium-2.0.1/README.md` & `dock-py-selenium-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `dock-py-selenium-2.0.1/dock_py_selenium/dock/dock.py` & `dock-py-selenium-2.1.1/dock_py_selenium/dock/dock.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.common.by import By
 from selenium.common.exceptions import NoSuchElementException
 from selenium.webdriver.chrome.options import Options as ChromeOptions
 
 # Set options
 options = ChromeOptions()
-options.add_argument("--headless")
+# options.add_argument("--headless")
 
 #driver settings
 driver = webdriver.Chrome(options=options)
 driver.maximize_window
 
 class Driver:
     # Initialized with driver
@@ -22,14 +22,20 @@
     def start(self):
         getUrl = input("Enter the url: ")
         self.driver.get(getUrl)
 
     # Gets the title of a webpage
     def getTitle(self):
         print(self.driver.title)
+
+    def checkTitle(self,title):
+        if title == self.driver.title:
+            print("Yes! The correct title is " + title)
+        else:
+            print("The title " + title + " is incorrect.")
     
     # Only checks button & input of type submit
     def checkClick(self, element):
         cur_url = self.driver.current_url
 
         if element == "button":
             try:
@@ -56,77 +62,109 @@
             print("The button is clickable.")
         else:
             print("The button is not clickable.")
 
     # Checks for the availability of an element in a page
     def checkElement(self,elem,i):
         match elem:
-            case "ID":
+            case "id":
                 try:
                     e = self.driver.find_element(By.ID, i)
                     print("The element with ID '" + i + "' is available.")
                     return e
                 except NoSuchElementException as err:
                     print("Exception: " + err.msg)
             
-            case "NAME":
+            case "name":
                 try:
                     e = self.driver.find_element(By.NAME, i)
                     print("The element with name '" + i + "' is available.")
                     return e
                 except NoSuchElementException as err:
                     print("Exception: " + err.msg)
             
-            case "CLASS_NAME":
+            case "pname":
+                try:
+                    e = self.driver.find_elements(By.NAME, i)
+                    print("The elements with name '" + i + "' is available.")
+                    return e
+                except NoSuchElementException as err:
+                    print("Exception: " + err.msg)
+            
+            case "class":
                 try:
                     e = self.driver.find_element(By.CLASS_NAME, i)
                     print("The element with class name '" + i + "' is available.")
                     return e
                 except NoSuchElementException as err:
                     print("Exception: " + err.msg)
+
+            case "pclass":
+                try:
+                    e = self.driver.find_elements(By.CLASS_NAME, i)
+                    print("The elements with class name '" + i + "' is available.")
+                    return e
+                except NoSuchElementException as err:
+                    print("Exception: " + err.msg)
             
-            case "TAG_NAME":
+            case "tag":
                 try:
-                    e = self.driver.find_element(By.TAG_NAME, i)
-                    print("The element with tag name '" + i + "' is available.")
+                    e = self.driver.find_elements(By.TAG_NAME, i)
+                    print("The elements with tag name '" + i + "' is available.")
                     return e
                 except NoSuchElementException as err:
                     print("Exception: " + err.msg)
             
-            case "LINK_TEXT":
+            case "link_text":
                 try:
                     e = self.driver.find_element(By.LINK_TEXT, i)
                     print("The element with link text '" + i + "' is available.")
                     return e
                 except NoSuchElementException as err:
                     print("Exception: " + err.msg)
             
-            case "PARTIAL_LINK_TEXT":
+            case "partial_link_text":
                 try:
                     e = self.driver.find_element(By.PARTIAL_LINK_TEXT, i)
                     print("The element with partial link text '" + i + "' is available.")
                     return e
                 except NoSuchElementException as err:
                     print("Exception: " + err.msg)
             
-            case "CSS_SELECTOR":
+            case "selector":
                 try:
                     e = self.driver.find_element(By.CSS_SELECTOR, i)
                     print("The element with CSS selector '" + i + "' is available.")
                     return e
                 except NoSuchElementException as err:
                     print("Exception: " + err.msg)
             
-            case "XPATH":
+            case "pselector":
+                try:
+                    e = self.driver.find_elements(By.CSS_SELECTOR, i)
+                    print("The elements with CSS selector '" + i + "' is available.")
+                    return e
+                except NoSuchElementException as err:
+                    print("Exception: " + err.msg)
+            
+            case "xpath":
                 try:
                     e = self.driver.find_element(By.XPATH, i)
                     print("The element with XPath '" + i + "' is available.")
                     return e
                 except NoSuchElementException as err:
                     print("Exception: " + err.msg)
+
+            case "pxpath":
+                try:
+                    e = self.driver.find_elements(By.XPATH, i)
+                    print("The element with XPath '" + i + "' is available.")
+                    return e
+                except NoSuchElementException as err:
+                    print("Exception: " + err.msg)
             
             case _:
                 print("Invalid element.")
 
    
 
     # Rerun in dock for 'x' times
```

### Comparing `dock-py-selenium-2.0.1/setup.py` & `dock-py-selenium-2.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="dock-py-selenium",
-    version="2.0.1",
+    version="2.1.1",
     author="Bishal Shrestha",
     author_email="iambstha@gmail.com",
     description="A startup / mockup folder for a selenium project with custom methods.",
     long_description="# A startup / mockup folder for a selenium project with custom methods.",
     long_description_content_type="text/markdown",
     url="https://github.com/iambstha/dock-py-selenium",
     packages=["dock_py_selenium.dock"],
```

