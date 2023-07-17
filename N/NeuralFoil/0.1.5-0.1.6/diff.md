# Comparing `tmp/NeuralFoil-0.1.5.tar.gz` & `tmp/NeuralFoil-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NeuralFoil-0.1.5.tar", last modified: Mon Jul 17 16:36:43 2023, max compression
+gzip compressed data, was "NeuralFoil-0.1.6.tar", last modified: Mon Jul 17 20:03:02 2023, max compression
```

## Comparing `NeuralFoil-0.1.5.tar` & `NeuralFoil-0.1.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:36:43.018868 NeuralFoil-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-17 16:36:29.000000 NeuralFoil-0.1.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-17 16:36:29.000000 NeuralFoil-0.1.5/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:36:43.014868 NeuralFoil-0.1.5/NeuralFoil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22027 2023-07-17 16:36:42.000000 NeuralFoil-0.1.5/NeuralFoil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-17 16:36:42.000000 NeuralFoil-0.1.5/NeuralFoil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 16:36:42.000000 NeuralFoil-0.1.5/NeuralFoil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-17 16:36:42.000000 NeuralFoil-0.1.5/NeuralFoil.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-17 16:36:42.000000 NeuralFoil-0.1.5/NeuralFoil.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    22027 2023-07-17 16:36:43.018868 NeuralFoil-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20996 2023-07-17 16:36:29.000000 NeuralFoil-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:36:43.014868 NeuralFoil-0.1.5/neuralfoil/
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-17 16:36:29.000000 NeuralFoil-0.1.5/neuralfoil/CL_linear_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-17 16:36:29.000000 NeuralFoil-0.1.5/neuralfoil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8340 2023-07-17 16:36:29.000000 NeuralFoil-0.1.5/neuralfoil/neuralfoil.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:36:43.018868 NeuralFoil-0.1.5/neuralfoil/nn_weights_and_biases/
--rw-r--r--   0 runner    (1001) docker     (123)   139485 2023-07-17 16:36:29.000000 NeuralFoil-0.1.5/neuralfoil/nn_weights_and_biases/nn-large.npz
--rw-r--r--   0 runner    (1001) docker     (123)    39576 2023-07-17 16:36:29.000000 NeuralFoil-0.1.5/neuralfoil/nn_weights_and_biases/nn-medium.npz
--rw-r--r--   0 runner    (1001) docker     (123)    15244 2023-07-17 16:36:29.000000 NeuralFoil-0.1.5/neuralfoil/nn_weights_and_biases/nn-small.npz
--rw-r--r--   0 runner    (1001) docker     (123)   532014 2023-07-17 16:36:29.000000 NeuralFoil-0.1.5/neuralfoil/nn_weights_and_biases/nn-xlarge.npz
--rw-r--r--   0 runner    (1001) docker     (123)     8724 2023-07-17 16:36:29.000000 NeuralFoil-0.1.5/neuralfoil/nn_weights_and_biases/nn-xsmall.npz
--rw-r--r--   0 runner    (1001) docker     (123)   779729 2023-07-17 16:36:29.000000 NeuralFoil-0.1.5/neuralfoil/nn_weights_and_biases/nn-xxlarge.npz
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-07-17 16:36:29.000000 NeuralFoil-0.1.5/neuralfoil/nn_weights_and_biases/nn-xxsmall.npz
--rw-r--r--   0 runner    (1001) docker     (123)  3052473 2023-07-17 16:36:29.000000 NeuralFoil-0.1.5/neuralfoil/nn_weights_and_biases/nn-xxxlarge.npz
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 16:36:43.018868 NeuralFoil-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-17 16:36:29.000000 NeuralFoil-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:03:02.410339 NeuralFoil-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-17 20:02:51.000000 NeuralFoil-0.1.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-17 20:02:51.000000 NeuralFoil-0.1.6/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:03:02.406339 NeuralFoil-0.1.6/NeuralFoil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22027 2023-07-17 20:03:02.000000 NeuralFoil-0.1.6/NeuralFoil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-17 20:03:02.000000 NeuralFoil-0.1.6/NeuralFoil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 20:03:02.000000 NeuralFoil-0.1.6/NeuralFoil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-17 20:03:02.000000 NeuralFoil-0.1.6/NeuralFoil.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-17 20:03:02.000000 NeuralFoil-0.1.6/NeuralFoil.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    22027 2023-07-17 20:03:02.410339 NeuralFoil-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20996 2023-07-17 20:02:51.000000 NeuralFoil-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:03:02.406339 NeuralFoil-0.1.6/neuralfoil/
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-17 20:02:51.000000 NeuralFoil-0.1.6/neuralfoil/CL_linear_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-17 20:02:51.000000 NeuralFoil-0.1.6/neuralfoil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8340 2023-07-17 20:02:51.000000 NeuralFoil-0.1.6/neuralfoil/neuralfoil.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:03:02.406339 NeuralFoil-0.1.6/neuralfoil/nn_weights_and_biases/
+-rw-r--r--   0 runner    (1001) docker     (123)   139485 2023-07-17 20:02:51.000000 NeuralFoil-0.1.6/neuralfoil/nn_weights_and_biases/nn-large.npz
+-rw-r--r--   0 runner    (1001) docker     (123)    39576 2023-07-17 20:02:51.000000 NeuralFoil-0.1.6/neuralfoil/nn_weights_and_biases/nn-medium.npz
+-rw-r--r--   0 runner    (1001) docker     (123)    15244 2023-07-17 20:02:51.000000 NeuralFoil-0.1.6/neuralfoil/nn_weights_and_biases/nn-small.npz
+-rw-r--r--   0 runner    (1001) docker     (123)   532014 2023-07-17 20:02:51.000000 NeuralFoil-0.1.6/neuralfoil/nn_weights_and_biases/nn-xlarge.npz
+-rw-r--r--   0 runner    (1001) docker     (123)     8724 2023-07-17 20:02:51.000000 NeuralFoil-0.1.6/neuralfoil/nn_weights_and_biases/nn-xsmall.npz
+-rw-r--r--   0 runner    (1001) docker     (123)   779729 2023-07-17 20:02:51.000000 NeuralFoil-0.1.6/neuralfoil/nn_weights_and_biases/nn-xxlarge.npz
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-07-17 20:02:51.000000 NeuralFoil-0.1.6/neuralfoil/nn_weights_and_biases/nn-xxsmall.npz
+-rw-r--r--   0 runner    (1001) docker     (123)  3052473 2023-07-17 20:02:51.000000 NeuralFoil-0.1.6/neuralfoil/nn_weights_and_biases/nn-xxxlarge.npz
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 20:03:02.410339 NeuralFoil-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-07-17 20:02:51.000000 NeuralFoil-0.1.6/setup.py
```

### Comparing `NeuralFoil-0.1.5/LICENSE.txt` & `NeuralFoil-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.5/NeuralFoil.egg-info/PKG-INFO` & `NeuralFoil-0.1.6/NeuralFoil.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NeuralFoil
-Version: 0.1.5
+Version: 0.1.6
 Summary: NeuralFoil is an airfoil aerodynamics analysis tool using physics-informed machine learning, in pure Python/NumPy.
 Home-page: https://github.com/peterdsharpe/NeuralFoil
 Author: Peter Sharpe
 Author-email: pds@mit.edu
 Project-URL: Source, https://github.com/peterdsharpe/NeuralFoil
 Project-URL: Bug Reports, https://github.com/peterdsharpe/NeuralFoil/issues
 Keywords: python machine learning analysis optimization aerospace airplane cfd aircraft hydrodynamics aerodynamics sailing propeller airfoil xfoil design mdo mdao physics informed neural network
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: NeuralFoil Version: 0.1.5 Summary: NeuralFoil is an
+Metadata-Version: 2.1 Name: NeuralFoil Version: 0.1.6 Summary: NeuralFoil is an
 airfoil aerodynamics analysis tool using physics-informed machine learning, in
 pure Python/NumPy. Home-page: https://github.com/peterdsharpe/NeuralFoil
 Author: Peter Sharpe Author-email: pds@mit.edu Project-URL: Source, https://
 github.com/peterdsharpe/NeuralFoil Project-URL: Bug Reports, https://
 github.com/peterdsharpe/NeuralFoil/issues Keywords: python machine learning
 analysis optimization aerospace airplane cfd aircraft hydrodynamics
 aerodynamics sailing propeller airfoil xfoil design mdo mdao physics informed
```

### Comparing `NeuralFoil-0.1.5/NeuralFoil.egg-info/SOURCES.txt` & `NeuralFoil-0.1.6/NeuralFoil.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.5/PKG-INFO` & `NeuralFoil-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NeuralFoil
-Version: 0.1.5
+Version: 0.1.6
 Summary: NeuralFoil is an airfoil aerodynamics analysis tool using physics-informed machine learning, in pure Python/NumPy.
 Home-page: https://github.com/peterdsharpe/NeuralFoil
 Author: Peter Sharpe
 Author-email: pds@mit.edu
 Project-URL: Source, https://github.com/peterdsharpe/NeuralFoil
 Project-URL: Bug Reports, https://github.com/peterdsharpe/NeuralFoil/issues
 Keywords: python machine learning analysis optimization aerospace airplane cfd aircraft hydrodynamics aerodynamics sailing propeller airfoil xfoil design mdo mdao physics informed neural network
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: NeuralFoil Version: 0.1.5 Summary: NeuralFoil is an
+Metadata-Version: 2.1 Name: NeuralFoil Version: 0.1.6 Summary: NeuralFoil is an
 airfoil aerodynamics analysis tool using physics-informed machine learning, in
 pure Python/NumPy. Home-page: https://github.com/peterdsharpe/NeuralFoil
 Author: Peter Sharpe Author-email: pds@mit.edu Project-URL: Source, https://
 github.com/peterdsharpe/NeuralFoil Project-URL: Bug Reports, https://
 github.com/peterdsharpe/NeuralFoil/issues Keywords: python machine learning
 analysis optimization aerospace airplane cfd aircraft hydrodynamics
 aerodynamics sailing propeller airfoil xfoil design mdo mdao physics informed
```

### Comparing `NeuralFoil-0.1.5/README.md` & `NeuralFoil-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.5/neuralfoil/CL_linear_regression.py` & `NeuralFoil-0.1.6/neuralfoil/CL_linear_regression.py`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.5/neuralfoil/neuralfoil.py` & `NeuralFoil-0.1.6/neuralfoil/neuralfoil.py`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.5/neuralfoil/nn_weights_and_biases/nn-large.npz` & `NeuralFoil-0.1.6/neuralfoil/nn_weights_and_biases/nn-large.npz`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.5/neuralfoil/nn_weights_and_biases/nn-medium.npz` & `NeuralFoil-0.1.6/neuralfoil/nn_weights_and_biases/nn-medium.npz`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.5/neuralfoil/nn_weights_and_biases/nn-small.npz` & `NeuralFoil-0.1.6/neuralfoil/nn_weights_and_biases/nn-small.npz`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.5/neuralfoil/nn_weights_and_biases/nn-xlarge.npz` & `NeuralFoil-0.1.6/neuralfoil/nn_weights_and_biases/nn-xlarge.npz`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.5/neuralfoil/nn_weights_and_biases/nn-xsmall.npz` & `NeuralFoil-0.1.6/neuralfoil/nn_weights_and_biases/nn-xsmall.npz`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.5/neuralfoil/nn_weights_and_biases/nn-xxlarge.npz` & `NeuralFoil-0.1.6/neuralfoil/nn_weights_and_biases/nn-xxlarge.npz`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.5/neuralfoil/nn_weights_and_biases/nn-xxsmall.npz` & `NeuralFoil-0.1.6/neuralfoil/nn_weights_and_biases/nn-xxsmall.npz`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.5/neuralfoil/nn_weights_and_biases/nn-xxxlarge.npz` & `NeuralFoil-0.1.6/neuralfoil/nn_weights_and_biases/nn-xxxlarge.npz`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.5/setup.py` & `NeuralFoil-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         'Programming Language :: Python :: 3',
     ],
     keywords='python machine learning analysis optimization aerospace airplane cfd aircraft hydrodynamics aerodynamics sailing propeller airfoil xfoil design mdo mdao physics informed neural network',
     packages=["neuralfoil"],  # find_packages(exclude=['docs', 'media', 'examples', 'studies'])
     python_requires='>=3.7',
     install_requires=[
         'numpy >= 1',
-        'aerosandbox >= 4.0.11'
+        'aerosandbox >= 4.1.0'
     ],
     extras_require={
         "training": [
             'torch',
             'ray',
             'polars',
             'tqdm'
```

