# Comparing `tmp/minidevice-2.1.6.tar.gz` & `tmp/minidevice-2.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minidevice-2.1.6.tar", last modified: Mon Jul 17 03:18:56 2023, max compression
+gzip compressed data, was "minidevice-2.1.7.tar", last modified: Mon Jul 17 07:40:48 2023, max compression
```

## Comparing `minidevice-2.1.6.tar` & `minidevice-2.1.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 03:18:56.127942 minidevice-2.1.6/
--rw-rw-rw-   0        0        0      811 2023-07-17 03:18:56.126941 minidevice-2.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      517 2023-07-05 10:51:23.000000 minidevice-2.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 03:18:56.115944 minidevice-2.1.6/minidevice/
--rw-rw-rw-   0        0        0     2268 2023-07-17 03:17:40.000000 minidevice-2.1.6/minidevice/DroidCast.py
--rw-rw-rw-   0        0        0     2178 2023-07-05 10:51:23.000000 minidevice-2.1.6/minidevice/QueueUtils.py
--rw-rw-rw-   0        0        0      208 2023-07-17 03:17:25.000000 minidevice-2.1.6/minidevice/__init__.py
--rw-rw-rw-   0        0        0      700 2023-07-17 03:17:30.000000 minidevice-2.1.6/minidevice/adbcap.py
--rw-rw-rw-   0        0        0      725 2023-07-06 16:43:00.000000 minidevice-2.1.6/minidevice/adbtouch.py
--rw-rw-rw-   0        0        0    12040 2023-07-17 03:17:45.000000 minidevice-2.1.6/minidevice/minicap.py
--rw-rw-rw-   0        0        0     1155 2023-07-06 16:43:00.000000 minidevice-2.1.6/minidevice/minitouch.py
--rw-rw-rw-   0        0        0      690 2023-07-05 11:03:04.000000 minidevice-2.1.6/minidevice/screencap.py
--rw-rw-rw-   0        0        0      605 2023-07-05 11:03:04.000000 minidevice-2.1.6/minidevice/touch.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:18:56.125941 minidevice-2.1.6/minidevice.egg-info/
--rw-rw-rw-   0        0        0      811 2023-07-17 03:18:55.000000 minidevice-2.1.6/minidevice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      393 2023-07-17 03:18:55.000000 minidevice-2.1.6/minidevice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 03:18:55.000000 minidevice-2.1.6/minidevice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-07-17 03:18:55.000000 minidevice-2.1.6/minidevice.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-17 03:18:55.000000 minidevice-2.1.6/minidevice.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-17 03:18:56.128940 minidevice-2.1.6/setup.cfg
--rw-rw-rw-   0        0        0      796 2023-07-17 03:08:57.000000 minidevice-2.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 07:40:48.972924 minidevice-2.1.7/
+-rw-rw-rw-   0        0        0      787 2023-07-17 07:40:48.971924 minidevice-2.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      493 2023-07-17 07:40:09.000000 minidevice-2.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 07:40:48.957927 minidevice-2.1.7/minidevice/
+-rw-rw-rw-   0        0        0     2268 2023-07-17 03:17:40.000000 minidevice-2.1.7/minidevice/DroidCast.py
+-rw-rw-rw-   0        0        0     2178 2023-07-05 10:51:23.000000 minidevice-2.1.7/minidevice/QueueUtils.py
+-rw-rw-rw-   0        0        0      208 2023-07-17 03:17:25.000000 minidevice-2.1.7/minidevice/__init__.py
+-rw-rw-rw-   0        0        0      700 2023-07-17 03:17:30.000000 minidevice-2.1.7/minidevice/adbcap.py
+-rw-rw-rw-   0        0        0      725 2023-07-06 16:43:00.000000 minidevice-2.1.7/minidevice/adbtouch.py
+-rw-rw-rw-   0        0        0    12040 2023-07-17 03:17:45.000000 minidevice-2.1.7/minidevice/minicap.py
+-rw-rw-rw-   0        0        0     1171 2023-07-17 07:33:55.000000 minidevice-2.1.7/minidevice/minitouch.py
+-rw-rw-rw-   0        0        0      690 2023-07-05 11:03:04.000000 minidevice-2.1.7/minidevice/screencap.py
+-rw-rw-rw-   0        0        0      605 2023-07-05 11:03:04.000000 minidevice-2.1.7/minidevice/touch.py
+drwxrwxrwx   0        0        0        0 2023-07-17 07:40:48.969925 minidevice-2.1.7/minidevice.egg-info/
+-rw-rw-rw-   0        0        0      787 2023-07-17 07:40:48.000000 minidevice-2.1.7/minidevice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      393 2023-07-17 07:40:48.000000 minidevice-2.1.7/minidevice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 07:40:48.000000 minidevice-2.1.7/minidevice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-07-17 07:40:48.000000 minidevice-2.1.7/minidevice.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-17 07:40:48.000000 minidevice-2.1.7/minidevice.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 07:40:48.972924 minidevice-2.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      796 2023-07-17 07:40:39.000000 minidevice-2.1.7/setup.py
```

### Comparing `minidevice-2.1.6/PKG-INFO` & `minidevice-2.1.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minidevice
-Version: 2.1.6
+Version: 2.1.7
 Summary: Android Auto Pypi
 Home-page: https://github.com/NakanoSanku/minidevice
 Author: KateTseng
 Author-email: Kate.TsengK@outlook.com
 License: MIT
 Keywords: game
 Requires-Python: >=3
@@ -21,12 +21,12 @@
 ## 已知bug
 - [ ] 转发端口清理失败
 ## Feature
 - screencap
     - Minicap
     - ADBcap
     - DroidCast
-    - ScrcpyCap
+    
 - touch
     - Minitouch
     - ADBtouch
-    - ScrcpyTouch
+
```

### Comparing `minidevice-2.1.6/minidevice/DroidCast.py` & `minidevice-2.1.7/minidevice/DroidCast.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.1.6/minidevice/QueueUtils.py` & `minidevice-2.1.7/minidevice/QueueUtils.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.1.6/minidevice/adbcap.py` & `minidevice-2.1.7/minidevice/adbcap.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.1.6/minidevice/adbtouch.py` & `minidevice-2.1.7/minidevice/adbtouch.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.1.6/minidevice/minicap.py` & `minidevice-2.1.7/minidevice/minicap.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.1.6/minidevice/minitouch.py` & `minidevice-2.1.7/minidevice/minitouch.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,11 +30,11 @@
         self.adb.sync.push(f"{MINITOUCH_PATH}/{self.abi}/minitouch", MNT_HOME)
         self.adb.shell(f"chmod +x {MNT_HOME}")
 
     def click(self, x: int, y: int, duration: int = 100):
         MNTDevice.tap(self, [(x, y)], duration=duration)
 
     def swipe(self, points: list, duration: int = 300):
-        MNTDevice.swipe(self, points, duration=duration)
+        MNTDevice.swipe(self, points, duration=duration/(len(points)-1))
 
     def __del__(self):
         MNTDevice.stop(self)
```

### Comparing `minidevice-2.1.6/minidevice/screencap.py` & `minidevice-2.1.7/minidevice/screencap.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.1.6/minidevice/touch.py` & `minidevice-2.1.7/minidevice/touch.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.1.6/minidevice.egg-info/PKG-INFO` & `minidevice-2.1.7/minidevice.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minidevice
-Version: 2.1.6
+Version: 2.1.7
 Summary: Android Auto Pypi
 Home-page: https://github.com/NakanoSanku/minidevice
 Author: KateTseng
 Author-email: Kate.TsengK@outlook.com
 License: MIT
 Keywords: game
 Requires-Python: >=3
@@ -21,12 +21,12 @@
 ## 已知bug
 - [ ] 转发端口清理失败
 ## Feature
 - screencap
     - Minicap
     - ADBcap
     - DroidCast
-    - ScrcpyCap
+    
 - touch
     - Minitouch
     - ADBtouch
-    - ScrcpyTouch
+
```

### Comparing `minidevice-2.1.6/setup.py` & `minidevice-2.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as fp:
     long_description = fp.read()
 
 setup(name='minidevice',
-      version='2.1.6',
+      version='2.1.7',
       description='Android Auto Pypi',
       author='KateTseng',
       author_email='Kate.TsengK@outlook.com',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/NakanoSanku/minidevice',
       license='MIT',
```

