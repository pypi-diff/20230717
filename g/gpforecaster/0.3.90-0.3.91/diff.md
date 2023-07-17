# Comparing `tmp/gpforecaster-0.3.90.tar.gz` & `tmp/gpforecaster-0.3.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpforecaster-0.3.90.tar", last modified: Mon Jul 17 08:58:41 2023, max compression
+gzip compressed data, was "gpforecaster-0.3.91.tar", last modified: Mon Jul 17 09:33:00 2023, max compression
```

## Comparing `gpforecaster-0.3.90.tar` & `gpforecaster-0.3.91.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:58:41.046911 gpforecaster-0.3.90/
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-17 08:58:30.000000 gpforecaster-0.3.90/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-17 08:58:41.046911 gpforecaster-0.3.90/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-07-17 08:58:30.000000 gpforecaster-0.3.90/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:58:41.038911 gpforecaster-0.3.90/gpforecaster/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-17 08:58:30.000000 gpforecaster-0.3.90/gpforecaster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:58:41.042911 gpforecaster-0.3.90/gpforecaster/model/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-17 08:58:30.000000 gpforecaster-0.3.90/gpforecaster/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-17 08:58:30.000000 gpforecaster-0.3.90/gpforecaster/model/gp.py
--rw-r--r--   0 runner    (1001) docker     (123)    38269 2023-07-17 08:58:30.000000 gpforecaster-0.3.90/gpforecaster/model/gpf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-07-17 08:58:30.000000 gpforecaster-0.3.90/gpforecaster/model/hyperparameter_tuning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-07-17 08:58:30.000000 gpforecaster-0.3.90/gpforecaster/model/mean_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-17 08:58:30.000000 gpforecaster-0.3.90/gpforecaster/model/mlls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:58:41.042911 gpforecaster-0.3.90/gpforecaster/results/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-17 08:58:30.000000 gpforecaster-0.3.90/gpforecaster/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-07-17 08:58:30.000000 gpforecaster-0.3.90/gpforecaster/results/calculate_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:58:41.046911 gpforecaster-0.3.90/gpforecaster/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:58:30.000000 gpforecaster-0.3.90/gpforecaster/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-17 08:58:30.000000 gpforecaster-0.3.90/gpforecaster/tests/test_calculate_results.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-17 08:58:30.000000 gpforecaster-0.3.90/gpforecaster/tests/test_early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-17 08:58:30.000000 gpforecaster-0.3.90/gpforecaster/tests/test_hyperparameter_tuning.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-17 08:58:30.000000 gpforecaster-0.3.90/gpforecaster/tests/test_hyperparameter_tuning_m5.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-17 08:58:30.000000 gpforecaster-0.3.90/gpforecaster/tests/test_model_results_m5.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-17 08:58:30.000000 gpforecaster-0.3.90/gpforecaster/tests/test_model_results_police.py
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-07-17 08:58:30.000000 gpforecaster-0.3.90/gpforecaster/tests/test_model_results_prison.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-17 08:58:30.000000 gpforecaster-0.3.90/gpforecaster/tests/test_results_partial_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-17 08:58:30.000000 gpforecaster-0.3.90/gpforecaster/tests/test_run_model_with_sampled_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-17 08:58:30.000000 gpforecaster-0.3.90/gpforecaster/tests/test_sparse_gps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-07-17 08:58:30.000000 gpforecaster-0.3.90/gpforecaster/tests/test_store_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-17 08:58:30.000000 gpforecaster-0.3.90/gpforecaster/tests/test_svg_gps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-17 08:58:30.000000 gpforecaster-0.3.90/gpforecaster/tests/test_tourism_gpf_with_local_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:58:41.046911 gpforecaster-0.3.90/gpforecaster/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:58:30.000000 gpforecaster-0.3.90/gpforecaster/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-17 08:58:30.000000 gpforecaster-0.3.90/gpforecaster/utils/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:58:41.046911 gpforecaster-0.3.90/gpforecaster/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-17 08:58:30.000000 gpforecaster-0.3.90/gpforecaster/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-07-17 08:58:30.000000 gpforecaster-0.3.90/gpforecaster/visualization/plot_predictions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:58:41.038911 gpforecaster-0.3.90/gpforecaster.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-17 08:58:40.000000 gpforecaster-0.3.90/gpforecaster.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-17 08:58:41.000000 gpforecaster-0.3.90/gpforecaster.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 08:58:40.000000 gpforecaster-0.3.90/gpforecaster.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-17 08:58:40.000000 gpforecaster-0.3.90/gpforecaster.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-17 08:58:40.000000 gpforecaster-0.3.90/gpforecaster.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 08:58:41.046911 gpforecaster-0.3.90/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-17 08:58:30.000000 gpforecaster-0.3.90/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:33:00.567032 gpforecaster-0.3.91/
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-17 09:32:47.000000 gpforecaster-0.3.91/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-17 09:33:00.567032 gpforecaster-0.3.91/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-07-17 09:32:47.000000 gpforecaster-0.3.91/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:33:00.563032 gpforecaster-0.3.91/gpforecaster/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-17 09:32:47.000000 gpforecaster-0.3.91/gpforecaster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:33:00.563032 gpforecaster-0.3.91/gpforecaster/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-17 09:32:47.000000 gpforecaster-0.3.91/gpforecaster/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-17 09:32:47.000000 gpforecaster-0.3.91/gpforecaster/model/gp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38424 2023-07-17 09:32:47.000000 gpforecaster-0.3.91/gpforecaster/model/gpf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-07-17 09:32:47.000000 gpforecaster-0.3.91/gpforecaster/model/hyperparameter_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-07-17 09:32:47.000000 gpforecaster-0.3.91/gpforecaster/model/mean_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-17 09:32:47.000000 gpforecaster-0.3.91/gpforecaster/model/mlls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:33:00.563032 gpforecaster-0.3.91/gpforecaster/results/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-17 09:32:47.000000 gpforecaster-0.3.91/gpforecaster/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-07-17 09:32:47.000000 gpforecaster-0.3.91/gpforecaster/results/calculate_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:33:00.563032 gpforecaster-0.3.91/gpforecaster/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:32:47.000000 gpforecaster-0.3.91/gpforecaster/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-17 09:32:47.000000 gpforecaster-0.3.91/gpforecaster/tests/test_calculate_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-17 09:32:47.000000 gpforecaster-0.3.91/gpforecaster/tests/test_early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-17 09:32:47.000000 gpforecaster-0.3.91/gpforecaster/tests/test_hyperparameter_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-17 09:32:47.000000 gpforecaster-0.3.91/gpforecaster/tests/test_hyperparameter_tuning_m5.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-17 09:32:47.000000 gpforecaster-0.3.91/gpforecaster/tests/test_model_results_m5.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-17 09:32:47.000000 gpforecaster-0.3.91/gpforecaster/tests/test_model_results_police.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-07-17 09:32:47.000000 gpforecaster-0.3.91/gpforecaster/tests/test_model_results_prison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-17 09:32:47.000000 gpforecaster-0.3.91/gpforecaster/tests/test_results_partial_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-17 09:32:47.000000 gpforecaster-0.3.91/gpforecaster/tests/test_run_model_with_sampled_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-17 09:32:47.000000 gpforecaster-0.3.91/gpforecaster/tests/test_sparse_gps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-07-17 09:32:47.000000 gpforecaster-0.3.91/gpforecaster/tests/test_store_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-17 09:32:47.000000 gpforecaster-0.3.91/gpforecaster/tests/test_svg_gps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-17 09:32:47.000000 gpforecaster-0.3.91/gpforecaster/tests/test_tourism_gpf_with_local_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:33:00.563032 gpforecaster-0.3.91/gpforecaster/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:32:47.000000 gpforecaster-0.3.91/gpforecaster/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-17 09:32:47.000000 gpforecaster-0.3.91/gpforecaster/utils/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:33:00.563032 gpforecaster-0.3.91/gpforecaster/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-17 09:32:47.000000 gpforecaster-0.3.91/gpforecaster/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-07-17 09:32:47.000000 gpforecaster-0.3.91/gpforecaster/visualization/plot_predictions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:33:00.563032 gpforecaster-0.3.91/gpforecaster.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-17 09:33:00.000000 gpforecaster-0.3.91/gpforecaster.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-17 09:33:00.000000 gpforecaster-0.3.91/gpforecaster.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 09:33:00.000000 gpforecaster-0.3.91/gpforecaster.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-17 09:33:00.000000 gpforecaster-0.3.91/gpforecaster.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-17 09:33:00.000000 gpforecaster-0.3.91/gpforecaster.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 09:33:00.567032 gpforecaster-0.3.91/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-17 09:32:47.000000 gpforecaster-0.3.91/setup.py
```

### Comparing `gpforecaster-0.3.90/LICENCE` & `gpforecaster-0.3.91/LICENCE`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.90/PKG-INFO` & `gpforecaster-0.3.91/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpforecaster
-Version: 0.3.90
+Version: 0.3.91
 Summary: Hierarchical time series forecasting model using Gaussian Processes
 Home-page: UNKNOWN
 Author: Luis Roque
 Author-email: <roque0luis@gmail.com>
 License: UNKNOWN
 Keywords: python,time series,hierarchical,forecasting,gaussian process,machine learning
 Platform: UNKNOWN
```

### Comparing `gpforecaster-0.3.90/README.md` & `gpforecaster-0.3.91/README.md`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.90/gpforecaster/model/gp.py` & `gpforecaster-0.3.91/gpforecaster/model/gp.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.90/gpforecaster/model/gpf.py` & `gpforecaster-0.3.91/gpforecaster/model/gpf.py`

 * *Files 1% similar despite different names*

```diff
@@ -811,19 +811,24 @@
             hierarchical_pred = self.hierarchical_data_summary(val_pred)
             concatenated_pred = self.concatenate_arrays(hierarchical_pred)
 
             concatenated_pred = concatenated_pred.cpu().numpy()
             val_y = val_y.cpu().numpy()
             train_y = train_y.cpu().numpy()
 
+            if train_y.shape[0] < self.seasonality:
+                sp = 1  # non-seasonal case, use a lag of 1
+            else:
+                sp = self.seasonality
+
             val_loss = self.mase(
                 y_pred=concatenated_pred,
                 y_true=val_y,
                 y_train=train_y,
-                sp=self.seasonality,
+                sp=sp,
             ).mean()
 
         return val_loss.item()
 
     @staticmethod
     def _create_directory_if_not_exists(directory_path):
         if not os.path.exists(directory_path):
```

### Comparing `gpforecaster-0.3.90/gpforecaster/model/hyperparameter_tuning.py` & `gpforecaster-0.3.91/gpforecaster/model/hyperparameter_tuning.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.90/gpforecaster/model/mean_functions.py` & `gpforecaster-0.3.91/gpforecaster/model/mean_functions.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.90/gpforecaster/model/mlls.py` & `gpforecaster-0.3.91/gpforecaster/model/mlls.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.90/gpforecaster/results/calculate_metrics.py` & `gpforecaster-0.3.91/gpforecaster/results/calculate_metrics.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.90/gpforecaster/tests/test_calculate_results.py` & `gpforecaster-0.3.91/gpforecaster/tests/test_calculate_results.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.90/gpforecaster/tests/test_early_stopping.py` & `gpforecaster-0.3.91/gpforecaster/tests/test_early_stopping.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.90/gpforecaster/tests/test_hyperparameter_tuning.py` & `gpforecaster-0.3.91/gpforecaster/tests/test_hyperparameter_tuning.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.90/gpforecaster/tests/test_hyperparameter_tuning_m5.py` & `gpforecaster-0.3.91/gpforecaster/tests/test_hyperparameter_tuning_m5.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.90/gpforecaster/tests/test_model_results_m5.py` & `gpforecaster-0.3.91/gpforecaster/tests/test_model_results_m5.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.90/gpforecaster/tests/test_model_results_police.py` & `gpforecaster-0.3.91/gpforecaster/tests/test_model_results_police.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.90/gpforecaster/tests/test_model_results_prison.py` & `gpforecaster-0.3.91/gpforecaster/tests/test_model_results_prison.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.90/gpforecaster/tests/test_results_partial_data.py` & `gpforecaster-0.3.91/gpforecaster/tests/test_results_partial_data.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.90/gpforecaster/tests/test_run_model_with_sampled_dataset.py` & `gpforecaster-0.3.91/gpforecaster/tests/test_run_model_with_sampled_dataset.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.90/gpforecaster/tests/test_sparse_gps.py` & `gpforecaster-0.3.91/gpforecaster/tests/test_sparse_gps.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.90/gpforecaster/tests/test_store_results.py` & `gpforecaster-0.3.91/gpforecaster/tests/test_store_results.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.90/gpforecaster/tests/test_svg_gps.py` & `gpforecaster-0.3.91/gpforecaster/tests/test_svg_gps.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.90/gpforecaster/tests/test_tourism_gpf_with_local_file.py` & `gpforecaster-0.3.91/gpforecaster/tests/test_tourism_gpf_with_local_file.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.90/gpforecaster/utils/logger.py` & `gpforecaster-0.3.91/gpforecaster/utils/logger.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.90/gpforecaster/visualization/plot_predictions.py` & `gpforecaster-0.3.91/gpforecaster/visualization/plot_predictions.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.90/gpforecaster.egg-info/PKG-INFO` & `gpforecaster-0.3.91/gpforecaster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpforecaster
-Version: 0.3.90
+Version: 0.3.91
 Summary: Hierarchical time series forecasting model using Gaussian Processes
 Home-page: UNKNOWN
 Author: Luis Roque
 Author-email: <roque0luis@gmail.com>
 License: UNKNOWN
 Keywords: python,time series,hierarchical,forecasting,gaussian process,machine learning
 Platform: UNKNOWN
```

### Comparing `gpforecaster-0.3.90/gpforecaster.egg-info/SOURCES.txt` & `gpforecaster-0.3.91/gpforecaster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.90/setup.py` & `gpforecaster-0.3.91/setup.py`

 * *Files identical despite different names*

