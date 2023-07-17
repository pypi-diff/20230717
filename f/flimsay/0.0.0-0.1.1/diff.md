# Comparing `tmp/flimsay-0.0.0.tar.gz` & `tmp/flimsay-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flimsay-0.0.0.tar", last modified: Fri Jul 14 16:34:42 2023, max compression
+gzip compressed data, was "flimsay-0.1.1.tar", last modified: Mon Jul 17 17:23:37 2023, max compression
```

## Comparing `flimsay-0.0.0.tar` & `flimsay-0.1.1.tar`

### file list

```diff
@@ -1,63 +1,64 @@
-drwxr-xr-x   0 sebastianpaez   (501) staff       (20)        0 2023-07-14 16:34:42.674245 flimsay-0.0.0/
--rw-r--r--   0 sebastianpaez   (501) staff       (20)       47 2023-07-14 16:02:12.000000 flimsay-0.0.0/.gitignore
--rw-r--r--   0 sebastianpaez   (501) staff       (20)      591 2023-07-14 16:02:12.000000 flimsay-0.0.0/.pre-commit-config.yaml
--rw-r--r--   0 sebastianpaez   (501) staff       (20)     7390 2023-07-14 16:34:42.674019 flimsay-0.0.0/PKG-INFO
--rw-r--r--   0 sebastianpaez   (501) staff       (20)     6716 2023-07-14 16:02:12.000000 flimsay-0.0.0/README.md
--rw-r--r--   0 sebastianpaez   (501) staff       (20)     3471 2023-07-14 16:02:12.000000 flimsay-0.0.0/README.qmd
-drwxr-xr-x   0 sebastianpaez   (501) staff       (20)        0 2023-07-14 16:34:42.657042 flimsay-0.0.0/flimsay/
--rw-r--r--   0 sebastianpaez   (501) staff       (20)        0 2023-07-14 16:02:12.000000 flimsay-0.0.0/flimsay/__init__.py
--rw-r--r--   0 sebastianpaez   (501) staff       (20)     8286 2023-07-14 16:02:12.000000 flimsay-0.0.0/flimsay/blib.py
--rw-r--r--   0 sebastianpaez   (501) staff       (20)        1 2023-07-14 16:02:12.000000 flimsay-0.0.0/flimsay/cli.py
--rw-r--r--   0 sebastianpaez   (501) staff       (20)     1014 2023-07-14 16:02:12.000000 flimsay-0.0.0/flimsay/constants.py
--rw-r--r--   0 sebastianpaez   (501) staff       (20)     7017 2023-07-14 16:02:12.000000 flimsay-0.0.0/flimsay/data.py
--rw-r--r--   0 sebastianpaez   (501) staff       (20)     7928 2023-07-14 16:02:12.000000 flimsay-0.0.0/flimsay/features.py
--rw-r--r--   0 sebastianpaez   (501) staff       (20)     1263 2023-07-14 16:02:12.000000 flimsay-0.0.0/flimsay/mass.py
--rw-r--r--   0 sebastianpaez   (501) staff       (20)     1030 2023-07-14 16:02:12.000000 flimsay-0.0.0/flimsay/model.py
-drwxr-xr-x   0 sebastianpaez   (501) staff       (20)        0 2023-07-14 16:34:42.660680 flimsay-0.0.0/flimsay/weights/
--rw-r--r--   0 sebastianpaez   (501) staff       (20)  1750627 2023-07-14 16:02:12.000000 flimsay-0.0.0/flimsay/weights/ccs_model.txt
--rw-r--r--   0 sebastianpaez   (501) staff       (20)  2534003 2023-07-14 16:02:12.000000 flimsay-0.0.0/flimsay/weights/one_over_k0_model.txt
-drwxr-xr-x   0 sebastianpaez   (501) staff       (20)        0 2023-07-14 16:34:42.657649 flimsay-0.0.0/flimsay.egg-info/
--rw-r--r--   0 sebastianpaez   (501) staff       (20)     7390 2023-07-14 16:34:42.000000 flimsay-0.0.0/flimsay.egg-info/PKG-INFO
--rw-r--r--   0 sebastianpaez   (501) staff       (20)     1343 2023-07-14 16:34:42.000000 flimsay-0.0.0/flimsay.egg-info/SOURCES.txt
--rw-r--r--   0 sebastianpaez   (501) staff       (20)        1 2023-07-14 16:34:42.000000 flimsay-0.0.0/flimsay.egg-info/dependency_links.txt
--rw-r--r--   0 sebastianpaez   (501) staff       (20)      237 2023-07-14 16:34:42.000000 flimsay-0.0.0/flimsay.egg-info/requires.txt
--rw-r--r--   0 sebastianpaez   (501) staff       (20)        8 2023-07-14 16:34:42.000000 flimsay-0.0.0/flimsay.egg-info/top_level.txt
--rw-r--r--   0 sebastianpaez   (501) staff       (20)     2519 2023-07-14 16:02:12.000000 flimsay-0.0.0/pyproject.toml
--rw-r--r--   0 sebastianpaez   (501) staff       (20)       38 2023-07-14 16:34:42.674296 flimsay-0.0.0/setup.cfg
-drwxr-xr-x   0 sebastianpaez   (501) staff       (20)        0 2023-07-14 16:34:42.654440 flimsay-0.0.0/tests/
-drwxr-xr-x   0 sebastianpaez   (501) staff       (20)        0 2023-07-14 16:34:42.665244 flimsay-0.0.0/tests/unit_tests/
--rw-r--r--   0 sebastianpaez   (501) staff       (20)     1759 2023-07-14 16:02:12.000000 flimsay-0.0.0/tests/unit_tests/features.py
-drwxr-xr-x   0 sebastianpaez   (501) staff       (20)        0 2023-07-14 16:34:42.666186 flimsay-0.0.0/train/
-drwxr-xr-x   0 sebastianpaez   (501) staff       (20)        0 2023-07-14 16:34:42.666467 flimsay-0.0.0/train/.dvc/
--rw-r--r--   0 sebastianpaez   (501) staff       (20)       26 2023-07-14 16:02:12.000000 flimsay-0.0.0/train/.dvc/.gitignore
--rw-r--r--   0 sebastianpaez   (501) staff       (20)       28 2023-07-14 16:02:12.000000 flimsay-0.0.0/train/.dvc/config
--rw-r--r--   0 sebastianpaez   (501) staff       (20)      139 2023-07-14 16:02:12.000000 flimsay-0.0.0/train/.dvcignore
--rw-r--r--   0 sebastianpaez   (501) staff       (20)       20 2023-07-14 16:02:12.000000 flimsay-0.0.0/train/.gitignore
-drwxr-xr-x   0 sebastianpaez   (501) staff       (20)        0 2023-07-14 16:34:42.666619 flimsay-0.0.0/train/data/
--rw-r--r--   0 sebastianpaez   (501) staff       (20)       83 2023-07-14 16:02:12.000000 flimsay-0.0.0/train/data/.gitignore
--rw-r--r--   0 sebastianpaez   (501) staff       (20)     3113 2023-07-14 16:02:12.000000 flimsay-0.0.0/train/dvc.lock
--rw-r--r--   0 sebastianpaez   (501) staff       (20)     2254 2023-07-14 16:02:12.000000 flimsay-0.0.0/train/dvc.yaml
-drwxr-xr-x   0 sebastianpaez   (501) staff       (20)        0 2023-07-14 16:34:42.670595 flimsay-0.0.0/train/plots/
--rw-r--r--   0 sebastianpaez   (501) staff       (20)        0 2023-07-14 16:02:12.000000 flimsay-0.0.0/train/plots/.gitignore
--rw-r--r--   0 sebastianpaez   (501) staff       (20)    40022 2023-07-14 16:02:12.000000 flimsay-0.0.0/train/plots/ccs_cumulative_error.png
--rw-r--r--   0 sebastianpaez   (501) staff       (20)    17478 2023-07-14 16:02:12.000000 flimsay-0.0.0/train/plots/ccs_error.png
--rw-r--r--   0 sebastianpaez   (501) staff       (20)    28471 2023-07-14 16:02:12.000000 flimsay-0.0.0/train/plots/ccs_feature_importance.png
--rw-r--r--   0 sebastianpaez   (501) staff       (20)       59 2023-07-14 16:02:12.000000 flimsay-0.0.0/train/plots/ccs_metrics.toml
--rw-r--r--   0 sebastianpaez   (501) staff       (20)       60 2023-07-14 16:02:12.000000 flimsay-0.0.0/train/plots/ccs_model_metrics.toml
--rw-r--r--   0 sebastianpaez   (501) staff       (20)   118125 2023-07-14 16:02:12.000000 flimsay-0.0.0/train/plots/ccs_mz_vs_error.png
--rw-r--r--   0 sebastianpaez   (501) staff       (20)    71311 2023-07-14 16:02:12.000000 flimsay-0.0.0/train/plots/ccs_predicted_vs_real.png
--rw-r--r--   0 sebastianpaez   (501) staff       (20)    30423 2023-07-14 16:02:12.000000 flimsay-0.0.0/train/plots/one_over_k0_model_feature_importance.png
--rw-r--r--   0 sebastianpaez   (501) staff       (20)   185052 2023-07-14 16:02:12.000000 flimsay-0.0.0/train/plots/one_over_k0_model_ims_error.png
--rw-r--r--   0 sebastianpaez   (501) staff       (20)    42464 2023-07-14 16:02:12.000000 flimsay-0.0.0/train/plots/one_over_k0_model_ims_error_cumulative.png
--rw-r--r--   0 sebastianpaez   (501) staff       (20)    28422 2023-07-14 16:02:12.000000 flimsay-0.0.0/train/plots/one_over_k0_model_ims_error_hist.png
--rw-r--r--   0 sebastianpaez   (501) staff       (20)    90614 2023-07-14 16:02:12.000000 flimsay-0.0.0/train/plots/one_over_k0_model_ims_pred_vs_true.png
--rw-r--r--   0 sebastianpaez   (501) staff       (20)       66 2023-07-14 16:02:12.000000 flimsay-0.0.0/train/plots/one_over_k0_model_metrics.toml
-drwxr-xr-x   0 sebastianpaez   (501) staff       (20)        0 2023-07-14 16:34:42.671250 flimsay-0.0.0/train/scripts/
--rw-r--r--   0 sebastianpaez   (501) staff       (20)        0 2023-07-14 16:02:12.000000 flimsay-0.0.0/train/scripts/__init__.py
--rw-r--r--   0 sebastianpaez   (501) staff       (20)     4449 2023-07-14 16:02:12.000000 flimsay-0.0.0/train/scripts/dataset_utils.py
--rw-r--r--   0 sebastianpaez   (501) staff       (20)     7037 2023-07-14 16:02:12.000000 flimsay-0.0.0/train/scripts/train_1ok0.py
--rw-r--r--   0 sebastianpaez   (501) staff       (20)     5358 2023-07-14 16:02:12.000000 flimsay-0.0.0/train/scripts/train_ccs.py
-drwxr-xr-x   0 sebastianpaez   (501) staff       (20)        0 2023-07-14 16:34:42.672472 flimsay-0.0.0/train/weights/
--rw-r--r--   0 sebastianpaez   (501) staff       (20)        0 2023-07-14 16:02:12.000000 flimsay-0.0.0/train/weights/.gitignore
--rw-r--r--   0 sebastianpaez   (501) staff       (20)  1750627 2023-07-14 16:02:12.000000 flimsay-0.0.0/train/weights/ccs_model.txt
--rw-r--r--   0 sebastianpaez   (501) staff       (20)  2534003 2023-07-14 16:02:12.000000 flimsay-0.0.0/train/weights/one_over_k0_model.txt
+drwxr-xr-x   0 sebastianpaez   (502) staff       (20)        0 2023-07-17 17:23:37.454033 flimsay-0.1.1/
+-rw-r--r--   0 sebastianpaez   (502) staff       (20)       60 2023-07-17 15:53:38.000000 flimsay-0.1.1/.gitignore
+-rw-r--r--   0 sebastianpaez   (502) staff       (20)      639 2023-07-17 16:29:58.000000 flimsay-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 sebastianpaez   (502) staff       (20)     8531 2023-07-17 17:23:37.448237 flimsay-0.1.1/PKG-INFO
+-rw-r--r--   0 sebastianpaez   (502) staff       (20)     7835 2023-07-17 08:59:32.000000 flimsay-0.1.1/README.md
+-rw-r--r--   0 sebastianpaez   (502) staff       (20)     3846 2023-07-17 10:11:50.000000 flimsay-0.1.1/README.qmd
+drwxr-xr-x   0 sebastianpaez   (502) staff       (20)        0 2023-07-17 17:23:37.413510 flimsay-0.1.1/flimsay/
+-rw-r--r--   0 sebastianpaez   (502) staff       (20)       74 2023-07-17 10:10:51.000000 flimsay-0.1.1/flimsay/__init__.py
+-rw-r--r--   0 sebastianpaez   (502) staff       (20)     9109 2023-07-17 09:22:37.000000 flimsay-0.1.1/flimsay/blib.py
+-rw-r--r--   0 sebastianpaez   (502) staff       (20)      472 2023-07-17 08:34:54.000000 flimsay-0.1.1/flimsay/cli.py
+-rw-r--r--   0 sebastianpaez   (502) staff       (20)     1014 2023-07-14 08:29:17.000000 flimsay-0.1.1/flimsay/constants.py
+-rw-r--r--   0 sebastianpaez   (502) staff       (20)     7017 2023-07-13 22:47:19.000000 flimsay-0.1.1/flimsay/data.py
+-rw-r--r--   0 sebastianpaez   (502) staff       (20)    10778 2023-07-17 06:30:27.000000 flimsay-0.1.1/flimsay/features.py
+-rw-r--r--   0 sebastianpaez   (502) staff       (20)     1320 2023-07-17 05:36:42.000000 flimsay-0.1.1/flimsay/mass.py
+-rw-r--r--   0 sebastianpaez   (502) staff       (20)     2078 2023-07-17 16:24:59.000000 flimsay-0.1.1/flimsay/model.py
+drwxr-xr-x   0 sebastianpaez   (502) staff       (20)        0 2023-07-17 17:23:37.420386 flimsay-0.1.1/flimsay/weights/
+-rw-r--r--   0 sebastianpaez   (502) staff       (20)  1750627 2023-07-17 16:09:46.000000 flimsay-0.1.1/flimsay/weights/ccs_model.txt
+-rw-r--r--   0 sebastianpaez   (502) staff       (20)  2534003 2023-07-17 16:10:39.000000 flimsay-0.1.1/flimsay/weights/one_over_k0_model.txt
+drwxr-xr-x   0 sebastianpaez   (502) staff       (20)        0 2023-07-17 17:23:37.415657 flimsay-0.1.1/flimsay.egg-info/
+-rw-r--r--   0 sebastianpaez   (502) staff       (20)     8531 2023-07-17 17:23:37.000000 flimsay-0.1.1/flimsay.egg-info/PKG-INFO
+-rw-r--r--   0 sebastianpaez   (502) staff       (20)     1384 2023-07-17 17:23:37.000000 flimsay-0.1.1/flimsay.egg-info/SOURCES.txt
+-rw-r--r--   0 sebastianpaez   (502) staff       (20)        1 2023-07-17 17:23:37.000000 flimsay-0.1.1/flimsay.egg-info/dependency_links.txt
+-rw-r--r--   0 sebastianpaez   (502) staff       (20)       44 2023-07-17 17:23:37.000000 flimsay-0.1.1/flimsay.egg-info/entry_points.txt
+-rw-r--r--   0 sebastianpaez   (502) staff       (20)      327 2023-07-17 17:23:37.000000 flimsay-0.1.1/flimsay.egg-info/requires.txt
+-rw-r--r--   0 sebastianpaez   (502) staff       (20)        8 2023-07-17 17:23:37.000000 flimsay-0.1.1/flimsay.egg-info/top_level.txt
+-rw-r--r--   0 sebastianpaez   (502) staff       (20)     3078 2023-07-17 17:02:52.000000 flimsay-0.1.1/pyproject.toml
+-rw-r--r--   0 sebastianpaez   (502) staff       (20)       38 2023-07-17 17:23:37.454216 flimsay-0.1.1/setup.cfg
+drwxr-xr-x   0 sebastianpaez   (502) staff       (20)        0 2023-07-17 17:23:37.406264 flimsay-0.1.1/tests/
+drwxr-xr-x   0 sebastianpaez   (502) staff       (20)        0 2023-07-17 17:23:37.425155 flimsay-0.1.1/tests/unit_tests/
+-rw-r--r--   0 sebastianpaez   (502) staff       (20)     2773 2023-07-17 16:28:12.000000 flimsay-0.1.1/tests/unit_tests/test_features.py
+-rw-r--r--   0 sebastianpaez   (502) staff       (20)     2336 2023-07-17 16:28:29.000000 flimsay-0.1.1/tests/unit_tests/test_model.py
+drwxr-xr-x   0 sebastianpaez   (502) staff       (20)        0 2023-07-17 17:23:37.432263 flimsay-0.1.1/train/
+drwxr-xr-x   0 sebastianpaez   (502) staff       (20)        0 2023-07-17 17:23:37.433192 flimsay-0.1.1/train/.dvc/
+-rw-r--r--   0 sebastianpaez   (502) staff       (20)       26 2023-07-10 16:32:37.000000 flimsay-0.1.1/train/.dvc/.gitignore
+-rw-r--r--   0 sebastianpaez   (502) staff       (20)       28 2023-07-13 21:12:46.000000 flimsay-0.1.1/train/.dvc/config
+-rw-r--r--   0 sebastianpaez   (502) staff       (20)      139 2023-07-10 16:32:37.000000 flimsay-0.1.1/train/.dvcignore
+-rw-r--r--   0 sebastianpaez   (502) staff       (20)       20 2023-07-13 18:07:29.000000 flimsay-0.1.1/train/.gitignore
+drwxr-xr-x   0 sebastianpaez   (502) staff       (20)        0 2023-07-17 17:23:37.433847 flimsay-0.1.1/train/data/
+-rw-r--r--   0 sebastianpaez   (502) staff       (20)       83 2023-07-14 05:54:25.000000 flimsay-0.1.1/train/data/.gitignore
+-rw-r--r--   0 sebastianpaez   (502) staff       (20)     3113 2023-07-17 16:12:22.000000 flimsay-0.1.1/train/dvc.lock
+-rw-r--r--   0 sebastianpaez   (502) staff       (20)     2254 2023-07-14 06:01:48.000000 flimsay-0.1.1/train/dvc.yaml
+drwxr-xr-x   0 sebastianpaez   (502) staff       (20)        0 2023-07-17 17:23:37.441917 flimsay-0.1.1/train/plots/
+-rw-r--r--   0 sebastianpaez   (502) staff       (20)        0 2023-07-13 21:15:52.000000 flimsay-0.1.1/train/plots/.gitignore
+-rw-r--r--   0 sebastianpaez   (502) staff       (20)    40022 2023-07-17 16:09:48.000000 flimsay-0.1.1/train/plots/ccs_cumulative_error.png
+-rw-r--r--   0 sebastianpaez   (502) staff       (20)    17478 2023-07-17 16:09:47.000000 flimsay-0.1.1/train/plots/ccs_error.png
+-rw-r--r--   0 sebastianpaez   (502) staff       (20)    28471 2023-07-17 16:09:47.000000 flimsay-0.1.1/train/plots/ccs_feature_importance.png
+-rw-r--r--   0 sebastianpaez   (502) staff       (20)       60 2023-07-17 16:09:48.000000 flimsay-0.1.1/train/plots/ccs_model_metrics.toml
+-rw-r--r--   0 sebastianpaez   (502) staff       (20)   118125 2023-07-17 16:09:47.000000 flimsay-0.1.1/train/plots/ccs_mz_vs_error.png
+-rw-r--r--   0 sebastianpaez   (502) staff       (20)    71311 2023-07-17 16:09:47.000000 flimsay-0.1.1/train/plots/ccs_predicted_vs_real.png
+-rw-r--r--   0 sebastianpaez   (502) staff       (20)    30423 2023-07-17 16:10:39.000000 flimsay-0.1.1/train/plots/one_over_k0_model_feature_importance.png
+-rw-r--r--   0 sebastianpaez   (502) staff       (20)   185052 2023-07-17 16:10:40.000000 flimsay-0.1.1/train/plots/one_over_k0_model_ims_error.png
+-rw-r--r--   0 sebastianpaez   (502) staff       (20)    42464 2023-07-17 16:10:40.000000 flimsay-0.1.1/train/plots/one_over_k0_model_ims_error_cumulative.png
+-rw-r--r--   0 sebastianpaez   (502) staff       (20)    28422 2023-07-17 16:10:40.000000 flimsay-0.1.1/train/plots/one_over_k0_model_ims_error_hist.png
+-rw-r--r--   0 sebastianpaez   (502) staff       (20)    90614 2023-07-17 16:10:41.000000 flimsay-0.1.1/train/plots/one_over_k0_model_ims_pred_vs_true.png
+-rw-r--r--   0 sebastianpaez   (502) staff       (20)       66 2023-07-17 16:10:41.000000 flimsay-0.1.1/train/plots/one_over_k0_model_metrics.toml
+drwxr-xr-x   0 sebastianpaez   (502) staff       (20)        0 2023-07-17 17:23:37.444532 flimsay-0.1.1/train/scripts/
+-rw-r--r--   0 sebastianpaez   (502) staff       (20)        0 2023-07-14 14:26:09.000000 flimsay-0.1.1/train/scripts/__init__.py
+-rw-r--r--   0 sebastianpaez   (502) staff       (20)     4449 2023-07-14 15:40:08.000000 flimsay-0.1.1/train/scripts/dataset_utils.py
+-rw-r--r--   0 sebastianpaez   (502) staff       (20)     7037 2023-07-14 15:40:08.000000 flimsay-0.1.1/train/scripts/train_1ok0.py
+-rw-r--r--   0 sebastianpaez   (502) staff       (20)     5358 2023-07-14 15:40:08.000000 flimsay-0.1.1/train/scripts/train_ccs.py
+drwxr-xr-x   0 sebastianpaez   (502) staff       (20)        0 2023-07-17 17:23:37.446789 flimsay-0.1.1/train/weights/
+-rw-r--r--   0 sebastianpaez   (502) staff       (20)        0 2023-07-13 18:07:02.000000 flimsay-0.1.1/train/weights/.gitignore
+-rw-r--r--   0 sebastianpaez   (502) staff       (20)  1750627 2023-07-17 16:09:46.000000 flimsay-0.1.1/train/weights/ccs_model.txt
+-rw-r--r--   0 sebastianpaez   (502) staff       (20)  2534003 2023-07-17 16:10:39.000000 flimsay-0.1.1/train/weights/one_over_k0_model.txt
```

### Comparing `flimsay-0.0.0/PKG-INFO` & `flimsay-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: flimsay
-Version: 0.0.0
+Version: 0.1.1
 Summary: A super simple fast IMS predictor
 Author-email: Sebastian Paez <spaez@talus.bio>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/TalusBio/flimsay
 Project-URL: Documentation, https://TalusBio.github.io/flimsay
 Keywords: proteomics,dia,ion mobility
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Requires-Python: <3.11,>=3.9
+Requires-Python: <3.12,>=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: plot
+Provides-Extra: build
 Provides-Extra: dev
 
 # Flimsy: Fun/Fast Simple IMS Anyone like You can use.
 Sebastian Paez
 
 This repository implements a very simple LGBM model to predict ion
 mobility from peptides.
@@ -35,18 +36,27 @@
 ```
 
 ``` shell
 $ flimsay fill_blib mylibrary.blib # This will add ion mobility data to a .blib file.
 ```
 
 ``` python
-# ! flimsay fill_blib --help
-# Not yet implemented
+! flimsay fill_blib --help
 ```
 
+
+     Usage: flimsay fill_blib [OPTIONS] BLIB OUT_BLIB
+
+     Add ion mobility prediction to a .blib file.
+
+    ╭─ Options ────────────────────────────────────────────────────────────────────╮
+    │ --overwrite      Whether to overwrite output file, if it exists              │
+    │ --help           Show this message and exit.                                 │
+    ╰──────────────────────────────────────────────────────────────────────────────╯
+
 ### Python
 
 #### Single peptide
 
 ``` python
 from flimsay.model import FlimsayModel
 
@@ -70,15 +80,15 @@
     stripped_sequence_name="Stripped_Seqs",
     calc_masses=True,
     default_charge=2,
 )
 df
 ```
 
-    2023-07-14 07:55:41.608 | WARNING  | flimsay.features:add_features:135 - Charge not provided, using default charge of 2
+    2023-07-17 01:54:10.066 | WARNING  | flimsay.features:add_features:163 - Charge not provided, using default charge of 2
 
 <div>
 <style scoped>
     .dataframe tbody tr th:only-of-type {
         vertical-align: middle;
     }
 &#10;    .dataframe tbody tr th {
@@ -104,31 +114,31 @@
     {'ccs': array([315.32424627, 306.70134752, 314.87268797]),
      'one_over_k0': array([0.78718781, 0.72658194, 0.78525451])}
 
 ## Performance
 
 ### Prediction Performance
 
-![](train/plots/one_over_k0_model_ims_pred_vs_true.png)
+![](https://github.com/TalusBio/flimsay/blob/main/train/plots/one_over_k0_model_ims_pred_vs_true.png)
 
-![](train/plots/ccs_predicted_vs_real.png)
+![](https://github.com/TalusBio/flimsay/blob/main/train/plots/ccs_predicted_vs_real.png)
 
 ### Prediction Speed
 
 #### Single peptide prediction
 
 ``` python
 from flimsay.model import FlimsayModel
 
 model_instance = FlimsayModel()
 
 %timeit model_instance.predict_peptide("MYPEPTIDEK", charge=3)
 ```
 
-    125 µs ± 5.72 µs per loop (mean ± std. dev. of 7 runs, 10,000 loops each)
+    135 µs ± 10.7 µs per loop (mean ± std. dev. of 7 runs, 10,000 loops each)
 
 In my laptop that takes 133 microseconds per peptide, or roughly 7,500
 peptides per second.
 
 #### Batch Prediction
 
 ``` python
@@ -155,15 +165,15 @@
 df = add_features(df, stripped_sequence_name="Stripped_Seqs")
 
 
 # Now we get to run the prediction!
 %timeit model_instance.predict(df)
 ```
 
-    7.15 s ± 547 ms per loop (mean ± std. dev. of 7 runs, 1 loop each)
+    7.79 s ± 1.42 s per loop (mean ± std. dev. of 7 runs, 1 loop each)
 
 In my system every million peptides is predicted in 8.86 seconds, that is
 113,000 per second.
 
 ## Motivation
 
 There is a fair amount of data on CCS and ion mobility of peptides but
@@ -228,7 +238,13 @@
 git clone {this repo}
 cd flimsay/train
 dvc repro
 ```
 
 Running this should automatically download the data, trian the models,
 calculate and update the metrics.
+
+The current version of this repo uses predominantly the data from: -
+Meier, F., Köhler, N.D., Brunner, AD. et al. Deep learning the
+collisional cross sections of the peptide universe from a million
+experimental values. Nat Commun 12, 1185 (2021).
+https://doi.org/10.1038/s41467-021-21352-8
```

### Comparing `flimsay-0.0.0/README.md` & `flimsay-0.1.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -16,18 +16,27 @@
 ```
 
 ``` shell
 $ flimsay fill_blib mylibrary.blib # This will add ion mobility data to a .blib file.
 ```
 
 ``` python
-# ! flimsay fill_blib --help
-# Not yet implemented
+! flimsay fill_blib --help
 ```
 
+
+     Usage: flimsay fill_blib [OPTIONS] BLIB OUT_BLIB
+
+     Add ion mobility prediction to a .blib file.
+
+    ╭─ Options ────────────────────────────────────────────────────────────────────╮
+    │ --overwrite      Whether to overwrite output file, if it exists              │
+    │ --help           Show this message and exit.                                 │
+    ╰──────────────────────────────────────────────────────────────────────────────╯
+
 ### Python
 
 #### Single peptide
 
 ``` python
 from flimsay.model import FlimsayModel
 
@@ -51,15 +60,15 @@
     stripped_sequence_name="Stripped_Seqs",
     calc_masses=True,
     default_charge=2,
 )
 df
 ```
 
-    2023-07-14 07:55:41.608 | WARNING  | flimsay.features:add_features:135 - Charge not provided, using default charge of 2
+    2023-07-17 01:54:10.066 | WARNING  | flimsay.features:add_features:163 - Charge not provided, using default charge of 2
 
 <div>
 <style scoped>
     .dataframe tbody tr th:only-of-type {
         vertical-align: middle;
     }
 &#10;    .dataframe tbody tr th {
@@ -85,31 +94,31 @@
     {'ccs': array([315.32424627, 306.70134752, 314.87268797]),
      'one_over_k0': array([0.78718781, 0.72658194, 0.78525451])}
 
 ## Performance
 
 ### Prediction Performance
 
-![](train/plots/one_over_k0_model_ims_pred_vs_true.png)
+![](https://github.com/TalusBio/flimsay/blob/main/train/plots/one_over_k0_model_ims_pred_vs_true.png)
 
-![](train/plots/ccs_predicted_vs_real.png)
+![](https://github.com/TalusBio/flimsay/blob/main/train/plots/ccs_predicted_vs_real.png)
 
 ### Prediction Speed
 
 #### Single peptide prediction
 
 ``` python
 from flimsay.model import FlimsayModel
 
 model_instance = FlimsayModel()
 
 %timeit model_instance.predict_peptide("MYPEPTIDEK", charge=3)
 ```
 
-    125 µs ± 5.72 µs per loop (mean ± std. dev. of 7 runs, 10,000 loops each)
+    135 µs ± 10.7 µs per loop (mean ± std. dev. of 7 runs, 10,000 loops each)
 
 In my laptop that takes 133 microseconds per peptide, or roughly 7,500
 peptides per second.
 
 #### Batch Prediction
 
 ``` python
@@ -136,15 +145,15 @@
 df = add_features(df, stripped_sequence_name="Stripped_Seqs")
 
 
 # Now we get to run the prediction!
 %timeit model_instance.predict(df)
 ```
 
-    7.15 s ± 547 ms per loop (mean ± std. dev. of 7 runs, 1 loop each)
+    7.79 s ± 1.42 s per loop (mean ± std. dev. of 7 runs, 1 loop each)
 
 In my system every million peptides is predicted in 8.86 seconds, that is
 113,000 per second.
 
 ## Motivation
 
 There is a fair amount of data on CCS and ion mobility of peptides but
@@ -209,7 +218,13 @@
 git clone {this repo}
 cd flimsay/train
 dvc repro
 ```
 
 Running this should automatically download the data, trian the models,
 calculate and update the metrics.
+
+The current version of this repo uses predominantly the data from: -
+Meier, F., Köhler, N.D., Brunner, AD. et al. Deep learning the
+collisional cross sections of the peptide universe from a million
+experimental values. Nat Commun 12, 1185 (2021).
+https://doi.org/10.1038/s41467-021-21352-8
```

### Comparing `flimsay-0.0.0/README.qmd` & `flimsay-0.1.1/README.qmd`

 * *Files 17% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 ---
 title: "Flimsy: Fun/Fast Simple IMS Anyone like You can use."
 author: "Sebastian Paez"
 format:
   gfm
 ---
 
+version = 0.1.1
 
 This repository implements a very simple LGBM model
 to predict ion mobility from peptides.
 
-
 ## Usage
 
 There are two main ways to interact with `flimsay`, one is using python and the other one is using the python api directly.
 
 ### CLI
 
 ```shell
@@ -22,16 +22,15 @@
 ```
 
 ```shell
 $ flimsay fill_blib mylibrary.blib # This will add ion mobility data to a .blib file.
 ```
 
 ```{python}
-# ! flimsay fill_blib --help
-# Not yet implemented
+! flimsay fill_blib --help
 ```
 
 ### Python
 
 #### Single peptide
 
 ```{python}
@@ -63,17 +62,17 @@
 model_instance.predict(df[FEATURE_COLUMNS])
 ```
 
 ## Performance
 
 ### Prediction Performance
 
-![](train/plots/one_over_k0_model_ims_pred_vs_true.png)
+![](https://github.com/TalusBio/flimsay/blob/main/train/plots/one_over_k0_model_ims_pred_vs_true.png)
 
-![](train/plots/ccs_predicted_vs_real.png)
+![](https://github.com/TalusBio/flimsay/blob/main/train/plots/ccs_predicted_vs_real.png)
 
 ### Prediction Speed
 
 #### Single peptide prediction
 
 ```{python}
 from flimsay.model import FlimsayModel
@@ -149,7 +148,10 @@
 git clone {this repo}
 cd flimsay/train
 dvc repro
 ```
 
 Running this should automatically download the data,
 trian the models, calculate and update the metrics.
+
+The current version of this repo uses predominantly the data from:
+- Meier, F., Köhler, N.D., Brunner, AD. et al. Deep learning the collisional cross sections of the peptide universe from a million experimental values. Nat Commun 12, 1185 (2021). https://doi.org/10.1038/s41467-021-21352-8
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `flimsay-0.0.0/flimsay/blib.py` & `flimsay-0.1.1/flimsay/blib.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-import argparse
+import os
+import shutil
 import sqlite3
+from pathlib import Path
 
 import pandas as pd
 from loguru import logger
 
 from .features import FEATURE_COLUMNS, add_features, mz_to_mass
 from .model import FlimsayModel
 
@@ -69,17 +71,49 @@
     numSpecs INTEGER,
     majorVersion INTEGER,
     minorVersion INTEGER
 );
 """
 
 
-def main(blib):
+def fill_blib(
+    blib: os.PathLike,
+    out_blib: os.PathLike,
+    overwrite: bool = False,
+) -> None:
+    """Fill a blib file with predicted ion mobility values.
+
+    Parameters
+    ----------
+    blib : os.PathLike
+        Path to the input blib file.
+    out_blib : os.PathLike
+        Path to the output blib file.
+    overwrite : bool, optional
+        Whether to overwrite the output file if it already exists, by default False
+    """
     pred_model = FlimsayModel()
-    conn = sqlite3.connect(blib)
+
+    out_blib = Path(out_blib)
+    blib = Path(blib)
+
+    if out_blib.exists() and not overwrite:
+        raise FileExistsError("Output file already exists")
+
+    if not blib.exists():
+        raise FileNotFoundError(f"Input file '{blib}' does not exist")
+
+    if not out_blib.parent.exists():
+        out_blib.parent.mkdir(parents=True)
+
+    logger.info("Copying file")
+    shutil.copy(blib, out_blib)
+
+    logger.info("Connecting to database")
+    conn = sqlite3.connect(out_blib)
     cur = conn.cursor()
     logger.info("Reading from file")
     df = pd.read_sql_query("SELECT * FROM RefSpectra", conn)
     logger.info(df.head())
 
     pred_df = df[["id", "peptideSeq", "precursorMZ", "precursorCharge"]].copy()
     pred_df["PeptideSequence"] = pred_df["peptideSeq"]
@@ -125,48 +159,55 @@
         conn,
         if_exists="append",
         index=False,
         schema=REF_SPECTRA_SCHEMA,
     )
 
     logger.info("Updating RetentionTimes Table")
-    rtdf = pd.read_sql_query("SELECT * FROM RetentionTimes", conn)
-
     try:
-        del rtdf["ionMobilityValue"]
-    except KeyError:
-        pass
+        rtdf = pd.read_sql_query("SELECT * FROM RetentionTimes", conn)
+        try:
+            del rtdf["ionMobilityValue"]
+        except KeyError:
+            pass
 
-    rtdf["ionMobility"] = [id_to_imns[x] for x in rtdf["RefSpectraID"]]
-    rtdf["collisionalCrossSectionSqA"] = [id_to_ccs[x] for x in rtdf["RefSpectraID"]]
-    rtdf["ionMobilityType"] = 2
-    rtdf["ionMobilityHighEnergyOffset"] = float(0)
-
-    # Making sure this is a float
-    im_offset = rtdf["ionMobilityHighEnergyOffset"].astype("float64")
-    rtdf["ionMobilityHighEnergyOffset"] = im_offset
-
-    cur.execute("DROP TABLE RetentionTimes")
-    cur.executescript(RT_SCHEMA)
-    rtdf.to_sql(
-        "RetentionTimes",
-        conn,
-        if_exists="replace",
-        index=False,
-        schema=RT_SCHEMA,
-    )
+        rtdf["ionMobility"] = [id_to_imns[x] for x in rtdf["RefSpectraID"]]
+        rtdf["collisionalCrossSectionSqA"] = [
+            id_to_ccs[x] for x in rtdf["RefSpectraID"]
+        ]
+        rtdf["ionMobilityType"] = 2
+        rtdf["ionMobilityHighEnergyOffset"] = float(0)
+
+        # Making sure this is a float
+        im_offset = rtdf["ionMobilityHighEnergyOffset"].astype("float64")
+        rtdf["ionMobilityHighEnergyOffset"] = im_offset
+
+        cur.execute("DROP TABLE RetentionTimes")
+        cur.executescript(RT_SCHEMA)
+        rtdf.to_sql(
+            "RetentionTimes",
+            conn,
+            if_exists="replace",
+            index=False,
+            schema=RT_SCHEMA,
+        )
+
+        logger.debug("Printing header of the new RetentionTimes table")
+        df = pd.read_sql_query("SELECT * FROM RetentionTimes LIMIT 5", conn)
+        logger.debug(df.head())
+    except pd.errors.DatabaseError:
+        logger.warning(
+            "No RetentionTimes table found, will proceed without updating it.",
+        )
 
     # Just a print for sanity checking
-    logger.debug("Printing header of the new table")
+    logger.debug("Printing header of the new RefSpectra table")
     df = pd.read_sql_query("SELECT * FROM RefSpectra LIMIT 5", conn)
     logger.debug(df.head())
 
-    df = pd.read_sql_query("SELECT * FROM RetentionTimes LIMIT 5", conn)
-    logger.debug(df.head())
-
     logger.info("Creating ims info table")
     # Encyclopedia does not write this table, so we add it here
     try:
         cur.executescript("""
             CREATE TABLE IonMobilityTypes (
                 id INTEGER PRIMARY KEY,
                 ionMobilityType VARCHAR(128)
@@ -193,22 +234,7 @@
     cur.execute("DROP TABLE LibInfo")
     cur.executescript(LIBINFO_SCHEMA)
     df.to_sql("LibInfo", conn, if_exists="append", index=False, schema=LIBINFO_SCHEMA)
 
     conn.commit()
     conn.close()
     logger.info("Done!")
-
-
-if __name__ == "__main__":
-    parser = argparse.ArgumentParser(description="Add IMS to BLIB")
-    parser.add_argument("blib", help="BLIB file")
-
-    args, unknown = parser.parse_known_args()
-    if unknown:
-        raise RuntimeError("Unrecognized arguments: ", unknown)
-    else:
-        main(
-            args.blib,
-            one_over_k0_model_file=args.one_over_k0_model_file,
-            ccs_model_file=args.ccs_model_file,
-        )
```

### Comparing `flimsay-0.0.0/flimsay/constants.py` & `flimsay-0.1.1/flimsay/constants.py`

 * *Files identical despite different names*

### Comparing `flimsay-0.0.0/flimsay/data.py` & `flimsay-0.1.1/flimsay/data.py`

 * *Files identical despite different names*

### Comparing `flimsay-0.0.0/flimsay/mass.py` & `flimsay-0.1.1/flimsay/mass.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from .constants import PROTON, STD_AA_MASS, WATER
 
 
-def mz_to_mass(mz, charge):
+def mz_to_mass(mz: float, charge: int) -> float:
     """Calculate the mass of a peptide given its m/z and charge.
 
     Examples
     --------
     >>> mz_to_mass(500.000, 2)
     997.98434993586
     """
     return (mz * charge) - charge * PROTON
 
 
-def mass_to_mz(mass, charge):
+def mass_to_mz(mass: float, charge: int) -> float:
     """Calculate the m/z of a peptide given its mass and charge.
 
     This assumes the charge adduct is a proton.
 
     Examples
     --------
     >>> mass_to_mz(1000.000, 2)
@@ -26,15 +26,15 @@
 
 
 # ACLLPEPTK
 # 1027.5372 = Mass for carbamidomethylated version of the peptide
 # From https://web.expasy.org/peptide_mass/
 
 
-def calc_mass(sequence) -> float:
+def calc_mass(sequence: str) -> float:
     """Calculate the mass of a peptide sequence.
 
     Parameters
     ----------
     sequence : str
         Peptide
 
@@ -50,9 +50,9 @@
     1027.53721747546
     """
     mass = WATER
     for aa in sequence:
         try:
             mass += STD_AA_MASS[aa]
         except KeyError:
-            raise KeyError(f"Unknown amino acid: {aa} in peptide: {sequence}")
+            raise KeyError(f"Unknown amino acid: {aa} in peptide: {sequence}") from None
     return mass
```

### Comparing `flimsay-0.0.0/flimsay/weights/ccs_model.txt` & `flimsay-0.1.1/flimsay/weights/ccs_model.txt`

 * *Files identical despite different names*

### Comparing `flimsay-0.0.0/flimsay/weights/one_over_k0_model.txt` & `flimsay-0.1.1/flimsay/weights/one_over_k0_model.txt`

 * *Files identical despite different names*

### Comparing `flimsay-0.0.0/flimsay.egg-info/PKG-INFO` & `flimsay-0.1.1/flimsay.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: flimsay
-Version: 0.0.0
+Version: 0.1.1
 Summary: A super simple fast IMS predictor
 Author-email: Sebastian Paez <spaez@talus.bio>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/TalusBio/flimsay
 Project-URL: Documentation, https://TalusBio.github.io/flimsay
 Keywords: proteomics,dia,ion mobility
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Requires-Python: <3.11,>=3.9
+Requires-Python: <3.12,>=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: plot
+Provides-Extra: build
 Provides-Extra: dev
 
 # Flimsy: Fun/Fast Simple IMS Anyone like You can use.
 Sebastian Paez
 
 This repository implements a very simple LGBM model to predict ion
 mobility from peptides.
@@ -35,18 +36,27 @@
 ```
 
 ``` shell
 $ flimsay fill_blib mylibrary.blib # This will add ion mobility data to a .blib file.
 ```
 
 ``` python
-# ! flimsay fill_blib --help
-# Not yet implemented
+! flimsay fill_blib --help
 ```
 
+
+     Usage: flimsay fill_blib [OPTIONS] BLIB OUT_BLIB
+
+     Add ion mobility prediction to a .blib file.
+
+    ╭─ Options ────────────────────────────────────────────────────────────────────╮
+    │ --overwrite      Whether to overwrite output file, if it exists              │
+    │ --help           Show this message and exit.                                 │
+    ╰──────────────────────────────────────────────────────────────────────────────╯
+
 ### Python
 
 #### Single peptide
 
 ``` python
 from flimsay.model import FlimsayModel
 
@@ -70,15 +80,15 @@
     stripped_sequence_name="Stripped_Seqs",
     calc_masses=True,
     default_charge=2,
 )
 df
 ```
 
-    2023-07-14 07:55:41.608 | WARNING  | flimsay.features:add_features:135 - Charge not provided, using default charge of 2
+    2023-07-17 01:54:10.066 | WARNING  | flimsay.features:add_features:163 - Charge not provided, using default charge of 2
 
 <div>
 <style scoped>
     .dataframe tbody tr th:only-of-type {
         vertical-align: middle;
     }
 &#10;    .dataframe tbody tr th {
@@ -104,31 +114,31 @@
     {'ccs': array([315.32424627, 306.70134752, 314.87268797]),
      'one_over_k0': array([0.78718781, 0.72658194, 0.78525451])}
 
 ## Performance
 
 ### Prediction Performance
 
-![](train/plots/one_over_k0_model_ims_pred_vs_true.png)
+![](https://github.com/TalusBio/flimsay/blob/main/train/plots/one_over_k0_model_ims_pred_vs_true.png)
 
-![](train/plots/ccs_predicted_vs_real.png)
+![](https://github.com/TalusBio/flimsay/blob/main/train/plots/ccs_predicted_vs_real.png)
 
 ### Prediction Speed
 
 #### Single peptide prediction
 
 ``` python
 from flimsay.model import FlimsayModel
 
 model_instance = FlimsayModel()
 
 %timeit model_instance.predict_peptide("MYPEPTIDEK", charge=3)
 ```
 
-    125 µs ± 5.72 µs per loop (mean ± std. dev. of 7 runs, 10,000 loops each)
+    135 µs ± 10.7 µs per loop (mean ± std. dev. of 7 runs, 10,000 loops each)
 
 In my laptop that takes 133 microseconds per peptide, or roughly 7,500
 peptides per second.
 
 #### Batch Prediction
 
 ``` python
@@ -155,15 +165,15 @@
 df = add_features(df, stripped_sequence_name="Stripped_Seqs")
 
 
 # Now we get to run the prediction!
 %timeit model_instance.predict(df)
 ```
 
-    7.15 s ± 547 ms per loop (mean ± std. dev. of 7 runs, 1 loop each)
+    7.79 s ± 1.42 s per loop (mean ± std. dev. of 7 runs, 1 loop each)
 
 In my system every million peptides is predicted in 8.86 seconds, that is
 113,000 per second.
 
 ## Motivation
 
 There is a fair amount of data on CCS and ion mobility of peptides but
@@ -228,7 +238,13 @@
 git clone {this repo}
 cd flimsay/train
 dvc repro
 ```
 
 Running this should automatically download the data, trian the models,
 calculate and update the metrics.
+
+The current version of this repo uses predominantly the data from: -
+Meier, F., Köhler, N.D., Brunner, AD. et al. Deep learning the
+collisional cross sections of the peptide universe from a million
+experimental values. Nat Commun 12, 1185 (2021).
+https://doi.org/10.1038/s41467-021-21352-8
```

### Comparing `flimsay-0.0.0/flimsay.egg-info/SOURCES.txt` & `flimsay-0.1.1/flimsay.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -10,31 +10,32 @@
 flimsay/data.py
 flimsay/features.py
 flimsay/mass.py
 flimsay/model.py
 flimsay.egg-info/PKG-INFO
 flimsay.egg-info/SOURCES.txt
 flimsay.egg-info/dependency_links.txt
+flimsay.egg-info/entry_points.txt
 flimsay.egg-info/requires.txt
 flimsay.egg-info/top_level.txt
 flimsay/weights/ccs_model.txt
 flimsay/weights/one_over_k0_model.txt
-tests/unit_tests/features.py
+tests/unit_tests/test_features.py
+tests/unit_tests/test_model.py
 train/.dvcignore
 train/.gitignore
 train/dvc.lock
 train/dvc.yaml
 train/.dvc/.gitignore
 train/.dvc/config
 train/data/.gitignore
 train/plots/.gitignore
 train/plots/ccs_cumulative_error.png
 train/plots/ccs_error.png
 train/plots/ccs_feature_importance.png
-train/plots/ccs_metrics.toml
 train/plots/ccs_model_metrics.toml
 train/plots/ccs_mz_vs_error.png
 train/plots/ccs_predicted_vs_real.png
 train/plots/one_over_k0_model_feature_importance.png
 train/plots/one_over_k0_model_ims_error.png
 train/plots/one_over_k0_model_ims_error_cumulative.png
 train/plots/one_over_k0_model_ims_error_hist.png
```

### Comparing `flimsay-0.0.0/pyproject.toml` & `flimsay-0.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 [build-system]
-requires = ["setuptools", "setuptools-scm"]
+requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "flimsay"
+version = "0.1.1"
 authors = [
     {name = "Sebastian Paez", email = "spaez@talus.bio"},
 ]
 description = "A super simple fast IMS predictor"
-requires-python = ">=3.9,<3.11"
+requires-python = ">=3.9,<3.12"
 keywords = ["proteomics", "dia", "ion mobility"]
 license = {text = "Apache 2.0"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering :: Bio-Informatics",
 ]
 dependencies = [
     "pandas >= 2.0.0",
     "numpy == 1.24.0",
     "tqdm >= 4.64.1",
     "loguru >= 0.6.0",
     "lightgbm >= 3.3.5",
+    "rich-click >= 1.6.1",
 ]
-dynamic = ["version"]
 
-# [project.scripts]
-# flimsay = "flimsay.cli:main_cli"
+[project.scripts]
+flimsay = "flimsay.cli:cli"
 
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
 
 [project.urls]
 Homepage = "https://github.com/TalusBio/flimsay"
@@ -43,35 +44,45 @@
     "pytest-datadir >= 1.4.1",
     "pytest-cov >= 4.0.0",
 ]
 plot = [
     "matplotlib",
     "vizta",
 ]
+build = [
+    "nbformat",
+    "nbclient",
+    "ipykernel",
+    "wheel",
+    "build",
+    "twine",
+]
 dev = [
     "ruff >= 0.0.253",
     "black >= 23.1.0",
     "isort >=  5.12.0",
     "pylance >= 0.3.9",
     "jupyter >= 1.0.0",
+    "pip-tools >= 7.0.0"
 ]
 
 [tool.setuptools.packages.find]
 include = ["flimsay"]
 
 [tool.setuptools.package-data]
 flimsay = ["*.txt"]
 
+
 [tool.pytest.ini_options]
 minversion = "6.0"
-addopts = "--doctest-modules -v"
+addopts = "--doctest-modules -v --cov=flimsay"
 doctest_optionflags = "NORMALIZE_WHITESPACE"
 testpaths = [
     "flimsay",
-    "tests",
+    "tests/unit_tests",
 ]
 
 [tool.ruff]
 line-length = 88
 select = ["E", "F", "B","W", "C", "I", "D", "UP", "N", "ANN", "T20", "COM"]
 target-version = "py39"
 
@@ -83,21 +94,39 @@
 # D401 First line of docstring should be in imperative mood
 ignore = ["D213", "ANN101", "D203", "D100", "ANN102", "D401"]
 
 fix = true
 
 [tool.ruff.per-file-ignores]
 "**__init__.py" = ["D104"]
+"tests/**.py" = ["ANN201", "ANN001", "ANN202"]
 
 # ANN001 Missing type annotation for function argument
 # Ignoring in the cli since it is redundant with the click options
 # D103 Missing docstring in public function
 # Information in the help of the click command.
-"diadem/cli.py" = ["ANN001", "D103"]
+"flimsay/cli.py" = ["ANN001", "ANN201", "D103"]
 
 [tool.black]
 line-length = 88
 target-version = ['py39', 'py310', 'py311']
 preview = true
 
 [tool.isort]
 profile = "black"
+
+[tool.bumpver]
+current_version = "0.1.1"
+version_pattern = "MAJOR.MINOR.PATCH"
+commit_message = "bump version {old_version} -> {new_version}"
+commit = true
+tag = true
+push = true
+
+[tool.bumpver.file_patterns]
+"pyproject.toml" = [
+    'current_version = "{version}"',
+    'version = "{version}"',
+]
+"README.qmd" = [
+    "version = {version}",
+]
```

### Comparing `flimsay-0.0.0/train/dvc.lock` & `flimsay-0.1.1/train/dvc.lock`

 * *Files identical despite different names*

### Comparing `flimsay-0.0.0/train/dvc.yaml` & `flimsay-0.1.1/train/dvc.yaml`

 * *Files identical despite different names*

### Comparing `flimsay-0.0.0/train/plots/ccs_cumulative_error.png` & `flimsay-0.1.1/train/plots/ccs_cumulative_error.png`

 * *Files identical despite different names*

### Comparing `flimsay-0.0.0/train/plots/ccs_error.png` & `flimsay-0.1.1/train/plots/ccs_error.png`

 * *Files identical despite different names*

### Comparing `flimsay-0.0.0/train/plots/ccs_feature_importance.png` & `flimsay-0.1.1/train/plots/ccs_feature_importance.png`

 * *Files identical despite different names*

### Comparing `flimsay-0.0.0/train/plots/ccs_mz_vs_error.png` & `flimsay-0.1.1/train/plots/ccs_mz_vs_error.png`

 * *Files identical despite different names*

### Comparing `flimsay-0.0.0/train/plots/ccs_predicted_vs_real.png` & `flimsay-0.1.1/train/plots/ccs_predicted_vs_real.png`

 * *Files identical despite different names*

### Comparing `flimsay-0.0.0/train/plots/one_over_k0_model_feature_importance.png` & `flimsay-0.1.1/train/plots/one_over_k0_model_feature_importance.png`

 * *Files identical despite different names*

### Comparing `flimsay-0.0.0/train/plots/one_over_k0_model_ims_error.png` & `flimsay-0.1.1/train/plots/one_over_k0_model_ims_error.png`

 * *Files identical despite different names*

### Comparing `flimsay-0.0.0/train/plots/one_over_k0_model_ims_error_cumulative.png` & `flimsay-0.1.1/train/plots/one_over_k0_model_ims_error_cumulative.png`

 * *Files identical despite different names*

### Comparing `flimsay-0.0.0/train/plots/one_over_k0_model_ims_error_hist.png` & `flimsay-0.1.1/train/plots/one_over_k0_model_ims_error_hist.png`

 * *Files identical despite different names*

### Comparing `flimsay-0.0.0/train/plots/one_over_k0_model_ims_pred_vs_true.png` & `flimsay-0.1.1/train/plots/one_over_k0_model_ims_pred_vs_true.png`

 * *Files identical despite different names*

### Comparing `flimsay-0.0.0/train/scripts/dataset_utils.py` & `flimsay-0.1.1/train/scripts/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `flimsay-0.0.0/train/scripts/train_1ok0.py` & `flimsay-0.1.1/train/scripts/train_1ok0.py`

 * *Files identical despite different names*

### Comparing `flimsay-0.0.0/train/scripts/train_ccs.py` & `flimsay-0.1.1/train/scripts/train_ccs.py`

 * *Files identical despite different names*

### Comparing `flimsay-0.0.0/train/weights/ccs_model.txt` & `flimsay-0.1.1/train/weights/ccs_model.txt`

 * *Files identical despite different names*

### Comparing `flimsay-0.0.0/train/weights/one_over_k0_model.txt` & `flimsay-0.1.1/train/weights/one_over_k0_model.txt`

 * *Files identical despite different names*

