# Comparing `tmp/mapel-core-2.0.6.tar.gz` & `tmp/mapel-core-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapel-core-2.0.6.tar", last modified: Fri Jul 14 09:02:34 2023, max compression
+gzip compressed data, was "mapel-core-2.0.7.tar", last modified: Mon Jul 17 15:53:21 2023, max compression
```

## Comparing `mapel-core-2.0.6.tar` & `mapel-core-2.0.7.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:34.121503 mapel-core-2.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-14 09:02:16.000000 mapel-core-2.0.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-14 09:02:34.121503 mapel-core-2.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-14 09:02:16.000000 mapel-core-2.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-14 09:02:16.000000 mapel-core-2.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-14 09:02:16.000000 mapel-core-2.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 09:02:34.121503 mapel-core-2.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:34.117503 mapel-core-2.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:34.117503 mapel-core-2.0.6/src/mapel/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:34.117503 mapel-core-2.0.6/src/mapel/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:34.117503 mapel-core-2.0.6/src/mapel/core/embedding/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/embedding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/embedding/embed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/embedding/initial_positions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:34.117503 mapel-core-2.0.6/src/mapel/core/embedding/kamada_kawai/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/embedding/kamada_kawai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/embedding/kamada_kawai/energy_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/embedding/kamada_kawai/kamada_kawai.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/embedding/kamada_kawai/optimization_algorithms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:34.117503 mapel-core-2.0.6/src/mapel/core/embedding/simulated_annealing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/embedding/simulated_annealing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/embedding/simulated_annealing/simulated_annealing.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/embedding/simulated_annealing/simulated_annealing_energy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:34.121503 mapel-core-2.0.6/src/mapel/core/features/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/features/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/features/distortion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/features/mallows.py
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/features/monotonicity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/features/stability.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/features_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/glossary.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/inner_distances.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/matchings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:34.121503 mapel-core-2.0.6/src/mapel/core/objects/
--rw-r--r--   0 runner    (1001) docker     (123)    16676 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/objects/Experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/objects/Family.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/objects/Instance.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/objects/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:34.121503 mapel-core-2.0.6/src/mapel/core/persistence/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/persistence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/persistence/experiment_exports.py
--rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/persistence/experiment_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)    62429 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/printing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:34.121503 mapel-core-2.0.6/src/mapel_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-14 09:02:34.000000 mapel-core-2.0.6/src/mapel_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-14 09:02:34.000000 mapel-core-2.0.6/src/mapel_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 09:02:34.000000 mapel-core-2.0.6/src/mapel_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-14 09:02:34.000000 mapel-core-2.0.6/src/mapel_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-14 09:02:34.000000 mapel-core-2.0.6/src/mapel_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:21.521845 mapel-core-2.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-17 15:53:03.000000 mapel-core-2.0.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-17 15:53:21.521845 mapel-core-2.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-17 15:53:03.000000 mapel-core-2.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-17 15:53:03.000000 mapel-core-2.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-17 15:53:03.000000 mapel-core-2.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 15:53:21.521845 mapel-core-2.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:21.517845 mapel-core-2.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:21.513845 mapel-core-2.0.7/src/mapel/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:21.517845 mapel-core-2.0.7/src/mapel/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:03.000000 mapel-core-2.0.7/src/mapel/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:21.517845 mapel-core-2.0.7/src/mapel/core/embedding/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:03.000000 mapel-core-2.0.7/src/mapel/core/embedding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-07-17 15:53:03.000000 mapel-core-2.0.7/src/mapel/core/embedding/embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-07-17 15:53:03.000000 mapel-core-2.0.7/src/mapel/core/embedding/initial_positions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:21.517845 mapel-core-2.0.7/src/mapel/core/embedding/kamada_kawai/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:03.000000 mapel-core-2.0.7/src/mapel/core/embedding/kamada_kawai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-07-17 15:53:03.000000 mapel-core-2.0.7/src/mapel/core/embedding/kamada_kawai/energy_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-07-17 15:53:03.000000 mapel-core-2.0.7/src/mapel/core/embedding/kamada_kawai/kamada_kawai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-07-17 15:53:03.000000 mapel-core-2.0.7/src/mapel/core/embedding/kamada_kawai/optimization_algorithms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:21.517845 mapel-core-2.0.7/src/mapel/core/embedding/simulated_annealing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:03.000000 mapel-core-2.0.7/src/mapel/core/embedding/simulated_annealing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-07-17 15:53:03.000000 mapel-core-2.0.7/src/mapel/core/embedding/simulated_annealing/simulated_annealing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-17 15:53:03.000000 mapel-core-2.0.7/src/mapel/core/embedding/simulated_annealing/simulated_annealing_energy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:21.517845 mapel-core-2.0.7/src/mapel/core/features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:03.000000 mapel-core-2.0.7/src/mapel/core/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-17 15:53:03.000000 mapel-core-2.0.7/src/mapel/core/features/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-07-17 15:53:03.000000 mapel-core-2.0.7/src/mapel/core/features/distortion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-07-17 15:53:03.000000 mapel-core-2.0.7/src/mapel/core/features/mallows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-07-17 15:53:03.000000 mapel-core-2.0.7/src/mapel/core/features/monotonicity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-07-17 15:53:03.000000 mapel-core-2.0.7/src/mapel/core/features/stability.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-17 15:53:03.000000 mapel-core-2.0.7/src/mapel/core/features_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-07-17 15:53:03.000000 mapel-core-2.0.7/src/mapel/core/glossary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-07-17 15:53:03.000000 mapel-core-2.0.7/src/mapel/core/inner_distances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-07-17 15:53:03.000000 mapel-core-2.0.7/src/mapel/core/matchings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:21.517845 mapel-core-2.0.7/src/mapel/core/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)    16789 2023-07-17 15:53:03.000000 mapel-core-2.0.7/src/mapel/core/objects/Experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-17 15:53:03.000000 mapel-core-2.0.7/src/mapel/core/objects/Family.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-17 15:53:03.000000 mapel-core-2.0.7/src/mapel/core/objects/Instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:03.000000 mapel-core-2.0.7/src/mapel/core/objects/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:21.517845 mapel-core-2.0.7/src/mapel/core/persistence/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:03.000000 mapel-core-2.0.7/src/mapel/core/persistence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-07-17 15:53:03.000000 mapel-core-2.0.7/src/mapel/core/persistence/experiment_exports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-07-17 15:53:03.000000 mapel-core-2.0.7/src/mapel/core/persistence/experiment_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62429 2023-07-17 15:53:03.000000 mapel-core-2.0.7/src/mapel/core/printing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-17 15:53:03.000000 mapel-core-2.0.7/src/mapel/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:21.521845 mapel-core-2.0.7/src/mapel_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-17 15:53:21.000000 mapel-core-2.0.7/src/mapel_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-17 15:53:21.000000 mapel-core-2.0.7/src/mapel_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 15:53:21.000000 mapel-core-2.0.7/src/mapel_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-17 15:53:21.000000 mapel-core-2.0.7/src/mapel_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-17 15:53:21.000000 mapel-core-2.0.7/src/mapel_core.egg-info/top_level.txt
```

### Comparing `mapel-core-2.0.6/LICENSE.txt` & `mapel-core-2.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.6/PKG-INFO` & `mapel-core-2.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapel-core
-Version: 2.0.6
+Version: 2.0.7
 Summary: Map of Elections---essential parts
 Author-email: Stanislaw Szufa <s.szufa@gmail.com>, Niclas Boehmer <niclas.boehmer@tu-berlin.de>, Andrzej Kaczmarczyk <andrzej.kaczmarczyk@agh.edu.pl>, Kasper Sapala <kasper.sapala@gmail.com>, Tomasz Was <tomasz.t.was@gmail.com>
 License: Copyright (c) 2018-2022 Stanisław Szufa and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `mapel-core-2.0.6/README.md` & `mapel-core-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.6/pyproject.toml` & `mapel-core-2.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65", "wheel", "pybind11>=2.6.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mapel-core"
-version = "2.0.6"
+version = "2.0.7"
 authors = [
  {name = "Stanislaw Szufa", email = "s.szufa@gmail.com"},
  {name = "Niclas Boehmer", email = "niclas.boehmer@tu-berlin.de"},
  {name = "Andrzej Kaczmarczyk", email = "andrzej.kaczmarczyk@agh.edu.pl"},
  {name = "Kasper Sapala", email = "kasper.sapala@gmail.com"},
  {name = "Tomasz Was", email = "tomasz.t.was@gmail.com"},
 ]
```

### Comparing `mapel-core-2.0.6/src/mapel/core/embedding/embed.py` & `mapel-core-2.0.7/src/mapel/core/embedding/embed.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.6/src/mapel/core/embedding/initial_positions.py` & `mapel-core-2.0.7/src/mapel/core/embedding/initial_positions.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.6/src/mapel/core/embedding/kamada_kawai/energy_functions.py` & `mapel-core-2.0.7/src/mapel/core/embedding/kamada_kawai/energy_functions.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.6/src/mapel/core/embedding/kamada_kawai/kamada_kawai.py` & `mapel-core-2.0.7/src/mapel/core/embedding/kamada_kawai/kamada_kawai.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.6/src/mapel/core/embedding/kamada_kawai/optimization_algorithms.py` & `mapel-core-2.0.7/src/mapel/core/embedding/kamada_kawai/optimization_algorithms.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.6/src/mapel/core/embedding/simulated_annealing/simulated_annealing.py` & `mapel-core-2.0.7/src/mapel/core/embedding/simulated_annealing/simulated_annealing.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.6/src/mapel/core/embedding/simulated_annealing/simulated_annealing_energy.py` & `mapel-core-2.0.7/src/mapel/core/embedding/simulated_annealing/simulated_annealing_energy.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.6/src/mapel/core/features/common.py` & `mapel-core-2.0.7/src/mapel/core/features/common.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.6/src/mapel/core/features/distortion.py` & `mapel-core-2.0.7/src/mapel/core/features/distortion.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.6/src/mapel/core/features/mallows.py` & `mapel-core-2.0.7/src/mapel/core/features/mallows.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.6/src/mapel/core/features/monotonicity.py` & `mapel-core-2.0.7/src/mapel/core/features/monotonicity.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.6/src/mapel/core/features/stability.py` & `mapel-core-2.0.7/src/mapel/core/features/stability.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.6/src/mapel/core/features_main.py` & `mapel-core-2.0.7/src/mapel/core/features_main.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.6/src/mapel/core/glossary.py` & `mapel-core-2.0.7/src/mapel/core/glossary.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.6/src/mapel/core/inner_distances.py` & `mapel-core-2.0.7/src/mapel/core/inner_distances.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import copy
+from copy import deepcopy
 import math
 import numpy as np
 import itertools
 
 
 def map_str_to_func(name):
     return {'l1': l1,
@@ -56,15 +56,15 @@
                    for i in range(len(vector_1))])
     return math.sqrt(1 - (1 / math.sqrt(h1 * h2 * len(vector_1) * len(vector_1)))
                      * product)
 
 
 def emd(vector_1, vector_2):
     """ compute EMD metric """
-    vector_1 = copy.deepcopy(vector_1)
+    vector_1 = deepcopy(vector_1)
     dirt = 0.
     for i in range(len(vector_1) - 1):
         surplus = vector_1[i] - vector_2[i]
         dirt += abs(surplus)
         vector_1[i + 1] += surplus
     return dirt
 
@@ -79,15 +79,15 @@
     """ Return: Positional vote """
     return [vote.index(i) for i in range(len(vote)+1) if i in vote]
 
 
 def swap_distance(vote_1: list, vote_2: list, matching=None) -> int:
     """ Return: Swap distance between two votes """
 
-    new_vote_2 = copy.deepcopy(vote_2)
+    new_vote_2 = deepcopy(vote_2)
     if matching is not None:
         for i in range(len(vote_2)):
             new_vote_2[i] = matching[vote_2[i]]
 
     pote_1 = vote_to_pote(vote_1)
     pote_2 = vote_to_pote(new_vote_2)
```

### Comparing `mapel-core-2.0.6/src/mapel/core/matchings.py` & `mapel-core-2.0.7/src/mapel/core/matchings.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.6/src/mapel/core/objects/Experiment.py` & `mapel-core-2.0.7/src/mapel/core/objects/Experiment.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,19 @@
             self.experiment_id = experiment_id
             self.add_folders_to_experiment()
             self.families = self.import_controllers()
 
             self.import_instances(instances)
             self.import_distances(distances)
             self.import_coordinates(coordinates, coordinates_names)
+        else:
+            self.instances = {}
+            self.distances = {}
+            self.coordinates = {}
+
 
     def import_instances(self, instances):
         if isinstance(instances, dict):
             self.instances = instances
         elif self.is_imported and self.experiment_id is not None:
 
             try:
```

### Comparing `mapel-core-2.0.6/src/mapel/core/objects/Family.py` & `mapel-core-2.0.7/src/mapel/core/objects/Family.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.6/src/mapel/core/persistence/experiment_exports.py` & `mapel-core-2.0.7/src/mapel/core/persistence/experiment_exports.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,16 @@
         path = os.path.join(os.getcwd(), "experiments", experiment.experiment_id,
                             "features", f'{saveas}.csv')
 
     with open(path, 'w', newline='') as csv_file:
         writer = csv.writer(csv_file, delimiter=';')
         header = ['instance_id'] + list(feature_dict.keys())
         writer.writerow(header)
-        for instance_id in feature_dict['instance_id']:
+        any_key = [key for key in feature_dict.keys()][0]
+        for instance_id in feature_dict[any_key]:
             row = [instance_id] + [feature_dict[key][instance_id] for key in feature_dict.keys()]
             writer.writerow(row)
 
 
 def export_feature_from_function_to_file(experiment, feature_id, feature_dict):
     path_to_file = os.path.join(os.getcwd(), "experiments", experiment.experiment_id, "features",
                                 f'{feature_id}_{experiment.embedding_id}.csv')
```

### Comparing `mapel-core-2.0.6/src/mapel/core/persistence/experiment_imports.py` & `mapel-core-2.0.7/src/mapel/core/persistence/experiment_imports.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.6/src/mapel/core/printing.py` & `mapel-core-2.0.7/src/mapel/core/printing.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.6/src/mapel/core/utils.py` & `mapel-core-2.0.7/src/mapel/core/utils.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.6/src/mapel_core.egg-info/PKG-INFO` & `mapel-core-2.0.7/src/mapel_core.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapel-core
-Version: 2.0.6
+Version: 2.0.7
 Summary: Map of Elections---essential parts
 Author-email: Stanislaw Szufa <s.szufa@gmail.com>, Niclas Boehmer <niclas.boehmer@tu-berlin.de>, Andrzej Kaczmarczyk <andrzej.kaczmarczyk@agh.edu.pl>, Kasper Sapala <kasper.sapala@gmail.com>, Tomasz Was <tomasz.t.was@gmail.com>
 License: Copyright (c) 2018-2022 Stanisław Szufa and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `mapel-core-2.0.6/src/mapel_core.egg-info/SOURCES.txt` & `mapel-core-2.0.7/src/mapel_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

