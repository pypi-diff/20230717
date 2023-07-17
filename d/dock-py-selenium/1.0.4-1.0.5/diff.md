# Comparing `tmp/dock-py-selenium-1.0.4.tar.gz` & `tmp/dock-py-selenium-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dock-py-selenium-1.0.4.tar", last modified: Mon Jul 17 05:27:08 2023, max compression
+gzip compressed data, was "dock-py-selenium-1.0.5.tar", last modified: Mon Jul 17 05:35:38 2023, max compression
```

## Comparing `dock-py-selenium-1.0.4.tar` & `dock-py-selenium-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 05:27:08.384808 dock-py-selenium-1.0.4/
--rw-rw-rw-   0        0        0      656 2023-07-17 05:27:08.382812 dock-py-selenium-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      963 2023-07-17 05:14:12.000000 dock-py-selenium-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 05:27:08.304023 dock-py-selenium-1.0.4/dock_py_selenium/
-drwxrwxrwx   0        0        0        0 2023-07-17 05:27:08.379820 dock-py-selenium-1.0.4/dock_py_selenium/dock/
--rw-rw-rw-   0        0        0     5138 2023-07-17 05:04:43.000000 dock-py-selenium-1.0.4/dock_py_selenium/dock/dock.py
-drwxrwxrwx   0        0        0        0 2023-07-17 05:27:08.376829 dock-py-selenium-1.0.4/dock_py_selenium.egg-info/
--rw-rw-rw-   0        0        0      656 2023-07-17 05:27:08.000000 dock-py-selenium-1.0.4/dock_py_selenium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      247 2023-07-17 05:27:08.000000 dock-py-selenium-1.0.4/dock_py_selenium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 05:27:08.000000 dock-py-selenium-1.0.4/dock_py_selenium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-17 05:27:08.000000 dock-py-selenium-1.0.4/dock_py_selenium.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-17 05:27:08.000000 dock-py-selenium-1.0.4/dock_py_selenium.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-17 05:27:08.384808 dock-py-selenium-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      859 2023-07-17 05:26:55.000000 dock-py-selenium-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 05:35:38.083231 dock-py-selenium-1.0.5/
+-rw-rw-rw-   0        0        0      497 2023-07-17 05:35:38.081237 dock-py-selenium-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      963 2023-07-17 05:14:12.000000 dock-py-selenium-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 05:35:38.007258 dock-py-selenium-1.0.5/dock_py_selenium/
+drwxrwxrwx   0        0        0        0 2023-07-17 05:35:38.079254 dock-py-selenium-1.0.5/dock_py_selenium/dock/
+-rw-rw-rw-   0        0        0     5238 2023-07-17 05:35:31.000000 dock-py-selenium-1.0.5/dock_py_selenium/dock/dock.py
+drwxrwxrwx   0        0        0        0 2023-07-17 05:35:38.074257 dock-py-selenium-1.0.5/dock_py_selenium.egg-info/
+-rw-rw-rw-   0        0        0      497 2023-07-17 05:35:37.000000 dock-py-selenium-1.0.5/dock_py_selenium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      247 2023-07-17 05:35:37.000000 dock-py-selenium-1.0.5/dock_py_selenium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 05:35:37.000000 dock-py-selenium-1.0.5/dock_py_selenium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-17 05:35:37.000000 dock-py-selenium-1.0.5/dock_py_selenium.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-17 05:35:37.000000 dock-py-selenium-1.0.5/dock_py_selenium.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 05:35:38.083231 dock-py-selenium-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      703 2023-07-17 05:29:25.000000 dock-py-selenium-1.0.5/setup.py
```

### Comparing `dock-py-selenium-1.0.4/README.md` & `dock-py-selenium-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `dock-py-selenium-1.0.4/dock_py_selenium/dock/dock.py` & `dock-py-selenium-1.0.5/dock_py_selenium/dock/dock.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 driver.maximize_window
 
 class Driver:
     # Initialized with driver
     def __init__(self, driver):
         self.driver = driver
 
+    def start(self):
+        getUrl = input("Enter the url: ")
+        self.driver.get(getUrl)
+
     # Gets the title of a webpage
     def getTitle(self):
         print(self.driver.title)
     
     # Only checks button & input of type submit
     def checkClick(self,element):
         cur_url = self.driver.current_url
```

### Comparing `dock-py-selenium-1.0.4/setup.py` & `dock-py-selenium-1.0.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 from setuptools import setup
 
 setup(
     name="dock-py-selenium",
-    version="1.0.4",
+    version="1.0.5",
     author="Bishal Shrestha",
     author_email="iambstha@gmail.com",
     description="A startup / mockup folder for a selenium project with custom methods.",
     long_description="",
     long_description_content_type="text/markdown",
     url="https://github.com/iambstha/dock-py-selenium",
     packages=["dock_py_selenium.dock"],
     install_requires=[
         "selenium",
     ],
     classifiers=[
-        "Development Status :: 5 - Production/Stable",
+        "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
     ],
 )
```

