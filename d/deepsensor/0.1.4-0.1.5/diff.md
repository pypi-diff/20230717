# Comparing `tmp/deepsensor-0.1.4.tar.gz` & `tmp/deepsensor-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepsensor-0.1.4.tar", last modified: Mon Jul  3 12:19:26 2023, max compression
+gzip compressed data, was "deepsensor-0.1.5.tar", last modified: Mon Jul 17 17:08:16 2023, max compression
```

## Comparing `deepsensor-0.1.4.tar` & `deepsensor-0.1.5.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:19:26.801427 deepsensor-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-07-03 12:19:26.801427 deepsensor-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5827 2023-07-03 12:19:18.000000 deepsensor-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:19:26.797426 deepsensor-0.1.4/deepsensor/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-03 12:19:18.000000 deepsensor-0.1.4/deepsensor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:19:26.797426 deepsensor-0.1.4/deepsensor/active_learning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:19:18.000000 deepsensor-0.1.4/deepsensor/active_learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-07-03 12:19:18.000000 deepsensor-0.1.4/deepsensor/active_learning/acquisition_fns.py
--rw-r--r--   0 runner    (1001) docker     (123)    16761 2023-07-03 12:19:18.000000 deepsensor-0.1.4/deepsensor/active_learning/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-03 12:19:18.000000 deepsensor-0.1.4/deepsensor/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:19:26.797426 deepsensor-0.1.4/deepsensor/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:19:18.000000 deepsensor-0.1.4/deepsensor/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24110 2023-07-03 12:19:18.000000 deepsensor-0.1.4/deepsensor/data/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    15602 2023-07-03 12:19:18.000000 deepsensor-0.1.4/deepsensor/data/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-07-03 12:19:18.000000 deepsensor-0.1.4/deepsensor/data/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-07-03 12:19:18.000000 deepsensor-0.1.4/deepsensor/data/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-03 12:19:18.000000 deepsensor-0.1.4/deepsensor/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:19:26.801427 deepsensor-0.1.4/deepsensor/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:19:18.000000 deepsensor-0.1.4/deepsensor/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20840 2023-07-03 12:19:18.000000 deepsensor-0.1.4/deepsensor/model/convnp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-07-03 12:19:18.000000 deepsensor-0.1.4/deepsensor/model/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    12931 2023-07-03 12:19:18.000000 deepsensor-0.1.4/deepsensor/model/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8597 2023-07-03 12:19:18.000000 deepsensor-0.1.4/deepsensor/model/nps.py
--rw-r--r--   0 runner    (1001) docker     (123)    13109 2023-07-03 12:19:18.000000 deepsensor-0.1.4/deepsensor/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:19:18.000000 deepsensor-0.1.4/deepsensor/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:19:26.801427 deepsensor-0.1.4/deepsensor/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-03 12:19:18.000000 deepsensor-0.1.4/deepsensor/tensorflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:19:26.801427 deepsensor-0.1.4/deepsensor/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-03 12:19:18.000000 deepsensor-0.1.4/deepsensor/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:19:26.801427 deepsensor-0.1.4/deepsensor/train/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:19:18.000000 deepsensor-0.1.4/deepsensor/train/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-07-03 12:19:18.000000 deepsensor-0.1.4/deepsensor/train/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:19:26.797426 deepsensor-0.1.4/deepsensor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-07-03 12:19:26.000000 deepsensor-0.1.4/deepsensor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-03 12:19:26.000000 deepsensor-0.1.4/deepsensor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 12:19:26.000000 deepsensor-0.1.4/deepsensor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 12:19:26.000000 deepsensor-0.1.4/deepsensor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-03 12:19:26.000000 deepsensor-0.1.4/deepsensor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-03 12:19:26.000000 deepsensor-0.1.4/deepsensor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-03 12:19:18.000000 deepsensor-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-03 12:19:26.801427 deepsensor-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-03 12:19:18.000000 deepsensor-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:19:26.801427 deepsensor-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:19:18.000000 deepsensor-0.1.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5007 2023-07-03 12:19:18.000000 deepsensor-0.1.4/tests/test_active_learning.py
--rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-07-03 12:19:18.000000 deepsensor-0.1.4/tests/test_data_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10137 2023-07-03 12:19:18.000000 deepsensor-0.1.4/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-03 12:19:18.000000 deepsensor-0.1.4/tests/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-07-03 12:19:18.000000 deepsensor-0.1.4/tests/test_task_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-07-03 12:19:18.000000 deepsensor-0.1.4/tests/test_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-03 12:19:18.000000 deepsensor-0.1.4/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:08:16.088207 deepsensor-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     7133 2023-07-17 17:08:16.088207 deepsensor-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6735 2023-07-17 17:08:02.000000 deepsensor-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:08:16.084206 deepsensor-0.1.5/deepsensor/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-17 17:08:02.000000 deepsensor-0.1.5/deepsensor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:08:16.084206 deepsensor-0.1.5/deepsensor/active_learning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 17:08:02.000000 deepsensor-0.1.5/deepsensor/active_learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-07-17 17:08:02.000000 deepsensor-0.1.5/deepsensor/active_learning/acquisition_fns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19422 2023-07-17 17:08:02.000000 deepsensor-0.1.5/deepsensor/active_learning/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-17 17:08:02.000000 deepsensor-0.1.5/deepsensor/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:08:16.084206 deepsensor-0.1.5/deepsensor/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 17:08:02.000000 deepsensor-0.1.5/deepsensor/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27308 2023-07-17 17:08:02.000000 deepsensor-0.1.5/deepsensor/data/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16620 2023-07-17 17:08:02.000000 deepsensor-0.1.5/deepsensor/data/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-07-17 17:08:02.000000 deepsensor-0.1.5/deepsensor/data/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-07-17 17:08:02.000000 deepsensor-0.1.5/deepsensor/data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-17 17:08:02.000000 deepsensor-0.1.5/deepsensor/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:08:16.088207 deepsensor-0.1.5/deepsensor/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 17:08:02.000000 deepsensor-0.1.5/deepsensor/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22963 2023-07-17 17:08:02.000000 deepsensor-0.1.5/deepsensor/model/convnp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-07-17 17:08:02.000000 deepsensor-0.1.5/deepsensor/model/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18195 2023-07-17 17:08:02.000000 deepsensor-0.1.5/deepsensor/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8443 2023-07-17 17:08:02.000000 deepsensor-0.1.5/deepsensor/model/nps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14590 2023-07-17 17:08:02.000000 deepsensor-0.1.5/deepsensor/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 17:08:02.000000 deepsensor-0.1.5/deepsensor/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:08:16.088207 deepsensor-0.1.5/deepsensor/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-17 17:08:02.000000 deepsensor-0.1.5/deepsensor/tensorflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:08:16.088207 deepsensor-0.1.5/deepsensor/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-17 17:08:02.000000 deepsensor-0.1.5/deepsensor/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:08:16.088207 deepsensor-0.1.5/deepsensor/train/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 17:08:02.000000 deepsensor-0.1.5/deepsensor/train/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-07-17 17:08:02.000000 deepsensor-0.1.5/deepsensor/train/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:08:16.084206 deepsensor-0.1.5/deepsensor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7133 2023-07-17 17:08:16.000000 deepsensor-0.1.5/deepsensor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-17 17:08:16.000000 deepsensor-0.1.5/deepsensor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 17:08:16.000000 deepsensor-0.1.5/deepsensor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 17:08:16.000000 deepsensor-0.1.5/deepsensor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-17 17:08:16.000000 deepsensor-0.1.5/deepsensor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-17 17:08:16.000000 deepsensor-0.1.5/deepsensor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-17 17:08:02.000000 deepsensor-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-17 17:08:16.088207 deepsensor-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-17 17:08:02.000000 deepsensor-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:08:16.088207 deepsensor-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 17:08:02.000000 deepsensor-0.1.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-07-17 17:08:02.000000 deepsensor-0.1.5/tests/test_active_learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-07-17 17:08:02.000000 deepsensor-0.1.5/tests/test_data_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14775 2023-07-17 17:08:02.000000 deepsensor-0.1.5/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-17 17:08:02.000000 deepsensor-0.1.5/tests/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7495 2023-07-17 17:08:02.000000 deepsensor-0.1.5/tests/test_task_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-07-17 17:08:02.000000 deepsensor-0.1.5/tests/test_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-17 17:08:02.000000 deepsensor-0.1.5/tests/utils.py
```

### Comparing `deepsensor-0.1.4/PKG-INFO` & `deepsensor-0.1.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepsensor
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python package for modelling xarray and pandas data with neural processes.
 Home-page: https://github.com/tom-andersson/deepsensor
 Author: Tom R. Andersson
 Author-email: tomand@bas.ac.uk
 License: MIT
 Platform: unix
 Platform: linux
@@ -22,15 +22,15 @@
 
 
 <p style="text-align: center; font-size: 15px">A Python package and open-source project for modelling environmental
 data with neural processes</p>
 
 -----------
 
-[![release](https://img.shields.io/badge/release-v0.1.3-green?logo=github)](https://github.com/tom-andersson/deepsensor/releases)
+[![release](https://img.shields.io/badge/release-v0.1.5-green?logo=github)](https://github.com/tom-andersson/deepsensor/releases)
 ![Tests](https://github.com/tom-andersson/deepsensor/actions/workflows/tests.yml/badge.svg)
 [![Coverage Status](https://coveralls.io/repos/github/tom-andersson/deepsensor/badge.svg?branch=main)](https://coveralls.io/github/tom-andersson/deepsensor?branch=main)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 **NOTE**: This package is currently undergoing very active development. If you are interested in using
 DeepSensor, please get in touch first (tomand@bas.ac.uk).
 
@@ -66,25 +66,24 @@
 Simply `import deepsensor.torch` or `import deepsensor.tensorflow` to choose between them!
 
 Quick start
 ----------
 
 Here we will demonstrate a simple example of training a convolutional conditional neural process
 (ConvCNP) to spatially interpolate ERA5 data.
-First, pip install the package. In this case we will use the TensorFlow backend.
+First, pip install the package. In this case we will use the PyTorch backend.
 ```bash
 pip install deepsensor
-pip install tensorflow
-pip install tensorflow-probability
+pip install torch
 ```
 
-We can go from imports to predictions with a trained model in <30 lines of code!
+We can go from imports to predictions with a trained model in less than 30 lines of code!
 
 ```python
-import deepsensor.tensorflow
+import deepsensor.torch
 from deepsensor.data.loader import TaskLoader
 from deepsensor.data.processor import DataProcessor
 from deepsensor.model.convnp import ConvNP
 from deepsensor.train.train import train_epoch
 
 import xarray as xr
 import pandas as pd
@@ -102,23 +101,23 @@
 
 # Set up model
 model = ConvNP(data_processor, task_loader)
 
 # Generate training tasks with up to 10% of grid cells passed as context and all grid cells
 # passed as targets
 train_tasks = []
-for date in pd.date_range("2013-01-01", "2014-11-30"):
+for date in pd.date_range("2013-01-01", "2014-11-30")[::7]:
     task = task_loader(date, context_sampling=np.random.uniform(0.0, 0.1), target_sampling="all")
     train_tasks.append(task)
 
 # Train model
-for epoch in range(100):
+for epoch in range(10):
     train_epoch(model, train_tasks, progress_bar=True)
 
-# Predict on new task with 10% of context data
+# Predict on new task with 10% of context data and a dense grid of target points
 test_task = task_loader("2014-12-31", 0.1)
 mean_ds, std_ds = model.predict(test_task, X_t=ds_raw)
 ```
 
 After training, the model can predict directly to `xarray` in your data's original units and coordinate system:
 ```python
 >>> mean_ds
@@ -128,14 +127,36 @@
   * time     (time) datetime64[ns] 2014-12-31
   * lat      (lat) float32 75.0 72.5 70.0 67.5 65.0 ... 25.0 22.5 20.0 17.5 15.0
   * lon      (lon) float32 200.0 202.5 205.0 207.5 ... 322.5 325.0 327.5 330.0
 Data variables:
     air      (time, lat, lon) float32 246.7 244.4 245.5 ... 290.2 289.8 289.4
 ```
 
+We can also predict directly to `pandas` containing a timeseries of predictions at off-grid locations
+by passing a `numpy` array of target locations to the `X_t` argument of `.predict`:
+```python
+# Predict at two off-grid locations for three days in December 2014
+test_tasks = task_loader(pd.date_range("2014-12-01", "2014-12-31"), 0.1)
+mean_df, std_df = model.predict(test_tasks, X_t=np.array([[50, 280], [40, 250]]).T)
+```
+
+```python
+>>> mean_df
+                              air
+time       lat  lon              
+2014-12-01 50.0 280.0  260.183056
+           40.0 250.0  277.947373
+2014-12-02 50.0 280.0   261.08943
+           40.0 250.0  278.219599
+2014-12-03 50.0 280.0  257.128185
+           40.0 250.0  278.444229
+```
+
+This quickstart example is also available as a [Jupyter notebook](https://github.com/tom-andersson/deepsensor/blob/main/notebooks/quickstart_example.ipynb) with added visualisations.
+
 Extending DeepSensor with new models
 ----------
 To extend DeepSensor with a new model, simply create a new class that inherits from `deepsensor.model.DeepSensorModel`
 and implement the low-level prediction methods defined in `deepsensor.model.ProbabilisticModel`,
 such as `.mean` and `.stddev`.
 ```python
 class NewModel(DeepSensorModel):
```

### Comparing `deepsensor-0.1.4/README.md` & `deepsensor-0.1.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 <p style="text-align: center; font-size: 15px">A Python package and open-source project for modelling environmental
 data with neural processes</p>
 
 -----------
 
-[![release](https://img.shields.io/badge/release-v0.1.3-green?logo=github)](https://github.com/tom-andersson/deepsensor/releases)
+[![release](https://img.shields.io/badge/release-v0.1.5-green?logo=github)](https://github.com/tom-andersson/deepsensor/releases)
 ![Tests](https://github.com/tom-andersson/deepsensor/actions/workflows/tests.yml/badge.svg)
 [![Coverage Status](https://coveralls.io/repos/github/tom-andersson/deepsensor/badge.svg?branch=main)](https://coveralls.io/github/tom-andersson/deepsensor?branch=main)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 **NOTE**: This package is currently undergoing very active development. If you are interested in using
 DeepSensor, please get in touch first (tomand@bas.ac.uk).
 
@@ -51,25 +51,24 @@
 Simply `import deepsensor.torch` or `import deepsensor.tensorflow` to choose between them!
 
 Quick start
 ----------
 
 Here we will demonstrate a simple example of training a convolutional conditional neural process
 (ConvCNP) to spatially interpolate ERA5 data.
-First, pip install the package. In this case we will use the TensorFlow backend.
+First, pip install the package. In this case we will use the PyTorch backend.
 ```bash
 pip install deepsensor
-pip install tensorflow
-pip install tensorflow-probability
+pip install torch
 ```
 
-We can go from imports to predictions with a trained model in <30 lines of code!
+We can go from imports to predictions with a trained model in less than 30 lines of code!
 
 ```python
-import deepsensor.tensorflow
+import deepsensor.torch
 from deepsensor.data.loader import TaskLoader
 from deepsensor.data.processor import DataProcessor
 from deepsensor.model.convnp import ConvNP
 from deepsensor.train.train import train_epoch
 
 import xarray as xr
 import pandas as pd
@@ -87,23 +86,23 @@
 
 # Set up model
 model = ConvNP(data_processor, task_loader)
 
 # Generate training tasks with up to 10% of grid cells passed as context and all grid cells
 # passed as targets
 train_tasks = []
-for date in pd.date_range("2013-01-01", "2014-11-30"):
+for date in pd.date_range("2013-01-01", "2014-11-30")[::7]:
     task = task_loader(date, context_sampling=np.random.uniform(0.0, 0.1), target_sampling="all")
     train_tasks.append(task)
 
 # Train model
-for epoch in range(100):
+for epoch in range(10):
     train_epoch(model, train_tasks, progress_bar=True)
 
-# Predict on new task with 10% of context data
+# Predict on new task with 10% of context data and a dense grid of target points
 test_task = task_loader("2014-12-31", 0.1)
 mean_ds, std_ds = model.predict(test_task, X_t=ds_raw)
 ```
 
 After training, the model can predict directly to `xarray` in your data's original units and coordinate system:
 ```python
 >>> mean_ds
@@ -113,14 +112,36 @@
   * time     (time) datetime64[ns] 2014-12-31
   * lat      (lat) float32 75.0 72.5 70.0 67.5 65.0 ... 25.0 22.5 20.0 17.5 15.0
   * lon      (lon) float32 200.0 202.5 205.0 207.5 ... 322.5 325.0 327.5 330.0
 Data variables:
     air      (time, lat, lon) float32 246.7 244.4 245.5 ... 290.2 289.8 289.4
 ```
 
+We can also predict directly to `pandas` containing a timeseries of predictions at off-grid locations
+by passing a `numpy` array of target locations to the `X_t` argument of `.predict`:
+```python
+# Predict at two off-grid locations for three days in December 2014
+test_tasks = task_loader(pd.date_range("2014-12-01", "2014-12-31"), 0.1)
+mean_df, std_df = model.predict(test_tasks, X_t=np.array([[50, 280], [40, 250]]).T)
+```
+
+```python
+>>> mean_df
+                              air
+time       lat  lon              
+2014-12-01 50.0 280.0  260.183056
+           40.0 250.0  277.947373
+2014-12-02 50.0 280.0   261.08943
+           40.0 250.0  278.219599
+2014-12-03 50.0 280.0  257.128185
+           40.0 250.0  278.444229
+```
+
+This quickstart example is also available as a [Jupyter notebook](https://github.com/tom-andersson/deepsensor/blob/main/notebooks/quickstart_example.ipynb) with added visualisations.
+
 Extending DeepSensor with new models
 ----------
 To extend DeepSensor with a new model, simply create a new class that inherits from `deepsensor.model.DeepSensorModel`
 and implement the low-level prediction methods defined in `deepsensor.model.ProbabilisticModel`,
 such as `.mean` and `.stddev`.
 ```python
 class NewModel(DeepSensorModel):
```

### Comparing `deepsensor-0.1.4/deepsensor/__init__.py` & `deepsensor-0.1.5/deepsensor/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.4/deepsensor/active_learning/acquisition_fns.py` & `deepsensor-0.1.5/deepsensor/active_learning/acquisition_fns.py`

 * *Files 18% similar despite different names*

```diff
@@ -29,14 +29,18 @@
 
         Returns:
             np.ndarray: Acquisition function value/s. Shape ().
         """
         raise NotImplementedError
 
 
+class AcquisitionFunctionOracle(AcquisitionFunction):
+    """Signifies that the acquisition function is computed using the true target values."""
+
+
 class AcquisitionFunctionParallel(AcquisitionFunction):
     """
     Parent class for acquisition functions that are computed across all search points in parallel.
     """
 
     def __call__(self, task: Task, X_s: np.ndarray):
         """
@@ -88,14 +92,48 @@
 class JointEntropy(AcquisitionFunction):
     """Joint entropy of the predictive distribution."""
 
     def __call__(self, task):
         return self.model.joint_entropy(task)
 
 
+class OracleMAE(AcquisitionFunctionOracle):
+    """Oracle mean absolute error."""
+
+    def __call__(self, task):
+        pred = self.model.mean(task)
+        true = task["Y_t"]
+        return np.mean(np.abs(pred - true))
+
+
+class OracleRMSE(AcquisitionFunctionOracle):
+    """Oracle root mean squared error."""
+
+    def __call__(self, task):
+        pred = self.model.mean(task)
+        true = task["Y_t"]
+        return np.sqrt(np.mean((pred - true) ** 2))
+
+
+class OracleMarginalNLL(AcquisitionFunctionOracle):
+    """Oracle marginal negative log-likelihood."""
+
+    def __call__(self, task):
+        pred = self.model.mean(task)
+        true = task["Y_t"]
+        return -np.mean(norm.logpdf(true, loc=pred, scale=self.model.stddev(task)))
+
+
+class OracleJointNLL(AcquisitionFunctionOracle):
+    """Oracle joint negative log-likelihood."""
+
+    def __call__(self, task):
+        return -self.model.logpdf(task)
+
+
 class Random(AcquisitionFunctionParallel):
     """Random acquisition function."""
 
     def __init__(self, seed: int = 42):
         self.rng = np.random.default_rng(seed)
 
     def __call__(self, task, X_s):
@@ -136,15 +174,18 @@
         task = copy.deepcopy(task)
         task["X_t"] = X_s
 
         return self.model.stddev(task)[target_set_idx]
 
 
 class ExpectedImprovement(AcquisitionFunctionParallel):
-    """Expected improvement acquisition function."""
+    """Expected improvement acquisition function
+
+    Note, the current implementation of this acquisition function is only valid for maximisation.
+    """
 
     def __init__(self, model: ProbabilisticModel, context_set_idx: int = 0):
         """
         Args:
             model (ProbabilisticModel):
             context_set_idx (int): Index of context set to add new observations to when computing
                 the acquisition function.
@@ -165,16 +206,21 @@
         # Set the target points to the search points
         task = copy.deepcopy(task)
         task["X_t"] = X_s
 
         # Compute the predictive mean and variance of the target set
         mean = self.model.mean(task)[target_set_idx]
 
-        # Compute the best target value seen so far
-        best_target_value = task["Y_c"][self.context_set_idx].max()
+        if task["Y_c"][self.context_set_idx].size == 0:
+            # No previous context points, so heuristically use the predictive mean as the
+            # acquisition function. This will at least select the most positive predicted mean.
+            return self.model.mean(task)[target_set_idx]
+        else:
+            # Determine the best target value seen so far
+            best_target_value = task["Y_c"][self.context_set_idx].max()
 
         # Compute the standard deviation of the context set
         stddev = self.model.stddev(task)[self.context_set_idx]
 
         # Compute the expected improvement
         Z = (mean - best_target_value) / stddev
         ei = stddev * (mean - best_target_value) * norm.cdf(Z) + stddev * norm.pdf(Z)
```

### Comparing `deepsensor-0.1.4/deepsensor/active_learning/algorithms.py` & `deepsensor-0.1.5/deepsensor/active_learning/algorithms.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 import copy
 
+from deepsensor.data.loader import TaskLoader
 from deepsensor.data.processor import (
     xarray_to_coord_array_normalised,
     mask_coord_array_normalised,
+    da1_da2_same_grid,
+    interp_da1_to_da2,
 )
 from deepsensor.model.model import DeepSensorModel, create_empty_spatiotemporal_xarray
 from deepsensor.data.task import Task, append_obs_to_task
 from deepsensor.active_learning.acquisition_fns import (
     AcquisitionFunction,
     AcquisitionFunctionParallel,
+    AcquisitionFunctionOracle,
 )
 
 import numpy as np
 import xarray as xr
 import pandas as pd
 from tqdm import tqdm
 
@@ -28,35 +32,47 @@
         X_s: Union[xr.Dataset, xr.DataArray, pd.DataFrame, pd.Series, pd.Index],
         X_t: Union[xr.Dataset, xr.DataArray, pd.DataFrame, pd.Series, pd.Index],
         X_s_mask: Union[xr.Dataset, xr.DataArray] = None,
         X_t_mask: Union[xr.Dataset, xr.DataArray] = None,
         N_new_context: int = 1,
         X_normalised: bool = False,
         model_infill_method: str = "mean",
-        query_groundtruth: xr.DataArray = None,  # TODO remove "groundtruth" from name?
-        placed_groundtruth: xr.DataArray = None,  # TODO rename to "proposed_"?
+        query_infill: xr.DataArray = None,
+        proposed_infill: xr.DataArray = None,
         context_set_idx: int = 0,
         target_set_idx: int = 0,
         progress_bar: int = 0,
         min_or_max: str = "min",
+        task_loader: TaskLoader = None,  # OPTIONAL for oracle acquisition functions only
+        verbose: bool = False,
     ):
+        """
+
+        Arguments:
+            model {DeepSensorModel} -- Trained model to use for proposing new context points.
+            X_s {Union[xr.Dataset, xr.DataArray} -- Search coordinates.
+            X_t {Union[xr.Dataset, xr.DataArray} -- Target coordinates.
+            X_s_mask {Union[xr.Dataset, xr.DataArray], optional} -- Mask for search coordinates.
+                If provided, only points where mask is True will be considered. Defaults to None.
+        """
         if not isinstance(model, DeepSensorModel):
             raise ValueError(
                 f"`model` must inherit from DeepSensorModel, but parent classes are {model.__class__.__bases__}"
             )
 
+        self._validate_n_new_context(X_s, N_new_context)
+
         self.model = model
         self.N_new_context = N_new_context
         self.progress_bar = progress_bar
         self.model_infill_method = model_infill_method
-        self.query_groundtruth = query_groundtruth
-        self.placed_groundtruth = placed_groundtruth
         self.context_set_idx = context_set_idx
         self.target_set_idx = target_set_idx
         self.min_or_max = min_or_max
+        self.task_loader = task_loader
 
         self.X_s_mask = X_s_mask
         self.X_t_mask = X_t_mask
 
         if min_or_max not in ["min", "max"]:
             raise ValueError(
                 f"min_or_max must be 'min' or 'max', not {self.min_or_max}"
@@ -76,47 +92,56 @@
 
         self.X_s = X_s
         self.X_t = X_t
 
         # Interpolate masks onto search and target coords
         self.X_s_mask, self.X_t_mask = self._process_masks(X_s_mask, X_t_mask, X_s, X_t)
 
-        self._validate_n_new_context(X_s, N_new_context)
+        # Interpolate overridden infill datasets at search points if necessary
+        if query_infill is not None and not da1_da2_same_grid(query_infill, X_s):
+            if verbose:
+                print("query_infill not on search grid, interpolating.")
+            query_infill = interp_da1_to_da2(query_infill, self.X_s)
+        if proposed_infill is not None and not da1_da2_same_grid(proposed_infill, X_s):
+            if verbose:
+                print("proposed_infill not on search grid, interpolating.")
+            proposed_infill = interp_da1_to_da2(proposed_infill, self.X_s)
+        self.query_infill = query_infill
+        self.proposed_infill = proposed_infill
 
         # Convert target coords to numpy arrays and assign to tasks
         if isinstance(X_t, (xr.Dataset, xr.DataArray)):
             if self.X_t_mask is None:
                 # Targets on grid
                 self.X_t_arr = (X_t["x1"].values, X_t["x2"].values)
             else:
                 # Remove points that lie outside the mask
                 X_t_arr_all = xarray_to_coord_array_normalised(X_t)
                 self.X_t_arr = mask_coord_array_normalised(X_t_arr_all, self.X_t_mask)
-        elif isinstance(X_s, (pd.DataFrame, pd.Series, pd.Index)):
+        elif isinstance(X_t, (pd.DataFrame, pd.Series, pd.Index)):
             self.X_t_arr = X_t.reset_index()[["x1", "x2"]].values.T
         else:
             raise TypeError(f"Unsupported type for X_t: {type(X_t)}")
 
         # Construct search array
         if isinstance(X_s, (xr.Dataset, xr.DataArray)):
             X_s_arr = xarray_to_coord_array_normalised(X_s)
             if X_s_mask is not None:
-                # Why are there more values in X_s than X_s_mask?
-                # Probably because
                 X_s_arr = mask_coord_array_normalised(X_s_arr, self.X_s_mask)
         self.X_s_arr = X_s_arr
 
         self.X_new = []  # List of new proposed context locations
 
     @classmethod
     def _validate_n_new_context(
         cls, X_s: Union[xr.Dataset, xr.DataArray], N_new_context: int
     ):
         if isinstance(X_s, (xr.Dataset, xr.DataArray)):
-            X_s = X_s.to_array()
+            if isinstance(X_s, xr.Dataset):
+                X_s = X_s.to_array()
             N_s = X_s.shape[-2] * X_s.shape[-1]
         elif isinstance(X_s, (pd.DataFrame, pd.Series, pd.Index)):
             N_s = len(X_s)
 
         if not 0 < N_new_context < N_s:
             raise ValueError(
                 f"Number of new context ({N_new_context}) must be greater than zero "
@@ -124,19 +149,23 @@
             )
 
     @classmethod
     def _process_masks(cls, X_s_mask: xr.DataArray, X_t_mask: xr.DataArray, X_s, X_t):
         """Process masks by interpolating to X_s and X_t"""
         # TODO avoid repeated code
         if X_s_mask is not None:
-            X_s_mask = X_s_mask.interp_like(X_s, method="nearest")
+            X_s_mask = X_s_mask.astype(float).interp_like(
+                X_s, method="nearest", kwargs={"fill_value": 0}
+            )
             X_s_mask.data = X_s_mask.data.astype(bool)
             X_s_mask.load()
         if X_t_mask is not None:
-            X_t_mask = X_t_mask.interp_like(X_t, method="nearest")
+            X_t_mask = X_t_mask.astype(float).interp_like(
+                X_t, method="nearest", kwargs={"fill_value": 0}
+            )
             X_t_mask.data = X_t_mask.data.astype(bool)
             X_t_mask.load()
 
         return X_s_mask, X_t_mask
 
     def _get_times_from_tasks(self):
         """Get times from tasks"""
@@ -176,15 +205,15 @@
         passed back in to the model at the chosen placement locations in the order of greedy
         placement.  - Yes this is correct. TODO integrate in docstring.
         """
         if self.model_infill_method == "mean":
             infill_ds, _ = self.model.predict(
                 self.tasks,
                 X_s,
-                X_t_normalised=True,
+                X_t_is_normalised=True,
                 unnormalise=False,
                 progress_bar=self.progress_bar >= 4,
             )
 
         elif self.model_infill_method == "sample":
             # _, _, infill_ds = self.model.predict(
             #     self.tasks, X_s, X_t_normalised=True, unnormalise=False,
@@ -200,22 +229,27 @@
         else:
             raise ValueError(
                 f"Unsupported model_infill_method: {self.model_infill_method}"
             )
 
         return infill_ds
 
-    def _sample_y_infill(self, time, x1, x2):
+    def _sample_y_infill(self, infill_ds, time, x1, x2):
         """Sample infill values at a single location"""
-        if isinstance(self.infill_ds, (xr.Dataset, xr.DataArray)):
-            y = self.infill_ds.sel(time=time, x1=x1, x2=x2)
-            y = y.to_array().data
+        if isinstance(infill_ds, (xr.Dataset, xr.DataArray)):
+            y = infill_ds.sel(time=time, x1=x1, x2=x2)
+            if isinstance(y, xr.Dataset):
+                y = y.to_array()
+            y = y.data
             y = y.reshape(1, y.size)  # 1 observation with N dimensions
         else:
-            raise NotImplementedError("TODO")
+            raise NotImplementedError(
+                f"infill_ds must be xr.Dataset or xr.DataArray, "
+                f"not {type(infill_ds)}"
+            )
         return y
 
     def _build_acquisition_fn_ds(self, X_s: Union[xr.Dataset, xr.DataArray]):
         """Initialise xr.DataArray for storing acquisition function values on search grid"""
         prepend_dims = ["iteration"]  # , "sample"]  # MC sample TODO
         prepend_coords = {
             "iteration": range(self.N_new_context),
@@ -286,30 +320,37 @@
                     np.rollaxis(self.X_s_arr[:, np.newaxis], 2),
                     desc="Search",
                     position=6,
                     leave=True,
                     disable=self.progress_bar < 5,
                 ):
                     y_query = self._sample_y_infill(
-                        time=task["time"], x1=x_query[0], x2=x_query[1]
+                        self.query_infill,
+                        time=task["time"],
+                        x1=x_query[0],
+                        x2=x_query[1],
                     )
                     task_with_new = append_obs_to_task(
                         task, x_query, y_query, self.context_set_idx
                     )
                     importance = acquisition_fn(task_with_new)
 
                     # TODO make computing the difference a bool
                     importance = importance - importance_bef
 
                     importances.append(importance)
 
             else:
+                allowed_classes = [
+                    AcquisitionFunction,
+                    AcquisitionFunctionParallel,
+                    AcquisitionFunctionOracle,
+                ]
                 raise ValueError(
-                    f"Acquisition function needs to inherit from AcquisitionFunction or AcquisitionFunctionParallel "
-                    f"but inherits from {acquisition_fn.__class__.__name__}"
+                    f"Acquisition function needs to inherit from one of {allowed_classes}."
                 )
 
             importances = np.array(importances)
             importances_list.append(importances)
 
             if self.X_s_mask is not None:
                 self.acquisition_fn_ds.loc[self.iteration, task["time"]].data[
@@ -362,33 +403,50 @@
     ) -> Tuple[pd.DataFrame, xr.Dataset]:  # TODO is this correct use of typing?
         """
         Iteratively... docstring TODO
 
         Returns a tensor of proposed new sensor locations (in greedy iteration/priority order)
             and their corresponding list of indexes in the search space.
         """
+        if (
+            isinstance(acquisition_fn, AcquisitionFunctionOracle)
+            and self.task_loader is None
+        ):
+            raise ValueError(
+                "AcquisitionFunctionOracle requires a task_loader function to be passed to the GreedyOptimal constructor."
+            )
+
         self.min_or_max = min_or_max
 
         if isinstance(tasks, Task):
             tasks = [tasks]
 
         # Make deepcopys so that original tasks are not modified
         tasks = copy.deepcopy(tasks)
 
         # Add target set to tasks
         for i, task in enumerate(tasks):
             tasks[i]["X_t"][self.target_set_idx] = self.X_t_arr
+            if isinstance(acquisition_fn, AcquisitionFunctionOracle):
+                # Sample ground truth y-values at target points `self.X_t_arr` using `self.task_loader`
+                date = tasks[i]["time"]
+                task_with_Y_t = self.task_loader(
+                    date, context_sampling=0, target_sampling=self.X_t_arr
+                )
+                tasks[i]["Y_t"] = task_with_Y_t["Y_t"]
 
         self.tasks = tasks
 
-        # Generate infill values at search points
-        if self.query_groundtruth is not None:
-            self.infill_ds = self.query_groundtruth
-        else:
-            self.infill_ds = self._model_infill_at_search_points(self.X_s)
+        # Generate infill values at search points if not overridden
+        if self.query_infill is None or self.proposed_infill is None:
+            model_infill = self._model_infill_at_search_points(self.X_s)
+            if self.query_infill is None:
+                self.query_infill = model_infill
+            if self.proposed_infill is None:
+                self.proposed_infill = model_infill
 
         # Instantiate empty acquisition function object
         self._init_acquisition_fn_ds(self.X_s)
 
         self.iteration = 0
 
         # List of new proposed sensor locations
@@ -404,17 +462,18 @@
             desc="Placement",
             position=2,
             leave=True,
             disable=self.progress_bar < 3,
         ):
             x_new = self._single_greedy_iteration(acquisition_fn)
 
+            # Append new proposed context points to each task
             for i, task in enumerate(self.tasks):
                 y_new = self._sample_y_infill(
-                    time=task["time"], x1=x_new[0], x2=x_new[1]
+                    self.proposed_infill, time=task["time"], x1=x_new[0], x2=x_new[1]
                 )
                 self.tasks[i] = append_obs_to_task(
                     task, x_new, y_new, self.context_set_idx
                 )
 
         X_new = np.concatenate(self.X_new, axis=1)
```

### Comparing `deepsensor-0.1.4/deepsensor/data/loader.py` & `deepsensor-0.1.5/deepsensor/data/loader.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 import numpy as np
 import xarray as xr
 import pandas as pd
 
 from typing import List, Tuple, Union
 
+from deepsensor.errors import InvalidSamplingStrategyError
+
 
 class TaskLoader:
     def __init__(
         self,
         context: Union[
             xr.DataArray,
             xr.Dataset,
@@ -23,14 +25,15 @@
             List[Union[xr.DataArray, xr.Dataset, pd.DataFrame]],
         ],
         links: Union[Tuple, List[Tuple[int, int]], None] = None,
         context_delta_t: Union[int, List[int]] = 0,
         target_delta_t: Union[int, List[int]] = 0,
         time_freq: str = "D",
         xarray_interp_method: str = "linear",
+        discrete_xarray_sampling: bool = False,
         dtype: object = "float32",
     ) -> None:
         """Initialise a TaskLoader object
 
         :param context: Context data. Can be a single xr.DataArray, xr.Dataset or pd.DataFrame,
             or a list/tuple of these.
         :param target: Target data. Can be a single xr.DataArray, xr.Dataset or pd.DataFrame,
@@ -41,19 +44,23 @@
             link. If None, no links are specified. Default: None.
         :param context_delta_t: Time difference between context data and t=0 (task init time).
             Can be a single int (same for all context data) or a list/tuple of ints.
         :param target_delta_t: Time difference between target data and t=0 (task init time).
             Can be a single int (same for all target data) or a list/tuple of ints.
         :param time_freq: Time frequency of the data. Default: 'D' (daily).
         :param xarray_interp_method: Interpolation method to use when interpolating xr.DataArray
+        :param discrete_xarray_sampling: When randomly sampling xarray variables, whether to sample
+            at discrete points defined at grid cell centres, or at continuous points within the grid.
+            Default is False.
         :param dtype: Data type of the data. Used to cast the data to the specified dtype.
             Default: 'float32'.
         """
         self.time_freq = time_freq
         self.xarray_interp_method = xarray_interp_method
+        self.discrete_xarray_sampling = discrete_xarray_sampling
         self.dtype = dtype
 
         if isinstance(context, (xr.DataArray, xr.Dataset, pd.DataFrame, pd.Series)):
             context = (context,)
         if isinstance(target, (xr.DataArray, xr.Dataset, pd.DataFrame, pd.Series)):
             target = (target,)
         context, target = self.cast_context_and_target_to_dtype(context, target)
@@ -287,60 +294,86 @@
 
         if isinstance(sampling_strat, float):
             sampling_strat = int(sampling_strat * da.size)
 
         if isinstance(sampling_strat, (int, np.integer)):
             N = sampling_strat
             rng = np.random.default_rng(seed)
-            x1 = rng.choice(da.coords["x1"].values, N, replace=True)
-            x2 = rng.choice(da.coords["x2"].values, N, replace=True)
-            X_c = np.array([x1, x2])
-            Y_c = da.sel(x1=xr.DataArray(x1), x2=xr.DataArray(x2)).data
+            if self.discrete_xarray_sampling:
+                x1 = rng.choice(da.coords["x1"].values, N, replace=True)
+                x2 = rng.choice(da.coords["x2"].values, N, replace=True)
+                Y_c = da.sel(x1=xr.DataArray(x1), x2=xr.DataArray(x2)).data
+            elif not self.discrete_xarray_sampling:
+                if N == 0:
+                    # Catch zero-context edge case before interp fails
+                    X_c = np.zeros((2, 0), dtype=self.dtype)
+                    if isinstance(da, xr.Dataset):
+                        dim = len(da.data_vars)  # Multiple data variables
+                    elif isinstance(da, xr.DataArray):
+                        dim = 1  # Single data variable
+                    Y_c = np.zeros((dim, 0), dtype=self.dtype)
+                    return X_c, Y_c
+                x1 = rng.uniform(da.coords["x1"].min(), da.coords["x1"].max(), N)
+                x2 = rng.uniform(da.coords["x2"].min(), da.coords["x2"].max(), N)
+                Y_c = da.interp(
+                    x1=xr.DataArray(x1),
+                    x2=xr.DataArray(x2),
+                    method=self.xarray_interp_method,
+                    kwargs=dict(fill_value=None, bounds_error=True),
+                )
+                Y_c = np.array(Y_c, dtype=self.dtype)
+            X_c = np.array([x1, x2], dtype=self.dtype)
             if Y_c.ndim == 1:
                 # returned a 1D array, but we need a 2D array of shape (variable, N)
                 Y_c = Y_c.reshape(1, *Y_c.shape)
 
         elif isinstance(sampling_strat, np.ndarray):
             X_c = sampling_strat.astype(self.dtype)
-            Y_c = np.array(
-                da.interp(
+            try:
+                Y_c = da.interp(
                     x1=xr.DataArray(X_c[0]),
                     x2=xr.DataArray(X_c[1]),
                     method=self.xarray_interp_method,
-                    kwargs=dict(fill_value=None, bounds_error=False),
-                ),
-                dtype=self.dtype,
-            )
+                    kwargs=dict(fill_value=None, bounds_error=True),
+                )
+            except ValueError:
+                raise InvalidSamplingStrategyError(
+                    f"Passed a numpy coordinate array to sample xarray object, "
+                    f"but the coordinates are out of bounds."
+                )
+            Y_c = np.array(Y_c, dtype=self.dtype)
             if Y_c.ndim == 1:
                 # returned a 1D array, but we need a 2D array of shape (variable, N)
                 Y_c = Y_c.reshape(1, *Y_c.shape)
 
         elif sampling_strat == "all":
             X_c = (
                 da.coords["x1"].values[np.newaxis],
                 da.coords["x2"].values[np.newaxis],
             )
             Y_c = da.data
             if Y_c.ndim == 2:
                 # returned a 2D array, but we need a 3D array of shape (variable, N_x1, N_x2)
                 Y_c = Y_c.reshape(1, *Y_c.shape)
         else:
-            raise ValueError(f"Unknown sampling strategy {sampling_strat}")
+            raise InvalidSamplingStrategyError(
+                f"Unknown sampling strategy {sampling_strat}"
+            )
 
         return X_c, Y_c
 
     def sample_df(
         self,
         df: Union[pd.DataFrame, pd.Series],
-        sampling_strat: Union[str, int, float],
+        sampling_strat: Union[str, int, float, np.ndarray],
         seed: int = None,
     ) -> (np.ndarray, np.ndarray):
         """Sample a DataArray according to a given strategy
 
-        :param da: DataArray to sample, assumed to be sliced for the task already
+        :param da: DataArray to sample, assumed to be time-sliced for the task already
         :param sampling_strat: Sampling strategy, either "all" or an integer for random grid cell sampling
         :param seed: Seed for random sampling
         :return: Sampled DataArray
         """
         df = df.dropna(how="any")  # If any obs are NaN, drop them
 
         if isinstance(sampling_strat, float):
@@ -353,30 +386,48 @@
             X_c = df.loc[idx].reset_index()[["x1", "x2"]].values.T.astype(self.dtype)
             Y_c = df.loc[idx].values.T
         elif sampling_strat in ["all", "split"]:
             # NOTE if "split", we assume that the context-target split has already been applied to the df
             # in an earlier scope with access to both the context and target data. This is maybe risky!
             X_c = df.reset_index()[["x1", "x2"]].values.T.astype(self.dtype)
             Y_c = df.values.T
+        elif isinstance(sampling_strat, np.ndarray):
+            X_c = sampling_strat.astype(self.dtype)
+            x1match = np.in1d(df.index.get_level_values("x1"), X_c[0])
+            x2match = np.in1d(df.index.get_level_values("x2"), X_c[1])
+            num_matches = np.sum(x1match & x2match)
+
+            # Check that we got all the samples we asked for
+            if num_matches != X_c.shape[1]:
+                raise InvalidSamplingStrategyError(
+                    f"Passed a numpy coordinate array to sample pandas DataFrame, "
+                    f"but the DataFrame did not contain all the requested samples. "
+                    f"Requested {X_c.shape[1]} samples but only got {num_matches}."
+                )
+
+            Y_c = df[x1match & x2match].values.T
         else:
-            raise ValueError(f"Unknown sampling strategy {sampling_strat}")
+            raise InvalidSamplingStrategyError(
+                f"Unknown sampling strategy {sampling_strat}"
+            )
 
         return X_c, Y_c
 
     def task_generation(
         self,
         date: pd.Timestamp,
         context_sampling: Union[
             str, int, float, np.ndarray, List[Union[str, int, float, np.ndarray]]
         ] = "all",
         target_sampling: Union[
             str, int, float, np.ndarray, List[Union[str, int, float, np.ndarray]]
         ] = "all",
         split_frac: float = 0.5,
-        deterministic: bool = False,
+        datewise_deterministic: bool = False,
+        seed_override=None,
     ) -> Task:
         """Generate a task for a given date
 
         There are several sampling strategies available for the context and target data:
         - "all": Sample all observations.
         - int: Sample N observations uniformly at random.
         - float: Sample a fraction of observations uniformly at random.
@@ -387,15 +438,17 @@
         :param context_sampling: Sampling strategy for the context data, either a list of
             sampling strategies for each context set, or a single strategy applied to all context sets
         :param target_sampling: Sampling strategy for the target data, either a list of
             sampling strategies for each target set, or a single strategy applied to all target sets
         :param split_frac: The fraction of observations to use for the context set with the "split"
             sampling strategy for linked context and target set pairs. The remaining observations
             are used for the target set. Default is 0.5.
-        :param: deterministic: Whether random sampling is deterministic based on the date. Default is False.
+        :param: datewise_deterministic: Whether random sampling is datewise_deterministic based on the date. Default is False.
+        :param seed_override: Override the seed for random sampling. This can be used to use the same
+            random sampling at different `date`s. Default is None.
         :return: Task object containing the context and target data
         """
 
         def check_sampling_strat(sampling_strat, set):
             """Check the sampling strategy
 
             Ensure `sampling_strat` is either a single strategy (broadcast to all sets) or a list
@@ -403,34 +456,38 @@
             of sets and return.
             """
             if not isinstance(sampling_strat, (list, tuple)):
                 sampling_strat = tuple([sampling_strat] * len(set))
             elif isinstance(sampling_strat, (list, tuple)) and len(
                 sampling_strat
             ) != len(set):
-                raise ValueError(
-                    f"Length of sampling_strat ({len(sampling_strat)}) must match number of"
+                raise InvalidSamplingStrategyError(
+                    f"Length of sampling_strat ({len(sampling_strat)}) must match number of "
                     f"context sets ({len(set)})"
                 )
 
             for strat in sampling_strat:
                 if not isinstance(strat, (str, int, np.integer, float, np.ndarray)):
-                    raise ValueError(
+                    raise InvalidSamplingStrategyError(
                         f"Unknown sampling strategy {strat} of type {type(strat)}"
                     )
-                if isinstance(strat, str) and strat not in ["all", "split"]:
-                    raise ValueError(f"Unknown sampling strategy {strat} for type str")
-                if isinstance(strat, float) and not 0 <= strat <= 1:
-                    raise ValueError(
+                elif isinstance(strat, str) and strat not in ["all", "split"]:
+                    raise InvalidSamplingStrategyError(
+                        f"Unknown sampling strategy {strat} for type str"
+                    )
+                elif isinstance(strat, float) and not 0 <= strat <= 1:
+                    raise InvalidSamplingStrategyError(
                         f"If sampling strategy is a float, must be fraction must be in [0, 1], got {strat}"
                     )
-                if isinstance(strat, int) and strat <= 0:
-                    raise ValueError(f"Sampling N must be positive, got {strat}")
-                if isinstance(strat, np.ndarray) and strat.shape[0] != 2:
-                    raise ValueError(
+                elif isinstance(strat, int) and strat < 0:
+                    raise InvalidSamplingStrategyError(
+                        f"Sampling N must be positive, got {strat}"
+                    )
+                elif isinstance(strat, np.ndarray) and strat.shape[0] != 2:
+                    raise InvalidSamplingStrategyError(
                         f"Sampling coordinates must be of shape (2, N), got {strat.shape}"
                     )
 
             return sampling_strat
 
         def time_slice_variable(var, delta_t):
             """Slice a variable by a given time delta"""
@@ -478,15 +535,18 @@
             raise ValueError(
                 "Cannot use 'split' sampling strategy for target set and not context set"
             )
 
         if not isinstance(date, pd.Timestamp):
             date = pd.Timestamp(date)
 
-        if deterministic:
+        if seed_override is not None:
+            # Override the seed for random sampling
+            seed = seed_override
+        elif datewise_deterministic:
             # Generate a deterministic seed, based on the date, for random sampling
             seed = int(date.strftime("%Y%m%d"))
         else:
             # 'Truly' random sampling
             seed = None
 
         task = {}
```

### Comparing `deepsensor-0.1.4/deepsensor/data/processor.py` & `deepsensor-0.1.5/deepsensor/data/processor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-import numpy
 import numpy as np
-import xarray
 
 import xarray as xr
 import pandas as pd
 
 import pprint
 
 from copy import deepcopy
@@ -47,14 +45,18 @@
 
         self.norm_params = norm_params
 
         if "coords" not in self.norm_params:
             # Add coordinate normalisation info to norm_params
             self.set_coord_params(time_name, x1_name, x1_map, x2_name, x2_map)
 
+        self.raw_spatial_coord_names = [
+            self.norm_params["coords"][coord]["name"] for coord in ["x1", "x2"]
+        ]
+
         self.deepcopy = deepcopy
         self.verbose = verbose
 
         self.valid_methods = ["mean_std", "min_max"]
 
     def _validate_maps(self, x1_map, x2_map):
         """Ensure the maps are valid and of appropriate types."""
@@ -291,62 +293,72 @@
         if isinstance(data, (pd.DataFrame, pd.Series)):
             # Set index back to original
             [indexes.remove(old_coord_ID) for old_coord_ID in old_coord_IDs]
             indexes = new_coord_IDs + indexes  # Put dims first
             data = data.set_index(indexes)
         return data
 
+    def map_array(
+        self,
+        data: Union[xr.DataArray, xr.Dataset, pd.DataFrame, pd.Series, np.ndarray],
+        var_ID: str,
+        method: str = "mean_std",
+        unnorm: bool = False,
+        add_offset=True,
+    ):
+        """Normalise or unnormalise the data values in an xarray, pandas, or numpy object"""
+        param1, param2 = self.get_norm_params(var_ID, data, method, unnorm)
+        if method == "mean_std":
+            if not unnorm:
+                scale = 1 / param2
+                offset = -param1 / param2
+            else:
+                scale = param2
+                offset = param1
+        elif method == "min_max":
+            if not unnorm:
+                scale = 2 / (param2 - param1)
+                offset = -(param2 + param1) / (param2 - param1)
+            else:
+                scale = (param2 - param1) / 2
+                offset = (param2 + param1) / 2
+        else:
+            raise ValueError(
+                f"Method {method} not recognised. Use 'mean_std' or 'min_max'."
+            )
+        data = data * scale
+        if add_offset:
+            data = data + offset
+        return data
+
     def map(
         self,
         data: Union[xr.DataArray, xr.Dataset, pd.DataFrame, pd.Series],
         method: str = "mean_std",
         add_offset: bool = True,
         unnorm: bool = False,
     ):
-        """Normalise or unnormalise data"""
+        """Normalise or unnormalise the data values and coords in an xarray or pandas object"""
         if self.deepcopy:
             data = deepcopy(data)
 
-        def mapper(data, param1, param2, method):
-            if method == "mean_std":
-                if not unnorm:
-                    scale = 1 / param2
-                    offset = -param1 / param2
-                else:
-                    scale = param2
-                    offset = param1
-            elif method == "min_max":
-                if not unnorm:
-                    scale = 2 / (param2 - param1)
-                    offset = -(param2 + param1) / (param2 - param1)
-                else:
-                    scale = (param2 - param1) / 2
-                    offset = (param2 + param1) / 2
-            data = data * scale
-            if add_offset:
-                data = data + offset
-            return data
-
         if isinstance(data, (xr.DataArray, xr.Dataset)) and not unnorm:
             self._validate_xr(data)
         elif isinstance(data, (pd.DataFrame, pd.Series)) and not unnorm:
             self._validate_pandas(data)
 
         if isinstance(data, (xr.DataArray, pd.Series)):
             # Single var
-            var_ID = data.name
-            param1, param2 = self.get_norm_params(var_ID, data, method, unnorm)
-            data = mapper(data, param1, param2, method)
+            data = self.map_array(data, data.name, method, unnorm, add_offset)
         elif isinstance(data, (xr.Dataset, pd.DataFrame)):
             # Multiple vars
             for var_ID in data:
-                param1, param2 = self.get_norm_params(
-                    var_ID, data[var_ID], method, unnorm
+                data[var_ID] = self.map_array(
+                    data[var_ID], var_ID, method, unnorm, add_offset
                 )
-                data[var_ID] = mapper(data[var_ID], param1, param2, method)
 
         data = self.map_coords(data, unnorm=unnorm)
 
         return data
 
     def __call__(
         self,
@@ -402,7 +414,25 @@
         {"x1": xr.DataArray(coord_arr[0]), "x2": xr.DataArray(coord_arr[1])},
         method="nearest",
         kwargs=dict(fill_value=None, bounds_error=False),
     ).data.astype(
         bool
     )  # Shape `coord_arr.shape[1]`, False if point is outside mask
     return coord_arr[:, mask_da]
+
+
+def da1_da2_same_grid(da1: xr.DataArray, da2: xr.DataArray) -> bool:
+    """Check if da1 and da2 are on the same grid
+
+    Note: da1 and da2 are assumed normalised by DataProcessor.
+    """
+    x1equal = np.array_equal(da1["x1"].values, da2["x1"].values)
+    x2equal = np.array_equal(da1["x2"].values, da2["x2"].values)
+    return x1equal and x2equal
+
+
+def interp_da1_to_da2(da1: xr.DataArray, da2: xr.DataArray) -> xr.DataArray:
+    """Interpolate da1 to da2
+
+    Note: da1 and da2 are assumed normalised by DataProcessor.
+    """
+    return da1.interp(x1=da2["x1"], x2=da2["x2"], method="nearest")
```

### Comparing `deepsensor-0.1.4/deepsensor/data/task.py` & `deepsensor-0.1.5/deepsensor/data/task.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import deepsensor
 
+from typing import Union, Tuple
 import numpy as np
 import lab as B
 import plum
 import copy
 
 from deepsensor.errors import TaskSetIndexError, GriddedDataError
 
@@ -13,15 +14,16 @@
 
     Inherits from `dict` and adds methods for printing and modifying the data.
     """
 
     def __init__(self, task_dict: dict) -> None:
         """Initialise a Task object.
 
-        :param task_dict: Dictionary containing the task information.
+        Args:
+            task_dict (dict): Dictionary containing the task.
         """
         super().__init__(task_dict)
 
     @classmethod
     def summarise_str(cls, k, v):
         if plum.isinstance(v, B.Numeric):
             return v.shape
@@ -147,7 +149,37 @@
 
     # Append proxy observations
     task_with_new["Y_c"][context_set_idx] = np.concatenate(
         [task["Y_c"][context_set_idx], Y_new], axis=-1
     )
 
     return task_with_new
+
+
+def flatten_X(X: Union[np.ndarray, Tuple[np.ndarray, np.ndarray]]) -> np.ndarray:
+    """Convert tuple of gridded coords to (2, N) array if necessary"""
+    if type(X) is tuple:
+        X1, X2 = np.meshgrid(X[0], X[1], indexing="ij")
+        X = np.stack([X1.ravel(), X2.ravel()], axis=0)
+    return X
+
+
+def flatten_Y(Y: Union[np.ndarray, Tuple[np.ndarray, np.ndarray]]) -> np.ndarray:
+    """Convert gridded data of shape (N_dim, N_x1, N_x2) to (N_dim, N_x1 * N_x2) array if necessary"""
+    if Y.ndim == 3:
+        Y = Y.reshape(*Y.shape[:-2], -1)
+    return Y
+
+
+def flatten_gridded_data_in_task(task: Task) -> Task:
+    """Convert any gridded data in `Task` to flattened arrays
+
+    Necessary for AR sampling, which doesn't yet permit gridded context sets
+    """
+    task_flattened = copy.deepcopy(task)
+
+    task_flattened["X_c"] = [flatten_X(X) for X in task["X_c"]]
+    task_flattened["Y_c"] = [flatten_Y(Y) for Y in task["Y_c"]]
+    task_flattened["X_t"] = [flatten_X(X) for X in task["X_t"]]
+    task_flattened["Y_t"] = [flatten_Y(Y) for Y in task["Y_t"]]
+
+    return task_flattened
```

### Comparing `deepsensor-0.1.4/deepsensor/data/utils.py` & `deepsensor-0.1.5/deepsensor/data/utils.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.4/deepsensor/model/convnp.py` & `deepsensor-0.1.5/deepsensor/model/convnp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 import copy
+import warnings
 from typing import Union, List
 
 import lab as B
 import numpy as np
 from matrix import Diagonal
 from plum import ModuleType, dispatch
 
 from deepsensor import backend
 from deepsensor.data.loader import TaskLoader
 from deepsensor.data.processor import DataProcessor
-from deepsensor.data.task import Task
+from deepsensor.data.task import (
+    Task,
+    flatten_gridded_data_in_task,
+    flatten_X,
+    flatten_Y,
+)
 from deepsensor.model.defaults import gen_ppu, gen_encoder_scales, gen_decoder_scale
 from deepsensor.model.model import DeepSensorModel
 from deepsensor.model.nps import (
     construct_neural_process,
-    run_nps_model,
     convert_task_to_nps_args,
+    run_nps_model,
+    run_nps_model_ar,
 )
 
 TFModel = ModuleType("tensorflow.keras", "Model")
 TorchModel = ModuleType("torch.nn", "Module")
 
 
 class ConvNP(DeepSensorModel):
@@ -167,19 +174,21 @@
         """Cast numpy arrays to TensorFlow or PyTorch tensors, add batch dim, and mask NaNs"""
 
         def array_modify_fn(arr):
             arr = arr[np.newaxis, ...]  # Add batch dim
 
             arr = arr.astype(np.float32)  # Cast to float32
 
-            # Find NaNs and keep size-1 variable dim
-            mask = np.any(np.isnan(arr), axis=1, keepdims=True)
+            # Find NaNs
+            mask = np.isnan(arr)
             if np.any(mask):
                 # Set NaNs to zero - necessary for `neuralprocesses` (can't have NaNs)
                 arr[mask] = 0.0
+                # Mask array (True for observed, False for missing) - keep size 1 variable dim
+                mask = ~np.any(mask, axis=1, keepdims=True)
 
             # Convert to tensor object based on deep learning backend
             arr = backend.convert_to_tensor(arr)
 
             # Convert to `nps.Masked` object if there are NaNs
             if B.any(mask):
                 arr = backend.nps.Masked(arr, B.cast(B.dtype(arr), mask))
@@ -340,15 +349,25 @@
         num_lv_samples: If latent variable model, number of lv samples for evaluating the loss
         normalise
 
         Returns
         -------
 
         """
+        # Remove NaNs from the target data if present
+        task, nans_present = remove_nans_from_task_Y_t_if_present(task)
+        # if nans_present:
+        #     TODO raise error like:
+        #     warnings.warn(
+        #         "NaNs present in the target data. These will be removed before evaluating the loss.",
+        #
+        #     )
+
         task = ConvNP.check_task(task)
+
         context_data, xt, yt, model_kwargs = convert_task_to_nps_args(task)
 
         logpdfs = backend.nps.loglik(
             self.model,
             context_data,
             xt,
             yt,
@@ -359,72 +378,93 @@
         )
 
         loss = -B.mean(logpdfs)
 
         return loss
 
     def ar_sample(
-        self, task: Task, n_samples=1, X_target_AR=None, ar_subsample_factor=1
+        self,
+        task: Task,
+        n_samples=1,
+        X_target_AR=None,
+        ar_subsample_factor=1,
+        fill_type="mean",
     ):
-        """AR sampling with optional functionality to only draw AR samples over a subset of the
-        target set and then infull the rest of the sample with the model mean conditioned on the
-        AR samples."""
+        """Autoregressive sampling from the model.
+
+        AR sampling with optional functionality to only draw AR samples over a subset of the
+        target set and then infill the rest of the sample with the model mean or joint sample
+        conditioned on the AR samples.
+
+        NOTE:
+            - AR sampling only works for 0th context/target set
+        """
+
+        # AR sampling requires gridded data to be flattened, not coordinate tuples
+        task_arsample = copy.deepcopy(task)
+        task = copy.deepcopy(task)
+
         if X_target_AR is not None:
             # User has specified a set of locations to draw AR samples over
-            task_arsample = copy.deepcopy(task)
             task_arsample["X_t"][0] = X_target_AR
         elif ar_subsample_factor > 1:
             # Subsample target locations to draw AR samples over
-            task_arsample = copy.deepcopy(task)
             xt = task["X_t"][0]
-            ndim_2d = np.sqrt(xt.shape[-1])
-            if int(ndim_2d) == ndim_2d:
-                # Targets on a square: subsample targets for AR along both spatial dimension
-                xt_2d = xt.reshape(-1, int(ndim_2d), int(ndim_2d))
-                xt = xt_2d[..., ::ar_subsample_factor, ::ar_subsample_factor].reshape(
-                    2, -1
+            if isinstance(xt, tuple):
+                # Targets on a grid: subsample targets for AR along spatial dimension
+                xt = (
+                    xt[0][..., ::ar_subsample_factor],
+                    xt[1][..., ::ar_subsample_factor],
                 )
             else:
                 xt = xt[..., ::ar_subsample_factor]
             task_arsample["X_t"][0] = xt
         else:
             task_arsample = copy.deepcopy(task)
 
+        task = flatten_gridded_data_in_task(task)
+        task_arsample = flatten_gridded_data_in_task(task_arsample)
+
         task_arsample = ConvNP.check_task(task_arsample)
         task = ConvNP.check_task(task)
 
-        mean, variance, noiseless_samples, noisy_samples = run_nps_model_ar(
-            self.model, task_arsample, num_samples=n_samples
-        )
+        if backend.str == "torch":
+            import torch
+
+            # Run AR sampling with torch.no_grad() to avoid prohibitive backprop computation for AR
+            with torch.no_grad():
+                mean, variance, noiseless_samples, noisy_samples = run_nps_model_ar(
+                    self.model, task_arsample, num_samples=n_samples
+                )
+        else:
+            mean, variance, noiseless_samples, noisy_samples = run_nps_model_ar(
+                self.model, task_arsample, num_samples=n_samples
+            )
 
         # Slice out first (and assumed only) target entry in nps.Aggregate object
-        noiseless_samples = B.to_numpy(noiseless_samples)[0]
+        noiseless_samples = B.to_numpy(noiseless_samples)
 
         if ar_subsample_factor > 1 or X_target_AR is not None:
             # AR sample locations not equal to target locations - infill the rest of the
             # sample with the model mean conditioned on the AR samples
             full_samples = []
             for sample in noiseless_samples:
                 task_with_sample = copy.deepcopy(task)
-                task_with_sample["X_c"][0] = np.concatenate(
-                    [task["X_c"][0], task_arsample["X_t"][0]], axis=-1
-                )
-                task_with_sample["Y_c"][0] = np.concatenate(
-                    [task["Y_c"][0], sample], axis=-1
+                task_with_sample["X_c"][0] = B.concat(
+                    task["X_c"][0], task_arsample["X_t"][0], axis=-1
                 )
+                task_with_sample["Y_c"][0] = B.concat(task["Y_c"][0], sample, axis=-1)
 
-                if type(self) is ConvCNP:
-                    # Independent predictions for each target location - just compute the mean
-                    # conditioned on the AR samples
+                if fill_type == "mean":
+                    # Compute the mean conditioned on the AR samples
                     pred = self.mean(
                         task_with_sample
                     )  # Should this be a `.sample` call?
-                else:
+                elif fill_type == "sample":
                     # Sample from joint distribution over all target locations
-                    # NOTE Risky to assume all model classes other than `ConvCNP` model correlations.
                     pred = self.sample(task_with_sample, n_samples=1)
 
                 full_samples.append(pred)
             full_samples = np.stack(full_samples, axis=0)
 
             return full_samples
         else:
@@ -509,7 +549,39 @@
     # merged_task["Y_t"] = backend.nps.Aggregate(*yts)
 
     merged_task["time"] = [t["time"] for t in tasks]
 
     merged_task = Task(merged_task)
 
     return merged_task
+
+
+def remove_nans_from_task_Y_t_if_present(task):
+    """If NaNs are present in task["Y_t"], remove them (and corresponding task["X_t"])"""
+    Y_t_nans_list = []
+    # First check whether there are any NaNs that we need to remove
+    nans_present = False
+    for Y_t_nans in Y_t_nans_list:
+        if B.any(Y_t_nans):
+            nans_present = True
+
+    if nans_present:
+        for i, (X, Y) in enumerate(zip(task["X_t"], task["Y_t"])):
+            Y = flatten_Y(Y)
+            Y_t_nans = B.any(B.isnan(Y), axis=0)  # shape (n_targets,)
+            Y_t_nans_list.append(Y_t_nans)
+
+    if not nans_present:
+        return task, False
+
+    # NaNs present in task - make deep copy and remove NaNs
+    task = copy.deepcopy(task)
+    for i, (X, Y, Y_t_nans) in enumerate(zip(task["X_t"], task["Y_t"], Y_t_nans_list)):
+        if B.any(Y_t_nans):
+            if isinstance(X, tuple):
+                # Gridded data
+                X = flatten_X(X)
+                Y = flatten_Y(Y)
+            task["X_t"][i] = X[:, ~Y_t_nans]
+            task["Y_t"][i] = Y[:, ~Y_t_nans]
+
+    return task, True
```

### Comparing `deepsensor-0.1.4/deepsensor/model/defaults.py` & `deepsensor-0.1.5/deepsensor/model/defaults.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.4/deepsensor/model/model.py` & `deepsensor-0.1.5/deepsensor/model/model.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from deepsensor.data.loader import TaskLoader
 from deepsensor.data.processor import DataProcessor
 from deepsensor.data.task import Task
 
 from typing import List, Union
+import copy
 
 import time
 from tqdm import tqdm
 
 import numpy as np
 import pandas as pd
 import xarray as xr
@@ -31,32 +32,42 @@
     if prepend_coords is None:
         prepend_coords = {}
 
     # Check for any repeated data_vars
     if len(data_vars) != len(set(data_vars)):
         raise ValueError(
             f"Duplicate data_vars found in data_vars: {data_vars}. "
-            "This woudld cause the xarray.Dataset to have fewer variables than expected."
+            "This would cause the xarray.Dataset to have fewer variables than expected."
         )
 
     x1_raw = X.coords[coord_names["x1"]]
     x2_raw = X.coords[coord_names["x2"]]
 
-    x1_predict = np.linspace(
-        x1_raw[0],
-        x1_raw[-1],
-        int(x1_raw.size * resolution_factor),
-        dtype="float32",
-    )
-    x2_predict = np.linspace(
-        x2_raw[0],
-        x2_raw[-1],
-        int(x2_raw.size * resolution_factor),
-        dtype="float32",
-    )
+    # Assert uniform spacing
+    if not np.allclose(np.diff(x1_raw), np.diff(x1_raw)[0]):
+        raise ValueError(f"Coordinate {coord_names['x1']} must be uniformly spaced.")
+    if not np.allclose(np.diff(x2_raw), np.diff(x2_raw)[0]):
+        raise ValueError(f"Coordinate {coord_names['x2']} must be uniformly spaced.")
+
+    if resolution_factor == 1.0:
+        x1_predict = x1_raw
+        x2_predict = x2_raw
+    else:
+        x1_predict = np.linspace(
+            x1_raw[0],
+            x1_raw[-1],
+            int(x1_raw.size * resolution_factor),
+            dtype="float32",
+        )
+        x2_predict = np.linspace(
+            x2_raw[0],
+            x2_raw[-1],
+            int(x2_raw.size * resolution_factor),
+            dtype="float32",
+        )
 
     if len(prepend_dims) != len(set(prepend_dims)):
         # TODO unit test
         raise ValueError(
             f"Length of prepend_dims ({len(prepend_dims)}) must be equal to length of "
             f"prepend_coords ({len(prepend_coords)})."
         )
@@ -176,100 +187,171 @@
         """
         self.task_loader = task_loader
         self.data_processor = data_processor
 
     def predict(
         self,
         tasks: Union[List[Task], Task],
-        X_t: Union[xr.Dataset, xr.DataArray, pd.DataFrame, pd.Series, pd.Index],
-        X_t_normalised: bool = False,
+        X_t: Union[
+            xr.Dataset, xr.DataArray, pd.DataFrame, pd.Series, pd.Index, np.ndarray
+        ],
+        X_t_is_normalised: bool = False,
         resolution_factor=1,
         n_samples=0,
+        ar_sample=False,
+        ar_subsample_factor=1,
         unnormalise=True,
         seed=0,
+        append_indexes: dict = None,
         progress_bar=0,
         verbose=False,
     ):
         """Predict on a regular grid or at off-grid locations.
 
         TODO:
         - Test with multiple targets model
 
-        :param tasks: List of tasks containing context data.
-        :param X_t: Target locations to predict at. Can be an xarray object containing
-            on-grid locations or a pandas object containing off-grid locations.
-        :param X_t_normalised: Whether the `X_t` coords are normalised.
-            If False, will normalise the coords before passing to model. Default False.
-        :param resolution_factor: Optional factor to increase the resolution of the
-            target grid by. E.g. 2 will double the target resolution, 0.5 will halve it.
-            Applies to on-grid predictions only. Default 1.
-        :param n_samples: Number of joint samples to draw from the model.
-            If 0, will not draw samples. Default 0.
-        :param unnormalise: Whether to unnormalise the predictions. Only works if
-            `self` has a `data_processor` and `task_loader` attribute. Default True.
-        :param seed: Random seed for deterministic sampling. Default 0.
-        :param progress_bar: Whether to display a progress bar over tasks. Default 0.
-        :param verbose: Whether to print time taken for prediction. Default False.
+        Args:
+            tasks: List of tasks containing context data.
+            X_t: Target locations to predict at. Can be an xarray object containing
+                on-grid locations or a pandas object containing off-grid locations.
+            X_t_is_normalised: Whether the `X_t` coords are normalised.
+                If False, will normalise the coords before passing to model. Default False.
+            resolution_factor: Optional factor to increase the resolution of the
+                target grid by. E.g. 2 will double the target resolution, 0.5 will halve it.
+                Applies to on-grid predictions only. Default 1.
+            n_samples: Number of joint samples to draw from the model.
+                If 0, will not draw samples. Default 0.
+            ar_sample: Whether to use autoregressive sampling. Default False.
+            unnormalise: Whether to unnormalise the predictions. Only works if
+                `self` has a `data_processor` and `task_loader` attribute. Default True.
+            seed: Random seed for deterministic sampling. Default 0.
+            append_indexes: Dictionary of index metadata to append to pandas indexes
+                in the off-grid case. Default None.
+            progress_bar: Whether to display a progress bar over tasks. Default 0.
+            verbose: Whether to print time taken for prediction. Default False.
 
         Returns:
             - If X_t is a pandas object, returns pandas objects containing off-grid predictions.
             - If X_t is an xarray object, returns xarray object containing on-grid predictions.
             - If n_samples == 0, returns only mean and std predictions.
             - If n_samples > 0, returns mean, std and samples predictions.
         """
         tic = time.time()
 
+        if not isinstance(X_t, (xr.DataArray, xr.Dataset)):
+            if resolution_factor != 1:
+                raise ValueError(
+                    "resolution_factor can only be used with on-grid predictions."
+                )
+            if ar_subsample_factor != 1:
+                raise ValueError(
+                    "ar_subsample_factor can only be used with on-grid predictions."
+                )
+        if not isinstance(X_t, (pd.DataFrame, pd.Series, pd.Index, np.ndarray)):
+            if append_indexes is not None:
+                raise ValueError(
+                    "append_indexes can only be used with off-grid predictions."
+                )
+
+        if isinstance(X_t, (xr.DataArray, xr.Dataset)):
+            mode = "on-grid"
+        elif isinstance(X_t, (pd.DataFrame, pd.Series, pd.Index, np.ndarray)):
+            mode = "off-grid"
+        else:
+            raise ValueError(
+                f"X_t must be and xarray, pandas or numpy object. Got {type(X_t)}."
+            )
+
         if type(tasks) is Task:
             tasks = [tasks]
 
         if n_samples >= 1:
             B.set_random_seed(seed)
             np.random.seed(seed)
 
         dates = [task["time"] for task in tasks]
 
         # Flatten tuple of tups to single list
         target_var_IDs = [
             var_ID for set in self.task_loader.target_var_IDs for var_ID in set
         ]
 
+        # Pre-process X_t if necessary
         if isinstance(X_t, pd.Index):
             X_t = pd.DataFrame(index=X_t)
+        elif isinstance(X_t, np.ndarray):
+            # Convert to empty dataframe with normalised or unnormalised coord names
+            if X_t_is_normalised:
+                index_names = ["x1", "x2"]
+            else:
+                index_names = self.data_processor.raw_spatial_coord_names
+            X_t = pd.DataFrame(X_t.T, columns=index_names)
+            X_t = X_t.set_index(index_names)
+        if mode == "off-grid" and append_indexes is not None:
+            # Check append_indexes are all same length as X_t
+            if append_indexes is not None:
+                for idx, vals in append_indexes.items():
+                    if len(vals) != len(X_t):
+                        raise ValueError(
+                            f"append_indexes[{idx}] must be same length as X_t, got {len(vals)} and {len(X_t)} respectively."
+                        )
+            X_t = X_t.reset_index()
+            X_t = pd.concat([X_t, pd.DataFrame(append_indexes)], axis=1)
+            X_t = X_t.set_index(list(X_t.columns))
 
-        if not X_t_normalised:
-            X_t = self.data_processor.map_coords(X_t)  # Normalise
+        if X_t_is_normalised:
+            X_t_normalised = X_t
 
-        if isinstance(X_t, (xr.DataArray, xr.Dataset)):
-            mode = "on-grid"
-        elif isinstance(X_t, (pd.DataFrame, pd.Series, pd.Index)):
-            mode = "off-grid"
+            # Unnormalise coords to use for xarray/pandas objects for storing predictions
+            X_t = self.data_processor.map_coords(X_t, unnorm=True)
         else:
-            raise ValueError(
-                f"X_t must be an xarray object or a pandas object, not {type(X_t)}"
-            )
+            # Normalise coords to use for model
+            X_t_normalised = self.data_processor.map_coords(X_t)
+
+        if mode == "on-grid":
+            X_t_arr = (X_t_normalised["x1"].values, X_t_normalised["x2"].values)
+        elif mode == "off-grid":
+            X_t_arr = X_t_normalised.reset_index()[["x1", "x2"]].values.T
+
+        if not unnormalise:
+            X_t = X_t_normalised
+            coord_names = {"x1": "x1", "x2": "x2"}
+        elif unnormalise:
+            coord_names = {
+                "x1": self.data_processor.raw_spatial_coord_names[0],
+                "x2": self.data_processor.raw_spatial_coord_names[1],
+            }
 
+        # Create empty xarray/pandas objects to store predictions
         if mode == "on-grid":
             mean = create_empty_spatiotemporal_xarray(
-                X_t, dates, resolution_factor, data_vars=target_var_IDs
+                X_t,
+                dates,
+                resolution_factor,
+                data_vars=target_var_IDs,
+                coord_names=coord_names,
             ).to_array(dim="data_var")
             std = create_empty_spatiotemporal_xarray(
-                X_t, dates, resolution_factor, data_vars=target_var_IDs
+                X_t,
+                dates,
+                resolution_factor,
+                data_vars=target_var_IDs,
+                coord_names=coord_names,
             ).to_array(dim="data_var")
             if n_samples >= 1:
                 samples = create_empty_spatiotemporal_xarray(
                     X_t,
                     dates,
                     resolution_factor,
                     data_vars=target_var_IDs,
+                    coord_names=coord_names,
                     prepend_dims=["sample"],
                     prepend_coords={"sample": np.arange(n_samples)},
                 ).to_array(dim="data_var")
-
-            X_t_arr = (mean["x1"].values, mean["x2"].values)
-
         elif mode == "off-grid":
             # Repeat target locs for each date to create multiindex
             idxs = [(date, *idxs) for date in dates for idxs in X_t.index]
             index = pd.MultiIndex.from_tuples(idxs, names=["time", *X_t.index.names])
             mean = pd.DataFrame(index=index, columns=target_var_IDs)
             std = pd.DataFrame(index=index, columns=target_var_IDs)
             if n_samples >= 1:
@@ -280,40 +362,85 @@
                     for idxs in X_t.index
                 ]
                 index_samples = pd.MultiIndex.from_tuples(
                     idxs_samples, names=["sample", "time", *X_t.index.names]
                 )
                 samples = pd.DataFrame(index=index_samples, columns=target_var_IDs)
 
-            X_t_arr = X_t.reset_index()[["x1", "x2"]].values.T
+        def unnormalise_pred_array(arr, **kwargs):
+            var_IDs_flattened = [
+                var_ID
+                for var_IDs in self.task_loader.target_var_IDs
+                for var_ID in var_IDs
+            ]
+            assert arr.shape[0] == len(var_IDs_flattened)
+            for i, var_ID in enumerate(var_IDs_flattened):
+                arr[i] = self.data_processor.map_array(
+                    arr[i], var_ID, method="mean_std", unnorm=True, **kwargs
+                )
+            return arr
+
+        # Don't change tasks by reference when overriding target locations
+        tasks = copy.deepcopy(tasks)
 
         for task in tqdm(tasks, position=0, disable=progress_bar < 1, leave=True):
-            # TODO - repeat based on number of targets?
-            task["X_t"] = [X_t_arr]
+            task["X_t"] = [X_t_arr for _ in range(len(task["X_t"]))]
 
             # If `DeepSensor` model child has been sub-classed with a `__call__` method,
             # we assume this is a distribution-like object that can be used to compute
             # mean, std and samples. Otherwise, run the model with `Task` for each prediction type.
             if hasattr(self, "__call__"):
                 # Run model forwards once to generate output distribution, which we re-use
                 dist = self(task, n_samples=n_samples)
                 mean_arr = self.mean(dist)
                 std_arr = self.stddev(dist)
                 if n_samples >= 1:
                     B.set_random_seed(seed)
                     np.random.seed(seed)
-                    samples_arr = self.sample(dist, n_samples=n_samples)
+                    if ar_sample:
+                        samples_arr = self.ar_sample(
+                            task,
+                            n_samples=n_samples,
+                            ar_subsample_factor=ar_subsample_factor,
+                        )
+                        samples_arr = samples_arr.reshape((n_samples, *mean_arr.shape))
+                    else:
+                        samples_arr = self.sample(dist, n_samples=n_samples)
             else:
                 # Re-run model for each prediction type
                 mean_arr = self.mean(task)
                 std_arr = self.stddev(task)
                 if n_samples >= 1:
                     B.set_random_seed(seed)
                     np.random.seed(seed)
-                    samples_arr = self.sample(task, n_samples=n_samples)
+                    if ar_sample:
+                        samples_arr = self.ar_sample(
+                            task,
+                            n_samples=n_samples,
+                            ar_subsample_factor=ar_subsample_factor,
+                        )
+                        samples_arr = samples_arr.reshape((n_samples, *mean_arr.shape))
+                    else:
+                        samples_arr = self.sample(task, n_samples=n_samples)
+
+            # Concatenate multi-target predictions
+            if isinstance(mean_arr, (list, tuple)):
+                mean_arr = np.concatenate(mean_arr, axis=0)
+                std_arr = np.concatenate(std_arr, axis=0)
+                if n_samples >= 1:
+                    samples_arr = np.concatenate(samples_arr, axis=0)
+
+            if unnormalise:
+                mean_arr = unnormalise_pred_array(mean_arr)
+                std_arr = unnormalise_pred_array(std_arr, add_offset=False)
+                if n_samples >= 1:
+                    for sample_i in range(n_samples):
+                        samples_arr[sample_i] = unnormalise_pred_array(
+                            samples_arr[sample_i]
+                        )
 
             if mode == "on-grid":
                 mean.loc[:, task["time"], :, :] = mean_arr
                 std.loc[:, task["time"], :, :] = std_arr
                 if n_samples >= 1:
                     for sample_i in range(n_samples):
                         samples.loc[:, sample_i, task["time"], :, :] = samples_arr[
@@ -329,24 +456,14 @@
 
         if mode == "on-grid":
             mean = mean.to_dataset(dim="data_var")
             std = std.to_dataset(dim="data_var")
             if n_samples >= 1:
                 samples = samples.to_dataset(dim="data_var")
 
-        if (
-            self.task_loader is not None
-            and self.data_processor is not None
-            and unnormalise == True
-        ):
-            mean = self.data_processor.unnormalise(mean)
-            std = self.data_processor.unnormalise(std, add_offset=False)
-            if n_samples >= 1:
-                samples = self.data_processor.unnormalise(samples)
-
         if verbose:
             dur = time.time() - tic
             print(f"Done in {np.floor(dur / 60)}m:{dur % 60:.0f}s.\n")
 
         if n_samples >= 1:
             return mean, std, samples
         else:
```

### Comparing `deepsensor-0.1.4/deepsensor/model/nps.py` & `deepsensor-0.1.5/deepsensor/model/nps.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,69 +8,69 @@
     """Infer & build model call signature from `task` dict
 
     TODO move to ConvNP class?
     """
 
     context_data = list(zip(task["X_c"], task["Y_c"]))
 
-    # context_data = [nps.mask.merge_contexts(ctx, multiple=5000) for ctx in context_data]
-    # context_data[0] = nps.mask.merge_contexts(context_data[0], multiple=5000)  # TEMP not converting gridded
-
-    # TEMP: assume target sets all on same spatial locations
-    #   just use the first entry from the lists of target data
-    # xt = task["X_t"][0]
-    # yt = B.concat(*task["Y_t"], axis=1)
-
     if len(task["X_t"]) == 1 and len(task["Y_t"]) == 1:
         # Single target set
         xt = task["X_t"][0]
         yt = task["Y_t"][0]
     elif len(task["X_t"]) > 1 and len(task["Y_t"]) > 1:
         # Multiple target sets, different target locations
         xt = backend.nps.AggregateInput(*[(xt, i) for i, xt in enumerate(task["X_t"])])
-        yt = backend.nps.Aggregate(*[yt for yt in enumerate(task["Y_t"])])
+        yt = backend.nps.Aggregate(*task["Y_t"])
     elif len(task["X_t"]) == 1 and len(task["Y_t"]) > 1:
         # Multiple target sets, same target locations
         xt = task["X_t"][0]
         yt = B.concat(*task["Y_t"], axis=1)
     else:
         raise ValueError(
             f"Incorrect target locations and target observations (got {len(task['X_t'])} and {len(task['Y_t'])})"
         )
 
-    # Assume one target set, convert to tf.Tensor and AggregateInput for AR
-    #   sampling
-    # xt = tf.cast(tf.convert_to_tensor(xt), tf.float32)
-    # xt = nps.aggregate.AggregateInput(
-    #     (xt, 0),
-    # )
-
     model_kwargs = {}
     if "Y_target_auxiliary" in task.keys():
         model_kwargs["aux_t"] = task["Y_target_auxiliary"]
 
     return context_data, xt, yt, model_kwargs
 
 
 def run_nps_model(neural_process, task, n_samples=None, requires_grad=False):
     """Run `neuralprocesses` model"""
-    context_data, xt, yt, model_kwargs = convert_task_to_nps_args(task)
+    context_data, xt, _, model_kwargs = convert_task_to_nps_args(task)
     if backend.str == "torch" and not requires_grad:
         # turn off grad
         import torch
 
         with torch.no_grad():
             dist = neural_process(
                 context_data, xt, **model_kwargs, num_samples=n_samples
             )
     else:
         dist = neural_process(context_data, xt, **model_kwargs, num_samples=n_samples)
     return dist
 
 
+def run_nps_model_ar(neural_process, task, num_samples=1):
+    """Run `neural_process` in AR mode"""
+    context_data, xt, _, _ = convert_task_to_nps_args(task)
+
+    # NOTE can't use `model_kwargs` in AR mode (ie can't use auxiliary MLP at targets)
+    mean, variance, noiseless_samples, noisy_samples = backend.nps.ar_predict(
+        neural_process,
+        context_data,
+        xt,
+        num_samples=num_samples,
+    )
+
+    return mean, variance, noiseless_samples, noisy_samples
+
+
 def construct_neural_process(
     dim_x=2,
     dim_yc=1,
     dim_yt=1,
     dim_aux_t=None,
     dim_lv=0,
     conv_arch="unet",
```

### Comparing `deepsensor-0.1.4/deepsensor/plot.py` & `deepsensor-0.1.5/deepsensor/plot.py`

 * *Files 12% similar despite different names*

```diff
@@ -349,48 +349,99 @@
     ax.scatter(*X_new_df.values.T[::-1], s=3**2, c="r", linewidths=0.5)
     offgrid_context(ax, task, data_processor, s=3**2, linewidths=0.5)
 
     return fig
 
 
 def acquisition_fn(
-    task, acquisition_fn_ds, X_new_df, data_processor, crs, cmap="Greys_r", figsize=3
+    task,
+    acquisition_fn_ds,
+    X_new_df,
+    data_processor,
+    crs,
+    col_dim="iteration",
+    cmap="Greys_r",
+    figsize=3,
+    add_colorbar=True,
+    max_ncol=5,
 ):
-    if "time" in acquisition_fn_ds.dims:
-        # Average over time
-        acquisition_fn_ds = acquisition_fn_ds.mean("time")
-    if "sample" in acquisition_fn_ds.dims:
-        # Average over samples
-        acquisition_fn_ds = acquisition_fn_ds.mean("sample")
+    # Remove spatial dims using data_processor.raw_spatial_coords_names
+    plot_dims = [col_dim, *data_processor.raw_spatial_coord_names]
+    non_plot_dims = [dim for dim in acquisition_fn_ds.dims if dim not in plot_dims]
+    valid_avg_dims = ["time", "sample"]
+    for dim in non_plot_dims:
+        if dim not in valid_avg_dims:
+            raise ValueError(
+                f"Cannot average over dim {dim} for plotting. Must be one of {valid_avg_dims}. "
+                f"Select a single value for {dim} using `acquisition_fn_ds.sel({dim}=...)`."
+            )
+    if len(non_plot_dims) > 0:
+        # Average over non-plot dims
+        print(f"Averaging acquisition function over dims for plotting: {non_plot_dims}")
+        acquisition_fn_ds = acquisition_fn_ds.mean(dim=non_plot_dims)
+
+    col_vals = acquisition_fn_ds[col_dim].values
+    if col_vals.size == 1:
+        n_col_vals = 1
+    else:
+        n_col_vals = len(col_vals)
+    ncols = np.min([max_ncol, n_col_vals])
+
+    if n_col_vals > ncols:
+        nrows = int(np.ceil(n_col_vals / ncols))
+    else:
+        nrows = 1
 
-    ncols = np.max(acquisition_fn_ds.iteration.values) + 1
     fig, axes = plt.subplots(
-        subplot_kw={"projection": crs}, ncols=ncols, figsize=(figsize * ncols, figsize)
+        subplot_kw={"projection": crs},
+        ncols=ncols,
+        nrows=nrows,
+        figsize=(figsize * ncols, figsize * nrows),
     )
-    min, max = acquisition_fn_ds.min(), acquisition_fn_ds.max()
-    for iteration in range(len(acquisition_fn_ds.iteration)):
-        ax = axes[iteration]
-        if iteration == np.max(acquisition_fn_ds.iteration):
-            add_colorbar = True
+    if nrows == 1 and ncols == 1:
+        axes = [axes]
+    else:
+        axes = axes.ravel()
+    if add_colorbar:
+        min, max = acquisition_fn_ds.min(), acquisition_fn_ds.max()
+    else:
+        # Use different colour scales for each plot
+        min, max = None, None
+    for i, col_val in enumerate(col_vals):
+        ax = axes[i]
+        if i == len(col_vals):
+            final_axis = True
         else:
-            add_colorbar = False
-        acquisition_fn_ds.sel(iteration=iteration).plot(
+            final_axis = False
+        acquisition_fn_ds.sel(**{col_dim: col_val}).plot(
             ax=ax, cmap=cmap, vmin=min, vmax=max, add_colorbar=False
         )
-        if add_colorbar:
+        if add_colorbar and final_axis:
             im = ax.get_children()[0]
             label = acquisition_fn_ds.name
             cax = plt.axes([0.93, 0.035, 0.02, 0.91])  # add a small custom axis
             cbar = plt.colorbar(
                 im, cax=cax, label=label
             )  # specify axis for colorbar to occupy with cax
-        ax.set_title(f"Iteration {iteration+1}")
+        ax.set_title(f"{col_dim}={col_val}")
         ax.coastlines()
+        if col_dim == "iteration":
+            X_new_df_plot = X_new_df.loc[slice(0, col_val)].values.T[::-1]
+        else:
+            # Assumed plotting single iteration
+            iter = acquisition_fn_ds.iteration.values
+            assert iter.size == 1, "Expected single iteration"
+            X_new_df_plot = X_new_df.loc[slice(0, iter.item())].values.T[::-1]
         ax.scatter(
-            *X_new_df.loc[slice(0, iteration)].values.T[::-1],
+            *X_new_df_plot,
             s=3**2,
             c="r",
             linewidths=0.5,
         )
+
     offgrid_context(axes, task, data_processor, s=3**2, linewidths=0.5)
 
+    # Remove any unused axes
+    for ax in axes[len(col_vals) :]:
+        ax.remove()
+
     return fig
```

### Comparing `deepsensor-0.1.4/deepsensor/tensorflow/__init__.py` & `deepsensor-0.1.5/deepsensor/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.4/deepsensor/torch/__init__.py` & `deepsensor-0.1.5/deepsensor/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.4/deepsensor/train/train.py` & `deepsensor-0.1.5/deepsensor/train/train.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.4/deepsensor.egg-info/PKG-INFO` & `deepsensor-0.1.5/deepsensor.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepsensor
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python package for modelling xarray and pandas data with neural processes.
 Home-page: https://github.com/tom-andersson/deepsensor
 Author: Tom R. Andersson
 Author-email: tomand@bas.ac.uk
 License: MIT
 Platform: unix
 Platform: linux
@@ -22,15 +22,15 @@
 
 
 <p style="text-align: center; font-size: 15px">A Python package and open-source project for modelling environmental
 data with neural processes</p>
 
 -----------
 
-[![release](https://img.shields.io/badge/release-v0.1.3-green?logo=github)](https://github.com/tom-andersson/deepsensor/releases)
+[![release](https://img.shields.io/badge/release-v0.1.5-green?logo=github)](https://github.com/tom-andersson/deepsensor/releases)
 ![Tests](https://github.com/tom-andersson/deepsensor/actions/workflows/tests.yml/badge.svg)
 [![Coverage Status](https://coveralls.io/repos/github/tom-andersson/deepsensor/badge.svg?branch=main)](https://coveralls.io/github/tom-andersson/deepsensor?branch=main)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 **NOTE**: This package is currently undergoing very active development. If you are interested in using
 DeepSensor, please get in touch first (tomand@bas.ac.uk).
 
@@ -66,25 +66,24 @@
 Simply `import deepsensor.torch` or `import deepsensor.tensorflow` to choose between them!
 
 Quick start
 ----------
 
 Here we will demonstrate a simple example of training a convolutional conditional neural process
 (ConvCNP) to spatially interpolate ERA5 data.
-First, pip install the package. In this case we will use the TensorFlow backend.
+First, pip install the package. In this case we will use the PyTorch backend.
 ```bash
 pip install deepsensor
-pip install tensorflow
-pip install tensorflow-probability
+pip install torch
 ```
 
-We can go from imports to predictions with a trained model in <30 lines of code!
+We can go from imports to predictions with a trained model in less than 30 lines of code!
 
 ```python
-import deepsensor.tensorflow
+import deepsensor.torch
 from deepsensor.data.loader import TaskLoader
 from deepsensor.data.processor import DataProcessor
 from deepsensor.model.convnp import ConvNP
 from deepsensor.train.train import train_epoch
 
 import xarray as xr
 import pandas as pd
@@ -102,23 +101,23 @@
 
 # Set up model
 model = ConvNP(data_processor, task_loader)
 
 # Generate training tasks with up to 10% of grid cells passed as context and all grid cells
 # passed as targets
 train_tasks = []
-for date in pd.date_range("2013-01-01", "2014-11-30"):
+for date in pd.date_range("2013-01-01", "2014-11-30")[::7]:
     task = task_loader(date, context_sampling=np.random.uniform(0.0, 0.1), target_sampling="all")
     train_tasks.append(task)
 
 # Train model
-for epoch in range(100):
+for epoch in range(10):
     train_epoch(model, train_tasks, progress_bar=True)
 
-# Predict on new task with 10% of context data
+# Predict on new task with 10% of context data and a dense grid of target points
 test_task = task_loader("2014-12-31", 0.1)
 mean_ds, std_ds = model.predict(test_task, X_t=ds_raw)
 ```
 
 After training, the model can predict directly to `xarray` in your data's original units and coordinate system:
 ```python
 >>> mean_ds
@@ -128,14 +127,36 @@
   * time     (time) datetime64[ns] 2014-12-31
   * lat      (lat) float32 75.0 72.5 70.0 67.5 65.0 ... 25.0 22.5 20.0 17.5 15.0
   * lon      (lon) float32 200.0 202.5 205.0 207.5 ... 322.5 325.0 327.5 330.0
 Data variables:
     air      (time, lat, lon) float32 246.7 244.4 245.5 ... 290.2 289.8 289.4
 ```
 
+We can also predict directly to `pandas` containing a timeseries of predictions at off-grid locations
+by passing a `numpy` array of target locations to the `X_t` argument of `.predict`:
+```python
+# Predict at two off-grid locations for three days in December 2014
+test_tasks = task_loader(pd.date_range("2014-12-01", "2014-12-31"), 0.1)
+mean_df, std_df = model.predict(test_tasks, X_t=np.array([[50, 280], [40, 250]]).T)
+```
+
+```python
+>>> mean_df
+                              air
+time       lat  lon              
+2014-12-01 50.0 280.0  260.183056
+           40.0 250.0  277.947373
+2014-12-02 50.0 280.0   261.08943
+           40.0 250.0  278.219599
+2014-12-03 50.0 280.0  257.128185
+           40.0 250.0  278.444229
+```
+
+This quickstart example is also available as a [Jupyter notebook](https://github.com/tom-andersson/deepsensor/blob/main/notebooks/quickstart_example.ipynb) with added visualisations.
+
 Extending DeepSensor with new models
 ----------
 To extend DeepSensor with a new model, simply create a new class that inherits from `deepsensor.model.DeepSensorModel`
 and implement the low-level prediction methods defined in `deepsensor.model.ProbabilisticModel`,
 such as `.mean` and `.stddev`.
 ```python
 class NewModel(DeepSensorModel):
```

### Comparing `deepsensor-0.1.4/deepsensor.egg-info/SOURCES.txt` & `deepsensor-0.1.5/deepsensor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.4/setup.cfg` & `deepsensor-0.1.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = deepsensor
-version = 0.1.4
+version = 0.1.5
 author = Tom R. Andersson
 author_email = tomand@bas.ac.uk
 description = A Python package for modelling xarray and pandas data with neural processes.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tom-andersson/deepsensor
 license = MIT
```

### Comparing `deepsensor-0.1.4/tests/test_data_processor.py` & `deepsensor-0.1.5/tests/test_data_processor.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.4/tests/test_model.py` & `deepsensor-0.1.5/tests/test_model.py`

 * *Files 20% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         # It's safe to share data between tests because the TaskLoader does not modify data
         self.da = _gen_data_xr()
         self.df = _gen_data_pandas()
 
         self.dp = DataProcessor()
-        _ = self.dp([self.da, self.df])  # Compute normalization parameters
+        _ = self.dp([self.da, self.df])  # Compute normalisation parameters
 
     def _gen_task_loader_call_args(self, n_context, n_target):
         """Generate arguments for TaskLoader.__call__
 
         Loops over all possible combinations of context/target sampling methods
         and returns a list of arguments for TaskLoader.__call__.
         Options tested include:
@@ -187,22 +187,65 @@
             # Scalars
             x = model.logpdf(task)
             assert x.size == 1 and x.shape == ()
             x = model.joint_entropy(task)
             assert x.size == 1 and x.shape == ()
             x = model.mean_marginal_entropy(task)
             assert x.size == 1 and x.shape == ()
-            if n_target_sets == 1:
-                # TEMP loss function for multiple non-overlapping target sets is not yet implemented
-                x = B.to_numpy(model.loss_fn(task))
+            x = B.to_numpy(model.loss_fn(task))
             assert x.size == 1 and x.shape == ()
 
     @parameterized.expand(range(1, 4))
+    def test_nans_offgrid_context(self, ndim):
+        """Test that `ConvNP` can handle NaNs in offgrid context"""
+
+        tl = TaskLoader(
+            context=_gen_data_xr(data_vars=range(ndim)),
+            target=self.da,
+        )
+
+        # All NaNs
+        task = tl("2020-01-01", context_sampling=10, target_sampling=10)
+        task["Y_c"][0][:, 0] = np.nan
+        model = ConvNP(self.dp, tl, unet_channels=(5, 5, 5), verbose=False)
+        _ = model(task)
+
+        # One NaN
+        task = tl("2020-01-01", context_sampling=10, target_sampling=10)
+        task["Y_c"][0][0, 0] = np.nan
+        model = ConvNP(self.dp, tl, unet_channels=(5, 5, 5), verbose=False)
+        _ = model(task)
+
+    @parameterized.expand(range(1, 4))
+    def test_nans_gridded_context(self, ndim):
+        """Test that `ConvNP` can handle NaNs in gridded context"""
+
+        tl = TaskLoader(
+            context=_gen_data_xr(data_vars=range(ndim)),
+            target=self.da,
+        )
+
+        # All NaNs
+        task = tl("2020-01-01", context_sampling="all", target_sampling=10)
+        task["Y_c"][0][:, 0, 0] = np.nan
+        model = ConvNP(self.dp, tl, unet_channels=(5, 5, 5), verbose=False)
+        _ = model(task)
+
+        # One NaN
+        task = tl("2020-01-01", context_sampling="all", target_sampling=10)
+        task["Y_c"][0][0, 0, 0] = np.nan
+        model = ConvNP(self.dp, tl, unet_channels=(5, 5, 5), verbose=False)
+        _ = model(task)
+
+    @parameterized.expand(range(1, 4))
     def test_prediction_shapes_highlevel(self, target_dim):
-        """Test high-level `.predict` interface over a range of number of target sets"""
+        """Test high-level `.predict` interface over a range of number of target sets
+
+        TODO: implement and test multiple target sets for pandas case
+        """
 
         if target_dim > 1:
             # Avoid data var name clash in `predict`
             target_names = [f"target_{i}" for i in range(target_dim)]
             target = [self.da] * target_dim
             for i, name in enumerate(target_names):
                 target[i] = copy.deepcopy(target[i])
@@ -221,15 +264,17 @@
 
         # Gridded predictions
         n_samples = 5
         mean_ds, std_ds, samples_ds = model.predict(
             tasks,
             X_t=self.da,
             n_samples=n_samples,
-            unnormalise=False if target_dim > 1 else True,
+            unnormalise=True
+            if target_dim == 1
+            else False,  # TODO fix unnormalising for multiple equally named targets
         )
         assert [isinstance(ds, xr.Dataset) for ds in [mean_ds, std_ds, samples_ds]]
         assert_shape(
             mean_ds.to_array(),
             (target_dim, len(dates), self.da.x1.size, self.da.x2.size),
         )
         assert_shape(
@@ -237,42 +282,118 @@
             (target_dim, len(dates), self.da.x1.size, self.da.x2.size),
         )
         assert_shape(
             samples_ds.to_array(),
             (target_dim, n_samples, len(dates), self.da.x1.size, self.da.x2.size),
         )
 
-        # Offgrid predictions
+        # Offgrid predictions: test pandas `X_t` and numpy `X_t`
         n_samples = 5
-        X_t = self.df.loc[dates[0]]
-        mean_df, std_df, samples_df = model.predict(
-            tasks,
-            X_t=X_t,
-            n_samples=n_samples,
-            unnormalise=False if target_dim > 1 else True,
-        )
-        assert [isinstance(df, pd.DataFrame) for df in [mean_df, std_df, samples_df]]
-        n_preds = len(dates) * len(X_t)
-        assert_shape(mean_df, (n_preds, target_dim))
-        assert_shape(std_df, (n_preds, target_dim))
-        assert_shape(samples_df, (n_samples * n_preds, target_dim))
+        for X_t in [self.df.loc[dates[0]], np.zeros((2, 4))]:
+            mean_df, std_df, samples_df = model.predict(
+                tasks,
+                X_t=X_t,
+                n_samples=n_samples,
+                unnormalise=False if target_dim > 1 else True,
+            )
+            assert [
+                isinstance(df, pd.DataFrame) for df in [mean_df, std_df, samples_df]
+            ]
+            if isinstance(X_t, (pd.DataFrame, pd.Series, pd.Index)):
+                N_t = len(X_t)
+            elif isinstance(X_t, np.ndarray):
+                N_t = X_t.shape[-1]
+            n_preds = len(dates) * N_t
+            assert_shape(mean_df, (n_preds, target_dim))
+            assert_shape(std_df, (n_preds, target_dim))
+            assert_shape(samples_df, (n_samples * n_preds, target_dim))
 
     def test_nans_in_context(self):
         """Test nothing breaks when NaNs present in context"""
         tl = TaskLoader(context=self.da, target=self.da)
         task = tl("2020-01-01", context_sampling=10, target_sampling=10)
 
         # Convert first observation of context to NaN
         task["Y_c"][0][0] = np.nan
 
         model = ConvNP(self.dp, tl, unet_channels=(5, 5, 5), verbose=False)
 
         # Check that nothing breaks
         model(task)
 
+    def test_highlevel_predict_coords_align_with_X_t_ongrid(self):
+        """Test coordinates of the xarray returned predictions align with the coordinates of X_t"""
+
+        # Instantiate an xarray object that would lead to rounding errors
+        region_size = (61, 81)
+        lat_lims = (30, 75)
+        lon_lims = (-15, 45)
+        latitude = np.linspace(*lat_lims, region_size[0], dtype=np.float32)
+        longitude = np.linspace(*lon_lims, region_size[1], dtype=np.float32)
+        dummy_data = np.random.normal(size=(1, *region_size))
+        da_raw = xr.DataArray(
+            dummy_data,
+            dims=["time", "latitude", "longitude"],
+            coords={
+                "time": [pd.Timestamp("2020-01-01")],
+                "latitude": latitude,
+                "longitude": longitude,
+            },
+            name="dummy_data",
+        )
+
+        dp = DataProcessor(
+            x1_name="latitude", x1_map=lat_lims, x2_name="longitude", x2_map=lon_lims
+        )
+        da = dp(da_raw)
+
+        tl = TaskLoader(context=da, target=da)
+        model = ConvNP(dp, tl, unet_channels=(5, 5, 5), verbose=False)
+        task = tl("2020-01-01")
+        mean_ds, _ = model.predict(task, X_t=da_raw)
+
+        assert np.array_equal(mean_ds["latitude"], da_raw["latitude"])
+        assert np.array_equal(mean_ds["longitude"], da_raw["longitude"])
+
+    def test_highlevel_predict_coords_align_with_X_t_offgrid(self):
+        """Test coordinates of the pandas returned predictions align with the coordinates of X_t"""
+
+        # Instantiate a pandas object that would lead to rounding errors
+        region_size = (61, 81)
+        lat_lims = (30, 75)
+        lon_lims = (-15, 45)
+        latitude = np.linspace(*lat_lims, region_size[0], dtype=np.float32)
+        longitude = np.linspace(*lon_lims, region_size[1], dtype=np.float32)
+        dummy_data = np.random.normal(size=(region_size)).ravel()
+        df_raw = pd.DataFrame(
+            dummy_data,
+            index=pd.MultiIndex.from_product(
+                [[pd.Timestamp("2020-01-01")], latitude, longitude],
+                names=["time", "latitude", "longitude"],
+            ),
+            columns=["dummy_data"],
+        )
+
+        dp = DataProcessor(
+            x1_name="latitude", x1_map=lat_lims, x2_name="longitude", x2_map=lon_lims
+        )
+        df = dp(df_raw)
+
+        tl = TaskLoader(context=df, target=df)
+        model = ConvNP(dp, tl, unet_channels=(5, 5, 5), verbose=False)
+        task = tl("2020-01-01")
+        mean_df, _ = model.predict(task, X_t=df_raw.loc["2020-01-01"])
+
+        assert np.array_equal(
+            mean_df.reset_index()["latitude"], df_raw.reset_index()["latitude"]
+        )
+        assert np.array_equal(
+            mean_df.reset_index()["longitude"], df_raw.reset_index()["longitude"]
+        )
+
 
 def assert_shape(x, shape: tuple):
     """ex: assert_shape(conv_input_array, [8, 3, None, None])"""
     # TODO put this in a utils module?
     assert len(x.shape) == len(shape), (x.shape, shape)
     for _a, _b in zip(x.shape, shape):
         if isinstance(_b, int):
```

### Comparing `deepsensor-0.1.4/tests/test_plotting.py` & `deepsensor-0.1.5/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.4/tests/test_task_loader.py` & `deepsensor-0.1.5/tests/test_task_loader.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 
 import xarray as xr
 import numpy as np
 import pandas as pd
 import unittest
 
+from deepsensor.errors import InvalidSamplingStrategyError
 from tests.utils import gen_random_data_xr, gen_random_data_pandas
 
 from deepsensor.data.loader import TaskLoader
 
 
 def _gen_data_xr(coords=None, dims=None, data_vars=None):
     """Gen random normalised data"""
@@ -46,36 +47,40 @@
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         # It's safe to share data between tests because the TaskLoader does not modify data
         self.da = _gen_data_xr()
         self.df = _gen_data_pandas()
 
-    def _gen_task_loader_call_args(self, n_context, n_target):
+    def _gen_task_loader_call_args(self, n_context_sets, n_target_sets):
         """Generate arguments for TaskLoader.__call__
 
         Loops over all possible combinations of context/target sampling methods
         and returns a list of arguments for TaskLoader.__call__.
         Options tested include:
         - (int): Random number of samples
         - (float): Fraction of samples
         - "all": All samples
+        - (np.ndarray): Array of coordinates to sample from the dataset (WIP)
 
         Args:
-            n_context (int): Number of context samples
-            n_target (int): Number of target samples
+            n_context_sets (int): Number of context samples
+            n_target_sets (int): Number of target samples
         Returns:
             (tuple): Arguments for TaskLoader.__call__
         """
         for sampling_method in [
+            0.0,
+            0,
             10,
             0.5,
             "all",
+            np.zeros((2, 1)),
         ]:
-            yield [sampling_method] * n_context, [sampling_method] * n_target
+            yield [sampling_method] * n_context_sets, [sampling_method] * n_target_sets
 
     @parameterized.expand(range(1, 4))
     def test_loader_call(self, n_context_and_target):
         """Test TaskLoader.__call__ for all possible combinations of context/target sampling methods
 
         Generates all possible combinations of xarray and pandas context/target sets
         of length n_context_and_target and calls TaskLoader.__call__ with all possible sampling methods.
@@ -87,45 +92,77 @@
         context_ID_list = list(
             itertools.product(["xr", "pd"], repeat=n_context_and_target)
         )
         target_ID_list = list(
             itertools.product(["xr", "pd"], repeat=n_context_and_target)
         )
 
-        def set_list_to_data(set_list):
+        def data_type_ID_to_data(set_list):
+            """Converts a list of data type IDs ("pd" or "xr") to a list of data objects of that type
+
+            E.g. ["xr", "pd", "xr"] -> [self.da, self.df, self.da]
+            E.g. "xr" -> self.da
+            """
             if set_list == "xr":
                 return self.da
             elif set_list == "pd":
                 return self.df
             elif isinstance(set_list, (list, tuple)):
-                return [set_list_to_data(s) for s in set_list]
+                return [data_type_ID_to_data(s) for s in set_list]
 
         for context_IDs, target_IDs in zip(context_ID_list, target_ID_list):
-            tl = TaskLoader(
-                context=set_list_to_data(context_IDs),
-                target=set_list_to_data(target_IDs),
-            )
-            print(repr(tl))
-            print(tl)
+            context = data_type_ID_to_data(context_IDs)
+            target = data_type_ID_to_data(target_IDs)
+            tl = TaskLoader(context=context, target=target)
 
             for context_sampling, target_sampling in self._gen_task_loader_call_args(
                 n_context_and_target, n_context_and_target
             ):
                 task = tl("2020-01-01", context_sampling, target_sampling)
 
         return None
 
-    def test_wrong_length_sampling_strat(self):
-        """Sampling strategy must be same length as context/target"""
-        tl = TaskLoader(
-            context=self.da,
-            target=self.da,
-        )
-        with self.assertRaises(ValueError):
-            task = tl("2020-01-01", ["all", "all"], ["all", "all"])
+    def test_invalid_sampling_strat(self):
+        """Test invalid sampling strategy in `TaskLoader.__call__`
+
+        Here we only need to test context sampling strategies because the same code to check
+        the validity of the sampling strategy is used for context and target sampling.
+        """
+        invalid_context_sampling_strategies = [
+            # Sampling strategy must be same length as context/target
+            ["all", "all", "all"],
+            # If integer, sampling strategy must be positive
+            -1,
+            # If float, sampling strategy must be less than or equal to 1.0
+            1.1,
+            # If float, sampling strategy must be greater than or equal to 0.0
+            -0.1,
+            # If str, sampling strategy must be in ["all", "split"]
+            "invalid",
+            # If np.ndarray, sampling strategy must be shape (2, N)
+            np.zeros((1, 2, 2)),
+            # If np.ndarray, coordinates must exist in the dataset
+            np.ones((2, 1)) * 1000,
+            # Invalid type
+            dict(foo="bar"),
+        ]
+
+        for tl in [
+            TaskLoader(
+                context=self.da,
+                target=self.da,
+            ),
+            TaskLoader(
+                context=self.df,
+                target=self.df,
+            ),
+        ]:
+            for invalid_sampling_strategy in invalid_context_sampling_strategies:
+                with self.assertRaises(InvalidSamplingStrategyError):
+                    task = tl("2020-01-01", invalid_sampling_strategy)
 
     def test_split_fails_if_not_df(self):
         """The "split" sampling strategy only works with pandas objects (currently)"""
         with self.assertRaises(ValueError):
             # Indexes don't connect two pandas objects
             tl = TaskLoader(context=self.df, target=self.da, links=[(0, 0)])
```

### Comparing `deepsensor-0.1.4/tests/test_training.py` & `deepsensor-0.1.5/tests/test_training.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,7 +77,11 @@
         # batch_size = None
         batch_size = 5
         n_epochs = 10
         epoch_losses = []
         for epoch in tqdm(range(n_epochs)):
             batch_losses = train_epoch(model, train_tasks, batch_size=batch_size)
             epoch_losses.append(np.mean(batch_losses))
+
+        # Check for NaNs in the loss
+        loss = np.mean(epoch_losses)
+        self.assertFalse(np.isnan(loss))
```

### Comparing `deepsensor-0.1.4/tests/utils.py` & `deepsensor-0.1.5/tests/utils.py`

 * *Files identical despite different names*

