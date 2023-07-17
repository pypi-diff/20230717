# Comparing `tmp/gridstatusio-0.2.2.tar.gz` & `tmp/gridstatusio-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/github/workspace/dist/.tmp-1gjkv42a/gridstatusio-0.2.2.tar", last modified: Thu May 18 00:13:59 2023, max compression
+gzip compressed data, was "/github/workspace/dist/.tmp-o9g5tupz/gridstatusio-0.2.3.tar", last modified: Mon Jul 17 14:52:05 2023, max compression
```

## Comparing `gridstatusio-0.2.2.tar` & `gridstatusio-0.2.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:13:59.000000 gridstatusio-0.2.2/
--rw-r--r--   0 root         (0) root         (0)     1461 2023-05-18 00:13:45.000000 gridstatusio-0.2.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3258 2023-05-18 00:13:59.000000 gridstatusio-0.2.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      848 2023-05-18 00:13:45.000000 gridstatusio-0.2.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:13:59.000000 gridstatusio-0.2.2/gridstatusio/
--rw-r--r--   0 root         (0) root         (0)       98 2023-05-18 00:13:45.000000 gridstatusio-0.2.2/gridstatusio/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8550 2023-05-18 00:13:45.000000 gridstatusio-0.2.2/gridstatusio/gs_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:13:59.000000 gridstatusio-0.2.2/gridstatusio/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:13:45.000000 gridstatusio-0.2.2/gridstatusio/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1315 2023-05-18 00:13:45.000000 gridstatusio-0.2.2/gridstatusio/tests/test_api.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 00:13:45.000000 gridstatusio-0.2.2/gridstatusio/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:13:59.000000 gridstatusio-0.2.2/gridstatusio.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3258 2023-05-18 00:13:59.000000 gridstatusio-0.2.2/gridstatusio.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      348 2023-05-18 00:13:59.000000 gridstatusio-0.2.2/gridstatusio.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 00:13:59.000000 gridstatusio-0.2.2/gridstatusio.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      237 2023-05-18 00:13:59.000000 gridstatusio-0.2.2/gridstatusio.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-05-18 00:13:59.000000 gridstatusio-0.2.2/gridstatusio.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2319 2023-05-18 00:13:45.000000 gridstatusio-0.2.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-18 00:13:59.000000 gridstatusio-0.2.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 14:52:05.000000 gridstatusio-0.2.3/
+-rw-r--r--   0 root         (0) root         (0)     1461 2023-07-17 14:51:49.000000 gridstatusio-0.2.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3293 2023-07-17 14:52:05.000000 gridstatusio-0.2.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      883 2023-07-17 14:51:49.000000 gridstatusio-0.2.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 14:52:05.000000 gridstatusio-0.2.3/gridstatusio/
+-rw-r--r--   0 root         (0) root         (0)       98 2023-07-17 14:51:49.000000 gridstatusio-0.2.3/gridstatusio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8735 2023-07-17 14:51:49.000000 gridstatusio-0.2.3/gridstatusio/gs_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 14:52:05.000000 gridstatusio-0.2.3/gridstatusio/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 14:51:49.000000 gridstatusio-0.2.3/gridstatusio/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1609 2023-07-17 14:51:49.000000 gridstatusio-0.2.3/gridstatusio/tests/test_api.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 14:51:49.000000 gridstatusio-0.2.3/gridstatusio/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 14:52:05.000000 gridstatusio-0.2.3/gridstatusio.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3293 2023-07-17 14:52:05.000000 gridstatusio-0.2.3/gridstatusio.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      348 2023-07-17 14:52:05.000000 gridstatusio-0.2.3/gridstatusio.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 14:52:05.000000 gridstatusio-0.2.3/gridstatusio.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      237 2023-07-17 14:52:05.000000 gridstatusio-0.2.3/gridstatusio.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-07-17 14:52:05.000000 gridstatusio-0.2.3/gridstatusio.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2319 2023-07-17 14:51:49.000000 gridstatusio-0.2.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-17 14:52:05.000000 gridstatusio-0.2.3/setup.cfg
```

### Comparing `gridstatusio-0.2.2/LICENSE` & `gridstatusio-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gridstatusio-0.2.2/PKG-INFO` & `gridstatusio-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridstatusio
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python Client for GridStatus.io API
 Author-email: Max Kanter <kmax12@gmail.com>
 Maintainer-email: Max Kanter <kmax12@gmail.com>
 License: Copyright 2022 James Max Kanter
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
         
@@ -34,20 +34,27 @@
 
 # GridStatus.io Hosted API
 
 Python client for accessing the [GridStatus.io Hosted API](https://www.gridstatus.io/api).
 
 ## Installation
 
-You can install GridStatus.io Hosted API by running the following command in your terminal or command prompt:
+gridstatusio supports python 3.8+. Install with pip:
 
 ```bash
 pip install gridstatusio
 ```
 
+Upgrade using the following command
+
+```
+python -m pip install --upgrade gridstatusio
+```
+
+
 ## Getting Started
 
 Check out this example notebook: [Getting Started](/Examples/Getting%20Started.ipynb)
 
 ## Open Source
 
 If you prefer to use an open source library that fetches data directly from the source, you can check out the [github repo](https://github.com/kmax12/gridstatus). For more information on Hosted API vs Open Source API, please see this [guide](https://api.gridstatus.io/docs#section/Getting-Started/Open-Source)
```

### Comparing `gridstatusio-0.2.2/README.md` & `gridstatusio-0.2.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 # GridStatus.io Hosted API
 
 Python client for accessing the [GridStatus.io Hosted API](https://www.gridstatus.io/api).
 
 ## Installation
 
-You can install GridStatus.io Hosted API by running the following command in your terminal or command prompt:
+gridstatusio supports python 3.8+. Install with pip:
 
 ```bash
 pip install gridstatusio
 ```
 
+Upgrade using the following command
+
+```
+python -m pip install --upgrade gridstatusio
+```
+
+
 ## Getting Started
 
 Check out this example notebook: [Getting Started](/Examples/Getting%20Started.ipynb)
 
 ## Open Source
 
 If you prefer to use an open source library that fetches data directly from the source, you can check out the [github repo](https://github.com/kmax12/gridstatus). For more information on Hosted API vs Open Source API, please see this [guide](https://api.gridstatus.io/docs#section/Getting-Started/Open-Source)
```

### Comparing `gridstatusio-0.2.2/gridstatusio/gs_client.py` & `gridstatusio-0.2.3/gridstatusio/gs_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -212,33 +212,38 @@
             page += 1
             # time.sleep(
             #     0.1
             # )  # Add a small delay to ensure the output is updated correctly
 
         print()  # Add a newline for cleaner output
 
-        df = pd.concat(dfs)
+        df = pd.concat(dfs).reset_index(drop=True)
 
         # Print the additional information
         cprint(f"\nTotal number of rows: {len(df)}", "cyan")
         cprint(f"Total Time: {round(total_time, 2)} seconds", "cyan")
         cprint(
             f"Average time per page: {round(total_time / (page - 1), 2)} seconds",
             "cyan",
         )
 
         # convert to datetime for any columns that end in _utc
+        # or are of type object
         for col in df.columns:
-            if col.endswith("_utc"):
-                df[col] = pd.to_datetime(df[col], utc=True)
+
+            if df[col].dtype == "object" or col.endswith("_utc"):
+                try:
+                    df[col] = pd.to_datetime(df[col], utc=True)
+                except ValueError:
+                    pass
 
                 if tz != "UTC":
                     df[col] = df[col].dt.tz_convert(tz)
                     # rename with _utc suffix
-                    df = df.rename(columns={col: col[:-4] + "_local"})
+                    df = df.rename(columns={col: col.replace("_utc", "") + "_local"})
 
         return df
 
 
 if __name__ == "__main__":
     import os
```

### Comparing `gridstatusio-0.2.2/gridstatusio/tests/test_api.py` & `gridstatusio-0.2.3/gridstatusio/tests/test_api.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,14 +21,15 @@
         len(datasets) >= min_results
     ), f"Expected at least {min_results} results with filter term '{filter_term}'"
 
 
 def _check_dataframe(df):
     assert isinstance(df, pd.DataFrame)
     assert len(df) > 0
+    assert df.index.is_unique
 
 
 def test_set_api_works():
     client = gs.GridStatusClient(api_key="test")
     assert client.api_key == "test"
 
 
@@ -44,7 +45,21 @@
     )
 
     _check_dataframe(df)
 
     # make sure min of interval_start_utc equals start
     assert df["interval_start_utc"].min().strftime("%Y-%m-%d") == start
     assert df["interval_end_utc"].max().strftime("%Y-%m-%d") == end
+
+
+def test_index_unique_multiple_pages():
+    start = "2023-01-01"
+    end = "2023-01-02"
+    df = client.get_dataset(
+        dataset="isone_fuel_mix",
+        start=start,
+        end=end,
+        verbose=True,
+        limit=100,
+    )
+
+    _check_dataframe(df)
```

### Comparing `gridstatusio-0.2.2/gridstatusio.egg-info/PKG-INFO` & `gridstatusio-0.2.3/gridstatusio.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridstatusio
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python Client for GridStatus.io API
 Author-email: Max Kanter <kmax12@gmail.com>
 Maintainer-email: Max Kanter <kmax12@gmail.com>
 License: Copyright 2022 James Max Kanter
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
         
@@ -34,20 +34,27 @@
 
 # GridStatus.io Hosted API
 
 Python client for accessing the [GridStatus.io Hosted API](https://www.gridstatus.io/api).
 
 ## Installation
 
-You can install GridStatus.io Hosted API by running the following command in your terminal or command prompt:
+gridstatusio supports python 3.8+. Install with pip:
 
 ```bash
 pip install gridstatusio
 ```
 
+Upgrade using the following command
+
+```
+python -m pip install --upgrade gridstatusio
+```
+
+
 ## Getting Started
 
 Check out this example notebook: [Getting Started](/Examples/Getting%20Started.ipynb)
 
 ## Open Source
 
 If you prefer to use an open source library that fetches data directly from the source, you can check out the [github repo](https://github.com/kmax12/gridstatus). For more information on Hosted API vs Open Source API, please see this [guide](https://api.gridstatus.io/docs#section/Getting-Started/Open-Source)
```

### Comparing `gridstatusio-0.2.2/pyproject.toml` & `gridstatusio-0.2.3/pyproject.toml`

 * *Files identical despite different names*

