# Comparing `tmp/genomap-1.1.1.tar.gz` & `tmp/genomap-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genomap-1.1.1.tar", last modified: Sat Jul 15 00:41:23 2023, max compression
+gzip compressed data, was "genomap-1.2.1.tar", last modified: Mon Jul 17 19:40:42 2023, max compression
```

## Comparing `genomap-1.1.1.tar` & `genomap-1.2.1.tar`

### file list

```diff
@@ -1,45 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:41:23.029401 genomap-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-07-15 00:38:59.000000 genomap-1.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-15 00:38:59.000000 genomap-1.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-07-15 00:41:23.029401 genomap-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-07-15 00:39:00.000000 genomap-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:41:23.025400 genomap-1.1.1/data/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-15 00:39:00.000000 genomap-1.1.1/data/TM_data.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:41:23.025400 genomap-1.1.1/genomap/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-15 00:39:00.000000 genomap-1.1.1/genomap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:41:23.025400 genomap-1.1.1/genomap/bregman_genomap/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-15 00:39:00.000000 genomap-1.1.1/genomap/bregman_genomap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   125058 2023-07-15 00:39:00.000000 genomap-1.1.1/genomap/bregman_genomap/bregman_genomap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:41:23.025400 genomap-1.1.1/genomap/genoMOI/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-15 00:39:00.000000 genomap-1.1.1/genomap/genoMOI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-15 00:39:00.000000 genomap-1.1.1/genomap/genoMOI/genoMOI.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:41:23.025400 genomap-1.1.1/genomap/genoTraj/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-15 00:39:00.000000 genomap-1.1.1/genomap/genoTraj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-07-15 00:39:00.000000 genomap-1.1.1/genomap/genoTraj/genoTraj.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:41:23.025400 genomap-1.1.1/genomap/genoVis/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-15 00:39:00.000000 genomap-1.1.1/genomap/genoVis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-07-15 00:39:00.000000 genomap-1.1.1/genomap/genoVis/genoVis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-07-15 00:39:00.000000 genomap-1.1.1/genomap/genomap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:41:23.025400 genomap-1.1.1/genomap/genomapOPT/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-15 00:39:00.000000 genomap-1.1.1/genomap/genomapOPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-07-15 00:39:00.000000 genomap-1.1.1/genomap/genomapOPT/genomapOPT.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:41:23.029401 genomap-1.1.1/genomap/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-07-15 00:39:00.000000 genomap-1.1.1/genomap/utils/ConvDEC.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-15 00:39:00.000000 genomap-1.1.1/genomap/utils/ConvIDEC.py
--rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-07-15 00:39:00.000000 genomap-1.1.1/genomap/utils/FcDEC.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-15 00:39:00.000000 genomap-1.1.1/genomap/utils/FcIDEC.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-15 00:39:00.000000 genomap-1.1.1/genomap/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-15 00:39:00.000000 genomap-1.1.1/genomap/utils/class_discriminative_opt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-07-15 00:39:00.000000 genomap-1.1.1/genomap/utils/gTraj_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-15 00:39:00.000000 genomap-1.1.1/genomap/utils/group_centroid_opt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-15 00:39:00.000000 genomap-1.1.1/genomap/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-15 00:39:00.000000 genomap-1.1.1/genomap/utils/utils_MOI.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:41:23.025400 genomap-1.1.1/genomap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-07-15 00:41:22.000000 genomap-1.1.1/genomap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-15 00:41:22.000000 genomap-1.1.1/genomap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 00:41:22.000000 genomap-1.1.1/genomap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-15 00:41:22.000000 genomap-1.1.1/genomap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-15 00:41:22.000000 genomap-1.1.1/genomap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-15 00:39:00.000000 genomap-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 00:41:23.029401 genomap-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-15 00:39:00.000000 genomap-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:40:42.473471 genomap-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-07-17 19:35:42.000000 genomap-1.2.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-17 19:35:42.000000 genomap-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10426 2023-07-17 19:40:42.473471 genomap-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9992 2023-07-17 19:35:43.000000 genomap-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:40:42.445471 genomap-1.2.1/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-17 19:35:43.000000 genomap-1.2.1/data/TM_data.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:40:42.449471 genomap-1.2.1/genomap/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:40:42.449471 genomap-1.2.1/genomap/bregman_genomap/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/bregman_genomap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   125058 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/bregman_genomap/bregman_genomap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:40:42.453471 genomap-1.2.1/genomap/genoClassification/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/genoClassification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/genoClassification/genoClassification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:40:42.457471 genomap-1.2.1/genomap/genoDR/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/genoDR/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/genoDR/genoDimReduction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:40:42.457471 genomap-1.2.1/genomap/genoMOI/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/genoMOI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/genoMOI/genoMOI.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:40:42.457471 genomap-1.2.1/genomap/genoNetRegression/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/genoNetRegression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/genoNetRegression/genoNet_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:40:42.461471 genomap-1.2.1/genomap/genoRegression/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/genoRegression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/genoRegression/genoRegression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:40:42.461471 genomap-1.2.1/genomap/genoSig/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/genoSig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/genoSig/genoSig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:40:42.461471 genomap-1.2.1/genomap/genoTraj/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/genoTraj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/genoTraj/genoTraj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:40:42.465471 genomap-1.2.1/genomap/genoVis/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/genoVis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/genoVis/genoVis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/genomap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:40:42.465471 genomap-1.2.1/genomap/genomapOPT/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/genomapOPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/genomapOPT/genomapOPT.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:40:42.465471 genomap-1.2.1/genomap/genomapT/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/genomapT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/genomapT/genomapT.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:40:42.473471 genomap-1.2.1/genomap/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/utils/ConvDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/utils/ConvIDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/utils/FcDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/utils/FcIDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/utils/class_discriminative_opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/utils/gTraj_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/utils/group_centroid_opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/utils/util_Sig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/utils/utils_MOI.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:40:42.449471 genomap-1.2.1/genomap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10426 2023-07-17 19:40:42.000000 genomap-1.2.1/genomap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-17 19:40:42.000000 genomap-1.2.1/genomap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 19:40:42.000000 genomap-1.2.1/genomap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-17 19:40:42.000000 genomap-1.2.1/genomap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 19:40:42.000000 genomap-1.2.1/genomap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-17 19:35:43.000000 genomap-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 19:40:42.473471 genomap-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-17 19:35:43.000000 genomap-1.2.1/setup.py
```

### Comparing `genomap-1.1.1/LICENSE.txt` & `genomap-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `genomap-1.1.1/genomap/bregman_genomap/bregman_genomap.py` & `genomap-1.2.1/genomap/bregman_genomap/bregman_genomap.py`

 * *Files identical despite different names*

### Comparing `genomap-1.1.1/genomap/genoMOI/genoMOI.py` & `genomap-1.2.1/genomap/genoMOI/genoMOI.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 """
 Created on Wed Jul 12 16:11:15 2023
 
 @author: Md Tauhidul Islam, Ph.D., Dept. of Radiation Oncology, Stanford University
 """
 
 from tensorflow.keras.optimizers import Adam
-from genomap.utils import ConvIDEC
+from genomap.utils.ConvIDEC import ConvIDEC
 from sklearn.feature_selection import VarianceThreshold
 from genomap.genomap import construct_genomap
 import umap
 from genomap.utils.gTraj_utils import nearest_divisible_by_four
-from genomap.utils.utils_MOI import *
+from genomap.utils.utils_MOI import * 
+from genomap.utils.util_Sig import select_n_features
 
-def compute_genoMOI(*arrays,n_clusters=None, colNum, rowNum):  
+def genoMOI(*arrays,n_clusters=None, colNum, rowNum):  
 
 # arrays: number of arrays such as array1,array2
 # n_clusters: number of data classes
 # colNum and rowNum: column are rwo number of genomaps
 #
 # Pre-align data with bbknn
     batch_corrected_data=apply_bbknn_and_return_batch_corrected(*arrays)
@@ -46,20 +47,15 @@
 # pretrain_epochs: number of epoch for pre-training the CNN
 # maxiter: number of epoch of fine-tuning training
 # Construction of genomap    
     colNum=nearest_divisible_by_four(colNum)
     rowNum=nearest_divisible_by_four(rowNum)
     nump=rowNum*colNum 
     if nump<data.shape[1]:
-    # create an instance of the VarianceThreshold class
-        selector = VarianceThreshold( )
-    # fit the selector to the data and get the indices of the top n most variable features
-        var_threshold = selector.fit(data)
-        top_n_indices = var_threshold.get_support(indices=True)
-        data=data[:,top_n_indices[0:nump]]  
+        data,index=select_n_features(data,nump) 
     genoMaps=construct_genomap(data,rowNum,colNum,epsilon=0.0,num_iter=200)
 
 # Deep learning-based dimensionality reduction and clustering
     optimizer = Adam()    
     model = ConvIDEC(input_shape=genoMaps.shape[1:], filters=[32, 64, 128, 32], n_clusters=n_clusters)
     model.compile(optimizer=optimizer, loss=['kld', 'mse'], loss_weights=[0.1, 1.0])
     pretrain_optimizer ='adam'
```

### Comparing `genomap-1.1.1/genomap/genoTraj/genoTraj.py` & `genomap-1.2.1/genomap/genoTraj/genoTraj.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Wed Jul 12 15:14:53 2023
 
-@author: Windows
+"""
+Created on Sun Jul 16 21:27:17 2023
+@author: Md Tauhidul Islam, Research Scientist, Dept. of radiation Oncology, Stanford University
 """
 
-from genomap.utils.class_discriminative_opt import ClassDiscriminative_OPT
-from genomap.genomap import construct_genomap
-from genomap.utils.gTraj_utils import compute_cluster_distances, nearest_divisible_by_four
-from genomap.utils import ConvIDEC
-import numpy as np
 import phate
+import numpy as np
+from genomap.utils.class_discriminative_opt import ClassDiscriminative_OPT
 import scipy
-from sklearn.feature_selection import VarianceThreshold
+from genomap.utils.gTraj_utils import compute_cluster_distances, nearest_divisible_by_four
 from tensorflow.keras.optimizers import Adam
-
-# from gTraj_utils import nearest_divisible_by_four
+from genomap.utils.ConvIDEC import ConvIDEC
+from sklearn.feature_selection import VarianceThreshold
+from genomap.genomap import construct_genomap
+from genomap.utils.util_Sig import select_n_features
 
 def apply_genoTraj(data, y_pred):
 # data: input data
 # y_pred: predicted pseudo labels
     Kdis=compute_cluster_distances(data,y_pred);
 
 # Kdis = normalize(Kdis, axis=1, norm='l1')
@@ -31,33 +29,28 @@
     clf.fit(Kdis, y_pred)
     ccifOut = clf.transform(Kdis)
     ccifOutzc = scipy.stats.zscore(ccifOut, axis=0, ddof=1) # Z-score of the CCIF
     phate_op = phate.PHATE()
     data_phate = phate_op.fit_transform(ccifOutzc)
     return data_phate
 
-def compute_genoTraj(data,n_clusters = 33, colNum=32,rowNum=32,batch_size=64,verbose=1,
+def genoTraj(data,n_clusters = 33, colNum=32,rowNum=32,batch_size=64,verbose=1,
                     pretrain_epochs=100,maxiter=300):
 # rowNum and colNum are the row and column numbers of constructed genomaps
 # n_clusters: number of  pseudo-classes in the data, should be set as 17, 33 or 65
 # batch_size: number of samples in each mini batch while training the deep neural network
 # verbose: whether training progress will be shown or not
 # pretrain_epochs: number of epoch for pre-training the CNN
 # maxiter: number of epoch of fine-tuning training                    
 # Construction of genomap    
     colNum=nearest_divisible_by_four(colNum)
     rowNum=nearest_divisible_by_four(rowNum)
     nump=rowNum*colNum 
     if nump<data.shape[1]:
-    # create an instance of the VarianceThreshold class
-        selector = VarianceThreshold( )
-    # fit the selector to the data and get the indices of the top n most variable features
-        var_threshold = selector.fit(data)
-        top_n_indices = var_threshold.get_support(indices=True)
-        data=data[:,top_n_indices[0:nump]]  
+        data,index=select_n_features(data,nump)
     genoMaps=construct_genomap(data,rowNum,colNum,epsilon=0.0,num_iter=200)
 
 # Deep learning-based trajectory mapping
     optimizer = Adam()    
     model = ConvIDEC(input_shape=genoMaps.shape[1:], filters=[32, 64, 128, 32], n_clusters=n_clusters)
     model.compile(optimizer=optimizer, loss=['kld', 'mse'], loss_weights=[0.1, 1.0])
     pretrain_optimizer ='adam'
```

### Comparing `genomap-1.1.1/genomap/genoVis/genoVis.py` & `genomap-1.2.1/genomap/genoVis/genoVis.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,42 +2,38 @@
 """
 Created on Wed Jul 12 16:11:15 2023
 
 @author: Md Tauhidul Islam, Ph.D., Dept. of Radiation Oncology, Stanford University
 """
 
 from tensorflow.keras.optimizers import Adam
-from genomap.utils import ConvIDEC
+from genomap.utils.ConvIDEC import ConvIDEC
 from sklearn.feature_selection import VarianceThreshold
 from genomap.genomap import construct_genomap
 import umap
 from genomap.utils.gTraj_utils import nearest_divisible_by_four
 import scanpy as sc
 import numpy as np
 import pandas as pd
+from genomap.utils.util_Sig import select_n_features
 
-def compute_genoVis(data,n_clusters=None, colNum=32,rowNum=32,batch_size=64,verbose=1,
+def genoVis(data,n_clusters=None, colNum=32,rowNum=32,batch_size=64,verbose=1,
                     pretrain_epochs=100,maxiter=300):
 # rowNum and colNum are the row and column numbers of constructed genomaps
 # n_clusters: number of data classes in the data
 # batch_size: number of samples in each mini batch while training the deep neural network
 # verbose: whether training progress will be shown or not
 # pretrain_epochs: number of epoch for pre-training the CNN
 # maxiter: number of epoch of fine-tuning training
 # Construction of genomap    
     colNum=nearest_divisible_by_four(colNum)
     rowNum=nearest_divisible_by_four(rowNum)
     nump=rowNum*colNum 
     if nump<data.shape[1]:
-    # create an instance of the VarianceThreshold class
-        selector = VarianceThreshold( )
-    # fit the selector to the data and get the indices of the top n most variable features
-        var_threshold = selector.fit(data)
-        top_n_indices = var_threshold.get_support(indices=True)
-        data=data[:,top_n_indices[0:nump]]  
+        data,index=select_n_features(data,nump)
     genoMaps=construct_genomap(data,rowNum,colNum,epsilon=0.0,num_iter=200)
     
     if n_clusters==None:
         
         adata = convertToAnnData(data)
         # Perform Louvain clustering
         sc.pp.neighbors(adata)
```

### Comparing `genomap-1.1.1/genomap/genomap.py` & `genomap-1.2.1/genomap/genomapT/genomapT.py`

 * *Files 23% similar despite different names*

```diff
@@ -145,8 +145,71 @@
         ex = np.reshape(fullVec, (rowNum, colNum), order='F').copy()
         genomaps[i, :, :, 0] = ex
         
         
     return genomaps
 
 
+def construct_genomap_returnT(data,rowNum,colNum,epsilon=0,num_iter=1000):
+    """
+    Returns the constructed genomaps
+
+
+    Parameters
+    ----------
+    data : ndarray, shape (cellNum, geneNum)
+         gene expression data in cell X gene format. Each row corresponds
+         to one cell, whereas each column represents one gene
+    rowNum : int, 
+         number of rows in a genomap
+    colNum : int,
+         number of columns in a genomap
+
+    Returns
+    -------
+    genomaps : ndarray, shape (rowNum, colNum, zAxisDimension, cell number)
+           genomaps are formed for each cell. zAxisDimension is more than
+           1 when 3D genomaps are created. 
+    """
+
+    sizeData=data.shape
+    numCell=sizeData[0]
+    numGene=sizeData[1]
+    # distance matrix of 2D genomap grid
+    distMat = createMeshDistance(rowNum,colNum)
+    # gene-gene interaction matrix 
+    interactMat = createInteractionMatrix(data, metric='correlation')
+
+    totalGridPoint=rowNum*colNum
+    
+    if (numGene<totalGridPoint):
+        totalGridPointEff=numGene
+    else:
+        totalGridPointEff=totalGridPoint
+    
+    M = np.zeros((totalGridPointEff, totalGridPointEff))
+    p, q = create_space_distributions(totalGridPointEff, totalGridPointEff)
+
+   # Coupling matrix 
+    T = gromov_wasserstein_adjusted_norm(
+    M, interactMat, distMat[:totalGridPointEff,:totalGridPointEff], p, q, loss_fun='kl_loss', epsilon=epsilon,max_iter=num_iter)
+ 
+    projMat = T*totalGridPoint
+    # Data projected onto the couping matrix
+    projM = np.matmul(data, projMat)
+
+    genomaps = np.zeros((numCell,rowNum, colNum, 1))
+
+    px = np.asmatrix(projM)
+
+    # Formation of genomaps from the projected data
+    for i in range(0, numCell-1):
+        dx = px[i, :]
+        fullVec = np.zeros((1,rowNum*colNum))
+        fullVec[:dx.shape[0],:dx.shape[1]] = dx
+        ex = np.reshape(fullVec, (rowNum, colNum), order='F').copy()
+        genomaps[i, :, :, 0] = ex
+        
+        
+    return genomaps,T
+
```

### Comparing `genomap-1.1.1/genomap/genomapOPT/genomapOPT.py` & `genomap-1.2.1/genomap/genomapOPT/genomapOPT.py`

 * *Files identical despite different names*

### Comparing `genomap-1.1.1/genomap/utils/ConvDEC.py` & `genomap-1.2.1/genomap/utils/ConvDEC.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,7 +51,8 @@
         self.datagenx = ImageDataGenerator()
         self.autoencoder, self.encoder = CAE(input_shape, filters)
 
         # Define ConvIDEC model
         clustering_layer = ClusteringLayer(self.n_clusters, name='clustering')(self.encoder.output)
         self.model = Model(inputs=self.autoencoder.input,
                            outputs=clustering_layer)
+
```

### Comparing `genomap-1.1.1/genomap/utils/ConvIDEC.py` & `genomap-1.2.1/genomap/utils/ConvIDEC.py`

 * *Files identical despite different names*

### Comparing `genomap-1.1.1/genomap/utils/FcDEC.py` & `genomap-1.2.1/genomap/utils/FcDEC.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 from tensorflow.keras.models import Model
 from tensorflow.keras import callbacks
 from tensorflow.keras.initializers import VarianceScaling
 from tensorflow.keras.preprocessing.image import ImageDataGenerator
 from sklearn.cluster import KMeans
 from .metrics import *
 
-
 def autoencoder(dims, act='relu'):
     """
     Fully connected auto-encoder model, symmetric.
     Arguments:
         dims: list of number of units in each layer of encoder. dims[0] is input dim, dims[-1] is units in hidden layer.
             The decoder is symmetric with encoder. So number of layers of the auto-encoder is 2*len(dims)-1
         act: activation, not applied to Input, Hidden and Output layers
@@ -310,7 +309,8 @@
         logfile.close()
         print('saving model to:', save_dir + '/model_final.h5')
         self.model.save_weights(save_dir + '/model_final.h5')
         print('Clustering time: %ds' % (time() - t1))
         print('End clustering:', '-' * 60)
 
         return y_pred
+
```

### Comparing `genomap-1.1.1/genomap/utils/FcIDEC.py` & `genomap-1.2.1/genomap/utils/FcIDEC.py`

 * *Files identical despite different names*

### Comparing `genomap-1.1.1/genomap/utils/class_discriminative_opt.py` & `genomap-1.2.1/genomap/utils/class_discriminative_opt.py`

 * *Files identical despite different names*

### Comparing `genomap-1.1.1/genomap/utils/group_centroid_opt.py` & `genomap-1.2.1/genomap/utils/group_centroid_opt.py`

 * *Files identical despite different names*

### Comparing `genomap-1.1.1/genomap/utils/metrics.py` & `genomap-1.2.1/genomap/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `genomap-1.1.1/genomap/utils/utils_MOI.py` & `genomap-1.2.1/genomap/utils/utils_MOI.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 Created on Thu Jul 13 12:26:22 2023
 
 @author: Windows
 """
 import scanpy as sc
 import numpy as np
 import scipy.io
-import anndata
 import pandas as pd
 import anndata as ad
 
 
 def select_highly_variable_genes_top_genes(adata,n_top_genes=2500):
     # Select_highly_variable_genes of the data
     sc.pp.highly_variable_genes(adata, n_top_genes=n_top_genes, flavor='seurat_v3')
```

### Comparing `genomap-1.1.1/genomap.egg-info/SOURCES.txt` & `genomap-1.2.1/genomap.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -9,25 +9,38 @@
 genomap.egg-info/PKG-INFO
 genomap.egg-info/SOURCES.txt
 genomap.egg-info/dependency_links.txt
 genomap.egg-info/requires.txt
 genomap.egg-info/top_level.txt
 genomap/bregman_genomap/__init__.py
 genomap/bregman_genomap/bregman_genomap.py
+genomap/genoClassification/__init__.py
+genomap/genoClassification/genoClassification.py
+genomap/genoDR/__init__.py
+genomap/genoDR/genoDimReduction.py
 genomap/genoMOI/__init__.py
 genomap/genoMOI/genoMOI.py
+genomap/genoNetRegression/__init__.py
+genomap/genoNetRegression/genoNet_regression.py
+genomap/genoRegression/__init__.py
+genomap/genoRegression/genoRegression.py
+genomap/genoSig/__init__.py
+genomap/genoSig/genoSig.py
 genomap/genoTraj/__init__.py
 genomap/genoTraj/genoTraj.py
 genomap/genoVis/__init__.py
 genomap/genoVis/genoVis.py
 genomap/genomapOPT/__init__.py
 genomap/genomapOPT/genomapOPT.py
+genomap/genomapT/__init__.py
+genomap/genomapT/genomapT.py
 genomap/utils/ConvDEC.py
 genomap/utils/ConvIDEC.py
 genomap/utils/FcDEC.py
 genomap/utils/FcIDEC.py
 genomap/utils/__init__.py
 genomap/utils/class_discriminative_opt.py
 genomap/utils/gTraj_utils.py
 genomap/utils/group_centroid_opt.py
 genomap/utils/metrics.py
+genomap/utils/util_Sig.py
 genomap/utils/utils_MOI.py
```

### Comparing `genomap-1.1.1/setup.py` & `genomap-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="genomap",
-    version="1.1.1",
+    version="1.2.1",
     author="Md Tauhidul Islam",
     author_email="tauhid@stanford.edu",
     description="Genomap converts tabular gene expression data into spatially meaningful images.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/xinglab-ai/genomap",
     classifiers=[
```

