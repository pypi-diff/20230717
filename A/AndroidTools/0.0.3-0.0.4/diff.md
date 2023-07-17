# Comparing `tmp/AndroidTools-0.0.3.tar.gz` & `tmp/AndroidTools-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AndroidTools-0.0.3.tar", last modified: Mon Jul 17 08:28:41 2023, max compression
+gzip compressed data, was "AndroidTools-0.0.4.tar", last modified: Mon Jul 17 08:44:23 2023, max compression
```

## Comparing `AndroidTools-0.0.3.tar` & `AndroidTools-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2023-07-17 08:28:41.732102 AndroidTools-0.0.3/
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2023-07-17 08:28:41.730396 AndroidTools-0.0.3/AndTools/
--rw-r--r--   0 1a         (501) staff       (20)     2474 2023-07-17 07:35:22.000000 AndroidTools-0.0.3/AndTools/Pack.py
--rw-r--r--   0 1a         (501) staff       (20)     9323 2023-06-29 11:17:00.000000 AndroidTools-0.0.3/AndTools/TEA.py
--rw-r--r--   0 1a         (501) staff       (20)       75 2023-07-16 08:46:39.000000 AndroidTools-0.0.3/AndTools/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)      269 2023-07-17 08:24:35.000000 AndroidTools-0.0.3/AndTools/byte_.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2023-07-17 08:28:41.730919 AndroidTools-0.0.3/AndroidTools.egg-info/
--rw-r--r--   0 1a         (501) staff       (20)      639 2023-07-17 08:28:41.000000 AndroidTools-0.0.3/AndroidTools.egg-info/PKG-INFO
--rw-r--r--   0 1a         (501) staff       (20)      330 2023-07-17 08:28:41.000000 AndroidTools-0.0.3/AndroidTools.egg-info/SOURCES.txt
--rw-r--r--   0 1a         (501) staff       (20)        1 2023-07-17 08:28:41.000000 AndroidTools-0.0.3/AndroidTools.egg-info/dependency_links.txt
--rw-r--r--   0 1a         (501) staff       (20)       13 2023-07-17 08:28:41.000000 AndroidTools-0.0.3/AndroidTools.egg-info/top_level.txt
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2023-07-17 08:28:41.731518 AndroidTools-0.0.3/Jce/
--rw-r--r--   0 1a         (501) staff       (20)      115 2023-07-10 08:50:41.000000 AndroidTools-0.0.3/Jce/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     2191 2023-07-15 07:24:55.000000 AndroidTools-0.0.3/Jce/bytebuffer.py
--rw-r--r--   0 1a         (501) staff       (20)      193 2023-07-10 08:50:41.000000 AndroidTools-0.0.3/Jce/exception.py
--rw-r--r--   0 1a         (501) staff       (20)    11676 2023-07-16 08:28:14.000000 AndroidTools-0.0.3/Jce/stream.py
--rw-r--r--   0 1a         (501) staff       (20)     1725 2023-07-16 09:19:40.000000 AndroidTools-0.0.3/Jce/struct.py
--rw-r--r--   0 1a         (501) staff       (20)      639 2023-07-17 08:28:41.731981 AndroidTools-0.0.3/PKG-INFO
--rw-r--r--   0 1a         (501) staff       (20)      267 2023-07-16 09:28:20.000000 AndroidTools-0.0.3/README.md
--rw-r--r--   0 1a         (501) staff       (20)       38 2023-07-17 08:28:41.732147 AndroidTools-0.0.3/setup.cfg
--rw-r--r--   0 1a         (501) staff       (20)      622 2023-07-17 08:24:44.000000 AndroidTools-0.0.3/setup.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2023-07-17 08:28:41.731626 AndroidTools-0.0.3/test/
--rw-r--r--   0 1a         (501) staff       (20)      693 2023-07-16 08:31:43.000000 AndroidTools-0.0.3/test/test_Jce.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2023-07-17 08:44:23.156555 AndroidTools-0.0.4/
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2023-07-17 08:44:23.154154 AndroidTools-0.0.4/AndTools/
+-rw-r--r--   0 1a         (501) staff       (20)     2480 2023-07-17 08:44:13.000000 AndroidTools-0.0.4/AndTools/Pack.py
+-rw-r--r--   0 1a         (501) staff       (20)     9323 2023-06-29 11:17:00.000000 AndroidTools-0.0.4/AndTools/TEA.py
+-rw-r--r--   0 1a         (501) staff       (20)       75 2023-07-16 08:46:39.000000 AndroidTools-0.0.4/AndTools/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)      269 2023-07-17 08:24:35.000000 AndroidTools-0.0.4/AndTools/byte_.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2023-07-17 08:44:23.154797 AndroidTools-0.0.4/AndroidTools.egg-info/
+-rw-r--r--   0 1a         (501) staff       (20)      639 2023-07-17 08:44:23.000000 AndroidTools-0.0.4/AndroidTools.egg-info/PKG-INFO
+-rw-r--r--   0 1a         (501) staff       (20)      330 2023-07-17 08:44:23.000000 AndroidTools-0.0.4/AndroidTools.egg-info/SOURCES.txt
+-rw-r--r--   0 1a         (501) staff       (20)        1 2023-07-17 08:44:23.000000 AndroidTools-0.0.4/AndroidTools.egg-info/dependency_links.txt
+-rw-r--r--   0 1a         (501) staff       (20)       13 2023-07-17 08:44:23.000000 AndroidTools-0.0.4/AndroidTools.egg-info/top_level.txt
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2023-07-17 08:44:23.155880 AndroidTools-0.0.4/Jce/
+-rw-r--r--   0 1a         (501) staff       (20)      115 2023-07-10 08:50:41.000000 AndroidTools-0.0.4/Jce/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     2191 2023-07-15 07:24:55.000000 AndroidTools-0.0.4/Jce/bytebuffer.py
+-rw-r--r--   0 1a         (501) staff       (20)      193 2023-07-10 08:50:41.000000 AndroidTools-0.0.4/Jce/exception.py
+-rw-r--r--   0 1a         (501) staff       (20)    11676 2023-07-16 08:28:14.000000 AndroidTools-0.0.4/Jce/stream.py
+-rw-r--r--   0 1a         (501) staff       (20)     1725 2023-07-16 09:19:40.000000 AndroidTools-0.0.4/Jce/struct.py
+-rw-r--r--   0 1a         (501) staff       (20)      639 2023-07-17 08:44:23.156414 AndroidTools-0.0.4/PKG-INFO
+-rw-r--r--   0 1a         (501) staff       (20)      267 2023-07-16 09:28:20.000000 AndroidTools-0.0.4/README.md
+-rw-r--r--   0 1a         (501) staff       (20)       38 2023-07-17 08:44:23.156605 AndroidTools-0.0.4/setup.cfg
+-rw-r--r--   0 1a         (501) staff       (20)      622 2023-07-17 08:44:19.000000 AndroidTools-0.0.4/setup.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2023-07-17 08:44:23.156104 AndroidTools-0.0.4/test/
+-rw-r--r--   0 1a         (501) staff       (20)      693 2023-07-16 08:31:43.000000 AndroidTools-0.0.4/test/test_Jce.py
```

### Comparing `AndroidTools-0.0.3/AndTools/Pack.py` & `AndroidTools-0.0.4/AndTools/Pack.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,14 @@
             self._bytes_data.extend(int_temp.to_bytes(length, 'big'))
 
     def set_data(self, byte_temp):
         """置数据"""
         if byte_temp is not None:
             self._bytes_data = byte_temp
 
-    def get_bytes(self, Hex):
+    def get_bytes(self, Hex=False):
         if Hex:
             _bytes_temp = self._bytes_data.hex()
             _bytes_temp = hexFormat(_bytes_temp)
         else:
             _bytes_temp = self._bytes_data
         return _bytes_temp
```

### Comparing `AndroidTools-0.0.3/AndTools/TEA.py` & `AndroidTools-0.0.4/AndTools/TEA.py`

 * *Files identical despite different names*

### Comparing `AndroidTools-0.0.3/AndroidTools.egg-info/PKG-INFO` & `AndroidTools-0.0.4/AndroidTools.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AndroidTools
-Version: 0.0.3
+Version: 0.0.4
 Summary: Android Tools for Python
 Home-page: https://github.com/grayrail000/PyJce
 Author: 1a
 Author-email: grayrail1x3@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `AndroidTools-0.0.3/Jce/bytebuffer.py` & `AndroidTools-0.0.4/Jce/bytebuffer.py`

 * *Files identical despite different names*

### Comparing `AndroidTools-0.0.3/Jce/stream.py` & `AndroidTools-0.0.4/Jce/stream.py`

 * *Files identical despite different names*

### Comparing `AndroidTools-0.0.3/Jce/struct.py` & `AndroidTools-0.0.4/Jce/struct.py`

 * *Files identical despite different names*

### Comparing `AndroidTools-0.0.3/PKG-INFO` & `AndroidTools-0.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AndroidTools
-Version: 0.0.3
+Version: 0.0.4
 Summary: Android Tools for Python
 Home-page: https://github.com/grayrail000/PyJce
 Author: 1a
 Author-email: grayrail1x3@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `AndroidTools-0.0.3/setup.py` & `AndroidTools-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="AndroidTools",
-    version="0.0.3",
+    version="0.0.4",
     author="1a",
     author_email="grayrail1x3@gmail.com",
     description="Android Tools for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/grayrail000/PyJce",
     packages=setuptools.find_packages(),
```

### Comparing `AndroidTools-0.0.3/test/test_Jce.py` & `AndroidTools-0.0.4/test/test_Jce.py`

 * *Files identical despite different names*

