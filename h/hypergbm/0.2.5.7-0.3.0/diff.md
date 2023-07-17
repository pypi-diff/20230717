# Comparing `tmp/hypergbm-0.2.5.7.tar.gz` & `tmp/hypergbm-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypergbm-0.2.5.7.tar", last modified: Sat Nov 26 06:05:43 2022, max compression
+gzip compressed data, was "hypergbm-0.3.0.tar", last modified: Mon Jul 17 09:40:36 2023, max compression
```

## Comparing `hypergbm-0.2.5.7.tar` & `hypergbm-0.3.0.tar`

### file list

```diff
@@ -1,133 +1,140 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-26 06:05:43.725306 hypergbm-0.2.5.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8362 2022-11-26 06:05:43.725306 hypergbm-0.2.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6945 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-26 06:05:43.709306 hypergbm-0.2.5.7/hypergbm/
--rw-r--r--   0 runner    (1001) docker     (123)      471 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/cfg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-26 06:05:43.709306 hypergbm-0.2.5.7/hypergbm/cuml/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/cuml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/cuml/_estimators.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/cuml/_hyper_gbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/cuml/_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/cuml/_search_space.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-26 06:05:43.709306 hypergbm-0.2.5.7/hypergbm/dask/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/dask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8211 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/dask/_estimators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/dask/dask_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     7423 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/dask/dask_transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5386 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/dask/search_space.py
--rw-r--r--   0 runner    (1001) docker     (123)    29966 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/estimators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-26 06:05:43.713306 hypergbm-0.2.5.7/hypergbm/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    22901 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/examples/00.get-doc.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7634 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/examples/01.quick-start.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11487 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/examples/02.basic-setting.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6317 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/examples/11.feature_selection.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    69168 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/examples/12.collinearity_detection.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   113768 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/examples/13.drift_detection.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    20289 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/examples/14.feature_generation_datetime.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    22370 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/examples/15.feature_generation_latlong_text.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6533 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/examples/17.feature_reselection.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5844 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/examples/18.pseudo_labeling.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6939 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/examples/21.classbalance.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11374 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/examples/31.search_space.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8484 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/examples/32.customize_estimator.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5467 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/examples/51.HyperGBM.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   588048 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/examples/71.hypergbm_shap.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/examples/72.hypegbm_experiment_notebook_visualization.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   143657 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/examples/73.hypergbm_shap_explainer.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   205701 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/examples/74.hypergbm_experiment_explainer.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11423 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/examples/C01.quick-start-with-RAPIDS(cuDF_cuML).ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-26 06:05:43.705306 hypergbm-0.2.5.7/hypergbm/examples/datasets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-26 06:05:43.713306 hypergbm-0.2.5.7/hypergbm/examples/datasets/Bank/
--rw-r--r--   0 runner    (1001) docker     (123)   132253 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/examples/datasets/Bank/test.csv.gz
--rw-r--r--   0 runner    (1001) docker     (123)   521623 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/examples/datasets/Bank/train.csv.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-26 06:05:43.717306 hypergbm-0.2.5.7/hypergbm/examples/datasets/Magic/
--rw-r--r--   0 runner    (1001) docker     (123)   134499 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/examples/datasets/Magic/test.csv.gz
--rw-r--r--   0 runner    (1001) docker     (123)   503449 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/examples/datasets/Magic/train.csv.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-26 06:05:43.717306 hypergbm-0.2.5.7/hypergbm/examples/datasets/Metro_Interstate_Traffic_Volume/
--rw-r--r--   0 runner    (1001) docker     (123)   399489 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/examples/datasets/Metro_Interstate_Traffic_Volume/data.csv.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-26 06:05:43.717306 hypergbm-0.2.5.7/hypergbm/examples/datasets/Spambase/
--rw-r--r--   0 runner    (1001) docker     (123)    28076 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/examples/datasets/Spambase/test.csv.gz
--rw-r--r--   0 runner    (1001) docker     (123)   111675 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/examples/datasets/Spambase/train.csv.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-26 06:05:43.717306 hypergbm-0.2.5.7/hypergbm/examples/datasets/West_Nile_Virus/
--rw-r--r--   0 runner    (1001) docker     (123)    34249 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/examples/datasets/West_Nile_Virus/test.csv.gz
--rw-r--r--   0 runner    (1001) docker     (123)   128552 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/examples/datasets/West_Nile_Virus/train.csv.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-26 06:05:43.717306 hypergbm-0.2.5.7/hypergbm/examples/datasets/West_Nile_Virus_II/
--rw-r--r--   0 runner    (1001) docker     (123)    42471 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/examples/datasets/West_Nile_Virus_II/test.csv.gz
--rw-r--r--   0 runner    (1001) docker     (123)   159042 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/examples/datasets/West_Nile_Virus_II/train.csv.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-26 06:05:43.721306 hypergbm-0.2.5.7/hypergbm/examples/misc/
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/examples/misc/class_balancing.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4682 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/examples/misc/cross_validation.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/examples/misc/drift_detection.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/examples/misc/early_stopping.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6069 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/examples/misc/emsemble.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5208 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/examples/misc/estimators.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/examples/misc/feature_generation.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/examples/misc/feature_selection.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   443546 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/examples/misc/hypergbm_shap.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6864 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/examples/misc/infer_task_type.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6316 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/examples/misc/pseudo_labeling.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/examples/misc/searchers.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    16367 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-26 06:05:43.721306 hypergbm-0.2.5.7/hypergbm/experiment_callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/experiment_callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/experiment_callbacks/_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/experiment_callbacks/_hyper_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-26 06:05:43.721306 hypergbm-0.2.5.7/hypergbm/gbm_callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/gbm_callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/gbm_callbacks/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/gbm_callbacks/_catboost_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/gbm_callbacks/_lightgbm_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/gbm_callbacks/_xgboost_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/gpu_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    31513 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/hyper_gbm.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/job.py
--rw-r--r--   0 runner    (1001) docker     (123)    11830 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/search_space.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-26 06:05:43.721306 hypergbm-0.2.5.7/hypergbm/sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6560 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/sklearn/sklearn_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-26 06:05:43.721306 hypergbm-0.2.5.7/hypergbm/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-26 06:05:43.725306 hypergbm-0.2.5.7/hypergbm/tests/cuml_/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/tests/cuml_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/tests/cuml_/experiment_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/tests/cuml_/hypergbm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/tests/cuml_/run_experiment_cuml.py
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/tests/cuml_/run_hypergbm_cuml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-26 06:05:43.725306 hypergbm-0.2.5.7/hypergbm/tests/dask_/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/tests/dask_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/tests/dask_/experiment_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/tests/dask_/run_hypergbm_dask.py
--rw-r--r--   0 runner    (1001) docker     (123)     7691 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/tests/estimator_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    23089 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/tests/experiment_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/tests/hyperboard_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13156 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/tests/hypergbm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/tests/run_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/tests/run_experiment_explainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/tests/run_explainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/tests/run_hypergbm.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/tests/run_web_visualization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/tests/search_space_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-26 06:05:43.725306 hypergbm-0.2.5.7/hypergbm/tests/sklearn_/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/tests/sklearn_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10787 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/tests/sklearn_/sklearn_ops_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-26 06:05:43.725306 hypergbm-0.2.5.7/hypergbm/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/tests/utils/tool_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-26 06:05:43.725306 hypergbm-0.2.5.7/hypergbm/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9105 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/utils/kendall_tau_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    31938 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/hypergbm/utils/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-26 06:05:43.709306 hypergbm-0.2.5.7/hypergbm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8362 2022-11-26 06:05:43.000000 hypergbm-0.2.5.7/hypergbm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2022-11-26 06:05:43.000000 hypergbm-0.2.5.7/hypergbm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-11-26 06:05:43.000000 hypergbm-0.2.5.7/hypergbm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2022-11-26 06:05:43.000000 hypergbm-0.2.5.7/hypergbm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-11-26 06:05:43.000000 hypergbm-0.2.5.7/hypergbm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      451 2022-11-26 06:05:43.000000 hypergbm-0.2.5.7/hypergbm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2022-11-26 06:05:43.000000 hypergbm-0.2.5.7/hypergbm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-11-26 06:05:43.725306 hypergbm-0.2.5.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4322 2022-11-26 06:05:38.000000 hypergbm-0.2.5.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:40:36.152926 hypergbm-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 09:40:29.000000 hypergbm-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8790 2023-07-17 09:40:36.152926 hypergbm-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7408 2023-07-17 09:40:29.000000 hypergbm-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:40:36.132926 hypergbm-0.3.0/hypergbm/
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/cfg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:40:36.136926 hypergbm-0.3.0/hypergbm/cuml/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/cuml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/cuml/_estimators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/cuml/_hyper_gbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/cuml/_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/cuml/_search_space.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:40:36.136926 hypergbm-0.3.0/hypergbm/dask/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/dask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/dask/_estimators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/dask/dask_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/dask/dask_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5386 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/dask/search_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30552 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/estimators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:40:36.140926 hypergbm-0.3.0/hypergbm/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    22901 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/examples/00.get-doc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/examples/01.quick-start.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11487 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/examples/02.basic-setting.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/examples/11.feature_selection.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    69168 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/examples/12.collinearity_detection.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   113768 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/examples/13.drift_detection.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    20289 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/examples/14.feature_generation_datetime.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    22370 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/examples/15.feature_generation_latlong_text.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/examples/17.feature_reselection.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5844 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/examples/18.pseudo_labeling.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/examples/21.classbalance.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/examples/31.search_space.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8484 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/examples/32.customize_estimator.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    14800 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/examples/33.multiple_objectives.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/examples/51.HyperGBM.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   122416 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/examples/61.NSGAII_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   134107 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/examples/62.RNSGAII_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    94313 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/examples/63.MOEAD_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9934 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/examples/66.Objectives_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   588048 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/examples/71.hypergbm_shap.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/examples/72.hypegbm_experiment_notebook_visualization.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   143657 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/examples/73.hypergbm_shap_explainer.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   205701 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/examples/74.hypergbm_experiment_explainer.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11423 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/examples/C01.quick-start-with-RAPIDS(cuDF_cuML).ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:40:36.128926 hypergbm-0.3.0/hypergbm/examples/datasets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:40:36.140926 hypergbm-0.3.0/hypergbm/examples/datasets/Bank/
+-rw-r--r--   0 runner    (1001) docker     (123)   132253 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/examples/datasets/Bank/test.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (123)   521623 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/examples/datasets/Bank/train.csv.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:40:36.144926 hypergbm-0.3.0/hypergbm/examples/datasets/Magic/
+-rw-r--r--   0 runner    (1001) docker     (123)   134499 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/examples/datasets/Magic/test.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (123)   503449 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/examples/datasets/Magic/train.csv.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:40:36.144926 hypergbm-0.3.0/hypergbm/examples/datasets/Metro_Interstate_Traffic_Volume/
+-rw-r--r--   0 runner    (1001) docker     (123)   399489 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/examples/datasets/Metro_Interstate_Traffic_Volume/data.csv.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:40:36.144926 hypergbm-0.3.0/hypergbm/examples/datasets/Spambase/
+-rw-r--r--   0 runner    (1001) docker     (123)    28076 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/examples/datasets/Spambase/test.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (123)   111675 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/examples/datasets/Spambase/train.csv.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:40:36.144926 hypergbm-0.3.0/hypergbm/examples/datasets/West_Nile_Virus/
+-rw-r--r--   0 runner    (1001) docker     (123)    34249 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/examples/datasets/West_Nile_Virus/test.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (123)   128552 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/examples/datasets/West_Nile_Virus/train.csv.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:40:36.144926 hypergbm-0.3.0/hypergbm/examples/datasets/West_Nile_Virus_II/
+-rw-r--r--   0 runner    (1001) docker     (123)    42471 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/examples/datasets/West_Nile_Virus_II/test.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (123)   159042 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/examples/datasets/West_Nile_Virus_II/train.csv.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:40:36.148926 hypergbm-0.3.0/hypergbm/examples/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/examples/misc/class_balancing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/examples/misc/cross_validation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/examples/misc/drift_detection.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/examples/misc/early_stopping.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/examples/misc/emsemble.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/examples/misc/estimators.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/examples/misc/feature_generation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/examples/misc/feature_selection.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   443546 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/examples/misc/hypergbm_shap.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/examples/misc/infer_task_type.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/examples/misc/pseudo_labeling.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/examples/misc/searchers.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    16688 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:40:36.148926 hypergbm-0.3.0/hypergbm/experiment_callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/experiment_callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/experiment_callbacks/_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/experiment_callbacks/_hyper_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:40:36.148926 hypergbm-0.3.0/hypergbm/gbm_callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/gbm_callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/gbm_callbacks/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/gbm_callbacks/_catboost_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/gbm_callbacks/_lightgbm_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/gbm_callbacks/_xgboost_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/gpu_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31794 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/hyper_gbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/objectives.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13109 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/search_space.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:40:36.148926 hypergbm-0.3.0/hypergbm/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/sklearn/sklearn_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:40:36.152926 hypergbm-0.3.0/hypergbm/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:40:36.152926 hypergbm-0.3.0/hypergbm/tests/cuml_/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/tests/cuml_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/tests/cuml_/experiment_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/tests/cuml_/hypergbm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/tests/cuml_/run_experiment_cuml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/tests/cuml_/run_hypergbm_cuml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:40:36.152926 hypergbm-0.3.0/hypergbm/tests/dask_/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/tests/dask_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/tests/dask_/experiment_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/tests/dask_/run_hypergbm_dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/tests/estimator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24736 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/tests/experiment_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/tests/hyperboard_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14484 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/tests/hypergbm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/tests/run_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/tests/run_experiment_explainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/tests/run_explainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/tests/run_hypergbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/tests/run_web_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/tests/search_space_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:40:36.152926 hypergbm-0.3.0/hypergbm/tests/sklearn_/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/tests/sklearn_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10787 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/tests/sklearn_/sklearn_ops_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:40:36.152926 hypergbm-0.3.0/hypergbm/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/tests/utils/tool_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:40:36.152926 hypergbm-0.3.0/hypergbm/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/utils/detect_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/utils/kendall_tau_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31938 2023-07-17 09:40:29.000000 hypergbm-0.3.0/hypergbm/utils/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:40:36.136926 hypergbm-0.3.0/hypergbm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8790 2023-07-17 09:40:36.000000 hypergbm-0.3.0/hypergbm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-07-17 09:40:36.000000 hypergbm-0.3.0/hypergbm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 09:40:36.000000 hypergbm-0.3.0/hypergbm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-17 09:40:36.000000 hypergbm-0.3.0/hypergbm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 09:40:36.000000 hypergbm-0.3.0/hypergbm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-17 09:40:36.000000 hypergbm-0.3.0/hypergbm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-17 09:40:36.000000 hypergbm-0.3.0/hypergbm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 09:40:36.156926 hypergbm-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-07-17 09:40:29.000000 hypergbm-0.3.0/setup.py
```

### Comparing `hypergbm-0.2.5.7/LICENSE` & `hypergbm-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/PKG-INFO` & `hypergbm-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypergbm
-Version: 0.2.5.7
+Version: 0.3.0
 Summary: A full pipeline AutoML tool integrated various GBM models
 Home-page: https://github.com/DataCanvasIO/HyperGBM
 Author: DataCanvas Community
 Author-email: yangjian@zetyun.com
 License: Apache License 2.0
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -17,22 +17,23 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6.*
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: shap
+Provides-Extra: notebook
 Provides-Extra: board
 Provides-Extra: tests
-Provides-Extra: notebook
-Provides-Extra: shap
-Provides-Extra: dask
 Provides-Extra: zhcn
+Provides-Extra: dask
+Provides-Extra: fg
 Provides-Extra: all
 License-File: LICENSE
 
 <p align="center">
 <img src="https://github.com/DataCanvasIO/HyperGBM/raw/main/docs/static/images/HyperGBM.png" width="500" >
 
 
@@ -61,19 +62,14 @@
 
 Install HyperGBM with `conda` from the channel *conda-forge*:
 
 ```bash
 conda install -c conda-forge hypergbm
 ```
 
-On the Windows system, recommend install pyarrow(required by hypernets) 4.0 or earlier version with HyperGBM:
-
-```bash
-conda install -c conda-forge hypergbm "pyarrow<=4.0"
-```
 
 ### Pip
 
 Install HyperGBM with different `pip` options:
 
 * Typical installation:
 ```bash
@@ -83,15 +79,15 @@
 * To run HyperGBM in JupyterLab/Jupyter notebook, install with command:
 ```bash
 pip install hypergbm[notebook]
 ```
 
 * To support experiment visualization base on web, install with command:
 ```bash
-pip install hypergbm[board]
+pip install hypergbm[board] # Temporarily unavailable in version 0.3.x
 ```
 
 * To run HyperGBM in distributed Dask cluster, install with command:
 ```bash
 pip install hypergbm[dask]
 ```
 
@@ -154,29 +150,50 @@
 
 ## GPU Acceleration
 
 Hypergbm supports full pipeline GPU acceleration, including all steps from data processing to model training. In our experiments, we got a 50x performance improvement!  Most importantly, the model trained on GPU could be deployed to the environment without GPU hardware and software (e.g.,CUDA and cuML), which greatly reduces the cost of model deployment.
 
 ![Gpu Acceleration](https://github.com/DataCanvasIO/HyperGBM/raw/main/docs/static/images/gpu_speedup.png)
 
+## Documents
+
+* [Overview](https://hypergbm.readthedocs.io/en/latest/overview.html)
+* [Installation](https://hypergbm.readthedocs.io/en/latest/installation.html)
+* [Quick Start](https://hypergbm.readthedocs.io/en/latest/quick_start.html)
+* [Examples](https://hypergbm.readthedocs.io/en/latest/example.html)
+* [How-To](https://hypergbm.readthedocs.io/en/latest/how_to.html)
+* [Release Notes](https://hypergbm.readthedocs.io/en/latest/release_note.html)
+
 ## HyperGBM related projects
 * [Hypernets](https://github.com/DataCanvasIO/Hypernets): A general automated machine learning (AutoML) framework.
 * [HyperGBM](https://github.com/DataCanvasIO/HyperGBM): A full pipeline AutoML tool integrated various GBM models.
 * [HyperDT/DeepTables](https://github.com/DataCanvasIO/DeepTables): An AutoDL tool for tabular data.
 * [HyperTS](https://github.com/DataCanvasIO/HyperTS): A full pipeline AutoML&AutoDL tool for time series datasets.
 * [HyperKeras](https://github.com/DataCanvasIO/HyperKeras): An AutoDL tool for Neural Architecture Search and Hyperparameter Optimization on Tensorflow and Keras.
 * [HyperBoard](https://github.com/DataCanvasIO/HyperBoard): A visualization tool for Hypernets.
 * [Cooka](https://github.com/DataCanvasIO/Cooka): Lightweight interactive AutoML system.
 
-![DataCanvas AutoML Toolkit](https://github.com/DataCanvasIO/HyperGBM/raw/main/docs/static/images/DAT_logo.png)
+![DataCanvas AutoML Toolkit](https://raw.githubusercontent.com/DataCanvasIO/HyperGBM/main/docs/static/images/DAT_latest.png)
+
+## Citation
+
+If you use HyperGBM in your research, please cite us as follows:
+
+   Jian Yang, Xuefeng Li, Haifeng Wu. 
+   **HyperGBM: A full pipeline AutoML tool integrated with various GBM models.** https://github.com/DataCanvasIO/HyperGBM. 2020. Version 0.2.x.
+
+BibTex:
+
+```
+@misc{hypergbm,
+  author={Jian Yang, Xuefeng Li, Haifeng Wu},
+  title={{HyperGBM}: { A Full Pipeline AutoML Tool Integrated With Various GBM Models}},
+  howpublished={https://github.com/DataCanvasIO/HyperGBM},
+  note={Version 0.2.x},
+  year={2020}
+}
+```
 
-## Documents
 
-* [Overview](https://hypergbm.readthedocs.io/en/latest/overview.html)
-* [Installation](https://hypergbm.readthedocs.io/en/latest/installation.html)
-* [Quick Start](https://hypergbm.readthedocs.io/en/latest/quick_start.html)
-* [Examples](https://hypergbm.readthedocs.io/en/latest/example.html)
-* [How-To](https://hypergbm.readthedocs.io/en/latest/how_to.html)
-* [Release Notes](https://hypergbm.readthedocs.io/en/latest/release_note.html)
 
 ## DataCanvas
 HyperGBM is an open source project created by [DataCanvas](https://www.datacanvas.com/).
```

### Comparing `hypergbm-0.2.5.7/README.md` & `hypergbm-0.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -27,19 +27,14 @@
 
 Install HyperGBM with `conda` from the channel *conda-forge*:
 
 ```bash
 conda install -c conda-forge hypergbm
 ```
 
-On the Windows system, recommend install pyarrow(required by hypernets) 4.0 or earlier version with HyperGBM:
-
-```bash
-conda install -c conda-forge hypergbm "pyarrow<=4.0"
-```
 
 ### Pip
 
 Install HyperGBM with different `pip` options:
 
 * Typical installation:
 ```bash
@@ -49,15 +44,15 @@
 * To run HyperGBM in JupyterLab/Jupyter notebook, install with command:
 ```bash
 pip install hypergbm[notebook]
 ```
 
 * To support experiment visualization base on web, install with command:
 ```bash
-pip install hypergbm[board]
+pip install hypergbm[board] # Temporarily unavailable in version 0.3.x
 ```
 
 * To run HyperGBM in distributed Dask cluster, install with command:
 ```bash
 pip install hypergbm[dask]
 ```
 
@@ -120,29 +115,50 @@
 
 ## GPU Acceleration
 
 Hypergbm supports full pipeline GPU acceleration, including all steps from data processing to model training. In our experiments, we got a 50x performance improvement!  Most importantly, the model trained on GPU could be deployed to the environment without GPU hardware and software (e.g.,CUDA and cuML), which greatly reduces the cost of model deployment.
 
 ![Gpu Acceleration](docs/static/images/gpu_speedup.png)
 
+## Documents
+
+* [Overview](https://hypergbm.readthedocs.io/en/latest/overview.html)
+* [Installation](https://hypergbm.readthedocs.io/en/latest/installation.html)
+* [Quick Start](https://hypergbm.readthedocs.io/en/latest/quick_start.html)
+* [Examples](https://hypergbm.readthedocs.io/en/latest/example.html)
+* [How-To](https://hypergbm.readthedocs.io/en/latest/how_to.html)
+* [Release Notes](https://hypergbm.readthedocs.io/en/latest/release_note.html)
+
 ## HyperGBM related projects
 * [Hypernets](https://github.com/DataCanvasIO/Hypernets): A general automated machine learning (AutoML) framework.
 * [HyperGBM](https://github.com/DataCanvasIO/HyperGBM): A full pipeline AutoML tool integrated various GBM models.
 * [HyperDT/DeepTables](https://github.com/DataCanvasIO/DeepTables): An AutoDL tool for tabular data.
 * [HyperTS](https://github.com/DataCanvasIO/HyperTS): A full pipeline AutoML&AutoDL tool for time series datasets.
 * [HyperKeras](https://github.com/DataCanvasIO/HyperKeras): An AutoDL tool for Neural Architecture Search and Hyperparameter Optimization on Tensorflow and Keras.
 * [HyperBoard](https://github.com/DataCanvasIO/HyperBoard): A visualization tool for Hypernets.
 * [Cooka](https://github.com/DataCanvasIO/Cooka): Lightweight interactive AutoML system.
 
-![DataCanvas AutoML Toolkit](docs/static/images/DAT_logo.png)
+![DataCanvas AutoML Toolkit](https://raw.githubusercontent.com/DataCanvasIO/HyperGBM/main/docs/static/images/DAT_latest.png)
+
+## Citation
+
+If you use HyperGBM in your research, please cite us as follows:
+
+   Jian Yang, Xuefeng Li, Haifeng Wu. 
+   **HyperGBM: A full pipeline AutoML tool integrated with various GBM models.** https://github.com/DataCanvasIO/HyperGBM. 2020. Version 0.2.x.
+
+BibTex:
+
+```
+@misc{hypergbm,
+  author={Jian Yang, Xuefeng Li, Haifeng Wu},
+  title={{HyperGBM}: { A Full Pipeline AutoML Tool Integrated With Various GBM Models}},
+  howpublished={https://github.com/DataCanvasIO/HyperGBM},
+  note={Version 0.2.x},
+  year={2020}
+}
+```
 
-## Documents
 
-* [Overview](https://hypergbm.readthedocs.io/en/latest/overview.html)
-* [Installation](https://hypergbm.readthedocs.io/en/latest/installation.html)
-* [Quick Start](https://hypergbm.readthedocs.io/en/latest/quick_start.html)
-* [Examples](https://hypergbm.readthedocs.io/en/latest/example.html)
-* [How-To](https://hypergbm.readthedocs.io/en/latest/how_to.html)
-* [Release Notes](https://hypergbm.readthedocs.io/en/latest/release_note.html)
 
 ## DataCanvas
 HyperGBM is an open source project created by [DataCanvas](https://www.datacanvas.com/).
```

### Comparing `hypergbm-0.2.5.7/hypergbm/cfg.py` & `hypergbm-0.3.0/hypergbm/cfg.py`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/cuml/_estimators.py` & `hypergbm-0.3.0/hypergbm/cuml/_estimators.py`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/cuml/_hyper_gbm.py` & `hypergbm-0.3.0/hypergbm/cuml/_hyper_gbm.py`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/cuml/_ops.py` & `hypergbm-0.3.0/hypergbm/cuml/_ops.py`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/cuml/_search_space.py` & `hypergbm-0.3.0/hypergbm/cuml/_search_space.py`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/dask/_estimators.py` & `hypergbm-0.3.0/hypergbm/dask/_estimators.py`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/dask/dask_ops.py` & `hypergbm-0.3.0/hypergbm/dask/dask_ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         impute_strategy = Choice(['constant', 'most_frequent'])
     elif isinstance(impute_strategy, list):
         impute_strategy = Choice(impute_strategy)
     if isinstance(svd_components, list):
         svd_components = Choice(svd_components)
 
     def onehot_svd():
-        onehot = decorate(tf.SafeOneHotEncoder(name=f'categorical_onehot_{seq_no}', sparse=False))
+        onehot = decorate(tf.SafeOneHotEncoder(name=f'categorical_onehot_{seq_no}'))
         svd = decorate(tf.TruncatedSVD(n_components=svd_components, name=f'categorical_svd_{seq_no}'))
         optional_svd = Optional(svd, name=f'categorical_optional_svd_{seq_no}', keep_link=True)(onehot)
         return optional_svd
 
     imputer = decorate(tf.SimpleImputer(missing_values=np.nan, strategy=impute_strategy,
                                         name=f'categorical_imputer_{seq_no}', fill_value=''))
```

### Comparing `hypergbm-0.2.5.7/hypergbm/dask/dask_transformers.py` & `hypergbm-0.3.0/hypergbm/dask/dask_transformers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding:utf-8 -*-
 """
 
 """
-
+import inspect
 import numpy as np
 from dask_ml import impute as dimp
 from dask_ml import preprocessing as dm_pre
 
 from hypernets.pipeline.base import HyperTransformer, DataFrameMapper
 from hypernets.pipeline.transformers import AsTypeTransformer, PassThroughEstimator
 from hypernets.tabular.dask_ex import DaskToolBox
@@ -32,24 +32,30 @@
             kwargs['with_mean'] = with_mean
         if with_std is not None and with_std != True:
             kwargs['with_std'] = with_std
         HyperTransformer.__init__(self, dm_pre.StandardScaler, space, name, **kwargs)
 
 
 class SafeOneHotEncoder(HyperTransformer):
-    def __init__(self, categories='auto', drop=None, sparse=True, dtype=np.float64, space=None,
+    def __init__(self, categories='auto', drop=None, dtype=np.float64, space=None,
                  name=None, **kwargs):
         if categories is not None and categories != 'auto':
             kwargs['categories'] = categories
         # else:
         #     kwargs['categories'] = 'object'
         if drop is not None:
             kwargs['drop'] = drop
-        if sparse is not None and sparse != True:
-            kwargs['sparse'] = sparse
+
+        keys = set(inspect.signature(dm_pre.OneHotEncoder.__init__).parameters.keys())
+        if 'sparse_output' in keys:
+            # above sklearn 1.2
+            kwargs['sparse_output'] = False
+        else:
+            kwargs['sparse'] = False
+
         if dtype is not None and dtype != True:
             kwargs['dtype'] = dtype
         # if handle_unknown is not None and handle_unknown != 'error':
         # kwargs['handle_unknown'] = 'ignore' #fixme
 
         # HyperTransformer.__init__(self, dpre.OneHotEncoder, space, name, **kwargs)
         HyperTransformer.__init__(self, DaskToolBox.transformers['SafeOneHotEncoder'], space, name, **kwargs)
```

### Comparing `hypergbm-0.2.5.7/hypergbm/dask/search_space.py` & `hypergbm-0.3.0/hypergbm/dask/search_space.py`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/estimators.py` & `hypergbm-0.3.0/hypergbm/estimators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # -*- coding:utf-8 -*-
 """
 
 """
 import contextlib
+import inspect
 import os
 
 import catboost
 import lightgbm
 import numpy as np
 import pandas as pd
 import xgboost
 
+from hypergbm.utils.detect_estimator import detect_with_process
 from hypernets.core.search_space import ModuleSpace
 from hypernets.discriminators import UnPromisingTrial
 from hypernets.tabular import get_tool_box
 from hypernets.tabular.cache import cache
 from hypernets.tabular.cfg import TabularCfg as tcfg
 from hypernets.tabular.column_selector import column_object_category_bool, column_zero_or_positive_int32
 from hypernets.utils import const, logging, to_repr, Version
@@ -52,17 +54,17 @@
         # tb = get_tool_box(pd.DataFrame)
         # detected = tb.estimator_detector('lightgbm.LGBMClassifier', const.TASK_BINARY,
         #                                  # init_kwargs={'device': 'GPU', 'verbose': -1},
         #                                  init_kwargs={'device': 'GPU'},
         #                                  fit_kwargs={})()
         # logger.info(f'detect_estimator lightgbm.LGBMClassifier as {detected}')
         # _detected_lgbm_gpu = detected
-        _detected_lgbm_gpu = _tb_detect_estimator('lightgbm.LGBMClassifier', const.TASK_BINARY,
-                                                  init_kwargs={'device': 'GPU', 'verbose': -1},
-                                                  fit_kwargs={})
+        _detected_lgbm_gpu = detect_with_process('lightgbm.LGBMClassifier', const.TASK_BINARY,
+                                                 init_kwargs={'device': 'GPU', 'verbose': -1},
+                                                 fit_kwargs={})
 
     return 'fitted' in _detected_lgbm_gpu
 
 
 def get_categorical_features(X):
     cat_cols = column_object_category_bool(X)
     cat_cols += column_zero_or_positive_int32(X)
@@ -316,14 +318,23 @@
 
         if not kwargs.__contains__('categorical_feature'):
             cat_cols = get_categorical_features(X)
             kwargs['categorical_feature'] = cat_cols if len(cat_cols) > 0 else None
         if kwargs.get('early_stopping_rounds') is None and kwargs.get('eval_set') is not None:
             kwargs['early_stopping_rounds'] = _default_early_stopping_rounds(self)
 
+        lgbm_fit_args = inspect.signature(lightgbm.LGBMClassifier.fit).parameters.keys()
+        if 'verbose' in kwargs.keys() and 'verbose' not in lgbm_fit_args:
+            verbosity = kwargs.pop('verbose')
+            if verbosity == 0:
+                verbosity = -1
+            self.set_params(verbosity=verbosity)
+        if 'early_stopping_rounds' in kwargs.keys() and 'early_stopping_rounds' not in lgbm_fit_args:
+            self.set_params(early_stopping_rounds=kwargs.pop('early_stopping_rounds'))
+
         self.feature_names_in_ = X.columns.tolist()
         return kwargs
 
     def prepare_predict_X(self, X):
         feature_names = self.feature_names_in_
         if feature_names != X.columns.tolist():
             X = X[feature_names]
```

### Comparing `hypergbm-0.2.5.7/hypergbm/examples/00.get-doc.ipynb` & `hypergbm-0.3.0/hypergbm/examples/00.get-doc.ipynb`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/examples/01.quick-start.ipynb` & `hypergbm-0.3.0/hypergbm/examples/01.quick-start.ipynb`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/examples/02.basic-setting.ipynb` & `hypergbm-0.3.0/hypergbm/examples/02.basic-setting.ipynb`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/examples/11.feature_selection.ipynb` & `hypergbm-0.3.0/hypergbm/examples/11.feature_selection.ipynb`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/examples/12.collinearity_detection.ipynb` & `hypergbm-0.3.0/hypergbm/examples/12.collinearity_detection.ipynb`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/examples/13.drift_detection.ipynb` & `hypergbm-0.3.0/hypergbm/examples/13.drift_detection.ipynb`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/examples/14.feature_generation_datetime.ipynb` & `hypergbm-0.3.0/hypergbm/examples/14.feature_generation_datetime.ipynb`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/examples/15.feature_generation_latlong_text.ipynb` & `hypergbm-0.3.0/hypergbm/examples/15.feature_generation_latlong_text.ipynb`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/examples/17.feature_reselection.ipynb` & `hypergbm-0.3.0/hypergbm/examples/17.feature_reselection.ipynb`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/examples/18.pseudo_labeling.ipynb` & `hypergbm-0.3.0/hypergbm/examples/18.pseudo_labeling.ipynb`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/examples/21.classbalance.ipynb` & `hypergbm-0.3.0/hypergbm/examples/21.classbalance.ipynb`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/examples/31.search_space.ipynb` & `hypergbm-0.3.0/hypergbm/examples/31.search_space.ipynb`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/examples/32.customize_estimator.ipynb` & `hypergbm-0.3.0/hypergbm/examples/32.customize_estimator.ipynb`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/examples/51.HyperGBM.ipynb` & `hypergbm-0.3.0/hypergbm/examples/51.HyperGBM.ipynb`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/examples/71.hypergbm_shap.ipynb` & `hypergbm-0.3.0/hypergbm/examples/71.hypergbm_shap.ipynb`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/examples/72.hypegbm_experiment_notebook_visualization.ipynb` & `hypergbm-0.3.0/hypergbm/examples/72.hypegbm_experiment_notebook_visualization.ipynb`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/examples/73.hypergbm_shap_explainer.ipynb` & `hypergbm-0.3.0/hypergbm/examples/73.hypergbm_shap_explainer.ipynb`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/examples/74.hypergbm_experiment_explainer.ipynb` & `hypergbm-0.3.0/hypergbm/examples/74.hypergbm_experiment_explainer.ipynb`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/examples/C01.quick-start-with-RAPIDS(cuDF_cuML).ipynb` & `hypergbm-0.3.0/hypergbm/examples/C01.quick-start-with-RAPIDS(cuDF_cuML).ipynb`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/examples/datasets/Bank/test.csv.gz` & `hypergbm-0.3.0/hypergbm/examples/datasets/Bank/test.csv.gz`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/examples/datasets/Bank/train.csv.gz` & `hypergbm-0.3.0/hypergbm/examples/datasets/Bank/train.csv.gz`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/examples/datasets/Magic/test.csv.gz` & `hypergbm-0.3.0/hypergbm/examples/datasets/Magic/test.csv.gz`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/examples/datasets/Magic/train.csv.gz` & `hypergbm-0.3.0/hypergbm/examples/datasets/Magic/train.csv.gz`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/examples/datasets/Metro_Interstate_Traffic_Volume/data.csv.gz` & `hypergbm-0.3.0/hypergbm/examples/datasets/Metro_Interstate_Traffic_Volume/data.csv.gz`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/examples/datasets/Spambase/test.csv.gz` & `hypergbm-0.3.0/hypergbm/examples/datasets/Spambase/test.csv.gz`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/examples/datasets/Spambase/train.csv.gz` & `hypergbm-0.3.0/hypergbm/examples/datasets/Spambase/train.csv.gz`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/examples/datasets/West_Nile_Virus/test.csv.gz` & `hypergbm-0.3.0/hypergbm/examples/datasets/West_Nile_Virus/test.csv.gz`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/examples/datasets/West_Nile_Virus/train.csv.gz` & `hypergbm-0.3.0/hypergbm/examples/datasets/West_Nile_Virus/train.csv.gz`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/examples/datasets/West_Nile_Virus_II/test.csv.gz` & `hypergbm-0.3.0/hypergbm/examples/datasets/West_Nile_Virus_II/test.csv.gz`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/examples/datasets/West_Nile_Virus_II/train.csv.gz` & `hypergbm-0.3.0/hypergbm/examples/datasets/West_Nile_Virus_II/train.csv.gz`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/examples/misc/class_balancing.ipynb` & `hypergbm-0.3.0/hypergbm/examples/misc/class_balancing.ipynb`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/examples/misc/cross_validation.ipynb` & `hypergbm-0.3.0/hypergbm/examples/misc/cross_validation.ipynb`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/examples/misc/drift_detection.ipynb` & `hypergbm-0.3.0/hypergbm/examples/misc/drift_detection.ipynb`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/examples/misc/early_stopping.ipynb` & `hypergbm-0.3.0/hypergbm/examples/misc/early_stopping.ipynb`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/examples/misc/emsemble.ipynb` & `hypergbm-0.3.0/hypergbm/examples/misc/emsemble.ipynb`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/examples/misc/estimators.ipynb` & `hypergbm-0.3.0/hypergbm/examples/misc/estimators.ipynb`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/examples/misc/feature_generation.ipynb` & `hypergbm-0.3.0/hypergbm/examples/misc/feature_generation.ipynb`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/examples/misc/feature_selection.ipynb` & `hypergbm-0.3.0/hypergbm/examples/misc/feature_selection.ipynb`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/examples/misc/hypergbm_shap.ipynb` & `hypergbm-0.3.0/hypergbm/examples/misc/hypergbm_shap.ipynb`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/examples/misc/infer_task_type.ipynb` & `hypergbm-0.3.0/hypergbm/examples/misc/infer_task_type.ipynb`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/examples/misc/pseudo_labeling.ipynb` & `hypergbm-0.3.0/hypergbm/examples/misc/pseudo_labeling.ipynb`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/examples/misc/searchers.ipynb` & `hypergbm-0.3.0/hypergbm/examples/misc/searchers.ipynb`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/experiment.py` & `hypergbm-0.3.0/hypergbm/experiment.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding:utf-8 -*-
 __author__ = 'yangjian'
 
+from hypergbm.objectives import FeatureUsageObjective
 from hypernets.core import Callback
 
 """
 
 """
 import copy
 from typing import List
@@ -38,14 +39,15 @@
                     task=None,
                     id=None,
                     callbacks=None,
                     searcher=None,
                     search_space=None,
                     search_space_options=None,
                     search_callbacks=None,
+                    objectives=None,
                     early_stopping_rounds=10,
                     early_stopping_time_limit=3600,
                     early_stopping_reward=None,
                     reward_metric=None,
                     optimize_direction=None,
                     estimator_early_stopping_rounds=None,
                     hyper_model_cls=None,
@@ -214,24 +216,29 @@
                 create_web_vis_experiment_callback
             search_callbacks.append(create_web_vis_hyper_model_callback())
             callbacks.append(create_web_vis_experiment_callback(**webui_options))
         else:
             logger.warning("No web visualization module detected, please install by command:"
                            "\"pip install hboard\"")
 
+    # objectives
+    objectives_new = None if objectives is None else \
+        list(map(lambda _: FeatureUsageObjective() if _ == 'feature_usage' else _, objectives))
+
     experiment = _make_experiment(hyper_model_cls, train_data,
                                   target=target,
                                   eval_data=eval_data,
                                   test_data=test_data,
                                   task=task,
                                   id=id,
                                   callbacks=callbacks,
                                   searcher=searcher,
                                   search_space=search_space,
                                   search_callbacks=search_callbacks,
+                                  objectives=objectives_new,
                                   early_stopping_rounds=early_stopping_rounds,
                                   early_stopping_time_limit=early_stopping_time_limit,
                                   early_stopping_reward=early_stopping_reward,
                                   reward_metric=reward_metric,
                                   optimize_direction=optimize_direction,
                                   clear_cache=clear_cache,
                                   discriminator=discriminator,
```

### Comparing `hypergbm-0.2.5.7/hypergbm/experiment_callbacks/_hyper_model.py` & `hypergbm-0.3.0/hypergbm/experiment_callbacks/_hyper_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,14 +122,15 @@
             payload = {
                 'stepIndex': self.current_running_step_index,
                 'data': early_stopping_data.to_dict()
             }
             self.send_action(ActionType.EarlyStopped, payload)
 
     def on_trial_end(self, hyper_model, space, trial_no, reward, improved, elapsed):
+        reward = reward[0]
         self.assert_ready()
         trial_event_data = _parse_trial_end_event(hyper_model, space, trial_no, reward, improved, elapsed,
                                                   self.max_trials, self.current_running_step_index)
         self.send_action(ActionType.TrialEnd, trial_event_data)
 
 
 def create_notebook_hyper_model_callback():
```

### Comparing `hypergbm-0.2.5.7/hypergbm/gbm_callbacks/_base.py` & `hypergbm-0.3.0/hypergbm/gbm_callbacks/_base.py`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/gbm_callbacks/_catboost_callbacks.py` & `hypergbm-0.3.0/hypergbm/gbm_callbacks/_catboost_callbacks.py`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/gbm_callbacks/_xgboost_callbacks.py` & `hypergbm-0.3.0/hypergbm/gbm_callbacks/_xgboost_callbacks.py`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/hyper_gbm.py` & `hypergbm-0.3.0/hypergbm/hyper_gbm.py`

 * *Files 3% similar despite different names*

```diff
@@ -267,14 +267,18 @@
 
         if metrics is None:
             metrics = [self.reward_metric] if self.reward_metric is not None else ['accuracy']
 
         oof_ = []
         oof_scores = []
         cv_models_ = []
+        x_vals = []
+        y_vals = []
+        X_trains = []
+        y_trains = []
         self.pos_label = pos_label
         if pbar is not None:
             pbar.set_description('cross_validation')
         sel = tb.select_1d
         for n_fold, (train_idx, valid_idx) in enumerate(iterators.split(X, y)):
             if verbose > 0:
                 logger.info(f'fold {n_fold} started, memory free:{tb.memory_free() / GB:.3f}')
@@ -325,17 +329,23 @@
 
             if verbose > 0:
                 logger.info(f'fold {n_fold} get scores')
             fold_scores = self.get_scores(y_val_fold, proba, metrics)
             oof_scores.append(fold_scores)
             oof_.append((valid_idx, proba))
             cv_models_.append(fold_est)
+            x_vals.append(x_val_fold)
+            y_vals.append(y_val_fold)
+
+            X_trains.append(x_train_fold)
+            y_trains.append(y_train_fold)
 
             del fit_kwargs, sample_weight
-            del x_train_fold, y_train_fold, x_val_fold, y_val_fold, proba
+            # del x_train_fold, y_train_fold, proba
+            del proba
             tb.gc()
 
             if verbose > 0:
                 logger.info(f'fold {n_fold} done with {time.time() - fold_start_at} seconds')
             if pbar is not None:
                 pbar.update(1)
 
@@ -347,15 +357,15 @@
         scores = self.get_scores(y, oof_, metrics)
         if verbose > 0:
             logger.info(f'taken {time.time() - starttime}s')
 
         self.cv_ = True
         self.cv_models_ = cv_models_
 
-        return scores, oof_, oof_scores
+        return scores, oof_, oof_scores, X_trains, y_trains, x_vals, y_vals
 
     def get_scores(self, y, oof_, metrics):
         tb = get_tool_box(y)
         y, proba = tb.select_valid_oof(y, oof_)
         if self.task == const.TASK_REGRESSION:
             preds = proba
             proba = None
```

### Comparing `hypergbm-0.2.5.7/hypergbm/job.py` & `hypergbm-0.3.0/hypergbm/job.py`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/search_space.py` & `hypergbm-0.3.0/hypergbm/search_space.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,17 +8,20 @@
 from hypergbm.estimators import LightGBMEstimator, XGBoostEstimator, CatBoostEstimator, HistGBEstimator
 from hypergbm.estimators import detect_lgbm_gpu
 from hypergbm.sklearn.sklearn_ops import numeric_pipeline_simple, numeric_pipeline_complex, \
     categorical_pipeline_simple, categorical_pipeline_complex, \
     datetime_pipeline_simple, text_pipeline_simple
 from hypernets.core import randint
 from hypernets.core.ops import ModuleChoice, HyperInput
-from hypernets.core.search_space import HyperSpace, Choice, Int
+from hypernets.core.search_space import HyperSpace, Choice, Int, Real
 from hypernets.pipeline.base import DataFrameMapper
 from hypernets.tabular.column_selector import column_object
+from hypernets.pipeline.transformers import FeatureImportanceSelection
+from hypernets.tabular import column_selector
+
 from hypernets.utils import logging, get_params
 
 logger = logging.get_logger(__name__)
 
 
 def _merge_dict(*args):
     d = {}
@@ -45,23 +48,32 @@
         super().__init__()
 
         self.options = kwargs
 
     def create_preprocessor(self, hyper_input, options):
         raise NotImplementedError()
 
+    def create_feature_selection(self, hyper_input, options):
+        return None
+
     def create_estimators(self, hyper_input, options):
         raise NotImplementedError()
 
     def __call__(self, *args, **kwargs):
         space = HyperSpace()
         with space.as_default():
             options = _merge_dict(self.options, kwargs)
             hyper_input = HyperInput(name='input1')
-            self.create_estimators(self.create_preprocessor(hyper_input, options), options)
+
+            if "importances" in options and options["importances"] is not None:
+                importances = options.pop("importances")
+                ss = self.create_feature_selection(hyper_input, importances)
+                self.create_estimators(self.create_preprocessor(ss, options), options)
+            else:
+                self.create_estimators(self.create_preprocessor(hyper_input, options), options)
             space.set_inputs(hyper_input)
 
         return space
 
     def __repr__(self):
         params = get_params(self)
         params.update(self.options)
@@ -140,14 +152,27 @@
         if unused:
             for c in creators:
                 c.estimator_fit_kwargs.update(unused)
 
         estimators = [c() for c in creators]
         return ModuleChoice(estimators, name='estimator_options')(hyper_input)
 
+    def create_feature_selection(self, hyper_input, importances, seq_no=0):
+        from hypernets.pipeline.base import Pipeline
+        selection = FeatureImportanceSelection(name=f'feature_importance_selection_{seq_no}',
+                                               importances=importances,
+                                               quantile=Real(0, 1, step=0.1))
+        pipeline = Pipeline([selection],
+                            name=f'feature_selection_{seq_no}',
+                            columns=column_selector.column_all)(hyper_input)
+
+        preprocessor = DataFrameMapper(default=False, input_df=True, df_out=True,
+                                       df_out_dtype_transforms=None)([pipeline])
+        return preprocessor
+
 
 class GeneralSearchSpaceGenerator(BaseSearchSpaceGenerator):
     def __init__(self, enable_lightgbm=True, enable_xgb=True, enable_catboost=True, enable_histgb=False, **kwargs):
         super(GeneralSearchSpaceGenerator, self).__init__(**kwargs)
 
         self.enable_lightgbm = enable_lightgbm
         self.enable_xgb = enable_xgb
```

### Comparing `hypergbm-0.2.5.7/hypergbm/sklearn/sklearn_ops.py` & `hypergbm-0.3.0/hypergbm/sklearn/sklearn_ops.py`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/tests/cuml_/experiment_test.py` & `hypergbm-0.3.0/hypergbm/tests/cuml_/experiment_test.py`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/tests/cuml_/hypergbm_test.py` & `hypergbm-0.3.0/hypergbm/tests/cuml_/hypergbm_test.py`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/tests/cuml_/run_experiment_cuml.py` & `hypergbm-0.3.0/hypergbm/tests/cuml_/run_experiment_cuml.py`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/tests/cuml_/run_hypergbm_cuml.py` & `hypergbm-0.3.0/hypergbm/tests/cuml_/run_hypergbm_cuml.py`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/tests/dask_/run_hypergbm_dask.py` & `hypergbm-0.3.0/hypergbm/tests/dask_/run_hypergbm_dask.py`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/tests/estimator_test.py` & `hypergbm-0.3.0/hypergbm/tests/estimator_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from hypergbm.sklearn.sklearn_ops import categorical_pipeline_simple, numeric_pipeline_simple, \
     categorical_pipeline_complex, numeric_pipeline_complex
 from hypernets.core.ops import HyperInput, Choice, ModuleChoice
 from hypernets.core.search_space import HyperSpace, Real
 from hypernets.pipeline.base import DataFrameMapper
 from hypernets.tabular import get_tool_box
 from hypernets.tabular.datasets import dsutils
+from hypernets.utils import Version
 
 
 def get_space_multi_dataframemapper(default=False):
     space = HyperSpace()
     with space.as_default():
         input = HyperInput(name='input1')
         p1 = numeric_pipeline_simple(seq_no=0)(input)
@@ -129,16 +130,20 @@
     def test_lightgbm_early_stoping(self):
         df = dsutils.load_bank().head(1000)
         y = df.pop('y')
 
         X = get_tool_box(df).general_preprocessor(df).fit_transform(df)
         X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.3, stratify=y, random_state=9527)
         import lightgbm as lgbm
-        clf = lgbm.LGBMClassifier(n_estimators=1000)
-        clf.fit(X_train, y_train, eval_set=[(X_test, y_test)], early_stopping_rounds=5)
+        if Version(lgbm.__version__) >= Version('4.0.0'):
+            clf = lgbm.LGBMClassifier(n_estimators=1000, early_stopping_rounds=5)
+            clf.fit(X_train, y_train, eval_set=[(X_test, y_test)])
+        else:
+            clf = lgbm.LGBMClassifier(n_estimators=1000)
+            clf.fit(X_train, y_train, eval_set=[(X_test, y_test)], early_stopping_rounds=5)
 
         assert clf.best_iteration_ == 11
 
         clf = lgbm.LGBMClassifier(n_estimators=clf.best_iteration_)
         clf.fit(X_train, y_train)
         assert clf.booster_.params['num_iterations'] == 11
```

### Comparing `hypergbm-0.2.5.7/hypergbm/tests/experiment_test.py` & `hypergbm-0.3.0/hypergbm/tests/experiment_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from sklearn.model_selection import train_test_split
 
 from hypergbm import HyperGBM, CompeteExperiment
 from hypergbm.search_space import search_space_general, GeneralSearchSpaceGenerator
 from hypernets.core import OptimizeDirection, EarlyStoppingCallback
 from hypernets.experiment import GeneralExperiment, ExperimentCallback, ConsoleCallback, StepNames
 from hypernets.searchers import RandomSearcher
+from hypernets.tabular.feature_generators import is_feature_generator_ready
 
 from hypergbm import make_experiment
 from hypergbm.experiment import PipelineKernelExplainer, PipelineTreeExplainer
 from hypernets.tabular.datasets import dsutils
 
 from hypergbm.tests.hypergbm_test import TestShapExplainer
 
@@ -250,14 +251,15 @@
         self.run_binary(train_test_split_strategy='adversarial_validation')
 
     def test_binary_cross_validator(self):
         from hypernets.tabular.lifelong_learning import PrequentialSplit
         preq_split = PrequentialSplit(PrequentialSplit.STRATEGY_PREQ_BLS, n_splits=3)
         self.run_binary(cv=True, cross_validator=preq_split)
 
+    @pytest.mark.skipif(not is_feature_generator_ready, reason='feature_generator is not ready')
     def test_feature_generation(self):
         from hypernets.tabular.cfg import TabularCfg as tcfg
         tcfg.tfidf_primitive_output_feature_count = 5
 
         df = dsutils.load_movielens()
         df['genres'] = df['genres'].apply(lambda s: s.replace('|', ' '))
         df['timestamp'] = df['timestamp'].apply(datetime.fromtimestamp)
@@ -346,15 +348,15 @@
         if enable_ensemble:
             ensemble_size = 20
         else:
             ensemble_size = 0
 
         df = dsutils.load_boston()
         df_train, df_test = train_test_split(df, test_size=0.8, random_state=42)
-        
+
         search_space_options = dict(enable_lightgbm=False, enable_xgb=False, enable_catboost=False, enable_histgb=False)
         search_space_options[f'enable_{estimator_type}'] = True
 
         from hypergbm.search_space import GeneralSearchSpaceGenerator
         search_space = GeneralSearchSpaceGenerator(**search_space_options)
 
         experiment = make_experiment(df_train, target='target',
@@ -484,7 +486,44 @@
                 tree_values_list = self.run_tree_explainer(estimator, df_test, model_indexes=[max_weight_index])
                 assert len(tree_values_list) == 1
                 assert_shap_value(tree_values_list[0])
             else:
                 tree_values_list = self.run_tree_explainer(estimator, df_test, model_indexes=None)
                 # tree_values_list[0].shape=(3617,1)
                 assert_shap_value(tree_values_list)
+
+
+class TestObjectives:
+
+    def test_feature_usage(self):
+
+        from hypergbm import make_experiment
+
+        from hypernets.tabular import get_tool_box
+        from hypernets.tabular.datasets import dsutils
+        from hypernets.core.random_state import get_random_state
+
+        # hyn_logging.set_level(hyn_logging.WARN)
+        random_state = get_random_state()
+
+        df = dsutils.load_bank().head(1000)
+        tb = get_tool_box(df)
+        df_train, df_test = tb.train_test_split(df, test_size=0.2, random_state=9527)
+        experiment = make_experiment(df_train,
+                                     eval_data=df_test.copy(),
+                                     callbacks=[],
+                                     cv=False,
+                                     num_folds=3,
+                                     random_state=1234,
+                                     search_callbacks=[],
+                                     target='y',
+                                     searcher='nsga2',  # available MOO searcher: moead, nsga2, rnsga2
+                                     searcher_options={'population_size': 3},
+                                     reward_metric='logloss',
+                                     objectives=['feature_usage'],
+                                     early_stopping_rounds=10)
+
+        estimators = experiment.run(max_trials=5)
+        hyper_model = experiment.hyper_model_
+
+        assert hyper_model.history.get_best() is not None
+
```

### Comparing `hypergbm-0.2.5.7/hypergbm/tests/hyperboard_test.py` & `hypergbm-0.3.0/hypergbm/tests/hyperboard_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,94 +6,92 @@
 from hypernets.utils import logging
 from hypernets.tests.experiment import experiment_factory
 
 from hypergbm.experiment_callbacks import create_web_vis_experiment_callback, create_notebook_experiment_callback, \
     create_notebook_hyper_model_callback, create_web_vis_hyper_model_callback
 from hypergbm import make_experiment
 
-
 logger = logging.get_logger(__name__)
 
 
 def _notebook_widget_and_web_app_ready():
     try:
         import hboard
         import hboard_widget
         return True
     except:
         return False
 
 
-deps_ready = pytest.mark.skipif(not _notebook_widget_and_web_app_ready(),
-                                reason='hboard or hboard-widget not installed')
+need_hboard = pytest.mark.skipif(not _notebook_widget_and_web_app_ready(),
+                                 reason='hboard or hboard-widget not installed')
 
 
 def _run_experiment(creator):
     webui_model_callback = create_web_vis_hyper_model_callback()
     webui_callback = create_web_vis_experiment_callback(exit_web_server_on_finish=True)
     nb_model_callback = create_notebook_hyper_model_callback()
     nb_callback = create_notebook_experiment_callback()
 
     exp = creator(maker=make_experiment,
                   callbacks=[webui_callback, nb_callback],
                   search_callbacks=[webui_model_callback, nb_model_callback])
-    estimator = exp.run(max_trials=10)
+    estimator = exp.run(max_trials=3)
     assert estimator
-    
     logfile = webui_callback.get_log_file(exp)
     assert logfile
     with open(logfile, 'r', newline='\n') as f:
         events = [json.loads(line) for line in f.readlines()]
 
     assert events
     assert len(events) > 0
     return events
 
 
-@deps_ready
+@need_hboard
 def test_data_clean():
     _run_experiment(experiment_factory.create_data_clean_experiment)
 
 
-@deps_ready
+@need_hboard
 def test_drift_detection():
     _run_experiment(experiment_factory.create_drift_detection_experiment)
 
 
-@deps_ready
+@need_hboard
 def test_multicollinearity_detect():
     _run_experiment(experiment_factory.create_multicollinearity_detect_experiment)
 
 
-@deps_ready
+@need_hboard
 def test_feature_generation():
     _run_experiment(experiment_factory.create_feature_generation_experiment)
 
 
-@deps_ready
+@need_hboard
 def test_feature_reselection_experiment():
     _run_experiment(experiment_factory.create_feature_reselection_experiment)
 
 
-@deps_ready
+@need_hboard
 def test_feature_selection_experiment():
     _run_experiment(experiment_factory.create_feature_selection_experiment)
 
 
-@deps_ready
+@need_hboard
 def test_pseudo_labeling_experiment():
     _run_experiment(experiment_factory.create_pseudo_labeling_experiment)
 
 
-@deps_ready
+@need_hboard
 def test_disable_cv():
     _run_experiment(experiment_factory.create_disable_cv_experiment)
 
 
-@deps_ready
+@need_hboard
 def test_custom_metric_func():
     _run_experiment(experiment_factory.create_custom_reward_metric_func_experiment)
 
 
-@deps_ready
+@need_hboard
 def test_custom_metric_class():
     _run_experiment(experiment_factory.create_custom_reward_metric_class_experiment)
```

### Comparing `hypergbm-0.2.5.7/hypergbm/tests/hypergbm_test.py` & `hypergbm-0.3.0/hypergbm/tests/hypergbm_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,20 +8,23 @@
 import pytest
 
 from sklearn.model_selection import train_test_split
 
 from hypergbm import HyperGBM
 from hypergbm.estimators import LGBMClassifierWrapper
 from hypergbm.hyper_gbm import HyperGBMShapExplainer
+from hypergbm.objectives import FeatureUsageObjective
 from hypergbm.search_space import search_space_general, GeneralSearchSpaceGenerator
 from hypergbm.tests import test_output_dir
 from hypernets.core import set_random_state
 from hypernets.core.callbacks import SummaryCallback, FileLoggingCallback
 from hypernets.core.searcher import OptimizeDirection
 from hypernets.discriminators import PercentileDiscriminator
+from hypernets.model.objectives import PredictionObjective
+from hypernets.searchers import NSGAIISearcher
 from hypernets.searchers.random_searcher import RandomSearcher
 from hypernets.tabular.datasets import dsutils
 from hypernets.utils import fs
 
 try:
     import shap
     import matplotlib.pyplot as plt
@@ -301,7 +304,37 @@
         self.run_binary(self.validate_train_test_split_model, is_cv=False)
 
     def test_regression_cv_models(self):
         self.run_regression(self.validate_cv_models, is_cv=True)
 
     def test_regression_train_test_split_model(self):
         self.run_regression(self.validate_train_test_split_model, is_cv=False)
+
+
+class TestObjectivesInHyperGBM:
+
+    def test_feature_usage(self):
+        from hypernets.tabular.datasets import dsutils
+        df = dsutils.load_bank().head(1000)
+
+        rs = NSGAIISearcher(search_space_general, objectives=[PredictionObjective.create('accuracy'),
+                                                              FeatureUsageObjective()])
+
+        hk = HyperGBM(rs, task='binary',
+                      reward_metric='accuracy',
+                      callbacks=[SummaryCallback(), FileLoggingCallback(rs, output_dir=f'{test_output_dir}/hyn_logs')])
+        X_train, X_test = train_test_split(df.head(1000), test_size=0.2, random_state=42)
+        target = 'y'
+        y_train = X_train.pop(target)
+        y_test = X_test.pop(target)
+        is_cv = True
+
+        if is_cv:
+            hk.search(X_train, y_train, X_test, y_test, cv=True, num_folds=3, max_trials=2)
+        else:
+            hk.search(X_train, y_train, X_test, y_test, cv=False, max_trials=2)
+
+        best_trials = hk.get_best_trial()
+        assert best_trials
+        best_estimator = best_trials[0].get_model()
+        assert best_estimator.predict(X_test.copy()) is not None
+
```

### Comparing `hypergbm-0.2.5.7/hypergbm/tests/run_experiment.py` & `hypergbm-0.3.0/hypergbm/tests/run_experiment.py`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/tests/run_experiment_explainer.py` & `hypergbm-0.3.0/hypergbm/tests/run_experiment_explainer.py`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/tests/run_explainer.py` & `hypergbm-0.3.0/hypergbm/tests/run_explainer.py`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/tests/run_hypergbm.py` & `hypergbm-0.3.0/hypergbm/tests/run_hypergbm.py`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/tests/run_web_visualization.py` & `hypergbm-0.3.0/hypergbm/tests/run_web_visualization.py`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/tests/search_space_test.py` & `hypergbm-0.3.0/hypergbm/tests/search_space_test.py`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/tests/sklearn_/sklearn_ops_test.py` & `hypergbm-0.3.0/hypergbm/tests/sklearn_/sklearn_ops_test.py`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/tests/utils/tool_test.py` & `hypergbm-0.3.0/hypergbm/tests/utils/tool_test.py`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/utils/cli.py` & `hypergbm-0.3.0/hypergbm/utils/cli.py`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/utils/kendall_tau_test.py` & `hypergbm-0.3.0/hypergbm/utils/kendall_tau_test.py`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm/utils/tool.py` & `hypergbm-0.3.0/hypergbm/utils/tool.py`

 * *Files identical despite different names*

### Comparing `hypergbm-0.2.5.7/hypergbm.egg-info/PKG-INFO` & `hypergbm-0.3.0/hypergbm.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypergbm
-Version: 0.2.5.7
+Version: 0.3.0
 Summary: A full pipeline AutoML tool integrated various GBM models
 Home-page: https://github.com/DataCanvasIO/HyperGBM
 Author: DataCanvas Community
 Author-email: yangjian@zetyun.com
 License: Apache License 2.0
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -17,22 +17,23 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6.*
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: shap
+Provides-Extra: notebook
 Provides-Extra: board
 Provides-Extra: tests
-Provides-Extra: notebook
-Provides-Extra: shap
-Provides-Extra: dask
 Provides-Extra: zhcn
+Provides-Extra: dask
+Provides-Extra: fg
 Provides-Extra: all
 License-File: LICENSE
 
 <p align="center">
 <img src="https://github.com/DataCanvasIO/HyperGBM/raw/main/docs/static/images/HyperGBM.png" width="500" >
 
 
@@ -61,19 +62,14 @@
 
 Install HyperGBM with `conda` from the channel *conda-forge*:
 
 ```bash
 conda install -c conda-forge hypergbm
 ```
 
-On the Windows system, recommend install pyarrow(required by hypernets) 4.0 or earlier version with HyperGBM:
-
-```bash
-conda install -c conda-forge hypergbm "pyarrow<=4.0"
-```
 
 ### Pip
 
 Install HyperGBM with different `pip` options:
 
 * Typical installation:
 ```bash
@@ -83,15 +79,15 @@
 * To run HyperGBM in JupyterLab/Jupyter notebook, install with command:
 ```bash
 pip install hypergbm[notebook]
 ```
 
 * To support experiment visualization base on web, install with command:
 ```bash
-pip install hypergbm[board]
+pip install hypergbm[board] # Temporarily unavailable in version 0.3.x
 ```
 
 * To run HyperGBM in distributed Dask cluster, install with command:
 ```bash
 pip install hypergbm[dask]
 ```
 
@@ -154,29 +150,50 @@
 
 ## GPU Acceleration
 
 Hypergbm supports full pipeline GPU acceleration, including all steps from data processing to model training. In our experiments, we got a 50x performance improvement!  Most importantly, the model trained on GPU could be deployed to the environment without GPU hardware and software (e.g.,CUDA and cuML), which greatly reduces the cost of model deployment.
 
 ![Gpu Acceleration](https://github.com/DataCanvasIO/HyperGBM/raw/main/docs/static/images/gpu_speedup.png)
 
+## Documents
+
+* [Overview](https://hypergbm.readthedocs.io/en/latest/overview.html)
+* [Installation](https://hypergbm.readthedocs.io/en/latest/installation.html)
+* [Quick Start](https://hypergbm.readthedocs.io/en/latest/quick_start.html)
+* [Examples](https://hypergbm.readthedocs.io/en/latest/example.html)
+* [How-To](https://hypergbm.readthedocs.io/en/latest/how_to.html)
+* [Release Notes](https://hypergbm.readthedocs.io/en/latest/release_note.html)
+
 ## HyperGBM related projects
 * [Hypernets](https://github.com/DataCanvasIO/Hypernets): A general automated machine learning (AutoML) framework.
 * [HyperGBM](https://github.com/DataCanvasIO/HyperGBM): A full pipeline AutoML tool integrated various GBM models.
 * [HyperDT/DeepTables](https://github.com/DataCanvasIO/DeepTables): An AutoDL tool for tabular data.
 * [HyperTS](https://github.com/DataCanvasIO/HyperTS): A full pipeline AutoML&AutoDL tool for time series datasets.
 * [HyperKeras](https://github.com/DataCanvasIO/HyperKeras): An AutoDL tool for Neural Architecture Search and Hyperparameter Optimization on Tensorflow and Keras.
 * [HyperBoard](https://github.com/DataCanvasIO/HyperBoard): A visualization tool for Hypernets.
 * [Cooka](https://github.com/DataCanvasIO/Cooka): Lightweight interactive AutoML system.
 
-![DataCanvas AutoML Toolkit](https://github.com/DataCanvasIO/HyperGBM/raw/main/docs/static/images/DAT_logo.png)
+![DataCanvas AutoML Toolkit](https://raw.githubusercontent.com/DataCanvasIO/HyperGBM/main/docs/static/images/DAT_latest.png)
+
+## Citation
+
+If you use HyperGBM in your research, please cite us as follows:
+
+   Jian Yang, Xuefeng Li, Haifeng Wu. 
+   **HyperGBM: A full pipeline AutoML tool integrated with various GBM models.** https://github.com/DataCanvasIO/HyperGBM. 2020. Version 0.2.x.
+
+BibTex:
+
+```
+@misc{hypergbm,
+  author={Jian Yang, Xuefeng Li, Haifeng Wu},
+  title={{HyperGBM}: { A Full Pipeline AutoML Tool Integrated With Various GBM Models}},
+  howpublished={https://github.com/DataCanvasIO/HyperGBM},
+  note={Version 0.2.x},
+  year={2020}
+}
+```
 
-## Documents
 
-* [Overview](https://hypergbm.readthedocs.io/en/latest/overview.html)
-* [Installation](https://hypergbm.readthedocs.io/en/latest/installation.html)
-* [Quick Start](https://hypergbm.readthedocs.io/en/latest/quick_start.html)
-* [Examples](https://hypergbm.readthedocs.io/en/latest/example.html)
-* [How-To](https://hypergbm.readthedocs.io/en/latest/how_to.html)
-* [Release Notes](https://hypergbm.readthedocs.io/en/latest/release_note.html)
 
 ## DataCanvas
 HyperGBM is an open source project created by [DataCanvas](https://www.datacanvas.com/).
```

### Comparing `hypergbm-0.2.5.7/hypergbm.egg-info/SOURCES.txt` & `hypergbm-0.3.0/hypergbm.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 hypergbm/_version.py
 hypergbm/cfg.py
 hypergbm/estimators.py
 hypergbm/experiment.py
 hypergbm/gpu_job.py
 hypergbm/hyper_gbm.py
 hypergbm/job.py
+hypergbm/objectives.py
 hypergbm/search_space.py
 hypergbm.egg-info/PKG-INFO
 hypergbm.egg-info/SOURCES.txt
 hypergbm.egg-info/dependency_links.txt
 hypergbm.egg-info/entry_points.txt
 hypergbm.egg-info/not-zip-safe
 hypergbm.egg-info/requires.txt
@@ -37,15 +38,20 @@
 hypergbm/examples/14.feature_generation_datetime.ipynb
 hypergbm/examples/15.feature_generation_latlong_text.ipynb
 hypergbm/examples/17.feature_reselection.ipynb
 hypergbm/examples/18.pseudo_labeling.ipynb
 hypergbm/examples/21.classbalance.ipynb
 hypergbm/examples/31.search_space.ipynb
 hypergbm/examples/32.customize_estimator.ipynb
+hypergbm/examples/33.multiple_objectives.ipynb
 hypergbm/examples/51.HyperGBM.ipynb
+hypergbm/examples/61.NSGAII_example.ipynb
+hypergbm/examples/62.RNSGAII_example.ipynb
+hypergbm/examples/63.MOEAD_example.ipynb
+hypergbm/examples/66.Objectives_example.ipynb
 hypergbm/examples/71.hypergbm_shap.ipynb
 hypergbm/examples/72.hypegbm_experiment_notebook_visualization.ipynb
 hypergbm/examples/73.hypergbm_shap_explainer.ipynb
 hypergbm/examples/74.hypergbm_experiment_explainer.ipynb
 hypergbm/examples/C01.quick-start-with-RAPIDS(cuDF_cuML).ipynb
 hypergbm/examples/datasets/Bank/test.csv.gz
 hypergbm/examples/datasets/Bank/train.csv.gz
@@ -101,9 +107,10 @@
 hypergbm/tests/dask_/run_hypergbm_dask.py
 hypergbm/tests/sklearn_/__init__.py
 hypergbm/tests/sklearn_/sklearn_ops_test.py
 hypergbm/tests/utils/__init__.py
 hypergbm/tests/utils/tool_test.py
 hypergbm/utils/__init__.py
 hypergbm/utils/cli.py
+hypergbm/utils/detect_estimator.py
 hypergbm/utils/kendall_tau_test.py
 hypergbm/utils/tool.py
```

### Comparing `hypergbm-0.2.5.7/setup.py` & `hypergbm-0.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 
 version_ns = {}
 execfile(P.join(HERE, 'hypergbm', '_version.py'), version_ns)
 version = version_ns['__version__']
 
 print("__version__=" + version)
 
-MIN_PYTHON_VERSION = '>=3.6.*'
+MIN_PYTHON_VERSION = '>=3.6'
 
 # long_description = open('README.md', encoding='utf-8').read()
 long_description = read_description('README.md')
 
 requires = read_requirements()
 extras_require = read_extra_requirements()
```

