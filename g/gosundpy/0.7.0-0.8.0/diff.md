# Comparing `tmp/gosundpy-0.7.0.tar.gz` & `tmp/gosundpy-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gosundpy-0.7.0.tar", last modified: Wed Jul 12 00:30:25 2023, max compression
+gzip compressed data, was "gosundpy-0.8.0.tar", last modified: Sun Jul 16 23:17:37 2023, max compression
```

## Comparing `gosundpy-0.7.0.tar` & `gosundpy-0.8.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 rabo       (501) staff       (20)        0 2023-07-12 00:30:25.685336 gosundpy-0.7.0/
--rw-r--r--   0 rabo       (501) staff       (20)     1073 2022-10-16 07:49:52.000000 gosundpy-0.7.0/LICENSE
--rw-r--r--   0 rabo       (501) staff       (20)     2001 2023-07-12 00:30:25.685203 gosundpy-0.7.0/PKG-INFO
--rw-r--r--   0 rabo       (501) staff       (20)     1035 2022-11-27 06:20:19.000000 gosundpy-0.7.0/README.md
-drwxr-xr-x   0 rabo       (501) staff       (20)        0 2023-07-12 00:30:25.684329 gosundpy-0.7.0/gosundpy/
--rw-r--r--   0 rabo       (501) staff       (20)      645 2023-01-14 04:09:14.000000 gosundpy-0.7.0/gosundpy/__init__.py
--rw-r--r--   0 rabo       (501) staff       (20)     3357 2023-01-18 01:29:44.000000 gosundpy-0.7.0/gosundpy/device.py
--rw-r--r--   0 rabo       (501) staff       (20)      232 2023-01-17 09:35:40.000000 gosundpy-0.7.0/gosundpy/exceptions.py
--rw-r--r--   0 rabo       (501) staff       (20)     2621 2023-07-12 00:07:52.000000 gosundpy-0.7.0/gosundpy/gosund.py
--rw-r--r--   0 rabo       (501) staff       (20)     1047 2023-07-12 00:07:04.000000 gosundpy-0.7.0/gosundpy/utils.py
--rw-r--r--   0 rabo       (501) staff       (20)       18 2023-07-12 00:30:17.000000 gosundpy-0.7.0/gosundpy/version.py
-drwxr-xr-x   0 rabo       (501) staff       (20)        0 2023-07-12 00:30:25.684892 gosundpy-0.7.0/gosundpy.egg-info/
--rw-r--r--   0 rabo       (501) staff       (20)     2001 2023-07-12 00:30:25.000000 gosundpy-0.7.0/gosundpy.egg-info/PKG-INFO
--rw-r--r--   0 rabo       (501) staff       (20)      305 2023-07-12 00:30:25.000000 gosundpy-0.7.0/gosundpy.egg-info/SOURCES.txt
--rw-r--r--   0 rabo       (501) staff       (20)        1 2023-07-12 00:30:25.000000 gosundpy-0.7.0/gosundpy.egg-info/dependency_links.txt
--rw-r--r--   0 rabo       (501) staff       (20)       23 2023-07-12 00:30:25.000000 gosundpy-0.7.0/gosundpy.egg-info/requires.txt
--rw-r--r--   0 rabo       (501) staff       (20)        9 2023-07-12 00:30:25.000000 gosundpy-0.7.0/gosundpy.egg-info/top_level.txt
--rw-r--r--   0 rabo       (501) staff       (20)       38 2023-07-12 00:30:25.685381 gosundpy-0.7.0/setup.cfg
--rw-r--r--   0 rabo       (501) staff       (20)     1690 2022-10-16 07:49:52.000000 gosundpy-0.7.0/setup.py
+drwxr-xr-x   0 rabo       (501) staff       (20)        0 2023-07-16 23:17:37.264083 gosundpy-0.8.0/
+-rw-r--r--   0 rabo       (501) staff       (20)     1073 2022-10-16 07:49:52.000000 gosundpy-0.8.0/LICENSE
+-rw-r--r--   0 rabo       (501) staff       (20)     2001 2023-07-16 23:17:37.263982 gosundpy-0.8.0/PKG-INFO
+-rw-r--r--   0 rabo       (501) staff       (20)     1035 2022-11-27 06:20:19.000000 gosundpy-0.8.0/README.md
+drwxr-xr-x   0 rabo       (501) staff       (20)        0 2023-07-16 23:17:37.263287 gosundpy-0.8.0/gosundpy/
+-rw-r--r--   0 rabo       (501) staff       (20)      715 2023-07-16 23:14:15.000000 gosundpy-0.8.0/gosundpy/__init__.py
+-rw-r--r--   0 rabo       (501) staff       (20)     3357 2023-01-18 01:29:44.000000 gosundpy-0.8.0/gosundpy/device.py
+-rw-r--r--   0 rabo       (501) staff       (20)      411 2023-07-16 23:14:12.000000 gosundpy-0.8.0/gosundpy/exceptions.py
+-rw-r--r--   0 rabo       (501) staff       (20)     2621 2023-07-12 00:07:52.000000 gosundpy-0.8.0/gosundpy/gosund.py
+-rw-r--r--   0 rabo       (501) staff       (20)     1047 2023-07-12 00:07:04.000000 gosundpy-0.8.0/gosundpy/utils.py
+-rw-r--r--   0 rabo       (501) staff       (20)       18 2023-07-16 23:16:51.000000 gosundpy-0.8.0/gosundpy/version.py
+drwxr-xr-x   0 rabo       (501) staff       (20)        0 2023-07-16 23:17:37.263804 gosundpy-0.8.0/gosundpy.egg-info/
+-rw-r--r--   0 rabo       (501) staff       (20)     2001 2023-07-16 23:17:37.000000 gosundpy-0.8.0/gosundpy.egg-info/PKG-INFO
+-rw-r--r--   0 rabo       (501) staff       (20)      305 2023-07-16 23:17:37.000000 gosundpy-0.8.0/gosundpy.egg-info/SOURCES.txt
+-rw-r--r--   0 rabo       (501) staff       (20)        1 2023-07-16 23:17:37.000000 gosundpy-0.8.0/gosundpy.egg-info/dependency_links.txt
+-rw-r--r--   0 rabo       (501) staff       (20)       23 2023-07-16 23:17:37.000000 gosundpy-0.8.0/gosundpy.egg-info/requires.txt
+-rw-r--r--   0 rabo       (501) staff       (20)        9 2023-07-16 23:17:37.000000 gosundpy-0.8.0/gosundpy.egg-info/top_level.txt
+-rw-r--r--   0 rabo       (501) staff       (20)       38 2023-07-16 23:17:37.264119 gosundpy-0.8.0/setup.cfg
+-rw-r--r--   0 rabo       (501) staff       (20)     1690 2022-10-16 07:49:52.000000 gosundpy-0.8.0/setup.py
```

### Comparing `gosundpy-0.7.0/LICENSE` & `gosundpy-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gosundpy-0.7.0/PKG-INFO` & `gosundpy-0.8.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gosundpy
-Version: 0.7.0
+Version: 0.8.0
 Summary: Python API for controling Gosund smart devices
 Home-page: https://github.com/purple4reina/gosundpy
 Author: Rey Abolofia
 Author-email: purple4reina@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/purple4reina/gosundpy
 Project-URL: Bug Tracker, https://github.com/purple4reina/gosundpy/issues
```

### Comparing `gosundpy-0.7.0/README.md` & `gosundpy-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `gosundpy-0.7.0/gosundpy/__init__.py` & `gosundpy-0.8.0/gosundpy/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import os
 
 from .device import (GosundDevice, GosundSwitchDevice, GosundLightBulbDevice,
         GosundTempuratureHumiditySensorDevice, GosundLightSensorDevice,
         GosundMotionSensorDevice, GosundContactSensorDevice)
-from .exceptions import GosundException
+from .exceptions import GosundException, GosundDeviceOfflineException
 from .gosund import Gosund
 from .version import version
 
 __all__ = [
         'GosundDevice',
         'GosundSwitchDevice',
         'GosundLightBulbDevice',
         'GosundTempuratureHumiditySensorDevice',
         'GosundLightSensorDevice',
         'GosundMotionSensorDevice',
         'GosundContactSensorDevice',
         'GosundException',
+        'GosundDeviceOfflineException',
         'Gosund',
 ]
 
 __version__ = version
```

### Comparing `gosundpy-0.7.0/gosundpy/device.py` & `gosundpy-0.8.0/gosundpy/device.py`

 * *Files identical despite different names*

### Comparing `gosundpy-0.7.0/gosundpy/gosund.py` & `gosundpy-0.8.0/gosundpy/gosund.py`

 * *Files identical despite different names*

### Comparing `gosundpy-0.7.0/gosundpy/utils.py` & `gosundpy-0.8.0/gosundpy/utils.py`

 * *Files identical despite different names*

### Comparing `gosundpy-0.7.0/gosundpy.egg-info/PKG-INFO` & `gosundpy-0.8.0/gosundpy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gosundpy
-Version: 0.7.0
+Version: 0.8.0
 Summary: Python API for controling Gosund smart devices
 Home-page: https://github.com/purple4reina/gosundpy
 Author: Rey Abolofia
 Author-email: purple4reina@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/purple4reina/gosundpy
 Project-URL: Bug Tracker, https://github.com/purple4reina/gosundpy/issues
```

### Comparing `gosundpy-0.7.0/setup.py` & `gosundpy-0.8.0/setup.py`

 * *Files identical despite different names*

