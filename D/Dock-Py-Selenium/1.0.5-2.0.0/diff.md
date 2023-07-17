# Comparing `tmp/dock-py-selenium-1.0.5.tar.gz` & `tmp/Dock Py Selenium-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dock-py-selenium-1.0.5.tar", last modified: Mon Jul 17 05:35:38 2023, max compression
+gzip compressed data, was "Dock Py Selenium-2.0.0.tar", last modified: Mon Jul 17 05:45:46 2023, max compression
```

## Comparing `dock-py-selenium-1.0.5.tar` & `Dock Py Selenium-2.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 05:35:38.083231 dock-py-selenium-1.0.5/
--rw-rw-rw-   0        0        0      497 2023-07-17 05:35:38.081237 dock-py-selenium-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      963 2023-07-17 05:14:12.000000 dock-py-selenium-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 05:35:38.007258 dock-py-selenium-1.0.5/dock_py_selenium/
-drwxrwxrwx   0        0        0        0 2023-07-17 05:35:38.079254 dock-py-selenium-1.0.5/dock_py_selenium/dock/
--rw-rw-rw-   0        0        0     5238 2023-07-17 05:35:31.000000 dock-py-selenium-1.0.5/dock_py_selenium/dock/dock.py
-drwxrwxrwx   0        0        0        0 2023-07-17 05:35:38.074257 dock-py-selenium-1.0.5/dock_py_selenium.egg-info/
--rw-rw-rw-   0        0        0      497 2023-07-17 05:35:37.000000 dock-py-selenium-1.0.5/dock_py_selenium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      247 2023-07-17 05:35:37.000000 dock-py-selenium-1.0.5/dock_py_selenium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 05:35:37.000000 dock-py-selenium-1.0.5/dock_py_selenium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-17 05:35:37.000000 dock-py-selenium-1.0.5/dock_py_selenium.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-17 05:35:37.000000 dock-py-selenium-1.0.5/dock_py_selenium.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-17 05:35:38.083231 dock-py-selenium-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      703 2023-07-17 05:29:25.000000 dock-py-selenium-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 05:45:46.392917 Dock Py Selenium-2.0.0/
+drwxrwxrwx   0        0        0        0 2023-07-17 05:45:46.383226 Dock Py Selenium-2.0.0/Dock_Py_Selenium.egg-info/
+-rw-rw-rw-   0        0        0      497 2023-07-17 05:45:46.000000 Dock Py Selenium-2.0.0/Dock_Py_Selenium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      446 2023-07-17 05:45:46.000000 Dock Py Selenium-2.0.0/Dock_Py_Selenium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 05:45:46.000000 Dock Py Selenium-2.0.0/Dock_Py_Selenium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-17 05:45:46.000000 Dock Py Selenium-2.0.0/Dock_Py_Selenium.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-17 05:45:46.000000 Dock Py Selenium-2.0.0/Dock_Py_Selenium.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      497 2023-07-17 05:45:46.391916 Dock Py Selenium-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      963 2023-07-17 05:14:12.000000 Dock Py Selenium-2.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 05:45:46.322867 Dock Py Selenium-2.0.0/dock_py_selenium/
+drwxrwxrwx   0        0        0        0 2023-07-17 05:45:46.389219 Dock Py Selenium-2.0.0/dock_py_selenium/dock/
+-rw-rw-rw-   0        0        0     5238 2023-07-17 05:41:54.000000 Dock Py Selenium-2.0.0/dock_py_selenium/dock/dock.py
+-rw-rw-rw-   0        0        0       42 2023-07-17 05:45:46.394919 Dock Py Selenium-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      703 2023-07-17 05:45:01.000000 Dock Py Selenium-2.0.0/setup.py
```

### Comparing `dock-py-selenium-1.0.5/README.md` & `Dock Py Selenium-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `dock-py-selenium-1.0.5/dock_py_selenium/dock/dock.py` & `Dock Py Selenium-2.0.0/dock_py_selenium/dock/dock.py`

 * *Files identical despite different names*

### Comparing `dock-py-selenium-1.0.5/setup.py` & `Dock Py Selenium-2.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
-    name="dock-py-selenium",
-    version="1.0.5",
+    name="Dock Py Selenium",
+    version="2.0.0",
     author="Bishal Shrestha",
     author_email="iambstha@gmail.com",
     description="A startup / mockup folder for a selenium project with custom methods.",
     long_description="",
     long_description_content_type="text/markdown",
     url="https://github.com/iambstha/dock-py-selenium",
     packages=["dock_py_selenium.dock"],
```

