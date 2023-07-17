# Comparing `tmp/shinherpro-1.7.1.tar.gz` & `tmp/shinherpro-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shinherpro-1.7.1.tar", last modified: Wed Jul  5 13:38:01 2023, max compression
+gzip compressed data, was "shinherpro-1.7.3.tar", last modified: Mon Jul 17 12:11:31 2023, max compression
```

## Comparing `shinherpro-1.7.1.tar` & `shinherpro-1.7.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 13:38:01.758457 shinherpro-1.7.1/
--rw-rw-rw-   0        0        0      178 2023-07-05 13:38:01.758457 shinherpro-1.7.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-05 13:38:01.759454 shinherpro-1.7.1/setup.cfg
--rw-rw-rw-   0        0        0      785 2023-07-05 06:01:29.000000 shinherpro-1.7.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-05 13:38:01.747299 shinherpro-1.7.1/shinherpro/
--rw-rw-rw-   0        0        0    29020 2023-07-05 13:37:59.000000 shinherpro-1.7.1/shinherpro/TYAI.py
--rw-rw-rw-   0        0        0        0 2023-05-22 15:34:31.000000 shinherpro-1.7.1/shinherpro/__init__.py
--rw-rw-rw-   0        0        0     1421 2023-06-19 15:22:28.000000 shinherpro-1.7.1/shinherpro/chormeDriver.py
--rw-rw-rw-   0        0        0      547 2023-06-22 15:54:06.000000 shinherpro-1.7.1/shinherpro/logSave.py
--rw-rw-rw-   0        0        0     2127 2023-05-21 08:58:49.000000 shinherpro-1.7.1/shinherpro/vfcModel.py
-drwxrwxrwx   0        0        0        0 2023-07-05 13:38:01.757460 shinherpro-1.7.1/shinherpro.egg-info/
--rw-rw-rw-   0        0        0      178 2023-07-05 13:38:01.000000 shinherpro-1.7.1/shinherpro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-07-05 13:38:01.000000 shinherpro-1.7.1/shinherpro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 13:38:01.000000 shinherpro-1.7.1/shinherpro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2023-07-05 13:38:01.000000 shinherpro-1.7.1/shinherpro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-05 13:38:01.000000 shinherpro-1.7.1/shinherpro.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 12:11:31.072149 shinherpro-1.7.3/
+-rw-rw-rw-   0        0        0      178 2023-07-17 12:11:31.072149 shinherpro-1.7.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-17 12:11:31.072149 shinherpro-1.7.3/setup.cfg
+-rw-rw-rw-   0        0        0      785 2023-07-17 12:11:29.000000 shinherpro-1.7.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 12:11:31.052204 shinherpro-1.7.3/shinherpro/
+-rw-rw-rw-   0        0        0    29019 2023-07-17 11:43:49.000000 shinherpro-1.7.3/shinherpro/TYAI.py
+-rw-rw-rw-   0        0        0        0 2023-05-22 15:34:31.000000 shinherpro-1.7.3/shinherpro/__init__.py
+-rw-rw-rw-   0        0        0     1421 2023-06-19 15:22:28.000000 shinherpro-1.7.3/shinherpro/chormeDriver.py
+-rw-rw-rw-   0        0        0      547 2023-06-22 15:54:06.000000 shinherpro-1.7.3/shinherpro/logSave.py
+-rw-rw-rw-   0        0        0     3835 2023-07-17 12:01:19.000000 shinherpro-1.7.3/shinherpro/vfcModel.py
+drwxrwxrwx   0        0        0        0 2023-07-17 12:11:31.070156 shinherpro-1.7.3/shinherpro.egg-info/
+-rw-rw-rw-   0        0        0      178 2023-07-17 12:11:30.000000 shinherpro-1.7.3/shinherpro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2023-07-17 12:11:30.000000 shinherpro-1.7.3/shinherpro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 12:11:30.000000 shinherpro-1.7.3/shinherpro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2023-07-17 12:11:30.000000 shinherpro-1.7.3/shinherpro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-17 12:11:30.000000 shinherpro-1.7.3/shinherpro.egg-info/top_level.txt
```

### Comparing `shinherpro-1.7.1/setup.py` & `shinherpro-1.7.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
     def run(self):
         print("\033[98m 正在安裝shinher-pro...")
         install.run(self)
         print("shinherpro安裝完成！ \033[0m")
 
 setup(
     name='shinherpro',
-    version='1.7.1',
-    description='shinher-pro 1.7.1',
+    version='1.7.3',
+    description='shinher-pro 1.7.3',
     author='Yihuan',
     author_email='ivan17.lai@gmail.com',
     packages=['shinherpro'],
     install_requires=[
         'selenium',
         'beautifulsoup4',
         'keras',
```

### Comparing `shinherpro-1.7.1/shinherpro/TYAI.py` & `shinherpro-1.7.3/shinherpro/TYAI.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from shinherpro import vfcModel
 from shinherpro import chormeDriver
 from shinherpro import logSave
 import sys
 
 
 ###################################################
-# V 1.7.0 By Yihuan --> 2023/6/25
+# V 1.7.1 By Yihuan --> 2023/7/7
 
 RESET = "\033[0m"
 RED = "\033[31m"
 GREEN = "\033[32m"
 YELLOW = "\033[33m"
 
 global UserNameSave
```

### Comparing `shinherpro-1.7.1/shinherpro/chormeDriver.py` & `shinherpro-1.7.3/shinherpro/chormeDriver.py`

 * *Files identical despite different names*

### Comparing `shinherpro-1.7.1/shinherpro/logSave.py` & `shinherpro-1.7.3/shinherpro/logSave.py`

 * *Files identical despite different names*

