# Comparing `tmp/homeassistant-historical-sensor-2.0.0b0.tar.gz` & `tmp/homeassistant-historical-sensor-2.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "homeassistant-historical-sensor-2.0.0b0.tar", last modified: Thu Jul 13 17:04:54 2023, max compression
+gzip compressed data, was "homeassistant-historical-sensor-2.0.0rc1.tar", last modified: Mon Jul 17 15:31:58 2023, max compression
```

## Comparing `homeassistant-historical-sensor-2.0.0b0.tar` & `homeassistant-historical-sensor-2.0.0rc1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:04:54.034500 homeassistant-historical-sensor-2.0.0b0/
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-07-13 17:04:54.034500 homeassistant-historical-sensor-2.0.0b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-07-13 17:04:42.000000 homeassistant-historical-sensor-2.0.0b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:04:54.034500 homeassistant-historical-sensor-2.0.0b0/homeassistant_historical_sensor/
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-13 17:04:42.000000 homeassistant-historical-sensor-2.0.0b0/homeassistant_historical_sensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-07-13 17:04:42.000000 homeassistant-historical-sensor-2.0.0b0/homeassistant_historical_sensor/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-07-13 17:04:42.000000 homeassistant-historical-sensor-2.0.0b0/homeassistant_historical_sensor/patches.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-07-13 17:04:42.000000 homeassistant-historical-sensor-2.0.0b0/homeassistant_historical_sensor/recorderutil.py
--rw-r--r--   0 runner    (1001) docker     (123)    14575 2023-07-13 17:04:42.000000 homeassistant-historical-sensor-2.0.0b0/homeassistant_historical_sensor/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-13 17:04:42.000000 homeassistant-historical-sensor-2.0.0b0/homeassistant_historical_sensor/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:04:54.034500 homeassistant-historical-sensor-2.0.0b0/homeassistant_historical_sensor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-07-13 17:04:54.000000 homeassistant-historical-sensor-2.0.0b0/homeassistant_historical_sensor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-13 17:04:54.000000 homeassistant-historical-sensor-2.0.0b0/homeassistant_historical_sensor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 17:04:54.000000 homeassistant-historical-sensor-2.0.0b0/homeassistant_historical_sensor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-13 17:04:54.000000 homeassistant-historical-sensor-2.0.0b0/homeassistant_historical_sensor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-13 17:04:42.000000 homeassistant-historical-sensor-2.0.0b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-13 17:04:54.034500 homeassistant-historical-sensor-2.0.0b0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:31:58.910909 homeassistant-historical-sensor-2.0.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-17 15:31:58.910909 homeassistant-historical-sensor-2.0.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-07-17 15:31:47.000000 homeassistant-historical-sensor-2.0.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:31:58.906909 homeassistant-historical-sensor-2.0.0rc1/homeassistant_historical_sensor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-17 15:31:47.000000 homeassistant-historical-sensor-2.0.0rc1/homeassistant_historical_sensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-07-17 15:31:47.000000 homeassistant-historical-sensor-2.0.0rc1/homeassistant_historical_sensor/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-07-17 15:31:47.000000 homeassistant-historical-sensor-2.0.0rc1/homeassistant_historical_sensor/patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-07-17 15:31:47.000000 homeassistant-historical-sensor-2.0.0rc1/homeassistant_historical_sensor/recorderutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14581 2023-07-17 15:31:47.000000 homeassistant-historical-sensor-2.0.0rc1/homeassistant_historical_sensor/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-17 15:31:47.000000 homeassistant-historical-sensor-2.0.0rc1/homeassistant_historical_sensor/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:31:58.910909 homeassistant-historical-sensor-2.0.0rc1/homeassistant_historical_sensor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-17 15:31:58.000000 homeassistant-historical-sensor-2.0.0rc1/homeassistant_historical_sensor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-17 15:31:58.000000 homeassistant-historical-sensor-2.0.0rc1/homeassistant_historical_sensor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 15:31:58.000000 homeassistant-historical-sensor-2.0.0rc1/homeassistant_historical_sensor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-17 15:31:58.000000 homeassistant-historical-sensor-2.0.0rc1/homeassistant_historical_sensor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-17 15:31:47.000000 homeassistant-historical-sensor-2.0.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-17 15:31:58.910909 homeassistant-historical-sensor-2.0.0rc1/setup.cfg
```

### Comparing `homeassistant-historical-sensor-2.0.0b0/PKG-INFO` & `homeassistant-historical-sensor-2.0.0rc1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homeassistant-historical-sensor
-Version: 2.0.0b0
+Version: 2.0.0rc1
 Summary: Historical sensors for HomeAssistant
 Home-page: https://github.com/ldotlopez/ha-historical-sensor
 Author: Luis López
 Author-email: luis@cuarentaydos.com
 Project-URL: Repository, https://github.com/ldotlopez/ha-historical-sensor/
 Project-URL: Bug Tracker, https://github.com/ldotlopez/ha-historical-sensor/issues
 Requires-Python: >=3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: homeassistant-historical-sensor Version: 2.0.0b0
+Metadata-Version: 2.1 Name: homeassistant-historical-sensor Version: 2.0.0rc1
 Summary: Historical sensors for HomeAssistant Home-page: https://github.com/
 ldotlopez/ha-historical-sensor Author: Luis LÃ³pez Author-email:
 luis@cuarentaydos.com Project-URL: Repository, https://github.com/ldotlopez/ha-
 historical-sensor/ Project-URL: Bug Tracker, https://github.com/ldotlopez/ha-
 historical-sensor/issues Requires-Python: >=3.10 Description-Content-Type:
 text/markdown # Historical sensors for Home Assistant ![](icon-64.png)  !
 [GitHub Release (latest SemVer including pre-releases)](https://img.shields.io/
```

### Comparing `homeassistant-historical-sensor-2.0.0b0/README.md` & `homeassistant-historical-sensor-2.0.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `homeassistant-historical-sensor-2.0.0b0/homeassistant_historical_sensor/__init__.py` & `homeassistant-historical-sensor-2.0.0rc1/homeassistant_historical_sensor/__init__.py`

 * *Files identical despite different names*

### Comparing `homeassistant-historical-sensor-2.0.0b0/homeassistant_historical_sensor/consts.py` & `homeassistant-historical-sensor-2.0.0rc1/homeassistant_historical_sensor/consts.py`

 * *Files identical despite different names*

### Comparing `homeassistant-historical-sensor-2.0.0b0/homeassistant_historical_sensor/patches.py` & `homeassistant-historical-sensor-2.0.0rc1/homeassistant_historical_sensor/patches.py`

 * *Files identical despite different names*

### Comparing `homeassistant-historical-sensor-2.0.0b0/homeassistant_historical_sensor/recorderutil.py` & `homeassistant-historical-sensor-2.0.0rc1/homeassistant_historical_sensor/recorderutil.py`

 * *Files identical despite different names*

### Comparing `homeassistant-historical-sensor-2.0.0b0/homeassistant_historical_sensor/sensor.py` & `homeassistant-historical-sensor-2.0.0rc1/homeassistant_historical_sensor/sensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         # Setting state_class enables HomeAssistant to run statistic calculations on
         # this sensor.
         # We handle our own statistics and can be different from the Home Assisstant
         # ones (also, we don't fully understand some internal procedures of
         # HomeAssistant)
         #
 
-        if self.statistic_id and hasattr(self, "state_class"):
+        if self.statistic_id and getattr(self, "state_class", None):
             _LOGGER.warning(
                 f"{self.entity_id}: state_class attribute is set. "
                 "This is NOT supported, your statistics will be messed sooner or later"
             )
 
     @property
     def should_poll(self):
```

### Comparing `homeassistant-historical-sensor-2.0.0b0/homeassistant_historical_sensor/state.py` & `homeassistant-historical-sensor-2.0.0rc1/homeassistant_historical_sensor/state.py`

 * *Files identical despite different names*

### Comparing `homeassistant-historical-sensor-2.0.0b0/homeassistant_historical_sensor.egg-info/PKG-INFO` & `homeassistant-historical-sensor-2.0.0rc1/homeassistant_historical_sensor.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homeassistant-historical-sensor
-Version: 2.0.0b0
+Version: 2.0.0rc1
 Summary: Historical sensors for HomeAssistant
 Home-page: https://github.com/ldotlopez/ha-historical-sensor
 Author: Luis López
 Author-email: luis@cuarentaydos.com
 Project-URL: Repository, https://github.com/ldotlopez/ha-historical-sensor/
 Project-URL: Bug Tracker, https://github.com/ldotlopez/ha-historical-sensor/issues
 Requires-Python: >=3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: homeassistant-historical-sensor Version: 2.0.0b0
+Metadata-Version: 2.1 Name: homeassistant-historical-sensor Version: 2.0.0rc1
 Summary: Historical sensors for HomeAssistant Home-page: https://github.com/
 ldotlopez/ha-historical-sensor Author: Luis LÃ³pez Author-email:
 luis@cuarentaydos.com Project-URL: Repository, https://github.com/ldotlopez/ha-
 historical-sensor/ Project-URL: Bug Tracker, https://github.com/ldotlopez/ha-
 historical-sensor/issues Requires-Python: >=3.10 Description-Content-Type:
 text/markdown # Historical sensors for Home Assistant ![](icon-64.png)  !
 [GitHub Release (latest SemVer including pre-releases)](https://img.shields.io/
```

### Comparing `homeassistant-historical-sensor-2.0.0b0/homeassistant_historical_sensor.egg-info/SOURCES.txt` & `homeassistant-historical-sensor-2.0.0rc1/homeassistant_historical_sensor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `homeassistant-historical-sensor-2.0.0b0/setup.cfg` & `homeassistant-historical-sensor-2.0.0rc1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = homeassistant-historical-sensor
-version = 2.0.0b0
+version = 2.0.0rc1
 author = Luis López
 author_email = luis@cuarentaydos.com
 description = Historical sensors for HomeAssistant
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ldotlopez/ha-historical-sensor
 project_urls =
```

