# Comparing `tmp/CartiMorph_nnUNet-1.7.6.tar.gz` & `tmp/CartiMorph_nnUNet-1.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CartiMorph_nnUNet-1.7.6.tar", last modified: Sat Jul  1 16:05:47 2023, max compression
+gzip compressed data, was "CartiMorph_nnUNet-1.7.7.tar", last modified: Mon Jul 17 08:56:27 2023, max compression
```

## Comparing `CartiMorph_nnUNet-1.7.6.tar` & `CartiMorph_nnUNet-1.7.7.tar`

### file list

```diff
@@ -1,107 +1,108 @@
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-01 16:05:47.993248 CartiMorph_nnUNet-1.7.6/
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-01 16:05:47.969154 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/
--rw-r--r--   0 vincent    (501) staff       (20)      679 2023-07-01 16:05:34.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)      257 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/configuration.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-01 16:05:47.971037 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/dataset_conversion/
--rw-r--r--   0 vincent    (501) staff       (20)       55 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/dataset_conversion/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     3641 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/dataset_conversion/utils.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-01 16:05:47.972121 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/evaluation/
--rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/evaluation/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     2024 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/evaluation/add_mean_dice_to_json.py
--rw-r--r--   0 vincent    (501) staff       (20)    18791 2023-06-30 08:19:24.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/evaluation/evaluator.py
--rw-r--r--   0 vincent    (501) staff       (20)    13031 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/evaluation/metrics.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-01 16:05:47.972707 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/evaluation/model_selection/
--rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/evaluation/model_selection/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     7504 2023-06-30 08:20:42.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/evaluation/model_selection/ensemble.py
--rw-r--r--   0 vincent    (501) staff       (20)    13084 2023-06-30 07:26:20.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/evaluation/model_selection/figure_out_what_to_submit.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-01 16:05:47.974997 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/experiment_planning/
--rw-r--r--   0 vincent    (501) staff       (20)    11084 2023-06-30 08:07:52.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/experiment_planning/DatasetAnalyzer.py
--rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/experiment_planning/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)    10573 2023-06-30 08:09:29.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/experiment_planning/common_utils.py
--rw-r--r--   0 vincent    (501) staff       (20)     8872 2023-06-30 08:16:19.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/experiment_planning/experiment_planner_baseline_2DUNet.py
--rw-r--r--   0 vincent    (501) staff       (20)    26645 2023-06-30 08:15:35.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/experiment_planning/experiment_planner_baseline_3DUNet.py
--rw-r--r--   0 vincent    (501) staff       (20)    10184 2023-06-30 08:17:41.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/experiment_planning/nnUNet_plan_and_preprocess.py
--rw-r--r--   0 vincent    (501) staff       (20)     9703 2023-06-30 08:08:55.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/experiment_planning/utils.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-01 16:05:47.976823 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/inference/
--rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/inference/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     6322 2023-06-30 07:24:14.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/inference/ensemble_predictions.py
--rw-r--r--   0 vincent    (501) staff       (20)    44937 2023-06-30 08:05:12.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/inference/predict.py
--rw-r--r--   0 vincent    (501) staff       (20)    13889 2023-06-30 07:22:30.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/inference/predict_simple.py
--rw-r--r--   0 vincent    (501) staff       (20)    12231 2023-06-30 08:35:08.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/inference/segmentation_export.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-01 16:05:47.978201 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/network_architecture/
--rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/network_architecture/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)    21079 2023-06-30 08:12:26.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/network_architecture/generic_UNet.py
--rw-r--r--   0 vincent    (501) staff       (20)     1673 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/network_architecture/initialization.py
--rw-r--r--   0 vincent    (501) staff       (20)    44034 2023-06-30 08:13:21.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/network_architecture/neural_network.py
--rw-r--r--   0 vincent    (501) staff       (20)     2949 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/paths.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-01 16:05:47.979416 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/postprocessing/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/postprocessing/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)    19155 2023-06-30 08:35:41.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/postprocessing/connected_components.py
--rw-r--r--   0 vincent    (501) staff       (20)     4882 2023-07-01 12:35:01.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/postprocessing/consolidate_postprocessing.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-01 16:05:47.980914 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/preprocessing/
--rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/preprocessing/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     8571 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/preprocessing/cropping.py
--rw-r--r--   0 vincent    (501) staff       (20)    48230 2023-06-30 08:16:03.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/preprocessing/preprocessing.py
--rw-r--r--   0 vincent    (501) staff       (20)    12212 2023-06-30 08:17:17.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/preprocessing/sanity_checks.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-01 16:05:47.982001 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/run/
--rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/run/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     3884 2023-06-30 07:56:39.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/run/default_configuration.py
--rw-r--r--   0 vincent    (501) staff       (20)     2504 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/run/load_pretrained_weights.py
--rw-r--r--   0 vincent    (501) staff       (20)    11918 2023-06-30 08:04:26.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/run/run_training.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-01 16:05:47.982542 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/training/
--rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/training/__init__.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-01 16:05:47.982930 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/training/cascade_stuff/
--rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/training/cascade_stuff/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     6325 2023-06-30 07:59:12.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/training/cascade_stuff/predict_next_stage.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-01 16:05:47.984552 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/training/data_augmentation/
--rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/training/data_augmentation/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     4841 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/training/data_augmentation/custom_transforms.py
--rw-r--r--   0 vincent    (501) staff       (20)    12665 2023-06-30 08:47:23.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/training/data_augmentation/data_augmentation_moreDA.py
--rw-r--r--   0 vincent    (501) staff       (20)    12993 2023-06-30 08:38:21.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/training/data_augmentation/default_data_augmentation.py
--rw-r--r--   0 vincent    (501) staff       (20)     4137 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/training/data_augmentation/downsampling.py
--rw-r--r--   0 vincent    (501) staff       (20)     9029 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/training/data_augmentation/pyramid_augmentations.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-01 16:05:47.984967 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/training/dataloading/
--rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/training/dataloading/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)    33693 2023-06-30 08:37:03.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/training/dataloading/dataset_loading.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-01 16:05:47.985602 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/training/learning_rate/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/training/learning_rate/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)      807 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/training/learning_rate/poly_lr.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-01 16:05:47.987385 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/training/loss_functions/
--rw-r--r--   0 vincent    (501) staff       (20)     1375 2023-06-30 08:39:27.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/training/loss_functions/TopK_loss.py
--rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/training/loss_functions/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)      438 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/training/loss_functions/crossentropy.py
--rw-r--r--   0 vincent    (501) staff       (20)     1679 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/training/loss_functions/deep_supervision.py
--rw-r--r--   0 vincent    (501) staff       (20)    14004 2023-06-30 08:40:47.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/training/loss_functions/dice_loss.py
--rw-r--r--   0 vincent    (501) staff       (20)     7847 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/training/loss_functions/focal_loss.py
--rw-r--r--   0 vincent    (501) staff       (20)     7202 2023-06-30 08:14:47.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/training/model_restore.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-01 16:05:47.989842 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/training/network_training/
--rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/training/network_training/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)    31404 2023-06-30 08:41:20.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/training/network_training/network_trainer.py
--rw-r--r--   0 vincent    (501) staff       (20)    40059 2023-06-30 08:00:59.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/training/network_training/nnUNetTrainer.py
--rw-r--r--   0 vincent    (501) staff       (20)    16163 2023-06-30 08:01:58.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/training/network_training/nnUNetTrainerCascadeFullRes.py
--rw-r--r--   0 vincent    (501) staff       (20)    22788 2023-06-30 08:49:46.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/training/network_training/nnUNetTrainerV2.py
--rw-r--r--   0 vincent    (501) staff       (20)    19734 2023-06-30 08:02:22.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/training/network_training/nnUNetTrainerV2_CascadeFullRes.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-01 16:05:47.990306 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/training/optimizer/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/training/optimizer/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     6465 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/training/optimizer/ranger.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-01 16:05:47.992826 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/utilities/
--rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/utilities/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     1821 2023-07-01 12:36:03.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/utilities/folder_names.py
--rw-r--r--   0 vincent    (501) staff       (20)      990 2023-05-01 14:25:34.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/utilities/nd_softmax.py
--rw-r--r--   0 vincent    (501) staff       (20)      990 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/utilities/one_hot_encoding.py
--rw-r--r--   0 vincent    (501) staff       (20)     1510 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/utilities/set_n_proc_DA.py
--rw-r--r--   0 vincent    (501) staff       (20)     3525 2023-06-30 08:04:03.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/utilities/task_name_id_conversion.py
--rw-r--r--   0 vincent    (501) staff       (20)     1624 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/utilities/tensor_utilities.py
--rw-r--r--   0 vincent    (501) staff       (20)     1175 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/utilities/to_torch.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-01 16:05:47.970512 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet.egg-info/
--rw-r--r--   0 vincent    (501) staff       (20)      434 2023-07-01 16:05:47.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet.egg-info/PKG-INFO
--rw-r--r--   0 vincent    (501) staff       (20)     4229 2023-07-01 16:05:47.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet.egg-info/SOURCES.txt
--rw-r--r--   0 vincent    (501) staff       (20)        1 2023-07-01 16:05:47.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet.egg-info/dependency_links.txt
--rw-r--r--   0 vincent    (501) staff       (20)      571 2023-07-01 16:05:47.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet.egg-info/entry_points.txt
--rw-r--r--   0 vincent    (501) staff       (20)      151 2023-07-01 16:05:47.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet.egg-info/requires.txt
--rw-r--r--   0 vincent    (501) staff       (20)       18 2023-07-01 16:05:47.000000 CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet.egg-info/top_level.txt
--rw-r--r--   0 vincent    (501) staff       (20)    11357 2023-06-30 06:10:04.000000 CartiMorph_nnUNet-1.7.6/LICENSE
--rw-r--r--   0 vincent    (501) staff       (20)      434 2023-07-01 16:05:47.993103 CartiMorph_nnUNet-1.7.6/PKG-INFO
--rw-r--r--   0 vincent    (501) staff       (20)      640 2023-06-30 09:25:54.000000 CartiMorph_nnUNet-1.7.6/README.md
--rw-r--r--   0 vincent    (501) staff       (20)       38 2023-07-01 16:05:47.993292 CartiMorph_nnUNet-1.7.6/setup.cfg
--rwxr-xr-x   0 vincent    (501) staff       (20)     1773 2023-07-01 16:05:25.000000 CartiMorph_nnUNet-1.7.6/setup.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-17 08:56:27.637944 CartiMorph_nnUNet-1.7.7/
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-17 08:56:27.626576 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/
+-rw-r--r--   0 vincent    (501) staff       (20)      673 2023-07-17 08:54:11.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)      257 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/configuration.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-17 08:56:27.627580 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/dataset_conversion/
+-rw-r--r--   0 vincent    (501) staff       (20)       55 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/dataset_conversion/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)     3641 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/dataset_conversion/utils.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-17 08:56:27.628180 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/evaluation/
+-rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/evaluation/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)     2024 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/evaluation/add_mean_dice_to_json.py
+-rw-r--r--   0 vincent    (501) staff       (20)    18791 2023-06-30 08:19:24.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/evaluation/evaluator.py
+-rw-r--r--   0 vincent    (501) staff       (20)    13031 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/evaluation/metrics.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-17 08:56:27.628596 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/evaluation/model_selection/
+-rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/evaluation/model_selection/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)     7504 2023-06-30 08:20:42.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/evaluation/model_selection/ensemble.py
+-rw-r--r--   0 vincent    (501) staff       (20)    13084 2023-06-30 07:26:20.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/evaluation/model_selection/figure_out_what_to_submit.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-17 08:56:27.629709 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/experiment_planning/
+-rw-r--r--   0 vincent    (501) staff       (20)    11084 2023-06-30 08:07:52.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/experiment_planning/DatasetAnalyzer.py
+-rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/experiment_planning/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)    10573 2023-06-30 08:09:29.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/experiment_planning/common_utils.py
+-rw-r--r--   0 vincent    (501) staff       (20)     8872 2023-06-30 08:16:19.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/experiment_planning/experiment_planner_baseline_2DUNet.py
+-rw-r--r--   0 vincent    (501) staff       (20)    26645 2023-06-30 08:15:35.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/experiment_planning/experiment_planner_baseline_3DUNet.py
+-rw-r--r--   0 vincent    (501) staff       (20)    10184 2023-06-30 08:17:41.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/experiment_planning/nnUNet_plan_and_preprocess.py
+-rw-r--r--   0 vincent    (501) staff       (20)     4200 2023-07-17 08:53:19.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/experiment_planning/summarize_plans.py
+-rw-r--r--   0 vincent    (501) staff       (20)     9703 2023-06-30 08:08:55.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/experiment_planning/utils.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-17 08:56:27.630384 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/inference/
+-rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/inference/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)     6322 2023-06-30 07:24:14.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/inference/ensemble_predictions.py
+-rw-r--r--   0 vincent    (501) staff       (20)    44937 2023-06-30 08:05:12.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/inference/predict.py
+-rw-r--r--   0 vincent    (501) staff       (20)    13889 2023-06-30 07:22:30.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/inference/predict_simple.py
+-rw-r--r--   0 vincent    (501) staff       (20)    12231 2023-06-30 08:35:08.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/inference/segmentation_export.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-17 08:56:27.630903 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/network_architecture/
+-rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/network_architecture/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)    21079 2023-06-30 08:12:26.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/network_architecture/generic_UNet.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1673 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/network_architecture/initialization.py
+-rw-r--r--   0 vincent    (501) staff       (20)    44034 2023-06-30 08:13:21.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/network_architecture/neural_network.py
+-rw-r--r--   0 vincent    (501) staff       (20)     2949 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/paths.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-17 08:56:27.631291 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/postprocessing/
+-rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/postprocessing/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)    19155 2023-06-30 08:35:41.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/postprocessing/connected_components.py
+-rw-r--r--   0 vincent    (501) staff       (20)     4882 2023-07-01 12:35:01.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/postprocessing/consolidate_postprocessing.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-17 08:56:27.631823 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/preprocessing/
+-rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/preprocessing/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)     8571 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/preprocessing/cropping.py
+-rw-r--r--   0 vincent    (501) staff       (20)    48230 2023-06-30 08:16:03.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/preprocessing/preprocessing.py
+-rw-r--r--   0 vincent    (501) staff       (20)    12212 2023-06-30 08:17:17.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/preprocessing/sanity_checks.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-17 08:56:27.632321 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/run/
+-rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/run/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)     3884 2023-06-30 07:56:39.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/run/default_configuration.py
+-rw-r--r--   0 vincent    (501) staff       (20)     2504 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/run/load_pretrained_weights.py
+-rw-r--r--   0 vincent    (501) staff       (20)    11918 2023-06-30 08:04:26.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/run/run_training.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-17 08:56:27.632565 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/training/
+-rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/training/__init__.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-17 08:56:27.632807 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/training/cascade_stuff/
+-rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/training/cascade_stuff/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)     6325 2023-06-30 07:59:12.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/training/cascade_stuff/predict_next_stage.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-17 08:56:27.633651 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/training/data_augmentation/
+-rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/training/data_augmentation/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)     4841 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/training/data_augmentation/custom_transforms.py
+-rw-r--r--   0 vincent    (501) staff       (20)    12665 2023-06-30 08:47:23.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/training/data_augmentation/data_augmentation_moreDA.py
+-rw-r--r--   0 vincent    (501) staff       (20)    12993 2023-06-30 08:38:21.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/training/data_augmentation/default_data_augmentation.py
+-rw-r--r--   0 vincent    (501) staff       (20)     4137 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/training/data_augmentation/downsampling.py
+-rw-r--r--   0 vincent    (501) staff       (20)     9029 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/training/data_augmentation/pyramid_augmentations.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-17 08:56:27.633942 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/training/dataloading/
+-rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/training/dataloading/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)    33693 2023-06-30 08:37:03.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/training/dataloading/dataset_loading.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-17 08:56:27.634232 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/training/learning_rate/
+-rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/training/learning_rate/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)      807 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/training/learning_rate/poly_lr.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-17 08:56:27.635100 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/training/loss_functions/
+-rw-r--r--   0 vincent    (501) staff       (20)     1375 2023-06-30 08:39:27.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/training/loss_functions/TopK_loss.py
+-rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/training/loss_functions/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)      438 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/training/loss_functions/crossentropy.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1679 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/training/loss_functions/deep_supervision.py
+-rw-r--r--   0 vincent    (501) staff       (20)    14004 2023-06-30 08:40:47.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/training/loss_functions/dice_loss.py
+-rw-r--r--   0 vincent    (501) staff       (20)     7847 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/training/loss_functions/focal_loss.py
+-rw-r--r--   0 vincent    (501) staff       (20)     7202 2023-06-30 08:14:47.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/training/model_restore.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-17 08:56:27.636050 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/training/network_training/
+-rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/training/network_training/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)    31404 2023-06-30 08:41:20.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/training/network_training/network_trainer.py
+-rw-r--r--   0 vincent    (501) staff       (20)    40059 2023-06-30 08:00:59.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/training/network_training/nnUNetTrainer.py
+-rw-r--r--   0 vincent    (501) staff       (20)    16163 2023-06-30 08:01:58.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/training/network_training/nnUNetTrainerCascadeFullRes.py
+-rw-r--r--   0 vincent    (501) staff       (20)    22788 2023-06-30 08:49:46.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/training/network_training/nnUNetTrainerV2.py
+-rw-r--r--   0 vincent    (501) staff       (20)    19734 2023-06-30 08:02:22.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/training/network_training/nnUNetTrainerV2_CascadeFullRes.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-17 08:56:27.636328 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/training/optimizer/
+-rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/training/optimizer/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)     6465 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/training/optimizer/ranger.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-17 08:56:27.637645 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/utilities/
+-rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/utilities/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1821 2023-07-01 12:36:03.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/utilities/folder_names.py
+-rw-r--r--   0 vincent    (501) staff       (20)      990 2023-05-01 14:25:34.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/utilities/nd_softmax.py
+-rw-r--r--   0 vincent    (501) staff       (20)      990 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/utilities/one_hot_encoding.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1510 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/utilities/set_n_proc_DA.py
+-rw-r--r--   0 vincent    (501) staff       (20)     3525 2023-06-30 08:04:03.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/utilities/task_name_id_conversion.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1624 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/utilities/tensor_utilities.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1175 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/utilities/to_torch.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-17 08:56:27.627311 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet.egg-info/
+-rw-r--r--   0 vincent    (501) staff       (20)      401 2023-07-17 08:56:27.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet.egg-info/PKG-INFO
+-rw-r--r--   0 vincent    (501) staff       (20)     4286 2023-07-17 08:56:27.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet.egg-info/SOURCES.txt
+-rw-r--r--   0 vincent    (501) staff       (20)        1 2023-07-17 08:56:27.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet.egg-info/dependency_links.txt
+-rw-r--r--   0 vincent    (501) staff       (20)      571 2023-07-17 08:56:27.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet.egg-info/entry_points.txt
+-rw-r--r--   0 vincent    (501) staff       (20)      151 2023-07-17 08:56:27.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet.egg-info/requires.txt
+-rw-r--r--   0 vincent    (501) staff       (20)       18 2023-07-17 08:56:27.000000 CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet.egg-info/top_level.txt
+-rw-r--r--   0 vincent    (501) staff       (20)    11357 2023-06-30 06:10:04.000000 CartiMorph_nnUNet-1.7.7/LICENSE
+-rw-r--r--   0 vincent    (501) staff       (20)      401 2023-07-17 08:56:27.637824 CartiMorph_nnUNet-1.7.7/PKG-INFO
+-rw-r--r--   0 vincent    (501) staff       (20)      640 2023-07-05 08:20:41.000000 CartiMorph_nnUNet-1.7.7/README.md
+-rw-r--r--   0 vincent    (501) staff       (20)       38 2023-07-17 08:56:27.637986 CartiMorph_nnUNet-1.7.7/setup.cfg
+-rwxr-xr-x   0 vincent    (501) staff       (20)     1740 2023-07-17 08:56:12.000000 CartiMorph_nnUNet-1.7.7/setup.py
```

### Comparing `CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/__init__.py` & `CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import absolute_import
 
 print("\n\nThis is a modified version of nnU-Net (1.7.0) tailored for the CartiMorph framework (https://github.com/YongchengYAO/CartiMorph).")
 print("\nIf you are using CartiMorph, please cite the paper:")
 print("\nCartiMorph: a framework for automated knee articular cartilage morphometrics")
 
-print("\n\nPlease cite the following paper when using nnUNet:\nIsensee, F., Jaeger, P.F., Kohl, S.A.A. et al. "
+print("\n\nPlease also cite the following nnUNet paper:\nIsensee, F., Jaeger, P.F., Kohl, S.A.A. et al. "
       "\"nnU-Net: a self-configuring method for deep learning-based biomedical image segmentation.\" "
       "Nat Methods (2020). https://doi.org/10.1038/s41592-020-01008-z\n\n")
 
 from . import *
 
 # set version
-__version__ = '1.7.6'
+__version__ = '1.7.7'
```

### Comparing `CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/dataset_conversion/utils.py` & `CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/dataset_conversion/utils.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/evaluation/add_mean_dice_to_json.py` & `CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/evaluation/add_mean_dice_to_json.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/evaluation/evaluator.py` & `CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/evaluation/evaluator.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/evaluation/metrics.py` & `CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/evaluation/metrics.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/evaluation/model_selection/ensemble.py` & `CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/evaluation/model_selection/ensemble.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/evaluation/model_selection/figure_out_what_to_submit.py` & `CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/evaluation/model_selection/figure_out_what_to_submit.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/experiment_planning/DatasetAnalyzer.py` & `CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/experiment_planning/DatasetAnalyzer.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/experiment_planning/common_utils.py` & `CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/experiment_planning/common_utils.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/experiment_planning/experiment_planner_baseline_2DUNet.py` & `CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/experiment_planning/experiment_planner_baseline_2DUNet.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/experiment_planning/experiment_planner_baseline_3DUNet.py` & `CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/experiment_planning/experiment_planner_baseline_3DUNet.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/experiment_planning/nnUNet_plan_and_preprocess.py` & `CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/experiment_planning/nnUNet_plan_and_preprocess.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/experiment_planning/utils.py` & `CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/experiment_planning/utils.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/inference/ensemble_predictions.py` & `CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/inference/ensemble_predictions.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/inference/predict.py` & `CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/inference/predict.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/inference/predict_simple.py` & `CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/inference/predict_simple.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/inference/segmentation_export.py` & `CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/inference/segmentation_export.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/network_architecture/generic_UNet.py` & `CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/network_architecture/generic_UNet.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/network_architecture/initialization.py` & `CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/network_architecture/initialization.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/network_architecture/neural_network.py` & `CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/network_architecture/neural_network.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/paths.py` & `CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/paths.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/postprocessing/connected_components.py` & `CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/postprocessing/connected_components.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/postprocessing/consolidate_postprocessing.py` & `CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/postprocessing/consolidate_postprocessing.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/preprocessing/cropping.py` & `CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/preprocessing/cropping.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/preprocessing/preprocessing.py` & `CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/preprocessing/preprocessing.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/preprocessing/sanity_checks.py` & `CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/preprocessing/sanity_checks.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/run/default_configuration.py` & `CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/run/default_configuration.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/run/load_pretrained_weights.py` & `CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/run/load_pretrained_weights.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/run/run_training.py` & `CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/run/run_training.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/training/cascade_stuff/predict_next_stage.py` & `CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/training/cascade_stuff/predict_next_stage.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/training/data_augmentation/custom_transforms.py` & `CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/training/data_augmentation/custom_transforms.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/training/data_augmentation/data_augmentation_moreDA.py` & `CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/training/data_augmentation/data_augmentation_moreDA.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/training/data_augmentation/default_data_augmentation.py` & `CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/training/data_augmentation/default_data_augmentation.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/training/data_augmentation/downsampling.py` & `CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/training/data_augmentation/downsampling.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/training/data_augmentation/pyramid_augmentations.py` & `CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/training/data_augmentation/pyramid_augmentations.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/training/dataloading/dataset_loading.py` & `CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/training/dataloading/dataset_loading.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/training/learning_rate/poly_lr.py` & `CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/training/learning_rate/poly_lr.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/training/loss_functions/TopK_loss.py` & `CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/training/loss_functions/TopK_loss.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/training/loss_functions/deep_supervision.py` & `CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/training/loss_functions/deep_supervision.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/training/loss_functions/dice_loss.py` & `CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/training/loss_functions/dice_loss.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/training/loss_functions/focal_loss.py` & `CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/training/loss_functions/focal_loss.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/training/model_restore.py` & `CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/training/model_restore.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/training/network_training/network_trainer.py` & `CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/training/network_training/network_trainer.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/training/network_training/nnUNetTrainer.py` & `CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/training/network_training/nnUNetTrainer.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/training/network_training/nnUNetTrainerCascadeFullRes.py` & `CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/training/network_training/nnUNetTrainerCascadeFullRes.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/training/network_training/nnUNetTrainerV2.py` & `CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/training/network_training/nnUNetTrainerV2.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/training/network_training/nnUNetTrainerV2_CascadeFullRes.py` & `CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/training/network_training/nnUNetTrainerV2_CascadeFullRes.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/training/optimizer/ranger.py` & `CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/training/optimizer/ranger.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/utilities/folder_names.py` & `CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/utilities/folder_names.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/utilities/nd_softmax.py` & `CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/utilities/nd_softmax.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/utilities/one_hot_encoding.py` & `CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/utilities/one_hot_encoding.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/utilities/set_n_proc_DA.py` & `CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/utilities/set_n_proc_DA.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/utilities/task_name_id_conversion.py` & `CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/utilities/task_name_id_conversion.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/utilities/tensor_utilities.py` & `CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/utilities/tensor_utilities.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet/utilities/to_torch.py` & `CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet/utilities/to_torch.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet.egg-info/SOURCES.txt` & `CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 CartiMorph_nnUNet/evaluation/model_selection/figure_out_what_to_submit.py
 CartiMorph_nnUNet/experiment_planning/DatasetAnalyzer.py
 CartiMorph_nnUNet/experiment_planning/__init__.py
 CartiMorph_nnUNet/experiment_planning/common_utils.py
 CartiMorph_nnUNet/experiment_planning/experiment_planner_baseline_2DUNet.py
 CartiMorph_nnUNet/experiment_planning/experiment_planner_baseline_3DUNet.py
 CartiMorph_nnUNet/experiment_planning/nnUNet_plan_and_preprocess.py
+CartiMorph_nnUNet/experiment_planning/summarize_plans.py
 CartiMorph_nnUNet/experiment_planning/utils.py
 CartiMorph_nnUNet/inference/__init__.py
 CartiMorph_nnUNet/inference/ensemble_predictions.py
 CartiMorph_nnUNet/inference/predict.py
 CartiMorph_nnUNet/inference/predict_simple.py
 CartiMorph_nnUNet/inference/segmentation_export.py
 CartiMorph_nnUNet/network_architecture/__init__.py
```

### Comparing `CartiMorph_nnUNet-1.7.6/CartiMorph_nnUNet.egg-info/entry_points.txt` & `CartiMorph_nnUNet-1.7.7/CartiMorph_nnUNet.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.6/LICENSE` & `CartiMorph_nnUNet-1.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.6/README.md` & `CartiMorph_nnUNet-1.7.7/README.md`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.6/setup.py` & `CartiMorph_nnUNet-1.7.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_namespace_packages
 
 setup(name='CartiMorph_nnUNet',
       packages=find_namespace_packages(include=["CartiMorph_nnUNet", "CartiMorph_nnUNet.*"]),
-      version='1.7.6',
+      version='1.7.7',
       description='nnU-Net with minor revisions tailored for the CartiMorph framework.',
       url='https://github.com/YongchengYAO/CartiMorph-nnUNet',
-      author='Yongcheng Yao, Chinese University of Hong Kong',
+      author='Yongcheng Yao',
       license='Apache License Version 2.0, January 2004',
       install_requires=[
             "torch>1.10.0",
             "tqdm",
             "dicom2nifti",
             "scikit-image>=0.14",
             "medpy",
```

