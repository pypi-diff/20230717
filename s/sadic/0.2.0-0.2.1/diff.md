# Comparing `tmp/sadic-0.2.0.tar.gz` & `tmp/sadic-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sadic-0.2.0.tar", last modified: Mon Jul 17 15:20:36 2023, max compression
+gzip compressed data, was "sadic-0.2.1.tar", last modified: Mon Jul 17 16:44:15 2023, max compression
```

## Comparing `sadic-0.2.0.tar` & `sadic-0.2.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 giacomo   (1000) giacomo   (1000)        0 2023-07-17 15:20:36.640895 sadic-0.2.0/
--rw-r--r--   0 giacomo   (1000) giacomo   (1000)     1073 2023-05-04 09:36:44.000000 sadic-0.2.0/LICENSE
--rw-r--r--   0 giacomo   (1000) giacomo   (1000)      849 2023-07-17 15:20:36.640895 sadic-0.2.0/PKG-INFO
--rw-r--r--   0 giacomo   (1000) giacomo   (1000)       83 2022-12-22 13:05:48.000000 sadic-0.2.0/README.md
--rw-r--r--   0 giacomo   (1000) giacomo   (1000)       80 2023-05-04 09:24:50.000000 sadic-0.2.0/pyproject.toml
-drwxr-xr-x   0 giacomo   (1000) giacomo   (1000)        0 2023-07-17 15:20:36.590894 sadic-0.2.0/sadic/
--rw-r--r--   0 giacomo   (1000) giacomo   (1000)      235 2023-07-17 15:16:22.000000 sadic-0.2.0/sadic/__init__.py
-drwxr-xr-x   0 giacomo   (1000) giacomo   (1000)        0 2023-07-17 15:20:36.600894 sadic-0.2.0/sadic/algorithm/
--rw-r--r--   0 giacomo   (1000) giacomo   (1000)       40 2023-06-28 16:12:31.000000 sadic-0.2.0/sadic/algorithm/__init__.py
--rw-r--r--   0 giacomo   (1000) giacomo   (1000)    17154 2023-07-04 16:27:17.000000 sadic-0.2.0/sadic/algorithm/depth.py
--rw-r--r--   0 giacomo   (1000) giacomo   (1000)    13902 2023-06-28 15:16:01.000000 sadic-0.2.0/sadic/algorithm/radius.py
--rw-r--r--   0 giacomo   (1000) giacomo   (1000)     6694 2023-07-17 13:58:00.000000 sadic-0.2.0/sadic/api.py
-drwxr-xr-x   0 giacomo   (1000) giacomo   (1000)        0 2023-07-17 15:20:36.610895 sadic-0.2.0/sadic/pdb/
--rw-r--r--   0 giacomo   (1000) giacomo   (1000)      205 2023-07-05 12:45:05.000000 sadic-0.2.0/sadic/pdb/__init__.py
--rw-r--r--   0 giacomo   (1000) giacomo   (1000)    28554 2023-07-13 10:01:30.000000 sadic-0.2.0/sadic/pdb/pdbentity.py
--rw-r--r--   0 giacomo   (1000) giacomo   (1000)    34069 2023-07-17 14:24:23.000000 sadic-0.2.0/sadic/pdb/result.py
-drwxr-xr-x   0 giacomo   (1000) giacomo   (1000)        0 2023-07-17 15:20:36.610895 sadic-0.2.0/sadic/quantizer/
--rw-r--r--   0 giacomo   (1000) giacomo   (1000)      435 2023-06-28 16:12:33.000000 sadic-0.2.0/sadic/quantizer/__init__.py
--rw-r--r--   0 giacomo   (1000) giacomo   (1000)    14689 2023-07-05 10:39:23.000000 sadic-0.2.0/sadic/quantizer/quantizer.py
-drwxr-xr-x   0 giacomo   (1000) giacomo   (1000)        0 2023-07-17 15:20:36.630895 sadic-0.2.0/sadic/solid/
--rw-r--r--   0 giacomo   (1000) giacomo   (1000)      222 2023-06-28 16:13:18.000000 sadic-0.2.0/sadic/solid/__init__.py
--rw-r--r--   0 giacomo   (1000) giacomo   (1000)    14080 2023-07-05 09:01:23.000000 sadic-0.2.0/sadic/solid/multisphere.py
--rw-r--r--   0 giacomo   (1000) giacomo   (1000)     1103 2023-07-05 10:39:58.000000 sadic-0.2.0/sadic/solid/solid.py
--rw-r--r--   0 giacomo   (1000) giacomo   (1000)     2955 2023-07-05 09:00:29.000000 sadic-0.2.0/sadic/solid/sphere.py
--rw-r--r--   0 giacomo   (1000) giacomo   (1000)    23834 2023-07-05 08:59:26.000000 sadic-0.2.0/sadic/solid/voxel_solid.py
-drwxr-xr-x   0 giacomo   (1000) giacomo   (1000)        0 2023-07-17 15:20:36.640895 sadic-0.2.0/sadic/utils/
--rw-r--r--   0 giacomo   (1000) giacomo   (1000)       80 2023-07-05 10:31:34.000000 sadic-0.2.0/sadic/utils/__init__.py
--rw-r--r--   0 giacomo   (1000) giacomo   (1000)       81 2023-06-28 22:41:32.000000 sadic-0.2.0/sadic/utils/config.py
--rw-r--r--   0 giacomo   (1000) giacomo   (1000)      273 2023-07-05 10:38:14.000000 sadic-0.2.0/sadic/utils/repr.py
-drwxr-xr-x   0 giacomo   (1000) giacomo   (1000)        0 2023-07-17 15:20:36.600894 sadic-0.2.0/sadic.egg-info/
--rw-r--r--   0 giacomo   (1000) giacomo   (1000)      849 2023-07-17 15:20:36.000000 sadic-0.2.0/sadic.egg-info/PKG-INFO
--rw-r--r--   0 giacomo   (1000) giacomo   (1000)      604 2023-07-17 15:20:36.000000 sadic-0.2.0/sadic.egg-info/SOURCES.txt
--rw-r--r--   0 giacomo   (1000) giacomo   (1000)        1 2023-07-17 15:20:36.000000 sadic-0.2.0/sadic.egg-info/dependency_links.txt
--rw-r--r--   0 giacomo   (1000) giacomo   (1000)       48 2023-07-17 15:20:36.000000 sadic-0.2.0/sadic.egg-info/requires.txt
--rw-r--r--   0 giacomo   (1000) giacomo   (1000)        6 2023-07-17 15:20:36.000000 sadic-0.2.0/sadic.egg-info/top_level.txt
--rw-r--r--   0 giacomo   (1000) giacomo   (1000)       38 2023-07-17 15:20:36.640895 sadic-0.2.0/setup.cfg
--rw-r--r--   0 giacomo   (1000) giacomo   (1000)     1672 2023-07-05 10:01:38.000000 sadic-0.2.0/setup.py
+drwxr-xr-x   0 giacomo   (1000) giacomo   (1000)        0 2023-07-17 16:44:15.350894 sadic-0.2.1/
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)     1073 2023-05-04 09:36:44.000000 sadic-0.2.1/LICENSE
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)      849 2023-07-17 16:44:15.350894 sadic-0.2.1/PKG-INFO
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)       83 2022-12-22 13:05:48.000000 sadic-0.2.1/README.md
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)       80 2023-05-04 09:24:50.000000 sadic-0.2.1/pyproject.toml
+drwxr-xr-x   0 giacomo   (1000) giacomo   (1000)        0 2023-07-17 16:44:15.330894 sadic-0.2.1/sadic/
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)      235 2023-07-17 16:44:03.000000 sadic-0.2.1/sadic/__init__.py
+drwxr-xr-x   0 giacomo   (1000) giacomo   (1000)        0 2023-07-17 16:44:15.340894 sadic-0.2.1/sadic/algorithm/
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)       40 2023-06-28 16:12:31.000000 sadic-0.2.1/sadic/algorithm/__init__.py
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)    17154 2023-07-04 16:27:17.000000 sadic-0.2.1/sadic/algorithm/depth.py
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)    13902 2023-06-28 15:16:01.000000 sadic-0.2.1/sadic/algorithm/radius.py
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)     6694 2023-07-17 15:41:51.000000 sadic-0.2.1/sadic/api.py
+drwxr-xr-x   0 giacomo   (1000) giacomo   (1000)        0 2023-07-17 16:44:15.340894 sadic-0.2.1/sadic/pdb/
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)      205 2023-07-05 12:45:05.000000 sadic-0.2.1/sadic/pdb/__init__.py
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)    28554 2023-07-13 10:01:30.000000 sadic-0.2.1/sadic/pdb/pdbentity.py
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)    34026 2023-07-17 16:42:18.000000 sadic-0.2.1/sadic/pdb/result.py
+drwxr-xr-x   0 giacomo   (1000) giacomo   (1000)        0 2023-07-17 16:44:15.340894 sadic-0.2.1/sadic/quantizer/
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)      435 2023-06-28 16:12:33.000000 sadic-0.2.1/sadic/quantizer/__init__.py
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)    14689 2023-07-05 10:39:23.000000 sadic-0.2.1/sadic/quantizer/quantizer.py
+drwxr-xr-x   0 giacomo   (1000) giacomo   (1000)        0 2023-07-17 16:44:15.340894 sadic-0.2.1/sadic/solid/
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)      222 2023-06-28 16:13:18.000000 sadic-0.2.1/sadic/solid/__init__.py
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)    14080 2023-07-05 09:01:23.000000 sadic-0.2.1/sadic/solid/multisphere.py
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)     1103 2023-07-05 10:39:58.000000 sadic-0.2.1/sadic/solid/solid.py
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)     2955 2023-07-05 09:00:29.000000 sadic-0.2.1/sadic/solid/sphere.py
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)    23834 2023-07-05 08:59:26.000000 sadic-0.2.1/sadic/solid/voxel_solid.py
+drwxr-xr-x   0 giacomo   (1000) giacomo   (1000)        0 2023-07-17 16:44:15.350894 sadic-0.2.1/sadic/utils/
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)       80 2023-07-05 10:31:34.000000 sadic-0.2.1/sadic/utils/__init__.py
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)       81 2023-06-28 22:41:32.000000 sadic-0.2.1/sadic/utils/config.py
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)      273 2023-07-05 10:38:14.000000 sadic-0.2.1/sadic/utils/repr.py
+drwxr-xr-x   0 giacomo   (1000) giacomo   (1000)        0 2023-07-17 16:44:15.330894 sadic-0.2.1/sadic.egg-info/
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)      849 2023-07-17 16:44:15.000000 sadic-0.2.1/sadic.egg-info/PKG-INFO
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)      604 2023-07-17 16:44:15.000000 sadic-0.2.1/sadic.egg-info/SOURCES.txt
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)        1 2023-07-17 16:44:15.000000 sadic-0.2.1/sadic.egg-info/dependency_links.txt
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)       48 2023-07-17 16:44:15.000000 sadic-0.2.1/sadic.egg-info/requires.txt
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)        6 2023-07-17 16:44:15.000000 sadic-0.2.1/sadic.egg-info/top_level.txt
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)       38 2023-07-17 16:44:15.350894 sadic-0.2.1/setup.cfg
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)     1672 2023-07-05 10:01:38.000000 sadic-0.2.1/setup.py
```

### Comparing `sadic-0.2.0/LICENSE` & `sadic-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sadic-0.2.0/PKG-INFO` & `sadic-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sadic
-Version: 0.2.0
+Version: 0.2.1
 Summary: Reimplementation as a python package of the software for Simple Atom Depth Index Calculator (SADIC)
 Home-page: https://github.com/nunziati/sadic
 Author: Giacomo Nunziati
 Author-email: giacomo.nunziati.0@gmail.com
 License: GNU General Public License v3.0
 Keywords: protein atom depth
 Classifier: Development Status :: 1 - Planning
```

### Comparing `sadic-0.2.0/sadic/algorithm/depth.py` & `sadic-0.2.1/sadic/algorithm/depth.py`

 * *Files identical despite different names*

### Comparing `sadic-0.2.0/sadic/algorithm/radius.py` & `sadic-0.2.1/sadic/algorithm/radius.py`

 * *Files identical despite different names*

### Comparing `sadic-0.2.0/sadic/api.py` & `sadic-0.2.1/sadic/api.py`

 * *Files identical despite different names*

### Comparing `sadic-0.2.0/sadic/pdb/pdbentity.py` & `sadic-0.2.1/sadic/pdb/pdbentity.py`

 * *Files identical despite different names*

### Comparing `sadic-0.2.0/sadic/pdb/result.py` & `sadic-0.2.1/sadic/pdb/result.py`

 * *Files 1% similar despite different names*

```diff
@@ -531,17 +531,17 @@
         if not os.path.exists(os.path.dirname(path)):
             os.makedirs(os.path.dirname(path))
 
         depth_indexes = self.get_depth_index(get_index=True, model_aggregation=model_aggregation)
 
         with open(path, "w", encoding="utf-8") as file:
             if file_format == "sadicv1":
-                file.write(f"di\t{float(self.sadic_args['probe_radius']): .3f}")
+                file.write("di\t####")
                 for atom_index, depth_index in zip(depth_indexes[0], depth_indexes[1]):
-                    file.write(f"\n{atom_index}\t{depth_index: .3f}")
+                    file.write(f"\n{atom_index}\t{depth_index:.3f}")
 
     def summary(self) -> tuple[NDArray[np.int32], NDArray[np.float32], NDArray[np.float32]]:
         r"""Return a summary of the result object.
 
         It includes mean and standard deviation of the depth index of the atoms of the protein,
         among the different models.
         """
```

### Comparing `sadic-0.2.0/sadic/quantizer/quantizer.py` & `sadic-0.2.1/sadic/quantizer/quantizer.py`

 * *Files identical despite different names*

### Comparing `sadic-0.2.0/sadic/solid/multisphere.py` & `sadic-0.2.1/sadic/solid/multisphere.py`

 * *Files identical despite different names*

### Comparing `sadic-0.2.0/sadic/solid/solid.py` & `sadic-0.2.1/sadic/solid/solid.py`

 * *Files identical despite different names*

### Comparing `sadic-0.2.0/sadic/solid/sphere.py` & `sadic-0.2.1/sadic/solid/sphere.py`

 * *Files identical despite different names*

### Comparing `sadic-0.2.0/sadic/solid/voxel_solid.py` & `sadic-0.2.1/sadic/solid/voxel_solid.py`

 * *Files identical despite different names*

### Comparing `sadic-0.2.0/sadic.egg-info/PKG-INFO` & `sadic-0.2.1/sadic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sadic
-Version: 0.2.0
+Version: 0.2.1
 Summary: Reimplementation as a python package of the software for Simple Atom Depth Index Calculator (SADIC)
 Home-page: https://github.com/nunziati/sadic
 Author: Giacomo Nunziati
 Author-email: giacomo.nunziati.0@gmail.com
 License: GNU General Public License v3.0
 Keywords: protein atom depth
 Classifier: Development Status :: 1 - Planning
```

### Comparing `sadic-0.2.0/sadic.egg-info/SOURCES.txt` & `sadic-0.2.1/sadic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sadic-0.2.0/setup.py` & `sadic-0.2.1/setup.py`

 * *Files identical despite different names*

