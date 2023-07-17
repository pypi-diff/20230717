# Comparing `tmp/ecallisto_ng-0.1.7.tar.gz` & `tmp/ecallisto_ng-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecallisto_ng-0.1.7.tar", last modified: Mon Jul 17 09:45:51 2023, max compression
+gzip compressed data, was "ecallisto_ng-0.1.8.tar", last modified: Mon Jul 17 10:31:35 2023, max compression
```

## Comparing `ecallisto_ng-0.1.7.tar` & `ecallisto_ng-0.1.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-17 09:45:51.628325 ecallisto_ng-0.1.7/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1083 2023-07-06 16:13:05.000000 ecallisto_ng-0.1.7/LICENSE
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3608 2023-07-17 09:45:51.628325 ecallisto_ng-0.1.7/PKG-INFO
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3028 2023-07-17 09:45:19.000000 ecallisto_ng-0.1.7/README.md
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      858 2023-07-17 09:45:39.000000 ecallisto_ng-0.1.7/pyproject.toml
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)       38 2023-07-17 09:45:51.628325 ecallisto_ng-0.1.7/setup.cfg
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-17 09:45:51.628325 ecallisto_ng-0.1.7/src/
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-17 09:45:51.628325 ecallisto_ng-0.1.7/src/ecallisto_ng/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-06 17:35:07.000000 ecallisto_ng-0.1.7/src/ecallisto_ng/__init__.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-17 09:45:51.628325 ecallisto_ng-0.1.7/src/ecallisto_ng/data_fetching/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:39:51.000000 ecallisto_ng-0.1.7/src/ecallisto_ng/data_fetching/__init__.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     6190 2023-07-17 09:45:31.000000 ecallisto_ng-0.1.7/src/ecallisto_ng/data_fetching/get_data.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2006 2023-07-13 17:59:20.000000 ecallisto_ng-0.1.7/src/ecallisto_ng/data_fetching/get_information.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-17 09:45:51.628325 ecallisto_ng-0.1.7/src/ecallisto_ng/data_processing/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:39:54.000000 ecallisto_ng-0.1.7/src/ecallisto_ng/data_processing/__init__.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     5256 2023-07-11 08:45:15.000000 ecallisto_ng-0.1.7/src/ecallisto_ng/data_processing/utils.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-17 09:45:51.628325 ecallisto_ng-0.1.7/src/ecallisto_ng/plotting/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:40:01.000000 ecallisto_ng-0.1.7/src/ecallisto_ng/plotting/__init__.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2425 2023-07-10 17:56:33.000000 ecallisto_ng-0.1.7/src/ecallisto_ng/plotting/utils.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-17 09:45:51.628325 ecallisto_ng-0.1.7/src/ecallisto_ng.egg-info/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3608 2023-07-17 09:45:51.000000 ecallisto_ng-0.1.7/src/ecallisto_ng.egg-info/PKG-INFO
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      556 2023-07-17 09:45:51.000000 ecallisto_ng-0.1.7/src/ecallisto_ng.egg-info/SOURCES.txt
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        1 2023-07-17 09:45:51.000000 ecallisto_ng-0.1.7/src/ecallisto_ng.egg-info/dependency_links.txt
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      129 2023-07-17 09:45:51.000000 ecallisto_ng-0.1.7/src/ecallisto_ng.egg-info/requires.txt
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)       13 2023-07-17 09:45:51.000000 ecallisto_ng-0.1.7/src/ecallisto_ng.egg-info/top_level.txt
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-17 10:31:35.420928 ecallisto_ng-0.1.8/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1083 2023-07-06 16:13:05.000000 ecallisto_ng-0.1.8/LICENSE
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3608 2023-07-17 10:31:35.420928 ecallisto_ng-0.1.8/PKG-INFO
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3028 2023-07-17 09:45:19.000000 ecallisto_ng-0.1.8/README.md
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)      858 2023-07-17 10:28:05.000000 ecallisto_ng-0.1.8/pyproject.toml
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)       38 2023-07-17 10:31:35.420928 ecallisto_ng-0.1.8/setup.cfg
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-17 10:31:35.410095 ecallisto_ng-0.1.8/src/
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-17 10:31:35.420928 ecallisto_ng-0.1.8/src/ecallisto_ng/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-06 17:35:07.000000 ecallisto_ng-0.1.8/src/ecallisto_ng/__init__.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-17 10:31:35.420928 ecallisto_ng-0.1.8/src/ecallisto_ng/data_fetching/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:39:51.000000 ecallisto_ng-0.1.8/src/ecallisto_ng/data_fetching/__init__.py
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     6795 2023-07-17 10:27:28.000000 ecallisto_ng-0.1.8/src/ecallisto_ng/data_fetching/get_data.py
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2006 2023-07-13 17:59:20.000000 ecallisto_ng-0.1.8/src/ecallisto_ng/data_fetching/get_information.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-17 10:31:35.420928 ecallisto_ng-0.1.8/src/ecallisto_ng/data_processing/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:39:54.000000 ecallisto_ng-0.1.8/src/ecallisto_ng/data_processing/__init__.py
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     5256 2023-07-11 08:45:15.000000 ecallisto_ng-0.1.8/src/ecallisto_ng/data_processing/utils.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-17 10:31:35.420928 ecallisto_ng-0.1.8/src/ecallisto_ng/plotting/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:40:01.000000 ecallisto_ng-0.1.8/src/ecallisto_ng/plotting/__init__.py
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2425 2023-07-10 17:56:33.000000 ecallisto_ng-0.1.8/src/ecallisto_ng/plotting/utils.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-17 10:31:35.420928 ecallisto_ng-0.1.8/src/ecallisto_ng.egg-info/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3608 2023-07-17 10:31:35.000000 ecallisto_ng-0.1.8/src/ecallisto_ng.egg-info/PKG-INFO
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)      556 2023-07-17 10:31:35.000000 ecallisto_ng-0.1.8/src/ecallisto_ng.egg-info/SOURCES.txt
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        1 2023-07-17 10:31:35.000000 ecallisto_ng-0.1.8/src/ecallisto_ng.egg-info/dependency_links.txt
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)      129 2023-07-17 10:31:35.000000 ecallisto_ng-0.1.8/src/ecallisto_ng.egg-info/requires.txt
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)       13 2023-07-17 10:31:35.000000 ecallisto_ng-0.1.8/src/ecallisto_ng.egg-info/top_level.txt
```

### Comparing `ecallisto_ng-0.1.7/LICENSE` & `ecallisto_ng-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.1.7/PKG-INFO` & `ecallisto_ng-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecallisto_ng
-Version: 0.1.7
+Version: 0.1.8
 Summary: A Python package for the fetching (and some processing) of eCallisto data via the eCallisto API.
 Author-email: Vincenzo Timmel <vincenzo.timmel@fhnw.ch>
 Project-URL: Homepage, https://github.com/i4Ds/ecallisto_ng
 Project-URL: Bug Tracker, https://github.com/i4Ds/ecallisto_ng/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ecallisto_ng-0.1.7/README.md` & `ecallisto_ng-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.1.7/pyproject.toml` & `ecallisto_ng-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ecallisto_ng"
-version = "0.1.7"
+version = "0.1.8"
 authors = [{name = "Vincenzo Timmel", email = "vincenzo.timmel@fhnw.ch"}]
 description = "A Python package for the fetching (and some processing) of eCallisto data via the eCallisto API."
 readme = "README.md"
 
 requires-python = ">=3.9"
 
 classifiers = [
```

### Comparing `ecallisto_ng-0.1.7/src/ecallisto_ng/data_fetching/get_data.py` & `ecallisto_ng-0.1.8/src/ecallisto_ng/data_fetching/get_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 
 
 def get_data(
     instrument_name,
     start_datetime,
     end_datetime,
     timebucket=None,
-    agg_function=None
+    agg_function=None,
+    data_folder='ecallisto_ng_cache'
 ):
     """
     Get data from the eCallisto API. See: https://v000792.fhnw.ch/api/redoc
     Of course, this is just a wrapper around the requests.post function.
     Depending on the size, the request can take a while. For example, two
     weeks of data, aggregated in a specific way, can take around 20 seconds.
 
@@ -29,16 +30,16 @@
     end_datetime : str
         The end datetime of the data to get.
     timebucket : str
         In what time frame the data should be grouped (see timescaledb
         "timebucket" function)
     agg_function : str
         The aggregation function to use (see timescaledb "timebucket" function)
-    verbose : bool
-        Whether to print out the response from the API.
+    ecallisto_ng_cache : str
+        Where to save the cached data.
     Returns
     -------
     pandas.DataFrame
         A DataFrame containing the data from the eCallisto API.
     """
     data = {
         "instrument_name": instrument_name,
@@ -53,32 +54,41 @@
     )
 
     # Clean up dates to make it compatible with windows
     start_datetime = start_datetime.replace(":", "-")
     end_datetime = end_datetime.replace(":", "-")
 
     # Create file path
-    file_path = f"{instrument_name}_{start_datetime}_{end_datetime}_{timebucket}_{agg_function}.parquet"
+    file_path = os.path.join(data_folder, f"{instrument_name}_{start_datetime}_{end_datetime}_{timebucket}_{agg_function}.parquet")
+    os.makedirs(data_folder, exist_ok=True)
     if os.path.exists(file_path):
         print(f"Reading data from {file_path}")
         return pd.read_parquet(file_path)
     response = requests.post(BASE_URL + "/api/data", json=data, timeout=180)
 
     # Check if the request was successful
     if response.status_code == 200:
         # Get the URL for the parquet file
         parquet_url = response.json()["data_parquet_url"]
+        json_url = response.json()["info_json_url"]
 
         # Now we can start polling the URL until the parquet file is ready for download
         while True:
             # Try to download the parquet file
             file_response = requests.get(BASE_URL + parquet_url)
+            json_respone = requests.get(BASE_URL + json_url)
             
             # If the file is available, save it to disk
             if file_response.status_code == 200:
+                content_type = file_response.headers['Content-Type']
+                if content_type == 'application/json': # typical content-type for binary data, adjust if necessary
+                    print("Recieved json instead of parquet. This is usually because of an Error.")
+                    raise ValueError(json_respone.content)
+
+                # Check if file is not a json
                 with open(file_path, "wb") as f:
                     f.write(file_response.content)
                 return pd.read_parquet(file_path)
             elif file_response.status_code == 404:
                 # If the file is not found, sleep for a short period and try again
                 print("File not ready yet, waiting...")
                 time.sleep(5)
```

### Comparing `ecallisto_ng-0.1.7/src/ecallisto_ng/data_fetching/get_information.py` & `ecallisto_ng-0.1.8/src/ecallisto_ng/data_fetching/get_information.py`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.1.7/src/ecallisto_ng/data_processing/utils.py` & `ecallisto_ng-0.1.8/src/ecallisto_ng/data_processing/utils.py`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.1.7/src/ecallisto_ng/plotting/utils.py` & `ecallisto_ng-0.1.8/src/ecallisto_ng/plotting/utils.py`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.1.7/src/ecallisto_ng.egg-info/PKG-INFO` & `ecallisto_ng-0.1.8/src/ecallisto_ng.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecallisto-ng
-Version: 0.1.7
+Version: 0.1.8
 Summary: A Python package for the fetching (and some processing) of eCallisto data via the eCallisto API.
 Author-email: Vincenzo Timmel <vincenzo.timmel@fhnw.ch>
 Project-URL: Homepage, https://github.com/i4Ds/ecallisto_ng
 Project-URL: Bug Tracker, https://github.com/i4Ds/ecallisto_ng/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ecallisto_ng-0.1.7/src/ecallisto_ng.egg-info/SOURCES.txt` & `ecallisto_ng-0.1.8/src/ecallisto_ng.egg-info/SOURCES.txt`

 * *Files identical despite different names*

