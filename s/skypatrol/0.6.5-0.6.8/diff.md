# Comparing `tmp/skypatrol-0.6.5.tar.gz` & `tmp/skypatrol-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skypatrol-0.6.5.tar", last modified: Thu Sep 22 05:38:34 2022, max compression
+gzip compressed data, was "skypatrol-0.6.8.tar", last modified: Thu Feb 16 00:12:46 2023, max compression
```

## Comparing `skypatrol-0.6.5.tar` & `skypatrol-0.6.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2022-09-22 05:38:34.616889 skypatrol-0.6.5/
--rw-r--r--   0 daniel     (501) staff       (20)    35129 2022-09-12 22:39:52.000000 skypatrol-0.6.5/LICENSE
--rw-r--r--   0 daniel     (501) staff       (20)      236 2022-09-22 05:38:34.616760 skypatrol-0.6.5/PKG-INFO
--rw-r--r--   0 daniel     (501) staff       (20)    29901 2022-09-12 22:39:52.000000 skypatrol-0.6.5/README.md
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2022-09-22 05:38:34.615740 skypatrol-0.6.5/pyasassn/
--rw-r--r--   0 daniel     (501) staff       (20)        0 2022-09-12 22:39:52.000000 skypatrol-0.6.5/pyasassn/__init__.py
--rw-r--r--   0 daniel     (501) staff       (20)    23349 2022-09-22 05:36:19.000000 skypatrol-0.6.5/pyasassn/client.py
--rw-r--r--   0 daniel     (501) staff       (20)    15086 2022-09-12 22:39:52.000000 skypatrol-0.6.5/pyasassn/utils.py
--rw-r--r--   0 daniel     (501) staff       (20)       38 2022-09-22 05:38:34.616928 skypatrol-0.6.5/setup.cfg
--rw-r--r--   0 daniel     (501) staff       (20)      798 2022-09-22 05:36:19.000000 skypatrol-0.6.5/setup.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2022-09-22 05:38:34.616591 skypatrol-0.6.5/skypatrol.egg-info/
--rw-r--r--   0 daniel     (501) staff       (20)      236 2022-09-22 05:38:34.000000 skypatrol-0.6.5/skypatrol.egg-info/PKG-INFO
--rw-r--r--   0 daniel     (501) staff       (20)      280 2022-09-22 05:38:34.000000 skypatrol-0.6.5/skypatrol.egg-info/SOURCES.txt
--rw-r--r--   0 daniel     (501) staff       (20)        1 2022-09-22 05:38:34.000000 skypatrol-0.6.5/skypatrol.egg-info/dependency_links.txt
--rw-r--r--   0 daniel     (501) staff       (20)        1 2022-09-12 22:46:42.000000 skypatrol-0.6.5/skypatrol.egg-info/not-zip-safe
--rw-r--r--   0 daniel     (501) staff       (20)       49 2022-09-22 05:38:34.000000 skypatrol-0.6.5/skypatrol.egg-info/requires.txt
--rw-r--r--   0 daniel     (501) staff       (20)        9 2022-09-22 05:38:34.000000 skypatrol-0.6.5/skypatrol.egg-info/top_level.txt
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-02-16 00:12:46.671013 skypatrol-0.6.8/
+-rw-r--r--   0 daniel     (501) staff       (20)    35129 2023-02-14 21:33:14.000000 skypatrol-0.6.8/LICENSE
+-rw-r--r--   0 daniel     (501) staff       (20)      191 2023-02-16 00:12:46.670887 skypatrol-0.6.8/PKG-INFO
+-rw-r--r--   0 daniel     (501) staff       (20)    29901 2023-02-14 21:33:14.000000 skypatrol-0.6.8/README.md
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-02-16 00:12:46.669819 skypatrol-0.6.8/pyasassn/
+-rw-r--r--   0 daniel     (501) staff       (20)        0 2023-02-14 21:33:14.000000 skypatrol-0.6.8/pyasassn/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)    24422 2023-02-14 21:33:14.000000 skypatrol-0.6.8/pyasassn/client.py
+-rw-r--r--   0 daniel     (501) staff       (20)    19121 2023-02-14 21:33:14.000000 skypatrol-0.6.8/pyasassn/utils.py
+-rw-r--r--   0 daniel     (501) staff       (20)       38 2023-02-16 00:12:46.671049 skypatrol-0.6.8/setup.cfg
+-rw-r--r--   0 daniel     (501) staff       (20)      798 2023-02-14 21:33:14.000000 skypatrol-0.6.8/setup.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-02-16 00:12:46.670729 skypatrol-0.6.8/skypatrol.egg-info/
+-rw-r--r--   0 daniel     (501) staff       (20)      191 2023-02-16 00:12:46.000000 skypatrol-0.6.8/skypatrol.egg-info/PKG-INFO
+-rw-r--r--   0 daniel     (501) staff       (20)      280 2023-02-16 00:12:46.000000 skypatrol-0.6.8/skypatrol.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel     (501) staff       (20)        1 2023-02-16 00:12:46.000000 skypatrol-0.6.8/skypatrol.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel     (501) staff       (20)        1 2023-02-14 21:33:42.000000 skypatrol-0.6.8/skypatrol.egg-info/not-zip-safe
+-rw-r--r--   0 daniel     (501) staff       (20)       49 2023-02-16 00:12:46.000000 skypatrol-0.6.8/skypatrol.egg-info/requires.txt
+-rw-r--r--   0 daniel     (501) staff       (20)        9 2023-02-16 00:12:46.000000 skypatrol-0.6.8/skypatrol.egg-info/top_level.txt
```

### Comparing `skypatrol-0.6.5/LICENSE` & `skypatrol-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `skypatrol-0.6.5/README.md` & `skypatrol-0.6.8/README.md`

 * *Files identical despite different names*

### Comparing `skypatrol-0.6.5/pyasassn/client.py` & `skypatrol-0.6.8/pyasassn/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 import requests
 import pandas as pd
 import json
 import numpy as np
 import multiprocessing
 import re
 import os
-import pyarrow as pa
-import warnings
+import io
+import traceback
+from time import sleep
 
 from .utils import LightCurveCollection
 
 
 class SkyPatrolClient:
     """
             The SkyPatrolClient allows users to interact with the ASAS-SN Sky Patrol photometry database.
@@ -148,18 +149,20 @@
         if catalog not in self.catalogs.catalog_names() or catalog in [
             "asteroids",
             "comets",
         ]:
             raise ValueError("invalid catalog")
         if cols is None:
             cols = ["asas_sn_id", "ra_deg", "dec_deg"]
-            if catalog not in ["stellar_main", "master_list"]:
-                cols.append("name")
+            if catalog == "m_giants":
+                cols.append("gaia_id")
             elif catalog == "master_list":
                 cols.append("catalog_sources")
+            elif catalog not in ["stellar_main", "master_list"]:
+                cols.append("name")
         if set(cols).issubset(set(self.catalogs[catalog]["col_names"])) is False:
             raise ValueError(
                 "one or more of the listed cols is not a column name in the selected catalog"
             )
 
         # Change units
         if units != "deg":
@@ -250,30 +253,32 @@
 
         # Check catalog columns
         if id_col not in list(self.catalogs[catalog]["col_names"]):
             raise ValueError("invalid column")
         # Set default columns
         if cols is None and catalog not in ["asteroids", "comets"]:
             cols = ["asas_sn_id", "ra_deg", "dec_deg"]
-            if catalog not in ["stellar_main", "master_list"]:
-                cols.append("name")
+            if catalog == "m_giants":
+                cols.append("gaia_id")
             elif catalog == "master_list":
                 cols.append("catalog_sources")
+            elif catalog not in ["stellar_main", "master_list"]:
+                cols.append("name")
         if cols is None and catalog in ["asteroids", "comets"]:
             cols = ["name"]
         # Ensure valid columns
         if set(cols).issubset(set(self.catalogs[catalog]["col_names"])) is False:
             raise ValueError(
                 "one or more of the listed cols is not a column name in the selected catalog"
             )
         if id_col not in cols:
             cols.append(id_col)
 
         if type(target_ids) in [str, int]:
-            tar_ids = [target_ids]
+            target_ids = [target_ids]
 
         # Query API with list (POST METHOD)
         url = f"http://asassn-lb01.ifa.hawaii.edu:9006/lookup_targets/catalog_list"
         response = requests.post(
             url,
             json={
                 "tar_ids": target_ids,
@@ -346,18 +351,20 @@
             raise ValueError("'threads' must be integer value")
         # Valid catalogs
         if catalog not in self.catalogs.catalog_names():
             raise ValueError("invalid catalog")
         # Set default columns
         if cols is None and catalog not in ["asteroids", "comets"]:
             cols = ["asas_sn_id", "ra_deg", "dec_deg"]
-            if catalog not in ["stellar_main", "master_list"]:
-                cols.append("name")
+            if catalog == "m_giants":
+                cols.append("gaia_id")
             elif catalog == "master_list":
                 cols.append("catalog_sources")
+            elif catalog not in ["stellar_main", "master_list"]:
+                cols.append("name")
         if cols is None and catalog in ["asteroids", "comets"]:
             cols = ["name"]
         # Ensure valid columns
         if set(cols).issubset(set(self.catalogs[catalog]["col_names"])) is False:
             raise ValueError(
                 "one or more of the listed cols is not a column name in the selected catalog"
             )
@@ -439,25 +446,52 @@
             data = pd.concat(chunks)
             id_col = "asas_sn_id" if catalog not in ["asteroids", "comets"] else "name"
             return LightCurveCollection(data, self.index, id_col)
 
     def _get_lightcurve_chunk(
         self, query_hash, block_idx, catalog, save_dir, file_format
     ):
-        # Query API with (POST METHOD)
-        url = (
-            f"http://{self.block_servers[block_idx % len(self.block_servers)]}:9006/get_block/"
-            f"query_hash-{query_hash}-block_idx-{block_idx}-catalog-{catalog}"
-        )
-        response = requests.get(url).content
+        # Available servers
+        n_servers = len(self.block_servers)
+        # Start timeout at 0
+        timeout = 1
+        # Download server (for balance)
+        server_idx = block_idx % n_servers
+        # Success flag
+        success = False
+
+        # Loop through until we download or timeout
+        while success is False and timeout <= 5:
+            try:            
+                # Query API with (POST METHOD)
+                url = (
+                    f"http://{self.block_servers[server_idx]}:9006/get_block/"
+                    f"query_hash-{query_hash}-block_idx-{block_idx}-catalog-{catalog}"
+                )
+                response = requests.get(url)
+
+                # Pandas dataframe
+                data = _deserialize(response.content)
+                # ID and count
+                id_col = "asas_sn_id" if catalog not in ["asteroids", "comets"] else "name"
+                count = len(data[id_col].unique())
+
+                success = True
+            except:
+                sleep(timeout)
+                server_idx = (server_idx + 1) % n_servers
+                
+                # Raise timeout if we've tried all servers once
+                if (server_idx % n_servers) == (block_idx % n_servers):
+                    timeout += 1
+        
+        # If download fails, raise exception 
+        if success is False:
+            raise TimeoutError("Lightcurve servers unavailable, try again later")
 
-        # Pandas dataframe
-        data = _deserialize(response)
-        id_col = "asas_sn_id" if catalog not in ["asteroids", "comets"] else "name"
-        count = len(data[id_col].unique())
         # Write to disk or return in memory
         if save_dir is not None:
             lcs = LightCurveCollection(data, self.index, id_col)
             return lcs.save(save_dir, file_format, include_index=False), count
         else:
             return data, count
 
@@ -530,20 +564,17 @@
             """
             return self.__dict__.keys()
 
         def __getitem__(self, item):
             return self.__dict__[item]
 
 
-def _deserialize(response):
-    # Deserialize from arrow
-    with warnings.catch_warnings():
-        warnings.simplefilter(action="ignore", category=FutureWarning)
-        buff = pa.py_buffer(response)
-        return pa.deserialize(buff)
+def _deserialize(buffer):
+    # Deserialize from bytes
+    return pd.read_parquet(io.BytesIO(buffer))
 
 
 def _arc_to_deg(arc, unit):
     """
     Convert arc minutes or seconds to decimal degree units
 
     :param arc: length of arc, float or np array
@@ -570,21 +601,21 @@
         index = pd.read_parquet(os.path.join(save_dir, "index.parq"))
         files = glob(os.path.join(save_dir, "*.parq"))
         lc_files = list(filter(lambda i: os.path.basename(i) != "index.parq", files))
         data = pd.concat(pd.read_parquet(file) for file in lc_files)
 
     elif file_format == "pickle":
         index = pd.read_pickle(os.path.join(save_dir, "index.pkl"))
-        lc_files = glob(os.path.join(save_dir, "*.pkl"))
+        files = glob(os.path.join(save_dir, "*.pkl"))
         lc_files = list(filter(lambda i: os.path.basename(i) != "index.pkl", files))
         data = pd.concat(pd.read_pickle(file) for file in lc_files)
 
     elif file_format == "csv":
         index = pd.read_csv(os.path.join(save_dir, "index.csv"))
-        lc_files = glob(os.path.join(save_dir, "*.csv"))
+        files = glob(os.path.join(save_dir, "*.csv"))
         lc_files = list(filter(lambda i: os.path.basename(i) != "index.csv", files))
         data = pd.concat(pd.read_csv(file) for file in lc_files)
 
     else:
         raise ValueError(
             f"invalid format: '{file_format}' not in ['parquet', 'csv', 'pickle']"
         )
```

### Comparing `skypatrol-0.6.5/setup.py` & `skypatrol-0.6.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 # Get dependencies
 with open("requirements.txt") as f:
     install_requires = f.read().splitlines()
 
 setup(
     name="skypatrol",
-    version="0.6.5",
+    version="0.6.8",
     url="https://github.com/asas_sn/skypatrol/",
     author="ASAS-SN",
     author_email="kylehart@hawaii.edu",
     license="GPL v.3",
     packages=["pyasassn"],
     install_requires=install_requires,
     zip_safe=False,
```

