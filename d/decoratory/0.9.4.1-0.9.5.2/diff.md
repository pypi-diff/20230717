# Comparing `tmp/decoratory-0.9.4.1.tar.gz` & `tmp/decoratory-0.9.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decoratory-0.9.4.1.tar", last modified: Fri Jul 14 13:27:17 2023, max compression
+gzip compressed data, was "decoratory-0.9.5.2.tar", last modified: Mon Jul 17 13:44:55 2023, max compression
```

## Comparing `decoratory-0.9.4.1.tar` & `decoratory-0.9.5.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 13:27:17.257698 decoratory-0.9.4.1/
--rw-rw-rw-   0        0        0     1252 2023-06-27 11:25:14.000000 decoratory-0.9.4.1/License.txt
--rw-rw-rw-   0        0        0    48647 2023-07-14 13:27:17.257698 decoratory-0.9.4.1/PKG-INFO
--rw-rw-rw-   0        0        0    46898 2023-07-14 13:26:41.000000 decoratory-0.9.4.1/Readme.rst
--rw-rw-rw-   0        0        0        0 2023-06-23 16:09:56.000000 decoratory-0.9.4.1/Requirements.txt
-drwxrwxrwx   0        0        0        0 2023-07-14 13:27:16.710690 decoratory-0.9.4.1/Sources/
-drwxrwxrwx   0        0        0        0 2023-07-14 13:27:16.960653 decoratory-0.9.4.1/Sources/decoratory/
--rw-rw-rw-   0        0        0      249 2023-07-04 05:40:20.000000 decoratory-0.9.4.1/Sources/decoratory/__init__.py
--rw-rw-rw-   0        0        0     7623 2023-07-14 13:26:41.000000 decoratory-0.9.4.1/Sources/decoratory/__main__.py
--rw-rw-rw-   0        0        0     5889 2023-07-14 13:26:41.000000 decoratory-0.9.4.1/Sources/decoratory/banner.py
--rw-rw-rw-   0        0        0    19690 2023-07-14 13:26:41.000000 decoratory-0.9.4.1/Sources/decoratory/basic.py
--rw-rw-rw-   0        0        0    12426 2023-07-14 13:26:42.000000 decoratory-0.9.4.1/Sources/decoratory/multiton.py
--rw-rw-rw-   0        0        0    36916 2023-07-14 13:26:42.000000 decoratory-0.9.4.1/Sources/decoratory/observer.py
--rw-rw-rw-   0        0        0     8007 2023-07-14 13:26:42.000000 decoratory-0.9.4.1/Sources/decoratory/singleton.py
--rw-rw-rw-   0        0        0    10867 2023-07-14 13:26:42.000000 decoratory-0.9.4.1/Sources/decoratory/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-07-14 13:27:17.007527 decoratory-0.9.4.1/Sources/decoratory.egg-info/
--rw-rw-rw-   0        0        0    48647 2023-07-14 13:27:16.000000 decoratory-0.9.4.1/Sources/decoratory.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      586 2023-07-14 13:27:16.000000 decoratory-0.9.4.1/Sources/decoratory.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 13:27:16.000000 decoratory-0.9.4.1/Sources/decoratory.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-07-14 13:27:16.000000 decoratory-0.9.4.1/Sources/decoratory.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-14 13:27:17.210815 decoratory-0.9.4.1/Unittest/
--rw-rw-rw-   0        0        0    29042 2023-07-14 13:26:42.000000 decoratory-0.9.4.1/Unittest/test_basic.py
--rw-rw-rw-   0        0        0    23868 2023-07-14 13:26:42.000000 decoratory-0.9.4.1/Unittest/test_multiton.py
--rw-rw-rw-   0        0        0    40117 2023-07-14 13:26:42.000000 decoratory-0.9.4.1/Unittest/test_observer.py
--rw-rw-rw-   0        0        0    10739 2023-07-14 13:26:42.000000 decoratory-0.9.4.1/Unittest/test_singleton.py
--rw-rw-rw-   0        0        0    10203 2023-07-14 13:26:42.000000 decoratory-0.9.4.1/Unittest/test_wrapper.py
--rw-rw-rw-   0        0        0       42 2023-07-14 13:27:17.257698 decoratory-0.9.4.1/setup.cfg
--rw-rw-rw-   0        0        0     4668 2023-07-14 13:26:42.000000 decoratory-0.9.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 13:44:55.174665 decoratory-0.9.5.2/
+-rw-rw-rw-   0        0        0     1257 2023-07-15 14:55:02.000000 decoratory-0.9.5.2/License.txt
+-rw-rw-rw-   0        0        0    48567 2023-07-17 13:44:55.174665 decoratory-0.9.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0    46870 2023-07-17 13:43:02.000000 decoratory-0.9.5.2/Readme.rst
+-rw-rw-rw-   0        0        0        0 2023-06-23 16:09:56.000000 decoratory-0.9.5.2/Requirements.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 13:44:55.121293 decoratory-0.9.5.2/Sources/
+drwxrwxrwx   0        0        0        0 2023-07-17 13:44:55.152533 decoratory-0.9.5.2/Sources/decoratory/
+-rw-rw-rw-   0        0        0      249 2023-07-04 05:40:20.000000 decoratory-0.9.5.2/Sources/decoratory/__init__.py
+-rw-rw-rw-   0        0        0     7627 2023-07-17 13:44:21.000000 decoratory-0.9.5.2/Sources/decoratory/__main__.py
+-rw-rw-rw-   0        0        0     5893 2023-07-17 13:43:02.000000 decoratory-0.9.5.2/Sources/decoratory/banner.py
+-rw-rw-rw-   0        0        0    19694 2023-07-17 13:43:02.000000 decoratory-0.9.5.2/Sources/decoratory/basic.py
+-rw-rw-rw-   0        0        0    12430 2023-07-17 13:43:02.000000 decoratory-0.9.5.2/Sources/decoratory/multiton.py
+-rw-rw-rw-   0        0        0    36920 2023-07-17 13:43:02.000000 decoratory-0.9.5.2/Sources/decoratory/observer.py
+-rw-rw-rw-   0        0        0     8011 2023-07-17 13:43:02.000000 decoratory-0.9.5.2/Sources/decoratory/singleton.py
+-rw-rw-rw-   0        0        0    10871 2023-07-17 13:43:03.000000 decoratory-0.9.5.2/Sources/decoratory/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-07-17 13:44:55.168157 decoratory-0.9.5.2/Sources/decoratory.egg-info/
+-rw-rw-rw-   0        0        0    48567 2023-07-17 13:44:55.000000 decoratory-0.9.5.2/Sources/decoratory.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      586 2023-07-17 13:44:55.000000 decoratory-0.9.5.2/Sources/decoratory.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 13:44:55.000000 decoratory-0.9.5.2/Sources/decoratory.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-07-17 13:44:55.000000 decoratory-0.9.5.2/Sources/decoratory.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 13:44:55.174665 decoratory-0.9.5.2/Unittest/
+-rw-rw-rw-   0        0        0    29046 2023-07-17 13:43:03.000000 decoratory-0.9.5.2/Unittest/test_basic.py
+-rw-rw-rw-   0        0        0    23872 2023-07-17 13:43:03.000000 decoratory-0.9.5.2/Unittest/test_multiton.py
+-rw-rw-rw-   0        0        0    40121 2023-07-17 13:43:03.000000 decoratory-0.9.5.2/Unittest/test_observer.py
+-rw-rw-rw-   0        0        0    10743 2023-07-17 13:43:03.000000 decoratory-0.9.5.2/Unittest/test_singleton.py
+-rw-rw-rw-   0        0        0    10207 2023-07-17 13:43:03.000000 decoratory-0.9.5.2/Unittest/test_wrapper.py
+-rw-rw-rw-   0        0        0       42 2023-07-17 13:44:55.190319 decoratory-0.9.5.2/setup.cfg
+-rw-rw-rw-   0        0        0     4715 2023-07-17 13:44:21.000000 decoratory-0.9.5.2/setup.py
```

### Comparing `decoratory-0.9.4.1/License.txt` & `decoratory-0.9.5.2/License.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ===============================================================================
 MIT License
 ===============================================================================
 
-Copyright (c) 2023, Martin Abel
+Copyright (c) 2020-2023, Martin Abel
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `decoratory-0.9.4.1/PKG-INFO` & `decoratory-0.9.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: decoratory
-Version: 0.9.4.1
+Version: 0.9.5.2
 Summary: Decorators: Singleton, Multiton, Observer, Observable, generic Wrapper.
-Home-page: http://evation.eu/decoratory/index.html
-Download-URL: http://evation.eu/decoratory/Section/Download.html
+Home-page: http://evation.eu/index.html
+Download-URL: http://evation.eu/Section/Download.html
 Author: Martin Abel
 Author-email: Martin Abel <python@evation.eu>
 Maintainer: Martin Abel
 Maintainer-email: Martin Abel <python@evation.eu>
 License: MIT
-Project-URL: Projekt, http://evation.eu/decoratory/index.html
-Project-URL: Release Notes, http://evation.eu/decoratory/Section/ReleaseNotes.html
-Project-URL: Download, http://evation.eu/decoratory/Section/Download.html
+Project-URL: Projekt, http://decoratory.de/index.html
+Project-URL: Release Notes, http://evation.eu/Section/ReleaseNotes.html
+Project-URL: Download, http://evation.eu/Section/Download.html
 Keywords: decorator singleton multiton observer observable wrapper
 Platform: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
@@ -46,20 +46,20 @@
     __title__ = "Readme"
     __module__ = "Readme.rst"
     __author__ = "Martin Abel"
     __maintainer__ = "Martin Abel"
     __credits__ = ["Martin Abel"]
     __company__ = "eVation"
     __email__ = "python@evation.eu"
-    __url__ = "http://evation.eu/decoratory"
-    __copyright__ = f"(c) copyright 2020-2023, {__author__}"
+    __url__ = "http://evation.eu"
+    __copyright__ = f"(c) copyright 2020-2023, {__author__}, {__company__}"
     __created__ = "2020-01-01"
-    __version__ = "0.9.4.1"
-    __date__ = "2023-07-14"
-    __time__ = "15:26:41"
+    __version__ = "0.9.5.1"
+    __date__ = "2023-07-17"
+    __time__ = "15:43:02"
     __state__ = "Beta"
     __license__ = "MIT"
     --------------------------------------------------------------------------
 
 
 ==============================================================================
 Decoratory
@@ -1174,14 +1174,14 @@
 However, it bears the risk of losing track of all dependencies.
 
 
 ~~~ `contents <#toc>`_ ~~~ `singleton`_ ~~~ `multiton`_ ~~~ `wrapper`_ ~~~ `observer`_ ~~~
 
 
 .. ===========================================================================
-.. _project homepage: http://evation.eu/decoratory
+.. _project homepage: http://evation.eu/
 .. _singleton pattern: https://en.wikipedia.org/wiki/Singleton_pattern
 .. _multiton pattern: https://en.wikipedia.org/wiki/Multiton_pattern
 .. _observer pattern: https://en.wikipedia.org/wiki/Observer_pattern
-.. _Decorator Arguments Template: http://evation.eu/decoratory/Section/ArgumentsTemplate.html
-.. _Decorator Implementations: http://evation.eu/decoratory/Section/Decorators.html
+.. _Decorator Arguments Template: http://evation.eu/Section/ArgumentsTemplate.html
+.. _Decorator Implementations: http://evation.eu/Section/Decorators.html
```

### Comparing `decoratory-0.9.4.1/Readme.rst` & `decoratory-0.9.5.2/Readme.rst`

 * *Files 0% similar despite different names*

```diff
@@ -7,20 +7,20 @@
     __title__ = "Readme"
     __module__ = "Readme.rst"
     __author__ = "Martin Abel"
     __maintainer__ = "Martin Abel"
     __credits__ = ["Martin Abel"]
     __company__ = "eVation"
     __email__ = "python@evation.eu"
-    __url__ = "http://evation.eu/decoratory"
-    __copyright__ = f"(c) copyright 2020-2023, {__author__}"
+    __url__ = "http://evation.eu"
+    __copyright__ = f"(c) copyright 2020-2023, {__author__}, {__company__}"
     __created__ = "2020-01-01"
-    __version__ = "0.9.4.1"
-    __date__ = "2023-07-14"
-    __time__ = "15:26:41"
+    __version__ = "0.9.5.1"
+    __date__ = "2023-07-17"
+    __time__ = "15:43:02"
     __state__ = "Beta"
     __license__ = "MIT"
     --------------------------------------------------------------------------
 
 
 ==============================================================================
 Decoratory
@@ -1135,14 +1135,14 @@
 However, it bears the risk of losing track of all dependencies.
 
 
 ~~~ `contents <#toc>`_ ~~~ `singleton`_ ~~~ `multiton`_ ~~~ `wrapper`_ ~~~ `observer`_ ~~~
 
 
 .. ===========================================================================
-.. _project homepage: http://evation.eu/decoratory
+.. _project homepage: http://evation.eu/
 .. _singleton pattern: https://en.wikipedia.org/wiki/Singleton_pattern
 .. _multiton pattern: https://en.wikipedia.org/wiki/Multiton_pattern
 .. _observer pattern: https://en.wikipedia.org/wiki/Observer_pattern
-.. _Decorator Arguments Template: http://evation.eu/decoratory/Section/ArgumentsTemplate.html
-.. _Decorator Implementations: http://evation.eu/decoratory/Section/Decorators.html
+.. _Decorator Arguments Template: http://evation.eu/Section/ArgumentsTemplate.html
+.. _Decorator Implementations: http://evation.eu/Section/Decorators.html
```

### Comparing `decoratory-0.9.4.1/Sources/decoratory/__main__.py` & `decoratory-0.9.5.2/Sources/decoratory/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 __title__ = "Decoratory"
 __module__ = "__main__.py"
 __author__ = "Martin Abel"
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
-__url__ = "http://evation.eu/decoratory"
-__copyright__ = f"(c) copyright 2020-2023, {__author__}"
+__url__ = "http://evation.eu"
+__copyright__ = f"(c) copyright 2020-2023, {__author__}, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.4.1"
-__date__ = "2023-07-14"
-__time__ = "15:26:41"
+__version__ = "0.9.5.2"
+__date__ = "2023-07-17"
+__time__ = "15:44:21"
 __state__ = "Beta"
 __license__ = "MIT"
 
 __all__ = ["get_file_location"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
```

### Comparing `decoratory-0.9.4.1/Sources/decoratory/banner.py` & `decoratory-0.9.5.2/Sources/decoratory/banner.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 __title__ = "Banner"
 __module__ = "banner.py"
 __author__ = "Martin Abel"
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
-__url__ = "http://evation.eu/decoratory"
-__copyright__ = f"(c) copyright 2020-2023, {__author__}"
+__url__ = "http://evation.eu"
+__copyright__ = f"(c) copyright 2020-2023, {__author__}, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.4.1"
-__date__ = "2023-07-14"
-__time__ = "15:26:41"
+__version__ = "0.9.5.1"
+__date__ = "2023-07-17"
+__time__ = "15:43:02"
 __state__ = "Beta"
 __license__ = "MIT"
 
 __all__ = ["__banner"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
```

### Comparing `decoratory-0.9.4.1/Sources/decoratory/basic.py` & `decoratory-0.9.5.2/Sources/decoratory/basic.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,20 +34,20 @@
 __title__ = "Basic"
 __module__ = "basic.py"
 __author__ = "Martin Abel"
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
-__url__ = "http://evation.eu/decoratory"
-__copyright__ = f"(c) copyright 2020-2023, {__author__}"
+__url__ = "http://evation.eu"
+__copyright__ = f"(c) copyright 2020-2023, {__author__}, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.4.1"
-__date__ = "2023-07-14"
-__time__ = "15:26:41"
+__version__ = "0.9.5.1"
+__date__ = "2023-07-17"
+__time__ = "15:43:02"
 __state__ = "Beta"
 __license__ = "MIT"
 
 __all__ = ["Activation", "Parser", "F", "X", "BaseDecorator"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
```

### Comparing `decoratory-0.9.4.1/Sources/decoratory/multiton.py` & `decoratory-0.9.5.2/Sources/decoratory/multiton.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,20 +122,20 @@
 __title__ = "Multiton"
 __module__ = "multiton.py"
 __author__ = "Martin Abel"
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
-__url__ = "http://evation.eu/decoratory"
-__copyright__ = f"(c) copyright 2020-2023, {__author__}"
+__url__ = "http://evation.eu"
+__copyright__ = f"(c) copyright 2020-2023, {__author__}, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.4.1"
-__date__ = "2023-07-14"
-__time__ = "15:26:41"
+__version__ = "0.9.5.1"
+__date__ = "2023-07-17"
+__time__ = "15:43:02"
 __state__ = "Beta"
 __license__ = "MIT"
 
 __all__ = ["Multiton"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
```

### Comparing `decoratory-0.9.4.1/Sources/decoratory/observer.py` & `decoratory-0.9.5.2/Sources/decoratory/observer.py`

 * *Files 0% similar despite different names*

```diff
@@ -404,20 +404,20 @@
 __title__ = "Observer"
 __module__ = "observer.py"
 __author__ = "Martin Abel"
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
-__url__ = "http://evation.eu/decoratory"
-__copyright__ = f"(c) copyright 2020-2023, {__author__}"
+__url__ = "http://evation.eu"
+__copyright__ = f"(c) copyright 2020-2023, {__author__}, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.4.1"
-__date__ = "2023-07-14"
-__time__ = "15:26:41"
+__version__ = "0.9.5.1"
+__date__ = "2023-07-17"
+__time__ = "15:43:02"
 __state__ = "Beta"
 __license__ = "MIT"
 
 __all__ = ["Observer", "BaseObserver", "Observable", "BaseObservable"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
```

### Comparing `decoratory-0.9.4.1/Sources/decoratory/singleton.py` & `decoratory-0.9.5.2/Sources/decoratory/singleton.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,20 +81,20 @@
 __title__ = "Singleton"
 __module__ = "singleton.py"
 __author__ = "Martin Abel"
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
-__url__ = "http://evation.eu/decoratory"
-__copyright__ = f"(c) copyright 2020-2023, {__author__}"
+__url__ = "http://evation.eu"
+__copyright__ = f"(c) copyright 2020-2023, {__author__}, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.4.1"
-__date__ = "2023-07-14"
-__time__ = "15:26:41"
+__version__ = "0.9.5.1"
+__date__ = "2023-07-17"
+__time__ = "15:43:02"
 __state__ = "Beta"
 __license__ = "MIT"
 
 __all__ = ["Singleton", "SemiSingleton"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
```

### Comparing `decoratory-0.9.4.1/Sources/decoratory/wrapper.py` & `decoratory-0.9.5.2/Sources/decoratory/wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,20 +133,20 @@
 __title__ = "Wrapper"
 __module__ = "wrapper.py"
 __author__ = "Martin Abel"
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
-__url__ = "http://evation.eu/decoratory"
-__copyright__ = f"(c) copyright 2020-2023, {__author__}"
+__url__ = "http://evation.eu"
+__copyright__ = f"(c) copyright 2020-2023, {__author__}, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.4.1"
-__date__ = "2023-07-14"
-__time__ = "15:26:41"
+__version__ = "0.9.5.1"
+__date__ = "2023-07-17"
+__time__ = "15:43:02"
 __state__ = "Beta"
 __license__ = "MIT"
 
 __all__ = ["Wrapper"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
```

### Comparing `decoratory-0.9.4.1/Sources/decoratory.egg-info/PKG-INFO` & `decoratory-0.9.5.2/Sources/decoratory.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: decoratory
-Version: 0.9.4.1
+Version: 0.9.5.2
 Summary: Decorators: Singleton, Multiton, Observer, Observable, generic Wrapper.
-Home-page: http://evation.eu/decoratory/index.html
-Download-URL: http://evation.eu/decoratory/Section/Download.html
+Home-page: http://evation.eu/index.html
+Download-URL: http://evation.eu/Section/Download.html
 Author: Martin Abel
 Author-email: Martin Abel <python@evation.eu>
 Maintainer: Martin Abel
 Maintainer-email: Martin Abel <python@evation.eu>
 License: MIT
-Project-URL: Projekt, http://evation.eu/decoratory/index.html
-Project-URL: Release Notes, http://evation.eu/decoratory/Section/ReleaseNotes.html
-Project-URL: Download, http://evation.eu/decoratory/Section/Download.html
+Project-URL: Projekt, http://decoratory.de/index.html
+Project-URL: Release Notes, http://evation.eu/Section/ReleaseNotes.html
+Project-URL: Download, http://evation.eu/Section/Download.html
 Keywords: decorator singleton multiton observer observable wrapper
 Platform: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
@@ -46,20 +46,20 @@
     __title__ = "Readme"
     __module__ = "Readme.rst"
     __author__ = "Martin Abel"
     __maintainer__ = "Martin Abel"
     __credits__ = ["Martin Abel"]
     __company__ = "eVation"
     __email__ = "python@evation.eu"
-    __url__ = "http://evation.eu/decoratory"
-    __copyright__ = f"(c) copyright 2020-2023, {__author__}"
+    __url__ = "http://evation.eu"
+    __copyright__ = f"(c) copyright 2020-2023, {__author__}, {__company__}"
     __created__ = "2020-01-01"
-    __version__ = "0.9.4.1"
-    __date__ = "2023-07-14"
-    __time__ = "15:26:41"
+    __version__ = "0.9.5.1"
+    __date__ = "2023-07-17"
+    __time__ = "15:43:02"
     __state__ = "Beta"
     __license__ = "MIT"
     --------------------------------------------------------------------------
 
 
 ==============================================================================
 Decoratory
@@ -1174,14 +1174,14 @@
 However, it bears the risk of losing track of all dependencies.
 
 
 ~~~ `contents <#toc>`_ ~~~ `singleton`_ ~~~ `multiton`_ ~~~ `wrapper`_ ~~~ `observer`_ ~~~
 
 
 .. ===========================================================================
-.. _project homepage: http://evation.eu/decoratory
+.. _project homepage: http://evation.eu/
 .. _singleton pattern: https://en.wikipedia.org/wiki/Singleton_pattern
 .. _multiton pattern: https://en.wikipedia.org/wiki/Multiton_pattern
 .. _observer pattern: https://en.wikipedia.org/wiki/Observer_pattern
-.. _Decorator Arguments Template: http://evation.eu/decoratory/Section/ArgumentsTemplate.html
-.. _Decorator Implementations: http://evation.eu/decoratory/Section/Decorators.html
+.. _Decorator Arguments Template: http://evation.eu/Section/ArgumentsTemplate.html
+.. _Decorator Implementations: http://evation.eu/Section/Decorators.html
```

### Comparing `decoratory-0.9.4.1/Sources/decoratory.egg-info/SOURCES.txt` & `decoratory-0.9.5.2/Sources/decoratory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `decoratory-0.9.4.1/Unittest/test_basic.py` & `decoratory-0.9.5.2/Unittest/test_basic.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 __title__ = "Test_Basic"
 __module__ = "test_basic.py"
 __author__ = "Martin Abel"
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
-__url__ = "http://evation.eu/decoratory"
-__copyright__ = f"(c) copyright 2020-2023, {__author__}"
+__url__ = "http://evation.eu"
+__copyright__ = f"(c) copyright 2020-2023, {__author__}, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.4.1"
-__date__ = "2023-07-14"
-__time__ = "15:26:41"
+__version__ = "0.9.5.1"
+__date__ = "2023-07-17"
+__time__ = "15:43:02"
 __state__ = "Beta"
 __license__ = "MIT"
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 import unittest
```

### Comparing `decoratory-0.9.4.1/Unittest/test_multiton.py` & `decoratory-0.9.5.2/Unittest/test_multiton.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 __title__ = "Test Multiton"
 __module__ = "test_multiton.py"
 __author__ = "Martin Abel"
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
-__url__ = "http://evation.eu/decoratory"
-__copyright__ = f"(c) copyright 2020-2023, {__author__}"
+__url__ = "http://evation.eu"
+__copyright__ = f"(c) copyright 2020-2023, {__author__}, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.4.1"
-__date__ = "2023-07-14"
-__time__ = "15:26:41"
+__version__ = "0.9.5.1"
+__date__ = "2023-07-17"
+__time__ = "15:43:02"
 __state__ = "Beta"
 __license__ = "MIT"
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 import unittest
```

### Comparing `decoratory-0.9.4.1/Unittest/test_observer.py` & `decoratory-0.9.5.2/Unittest/test_observer.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 __title__ = "Test Observer"
 __module__ = "test_observer.py"
 __author__ = "Martin Abel"
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
-__url__ = "http://evation.eu/decoratory"
-__copyright__ = f"(c) copyright 2020-2023, {__author__}"
+__url__ = "http://evation.eu"
+__copyright__ = f"(c) copyright 2020-2023, {__author__}, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.4.1"
-__date__ = "2023-07-14"
-__time__ = "15:26:41"
+__version__ = "0.9.5.1"
+__date__ = "2023-07-17"
+__time__ = "15:43:02"
 __state__ = "Beta"
 __license__ = "MIT"
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 import unittest
```

### Comparing `decoratory-0.9.4.1/Unittest/test_singleton.py` & `decoratory-0.9.5.2/Unittest/test_singleton.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 __title__ = "Test Singleton"
 __module__ = "test_singleton.py"
 __author__ = "Martin Abel"
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
-__url__ = "http://evation.eu/decoratory"
-__copyright__ = f"(c) copyright 2020-2023, {__author__}"
+__url__ = "http://evation.eu"
+__copyright__ = f"(c) copyright 2020-2023, {__author__}, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.4.1"
-__date__ = "2023-07-14"
-__time__ = "15:26:41"
+__version__ = "0.9.5.1"
+__date__ = "2023-07-17"
+__time__ = "15:43:02"
 __state__ = "Beta"
 __license__ = "MIT"
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 import unittest
```

### Comparing `decoratory-0.9.4.1/Unittest/test_wrapper.py` & `decoratory-0.9.5.2/Unittest/test_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 __title__ = "Test Wrapper"
 __module__ = "test_wrapper.py"
 __author__ = "Martin Abel"
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
-__url__ = "http://evation.eu/decoratory"
-__copyright__ = f"(c) copyright 2020-2023, {__author__}"
+__url__ = "http://evation.eu"
+__copyright__ = f"(c) copyright 2020-2023, {__author__}, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.4.1"
-__date__ = "2023-07-14"
-__time__ = "15:26:41"
+__version__ = "0.9.5.1"
+__date__ = "2023-07-17"
+__time__ = "15:43:02"
 __state__ = "Beta"
 __license__ = "MIT"
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 import unittest
```

### Comparing `decoratory-0.9.4.1/setup.py` & `decoratory-0.9.5.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 __title__ = "decoratory"
 __module__ = "setup.py"
 __author__ = "Martin Abel"
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
-__url__ = "http://evation.eu/decoratory"
-__copyright__ = f"(c) copyright 2020-2023, {__author__}"
+__url__ = "http://evation.eu"
+__copyright__ = f"(c) copyright 2020-2023, {__author__}, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.4.1"
-__date__ = "2023-07-14"
-__time__ = "15:26:41"
+__version__ = "0.9.5.2"
+__date__ = "2023-07-17"
+__time__ = "15:44:21"
 __state__ = "Beta"
 __license__ = "MIT"
 
 # -----------------------------------------------------------------------------
 # Libraries
 from os.path import join
 from setuptools import setup, find_packages
@@ -67,17 +67,19 @@
     url="/".join([__url__, "index.html"]),
     download_url="/".join([__url__, "Section", "Download.html"]),
     description=('Decorators: Singleton, Multiton, Observer, Observable, '
                  'generic Wrapper.'),
     long_description=description,
     long_description_content_type='text/x-rst',
     project_urls={
-        'Projekt': "/".join([__url__, "index.html"]),
-        'Release Notes': "/".join([__url__, "Section", "ReleaseNotes.html"]),
-        'Download': "/".join([__url__, "Section", "Download.html"])},
+        'Projekt': "/".join(["http://decoratory.de", "index.html"]),
+        'Release Notes': "/".join(
+            [__url__, "Section", "ReleaseNotes.html"]),
+        'Download': "/".join(
+            [__url__, "Section", "Download.html"])},
     keywords='decorator singleton multiton observer observable wrapper',
     # Technical
     license=__license__,
     platforms=['Operating System :: OS Independent'],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
```

