# Comparing `tmp/pymetard-0.0.2.tar.gz` & `tmp/pymetard-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymetard-0.0.2.tar", last modified: Sun Jul 16 14:57:40 2023, max compression
+gzip compressed data, was "pymetard-0.0.3.tar", last modified: Mon Jul 17 04:21:46 2023, max compression
```

## Comparing `pymetard-0.0.2.tar` & `pymetard-0.0.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:57:40.773644 pymetard-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-16 14:57:31.000000 pymetard-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-16 14:57:40.773644 pymetard-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-16 14:57:31.000000 pymetard-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:57:40.769643 pymetard-0.0.2/pymetard/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-16 14:57:31.000000 pymetard-0.0.2/pymetard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-07-16 14:57:31.000000 pymetard-0.0.2/pymetard/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-16 14:57:31.000000 pymetard-0.0.2/pymetard/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:57:40.773644 pymetard-0.0.2/pymetard/metar/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-16 14:57:31.000000 pymetard-0.0.2/pymetard/metar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13049 2023-07-16 14:57:31.000000 pymetard-0.0.2/pymetard/metar/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-16 14:57:31.000000 pymetard-0.0.2/pymetard/metar/meteo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-16 14:57:31.000000 pymetard-0.0.2/pymetard/metar/station.py
--rw-r--r--   0 runner    (1001) docker     (123)   814165 2023-07-16 14:57:31.000000 pymetard-0.0.2/pymetard/metar/stations.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:57:40.769643 pymetard-0.0.2/pymetard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-16 14:57:40.000000 pymetard-0.0.2/pymetard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-16 14:57:40.000000 pymetard-0.0.2/pymetard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 14:57:40.000000 pymetard-0.0.2/pymetard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-16 14:57:40.000000 pymetard-0.0.2/pymetard.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-16 14:57:40.000000 pymetard-0.0.2/pymetard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-16 14:57:40.000000 pymetard-0.0.2/pymetard.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-16 14:57:31.000000 pymetard-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 14:57:40.773644 pymetard-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-16 14:57:31.000000 pymetard-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:57:40.773644 pymetard-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 14:57:31.000000 pymetard-0.0.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:57:40.773644 pymetard-0.0.2/tests/pymetard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 14:57:31.000000 pymetard-0.0.2/tests/pymetard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:57:40.773644 pymetard-0.0.2/tests/pymetard/metar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 14:57:31.000000 pymetard-0.0.2/tests/pymetard/metar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-16 14:57:31.000000 pymetard-0.0.2/tests/pymetard/metar/test_station.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:21:46.566873 pymetard-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-17 04:21:36.000000 pymetard-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-17 04:21:46.566873 pymetard-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-17 04:21:36.000000 pymetard-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:21:46.562873 pymetard-0.0.3/pymetard/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-17 04:21:36.000000 pymetard-0.0.3/pymetard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-07-17 04:21:36.000000 pymetard-0.0.3/pymetard/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-17 04:21:36.000000 pymetard-0.0.3/pymetard/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:21:46.562873 pymetard-0.0.3/pymetard/metar/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-17 04:21:36.000000 pymetard-0.0.3/pymetard/metar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13577 2023-07-17 04:21:36.000000 pymetard-0.0.3/pymetard/metar/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-17 04:21:36.000000 pymetard-0.0.3/pymetard/metar/meteo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-17 04:21:36.000000 pymetard-0.0.3/pymetard/metar/station.py
+-rw-r--r--   0 runner    (1001) docker     (123)   814165 2023-07-17 04:21:36.000000 pymetard-0.0.3/pymetard/metar/stations.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:21:46.562873 pymetard-0.0.3/pymetard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-17 04:21:46.000000 pymetard-0.0.3/pymetard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-17 04:21:46.000000 pymetard-0.0.3/pymetard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 04:21:46.000000 pymetard-0.0.3/pymetard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-17 04:21:46.000000 pymetard-0.0.3/pymetard.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-17 04:21:46.000000 pymetard-0.0.3/pymetard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-17 04:21:46.000000 pymetard-0.0.3/pymetard.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-17 04:21:36.000000 pymetard-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 04:21:46.566873 pymetard-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-17 04:21:36.000000 pymetard-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:21:46.566873 pymetard-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 04:21:36.000000 pymetard-0.0.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:21:46.566873 pymetard-0.0.3/tests/pymetard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 04:21:36.000000 pymetard-0.0.3/tests/pymetard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:21:46.566873 pymetard-0.0.3/tests/pymetard/metar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 04:21:36.000000 pymetard-0.0.3/tests/pymetard/metar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-17 04:21:36.000000 pymetard-0.0.3/tests/pymetard/metar/test_station.py
```

### Comparing `pymetard-0.0.2/LICENSE` & `pymetard-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pymetard-0.0.2/PKG-INFO` & `pymetard-0.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymetard
-Version: 0.0.2
+Version: 0.0.3
 Summary: Download parsed METAR data.
 Home-page: https://github.com/ai4time/pymetard
 Author: AI4Time
 Author-email: huang.yipeng@hotmail.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pymetard-0.0.2/pymetard/cli.py` & `pymetard-0.0.3/pymetard/cli.py`

 * *Files identical despite different names*

### Comparing `pymetard-0.0.2/pymetard/metar/downloader.py` & `pymetard-0.0.3/pymetard/metar/downloader.py`

 * *Files 5% similar despite different names*

```diff
@@ -360,14 +360,29 @@
         except requests.exceptions.ConnectionError as e:
             logger.error(
                 f"Failed to connect to {base_url} "
                 f"with params {params}. "
                 f"Error: {e}"
             )
             return False
+        except requests.exceptions.JSONDecodeError as e:
+            logger.error(
+                f"Failed to decode JSON response from {base_url} "
+                f"with params {params}. "
+                f"Response: {res.text}. "
+                f"Error: {e}"
+            )
+            return False
+        except Exception as e:
+            logger.error(
+                f"Failed to fetch data from {base_url} "
+                f"with params {params}. "
+                f"Error: {e}"
+            )
+            return False
 
         raw_metars = []
         for station in raw_json['STATION']:
             if 'OBSERVATIONS' not in station:
                 continue
             if 'metar_set_1' not in station['OBSERVATIONS']:
                 continue
```

### Comparing `pymetard-0.0.2/pymetard/metar/station.py` & `pymetard-0.0.3/pymetard/metar/station.py`

 * *Files identical despite different names*

### Comparing `pymetard-0.0.2/pymetard/metar/stations.txt` & `pymetard-0.0.3/pymetard/metar/stations.txt`

 * *Files identical despite different names*

### Comparing `pymetard-0.0.2/pymetard.egg-info/PKG-INFO` & `pymetard-0.0.3/pymetard.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymetard
-Version: 0.0.2
+Version: 0.0.3
 Summary: Download parsed METAR data.
 Home-page: https://github.com/ai4time/pymetard
 Author: AI4Time
 Author-email: huang.yipeng@hotmail.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pymetard-0.0.2/pymetard.egg-info/SOURCES.txt` & `pymetard-0.0.3/pymetard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymetard-0.0.2/setup.py` & `pymetard-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import io
 
 import setuptools
 
 
-CLIENT_VERSION = "0.0.2"
+CLIENT_VERSION = "0.0.3"
 PACKAGE_NAME = "pymetard"
 
 try:
     with io.open("README.md", encoding="utf-8") as f:
         LONG_DESCRIPTION = f.read()
 except FileNotFoundError:
     LONG_DESCRIPTION = ""
```

### Comparing `pymetard-0.0.2/tests/pymetard/metar/test_station.py` & `pymetard-0.0.3/tests/pymetard/metar/test_station.py`

 * *Files identical despite different names*

