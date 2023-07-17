# Comparing `tmp/lswifi-0.1.8.tar.gz` & `tmp/lswifi-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lswifi-0.1.8.tar", last modified: Sun Apr 18 21:46:21 2021, max compression
+gzip compressed data, was "lswifi-0.1.9.tar", last modified: Wed Apr 21 22:56:49 2021, max compression
```

## Comparing `lswifi-0.1.8.tar` & `lswifi-0.1.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2021-04-18 21:46:21.280241 lswifi-0.1.8/
--rw-rw-rw-   0        0        0     1468 2020-10-19 16:11:12.000000 lswifi-0.1.8/LICENSE
--rw-rw-rw-   0        0        0       25 2020-10-19 16:11:12.000000 lswifi-0.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0     4112 2021-04-18 21:46:21.281243 lswifi-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     2508 2021-04-18 21:34:39.000000 lswifi-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2021-04-18 21:46:21.239248 lswifi-0.1.8/lswifi/
--rw-rw-rw-   0        0        0        0 2020-10-19 16:11:12.000000 lswifi-0.1.8/lswifi/__init__.py
--rw-rw-rw-   0        0        0     3835 2021-01-19 02:46:33.000000 lswifi-0.1.8/lswifi/__main__.py
--rw-rw-rw-   0        0        0      265 2021-04-18 21:45:31.000000 lswifi-0.1.8/lswifi/__version__.py
--rw-rw-rw-   0        0        0     7366 2020-12-29 04:06:38.000000 lswifi-0.1.8/lswifi/appsetup.py
--rw-rw-rw-   0        0        0    16600 2021-04-18 21:32:37.000000 lswifi-0.1.8/lswifi/client.py
--rw-rw-rw-   0        0        0     7624 2021-04-18 21:32:20.000000 lswifi-0.1.8/lswifi/constants.py
--rw-rw-rw-   0        0        0    25812 2021-04-18 21:32:37.000000 lswifi-0.1.8/lswifi/core.py
--rw-rw-rw-   0        0        0   106873 2021-04-18 21:32:37.000000 lswifi-0.1.8/lswifi/elements.py
--rw-rw-rw-   0        0        0      878 2021-04-18 21:32:37.000000 lswifi-0.1.8/lswifi/guid.py
--rw-rw-rw-   0        0        0     6655 2021-04-18 21:32:20.000000 lswifi-0.1.8/lswifi/helpers.py
--rw-rw-rw-   0        0        0     4800 2021-04-18 21:32:37.000000 lswifi-0.1.8/lswifi/libpcap.py
--rw-rw-rw-   0        0        0    62739 2021-04-18 21:32:37.000000 lswifi-0.1.8/lswifi/wlanapi.py
-drwxrwxrwx   0        0        0        0 2021-04-18 21:46:21.278246 lswifi-0.1.8/lswifi.egg-info/
--rw-rw-rw-   0        0        0     4112 2021-04-18 21:46:20.000000 lswifi-0.1.8/lswifi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      420 2021-04-18 21:46:20.000000 lswifi-0.1.8/lswifi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-04-18 21:46:20.000000 lswifi-0.1.8/lswifi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2021-04-18 21:46:20.000000 lswifi-0.1.8/lswifi.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2021-04-18 21:46:20.000000 lswifi-0.1.8/lswifi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      112 2021-04-18 21:46:21.286241 lswifi-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1649 2020-10-19 16:11:12.000000 lswifi-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2021-04-21 22:56:49.077223 lswifi-0.1.9/
+-rw-rw-rw-   0        0        0     1468 2020-10-19 16:11:12.000000 lswifi-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0       25 2020-10-19 16:11:12.000000 lswifi-0.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     4112 2021-04-21 22:56:49.078229 lswifi-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2508 2021-04-18 21:34:39.000000 lswifi-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2021-04-21 22:56:49.014218 lswifi-0.1.9/lswifi/
+-rw-rw-rw-   0        0        0        0 2020-10-19 16:11:12.000000 lswifi-0.1.9/lswifi/__init__.py
+-rw-rw-rw-   0        0        0     3835 2021-01-19 02:46:33.000000 lswifi-0.1.9/lswifi/__main__.py
+-rw-rw-rw-   0        0        0      265 2021-04-21 22:49:55.000000 lswifi-0.1.9/lswifi/__version__.py
+-rw-rw-rw-   0        0        0     7366 2020-12-29 04:06:38.000000 lswifi-0.1.9/lswifi/appsetup.py
+-rw-rw-rw-   0        0        0    16600 2021-04-21 22:47:42.000000 lswifi-0.1.9/lswifi/client.py
+-rw-rw-rw-   0        0        0     7624 2021-04-18 21:32:20.000000 lswifi-0.1.9/lswifi/constants.py
+-rw-rw-rw-   0        0        0    25812 2021-04-21 22:47:42.000000 lswifi-0.1.9/lswifi/core.py
+-rw-rw-rw-   0        0        0   106939 2021-04-21 22:47:42.000000 lswifi-0.1.9/lswifi/elements.py
+-rw-rw-rw-   0        0        0      878 2021-04-21 22:47:42.000000 lswifi-0.1.9/lswifi/guid.py
+-rw-rw-rw-   0        0        0     6636 2021-04-21 22:44:45.000000 lswifi-0.1.9/lswifi/helpers.py
+-rw-rw-rw-   0        0        0     4800 2021-04-21 22:47:42.000000 lswifi-0.1.9/lswifi/libpcap.py
+-rw-rw-rw-   0        0        0    62739 2021-04-21 22:47:42.000000 lswifi-0.1.9/lswifi/wlanapi.py
+drwxrwxrwx   0        0        0        0 2021-04-21 22:56:49.074225 lswifi-0.1.9/lswifi.egg-info/
+-rw-rw-rw-   0        0        0     4112 2021-04-21 22:56:48.000000 lswifi-0.1.9/lswifi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      420 2021-04-21 22:56:48.000000 lswifi-0.1.9/lswifi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-04-21 22:56:48.000000 lswifi-0.1.9/lswifi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2021-04-21 22:56:48.000000 lswifi-0.1.9/lswifi.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2021-04-21 22:56:48.000000 lswifi-0.1.9/lswifi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      112 2021-04-21 22:56:49.089226 lswifi-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1649 2020-10-19 16:11:12.000000 lswifi-0.1.9/setup.py
```

### Comparing `lswifi-0.1.8/LICENSE` & `lswifi-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lswifi-0.1.8/PKG-INFO` & `lswifi-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lswifi
-Version: 0.1.8
+Version: 0.1.9
 Summary: a CLI Wi-Fi scanner tool for Windows
 Home-page: https://github.com/joshschmelzle/lswifi
 Author: Josh Schmelzle
 Author-email: josh@joshschmelzle.com
 License: UNKNOWN
 Description: ![coverage-badge](https://github.com/joshschmelzle/lswifi/blob/main/coverage.svg) [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-v2.0%20adopted-ff69b4.svg)](https://github.com/joshschmelzle/lswifi/blob/main/CODE_OF_CONDUCT.md)
```

### Comparing `lswifi-0.1.8/README.md` & `lswifi-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `lswifi-0.1.8/lswifi/__main__.py` & `lswifi-0.1.9/lswifi/__main__.py`

 * *Files identical despite different names*

### Comparing `lswifi-0.1.8/lswifi/appsetup.py` & `lswifi-0.1.9/lswifi/appsetup.py`

 * *Files identical despite different names*

### Comparing `lswifi-0.1.8/lswifi/client.py` & `lswifi-0.1.9/lswifi/client.py`

 * *Files identical despite different names*

### Comparing `lswifi-0.1.8/lswifi/constants.py` & `lswifi-0.1.9/lswifi/constants.py`

 * *Files identical despite different names*

### Comparing `lswifi-0.1.8/lswifi/core.py` & `lswifi-0.1.9/lswifi/core.py`

 * *Files identical despite different names*

### Comparing `lswifi-0.1.8/lswifi/elements.py` & `lswifi-0.1.9/lswifi/elements.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,15 +203,18 @@
         self.is_6ghz = is_six_band(int(frequency))
         if self.is_2ghz:
             band = "2GHz"
         if self.is_5ghz:
             band = "5GHz"
         if self.is_6ghz:
             band = "6GHz"
-        self.value = band
+        if band:
+            self.value = band
+        else:
+            self.value = ""
         self.header = Header("BAND")
         self.subheader = SubHeader("")
 
 
 class BeaconInterval(OutObject):
     """Base class for Beacon Interval"""
```

### Comparing `lswifi-0.1.8/lswifi/guid.py` & `lswifi-0.1.9/lswifi/guid.py`

 * *Files identical despite different names*

### Comparing `lswifi-0.1.8/lswifi/helpers.py` & `lswifi-0.1.9/lswifi/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -240,15 +240,15 @@
         return True
     else:
         return False
 
 
 def is_six_band(frequency: int) -> bool:
     """determines if a channel frequency is in the 6.0-7.125 GHz ISM band"""
-    if __get_digit(frequency, __num_digits(frequency) - 1) == 6:
+    if frequency > 5900 and frequency < 7125:
         return True
     else:
         return False
 
 
 def get_channel_number_from_frequency(frequency):
     """gets the 802.11 channel for a corresponding frequency
```

### Comparing `lswifi-0.1.8/lswifi/libpcap.py` & `lswifi-0.1.9/lswifi/libpcap.py`

 * *Files identical despite different names*

### Comparing `lswifi-0.1.8/lswifi/wlanapi.py` & `lswifi-0.1.9/lswifi/wlanapi.py`

 * *Files identical despite different names*

### Comparing `lswifi-0.1.8/lswifi.egg-info/PKG-INFO` & `lswifi-0.1.9/lswifi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lswifi
-Version: 0.1.8
+Version: 0.1.9
 Summary: a CLI Wi-Fi scanner tool for Windows
 Home-page: https://github.com/joshschmelzle/lswifi
 Author: Josh Schmelzle
 Author-email: josh@joshschmelzle.com
 License: UNKNOWN
 Description: ![coverage-badge](https://github.com/joshschmelzle/lswifi/blob/main/coverage.svg) [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-v2.0%20adopted-ff69b4.svg)](https://github.com/joshschmelzle/lswifi/blob/main/CODE_OF_CONDUCT.md)
```

### Comparing `lswifi-0.1.8/setup.py` & `lswifi-0.1.9/setup.py`

 * *Files identical despite different names*

