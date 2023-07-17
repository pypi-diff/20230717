# Comparing `tmp/pymycobot-3.1.6b2.tar.gz` & `tmp/pymycobot-3.1.6b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymycobot-3.1.6b2.tar", last modified: Wed Jul 12 09:01:57 2023, max compression
+gzip compressed data, was "pymycobot-3.1.6b3.tar", last modified: Mon Jul 17 11:35:58 2023, max compression
```

## Comparing `pymycobot-3.1.6b2.tar` & `pymycobot-3.1.6b3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 09:01:57.298094 pymycobot-3.1.6b2/
--rw-rw-rw-   0        0        0     1096 2022-06-28 10:55:58.000000 pymycobot-3.1.6b2/LICENSE
--rw-rw-rw-   0        0        0       51 2022-06-28 10:55:58.000000 pymycobot-3.1.6b2/MANIFEST.in
--rw-rw-rw-   0        0        0    59801 2023-07-12 09:01:57.297586 pymycobot-3.1.6b2/PKG-INFO
--rw-rw-rw-   0        0        0     1867 2022-07-22 06:29:08.000000 pymycobot-3.1.6b2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 09:01:57.258788 pymycobot-3.1.6b2/pymycobot/
--rw-rw-rw-   0        0        0    35112 2023-02-16 10:13:33.000000 pymycobot-3.1.6b2/pymycobot/Interface.py
--rw-rw-rw-   0        0        0     1681 2023-07-12 09:01:39.000000 pymycobot-3.1.6b2/pymycobot/__init__.py
--rw-rw-rw-   0        0        0     1968 2023-05-24 03:41:47.000000 pymycobot-3.1.6b2/pymycobot/bluet.py
--rw-rw-rw-   0        0        0      201 2023-07-12 07:37:01.000000 pymycobot-3.1.6b2/pymycobot/cobotx.py
--rw-rw-rw-   0        0        0    12367 2023-07-12 08:56:24.000000 pymycobot-3.1.6b2/pymycobot/common.py
--rw-rw-rw-   0        0        0     9159 2023-07-05 06:05:50.000000 pymycobot-3.1.6b2/pymycobot/elephantrobot.py
--rw-rw-rw-   0        0        0     3053 2022-06-28 10:55:58.000000 pymycobot-3.1.6b2/pymycobot/error.py
--rw-rw-rw-   0        0        0    34521 2023-07-06 02:36:43.000000 pymycobot-3.1.6b2/pymycobot/generate.py
--rw-rw-rw-   0        0        0      230 2022-06-28 10:55:58.000000 pymycobot-3.1.6b2/pymycobot/genre.py
--rw-rw-rw-   0        0        0      557 2022-06-28 10:55:58.000000 pymycobot-3.1.6b2/pymycobot/log.py
--rw-rw-rw-   0        0        0      206 2022-11-14 03:29:13.000000 pymycobot-3.1.6b2/pymycobot/mecharm.py
--rw-rw-rw-   0        0        0     9319 2023-07-12 08:57:21.000000 pymycobot-3.1.6b2/pymycobot/myarm.py
--rw-rw-rw-   0        0        0    13314 2023-06-27 03:24:50.000000 pymycobot-3.1.6b2/pymycobot/mybuddy.py
--rw-rw-rw-   0        0        0     4768 2022-07-20 06:10:10.000000 pymycobot-3.1.6b2/pymycobot/mybuddybluetooth.py
--rw-rw-rw-   0        0        0     4588 2022-10-14 05:56:03.000000 pymycobot-3.1.6b2/pymycobot/mybuddyemoticon.py
--rw-rw-rw-   0        0        0     7190 2022-09-13 08:59:04.000000 pymycobot-3.1.6b2/pymycobot/mybuddysocket.py
--rw-rw-rw-   0        0        0     7725 2023-07-06 02:40:02.000000 pymycobot-3.1.6b2/pymycobot/mycobot.py
--rw-rw-rw-   0        0        0     7385 2023-06-09 07:23:49.000000 pymycobot-3.1.6b2/pymycobot/mycobotsocket.py
--rw-rw-rw-   0        0        0     8707 2023-07-06 02:41:09.000000 pymycobot-3.1.6b2/pymycobot/mypalletizer.py
--rw-rw-rw-   0        0        0     7500 2023-05-24 08:28:04.000000 pymycobot-3.1.6b2/pymycobot/mypalletizersocket.py
--rw-rw-rw-   0        0        0    19696 2023-06-27 03:25:03.000000 pymycobot-3.1.6b2/pymycobot/ultraArm.py
--rw-rw-rw-   0        0        0      674 2022-06-28 10:55:58.000000 pymycobot-3.1.6b2/pymycobot/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-12 09:01:57.295272 pymycobot-3.1.6b2/pymycobot.egg-info/
--rw-rw-rw-   0        0        0    59801 2023-07-12 09:01:57.000000 pymycobot-3.1.6b2/pymycobot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      721 2023-07-12 09:01:57.000000 pymycobot-3.1.6b2/pymycobot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 09:01:57.000000 pymycobot-3.1.6b2/pymycobot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-12 09:01:57.000000 pymycobot-3.1.6b2/pymycobot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-12 09:01:57.000000 pymycobot-3.1.6b2/pymycobot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       26 2022-06-28 10:55:58.000000 pymycobot-3.1.6b2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 09:01:57.299221 pymycobot-3.1.6b2/setup.cfg
--rw-rw-rw-   0        0        0     3055 2022-08-30 07:24:54.000000 pymycobot-3.1.6b2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 11:35:58.273342 pymycobot-3.1.6b3/
+-rw-rw-rw-   0        0        0     1096 2022-06-28 10:55:58.000000 pymycobot-3.1.6b3/LICENSE
+-rw-rw-rw-   0        0        0       51 2022-06-28 10:55:58.000000 pymycobot-3.1.6b3/MANIFEST.in
+-rw-rw-rw-   0        0        0    59801 2023-07-17 11:35:58.272321 pymycobot-3.1.6b3/PKG-INFO
+-rw-rw-rw-   0        0        0     1867 2022-07-22 06:29:08.000000 pymycobot-3.1.6b3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 11:35:58.240063 pymycobot-3.1.6b3/pymycobot/
+-rw-rw-rw-   0        0        0    35112 2023-02-16 10:13:33.000000 pymycobot-3.1.6b3/pymycobot/Interface.py
+-rw-rw-rw-   0        0        0     1681 2023-07-17 11:32:05.000000 pymycobot-3.1.6b3/pymycobot/__init__.py
+-rw-rw-rw-   0        0        0     1968 2023-05-24 03:41:47.000000 pymycobot-3.1.6b3/pymycobot/bluet.py
+-rw-rw-rw-   0        0        0      201 2023-07-12 07:37:01.000000 pymycobot-3.1.6b3/pymycobot/cobotx.py
+-rw-rw-rw-   0        0        0    12394 2023-07-13 12:24:05.000000 pymycobot-3.1.6b3/pymycobot/common.py
+-rw-rw-rw-   0        0        0     9159 2023-07-05 06:05:50.000000 pymycobot-3.1.6b3/pymycobot/elephantrobot.py
+-rw-rw-rw-   0        0        0     3053 2022-06-28 10:55:58.000000 pymycobot-3.1.6b3/pymycobot/error.py
+-rw-rw-rw-   0        0        0    34521 2023-07-06 02:36:43.000000 pymycobot-3.1.6b3/pymycobot/generate.py
+-rw-rw-rw-   0        0        0      230 2022-06-28 10:55:58.000000 pymycobot-3.1.6b3/pymycobot/genre.py
+-rw-rw-rw-   0        0        0      557 2022-06-28 10:55:58.000000 pymycobot-3.1.6b3/pymycobot/log.py
+-rw-rw-rw-   0        0        0      206 2022-11-14 03:29:13.000000 pymycobot-3.1.6b3/pymycobot/mecharm.py
+-rw-rw-rw-   0        0        0     9329 2023-07-17 11:31:19.000000 pymycobot-3.1.6b3/pymycobot/myarm.py
+-rw-rw-rw-   0        0        0    13314 2023-06-27 03:24:50.000000 pymycobot-3.1.6b3/pymycobot/mybuddy.py
+-rw-rw-rw-   0        0        0     4768 2022-07-20 06:10:10.000000 pymycobot-3.1.6b3/pymycobot/mybuddybluetooth.py
+-rw-rw-rw-   0        0        0     4588 2022-10-14 05:56:03.000000 pymycobot-3.1.6b3/pymycobot/mybuddyemoticon.py
+-rw-rw-rw-   0        0        0     7190 2022-09-13 08:59:04.000000 pymycobot-3.1.6b3/pymycobot/mybuddysocket.py
+-rw-rw-rw-   0        0        0     7735 2023-07-17 11:32:34.000000 pymycobot-3.1.6b3/pymycobot/mycobot.py
+-rw-rw-rw-   0        0        0     7385 2023-06-09 07:23:49.000000 pymycobot-3.1.6b3/pymycobot/mycobotsocket.py
+-rw-rw-rw-   0        0        0     8707 2023-07-06 02:41:09.000000 pymycobot-3.1.6b3/pymycobot/mypalletizer.py
+-rw-rw-rw-   0        0        0     7500 2023-05-24 08:28:04.000000 pymycobot-3.1.6b3/pymycobot/mypalletizersocket.py
+-rw-rw-rw-   0        0        0    19696 2023-06-27 03:25:03.000000 pymycobot-3.1.6b3/pymycobot/ultraArm.py
+-rw-rw-rw-   0        0        0      674 2022-06-28 10:55:58.000000 pymycobot-3.1.6b3/pymycobot/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-17 11:35:58.269822 pymycobot-3.1.6b3/pymycobot.egg-info/
+-rw-rw-rw-   0        0        0    59801 2023-07-17 11:35:58.000000 pymycobot-3.1.6b3/pymycobot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      721 2023-07-17 11:35:58.000000 pymycobot-3.1.6b3/pymycobot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 11:35:58.000000 pymycobot-3.1.6b3/pymycobot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-17 11:35:58.000000 pymycobot-3.1.6b3/pymycobot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-17 11:35:58.000000 pymycobot-3.1.6b3/pymycobot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       26 2022-06-28 10:55:58.000000 pymycobot-3.1.6b3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 11:35:58.273342 pymycobot-3.1.6b3/setup.cfg
+-rw-rw-rw-   0        0        0     3055 2022-08-30 07:24:54.000000 pymycobot-3.1.6b3/setup.py
```

### Comparing `pymycobot-3.1.6b2/LICENSE` & `pymycobot-3.1.6b3/LICENSE`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.6b2/PKG-INFO` & `pymycobot-3.1.6b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymycobot
-Version: 3.1.6b2
+Version: 3.1.6b3
 Summary: Python API for serial communication of MyCobot.
 Home-page: https://github.com/elephantrobotics/pymycobot
 Author: Elephantrobotics
 Author-email: weiquan.xu@elephantrobotics.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `pymycobot-3.1.6b2/README.md` & `pymycobot-3.1.6b3/README.md`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.6b2/pymycobot/Interface.py` & `pymycobot-3.1.6b3/pymycobot/Interface.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.6b2/pymycobot/__init__.py` & `pymycobot-3.1.6b3/pymycobot/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 ]
 
 
 if sys.platform == "linux":
     from pymycobot.mybuddyemoticon import MyBuddyEmoticon
     __all__.append("MyBuddyEmoticon")
 
-__version__ = "3.1.6b2"
+__version__ = "3.1.6b3"
 __author__ = "Elephantrobotics"
 __email__ = "weiquan.xu@elephantrobotics.com"
 __git_url__ = "https://github.com/elephantrobotics/pymycobot"
 __copyright__ = "CopyRight (c) 2020-{0} Shenzhen Elephantrobotics technology".format(
     datetime.datetime.now().year
 )
```

### Comparing `pymycobot-3.1.6b2/pymycobot/bluet.py` & `pymycobot-3.1.6b3/pymycobot/bluet.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.6b2/pymycobot/common.py` & `pymycobot-3.1.6b3/pymycobot/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -379,14 +379,15 @@
             try:
                 self.sock.settimeout(1)
                 data = self.sock.recv(1024)
             except:
                 data = b""
         return data
     else:
+        # with self.lock:
         self.log.debug("_write: {}".format([hex(i) for i in command]))
         self._serial_port.write(command)
         self._serial_port.flush()
 
 
 def read(self, genre):
     datas = b""
```

### Comparing `pymycobot-3.1.6b2/pymycobot/elephantrobot.py` & `pymycobot-3.1.6b3/pymycobot/elephantrobot.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.6b2/pymycobot/error.py` & `pymycobot-3.1.6b3/pymycobot/error.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.6b2/pymycobot/generate.py` & `pymycobot-3.1.6b3/pymycobot/generate.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.6b2/pymycobot/log.py` & `pymycobot-3.1.6b3/pymycobot/log.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.6b2/pymycobot/myarm.py` & `pymycobot-3.1.6b3/pymycobot/myarm.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,23 +153,23 @@
                    for radian in radians]
         return self._mesg(ProtocolCode.SEND_ANGLES, degrees, speed)
 
     def sync_send_angles(self, degrees, speed, timeout=7):
         """Send the angle in synchronous state and return when the target point is reached
             
         Args:
-            degrees: a list of degree values(List[float]), length 6.
+            degrees: a list of degree values(List[float]), length 7.
             speed: (int) 0 ~ 100
             timeout: default 7s.
         """
         t = time.time()
         self.send_angles(degrees, speed)
         while time.time() - t < timeout:
             f = self.is_in_position(degrees, 0)
-            if f:
+            if f == 1:
                 break
             time.sleep(0.1)
         return self
 
     def sync_send_coords(self, coords, speed, mode, timeout=7):
         """Send the coord in synchronous state and return when the target point is reached
             
@@ -178,15 +178,15 @@
             speed: (int) 0 ~ 100
             mode: (int): 0 - angular, 1 - linear
             timeout: default 7s.
         """
         t = time.time()
         self.send_coords(coords, speed, mode)
         while time.time() - t < timeout:
-            if self.is_in_position(coords, 1):
+            if self.is_in_position(coords, 1) == 1:
                 break
             time.sleep(0.1)
         return self
 
     # Basic for raspberry pi.
     def gpio_init(self):
         """Init GPIO module, and set BCM mode."""
```

### Comparing `pymycobot-3.1.6b2/pymycobot/mybuddy.py` & `pymycobot-3.1.6b3/pymycobot/mybuddy.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.6b2/pymycobot/mybuddybluetooth.py` & `pymycobot-3.1.6b3/pymycobot/mybuddybluetooth.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.6b2/pymycobot/mybuddyemoticon.py` & `pymycobot-3.1.6b3/pymycobot/mybuddyemoticon.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.6b2/pymycobot/mybuddysocket.py` & `pymycobot-3.1.6b3/pymycobot/mybuddysocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.6b2/pymycobot/mycobot.py` & `pymycobot-3.1.6b3/pymycobot/mycobot.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,15 +164,15 @@
             speed: (int) 0 ~ 100
             timeout: default 7s.
         """
         t = time.time()
         self.send_angles(degrees, speed)
         while time.time() - t < timeout:
             f = self.is_in_position(degrees, 0)
-            if f:
+            if f == 1:
                 break
             time.sleep(0.1)
         return self
 
     def sync_send_coords(self, coords, speed, mode, timeout=7):
         """Send the coord in synchronous state and return when the target point is reached
             
@@ -181,15 +181,15 @@
             speed: (int) 0 ~ 100
             mode: (int): 0 - angular, 1 - linear
             timeout: default 7s.
         """
         t = time.time()
         self.send_coords(coords, speed, mode)
         while time.time() - t < timeout:
-            if self.is_in_position(coords, 1):
+            if self.is_in_position(coords, 1) == 1:
                 break
             time.sleep(0.1)
         return self
 
     # Basic for raspberry pi.
     def gpio_init(self):
         """Init GPIO module, and set BCM mode."""
```

### Comparing `pymycobot-3.1.6b2/pymycobot/mycobotsocket.py` & `pymycobot-3.1.6b3/pymycobot/mycobotsocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.6b2/pymycobot/mypalletizer.py` & `pymycobot-3.1.6b3/pymycobot/mypalletizer.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.6b2/pymycobot/mypalletizersocket.py` & `pymycobot-3.1.6b3/pymycobot/mypalletizersocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.6b2/pymycobot/ultraArm.py` & `pymycobot-3.1.6b3/pymycobot/ultraArm.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.6b2/pymycobot/utils.py` & `pymycobot-3.1.6b3/pymycobot/utils.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.6b2/pymycobot.egg-info/PKG-INFO` & `pymycobot-3.1.6b3/pymycobot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymycobot
-Version: 3.1.6b2
+Version: 3.1.6b3
 Summary: Python API for serial communication of MyCobot.
 Home-page: https://github.com/elephantrobotics/pymycobot
 Author: Elephantrobotics
 Author-email: weiquan.xu@elephantrobotics.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `pymycobot-3.1.6b2/pymycobot.egg-info/SOURCES.txt` & `pymycobot-3.1.6b3/pymycobot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.6b2/setup.py` & `pymycobot-3.1.6b3/setup.py`

 * *Files identical despite different names*

