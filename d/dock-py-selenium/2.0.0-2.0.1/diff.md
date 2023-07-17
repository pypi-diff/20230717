# Comparing `tmp/Dock Py Selenium-2.0.0.tar.gz` & `tmp/dock-py-selenium-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Dock Py Selenium-2.0.0.tar", last modified: Mon Jul 17 05:45:46 2023, max compression
+gzip compressed data, was "dock-py-selenium-2.0.1.tar", last modified: Mon Jul 17 06:56:48 2023, max compression
```

## Comparing `Dock Py Selenium-2.0.0.tar` & `dock-py-selenium-2.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 05:45:46.392917 Dock Py Selenium-2.0.0/
-drwxrwxrwx   0        0        0        0 2023-07-17 05:45:46.383226 Dock Py Selenium-2.0.0/Dock_Py_Selenium.egg-info/
--rw-rw-rw-   0        0        0      497 2023-07-17 05:45:46.000000 Dock Py Selenium-2.0.0/Dock_Py_Selenium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      446 2023-07-17 05:45:46.000000 Dock Py Selenium-2.0.0/Dock_Py_Selenium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 05:45:46.000000 Dock Py Selenium-2.0.0/Dock_Py_Selenium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-17 05:45:46.000000 Dock Py Selenium-2.0.0/Dock_Py_Selenium.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-17 05:45:46.000000 Dock Py Selenium-2.0.0/Dock_Py_Selenium.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      497 2023-07-17 05:45:46.391916 Dock Py Selenium-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      963 2023-07-17 05:14:12.000000 Dock Py Selenium-2.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 05:45:46.322867 Dock Py Selenium-2.0.0/dock_py_selenium/
-drwxrwxrwx   0        0        0        0 2023-07-17 05:45:46.389219 Dock Py Selenium-2.0.0/dock_py_selenium/dock/
--rw-rw-rw-   0        0        0     5238 2023-07-17 05:41:54.000000 Dock Py Selenium-2.0.0/dock_py_selenium/dock/dock.py
--rw-rw-rw-   0        0        0       42 2023-07-17 05:45:46.394919 Dock Py Selenium-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0      703 2023-07-17 05:45:01.000000 Dock Py Selenium-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:56:48.209811 dock-py-selenium-2.0.1/
+drwxrwxrwx   0        0        0        0 2023-07-17 06:56:48.198835 dock-py-selenium-2.0.1/Dock_Py_Selenium.egg-info/
+-rw-rw-rw-   0        0        0      572 2023-07-17 06:56:47.000000 dock-py-selenium-2.0.1/Dock_Py_Selenium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      446 2023-07-17 06:56:47.000000 dock-py-selenium-2.0.1/Dock_Py_Selenium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 06:56:47.000000 dock-py-selenium-2.0.1/Dock_Py_Selenium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-17 06:56:47.000000 dock-py-selenium-2.0.1/Dock_Py_Selenium.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-17 06:56:47.000000 dock-py-selenium-2.0.1/Dock_Py_Selenium.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      572 2023-07-17 06:56:48.206820 dock-py-selenium-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      971 2023-07-17 05:59:50.000000 dock-py-selenium-2.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 06:56:48.146218 dock-py-selenium-2.0.1/dock_py_selenium/
+drwxrwxrwx   0        0        0        0 2023-07-17 06:56:48.203834 dock-py-selenium-2.0.1/dock_py_selenium/dock/
+-rw-rw-rw-   0        0        0     5252 2023-07-17 06:56:27.000000 dock-py-selenium-2.0.1/dock_py_selenium/dock/dock.py
+-rw-rw-rw-   0        0        0       42 2023-07-17 06:56:48.210808 dock-py-selenium-2.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      774 2023-07-17 05:51:06.000000 dock-py-selenium-2.0.1/setup.py
```

### Comparing `Dock Py Selenium-2.0.0/README.md` & `dock-py-selenium-2.0.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ## Python only
 
 This is a startup directory to write the selenium scripts in python along with some customization.
 
 ### Steps.
 1. `pip install dock-py-selenium`
 2. Create a `test.py` file in your root directory and write your test scripts.
-3. Always bind any selenium script with the instance.
+3. Always bind any selenium script with the created instance.
 
 
 ## Features
 
 1. Setting a custom wait time for the webdriver `test_instance.wait(5)`
 2. Settting the number of times a test should be performed `test_instance.rerun(3, lambda: run())`
 3. Getting the title of the page `test_instance.getTitle()`
```

### Comparing `Dock Py Selenium-2.0.0/dock_py_selenium/dock/dock.py` & `dock-py-selenium-2.0.1/dock_py_selenium/dock/dock.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import time
 from selenium import webdriver
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.common.by import By
 from selenium.common.exceptions import NoSuchElementException
 from selenium.webdriver.chrome.options import Options as ChromeOptions
 
@@ -23,102 +24,107 @@
         self.driver.get(getUrl)
 
     # Gets the title of a webpage
     def getTitle(self):
         print(self.driver.title)
     
     # Only checks button & input of type submit
-    def checkClick(self,element):
+    def checkClick(self, element):
         cur_url = self.driver.current_url
-        match element:
-            case "button":
-                try:
-                    elem = self.driver.find_element(By.XPATH,  "//button[@type='submit']")
-                    elem.click()
-                    new_url = self.driver.current_url
-                    if cur_url != new_url:
-                        print("The button is clickable.")
-                    else:
-                        print("The button is not clickable.")
-                except NoSuchElementException as err:
-                    print("Exception: "+ err.msg)
-                except err:
-                    print("Error: " + err.msg)
-            case "input":
-                try:
-                    elem = self.driver.find_element(By.XPATH, "//input[@type='submit']")
-                    elem.click()
-                    new_url = self.driver.current_url
-                    if cur_url != new_url:
-                        print("The button is clickable.")
-                    else:
-                        print("The button is not clickable.")
-                except NoSuchElementException as err:
-                    print("Exception: "+ err.msg)
-                except err:
-                    print("Error: " + err.msg)
-            case _:
-                print("None")
+
+        if element == "button":
+            try:
+                elem = self.driver.find_element(By.XPATH, "//button[@type='submit']")
+                return lambda: self._click_button(elem, cur_url)
+            except NoSuchElementException as err:
+                print("Exception: " + err.msg)
+        elif element == "input":
+            try:
+                elem = self.driver.find_element(By.XPATH, "//input[@type='submit']")
+                return lambda: self._click_button(elem, cur_url)
+            except NoSuchElementException as err:
+                print("Exception: " + err.msg)
+        else:
+            print("Invalid element.")
+
+    def _click_button(self, button, cur_url):
+        initial_page_source = self.driver.page_source
+        button.click()
+        time.sleep(5)
+        updated_page_source = self.driver.page_source
+        
+        if initial_page_source != updated_page_source:
+            print("The button is clickable.")
+        else:
+            print("The button is not clickable.")
 
     # Checks for the availability of an element in a page
     def checkElement(self,elem,i):
         match elem:
             case "ID":
                 try:
                     e = self.driver.find_element(By.ID, i)
                     print("The element with ID '" + i + "' is available.")
+                    return e
                 except NoSuchElementException as err:
                     print("Exception: " + err.msg)
             
             case "NAME":
                 try:
                     e = self.driver.find_element(By.NAME, i)
                     print("The element with name '" + i + "' is available.")
+                    return e
                 except NoSuchElementException as err:
                     print("Exception: " + err.msg)
             
             case "CLASS_NAME":
                 try:
                     e = self.driver.find_element(By.CLASS_NAME, i)
                     print("The element with class name '" + i + "' is available.")
+                    return e
                 except NoSuchElementException as err:
                     print("Exception: " + err.msg)
             
             case "TAG_NAME":
                 try:
                     e = self.driver.find_element(By.TAG_NAME, i)
                     print("The element with tag name '" + i + "' is available.")
+                    return e
                 except NoSuchElementException as err:
                     print("Exception: " + err.msg)
             
             case "LINK_TEXT":
                 try:
                     e = self.driver.find_element(By.LINK_TEXT, i)
                     print("The element with link text '" + i + "' is available.")
+                    return e
                 except NoSuchElementException as err:
                     print("Exception: " + err.msg)
             
             case "PARTIAL_LINK_TEXT":
                 try:
                     e = self.driver.find_element(By.PARTIAL_LINK_TEXT, i)
                     print("The element with partial link text '" + i + "' is available.")
+                    return e
                 except NoSuchElementException as err:
                     print("Exception: " + err.msg)
             
             case "CSS_SELECTOR":
                 try:
                     e = self.driver.find_element(By.CSS_SELECTOR, i)
                     print("The element with CSS selector '" + i + "' is available.")
+                    return e
                 except NoSuchElementException as err:
                     print("Exception: " + err.msg)
             
             case "XPATH":
                 try:
                     e = self.driver.find_element(By.XPATH, i)
                     print("The element with XPath '" + i + "' is available.")
+                    return e
                 except NoSuchElementException as err:
                     print("Exception: " + err.msg)
             
             case _:
                 print("Invalid element.")
```

### Comparing `Dock Py Selenium-2.0.0/setup.py` & `dock-py-selenium-2.0.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup
 
 setup(
-    name="Dock Py Selenium",
-    version="2.0.0",
+    name="dock-py-selenium",
+    version="2.0.1",
     author="Bishal Shrestha",
     author_email="iambstha@gmail.com",
     description="A startup / mockup folder for a selenium project with custom methods.",
-    long_description="",
+    long_description="# A startup / mockup folder for a selenium project with custom methods.",
     long_description_content_type="text/markdown",
     url="https://github.com/iambstha/dock-py-selenium",
     packages=["dock_py_selenium.dock"],
     install_requires=[
         "selenium",
     ],
     classifiers=[
```

