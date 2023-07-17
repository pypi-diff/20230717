# Comparing `tmp/AndroidTools-0.0.1.tar.gz` & `tmp/AndroidTools-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AndroidTools-0.0.1.tar", last modified: Sun Jul 16 09:28:24 2023, max compression
+gzip compressed data, was "AndroidTools-0.0.2.tar", last modified: Mon Jul 17 08:05:43 2023, max compression
```

## Comparing `AndroidTools-0.0.1.tar` & `AndroidTools-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2023-07-16 09:28:24.785032 AndroidTools-0.0.1/
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2023-07-16 09:28:24.782556 AndroidTools-0.0.1/AndTools/
--rw-r--r--   0 1a         (501) staff       (20)     2336 2023-07-16 09:25:00.000000 AndroidTools-0.0.1/AndTools/Pack.py
--rw-r--r--   0 1a         (501) staff       (20)     9323 2023-06-29 11:17:00.000000 AndroidTools-0.0.1/AndTools/TEA.py
--rw-r--r--   0 1a         (501) staff       (20)       75 2023-07-16 08:46:39.000000 AndroidTools-0.0.1/AndTools/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)      122 2023-07-16 08:20:14.000000 AndroidTools-0.0.1/AndTools/byte_.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2023-07-16 09:28:24.783281 AndroidTools-0.0.1/AndroidTools.egg-info/
--rw-r--r--   0 1a         (501) staff       (20)      639 2023-07-16 09:28:24.000000 AndroidTools-0.0.1/AndroidTools.egg-info/PKG-INFO
--rw-r--r--   0 1a         (501) staff       (20)      330 2023-07-16 09:28:24.000000 AndroidTools-0.0.1/AndroidTools.egg-info/SOURCES.txt
--rw-r--r--   0 1a         (501) staff       (20)        1 2023-07-16 09:28:24.000000 AndroidTools-0.0.1/AndroidTools.egg-info/dependency_links.txt
--rw-r--r--   0 1a         (501) staff       (20)       13 2023-07-16 09:28:24.000000 AndroidTools-0.0.1/AndroidTools.egg-info/top_level.txt
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2023-07-16 09:28:24.784387 AndroidTools-0.0.1/Jce/
--rw-r--r--   0 1a         (501) staff       (20)      115 2023-07-10 08:50:41.000000 AndroidTools-0.0.1/Jce/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     2191 2023-07-15 07:24:55.000000 AndroidTools-0.0.1/Jce/bytebuffer.py
--rw-r--r--   0 1a         (501) staff       (20)      193 2023-07-10 08:50:41.000000 AndroidTools-0.0.1/Jce/exception.py
--rw-r--r--   0 1a         (501) staff       (20)    11676 2023-07-16 08:28:14.000000 AndroidTools-0.0.1/Jce/stream.py
--rw-r--r--   0 1a         (501) staff       (20)     1725 2023-07-16 09:19:40.000000 AndroidTools-0.0.1/Jce/struct.py
--rw-r--r--   0 1a         (501) staff       (20)      639 2023-07-16 09:28:24.784908 AndroidTools-0.0.1/PKG-INFO
--rw-r--r--   0 1a         (501) staff       (20)      267 2023-07-16 09:28:20.000000 AndroidTools-0.0.1/README.md
--rw-r--r--   0 1a         (501) staff       (20)       38 2023-07-16 09:28:24.785078 AndroidTools-0.0.1/setup.cfg
--rw-r--r--   0 1a         (501) staff       (20)      622 2023-07-16 07:58:24.000000 AndroidTools-0.0.1/setup.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2023-07-16 09:28:24.784614 AndroidTools-0.0.1/test/
--rw-r--r--   0 1a         (501) staff       (20)      693 2023-07-16 08:31:43.000000 AndroidTools-0.0.1/test/test_Jce.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2023-07-17 08:05:43.101369 AndroidTools-0.0.2/
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2023-07-17 08:05:43.098825 AndroidTools-0.0.2/AndTools/
+-rw-r--r--   0 1a         (501) staff       (20)     2474 2023-07-17 07:35:22.000000 AndroidTools-0.0.2/AndTools/Pack.py
+-rw-r--r--   0 1a         (501) staff       (20)     9323 2023-06-29 11:17:00.000000 AndroidTools-0.0.2/AndTools/TEA.py
+-rw-r--r--   0 1a         (501) staff       (20)       75 2023-07-16 08:46:39.000000 AndroidTools-0.0.2/AndTools/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)      122 2023-07-16 08:20:14.000000 AndroidTools-0.0.2/AndTools/byte_.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2023-07-17 08:05:43.099585 AndroidTools-0.0.2/AndroidTools.egg-info/
+-rw-r--r--   0 1a         (501) staff       (20)      639 2023-07-17 08:05:43.000000 AndroidTools-0.0.2/AndroidTools.egg-info/PKG-INFO
+-rw-r--r--   0 1a         (501) staff       (20)      330 2023-07-17 08:05:43.000000 AndroidTools-0.0.2/AndroidTools.egg-info/SOURCES.txt
+-rw-r--r--   0 1a         (501) staff       (20)        1 2023-07-17 08:05:43.000000 AndroidTools-0.0.2/AndroidTools.egg-info/dependency_links.txt
+-rw-r--r--   0 1a         (501) staff       (20)       13 2023-07-17 08:05:43.000000 AndroidTools-0.0.2/AndroidTools.egg-info/top_level.txt
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2023-07-17 08:05:43.100711 AndroidTools-0.0.2/Jce/
+-rw-r--r--   0 1a         (501) staff       (20)      115 2023-07-10 08:50:41.000000 AndroidTools-0.0.2/Jce/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     2191 2023-07-15 07:24:55.000000 AndroidTools-0.0.2/Jce/bytebuffer.py
+-rw-r--r--   0 1a         (501) staff       (20)      193 2023-07-10 08:50:41.000000 AndroidTools-0.0.2/Jce/exception.py
+-rw-r--r--   0 1a         (501) staff       (20)    11676 2023-07-16 08:28:14.000000 AndroidTools-0.0.2/Jce/stream.py
+-rw-r--r--   0 1a         (501) staff       (20)     1725 2023-07-16 09:19:40.000000 AndroidTools-0.0.2/Jce/struct.py
+-rw-r--r--   0 1a         (501) staff       (20)      639 2023-07-17 08:05:43.101258 AndroidTools-0.0.2/PKG-INFO
+-rw-r--r--   0 1a         (501) staff       (20)      267 2023-07-16 09:28:20.000000 AndroidTools-0.0.2/README.md
+-rw-r--r--   0 1a         (501) staff       (20)       38 2023-07-17 08:05:43.101412 AndroidTools-0.0.2/setup.cfg
+-rw-r--r--   0 1a         (501) staff       (20)      622 2023-07-17 07:35:27.000000 AndroidTools-0.0.2/setup.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2023-07-17 08:05:43.100958 AndroidTools-0.0.2/test/
+-rw-r--r--   0 1a         (501) staff       (20)      693 2023-07-16 08:31:43.000000 AndroidTools-0.0.2/test/test_Jce.py
```

### Comparing `AndroidTools-0.0.1/AndTools/Pack.py` & `AndroidTools-0.0.2/AndTools/Pack.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,18 @@
     def __init__(self):
         self._bytes_data = bytearray()
 
     def add_bin(self, bytes_temp):
         if bytes_temp is not None:
             self._bytes_data.extend(bytes_temp)
 
+    def add_Hex(self, bytes_temp):
+        if bytes_temp is not None:
+            self._bytes_data.extend(bytearray.fromhex(bytes_temp))
+
     def add_bytes(self, bytes_temp):
         """字节或字节集"""
         if bytes_temp is not None:
             self._bytes_data.append(bytes_temp)
 
     def add_int(self, int_temp, length=4):
         """整数
```

### Comparing `AndroidTools-0.0.1/AndTools/TEA.py` & `AndroidTools-0.0.2/AndTools/TEA.py`

 * *Files identical despite different names*

### Comparing `AndroidTools-0.0.1/AndroidTools.egg-info/PKG-INFO` & `AndroidTools-0.0.2/AndroidTools.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AndroidTools
-Version: 0.0.1
+Version: 0.0.2
 Summary: Android Tools for Python
 Home-page: https://github.com/grayrail000/PyJce
 Author: 1a
 Author-email: grayrail1x3@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `AndroidTools-0.0.1/Jce/bytebuffer.py` & `AndroidTools-0.0.2/Jce/bytebuffer.py`

 * *Files identical despite different names*

### Comparing `AndroidTools-0.0.1/Jce/stream.py` & `AndroidTools-0.0.2/Jce/stream.py`

 * *Files identical despite different names*

### Comparing `AndroidTools-0.0.1/Jce/struct.py` & `AndroidTools-0.0.2/Jce/struct.py`

 * *Files identical despite different names*

### Comparing `AndroidTools-0.0.1/PKG-INFO` & `AndroidTools-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AndroidTools
-Version: 0.0.1
+Version: 0.0.2
 Summary: Android Tools for Python
 Home-page: https://github.com/grayrail000/PyJce
 Author: 1a
 Author-email: grayrail1x3@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `AndroidTools-0.0.1/setup.py` & `AndroidTools-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="AndroidTools",
-    version="0.0.1",
+    version="0.0.2",
     author="1a",
     author_email="grayrail1x3@gmail.com",
     description="Android Tools for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/grayrail000/PyJce",
     packages=setuptools.find_packages(),
```

### Comparing `AndroidTools-0.0.1/test/test_Jce.py` & `AndroidTools-0.0.2/test/test_Jce.py`

 * *Files identical despite different names*

