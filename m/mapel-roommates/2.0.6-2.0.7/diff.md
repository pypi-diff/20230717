# Comparing `tmp/mapel-roommates-2.0.6.tar.gz` & `tmp/mapel-roommates-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapel-roommates-2.0.6.tar", last modified: Fri Jul 14 09:02:48 2023, max compression
+gzip compressed data, was "mapel-roommates-2.0.7.tar", last modified: Mon Jul 17 15:53:35 2023, max compression
```

## Comparing `mapel-roommates-2.0.6.tar` & `mapel-roommates-2.0.7.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:48.313692 mapel-roommates-2.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-14 09:02:16.000000 mapel-roommates-2.0.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-14 09:02:48.313692 mapel-roommates-2.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-14 09:02:16.000000 mapel-roommates-2.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-14 09:02:16.000000 mapel-roommates-2.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 09:02:16.000000 mapel-roommates-2.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 09:02:48.313692 mapel-roommates-2.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:48.309692 mapel-roommates-2.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:48.309692 mapel-roommates-2.0.6/src/mapel/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:48.309692 mapel-roommates-2.0.6/src/mapel/roommates/
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-14 09:02:16.000000 mapel-roommates-2.0.6/src/mapel/roommates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:48.309692 mapel-roommates-2.0.6/src/mapel/roommates/cultures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:16.000000 mapel-roommates-2.0.6/src/mapel/roommates/cultures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-14 09:02:16.000000 mapel-roommates-2.0.6/src/mapel/roommates/cultures/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10974 2023-07-14 09:02:16.000000 mapel-roommates-2.0.6/src/mapel/roommates/cultures/euclidean.py
--rw-r--r--   0 runner    (1001) docker     (123)    18776 2023-07-14 09:02:16.000000 mapel-roommates-2.0.6/src/mapel/roommates/cultures/group_separable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-14 09:02:16.000000 mapel-roommates-2.0.6/src/mapel/roommates/cultures/impartial.py
--rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-07-14 09:02:16.000000 mapel-roommates-2.0.6/src/mapel/roommates/cultures/mallows.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-14 09:02:16.000000 mapel-roommates-2.0.6/src/mapel/roommates/cultures/urn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-14 09:02:16.000000 mapel-roommates-2.0.6/src/mapel/roommates/cultures_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:48.309692 mapel-roommates-2.0.6/src/mapel/roommates/distances/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:16.000000 mapel-roommates-2.0.6/src/mapel/roommates/distances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-07-14 09:02:16.000000 mapel-roommates-2.0.6/src/mapel/roommates/distances/main_distances.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-07-14 09:02:16.000000 mapel-roommates-2.0.6/src/mapel/roommates/distances_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:48.309692 mapel-roommates-2.0.6/src/mapel/roommates/features/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:16.000000 mapel-roommates-2.0.6/src/mapel/roommates/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10122 2023-07-14 09:02:16.000000 mapel-roommates-2.0.6/src/mapel/roommates/features/basic_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-07-14 09:02:16.000000 mapel-roommates-2.0.6/src/mapel/roommates/features/distance_to_stability_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-14 09:02:16.000000 mapel-roommates-2.0.6/src/mapel/roommates/features_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:48.313692 mapel-roommates-2.0.6/src/mapel/roommates/objects/
--rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-07-14 09:02:16.000000 mapel-roommates-2.0.6/src/mapel/roommates/objects/Roommates.py
--rw-r--r--   0 runner    (1001) docker     (123)    18739 2023-07-14 09:02:16.000000 mapel-roommates-2.0.6/src/mapel/roommates/objects/RoommatesExperiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-07-14 09:02:16.000000 mapel-roommates-2.0.6/src/mapel/roommates/objects/RoommatesFamily.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:16.000000 mapel-roommates-2.0.6/src/mapel/roommates/objects/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:48.313692 mapel-roommates-2.0.6/src/mapel/roommates/persistence/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:16.000000 mapel-roommates-2.0.6/src/mapel/roommates/persistence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-07-14 09:02:16.000000 mapel-roommates-2.0.6/src/mapel/roommates/persistence/instance_exports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-14 09:02:16.000000 mapel-roommates-2.0.6/src/mapel/roommates/persistence/instance_imports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:48.313692 mapel-roommates-2.0.6/src/mapel_roommates.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-14 09:02:48.000000 mapel-roommates-2.0.6/src/mapel_roommates.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-14 09:02:48.000000 mapel-roommates-2.0.6/src/mapel_roommates.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 09:02:48.000000 mapel-roommates-2.0.6/src/mapel_roommates.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 09:02:48.000000 mapel-roommates-2.0.6/src/mapel_roommates.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-14 09:02:48.000000 mapel-roommates-2.0.6/src/mapel_roommates.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:35.177779 mapel-roommates-2.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-17 15:53:03.000000 mapel-roommates-2.0.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-17 15:53:35.177779 mapel-roommates-2.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-17 15:53:03.000000 mapel-roommates-2.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-17 15:53:03.000000 mapel-roommates-2.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-17 15:53:03.000000 mapel-roommates-2.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 15:53:35.177779 mapel-roommates-2.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:35.173779 mapel-roommates-2.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:35.173779 mapel-roommates-2.0.7/src/mapel/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:35.173779 mapel-roommates-2.0.7/src/mapel/roommates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-17 15:53:03.000000 mapel-roommates-2.0.7/src/mapel/roommates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:35.173779 mapel-roommates-2.0.7/src/mapel/roommates/cultures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:03.000000 mapel-roommates-2.0.7/src/mapel/roommates/cultures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-17 15:53:03.000000 mapel-roommates-2.0.7/src/mapel/roommates/cultures/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10974 2023-07-17 15:53:03.000000 mapel-roommates-2.0.7/src/mapel/roommates/cultures/euclidean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18776 2023-07-17 15:53:03.000000 mapel-roommates-2.0.7/src/mapel/roommates/cultures/group_separable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-17 15:53:03.000000 mapel-roommates-2.0.7/src/mapel/roommates/cultures/impartial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-07-17 15:53:03.000000 mapel-roommates-2.0.7/src/mapel/roommates/cultures/mallows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-17 15:53:03.000000 mapel-roommates-2.0.7/src/mapel/roommates/cultures/urn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-17 15:53:03.000000 mapel-roommates-2.0.7/src/mapel/roommates/cultures_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:35.173779 mapel-roommates-2.0.7/src/mapel/roommates/distances/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:03.000000 mapel-roommates-2.0.7/src/mapel/roommates/distances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-07-17 15:53:03.000000 mapel-roommates-2.0.7/src/mapel/roommates/distances/main_distances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-07-17 15:53:03.000000 mapel-roommates-2.0.7/src/mapel/roommates/distances_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:35.177779 mapel-roommates-2.0.7/src/mapel/roommates/features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:03.000000 mapel-roommates-2.0.7/src/mapel/roommates/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10122 2023-07-17 15:53:03.000000 mapel-roommates-2.0.7/src/mapel/roommates/features/basic_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-07-17 15:53:03.000000 mapel-roommates-2.0.7/src/mapel/roommates/features/distance_to_stability_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-17 15:53:03.000000 mapel-roommates-2.0.7/src/mapel/roommates/features_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:35.177779 mapel-roommates-2.0.7/src/mapel/roommates/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-07-17 15:53:03.000000 mapel-roommates-2.0.7/src/mapel/roommates/objects/Roommates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18660 2023-07-17 15:53:03.000000 mapel-roommates-2.0.7/src/mapel/roommates/objects/RoommatesExperiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-07-17 15:53:03.000000 mapel-roommates-2.0.7/src/mapel/roommates/objects/RoommatesFamily.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:03.000000 mapel-roommates-2.0.7/src/mapel/roommates/objects/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:35.177779 mapel-roommates-2.0.7/src/mapel/roommates/persistence/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:03.000000 mapel-roommates-2.0.7/src/mapel/roommates/persistence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-07-17 15:53:03.000000 mapel-roommates-2.0.7/src/mapel/roommates/persistence/instance_exports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-17 15:53:03.000000 mapel-roommates-2.0.7/src/mapel/roommates/persistence/instance_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:35.177779 mapel-roommates-2.0.7/src/mapel_roommates.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-17 15:53:35.000000 mapel-roommates-2.0.7/src/mapel_roommates.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-17 15:53:35.000000 mapel-roommates-2.0.7/src/mapel_roommates.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 15:53:35.000000 mapel-roommates-2.0.7/src/mapel_roommates.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-17 15:53:35.000000 mapel-roommates-2.0.7/src/mapel_roommates.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-17 15:53:35.000000 mapel-roommates-2.0.7/src/mapel_roommates.egg-info/top_level.txt
```

### Comparing `mapel-roommates-2.0.6/LICENSE.txt` & `mapel-roommates-2.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.6/PKG-INFO` & `mapel-roommates-2.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapel-roommates
-Version: 2.0.6
+Version: 2.0.7
 Summary: Map of Roommates
 Author-email: Stanislaw Szufa <s.szufa@gmail.com>, Niclas Boehmer <niclas.boehmer@tu-berlin.de>
 License: Copyright (c) 2018-2022 Stanislaw Szufa and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `mapel-roommates-2.0.6/README.md` & `mapel-roommates-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.6/pyproject.toml` & `mapel-roommates-2.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65", "wheel", "pybind11>=2.6.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mapel-roommates"
-version = "2.0.6"
+version = "2.0.7"
 authors = [
  {name = "Stanislaw Szufa", email = "s.szufa@gmail.com"},
  {name = "Niclas Boehmer", email = "niclas.boehmer@tu-berlin.de"},
 ]
 description = "Map of Roommates"
 classifiers=[
     "Programming Language :: Python :: 3",
```

### Comparing `mapel-roommates-2.0.6/src/mapel/roommates/__init__.py` & `mapel-roommates-2.0.7/src/mapel/roommates/__init__.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.6/src/mapel/roommates/cultures/euclidean.py` & `mapel-roommates-2.0.7/src/mapel/roommates/cultures/euclidean.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.6/src/mapel/roommates/cultures/group_separable.py` & `mapel-roommates-2.0.7/src/mapel/roommates/cultures/group_separable.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.6/src/mapel/roommates/cultures/impartial.py` & `mapel-roommates-2.0.7/src/mapel/roommates/cultures/impartial.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.6/src/mapel/roommates/cultures/mallows.py` & `mapel-roommates-2.0.7/src/mapel/roommates/cultures/mallows.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.6/src/mapel/roommates/cultures/urn.py` & `mapel-roommates-2.0.7/src/mapel/roommates/cultures/urn.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.6/src/mapel/roommates/cultures_.py` & `mapel-roommates-2.0.7/src/mapel/roommates/cultures_.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.6/src/mapel/roommates/distances/main_distances.py` & `mapel-roommates-2.0.7/src/mapel/roommates/distances/main_distances.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.6/src/mapel/roommates/distances_.py` & `mapel-roommates-2.0.7/src/mapel/roommates/distances_.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.6/src/mapel/roommates/features/basic_features.py` & `mapel-roommates-2.0.7/src/mapel/roommates/features/basic_features.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.6/src/mapel/roommates/features/distance_to_stability_features.py` & `mapel-roommates-2.0.7/src/mapel/roommates/features/distance_to_stability_features.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.6/src/mapel/roommates/features_.py` & `mapel-roommates-2.0.7/src/mapel/roommates/features_.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.6/src/mapel/roommates/objects/Roommates.py` & `mapel-roommates-2.0.7/src/mapel/roommates/objects/Roommates.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.6/src/mapel/roommates/objects/RoommatesExperiment.py` & `mapel-roommates-2.0.7/src/mapel/roommates/objects/RoommatesExperiment.py`

 * *Files 0% similar despite different names*

```diff
@@ -454,16 +454,15 @@
             # PREPARE MAP.CSV FILE
             path = os.path.join(os.getcwd(), "election", self.experiment_id, "map.csv")
 
             with open(path, 'w') as file_csv:
                 file_csv.write(
                     "size;num_agents;culture_id;params;color;alpha;family_id;label;marker;show\n")
                 file_csv.write("10;20;roommates_ic;{};black;1;IC;IC;o;t\n")
-        except FileExistsError:
-            print("Experiment already exists!")
+
 
 
     def get_election_id_from_model_name(self, culture_id: str) -> str:
         for family_id in self.families:
             if self.families[family_id].culture_id == culture_id:
                 return family_id
```

### Comparing `mapel-roommates-2.0.6/src/mapel/roommates/objects/RoommatesFamily.py` & `mapel-roommates-2.0.7/src/mapel/roommates/objects/RoommatesFamily.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.6/src/mapel/roommates/persistence/instance_exports.py` & `mapel-roommates-2.0.7/src/mapel/roommates/persistence/instance_exports.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.6/src/mapel/roommates/persistence/instance_imports.py` & `mapel-roommates-2.0.7/src/mapel/roommates/persistence/instance_imports.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.6/src/mapel_roommates.egg-info/PKG-INFO` & `mapel-roommates-2.0.7/src/mapel_roommates.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapel-roommates
-Version: 2.0.6
+Version: 2.0.7
 Summary: Map of Roommates
 Author-email: Stanislaw Szufa <s.szufa@gmail.com>, Niclas Boehmer <niclas.boehmer@tu-berlin.de>
 License: Copyright (c) 2018-2022 Stanislaw Szufa and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `mapel-roommates-2.0.6/src/mapel_roommates.egg-info/SOURCES.txt` & `mapel-roommates-2.0.7/src/mapel_roommates.egg-info/SOURCES.txt`

 * *Files identical despite different names*

