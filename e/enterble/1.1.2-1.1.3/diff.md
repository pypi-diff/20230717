# Comparing `tmp/enterble-1.1.2.tar.gz` & `tmp/enterble-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enterble-1.1.2.tar", last modified: Mon May 15 01:50:28 2023, max compression
+gzip compressed data, was "enterble-1.1.3.tar", last modified: Mon Jul 17 03:23:41 2023, max compression
```

## Comparing `enterble-1.1.2.tar` & `enterble-1.1.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 chenyitao   (501) staff       (20)        0 2023-05-15 01:50:28.181383 enterble-1.1.2/
--rw-r--r--   0 chenyitao   (501) staff       (20)     1055 2022-07-12 10:05:03.000000 enterble-1.1.2/LICENSE
--rw-r--r--   0 chenyitao   (501) staff       (20)     5763 2023-05-15 01:50:28.181172 enterble-1.1.2/PKG-INFO
--rw-r--r--   0 chenyitao   (501) staff       (20)     4746 2022-10-28 09:16:27.000000 enterble-1.1.2/README.md
-drwxr-xr-x   0 chenyitao   (501) staff       (20)        0 2023-05-15 01:50:28.177653 enterble-1.1.2/enterble/
--rw-r--r--   0 chenyitao   (501) staff       (20)      205 2022-07-14 03:48:18.000000 enterble-1.1.2/enterble/__init__.py
--rw-r--r--   0 chenyitao   (501) staff       (20)       22 2023-05-15 01:41:08.000000 enterble-1.1.2/enterble/__version__.py
-drwxr-xr-x   0 chenyitao   (501) staff       (20)        0 2023-05-15 01:50:28.178950 enterble-1.1.2/enterble/adapter/
--rw-r--r--   0 chenyitao   (501) staff       (20)        0 2022-07-14 03:49:28.000000 enterble-1.1.2/enterble/adapter/__init__.py
-drwxr-xr-x   0 chenyitao   (501) staff       (20)        0 2023-05-15 01:50:28.179357 enterble-1.1.2/enterble/adapter/flowtime/
--rw-r--r--   0 chenyitao   (501) staff       (20)        0 2022-07-12 06:12:45.000000 enterble-1.1.2/enterble/adapter/flowtime/__init__.py
--rw-r--r--   0 chenyitao   (501) staff       (20)     5169 2023-05-15 01:45:15.000000 enterble-1.1.2/enterble/adapter/flowtime/collector.py
-drwxr-xr-x   0 chenyitao   (501) staff       (20)        0 2023-05-15 01:50:28.180257 enterble-1.1.2/enterble/ble/
--rw-r--r--   0 chenyitao   (501) staff       (20)        0 2022-07-08 05:57:36.000000 enterble-1.1.2/enterble/ble/__init__.py
--rw-r--r--   0 chenyitao   (501) staff       (20)     9671 2022-10-28 09:04:15.000000 enterble-1.1.2/enterble/ble/device.py
--rw-r--r--   0 chenyitao   (501) staff       (20)     2443 2023-05-15 01:44:17.000000 enterble-1.1.2/enterble/ble/scanner.py
-drwxr-xr-x   0 chenyitao   (501) staff       (20)        0 2023-05-15 01:50:28.180707 enterble-1.1.2/enterble/collector/
--rw-r--r--   0 chenyitao   (501) staff       (20)        0 2022-07-14 03:48:57.000000 enterble-1.1.2/enterble/collector/__init__.py
--rw-r--r--   0 chenyitao   (501) staff       (20)     6538 2022-10-28 08:49:04.000000 enterble-1.1.2/enterble/collector/collector.py
-drwxr-xr-x   0 chenyitao   (501) staff       (20)        0 2023-05-15 01:50:28.178791 enterble-1.1.2/enterble.egg-info/
--rw-r--r--   0 chenyitao   (501) staff       (20)     5763 2023-05-15 01:50:28.000000 enterble-1.1.2/enterble.egg-info/PKG-INFO
--rw-r--r--   0 chenyitao   (501) staff       (20)      502 2023-05-15 01:50:28.000000 enterble-1.1.2/enterble.egg-info/SOURCES.txt
--rw-r--r--   0 chenyitao   (501) staff       (20)        1 2023-05-15 01:50:28.000000 enterble-1.1.2/enterble.egg-info/dependency_links.txt
--rw-r--r--   0 chenyitao   (501) staff       (20)        1 2022-07-14 03:44:23.000000 enterble-1.1.2/enterble.egg-info/not-zip-safe
--rw-r--r--   0 chenyitao   (501) staff       (20)       14 2023-05-15 01:50:28.000000 enterble-1.1.2/enterble.egg-info/requires.txt
--rw-r--r--   0 chenyitao   (501) staff       (20)        9 2023-05-15 01:50:28.000000 enterble-1.1.2/enterble.egg-info/top_level.txt
--rw-r--r--   0 chenyitao   (501) staff       (20)       38 2023-05-15 01:50:28.181442 enterble-1.1.2/setup.cfg
--rw-r--r--   0 chenyitao   (501) staff       (20)     1523 2023-05-15 01:50:20.000000 enterble-1.1.2/setup.py
+drwxr-xr-x   0 chenyitao   (501) staff       (20)        0 2023-07-17 03:23:41.195417 enterble-1.1.3/
+-rw-r--r--   0 chenyitao   (501) staff       (20)     1055 2022-07-12 10:05:03.000000 enterble-1.1.3/LICENSE
+-rw-r--r--   0 chenyitao   (501) staff       (20)     5783 2023-07-17 03:23:41.195220 enterble-1.1.3/PKG-INFO
+-rw-r--r--   0 chenyitao   (501) staff       (20)     4746 2022-10-28 09:16:27.000000 enterble-1.1.3/README.md
+drwxr-xr-x   0 chenyitao   (501) staff       (20)        0 2023-07-17 03:23:41.191569 enterble-1.1.3/enterble/
+-rw-r--r--   0 chenyitao   (501) staff       (20)      205 2022-07-14 03:48:18.000000 enterble-1.1.3/enterble/__init__.py
+-rw-r--r--   0 chenyitao   (501) staff       (20)       22 2023-07-17 03:21:34.000000 enterble-1.1.3/enterble/__version__.py
+drwxr-xr-x   0 chenyitao   (501) staff       (20)        0 2023-07-17 03:23:41.193239 enterble-1.1.3/enterble/adapter/
+-rw-r--r--   0 chenyitao   (501) staff       (20)        0 2022-07-14 03:49:28.000000 enterble-1.1.3/enterble/adapter/__init__.py
+drwxr-xr-x   0 chenyitao   (501) staff       (20)        0 2023-07-17 03:23:41.193498 enterble-1.1.3/enterble/adapter/flowtime/
+-rw-r--r--   0 chenyitao   (501) staff       (20)        0 2022-07-12 06:12:45.000000 enterble-1.1.3/enterble/adapter/flowtime/__init__.py
+-rw-r--r--   0 chenyitao   (501) staff       (20)     5169 2023-05-15 01:45:15.000000 enterble-1.1.3/enterble/adapter/flowtime/collector.py
+drwxr-xr-x   0 chenyitao   (501) staff       (20)        0 2023-07-17 03:23:41.194412 enterble-1.1.3/enterble/ble/
+-rw-r--r--   0 chenyitao   (501) staff       (20)        0 2022-07-08 05:57:36.000000 enterble-1.1.3/enterble/ble/__init__.py
+-rw-r--r--   0 chenyitao   (501) staff       (20)     9671 2022-10-28 09:04:15.000000 enterble-1.1.3/enterble/ble/device.py
+-rw-r--r--   0 chenyitao   (501) staff       (20)     2443 2023-05-15 01:44:17.000000 enterble-1.1.3/enterble/ble/scanner.py
+drwxr-xr-x   0 chenyitao   (501) staff       (20)        0 2023-07-17 03:23:41.194826 enterble-1.1.3/enterble/collector/
+-rw-r--r--   0 chenyitao   (501) staff       (20)        0 2022-07-14 03:48:57.000000 enterble-1.1.3/enterble/collector/__init__.py
+-rw-r--r--   0 chenyitao   (501) staff       (20)     6574 2023-07-17 03:20:28.000000 enterble-1.1.3/enterble/collector/collector.py
+drwxr-xr-x   0 chenyitao   (501) staff       (20)        0 2023-07-17 03:23:41.193053 enterble-1.1.3/enterble.egg-info/
+-rw-r--r--   0 chenyitao   (501) staff       (20)     5783 2023-07-17 03:23:41.000000 enterble-1.1.3/enterble.egg-info/PKG-INFO
+-rw-r--r--   0 chenyitao   (501) staff       (20)      502 2023-07-17 03:23:41.000000 enterble-1.1.3/enterble.egg-info/SOURCES.txt
+-rw-r--r--   0 chenyitao   (501) staff       (20)        1 2023-07-17 03:23:41.000000 enterble-1.1.3/enterble.egg-info/dependency_links.txt
+-rw-r--r--   0 chenyitao   (501) staff       (20)        1 2022-07-14 03:44:23.000000 enterble-1.1.3/enterble.egg-info/not-zip-safe
+-rw-r--r--   0 chenyitao   (501) staff       (20)       14 2023-07-17 03:23:41.000000 enterble-1.1.3/enterble.egg-info/requires.txt
+-rw-r--r--   0 chenyitao   (501) staff       (20)        9 2023-07-17 03:23:41.000000 enterble-1.1.3/enterble.egg-info/top_level.txt
+-rw-r--r--   0 chenyitao   (501) staff       (20)       38 2023-07-17 03:23:41.195471 enterble-1.1.3/setup.cfg
+-rw-r--r--   0 chenyitao   (501) staff       (20)     1523 2023-07-17 03:21:43.000000 enterble-1.1.3/setup.py
```

### Comparing `enterble-1.1.2/LICENSE` & `enterble-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `enterble-1.1.2/PKG-INFO` & `enterble-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: enterble
-Version: 1.1.2
+Version: 1.1.3
 Summary: BLE device scanner and data collector for Flowtime
 Home-page: https://github.com/Entertech/Enter-Biomodule-BLE-PC-SDK.git
 Author: Lockey
 Author-email: chenyitao@entertech.cn
 License: Entertech
+Platform: UNKNOWN
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
@@ -201,7 +202,9 @@
     loop = asyncio.get_event_loop()
     # 扫描设备
     # loop.run_until_complete(device_discover())
     # 采集数据
     loop.run_until_complete(data_collector())
 
 ```
+
+
```

### Comparing `enterble-1.1.2/README.md` & `enterble-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `enterble-1.1.2/enterble/adapter/flowtime/collector.py` & `enterble-1.1.3/enterble/adapter/flowtime/collector.py`

 * *Files identical despite different names*

### Comparing `enterble-1.1.2/enterble/ble/device.py` & `enterble-1.1.3/enterble/ble/device.py`

 * *Files identical despite different names*

### Comparing `enterble-1.1.2/enterble/ble/scanner.py` & `enterble-1.1.3/enterble/ble/scanner.py`

 * *Files identical despite different names*

### Comparing `enterble-1.1.2/enterble/collector/collector.py` & `enterble-1.1.3/enterble/collector/collector.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         """启动采集器"""
 
         # 扫描设备
         found = False
         while not found:
             logger.info('Scanning for %s...', self.name)
             self.device = await DeviceScanner.get_device(
-                self.name, self.model_nbr_uuid, self.device_identify
+                name=self.name, model_nbr_uuid=self.model_nbr_uuid, device_identify=self.device_identify
             )
             if self.device:
                 await self.device.set_soc_cal_call(self.device_soc_cal_callback)
                 found = True
                 logger.info('Found %s', self.device)
             else:
                 logger.info('%s not found, retrying...', self.name)
```

### Comparing `enterble-1.1.2/enterble.egg-info/PKG-INFO` & `enterble-1.1.3/enterble.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: enterble
-Version: 1.1.2
+Version: 1.1.3
 Summary: BLE device scanner and data collector for Flowtime
 Home-page: https://github.com/Entertech/Enter-Biomodule-BLE-PC-SDK.git
 Author: Lockey
 Author-email: chenyitao@entertech.cn
 License: Entertech
+Platform: UNKNOWN
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
@@ -201,7 +202,9 @@
     loop = asyncio.get_event_loop()
     # 扫描设备
     # loop.run_until_complete(device_discover())
     # 采集数据
     loop.run_until_complete(data_collector())
 
 ```
+
+
```

### Comparing `enterble-1.1.2/setup.py` & `enterble-1.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='enterble',
-    version='1.1.2',
+    version='1.1.3',
     description='BLE device scanner and data collector for Flowtime',
     long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',
     classifiers=[
         'Natural Language :: Chinese (Simplified)',
         "Development Status :: 4 - Beta",
         "Framework :: AsyncIO",
```

