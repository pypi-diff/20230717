# Comparing `tmp/minidevice-2.1.5.tar.gz` & `tmp/minidevice-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minidevice-2.1.5.tar", last modified: Wed Jul  5 11:38:58 2023, max compression
+gzip compressed data, was "minidevice-2.1.6.tar", last modified: Mon Jul 17 03:18:56 2023, max compression
```

## Comparing `minidevice-2.1.5.tar` & `minidevice-2.1.6.tar`

### file list

```diff
@@ -1,25 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 11:38:58.517990 minidevice-2.1.5/
--rw-rw-rw-   0        0        0      811 2023-07-05 11:38:58.517015 minidevice-2.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      517 2023-07-05 10:51:23.000000 minidevice-2.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-05 11:38:58.505311 minidevice-2.1.5/minidevice/
--rw-rw-rw-   0        0        0     2980 2023-07-05 11:03:04.000000 minidevice-2.1.5/minidevice/DroidCast.py
--rw-rw-rw-   0        0        0     2178 2023-07-05 10:51:23.000000 minidevice-2.1.5/minidevice/QueueUtils.py
--rw-rw-rw-   0        0        0      300 2023-07-05 11:03:04.000000 minidevice-2.1.5/minidevice/__init__.py
--rw-rw-rw-   0        0        0     5061 2023-07-05 11:36:46.000000 minidevice-2.1.5/minidevice/adb.py
--rw-rw-rw-   0        0        0      469 2023-07-05 11:03:04.000000 minidevice-2.1.5/minidevice/adbcap.py
--rw-rw-rw-   0        0        0      823 2023-07-05 11:03:04.000000 minidevice-2.1.5/minidevice/adbtouch.py
--rw-rw-rw-   0        0        0       39 2023-07-05 11:31:42.000000 minidevice-2.1.5/minidevice/logger.py
--rw-rw-rw-   0        0        0    13512 2023-07-05 11:36:46.000000 minidevice-2.1.5/minidevice/minicap.py
--rw-rw-rw-   0        0        0     1502 2023-07-05 11:03:04.000000 minidevice-2.1.5/minidevice/minitouch.py
--rw-rw-rw-   0        0        0      649 2023-07-05 11:03:04.000000 minidevice-2.1.5/minidevice/scrcpycap.py
--rw-rw-rw-   0        0        0     1035 2023-07-05 11:03:04.000000 minidevice-2.1.5/minidevice/scrcpytouch.py
--rw-rw-rw-   0        0        0      690 2023-07-05 11:03:04.000000 minidevice-2.1.5/minidevice/screencap.py
--rw-rw-rw-   0        0        0      605 2023-07-05 11:03:04.000000 minidevice-2.1.5/minidevice/touch.py
-drwxrwxrwx   0        0        0        0 2023-07-05 11:38:58.516039 minidevice-2.1.5/minidevice.egg-info/
--rw-rw-rw-   0        0        0      811 2023-07-05 11:38:58.000000 minidevice-2.1.5/minidevice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      482 2023-07-05 11:38:58.000000 minidevice-2.1.5/minidevice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 11:38:58.000000 minidevice-2.1.5/minidevice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2023-07-05 11:38:58.000000 minidevice-2.1.5/minidevice.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-05 11:38:58.000000 minidevice-2.1.5/minidevice.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-05 11:38:58.517990 minidevice-2.1.5/setup.cfg
--rw-rw-rw-   0        0        0      839 2023-07-05 11:03:04.000000 minidevice-2.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 03:18:56.127942 minidevice-2.1.6/
+-rw-rw-rw-   0        0        0      811 2023-07-17 03:18:56.126941 minidevice-2.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      517 2023-07-05 10:51:23.000000 minidevice-2.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 03:18:56.115944 minidevice-2.1.6/minidevice/
+-rw-rw-rw-   0        0        0     2268 2023-07-17 03:17:40.000000 minidevice-2.1.6/minidevice/DroidCast.py
+-rw-rw-rw-   0        0        0     2178 2023-07-05 10:51:23.000000 minidevice-2.1.6/minidevice/QueueUtils.py
+-rw-rw-rw-   0        0        0      208 2023-07-17 03:17:25.000000 minidevice-2.1.6/minidevice/__init__.py
+-rw-rw-rw-   0        0        0      700 2023-07-17 03:17:30.000000 minidevice-2.1.6/minidevice/adbcap.py
+-rw-rw-rw-   0        0        0      725 2023-07-06 16:43:00.000000 minidevice-2.1.6/minidevice/adbtouch.py
+-rw-rw-rw-   0        0        0    12040 2023-07-17 03:17:45.000000 minidevice-2.1.6/minidevice/minicap.py
+-rw-rw-rw-   0        0        0     1155 2023-07-06 16:43:00.000000 minidevice-2.1.6/minidevice/minitouch.py
+-rw-rw-rw-   0        0        0      690 2023-07-05 11:03:04.000000 minidevice-2.1.6/minidevice/screencap.py
+-rw-rw-rw-   0        0        0      605 2023-07-05 11:03:04.000000 minidevice-2.1.6/minidevice/touch.py
+drwxrwxrwx   0        0        0        0 2023-07-17 03:18:56.125941 minidevice-2.1.6/minidevice.egg-info/
+-rw-rw-rw-   0        0        0      811 2023-07-17 03:18:55.000000 minidevice-2.1.6/minidevice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      393 2023-07-17 03:18:55.000000 minidevice-2.1.6/minidevice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 03:18:55.000000 minidevice-2.1.6/minidevice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-07-17 03:18:55.000000 minidevice-2.1.6/minidevice.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-17 03:18:55.000000 minidevice-2.1.6/minidevice.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 03:18:56.128940 minidevice-2.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      796 2023-07-17 03:08:57.000000 minidevice-2.1.6/setup.py
```

### Comparing `minidevice-2.1.5/PKG-INFO` & `minidevice-2.1.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minidevice
-Version: 2.1.5
+Version: 2.1.6
 Summary: Android Auto Pypi
 Home-page: https://github.com/NakanoSanku/minidevice
 Author: KateTseng
 Author-email: Kate.TsengK@outlook.com
 License: MIT
 Keywords: game
 Requires-Python: >=3
```

### Comparing `minidevice-2.1.5/README.md` & `minidevice-2.1.6/README.md`

 * *Files identical despite different names*

### Comparing `minidevice-2.1.5/minidevice/DroidCast.py` & `minidevice-2.1.6/minidevice/DroidCast.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,82 +1,59 @@
 import os
 import subprocess
 
 import requests
+from adbutils import adb, adb_path
 
-from minidevice.adb import ADB, ADB_PATH
 from minidevice.screencap import ScreenCap
 
 WORK_DIR = os.path.dirname(__file__)
 APK_PATH = "{}/bin/DroidCast-debug-1.1.0.apk".format(WORK_DIR)
 APK_ANDROID_PATH = "/data/local/tmp/DroidCast-debug-1.0.apk"
 
 
 class DroidCast(ScreenCap):
-    def __init__(self, device, DroidCastServerPort=53516) -> None:
+    def __init__(self, device) -> None:
         """
         __init__ DroidCast截图方法
 
         Args:
             device (str): 设备id
-            DroidCastServerPort (int, optional): DroidCastServerPort服务端端口号. Defaults to 53516.
+
         """
-        self.droidcast_adb = ADB(device)
-        self.DroidCastServerPort = DroidCastServerPort
+        self.adb = adb.device(device)
         self.class_path = APK_ANDROID_PATH
         self.DroidCastSession = requests.Session()
         self.__install()
         self.__start()
 
     def __install(self):
-        self.droidcast_adb.push_file(APK_PATH, self.class_path)
-        self.droidcast_adb.install_apk(APK_PATH)
+        if "com.rayworks.droidcast" not in self.adb.list_packages():
+            self.adb.install(APK_PATH, nolaunch=True)
 
     def __start_droidcast(self):
-        out = str(
-            self.droidcast_adb.adb_command(
-                ["shell", "pm", "path", "com.rayworks.droidcast"]
-            )
-        )
-        prefix = "package:"
-        postfix = ".apk"
-        beg = out.index(prefix, 0)
-        end = out.rfind(postfix)
-
-        self.class_path = (
-                "CLASSPATH=" + out[beg + len(prefix): (end + len(postfix))].strip()
-        )
-        print(self.class_path)
-        start_droidcast_cmd = (
-            "exec app_process / com.rayworks.droidcast.Main --port={}".format(
-                self.DroidCastServerPort
-            )
-        )
+        out = self.adb.shell("pm path com.rayworks.droidcast")
+        self.class_path = "CLASSPATH=" + out.split(":")[1]
+        start_droidcast_cmd = "exec app_process / com.rayworks.droidcast.Main"
         self.droidcast_popen = subprocess.Popen(
             [
-                ADB_PATH,
+                adb_path(),
                 "-s",
-                self.droidcast_adb.device,
+                self.adb.serial,
                 "shell",
                 self.class_path,
                 start_droidcast_cmd,
             ],
             stderr=subprocess.DEVNULL,
             stdout=subprocess.DEVNULL,
         )
 
     def __forward_port(self):
-        self.droidcast_port = self.droidcast_adb.forward_port(
-            "tcp:{}".format(self.DroidCastServerPort)
-        )
-        self.droidcast_url = "http://localhost:{}/screenshot".format(
-            self.droidcast_port
-        )
-        print(self.droidcast_adb.list_forward_port())
-        print(self.droidcast_url)
+        self.droidcast_port = self.adb.forward_port(53516)
+        self.droidcast_url = f"http://localhost:{self.droidcast_port}/screenshot"
 
     def __start(self):
         self.__start_droidcast()
         self.__forward_port()
         self.screencap_raw()
         print("DroidCast启动完成")
 
@@ -88,7 +65,10 @@
         if self.droidcast_popen.poll() is not None:
             self.__stop()
             self.__start()
         return self.DroidCastSession.get(self.droidcast_url, timeout=3).content
 
     def __del__(self):
         self.__stop()
+
+    def __str__(self) -> str:
+        return "DroidCast-url:{}".format(self.droidcast_url)
```

### Comparing `minidevice-2.1.5/minidevice/QueueUtils.py` & `minidevice-2.1.6/minidevice/QueueUtils.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.1.5/minidevice/adbtouch.py` & `minidevice-2.1.6/minidevice/adbtouch.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,23 @@
-from minidevice.adb import ADB
-from minidevice.logger import logger
+from adbutils import adb
 from minidevice.touch import Touch
 
 
-class ADBtouch(Touch, ADB):
-    def __init__(self, device) -> None:
+class ADBtouch(Touch):
+    def __init__(self, serial) -> None:
         """
         __init__ ADB 操作方式
 
         Args:
-            device (str): 设备id
+            serial (str): 设备id
         """
-        ADB.__init__(self, device=device)
+        self.adb = adb.device(serial)
 
     def click(self, x: int, y: int, duration: int = 100):
-        ADB.click(self, x, y, duration)
-        logger.debug(f"ADB click ({x},{y}) consume:{duration}ms")
+        adb_command = ["input", "touchscreen", "swipe"]
+        adb_command.extend([str(x), str(y), str(x), str(y), str(duration)])
+        self.adb.shell(adb_command)
 
     def swipe(self, points: list, duration: int = 300):
         start_x, start_y = points[0]
         end_x, end_y = points[-1]
-        ADB.swipe(self, start_x, start_y, end_x, end_y, duration)
-        logger.debug(
-            f"ADB swipe from ({points[0]}) to ({points[-1]}) consume:{duration}ms"
-        )
+        self.adb.swipe(self, start_x, start_y, end_x, end_y, duration/1000)
```

### Comparing `minidevice-2.1.5/minidevice/minicap.py` & `minidevice-2.1.6/minidevice/minicap.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import os
 import socket
 import struct
 import subprocess
 import threading
 import time
 
+from adbutils import adb,adb_path
 from minidevice.QueueUtils import PipeQueue
-from minidevice.adb import ADB, ADB_PATH
-from minidevice.logger import logger
 from minidevice.screencap import ScreenCap
 
 WORK_DIR = os.path.dirname(__file__)
 MINICAP_PATH = "{}/bin/minicap/libs".format(WORK_DIR)
 MINICAPSO_PATH = "{}/bin/minicap/jni".format(WORK_DIR)
 
 
@@ -33,33 +32,33 @@
         self.VirtualWidth = 0  # 设备的虚拟宽度
         self.VirtualHeight = 0  # 设备的虚拟高度
         self.Orientation = 0  # 设备方向
         self.Quirks = 0  # 设备信息获取策略
 
     def __str__(self):
         message = (
-                "Banner [Version="
-                + str(self.Version)
-                + ", length="
-                + str(self.Length)
-                + ", Pid="
-                + str(self.Pid)
-                + ", realWidth="
-                + str(self.RealWidth)
-                + ", realHeight="
-                + str(self.RealHeight)
-                + ", virtualWidth="
-                + str(self.VirtualWidth)
-                + ", virtualHeight="
-                + str(self.VirtualHeight)
-                + ", orientation="
-                + str(self.Orientation)
-                + ", quirks="
-                + str(self.Quirks)
-                + "]"
+            "Banner [Version="
+            + str(self.Version)
+            + ", length="
+            + str(self.Length)
+            + ", Pid="
+            + str(self.Pid)
+            + ", realWidth="
+            + str(self.RealWidth)
+            + ", realHeight="
+            + str(self.RealHeight)
+            + ", virtualWidth="
+            + str(self.VirtualWidth)
+            + ", virtualHeight="
+            + str(self.VirtualHeight)
+            + ", orientation="
+            + str(self.Orientation)
+            + ", quirks="
+            + str(self.Quirks)
+            + "]"
         )
         return message
 
     def set_of_bytes(self, data):
         (
             self.Version,
             self.Length,
@@ -132,51 +131,51 @@
                     if readBannerBytes == 0:
                         self.banner.Version = chunk[cursor]
                     elif readBannerBytes == 1:
                         bannerLength = chunk[cursor]
                         self.banner.Length = bannerLength
                     elif readBannerBytes in [2, 3, 4, 5]:
                         self.banner.Pid += (
-                                                   chunk[cursor] << ((readBannerBytes - 2) * 8)
-                                           ) >> 0
+                            chunk[cursor] << ((readBannerBytes - 2) * 8)
+                        ) >> 0
                     elif readBannerBytes in [6, 7, 8, 9]:
                         self.banner.RealWidth += (
-                                                         chunk[cursor] << ((readBannerBytes - 6) * 8)
-                                                 ) >> 0
+                            chunk[cursor] << ((readBannerBytes - 6) * 8)
+                        ) >> 0
                     elif readBannerBytes in [10, 11, 12, 13]:
                         self.banner.RealHeight += (
-                                                          chunk[cursor] << ((readBannerBytes - 10) * 8)
-                                                  ) >> 0
+                            chunk[cursor] << ((readBannerBytes - 10) * 8)
+                        ) >> 0
                     elif readBannerBytes in [14, 15, 16, 17]:
                         self.banner.VirtualWidth += (
-                                                            chunk[cursor] << ((readBannerBytes - 14) * 8)
-                                                    ) >> 0
+                            chunk[cursor] << ((readBannerBytes - 14) * 8)
+                        ) >> 0
                     elif readBannerBytes in [18, 19, 20, 21]:
                         self.banner.VirtualHeight += (
-                                                             chunk[cursor] << ((readBannerBytes - 18) * 8)
-                                                     ) >> 0
+                            chunk[cursor] << ((readBannerBytes - 18) * 8)
+                        ) >> 0
                     elif readBannerBytes == 22:
                         self.banner.Orientation = chunk[cursor] * 90
                     elif readBannerBytes == 23:
                         self.banner.Quirks = chunk[cursor]
                     cursor += 1
                     readBannerBytes += 1
                     if readBannerBytes == bannerLength:
                         print(self.banner)
                 # 读取图片大小数据
                 elif readFrameBytes < 4:
                     frameBodyLength = frameBodyLength + (
-                            (chunk[cursor] << (readFrameBytes * 8)) >> 0
+                        (chunk[cursor] << (readFrameBytes * 8)) >> 0
                     )
                     cursor += 1
                     readFrameBytes += 1
                 # 读取图片内容
                 else:
                     if length - cursor >= frameBodyLength:
-                        dataBody = dataBody + chunk[cursor: (cursor + frameBodyLength)]
+                        dataBody = dataBody + chunk[cursor : (cursor + frameBodyLength)]
                         if dataBody[0] != 0xFF or dataBody[1] != 0xD8:
                             return
                         self.queue.put(dataBody)
                         cursor += frameBodyLength
                         frameBodyLength = 0
                         readFrameBytes = 0
                         dataBody = b""
@@ -192,137 +191,116 @@
             self.ReadImageStreamTask.join()  # 等待读取图像流的线程结束
         if self.minicapSocket:
             self.minicapSocket.close()  # 关闭 minicap 的 socket 连接
 
 
 class Minicap(ScreenCap):
     def __init__(
-            self,
-            device,
-            rate=15,
-            quality=100,
-            use_stream=True,
+        self,
+        serial,
+        rate=15,
+        quality=100,
+        use_stream=True,
     ) -> None:
         """
         __init__ minicap截图方式
 
         Args:
-            device (str): 设备id
+            serial (str): 设备id
             rate (int, optional): 截图帧率. Defaults to 15.
             quality (int, optional): 截图品质1~100之间. Defaults to 100.
             use_stream (bool, optional): 是否使用stream的方式. Defaults to True.
         """
-        self.minicap_adb = ADB(device)
+        self.adb = adb.device(serial)
         self.use_stream = use_stream
+        self.quality = quality
+        self.rate = rate
         self.__get_device_info()
-        minicap_name = "minicap_{}".format(time.time())
-        minicap_params = {
-            "minicap_name": minicap_name,
-            "rate": rate,
-            "quality": quality,
-        }
-        self.__get_minicap_params(**minicap_params)
         if self.use_stream:
             self.__start_minicap_by_stream()
 
     def screencap_raw(self) -> bytes:
         if self.use_stream:
             if self.minicap_popen.poll() is not None:
-                logger.warning("尝试重启minicap中")
                 self.__stop_minicap_by_stream()
                 self.__start_minicap_by_stream()
-            logger.debug("screen by minicap stream")
             return self.screen_queue.get()
         else:
-            logger.debug("screen by minicap frame")
             return self.__minicap_frame()
 
     def __minicap_frame(self):
         adb_command = [
             "shell",
             "LD_LIBRARY_PATH=/data/local/tmp",
             "/data/local/tmp/minicap",
         ]
         adb_command.extend(["-P", f"{self.vm_size}@{self.vm_size}/0"])
         adb_command.extend(["-Q", str(self.quality)])
         adb_command.extend(["-s"])
-        raw_data = self.minicap_adb.adb_command(adb_command)
+        raw_data = self.adb.shell(adb_command)
         jpg_data = raw_data.split(b"for JPG encoder\n" + line_breaker(self.sdk))[-1]
         jpg_data = jpg_data.replace(line_breaker(self.sdk), b"\n")
         return jpg_data
 
     def __get_device_info(self):
-        self.vm_size = self.minicap_adb.get_screen_resolution()
-        self.abi = self.minicap_adb.get_abi()
-        self.sdk = self.minicap_adb.get_sdk()
-
-    def __get_minicap_params(self, minicap_name, quality, rate):
-        self.minicap_name = minicap_name
-        self.quality = quality
-        self.rate = rate
+        self.vm_size = f"{self.adb.window_size().height}x{self.adb.window_size().width}"
+        self.abi = self.adb.getprop("ro.product.cpu.abi")
+        self.sdk = self.adb.getprop("ro.build.version.sdk")
 
     def __minicap_available(func):
         def wrapper(self, *args, **kwargs):
             try:
                 adb_command = [
-                    "shell",
                     "LD_LIBRARY_PATH=/data/local/tmp",
                     "/data/local/tmp/minicap",
                 ]
                 adb_command.extend(["-P", f"{self.vm_size}@{self.vm_size}/0"])
                 adb_command.extend(["-t"])
-                try:
-                    result = self.minicap_adb.adb_command(adb_command).strip()
-                except AttributeError:
-                    return False
-                if "OK" in result.decode("utf-8"):
+                result = self.adb.shell(adb_command)
+                if "OK" in result:
                     return func(self, *args, **kwargs)
+                print(result)
                 return False
             except subprocess.CalledProcessError:
                 return False
 
         return wrapper
 
     def __minicap_install(self):
-        if self.sdk == 32 and self.abi == "x86_64":
+        if str(self.sdk) == "32" and str(self.abi) == "x86_64":
             self.abi = "x86"
-
         MNC_HOME = "/data/local/tmp/minicap"
         MNC_SO_HOME = "/data/local/tmp/minicap.so"
 
-        self.minicap_adb.push_file(f"{MINICAP_PATH}/{self.abi}/minicap", MNC_HOME)
-        self.minicap_adb.push_file(
+        self.adb.sync.push(f"{MINICAP_PATH}/{self.abi}/minicap", MNC_HOME)
+        self.adb.sync.push(
             f"{MINICAPSO_PATH}/android-{self.sdk}/{self.abi}/minicap.so", MNC_SO_HOME
         )
-        self.minicap_adb.change_file_permission("+x", MNC_HOME)
+        self.adb.shell(["chmod +x", MNC_HOME])
 
     @__minicap_available
     def __start_minicap(self):
-        adb_command = [ADB_PATH]
-        if self.minicap_adb.device is not None:
-            adb_command.extend(["-s", self.minicap_adb.device])
+        adb_command = [adb_path()]
+        if self.adb.serial is not None:
+            adb_command.extend(["-s", self.adb.serial])
         adb_command.extend(
             ["shell", "LD_LIBRARY_PATH=/data/local/tmp", "/data/local/tmp/minicap"]
         )
-        adb_command.extend(["-n", f"{self.minicap_name}"])
         adb_command.extend(["-P", f"{self.vm_size}@{self.vm_size}/0"])
         adb_command.extend(["-Q", str(self.quality)])
         adb_command.extend(["-r", str(self.rate)])
         adb_command.extend(["-S"])
         self.minicap_popen = subprocess.Popen(
             adb_command, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL
         )
         time.sleep(2)
-        logger.info("启动minicap")
         return True
 
     def __forward_minicap(self):
-        self.minicap_port = self.minicap_adb.forward_port(
-            "localabstract:{}".format(self.minicap_name)
-        )
+        self.minicap_port = self.adb.forward_port("localabstract:minicap")
 
     def __read_minicap_stream(self):
         self.minicap_stream = MinicapStream.getBuilder("127.0.0.1", self.minicap_port)
         self.minicap_stream.run()
         self.banner = self.minicap_stream.banner
         self.screen_queue = self.minicap_stream.queue
 
@@ -332,22 +310,15 @@
             if not self.__start_minicap():
                 raise Exception("minicap不可用")
         self.__forward_minicap()
         self.__read_minicap_stream()
 
     def __stop_minicap_by_stream(self):
         self.minicap_stream.stop()  # 停止stream
-        # self.minicap_adb.remove_forward(self.minicap_port)  # 清理端口
         if self.minicap_popen.poll() is None:  # 清理管道
             self.minicap_popen.kill()
 
     def __del__(self):
         self.__stop_minicap_by_stream()
 
 
-if __name__ == "__main__":
-    a = Minicap("127.0.0.1:16384")
-    time.sleep(5)
-    import cv2
 
-    cv2.imshow("", a.screencap_opencv())
-    cv2.waitKey()
```

### Comparing `minidevice-2.1.5/minidevice/minitouch.py` & `minidevice-2.1.6/minidevice/minitouch.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,50 +1,40 @@
 import os
 
+from adbutils import adb
 from pyminitouch import MNTDevice
 
-from minidevice.adb import ADB
-from minidevice.logger import logger
 from minidevice.touch import Touch
 
 WORK_DIR = os.path.dirname(__file__)
 MINITOUCH_PATH = "{}/bin/minitouch/libs".format(WORK_DIR)
 
 
 class Minitouch(Touch, MNTDevice):
-    def __init__(self, device):
+    def __init__(self, serial):
         """
         __init__ minitouch点击方式
 
         Args:
             device (str): 设备id
         """
-        self.minitouch_adb = ADB(device)
+        self.adb = adb.device(serial)
         self.__get_device_info()
         self.__minitouch_install()
-        MNTDevice.__init__(self, device)
+        MNTDevice.__init__(self, serial)
 
     def __get_device_info(self):
-        self.abi = self.minitouch_adb.get_abi()
+        self.abi = self.adb.getprop("ro.product.cpu.abi")
 
     def __minitouch_install(self):
         MNT_HOME = "/data/local/tmp/minitouch"
-        self.minitouch_adb.push_file(f"{MINITOUCH_PATH}/{self.abi}/minitouch", MNT_HOME)
-        self.minitouch_adb.change_file_permission("+x", MNT_HOME)
+        self.adb.sync.push(f"{MINITOUCH_PATH}/{self.abi}/minitouch", MNT_HOME)
+        self.adb.shell(f"chmod +x {MNT_HOME}")
 
     def click(self, x: int, y: int, duration: int = 100):
         MNTDevice.tap(self, [(x, y)], duration=duration)
-        logger.debug(f"minitouch click ({x},{y}) consume:{duration}ms")
 
     def swipe(self, points: list, duration: int = 300):
         MNTDevice.swipe(self, points, duration=duration)
-        logger.debug(
-            f"minitouch swipe from ({points[0]}) to ({points[-1]}) consume:{duration}ms"
-        )
 
     def __del__(self):
         MNTDevice.stop(self)
-
-
-if __name__ == "__main__":
-    a = Minitouch("127.0.0.1:16384")
-    a.stop()
```

### Comparing `minidevice-2.1.5/minidevice/screencap.py` & `minidevice-2.1.6/minidevice/screencap.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.1.5/minidevice/touch.py` & `minidevice-2.1.6/minidevice/touch.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.1.5/minidevice.egg-info/PKG-INFO` & `minidevice-2.1.6/minidevice.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minidevice
-Version: 2.1.5
+Version: 2.1.6
 Summary: Android Auto Pypi
 Home-page: https://github.com/NakanoSanku/minidevice
 Author: KateTseng
 Author-email: Kate.TsengK@outlook.com
 License: MIT
 Keywords: game
 Requires-Python: >=3
```

### Comparing `minidevice-2.1.5/setup.py` & `minidevice-2.1.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as fp:
     long_description = fp.read()
 
 setup(name='minidevice',
-      version='2.1.5',
+      version='2.1.6',
       description='Android Auto Pypi',
       author='KateTseng',
       author_email='Kate.TsengK@outlook.com',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/NakanoSanku/minidevice',
       license='MIT',
       keywords='game',
       project_urls={},
       packages=find_packages(),
       include_package_data=True,
       install_requires=['opencv-python>=4.7.0.72',
                         'pyminitouch>=0.3.3',
-                        'scrcpy-client',
-                        'requests>=2.31.0'
+                        "adbutils==1.2.9"
                         ],
       python_requires='>=3'
       )
```

