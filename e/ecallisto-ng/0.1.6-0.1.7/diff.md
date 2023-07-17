# Comparing `tmp/ecallisto_ng-0.1.6.tar.gz` & `tmp/ecallisto_ng-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecallisto_ng-0.1.6.tar", last modified: Mon Jul 17 09:44:22 2023, max compression
+gzip compressed data, was "ecallisto_ng-0.1.7.tar", last modified: Mon Jul 17 09:45:51 2023, max compression
```

## Comparing `ecallisto_ng-0.1.6.tar` & `ecallisto_ng-0.1.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-17 09:44:22.578353 ecallisto_ng-0.1.6/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1083 2023-07-06 16:13:05.000000 ecallisto_ng-0.1.6/LICENSE
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3548 2023-07-17 09:44:22.578353 ecallisto_ng-0.1.6/PKG-INFO
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2967 2023-07-11 14:51:23.000000 ecallisto_ng-0.1.6/README.md
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      858 2023-07-17 09:43:27.000000 ecallisto_ng-0.1.6/pyproject.toml
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)       38 2023-07-17 09:44:22.578353 ecallisto_ng-0.1.6/setup.cfg
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-17 09:44:22.578353 ecallisto_ng-0.1.6/src/
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-17 09:44:22.578353 ecallisto_ng-0.1.6/src/ecallisto_ng/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-06 17:35:07.000000 ecallisto_ng-0.1.6/src/ecallisto_ng/__init__.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-17 09:44:22.578353 ecallisto_ng-0.1.6/src/ecallisto_ng/data_fetching/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:39:51.000000 ecallisto_ng-0.1.6/src/ecallisto_ng/data_fetching/__init__.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     6193 2023-07-17 09:44:10.000000 ecallisto_ng-0.1.6/src/ecallisto_ng/data_fetching/get_data.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2006 2023-07-13 17:59:20.000000 ecallisto_ng-0.1.6/src/ecallisto_ng/data_fetching/get_information.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-17 09:44:22.578353 ecallisto_ng-0.1.6/src/ecallisto_ng/data_processing/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:39:54.000000 ecallisto_ng-0.1.6/src/ecallisto_ng/data_processing/__init__.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     5256 2023-07-11 08:45:15.000000 ecallisto_ng-0.1.6/src/ecallisto_ng/data_processing/utils.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-17 09:44:22.578353 ecallisto_ng-0.1.6/src/ecallisto_ng/plotting/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:40:01.000000 ecallisto_ng-0.1.6/src/ecallisto_ng/plotting/__init__.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2425 2023-07-10 17:56:33.000000 ecallisto_ng-0.1.6/src/ecallisto_ng/plotting/utils.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-17 09:44:22.578353 ecallisto_ng-0.1.6/src/ecallisto_ng.egg-info/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3548 2023-07-17 09:44:22.000000 ecallisto_ng-0.1.6/src/ecallisto_ng.egg-info/PKG-INFO
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      556 2023-07-17 09:44:22.000000 ecallisto_ng-0.1.6/src/ecallisto_ng.egg-info/SOURCES.txt
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        1 2023-07-17 09:44:22.000000 ecallisto_ng-0.1.6/src/ecallisto_ng.egg-info/dependency_links.txt
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      129 2023-07-17 09:44:22.000000 ecallisto_ng-0.1.6/src/ecallisto_ng.egg-info/requires.txt
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)       13 2023-07-17 09:44:22.000000 ecallisto_ng-0.1.6/src/ecallisto_ng.egg-info/top_level.txt
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-17 09:45:51.628325 ecallisto_ng-0.1.7/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1083 2023-07-06 16:13:05.000000 ecallisto_ng-0.1.7/LICENSE
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3608 2023-07-17 09:45:51.628325 ecallisto_ng-0.1.7/PKG-INFO
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3028 2023-07-17 09:45:19.000000 ecallisto_ng-0.1.7/README.md
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)      858 2023-07-17 09:45:39.000000 ecallisto_ng-0.1.7/pyproject.toml
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)       38 2023-07-17 09:45:51.628325 ecallisto_ng-0.1.7/setup.cfg
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-17 09:45:51.628325 ecallisto_ng-0.1.7/src/
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-17 09:45:51.628325 ecallisto_ng-0.1.7/src/ecallisto_ng/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-06 17:35:07.000000 ecallisto_ng-0.1.7/src/ecallisto_ng/__init__.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-17 09:45:51.628325 ecallisto_ng-0.1.7/src/ecallisto_ng/data_fetching/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:39:51.000000 ecallisto_ng-0.1.7/src/ecallisto_ng/data_fetching/__init__.py
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     6190 2023-07-17 09:45:31.000000 ecallisto_ng-0.1.7/src/ecallisto_ng/data_fetching/get_data.py
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2006 2023-07-13 17:59:20.000000 ecallisto_ng-0.1.7/src/ecallisto_ng/data_fetching/get_information.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-17 09:45:51.628325 ecallisto_ng-0.1.7/src/ecallisto_ng/data_processing/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:39:54.000000 ecallisto_ng-0.1.7/src/ecallisto_ng/data_processing/__init__.py
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     5256 2023-07-11 08:45:15.000000 ecallisto_ng-0.1.7/src/ecallisto_ng/data_processing/utils.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-17 09:45:51.628325 ecallisto_ng-0.1.7/src/ecallisto_ng/plotting/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:40:01.000000 ecallisto_ng-0.1.7/src/ecallisto_ng/plotting/__init__.py
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2425 2023-07-10 17:56:33.000000 ecallisto_ng-0.1.7/src/ecallisto_ng/plotting/utils.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-17 09:45:51.628325 ecallisto_ng-0.1.7/src/ecallisto_ng.egg-info/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3608 2023-07-17 09:45:51.000000 ecallisto_ng-0.1.7/src/ecallisto_ng.egg-info/PKG-INFO
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)      556 2023-07-17 09:45:51.000000 ecallisto_ng-0.1.7/src/ecallisto_ng.egg-info/SOURCES.txt
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        1 2023-07-17 09:45:51.000000 ecallisto_ng-0.1.7/src/ecallisto_ng.egg-info/dependency_links.txt
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)      129 2023-07-17 09:45:51.000000 ecallisto_ng-0.1.7/src/ecallisto_ng.egg-info/requires.txt
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)       13 2023-07-17 09:45:51.000000 ecallisto_ng-0.1.7/src/ecallisto_ng.egg-info/top_level.txt
```

### Comparing `ecallisto_ng-0.1.6/LICENSE` & `ecallisto_ng-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.1.6/PKG-INFO` & `ecallisto_ng-0.1.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecallisto_ng
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Python package for the fetching (and some processing) of eCallisto data via the eCallisto API.
 Author-email: Vincenzo Timmel <vincenzo.timmel@fhnw.ch>
 Project-URL: Homepage, https://github.com/i4Ds/ecallisto_ng
 Project-URL: Bug Tracker, https://github.com/i4Ds/ecallisto_ng/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -79,8 +79,8 @@
 df = fill_missing_timesteps_with_nan(df)
 df = subtract_constant_background(df)
 df = subtract_rolling_background(df)
 
 plot_spectogram(df,  parameters["instrument_name"], parameters["start_datetime"], parameters["end_datetime"])
 ```
 These simple commands allow you to easily manipulate spectogram data, enabling effective use of the Ecallisto API for your needs.
-Be careful when using 
+Be careful when using `elimwrongchannels` after `fill_missing_timesteps_with_nan`.
```

### Comparing `ecallisto_ng-0.1.6/README.md` & `ecallisto_ng-0.1.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -65,8 +65,8 @@
 df = fill_missing_timesteps_with_nan(df)
 df = subtract_constant_background(df)
 df = subtract_rolling_background(df)
 
 plot_spectogram(df,  parameters["instrument_name"], parameters["start_datetime"], parameters["end_datetime"])
 ```
 These simple commands allow you to easily manipulate spectogram data, enabling effective use of the Ecallisto API for your needs.
-Be careful when using 
+Be careful when using `elimwrongchannels` after `fill_missing_timesteps_with_nan`.
```

### Comparing `ecallisto_ng-0.1.6/pyproject.toml` & `ecallisto_ng-0.1.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ecallisto_ng"
-version = "0.1.6"
+version = "0.1.7"
 authors = [{name = "Vincenzo Timmel", email = "vincenzo.timmel@fhnw.ch"}]
 description = "A Python package for the fetching (and some processing) of eCallisto data via the eCallisto API."
 readme = "README.md"
 
 requires-python = ">=3.9"
 
 classifiers = [
```

### Comparing `ecallisto_ng-0.1.6/src/ecallisto_ng/data_fetching/get_data.py` & `ecallisto_ng-0.1.7/src/ecallisto_ng/data_fetching/get_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,18 +47,19 @@
         "timebucket": timebucket,
         "agg_function": agg_function
     }
 
     assert pd.to_datetime(start_datetime) <= pd.to_datetime(end_datetime), (
         f"start_datetime ({start_datetime}) must be before end_datetime ({end_datetime})"
     )
+
     # Clean up dates to make it compatible with windows
     start_datetime = start_datetime.replace(":", "-")
     end_datetime = end_datetime.replace(":", "-")
-    
+
     # Create file path
     file_path = f"{instrument_name}_{start_datetime}_{end_datetime}_{timebucket}_{agg_function}.parquet"
     if os.path.exists(file_path):
         print(f"Reading data from {file_path}")
         return pd.read_parquet(file_path)
     response = requests.post(BASE_URL + "/api/data", json=data, timeout=180)
```

### Comparing `ecallisto_ng-0.1.6/src/ecallisto_ng/data_fetching/get_information.py` & `ecallisto_ng-0.1.7/src/ecallisto_ng/data_fetching/get_information.py`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.1.6/src/ecallisto_ng/data_processing/utils.py` & `ecallisto_ng-0.1.7/src/ecallisto_ng/data_processing/utils.py`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.1.6/src/ecallisto_ng/plotting/utils.py` & `ecallisto_ng-0.1.7/src/ecallisto_ng/plotting/utils.py`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.1.6/src/ecallisto_ng.egg-info/PKG-INFO` & `ecallisto_ng-0.1.7/src/ecallisto_ng.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecallisto-ng
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Python package for the fetching (and some processing) of eCallisto data via the eCallisto API.
 Author-email: Vincenzo Timmel <vincenzo.timmel@fhnw.ch>
 Project-URL: Homepage, https://github.com/i4Ds/ecallisto_ng
 Project-URL: Bug Tracker, https://github.com/i4Ds/ecallisto_ng/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -79,8 +79,8 @@
 df = fill_missing_timesteps_with_nan(df)
 df = subtract_constant_background(df)
 df = subtract_rolling_background(df)
 
 plot_spectogram(df,  parameters["instrument_name"], parameters["start_datetime"], parameters["end_datetime"])
 ```
 These simple commands allow you to easily manipulate spectogram data, enabling effective use of the Ecallisto API for your needs.
-Be careful when using 
+Be careful when using `elimwrongchannels` after `fill_missing_timesteps_with_nan`.
```

### Comparing `ecallisto_ng-0.1.6/src/ecallisto_ng.egg-info/SOURCES.txt` & `ecallisto_ng-0.1.7/src/ecallisto_ng.egg-info/SOURCES.txt`

 * *Files identical despite different names*

