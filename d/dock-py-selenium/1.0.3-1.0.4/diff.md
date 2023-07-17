# Comparing `tmp/dock-py-selenium-1.0.3.tar.gz` & `tmp/dock-py-selenium-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dock-py-selenium-1.0.3.tar", last modified: Mon Jul 17 05:05:13 2023, max compression
+gzip compressed data, was "dock-py-selenium-1.0.4.tar", last modified: Mon Jul 17 05:27:08 2023, max compression
```

## Comparing `dock-py-selenium-1.0.3.tar` & `dock-py-selenium-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 05:05:13.724522 dock-py-selenium-1.0.3/
--rw-rw-rw-   0        0        0      652 2023-07-17 05:05:13.723528 dock-py-selenium-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1069 2023-07-17 03:34:17.000000 dock-py-selenium-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 05:05:13.649721 dock-py-selenium-1.0.3/dock_py_selenium/
-drwxrwxrwx   0        0        0        0 2023-07-17 05:05:13.720532 dock-py-selenium-1.0.3/dock_py_selenium/dock/
--rw-rw-rw-   0        0        0     5138 2023-07-17 05:04:43.000000 dock-py-selenium-1.0.3/dock_py_selenium/dock/dock.py
-drwxrwxrwx   0        0        0        0 2023-07-17 05:05:13.709562 dock-py-selenium-1.0.3/dock_py_selenium.egg-info/
--rw-rw-rw-   0        0        0      652 2023-07-17 05:05:13.000000 dock-py-selenium-1.0.3/dock_py_selenium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      247 2023-07-17 05:05:13.000000 dock-py-selenium-1.0.3/dock_py_selenium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 05:05:13.000000 dock-py-selenium-1.0.3/dock_py_selenium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-17 05:05:13.000000 dock-py-selenium-1.0.3/dock_py_selenium.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-17 05:05:13.000000 dock-py-selenium-1.0.3/dock_py_selenium.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-17 05:05:13.725519 dock-py-selenium-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      855 2023-07-17 05:05:07.000000 dock-py-selenium-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 05:27:08.384808 dock-py-selenium-1.0.4/
+-rw-rw-rw-   0        0        0      656 2023-07-17 05:27:08.382812 dock-py-selenium-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      963 2023-07-17 05:14:12.000000 dock-py-selenium-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 05:27:08.304023 dock-py-selenium-1.0.4/dock_py_selenium/
+drwxrwxrwx   0        0        0        0 2023-07-17 05:27:08.379820 dock-py-selenium-1.0.4/dock_py_selenium/dock/
+-rw-rw-rw-   0        0        0     5138 2023-07-17 05:04:43.000000 dock-py-selenium-1.0.4/dock_py_selenium/dock/dock.py
+drwxrwxrwx   0        0        0        0 2023-07-17 05:27:08.376829 dock-py-selenium-1.0.4/dock_py_selenium.egg-info/
+-rw-rw-rw-   0        0        0      656 2023-07-17 05:27:08.000000 dock-py-selenium-1.0.4/dock_py_selenium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      247 2023-07-17 05:27:08.000000 dock-py-selenium-1.0.4/dock_py_selenium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 05:27:08.000000 dock-py-selenium-1.0.4/dock_py_selenium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-17 05:27:08.000000 dock-py-selenium-1.0.4/dock_py_selenium.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-17 05:27:08.000000 dock-py-selenium-1.0.4/dock_py_selenium.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 05:27:08.384808 dock-py-selenium-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      859 2023-07-17 05:26:55.000000 dock-py-selenium-1.0.4/setup.py
```

### Comparing `dock-py-selenium-1.0.3/PKG-INFO` & `dock-py-selenium-1.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: dock-py-selenium
-Version: 1.0.3
+Version: 1.0.4
 Summary: A startup / mockup folder for a selenium project with custom methods.
-Home-page: https://github.com/iambstha/dockSelenium
+Home-page: https://github.com/iambstha/dock-py-selenium
 Author: Bishal Shrestha
 Author-email: iambstha@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `dock-py-selenium-1.0.3/README.md` & `dock-py-selenium-1.0.4/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # DOCK SELENIUM
 
 ## Python only
 
 This is a startup directory to write the selenium scripts in python along with some customization.
 
 ### Steps.
-1. Clone [this](https://github.com/iambstha/dockSelenium) repository.
-2. Edit `test_script.py`. To make changes, write selenium scripts inside the run function defination.
-3. Always bind any selenium script with `d` while writing test scripts. For example `driver.find_element()` should be written as `d.driver.find_element()`
+1. `pip install dock-py-selenium`
+2. Create a `test.py` file in your root directory and write your test scripts.
+3. Always bind any selenium script with the instance.
 
 
 ## Features
 
-1. Setting a custom wait time for the webdriver `test.wait(5)`
-2. Settting the number of times a test should be performed `test.rerun(3, lambda: run())`
-3. Getting the title of the page `test.getTitle()`
-4. Checking whether the button or input type submit is clickable `test.checkClick("button")` or `test.checkClick("input")`
-5. Checking the presence of an element in a webpage `test.checkElement("CLASS_NAME","container")`
+1. Setting a custom wait time for the webdriver `test_instance.wait(5)`
+2. Settting the number of times a test should be performed `test_instance.rerun(3, lambda: run())`
+3. Getting the title of the page `test_instance.getTitle()`
+4. Checking whether the button or input type submit is clickable `test_instance.checkClick("button")` or `test_instance.checkClick("input")`
+5. Checking the presence of an element in a webpage `test_instance.checkElement("CLASS_NAME","container")`
 
 
 <mark> Note that, this project is still experimental and hence does not support the full render wait time for any test actions. </mark>
```

### Comparing `dock-py-selenium-1.0.3/dock_py_selenium/dock/dock.py` & `dock-py-selenium-1.0.4/dock_py_selenium/dock/dock.py`

 * *Files identical despite different names*

### Comparing `dock-py-selenium-1.0.3/dock_py_selenium.egg-info/PKG-INFO` & `dock-py-selenium-1.0.4/dock_py_selenium.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: dock-py-selenium
-Version: 1.0.3
+Version: 1.0.4
 Summary: A startup / mockup folder for a selenium project with custom methods.
-Home-page: https://github.com/iambstha/dockSelenium
+Home-page: https://github.com/iambstha/dock-py-selenium
 Author: Bishal Shrestha
 Author-email: iambstha@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `dock-py-selenium-1.0.3/setup.py` & `dock-py-selenium-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup
 
 setup(
     name="dock-py-selenium",
-    version="1.0.3",
+    version="1.0.4",
     author="Bishal Shrestha",
     author_email="iambstha@gmail.com",
     description="A startup / mockup folder for a selenium project with custom methods.",
     long_description="",
     long_description_content_type="text/markdown",
-    url="https://github.com/iambstha/dockSelenium",
+    url="https://github.com/iambstha/dock-py-selenium",
     packages=["dock_py_selenium.dock"],
     install_requires=[
         "selenium",
     ],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
```

