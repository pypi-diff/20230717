# Comparing `tmp/busGal_api-0.1.0.1.tar.gz` & `tmp/busGal_api-0.1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "busGal_api-0.1.0.1.tar", last modified: Sun Jul 16 22:22:29 2023, max compression
+gzip compressed data, was "busGal_api-0.1.0.2.tar", last modified: Mon Jul 17 00:18:40 2023, max compression
```

## Comparing `busGal_api-0.1.0.1.tar` & `busGal_api-0.1.0.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:22:29.812866 busGal_api-0.1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35150 2023-07-16 22:22:16.000000 busGal_api-0.1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-16 22:22:29.812866 busGal_api-0.1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-07-16 22:22:16.000000 busGal_api-0.1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:22:29.804866 busGal_api-0.1.0.1/busGal_api/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-16 22:22:16.000000 busGal_api-0.1.0.1/busGal_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:22:29.808866 busGal_api-0.1.0.1/busGal_api/accounts/
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-16 22:22:16.000000 busGal_api-0.1.0.1/busGal_api/accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9409 2023-07-16 22:22:16.000000 busGal_api-0.1.0.1/busGal_api/accounts/accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-16 22:22:16.000000 busGal_api-0.1.0.1/busGal_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-16 22:22:16.000000 busGal_api-0.1.0.1/busGal_api/known_servers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-07-16 22:22:16.000000 busGal_api-0.1.0.1/busGal_api/rest_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:22:29.812866 busGal_api-0.1.0.1/busGal_api/transport/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-16 22:22:16.000000 busGal_api-0.1.0.1/busGal_api/transport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-16 22:22:16.000000 busGal_api-0.1.0.1/busGal_api/transport/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12317 2023-07-16 22:22:16.000000 busGal_api-0.1.0.1/busGal_api/transport/expeditions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-07-16 22:22:16.000000 busGal_api-0.1.0.1/busGal_api/transport/lines.py
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-07-16 22:22:16.000000 busGal_api-0.1.0.1/busGal_api/transport/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-07-16 22:22:16.000000 busGal_api-0.1.0.1/busGal_api/transport/rates.py
--rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-07-16 22:22:16.000000 busGal_api-0.1.0.1/busGal_api/transport/stops.py
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-07-16 22:22:16.000000 busGal_api-0.1.0.1/busGal_api/transport/warning_alerts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:22:29.808866 busGal_api-0.1.0.1/busGal_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-16 22:22:29.000000 busGal_api-0.1.0.1/busGal_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-16 22:22:29.000000 busGal_api-0.1.0.1/busGal_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 22:22:29.000000 busGal_api-0.1.0.1/busGal_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-16 22:22:29.000000 busGal_api-0.1.0.1/busGal_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-16 22:22:29.000000 busGal_api-0.1.0.1/busGal_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 22:22:29.812866 busGal_api-0.1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-16 22:22:16.000000 busGal_api-0.1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 00:18:40.005704 busGal_api-0.1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35150 2023-07-17 00:18:30.000000 busGal_api-0.1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-17 00:18:40.005704 busGal_api-0.1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-07-17 00:18:30.000000 busGal_api-0.1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 00:18:40.001704 busGal_api-0.1.0.2/busGal_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-17 00:18:30.000000 busGal_api-0.1.0.2/busGal_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 00:18:40.001704 busGal_api-0.1.0.2/busGal_api/accounts/
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-17 00:18:30.000000 busGal_api-0.1.0.2/busGal_api/accounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9409 2023-07-17 00:18:30.000000 busGal_api-0.1.0.2/busGal_api/accounts/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-17 00:18:30.000000 busGal_api-0.1.0.2/busGal_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-17 00:18:30.000000 busGal_api-0.1.0.2/busGal_api/known_servers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-07-17 00:18:30.000000 busGal_api-0.1.0.2/busGal_api/rest_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 00:18:40.005704 busGal_api-0.1.0.2/busGal_api/transport/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-17 00:18:30.000000 busGal_api-0.1.0.2/busGal_api/transport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-17 00:18:30.000000 busGal_api-0.1.0.2/busGal_api/transport/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12317 2023-07-17 00:18:30.000000 busGal_api-0.1.0.2/busGal_api/transport/expeditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-07-17 00:18:30.000000 busGal_api-0.1.0.2/busGal_api/transport/lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-07-17 00:18:30.000000 busGal_api-0.1.0.2/busGal_api/transport/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-07-17 00:18:30.000000 busGal_api-0.1.0.2/busGal_api/transport/rates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-07-17 00:18:30.000000 busGal_api-0.1.0.2/busGal_api/transport/stops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-07-17 00:18:30.000000 busGal_api-0.1.0.2/busGal_api/transport/warning_alerts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 00:18:40.001704 busGal_api-0.1.0.2/busGal_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-17 00:18:39.000000 busGal_api-0.1.0.2/busGal_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-17 00:18:39.000000 busGal_api-0.1.0.2/busGal_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 00:18:39.000000 busGal_api-0.1.0.2/busGal_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-17 00:18:39.000000 busGal_api-0.1.0.2/busGal_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-17 00:18:39.000000 busGal_api-0.1.0.2/busGal_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 00:18:40.005704 busGal_api-0.1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-17 00:18:30.000000 busGal_api-0.1.0.2/setup.py
```

### Comparing `busGal_api-0.1.0.1/LICENSE` & `busGal_api-0.1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `busGal_api-0.1.0.1/PKG-INFO` & `busGal_api-0.1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: busGal_api
-Version: 0.1.0.1
+Version: 0.1.0.2
 Summary: Python API wrapper for the galician public transport
 Home-page: https://github.com/peprolinbot/bus.gal-api
 Author: Pedro Rey Anca
 Author-email: contact@peprolinbot.com
 Project-URL: Bug Tracker, https://github.com/peprolinbot/bus.gal-api/issues
 Project-URL: Documentation, https://busgal-api.readthedocs.io/en/latest/
 Keywords: bus,buses,transport,public transport,galicia,api
```

### Comparing `busGal_api-0.1.0.1/README.md` & `busGal_api-0.1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `busGal_api-0.1.0.1/busGal_api/accounts/__init__.py` & `busGal_api-0.1.0.2/busGal_api/accounts/__init__.py`

 * *Files identical despite different names*

### Comparing `busGal_api-0.1.0.1/busGal_api/accounts/accounts.py` & `busGal_api-0.1.0.2/busGal_api/accounts/accounts.py`

 * *Files identical despite different names*

### Comparing `busGal_api-0.1.0.1/busGal_api/rest_adapter.py` & `busGal_api-0.1.0.2/busGal_api/rest_adapter.py`

 * *Files identical despite different names*

### Comparing `busGal_api-0.1.0.1/busGal_api/transport/__init__.py` & `busGal_api-0.1.0.2/busGal_api/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `busGal_api-0.1.0.1/busGal_api/transport/__main__.py` & `busGal_api-0.1.0.2/busGal_api/transport/__main__.py`

 * *Files identical despite different names*

### Comparing `busGal_api-0.1.0.1/busGal_api/transport/expeditions.py` & `busGal_api-0.1.0.2/busGal_api/transport/expeditions.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,15 +155,15 @@
         """
 
         self.polyline = polyline
         """
         It represents stops the expedition goes trough in a special format. Only given in `get_expedition_details`
         """
 
-        self.bos_dot_gal_url = f"https://www.bus.gal/gl/service/expedition/{self.id}/nojs?ori={self.origin.bus_stop_id}&des={self.destination.bus_stop_id}&date={self.origin.time.strftime('%Y-%m-%d')}"
+        self.bus_dot_gal_url = f"https://www.bus.gal/gl/service/expedition/{self.id}/nojs?ori={self.origin.bus_stop_id}&des={self.destination.bus_stop_id}&date={self.origin.time.strftime('%Y-%m-%d')}"
         """
         Url on bus.gal for the expedition's details page. Shows it's itinerary and looks good, so I put it in here
         """
 
     def __repr__(self):
         return f"{self.origin}  |  {self.origin.time.strftime('%H:%M')}  --->  {self.destination}  |  {self.destination.time.strftime('%H:%M')}"
```

### Comparing `busGal_api-0.1.0.1/busGal_api/transport/lines.py` & `busGal_api-0.1.0.2/busGal_api/transport/lines.py`

 * *Files identical despite different names*

### Comparing `busGal_api-0.1.0.1/busGal_api/transport/operators.py` & `busGal_api-0.1.0.2/busGal_api/transport/operators.py`

 * *Files identical despite different names*

### Comparing `busGal_api-0.1.0.1/busGal_api/transport/rates.py` & `busGal_api-0.1.0.2/busGal_api/transport/rates.py`

 * *Files identical despite different names*

### Comparing `busGal_api-0.1.0.1/busGal_api/transport/stops.py` & `busGal_api-0.1.0.2/busGal_api/transport/stops.py`

 * *Files identical despite different names*

### Comparing `busGal_api-0.1.0.1/busGal_api/transport/warning_alerts.py` & `busGal_api-0.1.0.2/busGal_api/transport/warning_alerts.py`

 * *Files identical despite different names*

### Comparing `busGal_api-0.1.0.1/busGal_api.egg-info/PKG-INFO` & `busGal_api-0.1.0.2/busGal_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: busGal-api
-Version: 0.1.0.1
+Version: 0.1.0.2
 Summary: Python API wrapper for the galician public transport
 Home-page: https://github.com/peprolinbot/bus.gal-api
 Author: Pedro Rey Anca
 Author-email: contact@peprolinbot.com
 Project-URL: Bug Tracker, https://github.com/peprolinbot/bus.gal-api/issues
 Project-URL: Documentation, https://busgal-api.readthedocs.io/en/latest/
 Keywords: bus,buses,transport,public transport,galicia,api
```

### Comparing `busGal_api-0.1.0.1/busGal_api.egg-info/SOURCES.txt` & `busGal_api-0.1.0.2/busGal_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `busGal_api-0.1.0.1/setup.py` & `busGal_api-0.1.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.0.1' 
+VERSION = '0.1.0.2' 
 DESCRIPTION = 'Python API wrapper for the galician public transport'
 with open("README.md", "r", encoding="utf-8") as fh:
     LONG_DESCRIPTION = fh.read()
 
 setup(
         name="busGal_api", 
         version=VERSION,
```

