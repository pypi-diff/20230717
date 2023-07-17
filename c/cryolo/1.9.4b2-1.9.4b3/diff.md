# Comparing `tmp/cryolo-1.9.4b2.tar.gz` & `tmp/cryolo-1.9.4b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryolo-1.9.4b2.tar", last modified: Wed Mar 22 15:50:07 2023, max compression
+gzip compressed data, was "cryolo-1.9.4b3.tar", last modified: Wed Jul 12 10:48:52 2023, max compression
```

## Comparing `cryolo-1.9.4b2.tar` & `cryolo-1.9.4b3.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2023-03-22 15:50:07.124952 cryolo-1.9.4b2/
--rw-r--r--   0 twagner  (22293) domain users (32000)    17704 2023-02-09 08:33:23.000000 cryolo-1.9.4b2/.gitignore
--rw-r--r--   0 twagner  (22293) domain users (32000)      605 2022-08-09 07:16:57.000000 cryolo-1.9.4b2/.gitlab-ci.yml
-drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2023-03-22 15:50:07.108953 cryolo-1.9.4b2/.idea/
-drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2023-03-22 15:50:07.112953 cryolo-1.9.4b2/.idea/codeStyles/
--rw-r--r--   0 twagner  (22293) domain users (32000)      149 2018-12-11 09:23:01.000000 cryolo-1.9.4b2/.idea/codeStyles/codeStyleConfig.xml
--rw-r--r--   0 twagner  (22293) domain users (32000)      649 2022-08-09 07:16:57.000000 cryolo-1.9.4b2/Dockerfile
--rw-r--r--   0 twagner  (22293) domain users (32000)     6596 2019-09-10 13:28:55.000000 cryolo-1.9.4b2/LICENSE
--rw-r--r--   0 twagner  (22293) domain users (32000)       57 2022-08-09 07:16:57.000000 cryolo-1.9.4b2/MANIFEST.in
--rw-r--r--   0 twagner  (22293) domain users (32000)     1750 2023-03-22 15:50:07.124952 cryolo-1.9.4b2/PKG-INFO
--rw-r--r--   0 twagner  (22293) domain users (32000)      869 2022-08-11 12:21:51.000000 cryolo-1.9.4b2/README.md
--rw-r--r--   0 twagner  (22293) domain users (32000)     6593 2022-08-09 07:16:57.000000 cryolo-1.9.4b2/changelog.txt
-drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2023-03-22 15:50:07.116953 cryolo-1.9.4b2/cryolo/
--rw-r--r--   0 twagner  (22293) domain users (32000)    26925 2023-03-08 13:53:45.000000 cryolo-1.9.4b2/cryolo/CoordsIO.py
--rw-r--r--   0 twagner  (22293) domain users (32000)     2187 2022-08-09 07:16:57.000000 cryolo-1.9.4b2/cryolo/ExtendedModelCheckpoint.py
--rw-r--r--   0 twagner  (22293) domain users (32000)     3325 2022-08-09 07:16:57.000000 cryolo-1.9.4b2/cryolo/MultiGPUModelCheckpoint.py
--rw-r--r--   0 twagner  (22293) domain users (32000)     3475 2023-02-06 08:05:02.000000 cryolo-1.9.4b2/cryolo/SGDRSchedular.py
--rw-r--r--   0 twagner  (22293) domain users (32000)      162 2023-03-22 15:50:01.000000 cryolo-1.9.4b2/cryolo/__init__.py
-drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2023-03-22 15:50:07.120952 cryolo-1.9.4b2/cryolo/augmentation/
--rw-r--r--   0 twagner  (22293) domain users (32000)      877 2022-08-09 07:16:57.000000 cryolo-1.9.4b2/cryolo/augmentation/AddConstantAugmentation.py
--rw-r--r--   0 twagner  (22293) domain users (32000)     1436 2022-08-09 07:16:57.000000 cryolo-1.9.4b2/cryolo/augmentation/AdditiveGaussianNoiseAugmentation.py
--rw-r--r--   0 twagner  (22293) domain users (32000)      298 2022-08-09 07:16:57.000000 cryolo-1.9.4b2/cryolo/augmentation/AugmentationMethod.py
--rw-r--r--   0 twagner  (22293) domain users (32000)      895 2022-08-09 07:16:57.000000 cryolo-1.9.4b2/cryolo/augmentation/AverageBlurAugmentation.py
--rw-r--r--   0 twagner  (22293) domain users (32000)      980 2022-08-09 07:16:57.000000 cryolo-1.9.4b2/cryolo/augmentation/ContrastNormalizationAugmentation.py
--rw-r--r--   0 twagner  (22293) domain users (32000)     2128 2022-08-09 07:16:57.000000 cryolo-1.9.4b2/cryolo/augmentation/CustomRotationAugmentation.py
--rw-r--r--   0 twagner  (22293) domain users (32000)      995 2022-08-09 07:16:57.000000 cryolo-1.9.4b2/cryolo/augmentation/DropoutAugmentation.py
--rw-r--r--   0 twagner  (22293) domain users (32000)     1828 2022-08-09 07:16:57.000000 cryolo-1.9.4b2/cryolo/augmentation/FlipAugmentation.py
--rw-r--r--   0 twagner  (22293) domain users (32000)      957 2022-08-09 07:16:57.000000 cryolo-1.9.4b2/cryolo/augmentation/GaussBlurAugmentation.py
--rw-r--r--   0 twagner  (22293) domain users (32000)      851 2022-08-09 07:16:57.000000 cryolo-1.9.4b2/cryolo/augmentation/MultiplyAugmentation.py
--rw-r--r--   0 twagner  (22293) domain users (32000)     1979 2022-08-09 07:16:57.000000 cryolo-1.9.4b2/cryolo/augmentation/Rot90Augmentation.py
--rw-r--r--   0 twagner  (22293) domain users (32000)        0 2022-08-09 07:16:57.000000 cryolo-1.9.4b2/cryolo/augmentation/__init__.py
--rw-r--r--   0 twagner  (22293) domain users (32000)     3567 2022-08-09 07:16:57.000000 cryolo-1.9.4b2/cryolo/augmentation/augmentation.py
--rw-r--r--   0 twagner  (22293) domain users (32000)    20749 2023-02-06 08:06:46.000000 cryolo-1.9.4b2/cryolo/backend.py
--rw-r--r--   0 twagner  (22293) domain users (32000)     1156 2018-07-13 06:29:00.000000 cryolo-1.9.4b2/cryolo/config.json
--rw-r--r--   0 twagner  (22293) domain users (32000)     5662 2021-07-22 12:09:40.000000 cryolo-1.9.4b2/cryolo/config_tools.py
--rw-r--r--   0 twagner  (22293) domain users (32000)    16314 2023-02-07 16:04:16.000000 cryolo-1.9.4b2/cryolo/cryolo_main.py
--rw-r--r--   0 twagner  (22293) domain users (32000)    35754 2022-08-09 07:16:57.000000 cryolo-1.9.4b2/cryolo/eval.py
-drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2023-03-22 15:50:07.120952 cryolo-1.9.4b2/cryolo/evaluation/
--rw-r--r--   0 twagner  (22293) domain users (32000)        0 2022-08-09 07:16:57.000000 cryolo-1.9.4b2/cryolo/evaluation/__init__.py
--rw-r--r--   0 twagner  (22293) domain users (32000)     1683 2022-08-09 07:16:57.000000 cryolo-1.9.4b2/cryolo/evaluation/boxdataprovider.py
--rw-r--r--   0 twagner  (22293) domain users (32000)      356 2022-08-09 07:16:57.000000 cryolo-1.9.4b2/cryolo/evaluation/metric.py
--rw-r--r--   0 twagner  (22293) domain users (32000)     1021 2022-08-09 07:16:57.000000 cryolo-1.9.4b2/cryolo/evaluation/pathsboxdataprovider.py
--rw-r--r--   0 twagner  (22293) domain users (32000)     1592 2022-08-09 07:16:57.000000 cryolo-1.9.4b2/cryolo/evaluation/pathsfilamentprovider.py
--rw-r--r--   0 twagner  (22293) domain users (32000)     1437 2022-08-09 07:16:57.000000 cryolo-1.9.4b2/cryolo/evaluation/recallprecisionmetric3d.py
--rw-r--r--   0 twagner  (22293) domain users (32000)      699 2022-08-09 07:16:57.000000 cryolo-1.9.4b2/cryolo/evaluation/resultsview.py
--rw-r--r--   0 twagner  (22293) domain users (32000)     6272 2022-08-09 07:16:57.000000 cryolo-1.9.4b2/cryolo/evaluation/tomoevaluation.py
--rw-r--r--   0 twagner  (22293) domain users (32000)    39033 2023-03-22 15:14:59.000000 cryolo-1.9.4b2/cryolo/filament_tracer.py
--rw-r--r--   0 twagner  (22293) domain users (32000)    43716 2023-03-22 15:23:39.000000 cryolo-1.9.4b2/cryolo/frontend.py
--rw-r--r--   0 twagner  (22293) domain users (32000)    16846 2022-08-09 07:16:57.000000 cryolo-1.9.4b2/cryolo/grouping3d.py
--rw-r--r--   0 twagner  (22293) domain users (32000)     5599 2023-02-06 07:46:25.000000 cryolo-1.9.4b2/cryolo/imagereader.py
--rw-r--r--   0 twagner  (22293) domain users (32000)    12487 2023-02-28 12:22:42.000000 cryolo-1.9.4b2/cryolo/lowpass.py
--rw-r--r--   0 twagner  (22293) domain users (32000)    17815 2023-03-22 13:21:53.000000 cryolo-1.9.4b2/cryolo/patchwisebatchgenerator2.py
--rw-r--r--   0 twagner  (22293) domain users (32000)    88981 2023-02-28 12:21:24.000000 cryolo-1.9.4b2/cryolo/predict.py
--rw-r--r--   0 twagner  (22293) domain users (32000)    10378 2023-03-22 13:15:30.000000 cryolo-1.9.4b2/cryolo/preprocessing.py
--rw-r--r--   0 twagner  (22293) domain users (32000)     1440 2020-05-19 10:49:52.000000 cryolo-1.9.4b2/cryolo/test_gooey.py
--rw-r--r--   0 twagner  (22293) domain users (32000)    28112 2023-03-20 09:26:43.000000 cryolo-1.9.4b2/cryolo/train.py
--rw-r--r--   0 twagner  (22293) domain users (32000)    61880 2023-02-28 12:23:47.000000 cryolo-1.9.4b2/cryolo/utils.py
--rw-r--r--   0 twagner  (22293) domain users (32000)      693 2020-11-11 15:27:12.000000 cryolo-1.9.4b2/cryolo/vis_box_3d.py
--rw-r--r--   0 twagner  (22293) domain users (32000)     3960 2023-02-06 08:04:51.000000 cryolo-1.9.4b2/cryolo/warmup_callback.py
-drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2023-03-22 15:50:07.116953 cryolo-1.9.4b2/cryolo.egg-info/
--rw-r--r--   0 twagner  (22293) domain users (32000)     1750 2023-03-22 15:50:01.000000 cryolo-1.9.4b2/cryolo.egg-info/PKG-INFO
--rw-r--r--   0 twagner  (22293) domain users (32000)     2567 2023-03-22 15:50:07.000000 cryolo-1.9.4b2/cryolo.egg-info/SOURCES.txt
--rw-r--r--   0 twagner  (22293) domain users (32000)        1 2023-03-22 15:50:01.000000 cryolo-1.9.4b2/cryolo.egg-info/dependency_links.txt
--rw-r--r--   0 twagner  (22293) domain users (32000)      250 2023-03-22 15:50:01.000000 cryolo-1.9.4b2/cryolo.egg-info/entry_points.txt
--rw-r--r--   0 twagner  (22293) domain users (32000)      505 2023-03-22 15:50:01.000000 cryolo-1.9.4b2/cryolo.egg-info/requires.txt
--rw-r--r--   0 twagner  (22293) domain users (32000)       13 2023-03-22 15:50:01.000000 cryolo-1.9.4b2/cryolo.egg-info/top_level.txt
-drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2023-03-22 15:50:07.116953 cryolo-1.9.4b2/icons/
--rw-r--r--   0 twagner  (22293) domain users (32000)    15129 2019-07-30 13:12:26.000000 cryolo-1.9.4b2/icons/config_icon.png
--rw-r--r--   0 twagner  (22293) domain users (32000)   113506 2019-07-30 13:57:17.000000 cryolo-1.9.4b2/icons/program_icon.ico
--rw-r--r--   0 twagner  (22293) domain users (32000)     2628 2019-09-24 13:29:39.000000 cryolo-1.9.4b2/icons/program_icon.png
-drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2023-03-22 15:50:07.108953 cryolo-1.9.4b2/resources/
-drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2023-03-22 15:50:07.108953 cryolo-1.9.4b2/resources/test_FolderDataProvider/
-drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2023-03-22 15:50:07.120952 cryolo-1.9.4b2/resources/test_FolderDataProvider/00_gt/
--rw-r--r--   0 twagner  (22293) domain users (32000)      393 2022-08-09 07:16:59.000000 cryolo-1.9.4b2/resources/test_FolderDataProvider/00_gt/tomo018_10.cbox
-drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2023-03-22 15:50:07.120952 cryolo-1.9.4b2/resources/test_FolderDataProvider/00_measured/
--rw-r--r--   0 twagner  (22293) domain users (32000)    30847 2022-08-09 07:16:59.000000 cryolo-1.9.4b2/resources/test_FolderDataProvider/00_measured/tomo018_10.cbox
-drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2023-03-22 15:50:07.120952 cryolo-1.9.4b2/resources/test_FolderDataProvider/01_gt_filament/
--rw-r--r--   0 twagner  (22293) domain users (32000)    83564 2022-08-09 07:16:59.000000 cryolo-1.9.4b2/resources/test_FolderDataProvider/01_gt_filament/SarcDros_ba03_ex01_la03_to01_10.96Apx_lp60.cbox
--rw-r--r--   0 twagner  (22293) domain users (32000)       38 2023-03-22 15:50:07.124952 cryolo-1.9.4b2/setup.cfg
--rw-r--r--   0 twagner  (22293) domain users (32000)     7231 2023-02-28 17:54:03.000000 cryolo-1.9.4b2/setup.py
-drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2023-03-22 15:50:07.124952 cryolo-1.9.4b2/tests/
--rw-r--r--   0 twagner  (22293) domain users (32000)        0 2022-08-09 07:16:59.000000 cryolo-1.9.4b2/tests/__init__.py
-drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2023-03-22 15:50:07.124952 cryolo-1.9.4b2/tests/evaluation/
--rw-r--r--   0 twagner  (22293) domain users (32000)        0 2022-08-09 07:16:59.000000 cryolo-1.9.4b2/tests/evaluation/__init__.py
--rw-r--r--   0 twagner  (22293) domain users (32000)      367 2022-08-09 07:16:59.000000 cryolo-1.9.4b2/tests/evaluation/test_BoxDataProvider.py
--rw-r--r--   0 twagner  (22293) domain users (32000)     2462 2022-08-09 07:16:59.000000 cryolo-1.9.4b2/tests/evaluation/test_PathsDataProvider.py
--rw-r--r--   0 twagner  (22293) domain users (32000)     3667 2022-08-09 07:16:59.000000 cryolo-1.9.4b2/tests/evaluation/test_RecallPrecisionMetric3D.py
--rw-r--r--   0 twagner  (22293) domain users (32000)     5708 2022-08-09 07:16:59.000000 cryolo-1.9.4b2/tests/evaluation/test_tomoevaluation.py
--rw-r--r--   0 twagner  (22293) domain users (32000)     9757 2023-02-08 13:35:52.000000 cryolo-1.9.4b2/tests/test_CoordsIO.py
--rw-r--r--   0 twagner  (22293) domain users (32000)    16715 2022-08-09 07:16:59.000000 cryolo-1.9.4b2/tests/test_augmentation.py
--rw-r--r--   0 twagner  (22293) domain users (32000)      374 2022-08-09 07:16:59.000000 cryolo-1.9.4b2/tests/test_eval.py
--rw-r--r--   0 twagner  (22293) domain users (32000)    35400 2023-02-28 10:03:44.000000 cryolo-1.9.4b2/tests/test_filament_tracer.py
--rw-r--r--   0 twagner  (22293) domain users (32000)     3006 2022-08-09 07:16:59.000000 cryolo-1.9.4b2/tests/test_frontend.py
--rw-r--r--   0 twagner  (22293) domain users (32000)     5591 2022-08-09 07:16:59.000000 cryolo-1.9.4b2/tests/test_grouping3d.py
--rw-r--r--   0 twagner  (22293) domain users (32000)      494 2022-08-09 07:16:59.000000 cryolo-1.9.4b2/tests/test_lowpass.py
--rw-r--r--   0 twagner  (22293) domain users (32000)     1885 2022-08-09 07:16:59.000000 cryolo-1.9.4b2/tests/test_predict.py
--rw-r--r--   0 twagner  (22293) domain users (32000)      606 2022-08-09 07:16:59.000000 cryolo-1.9.4b2/tests/test_preprocessing.py
--rw-r--r--   0 twagner  (22293) domain users (32000)    26655 2022-08-09 07:16:59.000000 cryolo-1.9.4b2/tests/test_utils.py
--rw-r--r--   0 twagner  (22293) domain users (32000)      225 2022-08-09 07:16:59.000000 cryolo-1.9.4b2/updated_installation_instructions
+drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2023-07-12 10:48:52.220378 cryolo-1.9.4b3/
+-rw-r--r--   0 twagner  (22293) domain users (32000)    17704 2023-02-09 08:33:23.000000 cryolo-1.9.4b3/.gitignore
+-rw-r--r--   0 twagner  (22293) domain users (32000)      605 2022-08-09 07:16:57.000000 cryolo-1.9.4b3/.gitlab-ci.yml
+drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2023-07-12 10:48:52.212378 cryolo-1.9.4b3/.idea/
+drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2023-07-12 10:48:52.212378 cryolo-1.9.4b3/.idea/codeStyles/
+-rw-r--r--   0 twagner  (22293) domain users (32000)      149 2018-12-11 09:23:01.000000 cryolo-1.9.4b3/.idea/codeStyles/codeStyleConfig.xml
+-rw-r--r--   0 twagner  (22293) domain users (32000)      649 2022-08-09 07:16:57.000000 cryolo-1.9.4b3/Dockerfile
+-rw-r--r--   0 twagner  (22293) domain users (32000)     6596 2019-09-10 13:28:55.000000 cryolo-1.9.4b3/LICENSE
+-rw-r--r--   0 twagner  (22293) domain users (32000)       57 2022-08-09 07:16:57.000000 cryolo-1.9.4b3/MANIFEST.in
+-rw-r--r--   0 twagner  (22293) domain users (32000)     1750 2023-07-12 10:48:52.220378 cryolo-1.9.4b3/PKG-INFO
+-rw-r--r--   0 twagner  (22293) domain users (32000)      869 2022-08-11 12:21:51.000000 cryolo-1.9.4b3/README.md
+-rw-r--r--   0 twagner  (22293) domain users (32000)     6593 2022-08-09 07:16:57.000000 cryolo-1.9.4b3/changelog.txt
+drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2023-07-12 10:48:52.216378 cryolo-1.9.4b3/cryolo/
+-rw-r--r--   0 twagner  (22293) domain users (32000)    28321 2023-04-24 09:07:53.000000 cryolo-1.9.4b3/cryolo/CoordsIO.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)     2187 2022-08-09 07:16:57.000000 cryolo-1.9.4b3/cryolo/ExtendedModelCheckpoint.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)     3325 2022-08-09 07:16:57.000000 cryolo-1.9.4b3/cryolo/MultiGPUModelCheckpoint.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)     3475 2023-02-06 08:05:02.000000 cryolo-1.9.4b3/cryolo/SGDRSchedular.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)      162 2023-07-12 10:48:46.000000 cryolo-1.9.4b3/cryolo/__init__.py
+drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2023-07-12 10:48:52.220378 cryolo-1.9.4b3/cryolo/augmentation/
+-rw-r--r--   0 twagner  (22293) domain users (32000)      877 2022-08-09 07:16:57.000000 cryolo-1.9.4b3/cryolo/augmentation/AddConstantAugmentation.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)     1436 2022-08-09 07:16:57.000000 cryolo-1.9.4b3/cryolo/augmentation/AdditiveGaussianNoiseAugmentation.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)      298 2022-08-09 07:16:57.000000 cryolo-1.9.4b3/cryolo/augmentation/AugmentationMethod.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)      895 2022-08-09 07:16:57.000000 cryolo-1.9.4b3/cryolo/augmentation/AverageBlurAugmentation.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)      980 2022-08-09 07:16:57.000000 cryolo-1.9.4b3/cryolo/augmentation/ContrastNormalizationAugmentation.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)     2128 2022-08-09 07:16:57.000000 cryolo-1.9.4b3/cryolo/augmentation/CustomRotationAugmentation.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)      995 2022-08-09 07:16:57.000000 cryolo-1.9.4b3/cryolo/augmentation/DropoutAugmentation.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)     1828 2022-08-09 07:16:57.000000 cryolo-1.9.4b3/cryolo/augmentation/FlipAugmentation.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)      957 2022-08-09 07:16:57.000000 cryolo-1.9.4b3/cryolo/augmentation/GaussBlurAugmentation.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)      851 2022-08-09 07:16:57.000000 cryolo-1.9.4b3/cryolo/augmentation/MultiplyAugmentation.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)     1979 2022-08-09 07:16:57.000000 cryolo-1.9.4b3/cryolo/augmentation/Rot90Augmentation.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)        0 2022-08-09 07:16:57.000000 cryolo-1.9.4b3/cryolo/augmentation/__init__.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)     3567 2022-08-09 07:16:57.000000 cryolo-1.9.4b3/cryolo/augmentation/augmentation.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)    20749 2023-02-06 08:06:46.000000 cryolo-1.9.4b3/cryolo/backend.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)     1156 2018-07-13 06:29:00.000000 cryolo-1.9.4b3/cryolo/config.json
+-rw-r--r--   0 twagner  (22293) domain users (32000)     5662 2021-07-22 12:09:40.000000 cryolo-1.9.4b3/cryolo/config_tools.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)    16314 2023-02-07 16:04:16.000000 cryolo-1.9.4b3/cryolo/cryolo_main.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)    35754 2022-08-09 07:16:57.000000 cryolo-1.9.4b3/cryolo/eval.py
+drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2023-07-12 10:48:52.220378 cryolo-1.9.4b3/cryolo/evaluation/
+-rw-r--r--   0 twagner  (22293) domain users (32000)        0 2022-08-09 07:16:57.000000 cryolo-1.9.4b3/cryolo/evaluation/__init__.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)     1683 2022-08-09 07:16:57.000000 cryolo-1.9.4b3/cryolo/evaluation/boxdataprovider.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)      356 2022-08-09 07:16:57.000000 cryolo-1.9.4b3/cryolo/evaluation/metric.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)     1021 2022-08-09 07:16:57.000000 cryolo-1.9.4b3/cryolo/evaluation/pathsboxdataprovider.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)     1592 2022-08-09 07:16:57.000000 cryolo-1.9.4b3/cryolo/evaluation/pathsfilamentprovider.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)     1437 2022-08-09 07:16:57.000000 cryolo-1.9.4b3/cryolo/evaluation/recallprecisionmetric3d.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)      699 2022-08-09 07:16:57.000000 cryolo-1.9.4b3/cryolo/evaluation/resultsview.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)     6272 2022-08-09 07:16:57.000000 cryolo-1.9.4b3/cryolo/evaluation/tomoevaluation.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)    39033 2023-03-22 15:14:59.000000 cryolo-1.9.4b3/cryolo/filament_tracer.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)    43314 2023-03-23 10:12:00.000000 cryolo-1.9.4b3/cryolo/frontend.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)    16846 2022-08-09 07:16:57.000000 cryolo-1.9.4b3/cryolo/grouping3d.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)     5599 2023-02-06 07:46:25.000000 cryolo-1.9.4b3/cryolo/imagereader.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)    12487 2023-02-28 12:22:42.000000 cryolo-1.9.4b3/cryolo/lowpass.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)    17815 2023-07-12 10:42:10.000000 cryolo-1.9.4b3/cryolo/patchwisebatchgenerator2.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)    89490 2023-07-12 10:46:36.000000 cryolo-1.9.4b3/cryolo/predict.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)    10378 2023-03-22 13:15:30.000000 cryolo-1.9.4b3/cryolo/preprocessing.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)     1440 2020-05-19 10:49:52.000000 cryolo-1.9.4b3/cryolo/test_gooey.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)    28112 2023-03-20 09:26:43.000000 cryolo-1.9.4b3/cryolo/train.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)    61897 2023-07-12 10:41:46.000000 cryolo-1.9.4b3/cryolo/utils.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)      693 2020-11-11 15:27:12.000000 cryolo-1.9.4b3/cryolo/vis_box_3d.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)     3960 2023-02-06 08:04:51.000000 cryolo-1.9.4b3/cryolo/warmup_callback.py
+drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2023-07-12 10:48:52.216378 cryolo-1.9.4b3/cryolo.egg-info/
+-rw-r--r--   0 twagner  (22293) domain users (32000)     1750 2023-07-12 10:48:46.000000 cryolo-1.9.4b3/cryolo.egg-info/PKG-INFO
+-rw-r--r--   0 twagner  (22293) domain users (32000)     2567 2023-07-12 10:48:52.000000 cryolo-1.9.4b3/cryolo.egg-info/SOURCES.txt
+-rw-r--r--   0 twagner  (22293) domain users (32000)        1 2023-07-12 10:48:46.000000 cryolo-1.9.4b3/cryolo.egg-info/dependency_links.txt
+-rw-r--r--   0 twagner  (22293) domain users (32000)      250 2023-07-12 10:48:46.000000 cryolo-1.9.4b3/cryolo.egg-info/entry_points.txt
+-rw-r--r--   0 twagner  (22293) domain users (32000)      505 2023-07-12 10:48:46.000000 cryolo-1.9.4b3/cryolo.egg-info/requires.txt
+-rw-r--r--   0 twagner  (22293) domain users (32000)       13 2023-07-12 10:48:46.000000 cryolo-1.9.4b3/cryolo.egg-info/top_level.txt
+drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2023-07-12 10:48:52.216378 cryolo-1.9.4b3/icons/
+-rw-r--r--   0 twagner  (22293) domain users (32000)    15129 2019-07-30 13:12:26.000000 cryolo-1.9.4b3/icons/config_icon.png
+-rw-r--r--   0 twagner  (22293) domain users (32000)   113506 2019-07-30 13:57:17.000000 cryolo-1.9.4b3/icons/program_icon.ico
+-rw-r--r--   0 twagner  (22293) domain users (32000)     2628 2019-09-24 13:29:39.000000 cryolo-1.9.4b3/icons/program_icon.png
+drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2023-07-12 10:48:52.212378 cryolo-1.9.4b3/resources/
+drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2023-07-12 10:48:52.212378 cryolo-1.9.4b3/resources/test_FolderDataProvider/
+drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2023-07-12 10:48:52.220378 cryolo-1.9.4b3/resources/test_FolderDataProvider/00_gt/
+-rw-r--r--   0 twagner  (22293) domain users (32000)      393 2022-08-09 07:16:59.000000 cryolo-1.9.4b3/resources/test_FolderDataProvider/00_gt/tomo018_10.cbox
+drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2023-07-12 10:48:52.220378 cryolo-1.9.4b3/resources/test_FolderDataProvider/00_measured/
+-rw-r--r--   0 twagner  (22293) domain users (32000)    30847 2022-08-09 07:16:59.000000 cryolo-1.9.4b3/resources/test_FolderDataProvider/00_measured/tomo018_10.cbox
+drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2023-07-12 10:48:52.220378 cryolo-1.9.4b3/resources/test_FolderDataProvider/01_gt_filament/
+-rw-r--r--   0 twagner  (22293) domain users (32000)    83564 2022-08-09 07:16:59.000000 cryolo-1.9.4b3/resources/test_FolderDataProvider/01_gt_filament/SarcDros_ba03_ex01_la03_to01_10.96Apx_lp60.cbox
+-rw-r--r--   0 twagner  (22293) domain users (32000)       38 2023-07-12 10:48:52.220378 cryolo-1.9.4b3/setup.cfg
+-rw-r--r--   0 twagner  (22293) domain users (32000)     7231 2023-07-12 10:45:29.000000 cryolo-1.9.4b3/setup.py
+drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2023-07-12 10:48:52.220378 cryolo-1.9.4b3/tests/
+-rw-r--r--   0 twagner  (22293) domain users (32000)        0 2022-08-09 07:16:59.000000 cryolo-1.9.4b3/tests/__init__.py
+drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2023-07-12 10:48:52.220378 cryolo-1.9.4b3/tests/evaluation/
+-rw-r--r--   0 twagner  (22293) domain users (32000)        0 2022-08-09 07:16:59.000000 cryolo-1.9.4b3/tests/evaluation/__init__.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)      367 2022-08-09 07:16:59.000000 cryolo-1.9.4b3/tests/evaluation/test_BoxDataProvider.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)     2462 2022-08-09 07:16:59.000000 cryolo-1.9.4b3/tests/evaluation/test_PathsDataProvider.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)     3667 2022-08-09 07:16:59.000000 cryolo-1.9.4b3/tests/evaluation/test_RecallPrecisionMetric3D.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)     5708 2022-08-09 07:16:59.000000 cryolo-1.9.4b3/tests/evaluation/test_tomoevaluation.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)     9757 2023-02-08 13:35:52.000000 cryolo-1.9.4b3/tests/test_CoordsIO.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)    16715 2022-08-09 07:16:59.000000 cryolo-1.9.4b3/tests/test_augmentation.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)      374 2022-08-09 07:16:59.000000 cryolo-1.9.4b3/tests/test_eval.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)    35400 2023-02-28 10:03:44.000000 cryolo-1.9.4b3/tests/test_filament_tracer.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)     3006 2022-08-09 07:16:59.000000 cryolo-1.9.4b3/tests/test_frontend.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)     5591 2022-08-09 07:16:59.000000 cryolo-1.9.4b3/tests/test_grouping3d.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)      494 2022-08-09 07:16:59.000000 cryolo-1.9.4b3/tests/test_lowpass.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)     1885 2022-08-09 07:16:59.000000 cryolo-1.9.4b3/tests/test_predict.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)      606 2022-08-09 07:16:59.000000 cryolo-1.9.4b3/tests/test_preprocessing.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)    26655 2022-08-09 07:16:59.000000 cryolo-1.9.4b3/tests/test_utils.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)      225 2022-08-09 07:16:59.000000 cryolo-1.9.4b3/updated_installation_instructions
```

### Comparing `cryolo-1.9.4b2/.gitignore` & `cryolo-1.9.4b3/.gitignore`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/.gitlab-ci.yml` & `cryolo-1.9.4b3/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/Dockerfile` & `cryolo-1.9.4b3/Dockerfile`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/LICENSE` & `cryolo-1.9.4b3/LICENSE`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/PKG-INFO` & `cryolo-1.9.4b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryolo
-Version: 1.9.4b2
+Version: 1.9.4b3
 Summary: Picking procedure for cryo em single particle analysis
 Home-page: https://cryolo.readthedocs.io/en/stable/index.html
 Author: Thorsten Wagner
 Author-email: thorsten.wagner@mpi-dortmund.mpg.de
 License: Other/Proprietary License (all rights reserved)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `cryolo-1.9.4b2/README.md` & `cryolo-1.9.4b3/README.md`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/changelog.txt` & `cryolo-1.9.4b3/changelog.txt`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/cryolo/CoordsIO.py` & `cryolo-1.9.4b3/cryolo/CoordsIO.py`

 * *Files 6% similar despite different names*

```diff
@@ -235,29 +235,70 @@
     filaments_list = [Filament(filaments[key]) for key in filaments]
     if min_distance > 0:
         filaments_list = utils.resample_filaments(filaments_list, min_distance)
 
     return filaments_list
 
 
-def write_star_filemant_file(path, filaments):
-    columns = ['_rlnCoordinateX', '_rlnCoordinateY', '_rlnAutopickFigureOfMerit', '_rlnHelicalTubeID', '_rlnAnglePsiPrior']
+def write_star_filemant_file_2(path, filaments):
+    num_boxes = 2*len(filaments)
+
+    coords = np.zeros(shape=(num_boxes,2))
+    i = 0
+    for fil in filaments:
+        bstart = fil.boxes[0]
+        bend = fil.boxes[-1]
+        coords[i, 0] = bstart.x + bstart.w / 2
+        coords[i, 1] = bstart.y + bstart.h / 2
+        coords[i+1, 0] = bend.x + bend.w / 2
+        coords[i+1, 1] = bend.y + bend.h / 2
+        i = i + 2
+
+    df = pd.DataFrame(coords, columns=['_rlnCoordinateX', '_rlnCoordinateY'])
+    sfile = star.StarFile(path)
+    sfile.update('', df, True)
+    sfile.write_star_file(overwrite=True)
+
+def make_star_filament_dict_start_end(filaments) -> dict:
+    data_dict = {
+        "_rlnCoordinateX": [],
+        "_rlnCoordinateY": []
+    }
+    for fil in filaments:
+        bstart = fil.boxes[0]
+        bend = fil.boxes[-1]
+        data_dict["_rlnCoordinateX"].append(bstart.x + bstart.w / 2)
+        data_dict["_rlnCoordinateX"].append(bend.x + bend.w / 2)
+        data_dict["_rlnCoordinateY"].append(bstart.y + bstart.h / 2)
+        data_dict["_rlnCoordinateY"].append(bend.y + bend.h / 2)
+    return data_dict
+
+def make_star_filament_dict_segmented(filaments) -> dict:
+    columns = ['_rlnCoordinateX', '_rlnCoordinateY', '_rlnAutopickFigureOfMerit', '_rlnHelicalTubeID',
+               '_rlnAnglePsiPrior']
     data_dict = {}
     for clm in columns:
         data_dict[clm] = []
 
     for fil_id, fil in enumerate(filaments):
         utils.set_filament_psi_priors(fil)
         for box_index, box in enumerate(fil.boxes):
             data_dict['_rlnCoordinateX'].append(box.x + box.w / 2)
             data_dict['_rlnCoordinateY'].append(box.y + box.h / 2)
             data_dict['_rlnAutopickFigureOfMerit'].append(box.c)
             data_dict['_rlnHelicalTubeID'].append(fil_id + 1)
             data_dict['_rlnAnglePsiPrior'].append(fil.meta['psi'][box_index])
+    return data_dict
+
+def write_star_filemant_file(path, filaments, start_end=False):
 
+    if start_end:
+        data_dict = make_star_filament_dict_start_end(filaments)
+    else:
+        data_dict = make_star_filament_dict_segmented(filaments)
     df = pd.DataFrame(data_dict)
     sfile = star.StarFile(path)
     sfile.update('', df, True)
     sfile.write_star_file(overwrite=True)
 
 
 def write_cryosparc_star_file(path: str, coordinates: Union[List[BoundBox], List[Filament]], micrograph_name: str):
```

### Comparing `cryolo-1.9.4b2/cryolo/ExtendedModelCheckpoint.py` & `cryolo-1.9.4b3/cryolo/ExtendedModelCheckpoint.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/cryolo/MultiGPUModelCheckpoint.py` & `cryolo-1.9.4b3/cryolo/MultiGPUModelCheckpoint.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/cryolo/SGDRSchedular.py` & `cryolo-1.9.4b3/cryolo/SGDRSchedular.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/cryolo/augmentation/AddConstantAugmentation.py` & `cryolo-1.9.4b3/cryolo/augmentation/AddConstantAugmentation.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/cryolo/augmentation/AdditiveGaussianNoiseAugmentation.py` & `cryolo-1.9.4b3/cryolo/augmentation/AdditiveGaussianNoiseAugmentation.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/cryolo/augmentation/AverageBlurAugmentation.py` & `cryolo-1.9.4b3/cryolo/augmentation/AverageBlurAugmentation.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/cryolo/augmentation/ContrastNormalizationAugmentation.py` & `cryolo-1.9.4b3/cryolo/augmentation/ContrastNormalizationAugmentation.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/cryolo/augmentation/CustomRotationAugmentation.py` & `cryolo-1.9.4b3/cryolo/augmentation/CustomRotationAugmentation.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/cryolo/augmentation/DropoutAugmentation.py` & `cryolo-1.9.4b3/cryolo/augmentation/DropoutAugmentation.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/cryolo/augmentation/FlipAugmentation.py` & `cryolo-1.9.4b3/cryolo/augmentation/FlipAugmentation.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/cryolo/augmentation/GaussBlurAugmentation.py` & `cryolo-1.9.4b3/cryolo/augmentation/GaussBlurAugmentation.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/cryolo/augmentation/MultiplyAugmentation.py` & `cryolo-1.9.4b3/cryolo/augmentation/MultiplyAugmentation.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/cryolo/augmentation/Rot90Augmentation.py` & `cryolo-1.9.4b3/cryolo/augmentation/Rot90Augmentation.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/cryolo/augmentation/augmentation.py` & `cryolo-1.9.4b3/cryolo/augmentation/augmentation.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/cryolo/backend.py` & `cryolo-1.9.4b3/cryolo/backend.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/cryolo/config.json` & `cryolo-1.9.4b3/cryolo/config.json`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/cryolo/config_tools.py` & `cryolo-1.9.4b3/cryolo/config_tools.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/cryolo/cryolo_main.py` & `cryolo-1.9.4b3/cryolo/cryolo_main.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/cryolo/eval.py` & `cryolo-1.9.4b3/cryolo/eval.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/cryolo/evaluation/boxdataprovider.py` & `cryolo-1.9.4b3/cryolo/evaluation/boxdataprovider.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/cryolo/evaluation/pathsboxdataprovider.py` & `cryolo-1.9.4b3/cryolo/evaluation/pathsboxdataprovider.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/cryolo/evaluation/pathsfilamentprovider.py` & `cryolo-1.9.4b3/cryolo/evaluation/pathsfilamentprovider.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/cryolo/evaluation/recallprecisionmetric3d.py` & `cryolo-1.9.4b3/cryolo/evaluation/recallprecisionmetric3d.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/cryolo/evaluation/resultsview.py` & `cryolo-1.9.4b3/cryolo/evaluation/resultsview.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/cryolo/evaluation/tomoevaluation.py` & `cryolo-1.9.4b3/cryolo/evaluation/tomoevaluation.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/cryolo/filament_tracer.py` & `cryolo-1.9.4b3/cryolo/filament_tracer.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/cryolo/frontend.py` & `cryolo-1.9.4b3/cryolo/frontend.py`

 * *Files 1% similar despite different names*

```diff
@@ -384,33 +384,30 @@
             / (nb_coord_box + 1e-6)
             / 2.0
         )
 
         if self.is_filament_model:
             # I should do it similar to confidence, but not sure why the
             # division by 2 happens
-            #loss_angle = true_box_angle - pred_box_angle
-            '''
-            diff_angles_a = tf.abs(true_box_angle - pred_box_angle)
-            # Reason for +-0.5: The 0.5 is actuall +- PI, but the true angles are in the range from
-            # 0 to 1 instead of 0 to 2PI because they are normalized. 0.5 is also actually +- PI
-            diff_angles_b = tf.abs(true_box_angle - pred_box_angle + 1)
-            diff_angles_c = tf.abs(true_box_angle - pred_box_angle - 1)
-
-            diff_angles = tf.minimum(tf.math.minimum(diff_angles_a,diff_angles_b),diff_angles_c)
-            '''
             dot = tf.square(
                 tf.cos(true_box_angle*np.pi)*tf.cos(pred_box_angle*np.pi)+
                 tf.sin(true_box_angle*np.pi)*tf.sin(pred_box_angle*np.pi)
             )
             loss_angle = (
                 tf.reduce_sum((1-dot) * coord_mask[:,:,:,0,:]) # conf_mask
                 / (nb_coord_box + 1e-6) # nb_conf_box
                 / 2
             )
+            '''
+            loss_angle = tf.cond(
+                tf.less(seen, warmup_bs),
+                lambda: loss_angle * 0,
+                lambda: loss_angle
+            )
+            '''
 
 
         if self.experimental_loss:
             loss_conf_obj = (
                 tf.reduce_sum(tf.square(true_box_conf - pred_box_conf) * conf_mask_obj)
                 / (nb_conf_box_obj + 1e-6)
                 / 2.0
@@ -433,15 +430,15 @@
         )
         loss_class = tf.reduce_sum(loss_class * class_mask) / (nb_class_box + 1e-6)
 
         if self.experimental_loss:
             loss = loss_xy + loss_conf_obj + loss_conf_noobj + loss_class + loss_wh
         else:
             if self.is_filament_model:
-                loss = loss_xy + loss_conf + loss_class + loss_wh + loss_angle*2
+                loss = loss_xy + loss_conf + loss_class + loss_wh + loss_angle
             else:
                 loss = loss_xy + loss_conf + loss_class + loss_wh
 
         if self.debug:
             nb_true_box = tf.reduce_sum(y_true[..., 4])
             nb_pred_box = tf.reduce_sum(
                 tf.to_float(true_box_conf > 0.5) * tf.to_float(pred_box_conf > 0.3)
```

### Comparing `cryolo-1.9.4b2/cryolo/grouping3d.py` & `cryolo-1.9.4b3/cryolo/grouping3d.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/cryolo/imagereader.py` & `cryolo-1.9.4b3/cryolo/imagereader.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/cryolo/lowpass.py` & `cryolo-1.9.4b3/cryolo/lowpass.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/cryolo/patchwisebatchgenerator2.py` & `cryolo-1.9.4b3/cryolo/patchwisebatchgenerator2.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/cryolo/predict.py` & `cryolo-1.9.4b3/cryolo/predict.py`

 * *Files 1% similar despite different names*

```diff
@@ -845,15 +845,15 @@
                 #pool = multiprocessing.Pool(processes=num_cpus)
                 #print("NUM TRACERS:", len(filament_tracers), "CPUS", num_cpus)
 
                 with multiprocessing.Pool(processes=num_cpus) as pool:
                     subset_new_filaments = pool.map(
                                 trace_subset_filements,
                                 range(len(filament_tracers)),
-                                #chunksize=1,
+                                chunksize=1,
                             )
 
 
                 print("Tracing done")
                 for image_index, frame_index, filaments in subset_new_filaments:
 
                     if "filaments" not in picking_result_subset[image_index]:
@@ -1117,14 +1117,18 @@
                                 outdir, "EMAN_START_END", filename
                             )
                             filename = os.path.splitext(filename)[0] + ".star"
                             star_segmented = os.path.join(
                                 outdir, "STAR_FILAMENT_SEGMENTED", filename
                             )
 
+                            star_start_end = os.path.join(
+                                outdir, "STAR_FILAMENT_START_END", filename
+                            )
+
                             #star_cryopsarc = os.path.join(
                             #    outdir, "CRYOSPARC", "cryosparc.star"
                             #)
 
                             filename = os.path.splitext(filename)[0] + ".cbox"
                             cbox_segmented = os.path.join(
                                 outdir, "CBOX_FILAMENT_SEGMENTED", filename
@@ -1153,14 +1157,17 @@
 
                         if not os.path.exists(os.path.dirname(eman_start_end)):
                             os.makedirs(os.path.dirname(eman_start_end))
 
                         if not os.path.exists(os.path.dirname(star_segmented)):
                             os.makedirs(os.path.dirname(star_segmented))
 
+                        if not os.path.exists(os.path.dirname(star_start_end)):
+                            os.makedirs(os.path.dirname(star_start_end))
+
                         if not os.path.exists(os.path.dirname(cbox_segmented)):
                             os.makedirs(os.path.dirname(cbox_segmented))
 
                         if not os.path.exists(os.path.dirname(cbox_unfitlered)):
                             os.makedirs(os.path.dirname(cbox_unfitlered))
 
                        # if not os.path.exists(os.path.dirname(star_cryopsarc)):
@@ -1176,14 +1183,20 @@
                             filaments=result["filaments"][frame], path=eman_start_end
                         )
 
                         CoordsIO.write_star_filemant_file(
                             filaments=result["filaments"][frame], path=star_segmented
                         )
 
+                        CoordsIO.write_star_filemant_file(
+                            filaments=result["filaments"][frame], path=star_start_end, start_end=True
+                        )
+
+
+
                         CoordsIO.write_cbox_file(
                             coordinates=result["filaments"][frame],
                             path=cbox_segmented
                         )
 
                         CoordsIO.write_cbox_file(
                             coordinates=result["boxes_unfiltered"][frame],
```

### Comparing `cryolo-1.9.4b2/cryolo/preprocessing.py` & `cryolo-1.9.4b3/cryolo/preprocessing.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/cryolo/test_gooey.py` & `cryolo-1.9.4b3/cryolo/test_gooey.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/cryolo/train.py` & `cryolo-1.9.4b3/cryolo/train.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/cryolo/utils.py` & `cryolo-1.9.4b3/cryolo/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -305,15 +305,14 @@
     total_elength = distance_elem[-1]
 
 
     distance = distance_elem / distance_elem[-1]  # normalized
     fx, fy = interp1d(distance, x), interp1d(distance, y)
     if z is not None:
         fz = interp1d(distance, z)
-
     num = int(total_elength / new_distance) +1
 
     alpha = np.linspace(0, 1, num)
 
     x_regular, y_regular = fx(alpha), fy(alpha)
     if z is not None:
         z_regular = fz(alpha)
@@ -1658,15 +1657,15 @@
     return intersect
 
 def find_corresponding_path(list_of_paths,path):
     import pathlib
     import os
     pth = pathlib.PurePath(path)
     current_lookup_var = pth.name
-    paths = [path for path in list_of_paths if current_lookup_var in path]
+    paths = [path for path in list_of_paths if current_lookup_var == os.path.basename(path)]
     while len(paths) > 1:
         current_lookup_var = os.path.join(pth.parent.name,current_lookup_var)
         pth = pth.parent
         paths = [path for path in list_of_paths if current_lookup_var in path]
     return paths[0]
 
 def vector_to_direction(x,y):
```

### Comparing `cryolo-1.9.4b2/cryolo/vis_box_3d.py` & `cryolo-1.9.4b3/cryolo/vis_box_3d.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/cryolo/warmup_callback.py` & `cryolo-1.9.4b3/cryolo/warmup_callback.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/cryolo.egg-info/PKG-INFO` & `cryolo-1.9.4b3/cryolo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryolo
-Version: 1.9.4b2
+Version: 1.9.4b3
 Summary: Picking procedure for cryo em single particle analysis
 Home-page: https://cryolo.readthedocs.io/en/stable/index.html
 Author: Thorsten Wagner
 Author-email: thorsten.wagner@mpi-dortmund.mpg.de
 License: Other/Proprietary License (all rights reserved)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `cryolo-1.9.4b2/cryolo.egg-info/SOURCES.txt` & `cryolo-1.9.4b3/cryolo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/icons/config_icon.png` & `cryolo-1.9.4b3/icons/config_icon.png`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/icons/program_icon.ico` & `cryolo-1.9.4b3/icons/program_icon.ico`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/icons/program_icon.png` & `cryolo-1.9.4b3/icons/program_icon.png`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/resources/test_FolderDataProvider/00_measured/tomo018_10.cbox` & `cryolo-1.9.4b3/resources/test_FolderDataProvider/00_measured/tomo018_10.cbox`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/resources/test_FolderDataProvider/01_gt_filament/SarcDros_ba03_ex01_la03_to01_10.96Apx_lp60.cbox` & `cryolo-1.9.4b3/resources/test_FolderDataProvider/01_gt_filament/SarcDros_ba03_ex01_la03_to01_10.96Apx_lp60.cbox`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/setup.py` & `cryolo-1.9.4b3/setup.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/tests/evaluation/test_PathsDataProvider.py` & `cryolo-1.9.4b3/tests/evaluation/test_PathsDataProvider.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/tests/evaluation/test_RecallPrecisionMetric3D.py` & `cryolo-1.9.4b3/tests/evaluation/test_RecallPrecisionMetric3D.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/tests/evaluation/test_tomoevaluation.py` & `cryolo-1.9.4b3/tests/evaluation/test_tomoevaluation.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/tests/test_CoordsIO.py` & `cryolo-1.9.4b3/tests/test_CoordsIO.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/tests/test_augmentation.py` & `cryolo-1.9.4b3/tests/test_augmentation.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/tests/test_filament_tracer.py` & `cryolo-1.9.4b3/tests/test_filament_tracer.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/tests/test_frontend.py` & `cryolo-1.9.4b3/tests/test_frontend.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/tests/test_grouping3d.py` & `cryolo-1.9.4b3/tests/test_grouping3d.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/tests/test_predict.py` & `cryolo-1.9.4b3/tests/test_predict.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/tests/test_preprocessing.py` & `cryolo-1.9.4b3/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.4b2/tests/test_utils.py` & `cryolo-1.9.4b3/tests/test_utils.py`

 * *Files identical despite different names*

