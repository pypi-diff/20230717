# Comparing `tmp/pyScannerWrapper-0.1.0.tar.gz` & `tmp/pyScannerWrapper-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyScannerWrapper-0.1.0.tar", last modified: Sat Jul 15 17:00:11 2023, max compression
+gzip compressed data, was "pyScannerWrapper-0.2.0.tar", last modified: Sun Jul 16 22:37:15 2023, max compression
```

## Comparing `pyScannerWrapper-0.1.0.tar` & `pyScannerWrapper-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-07-15 17:00:11.769315 pyScannerWrapper-0.1.0/
--rw-r--r--   0 krystian  (1000) krystian  (1000)     1064 2023-07-14 00:11:55.000000 pyScannerWrapper-0.1.0/LICENSE.txt
--rw-r--r--   0 krystian  (1000) krystian  (1000)     1480 2023-07-15 17:00:11.769315 pyScannerWrapper-0.1.0/PKG-INFO
--rw-r--r--   0 krystian  (1000) krystian  (1000)      691 2023-07-15 16:58:27.000000 pyScannerWrapper-0.1.0/README.md
-drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-07-15 17:00:11.765982 pyScannerWrapper-0.1.0/pyScannerWrapper/
--rw-r--r--   0 krystian  (1000) krystian  (1000)       22 2023-07-15 16:58:27.000000 pyScannerWrapper-0.1.0/pyScannerWrapper/__init__.py
-drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-07-15 17:00:11.769315 pyScannerWrapper-0.1.0/pyScannerWrapper/core/
--rw-r--r--   0 krystian  (1000) krystian  (1000)     3297 2023-07-15 16:58:27.000000 pyScannerWrapper-0.1.0/pyScannerWrapper/core/_BaseScanner.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)       38 2023-07-14 19:04:47.000000 pyScannerWrapper-0.1.0/pyScannerWrapper/core/__init__.py
-drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-07-15 17:00:11.769315 pyScannerWrapper-0.1.0/pyScannerWrapper/exceptions/
--rw-r--r--   0 krystian  (1000) krystian  (1000)       52 2023-07-14 23:23:38.000000 pyScannerWrapper-0.1.0/pyScannerWrapper/exceptions/_ScannerNotFoundException.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)       64 2023-07-14 23:23:38.000000 pyScannerWrapper-0.1.0/pyScannerWrapper/exceptions/__init__.py
-drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-07-15 17:00:11.769315 pyScannerWrapper-0.1.0/pyScannerWrapper/scanners/
--rw-r--r--   0 krystian  (1000) krystian  (1000)     2551 2023-07-15 16:58:27.000000 pyScannerWrapper-0.1.0/pyScannerWrapper/scanners/_Masscan.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)       30 2023-07-14 19:04:47.000000 pyScannerWrapper-0.1.0/pyScannerWrapper/scanners/__init__.py
-drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-07-15 17:00:11.769315 pyScannerWrapper-0.1.0/pyScannerWrapper/structs/
--rw-r--r--   0 krystian  (1000) krystian  (1000)      106 2023-07-15 16:58:27.000000 pyScannerWrapper-0.1.0/pyScannerWrapper/structs/_ScanResults.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)       93 2023-07-15 16:58:27.000000 pyScannerWrapper-0.1.0/pyScannerWrapper/structs/_ServerResult.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)       78 2023-07-15 16:58:27.000000 pyScannerWrapper-0.1.0/pyScannerWrapper/structs/__init__.py
-drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-07-15 17:00:11.765982 pyScannerWrapper-0.1.0/pyScannerWrapper.egg-info/
--rw-r--r--   0 krystian  (1000) krystian  (1000)     1480 2023-07-15 17:00:11.000000 pyScannerWrapper-0.1.0/pyScannerWrapper.egg-info/PKG-INFO
--rw-r--r--   0 krystian  (1000) krystian  (1000)      584 2023-07-15 17:00:11.000000 pyScannerWrapper-0.1.0/pyScannerWrapper.egg-info/SOURCES.txt
--rw-r--r--   0 krystian  (1000) krystian  (1000)        1 2023-07-15 17:00:11.000000 pyScannerWrapper-0.1.0/pyScannerWrapper.egg-info/dependency_links.txt
--rw-r--r--   0 krystian  (1000) krystian  (1000)       17 2023-07-15 17:00:11.000000 pyScannerWrapper-0.1.0/pyScannerWrapper.egg-info/top_level.txt
--rw-r--r--   0 krystian  (1000) krystian  (1000)       38 2023-07-15 17:00:11.769315 pyScannerWrapper-0.1.0/setup.cfg
--rw-r--r--   0 krystian  (1000) krystian  (1000)     1278 2023-07-15 16:58:27.000000 pyScannerWrapper-0.1.0/setup.py
+drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-07-16 22:37:15.277324 pyScannerWrapper-0.2.0/
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     1064 2023-07-14 00:11:55.000000 pyScannerWrapper-0.2.0/LICENSE.txt
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     1480 2023-07-16 22:37:15.277324 pyScannerWrapper-0.2.0/PKG-INFO
+-rw-r--r--   0 krystian  (1000) krystian  (1000)      691 2023-07-15 16:58:27.000000 pyScannerWrapper-0.2.0/README.md
+drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-07-16 22:37:15.277324 pyScannerWrapper-0.2.0/pyScannerWrapper/
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       22 2023-07-16 22:36:01.000000 pyScannerWrapper-0.2.0/pyScannerWrapper/__init__.py
+drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-07-16 22:37:15.277324 pyScannerWrapper-0.2.0/pyScannerWrapper/core/
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     3297 2023-07-15 16:58:27.000000 pyScannerWrapper-0.2.0/pyScannerWrapper/core/_BaseScanner.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       38 2023-07-14 19:04:47.000000 pyScannerWrapper-0.2.0/pyScannerWrapper/core/__init__.py
+drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-07-16 22:37:15.277324 pyScannerWrapper-0.2.0/pyScannerWrapper/exceptions/
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       52 2023-07-14 23:23:38.000000 pyScannerWrapper-0.2.0/pyScannerWrapper/exceptions/_ScannerNotFoundException.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       64 2023-07-14 23:23:38.000000 pyScannerWrapper-0.2.0/pyScannerWrapper/exceptions/__init__.py
+drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-07-16 22:37:15.277324 pyScannerWrapper-0.2.0/pyScannerWrapper/scanners/
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     2444 2023-07-16 22:36:01.000000 pyScannerWrapper-0.2.0/pyScannerWrapper/scanners/_Masscan.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       30 2023-07-14 19:04:47.000000 pyScannerWrapper-0.2.0/pyScannerWrapper/scanners/__init__.py
+drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-07-16 22:37:15.277324 pyScannerWrapper-0.2.0/pyScannerWrapper/structs/
+-rw-r--r--   0 krystian  (1000) krystian  (1000)      106 2023-07-15 16:58:27.000000 pyScannerWrapper-0.2.0/pyScannerWrapper/structs/_ScanResults.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       93 2023-07-15 16:58:27.000000 pyScannerWrapper-0.2.0/pyScannerWrapper/structs/_ServerResult.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       78 2023-07-15 16:58:27.000000 pyScannerWrapper-0.2.0/pyScannerWrapper/structs/__init__.py
+drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-07-16 22:37:15.277324 pyScannerWrapper-0.2.0/pyScannerWrapper.egg-info/
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     1480 2023-07-16 22:37:15.000000 pyScannerWrapper-0.2.0/pyScannerWrapper.egg-info/PKG-INFO
+-rw-r--r--   0 krystian  (1000) krystian  (1000)      584 2023-07-16 22:37:15.000000 pyScannerWrapper-0.2.0/pyScannerWrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 krystian  (1000) krystian  (1000)        1 2023-07-16 22:37:15.000000 pyScannerWrapper-0.2.0/pyScannerWrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       17 2023-07-16 22:37:15.000000 pyScannerWrapper-0.2.0/pyScannerWrapper.egg-info/top_level.txt
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       38 2023-07-16 22:37:15.277324 pyScannerWrapper-0.2.0/setup.cfg
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     1278 2023-07-15 16:58:27.000000 pyScannerWrapper-0.2.0/setup.py
```

### Comparing `pyScannerWrapper-0.1.0/LICENSE.txt` & `pyScannerWrapper-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyScannerWrapper-0.1.0/PKG-INFO` & `pyScannerWrapper-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyScannerWrapper
-Version: 0.1.0
+Version: 0.2.0
 Summary: Easy-to-use Python wrapper for various port scanners.
 Home-page: https://github.com/Oreeeee/pyScannerWrapper
 Author: Oreeeee
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyScannerWrapper-0.1.0/README.md` & `pyScannerWrapper-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pyScannerWrapper-0.1.0/pyScannerWrapper/core/_BaseScanner.py` & `pyScannerWrapper-0.2.0/pyScannerWrapper/core/_BaseScanner.py`

 * *Files identical despite different names*

### Comparing `pyScannerWrapper-0.1.0/pyScannerWrapper/scanners/_Masscan.py` & `pyScannerWrapper-0.2.0/pyScannerWrapper/scanners/_Masscan.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,18 +14,14 @@
     def __init__(self):
         self.scanner_path_verify()
 
     def scan_internal(self) -> None:
         # Initialize results
         self.results = ScanResults(
             scanner_name=self.scanner_name,
-            start_time=None,
-            end_time=None,
-            time_took=None,
-            args=None,
             results=[],
         )
 
         # Add input file
         if self.input_file != "":
             self.scanner_args = f"{self.scanner_args} -iL {input_file}"
```

### Comparing `pyScannerWrapper-0.1.0/pyScannerWrapper.egg-info/PKG-INFO` & `pyScannerWrapper-0.2.0/pyScannerWrapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyScannerWrapper
-Version: 0.1.0
+Version: 0.2.0
 Summary: Easy-to-use Python wrapper for various port scanners.
 Home-page: https://github.com/Oreeeee/pyScannerWrapper
 Author: Oreeeee
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyScannerWrapper-0.1.0/pyScannerWrapper.egg-info/SOURCES.txt` & `pyScannerWrapper-0.2.0/pyScannerWrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyScannerWrapper-0.1.0/setup.py` & `pyScannerWrapper-0.2.0/setup.py`

 * *Files identical despite different names*

