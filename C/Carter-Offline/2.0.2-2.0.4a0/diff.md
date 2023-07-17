# Comparing `tmp/Carter-Offline-2.0.2.tar.gz` & `tmp/Carter-Offline-2.0.4a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Carter-Offline-2.0.2.tar", last modified: Fri Jul 14 15:35:56 2023, max compression
+gzip compressed data, was "Carter-Offline-2.0.4a0.tar", last modified: Mon Jul 17 11:39:52 2023, max compression
```

## Comparing `Carter-Offline-2.0.2.tar` & `Carter-Offline-2.0.4a0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-14 15:35:56.280927 Carter-Offline-2.0.2/
-drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-14 15:35:56.275361 Carter-Offline-2.0.2/CarterOffline/
-drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-14 15:35:56.275747 Carter-Offline-2.0.2/CarterOffline/Carter-Offline-SubFolder/
--rw-r--r--   0 cipher     (501) staff       (20)        0 2023-07-09 16:07:05.000000 Carter-Offline-2.0.2/CarterOffline/Carter-Offline-SubFolder/JanexSub.py
--rw-r--r--   0 cipher     (501) staff       (20)        0 2023-07-09 16:20:34.000000 Carter-Offline-2.0.2/CarterOffline/Carter-Offline-SubFolder/__init__.py
--rw-r--r--   0 cipher     (501) staff       (20)     5868 2023-07-14 14:47:21.000000 Carter-Offline-2.0.2/CarterOffline/__init__.py
--rw-r--r--   0 cipher     (501) staff       (20)      260 2023-07-07 20:07:57.000000 Carter-Offline-2.0.2/CarterOffline/chat.py
--rw-r--r--   0 cipher     (501) staff       (20)        1 2023-07-09 19:53:02.000000 Carter-Offline-2.0.2/CarterOffline/main.py
-drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-14 15:35:56.280629 Carter-Offline-2.0.2/Carter_Offline.egg-info/
--rw-r--r--   0 cipher     (501) staff       (20)     1891 2023-07-14 15:35:56.000000 Carter-Offline-2.0.2/Carter_Offline.egg-info/PKG-INFO
--rw-r--r--   0 cipher     (501) staff       (20)      387 2023-07-14 15:35:56.000000 Carter-Offline-2.0.2/Carter_Offline.egg-info/SOURCES.txt
--rw-r--r--   0 cipher     (501) staff       (20)        1 2023-07-14 15:35:56.000000 Carter-Offline-2.0.2/Carter_Offline.egg-info/dependency_links.txt
--rw-r--r--   0 cipher     (501) staff       (20)       22 2023-07-14 15:35:56.000000 Carter-Offline-2.0.2/Carter_Offline.egg-info/requires.txt
--rw-r--r--   0 cipher     (501) staff       (20)       14 2023-07-14 15:35:56.000000 Carter-Offline-2.0.2/Carter_Offline.egg-info/top_level.txt
--rw-r--r--   0 cipher     (501) staff       (20)     2950 2023-07-07 12:33:15.000000 Carter-Offline-2.0.2/LICENSE
--rw-r--r--   0 cipher     (501) staff       (20)     1891 2023-07-14 15:35:56.280809 Carter-Offline-2.0.2/PKG-INFO
--rw-r--r--   0 cipher     (501) staff       (20)     1504 2023-07-14 15:34:56.000000 Carter-Offline-2.0.2/README.md
--rw-r--r--   0 cipher     (501) staff       (20)       38 2023-07-14 15:35:56.280958 Carter-Offline-2.0.2/setup.cfg
--rw-r--r--   0 cipher     (501) staff       (20)     1322 2023-07-14 15:35:33.000000 Carter-Offline-2.0.2/setup.py
+drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-17 11:39:52.750916 Carter-Offline-2.0.4a0/
+drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-17 11:39:52.742247 Carter-Offline-2.0.4a0/CarterOffline/
+drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-17 11:39:52.742955 Carter-Offline-2.0.4a0/CarterOffline/Carter-Offline-SubFolder/
+-rw-r--r--   0 cipher     (501) staff       (20)        0 2023-07-09 16:07:05.000000 Carter-Offline-2.0.4a0/CarterOffline/Carter-Offline-SubFolder/JanexSub.py
+-rw-r--r--   0 cipher     (501) staff       (20)        0 2023-07-09 16:20:34.000000 Carter-Offline-2.0.4a0/CarterOffline/Carter-Offline-SubFolder/__init__.py
+-rw-r--r--   0 cipher     (501) staff       (20)     9763 2023-07-17 11:35:08.000000 Carter-Offline-2.0.4a0/CarterOffline/__init__.py
+-rw-r--r--   0 cipher     (501) staff       (20)      260 2023-07-07 20:07:57.000000 Carter-Offline-2.0.4a0/CarterOffline/chat.py
+-rw-r--r--   0 cipher     (501) staff       (20)        1 2023-07-09 19:53:02.000000 Carter-Offline-2.0.4a0/CarterOffline/main.py
+drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-17 11:39:52.750503 Carter-Offline-2.0.4a0/Carter_Offline.egg-info/
+-rw-r--r--   0 cipher     (501) staff       (20)     1893 2023-07-17 11:39:52.000000 Carter-Offline-2.0.4a0/Carter_Offline.egg-info/PKG-INFO
+-rw-r--r--   0 cipher     (501) staff       (20)      387 2023-07-17 11:39:52.000000 Carter-Offline-2.0.4a0/Carter_Offline.egg-info/SOURCES.txt
+-rw-r--r--   0 cipher     (501) staff       (20)        1 2023-07-17 11:39:52.000000 Carter-Offline-2.0.4a0/Carter_Offline.egg-info/dependency_links.txt
+-rw-r--r--   0 cipher     (501) staff       (20)       22 2023-07-17 11:39:52.000000 Carter-Offline-2.0.4a0/Carter_Offline.egg-info/requires.txt
+-rw-r--r--   0 cipher     (501) staff       (20)       14 2023-07-17 11:39:52.000000 Carter-Offline-2.0.4a0/Carter_Offline.egg-info/top_level.txt
+-rw-r--r--   0 cipher     (501) staff       (20)     2950 2023-07-07 12:33:15.000000 Carter-Offline-2.0.4a0/LICENSE
+-rw-r--r--   0 cipher     (501) staff       (20)     1893 2023-07-17 11:39:52.750757 Carter-Offline-2.0.4a0/PKG-INFO
+-rw-r--r--   0 cipher     (501) staff       (20)     1504 2023-07-14 15:34:56.000000 Carter-Offline-2.0.4a0/README.md
+-rw-r--r--   0 cipher     (501) staff       (20)       38 2023-07-17 11:39:52.750960 Carter-Offline-2.0.4a0/setup.cfg
+-rw-r--r--   0 cipher     (501) staff       (20)     1328 2023-07-17 11:39:49.000000 Carter-Offline-2.0.4a0/setup.py
```

### Comparing `Carter-Offline-2.0.2/Carter_Offline.egg-info/PKG-INFO` & `Carter-Offline-2.0.4a0/Carter_Offline.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Carter-Offline
-Version: 2.0.2
+Version: 2.0.4a0
 Home-page: https://github.com/Cipher58
 Download-URL: https://github.com/Cipher58/Carter-Offline/
 Author: Cipher58
 Author-email: cipher58public@gmail.com
 License: Lily 1.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `Carter-Offline-2.0.2/LICENSE` & `Carter-Offline-2.0.4a0/LICENSE`

 * *Files identical despite different names*

### Comparing `Carter-Offline-2.0.2/PKG-INFO` & `Carter-Offline-2.0.4a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Carter-Offline
-Version: 2.0.2
+Version: 2.0.4a0
 Home-page: https://github.com/Cipher58
 Download-URL: https://github.com/Cipher58/Carter-Offline/
 Author: Cipher58
 Author-email: cipher58public@gmail.com
 License: Lily 1.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `Carter-Offline-2.0.2/README.md` & `Carter-Offline-2.0.4a0/README.md`

 * *Files identical despite different names*

### Comparing `Carter-Offline-2.0.2/setup.py` & `Carter-Offline-2.0.4a0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 setuptools.setup(
     # Here is the module name.
     name="Carter-Offline",
 
     # version of the module
-    version="2.0.2",
+    version="2.0.4.alpha",
 
     # Name of Author
     author="Cipher58",
 
     download_url = 'https://github.com/Cipher58/Carter-Offline/',
 
     # your Email address
```

