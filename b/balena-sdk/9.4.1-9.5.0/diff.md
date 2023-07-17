# Comparing `tmp/balena-sdk-9.4.1.tar.gz` & `tmp/balena-sdk-9.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\balena-sdk-9.4.1.tar", last modified: Sat May 16 02:05:55 2020, max compression
+gzip compressed data, was "dist\balena-sdk-9.5.0.tar", last modified: Fri Jun 19 06:30:42 2020, max compression
```

## Comparing `balena-sdk-9.4.1.tar` & `balena-sdk-9.5.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2020-05-16 02:05:55.000000 balena-sdk-9.4.1/
--rw-rw-rw-   0        0        0      794 2020-05-16 02:05:55.000000 balena-sdk-9.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     3350 2020-05-16 02:05:15.000000 balena-sdk-9.4.1/README.md
-drwxrwxrwx   0        0        0        0 2020-05-16 02:05:55.000000 balena-sdk-9.4.1/balena/
--rw-rw-rw-   0        0        0     1560 2020-05-16 02:05:15.000000 balena-sdk-9.4.1/balena/__init__.py
--rw-rw-rw-   0        0        0    10093 2020-02-04 12:38:22.000000 balena-sdk-9.4.1/balena/auth.py
--rw-rw-rw-   0        0        0     9590 2019-11-21 08:59:45.000000 balena-sdk-9.4.1/balena/base_request.py
--rw-rw-rw-   0        0        0    10586 2019-11-21 08:59:45.000000 balena-sdk-9.4.1/balena/exceptions.py
--rw-rw-rw-   0        0        0     5544 2020-02-04 12:38:22.000000 balena-sdk-9.4.1/balena/logs.py
-drwxrwxrwx   0        0        0        0 2020-05-16 02:05:55.000000 balena-sdk-9.4.1/balena/models/
--rw-rw-rw-   0        0        0     1024 2018-10-30 15:20:37.000000 balena-sdk-9.4.1/balena/models/__init__.py
--rw-rw-rw-   0        0        0     2941 2018-10-30 15:20:37.000000 balena-sdk-9.4.1/balena/models/api_key.py
--rw-rw-rw-   0        0        0    31931 2020-03-13 19:02:31.000000 balena-sdk-9.4.1/balena/models/application.py
--rw-rw-rw-   0        0        0     2482 2020-02-04 12:38:22.000000 balena-sdk-9.4.1/balena/models/config.py
--rw-rw-rw-   0        0        0    11061 2018-10-30 15:20:37.000000 balena-sdk-9.4.1/balena/models/config_variable.py
--rw-rw-rw-   0        0        0    56289 2019-11-21 08:59:45.000000 balena-sdk-9.4.1/balena/models/device.py
--rw-rw-rw-   0        0        0    13686 2020-02-04 12:38:22.000000 balena-sdk-9.4.1/balena/models/device_os.py
--rw-rw-rw-   0        0        0    23054 2019-05-06 10:37:26.000000 balena-sdk-9.4.1/balena/models/environment_variables.py
--rw-rw-rw-   0        0        0     1801 2019-04-22 07:51:50.000000 balena-sdk-9.4.1/balena/models/hup.py
--rw-rw-rw-   0        0        0     2557 2018-10-30 15:20:37.000000 balena-sdk-9.4.1/balena/models/image.py
--rw-rw-rw-   0        0        0     2512 2018-10-30 15:20:37.000000 balena-sdk-9.4.1/balena/models/key.py
--rw-rw-rw-   0        0        0     6527 2019-11-21 08:59:45.000000 balena-sdk-9.4.1/balena/models/release.py
--rw-rw-rw-   0        0        0     1208 2018-10-30 15:20:37.000000 balena-sdk-9.4.1/balena/models/service.py
--rw-rw-rw-   0        0        0     1289 2018-10-30 15:20:37.000000 balena-sdk-9.4.1/balena/models/service_install.py
--rw-rw-rw-   0        0        0    22625 2019-11-21 08:59:45.000000 balena-sdk-9.4.1/balena/models/supervisor.py
--rw-rw-rw-   0        0        0    16482 2019-11-21 08:59:45.000000 balena-sdk-9.4.1/balena/models/tag.py
--rw-rw-rw-   0        0        0     2318 2019-11-21 08:59:45.000000 balena-sdk-9.4.1/balena/resources.py
--rw-rw-rw-   0        0        0     6889 2019-11-21 08:59:45.000000 balena-sdk-9.4.1/balena/settings.py
--rw-rw-rw-   0        0        0     3992 2018-10-30 15:20:37.000000 balena-sdk-9.4.1/balena/twofactor_auth.py
--rw-rw-rw-   0        0        0      306 2019-11-21 08:59:45.000000 balena-sdk-9.4.1/balena/utils.py
-drwxrwxrwx   0        0        0        0 2020-05-16 02:05:55.000000 balena-sdk-9.4.1/balena_sdk.egg-info/
--rw-rw-rw-   0        0        0      794 2020-05-16 02:05:55.000000 balena-sdk-9.4.1/balena_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      794 2020-05-16 02:05:55.000000 balena-sdk-9.4.1/balena_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-05-16 02:05:55.000000 balena-sdk-9.4.1/balena_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      140 2020-05-16 02:05:55.000000 balena-sdk-9.4.1/balena_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2020-05-16 02:05:55.000000 balena-sdk-9.4.1/balena_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2020-05-16 02:05:55.000000 balena-sdk-9.4.1/setup.cfg
--rw-rw-rw-   0        0        0     4035 2019-04-22 07:51:50.000000 balena-sdk-9.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2020-06-19 06:30:42.000000 balena-sdk-9.5.0/
+-rw-rw-rw-   0        0        0      794 2020-06-19 06:30:42.000000 balena-sdk-9.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3350 2020-05-16 02:05:15.000000 balena-sdk-9.5.0/README.md
+drwxrwxrwx   0        0        0        0 2020-06-19 06:30:42.000000 balena-sdk-9.5.0/balena/
+-rw-rw-rw-   0        0        0     1560 2020-06-19 06:30:01.000000 balena-sdk-9.5.0/balena/__init__.py
+-rw-rw-rw-   0        0        0    10093 2020-02-04 12:38:22.000000 balena-sdk-9.5.0/balena/auth.py
+-rw-rw-rw-   0        0        0     9590 2019-11-21 08:59:45.000000 balena-sdk-9.5.0/balena/base_request.py
+-rw-rw-rw-   0        0        0    10586 2019-11-21 08:59:45.000000 balena-sdk-9.5.0/balena/exceptions.py
+-rw-rw-rw-   0        0        0     5544 2020-02-04 12:38:22.000000 balena-sdk-9.5.0/balena/logs.py
+drwxrwxrwx   0        0        0        0 2020-06-19 06:30:42.000000 balena-sdk-9.5.0/balena/models/
+-rw-rw-rw-   0        0        0     1024 2018-10-30 15:20:37.000000 balena-sdk-9.5.0/balena/models/__init__.py
+-rw-rw-rw-   0        0        0     2941 2018-10-30 15:20:37.000000 balena-sdk-9.5.0/balena/models/api_key.py
+-rw-rw-rw-   0        0        0    31931 2020-03-13 19:02:31.000000 balena-sdk-9.5.0/balena/models/application.py
+-rw-rw-rw-   0        0        0     2482 2020-02-04 12:38:22.000000 balena-sdk-9.5.0/balena/models/config.py
+-rw-rw-rw-   0        0        0    11061 2018-10-30 15:20:37.000000 balena-sdk-9.5.0/balena/models/config_variable.py
+-rw-rw-rw-   0        0        0    56757 2020-06-19 06:30:01.000000 balena-sdk-9.5.0/balena/models/device.py
+-rw-rw-rw-   0        0        0    13686 2020-02-04 12:38:22.000000 balena-sdk-9.5.0/balena/models/device_os.py
+-rw-rw-rw-   0        0        0    23054 2019-05-06 10:37:26.000000 balena-sdk-9.5.0/balena/models/environment_variables.py
+-rw-rw-rw-   0        0        0     1801 2019-04-22 07:51:50.000000 balena-sdk-9.5.0/balena/models/hup.py
+-rw-rw-rw-   0        0        0     2557 2018-10-30 15:20:37.000000 balena-sdk-9.5.0/balena/models/image.py
+-rw-rw-rw-   0        0        0     2512 2018-10-30 15:20:37.000000 balena-sdk-9.5.0/balena/models/key.py
+-rw-rw-rw-   0        0        0     6527 2019-11-21 08:59:45.000000 balena-sdk-9.5.0/balena/models/release.py
+-rw-rw-rw-   0        0        0     1208 2018-10-30 15:20:37.000000 balena-sdk-9.5.0/balena/models/service.py
+-rw-rw-rw-   0        0        0     1289 2018-10-30 15:20:37.000000 balena-sdk-9.5.0/balena/models/service_install.py
+-rw-rw-rw-   0        0        0    22625 2019-11-21 08:59:45.000000 balena-sdk-9.5.0/balena/models/supervisor.py
+-rw-rw-rw-   0        0        0    16482 2019-11-21 08:59:45.000000 balena-sdk-9.5.0/balena/models/tag.py
+-rw-rw-rw-   0        0        0     2318 2019-11-21 08:59:45.000000 balena-sdk-9.5.0/balena/resources.py
+-rw-rw-rw-   0        0        0     6889 2019-11-21 08:59:45.000000 balena-sdk-9.5.0/balena/settings.py
+-rw-rw-rw-   0        0        0     3992 2018-10-30 15:20:37.000000 balena-sdk-9.5.0/balena/twofactor_auth.py
+-rw-rw-rw-   0        0        0      306 2019-11-21 08:59:45.000000 balena-sdk-9.5.0/balena/utils.py
+drwxrwxrwx   0        0        0        0 2020-06-19 06:30:42.000000 balena-sdk-9.5.0/balena_sdk.egg-info/
+-rw-rw-rw-   0        0        0      794 2020-06-19 06:30:42.000000 balena-sdk-9.5.0/balena_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      794 2020-06-19 06:30:42.000000 balena-sdk-9.5.0/balena_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2020-06-19 06:30:42.000000 balena-sdk-9.5.0/balena_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      140 2020-06-19 06:30:42.000000 balena-sdk-9.5.0/balena_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2020-06-19 06:30:42.000000 balena-sdk-9.5.0/balena_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2020-06-19 06:30:42.000000 balena-sdk-9.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     4035 2019-04-22 07:51:50.000000 balena-sdk-9.5.0/setup.py
```

### Comparing `balena-sdk-9.4.1/PKG-INFO` & `balena-sdk-9.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balena-sdk
-Version: 9.4.1
+Version: 9.5.0
 Summary: Balena SDK for Python
 Home-page: https://github.com/balena-io/balena-sdk-python
 Author: Balena
 Author-email: info@balena.io
 License: MIT
 Description: UNKNOWN
 Keywords: balena balena.io resin resin.io api sdk
```

### Comparing `balena-sdk-9.4.1/README.md` & `balena-sdk-9.5.0/README.md`

 * *Files identical despite different names*

### Comparing `balena-sdk-9.4.1/balena/__init__.py` & `balena-sdk-9.5.0/balena/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 from .auth import Auth
 from .logs import Logs
 from .settings import Settings
 from .models import Models
 from .twofactor_auth import TwoFactorAuth
 
 
-__version__ = '9.4.1'
+__version__ = '9.5.0'
 
 
 class Balena(object):
     """
     This class implements all functions supported by the python SDK.
     Attributes:
             settings (Settings): configuration settings for balena python SDK.
```

### Comparing `balena-sdk-9.4.1/balena/auth.py` & `balena-sdk-9.5.0/balena/auth.py`

 * *Files identical despite different names*

### Comparing `balena-sdk-9.4.1/balena/base_request.py` & `balena-sdk-9.5.0/balena/base_request.py`

 * *Files identical despite different names*

### Comparing `balena-sdk-9.4.1/balena/exceptions.py` & `balena-sdk-9.5.0/balena/exceptions.py`

 * *Files identical despite different names*

### Comparing `balena-sdk-9.4.1/balena/logs.py` & `balena-sdk-9.5.0/balena/logs.py`

 * *Files identical despite different names*

### Comparing `balena-sdk-9.4.1/balena/models/__init__.py` & `balena-sdk-9.5.0/balena/models/__init__.py`

 * *Files identical despite different names*

### Comparing `balena-sdk-9.4.1/balena/models/api_key.py` & `balena-sdk-9.5.0/balena/models/api_key.py`

 * *Files identical despite different names*

### Comparing `balena-sdk-9.4.1/balena/models/application.py` & `balena-sdk-9.5.0/balena/models/application.py`

 * *Files identical despite different names*

### Comparing `balena-sdk-9.4.1/balena/models/config.py` & `balena-sdk-9.5.0/balena/models/config.py`

 * *Files identical despite different names*

### Comparing `balena-sdk-9.4.1/balena/models/config_variable.py` & `balena-sdk-9.5.0/balena/models/config_variable.py`

 * *Files identical despite different names*

### Comparing `balena-sdk-9.4.1/balena/models/device.py` & `balena-sdk-9.5.0/balena/models/device.py`

 * *Files 1% similar despite different names*

```diff
@@ -1517,7 +1517,28 @@
                 'message': 'Supported'
             }
         except exceptions.LocalModeError as e:
             return {
                 'supported': False,
                 'message': e.message
             }
+
+    def get_mac_address(self, uuid):
+        """
+        Get the MAC addresses of a device.
+
+        Args:
+            uuid (str): device uuid.
+
+        Returns:
+            list: MAC addresses of a device.
+
+        Raises:
+            DeviceNotFound: if device couldn't be found.
+
+        """
+
+        device = self.get(uuid)
+        if 'mac_address' in device:
+            return device['mac_address'].split()
+        else:
+            return []
```

### Comparing `balena-sdk-9.4.1/balena/models/device_os.py` & `balena-sdk-9.5.0/balena/models/device_os.py`

 * *Files identical despite different names*

### Comparing `balena-sdk-9.4.1/balena/models/environment_variables.py` & `balena-sdk-9.5.0/balena/models/environment_variables.py`

 * *Files identical despite different names*

### Comparing `balena-sdk-9.4.1/balena/models/hup.py` & `balena-sdk-9.5.0/balena/models/hup.py`

 * *Files identical despite different names*

### Comparing `balena-sdk-9.4.1/balena/models/image.py` & `balena-sdk-9.5.0/balena/models/image.py`

 * *Files identical despite different names*

### Comparing `balena-sdk-9.4.1/balena/models/key.py` & `balena-sdk-9.5.0/balena/models/key.py`

 * *Files identical despite different names*

### Comparing `balena-sdk-9.4.1/balena/models/release.py` & `balena-sdk-9.5.0/balena/models/release.py`

 * *Files identical despite different names*

### Comparing `balena-sdk-9.4.1/balena/models/service.py` & `balena-sdk-9.5.0/balena/models/service.py`

 * *Files identical despite different names*

### Comparing `balena-sdk-9.4.1/balena/models/service_install.py` & `balena-sdk-9.5.0/balena/models/service_install.py`

 * *Files identical despite different names*

### Comparing `balena-sdk-9.4.1/balena/models/supervisor.py` & `balena-sdk-9.5.0/balena/models/supervisor.py`

 * *Files identical despite different names*

### Comparing `balena-sdk-9.4.1/balena/models/tag.py` & `balena-sdk-9.5.0/balena/models/tag.py`

 * *Files identical despite different names*

### Comparing `balena-sdk-9.4.1/balena/resources.py` & `balena-sdk-9.5.0/balena/resources.py`

 * *Files identical despite different names*

### Comparing `balena-sdk-9.4.1/balena/settings.py` & `balena-sdk-9.5.0/balena/settings.py`

 * *Files identical despite different names*

### Comparing `balena-sdk-9.4.1/balena/twofactor_auth.py` & `balena-sdk-9.5.0/balena/twofactor_auth.py`

 * *Files identical despite different names*

### Comparing `balena-sdk-9.4.1/balena_sdk.egg-info/PKG-INFO` & `balena-sdk-9.5.0/balena_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balena-sdk
-Version: 9.4.1
+Version: 9.5.0
 Summary: Balena SDK for Python
 Home-page: https://github.com/balena-io/balena-sdk-python
 Author: Balena
 Author-email: info@balena.io
 License: MIT
 Description: UNKNOWN
 Keywords: balena balena.io resin resin.io api sdk
```

### Comparing `balena-sdk-9.4.1/balena_sdk.egg-info/SOURCES.txt` & `balena-sdk-9.5.0/balena_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `balena-sdk-9.4.1/setup.py` & `balena-sdk-9.5.0/setup.py`

 * *Files identical despite different names*

