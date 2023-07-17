# Comparing `tmp/pynkdv-0.0.8.tar.gz` & `tmp/pynkdv-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynkdv-0.0.8.tar", last modified: Sun Apr  2 08:11:30 2023, max compression
+gzip compressed data, was "pynkdv-0.0.9.tar", last modified: Sun Apr  2 08:58:12 2023, max compression
```

## Comparing `pynkdv-0.0.8.tar` & `pynkdv-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 patrick    (502) staff       (20)        0 2023-04-02 08:11:30.271074 pynkdv-0.0.8/
--rw-r--r--   0 patrick    (502) staff       (20)      179 2023-04-02 08:11:30.270719 pynkdv-0.0.8/PKG-INFO
-drwxr-xr-x   0 patrick    (502) staff       (20)        0 2023-04-02 08:11:30.268443 pynkdv-0.0.8/pynkdv/
--rw-r--r--   0 patrick    (502) staff       (20)     9229 2023-04-02 08:11:27.000000 pynkdv-0.0.8/pynkdv/PyNKDV.py
--rw-r--r--   0 patrick    (502) staff       (20)       21 2023-03-28 04:41:44.000000 pynkdv-0.0.8/pynkdv/__init__.py
-drwxr-xr-x   0 patrick    (502) staff       (20)        0 2023-04-02 08:11:30.270316 pynkdv-0.0.8/pynkdv.egg-info/
--rw-r--r--   0 patrick    (502) staff       (20)      179 2023-04-02 08:11:30.000000 pynkdv-0.0.8/pynkdv.egg-info/PKG-INFO
--rw-r--r--   0 patrick    (502) staff       (20)      193 2023-04-02 08:11:30.000000 pynkdv-0.0.8/pynkdv.egg-info/SOURCES.txt
--rw-r--r--   0 patrick    (502) staff       (20)        1 2023-04-02 08:11:30.000000 pynkdv-0.0.8/pynkdv.egg-info/dependency_links.txt
--rw-r--r--   0 patrick    (502) staff       (20)       42 2023-04-02 08:11:30.000000 pynkdv-0.0.8/pynkdv.egg-info/requires.txt
--rw-r--r--   0 patrick    (502) staff       (20)        7 2023-04-02 08:11:30.000000 pynkdv-0.0.8/pynkdv.egg-info/top_level.txt
--rw-r--r--   0 patrick    (502) staff       (20)       38 2023-04-02 08:11:30.271181 pynkdv-0.0.8/setup.cfg
--rw-r--r--   0 patrick    (502) staff       (20)      401 2023-04-02 08:11:27.000000 pynkdv-0.0.8/setup.py
+drwxr-xr-x   0 patrick    (502) staff       (20)        0 2023-04-02 08:58:12.660232 pynkdv-0.0.9/
+-rw-r--r--   0 patrick    (502) staff       (20)      179 2023-04-02 08:58:12.659951 pynkdv-0.0.9/PKG-INFO
+drwxr-xr-x   0 patrick    (502) staff       (20)        0 2023-04-02 08:58:12.657784 pynkdv-0.0.9/pynkdv/
+-rw-r--r--   0 patrick    (502) staff       (20)     9303 2023-04-02 08:57:54.000000 pynkdv-0.0.9/pynkdv/PyNKDV.py
+-rw-r--r--   0 patrick    (502) staff       (20)       21 2023-03-28 04:41:44.000000 pynkdv-0.0.9/pynkdv/__init__.py
+drwxr-xr-x   0 patrick    (502) staff       (20)        0 2023-04-02 08:58:12.659600 pynkdv-0.0.9/pynkdv.egg-info/
+-rw-r--r--   0 patrick    (502) staff       (20)      179 2023-04-02 08:58:12.000000 pynkdv-0.0.9/pynkdv.egg-info/PKG-INFO
+-rw-r--r--   0 patrick    (502) staff       (20)      193 2023-04-02 08:58:12.000000 pynkdv-0.0.9/pynkdv.egg-info/SOURCES.txt
+-rw-r--r--   0 patrick    (502) staff       (20)        1 2023-04-02 08:58:12.000000 pynkdv-0.0.9/pynkdv.egg-info/dependency_links.txt
+-rw-r--r--   0 patrick    (502) staff       (20)       42 2023-04-02 08:58:12.000000 pynkdv-0.0.9/pynkdv.egg-info/requires.txt
+-rw-r--r--   0 patrick    (502) staff       (20)        7 2023-04-02 08:58:12.000000 pynkdv-0.0.9/pynkdv.egg-info/top_level.txt
+-rw-r--r--   0 patrick    (502) staff       (20)       38 2023-04-02 08:58:12.660322 pynkdv-0.0.9/setup.cfg
+-rw-r--r--   0 patrick    (502) staff       (20)      401 2023-04-02 08:57:54.000000 pynkdv-0.0.9/setup.py
```

### Comparing `pynkdv-0.0.8/pynkdv/PyNKDV.py` & `pynkdv-0.0.9/pynkdv/PyNKDV.py`

 * *Files 4% similar despite different names*

```diff
@@ -222,14 +222,16 @@
     road_data = [geo_path_2, 'test_write_file2']
     return road_data
 
 
 def output(results, output_file_name):
     df4 = gpd.read_file(results[1])
     df5 = pd.read_csv(results[0], sep=',', skiprows=1, names=['a', 'b', 'c', 'd', 'value'])['value']
+    if '.shp' not in output_file_name:
+        output_file_name += '.shp'
     add_kd_value(df4, df5, output_file_name)
     print('aoligei')
 
 
 class PyNKDV:
     def __init__(self, road_data, bandwidth=1000, lixel_size=5, num_threads=8):
         self.graph_path = road_data[0]
```

