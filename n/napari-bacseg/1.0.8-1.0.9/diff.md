# Comparing `tmp/napari-bacseg-1.0.8.tar.gz` & `tmp/napari-bacseg-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-bacseg-1.0.8.tar", last modified: Wed Jun 14 08:28:01 2023, max compression
+gzip compressed data, was "napari-bacseg-1.0.9.tar", last modified: Mon Jul 17 09:49:27 2023, max compression
```

## Comparing `napari-bacseg-1.0.8.tar` & `napari-bacseg-1.0.9.tar`

### file list

```diff
@@ -1,120 +1,122 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 08:28:01.941965 napari-bacseg-1.0.8/
-drwxrwxrwx   0        0        0        0 2023-06-14 08:28:01.575951 napari-bacseg-1.0.8/.github/
-drwxrwxrwx   0        0        0        0 2023-06-14 08:28:01.601704 napari-bacseg-1.0.8/.github/workflows/
--rw-rw-rw-   0        0        0     2904 2023-02-24 11:00:35.000000 napari-bacseg-1.0.8/.github/workflows/test_and_deploy.yml
--rw-rw-rw-   0        0        0     1239 2023-03-08 16:30:28.000000 napari-bacseg-1.0.8/.gitignore
-drwxrwxrwx   0        0        0        0 2023-06-14 08:28:01.607689 napari-bacseg-1.0.8/.napari-hub/
--rw-rw-rw-   0        0        0      472 2023-02-24 11:00:35.000000 napari-bacseg-1.0.8/.napari-hub/DESCRIPTION.md
--rw-rw-rw-   0        0        0      551 2023-02-24 11:00:35.000000 napari-bacseg-1.0.8/.napari-hub/config.yml
--rw-rw-rw-   0        0        0     1211 2023-02-24 11:01:10.000000 napari-bacseg-1.0.8/.pre-commit-config.yaml
--rw-rw-rw-   0        0        0     1515 2023-02-24 11:00:35.000000 napari-bacseg-1.0.8/LICENSE
--rw-rw-rw-   0        0        0      101 2023-02-24 11:00:35.000000 napari-bacseg-1.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     4732 2023-06-14 08:28:01.941965 napari-bacseg-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3859 2023-02-27 13:15:54.000000 napari-bacseg-1.0.8/README.md
--rw-rw-rw-   0        0        0      271 2023-02-27 13:15:54.000000 napari-bacseg-1.0.8/bacseg_ui.py
--rw-rw-rw-   0        0        0      988 2023-06-14 08:26:42.000000 napari-bacseg-1.0.8/pyproject.toml
--rw-rw-rw-   0        0        0     2035 2023-06-14 08:28:01.944957 napari-bacseg-1.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-14 08:28:01.576950 napari-bacseg-1.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-06-14 08:28:01.847723 napari-bacseg-1.0.8/src/_dev/
--rw-rw-rw-   0        0        0      560 2022-10-16 10:26:58.000000 napari-bacseg-1.0.8/src/_dev/Export Masks to AKSEG v5 dev.py
--rw-rw-rw-   0        0        0     8279 2023-02-24 14:29:04.000000 napari-bacseg-1.0.8/src/_dev/ScanR dev.py
--rw-rw-rw-   0        0        0      482 2022-05-26 11:42:59.000000 napari-bacseg-1.0.8/src/_dev/Troodos dev.py
--rw-rw-rw-   0        0        0        0 2022-04-28 17:23:51.000000 napari-bacseg-1.0.8/src/_dev/__init__.py
--rw-rw-rw-   0        0        0     1878 2023-02-24 12:15:54.000000 napari-bacseg-1.0.8/src/_dev/akseg_db_stats.py
--rw-rw-rw-   0        0        0    11262 2023-02-24 14:19:52.000000 napari-bacseg-1.0.8/src/_dev/akseg_dev.py
--rw-rw-rw-   0        0        0     4463 2023-02-24 14:19:52.000000 napari-bacseg-1.0.8/src/_dev/akseg_dev2.py
--rw-rw-rw-   0        0        0    10114 2023-02-24 14:36:34.000000 napari-bacseg-1.0.8/src/_dev/akseg_txt_metadata.py
--rw-rw-rw-   0        0        0    10960 2023-02-24 14:19:52.000000 napari-bacseg-1.0.8/src/_dev/align_alex_datadump.py
--rw-rw-rw-   0        0        0    28052 2023-02-24 14:19:52.000000 napari-bacseg-1.0.8/src/_dev/alison_datadump.py
--rw-rw-rw-   0        0        0     4168 2023-02-24 14:19:11.000000 napari-bacseg-1.0.8/src/_dev/autocontast_dev.py
--rw-rw-rw-   0        0        0      454 2023-02-24 14:19:52.000000 napari-bacseg-1.0.8/src/_dev/cellposedev.py
--rw-rw-rw-   0        0        0      367 2022-09-22 16:01:43.000000 napari-bacseg-1.0.8/src/_dev/cellposeshapely.py
--rw-rw-rw-   0        0        0     1279 2023-03-27 16:45:42.000000 napari-bacseg-1.0.8/src/_dev/chatGPT_midlines.py
--rw-rw-rw-   0        0        0     6105 2023-05-05 10:49:23.000000 napari-bacseg-1.0.8/src/_dev/check_AluGasketv12_DFP.py
--rw-rw-rw-   0        0        0     6452 2023-02-24 14:19:52.000000 napari-bacseg-1.0.8/src/_dev/check_metadata.py
--rw-rw-rw-   0        0        0     1650 2023-02-24 14:19:11.000000 napari-bacseg-1.0.8/src/_dev/colicoords_cellldist_dev.py
--rw-rw-rw-   0        0        0     3442 2023-02-24 14:19:11.000000 napari-bacseg-1.0.8/src/_dev/colicoords_ldist_dev.py
--rw-rw-rw-   0        0        0    11185 2023-02-24 14:36:34.000000 napari-bacseg-1.0.8/src/_dev/database_dev.py
--rw-rw-rw-   0        0        0     1023 2023-03-23 14:05:20.000000 napari-bacseg-1.0.8/src/_dev/deepsegmattest.py
--rw-rw-rw-   0        0        0      666 2023-03-22 14:37:10.000000 napari-bacseg-1.0.8/src/_dev/edit_database_columns.py
--rw-rw-rw-   0        0        0     1701 2023-02-24 12:15:54.000000 napari-bacseg-1.0.8/src/_dev/fits_dev.py
--rw-rw-rw-   0        0        0     7216 2023-02-24 14:19:52.000000 napari-bacseg-1.0.8/src/_dev/fix_alison_missing_file_list.py
--rw-rw-rw-   0        0        0     1126 2023-02-24 14:19:52.000000 napari-bacseg-1.0.8/src/_dev/generate_scanr_movie.py
--rw-rw-rw-   0        0        0    24393 2023-02-24 14:19:52.000000 napari-bacseg-1.0.8/src/_dev/get_akseg_stats.py
--rw-rw-rw-   0        0        0     2623 2022-11-14 15:25:24.000000 napari-bacseg-1.0.8/src/_dev/get_species_info.py
--rw-rw-rw-   0        0        0     1991 2023-06-13 13:41:08.000000 napari-bacseg-1.0.8/src/_dev/imagej_dev.py
--rw-rw-rw-   0        0        0     5034 2023-06-13 08:40:50.000000 napari-bacseg-1.0.8/src/_dev/json_nuclei_dev.py
--rw-rw-rw-   0        0        0     4255 2023-02-24 14:19:52.000000 napari-bacseg-1.0.8/src/_dev/luke__script.py
--rw-rw-rw-   0        0        0     5550 2023-02-24 14:21:12.000000 napari-bacseg-1.0.8/src/_dev/matplotlib_Events.py
--rw-rw-rw-   0        0        0    40825 2023-03-22 17:47:52.000000 napari-bacseg-1.0.8/src/_dev/move_AluGasketDFP.py
--rw-rw-rw-   0        0        0    44028 2023-04-04 10:28:53.000000 napari-bacseg-1.0.8/src/_dev/move_AluGasketDFP_poster.py
--rw-rw-rw-   0        0        0    48241 2023-04-26 15:22:38.000000 napari-bacseg-1.0.8/src/_dev/move_AluGasketv12_DFP.py
--rw-rw-rw-   0        0        0    46551 2023-05-05 08:15:07.000000 napari-bacseg-1.0.8/src/_dev/move_AluGasketv12_DFP_Titration.py
--rw-rw-rw-   0        0        0    35330 2023-03-13 15:20:23.000000 napari-bacseg-1.0.8/src/_dev/move_conor_nim_dfp_data.py
--rw-rw-rw-   0        0        0    34295 2023-03-08 10:06:11.000000 napari-bacseg-1.0.8/src/_dev/move_pillar_data.py
--rw-rw-rw-   0        0        0    37169 2023-02-24 14:19:52.000000 napari-bacseg-1.0.8/src/_dev/move_pillar_zstack_data.py
--rw-rw-rw-   0        0        0    57720 2023-02-24 14:29:03.000000 napari-bacseg-1.0.8/src/_dev/move_unlearning_files.py
--rw-rw-rw-   0        0        0      686 2023-02-14 15:45:10.000000 napari-bacseg-1.0.8/src/_dev/new_metadata2.pickle.py
--rw-rw-rw-   0        0        0     5989 2023-02-24 14:29:03.000000 napari-bacseg-1.0.8/src/_dev/new_read_akseg_directory.py
--rw-rw-rw-   0        0        0     7222 2023-02-24 14:19:52.000000 napari-bacseg-1.0.8/src/_dev/nim_dev.py
--rw-rw-rw-   0        0        0     3173 2023-02-24 14:19:52.000000 napari-bacseg-1.0.8/src/_dev/omnipose_dev.py
--rw-rw-rw-   0        0        0     4398 2023-02-24 14:29:04.000000 napari-bacseg-1.0.8/src/_dev/omnipose_midlines.py
--rw-rw-rw-   0        0        0     3032 2023-02-24 14:29:04.000000 napari-bacseg-1.0.8/src/_dev/omnipose_train.py
--rw-rw-rw-   0        0        0    33520 2023-02-24 14:29:03.000000 napari-bacseg-1.0.8/src/_dev/oufti_dilate.py
--rw-rw-rw-   0        0        0    37571 2023-03-06 10:55:01.000000 napari-bacseg-1.0.8/src/_dev/oufti_dilate_with_midlines.py
--rw-rw-rw-   0        0        0     4449 2023-05-04 09:42:23.000000 napari-bacseg-1.0.8/src/_dev/pandas_speed.py
--rw-rw-rw-   0        0        0    32011 2023-02-24 14:19:52.000000 napari-bacseg-1.0.8/src/_dev/process_alex_datadump.py
--rw-rw-rw-   0        0        0    32643 2023-02-24 14:19:52.000000 napari-bacseg-1.0.8/src/_dev/process_alex_datadump_clinical.py
--rw-rw-rw-   0        0        0    28804 2023-02-24 14:19:52.000000 napari-bacseg-1.0.8/src/_dev/process_conor_datadump.py
--rw-rw-rw-   0        0        0    30160 2023-02-24 14:19:52.000000 napari-bacseg-1.0.8/src/_dev/process_gramstain_datadump.py
--rw-rw-rw-   0        0        0      576 2022-08-16 09:34:20.000000 napari-bacseg-1.0.8/src/_dev/read_non_tif.py
--rw-rw-rw-   0        0        0     7794 2023-02-24 14:19:52.000000 napari-bacseg-1.0.8/src/_dev/rebuild_usermeta.py
--rw-rw-rw-   0        0        0    10440 2023-02-24 14:19:52.000000 napari-bacseg-1.0.8/src/_dev/rebuild_usermeta_2.py
--rw-rw-rw-   0        0        0     3034 2023-03-23 13:58:59.000000 napari-bacseg-1.0.8/src/_dev/recreate_user_metadata.py
--rw-rw-rw-   0        0        0     2117 2023-04-20 14:14:30.000000 napari-bacseg-1.0.8/src/_dev/scalebar_dev.py
--rw-rw-rw-   0        0        0    25122 2023-02-24 14:19:52.000000 napari-bacseg-1.0.8/src/_dev/sort_midlines.py
--rw-rw-rw-   0        0        0     9633 2023-02-24 14:19:52.000000 napari-bacseg-1.0.8/src/_dev/stelios_stats.py
--rw-rw-rw-   0        0        0      644 2023-02-24 14:19:52.000000 napari-bacseg-1.0.8/src/_dev/tile_meta_check.py
--rw-rw-rw-   0        0        0     1615 2022-07-22 11:43:30.000000 napari-bacseg-1.0.8/src/_dev/tiler_dev.py
--rw-rw-rw-   0        0        0     3064 2023-02-24 14:29:04.000000 napari-bacseg-1.0.8/src/_dev/updade_akseg_metadata.py
--rw-rw-rw-   0        0        0     2057 2023-02-24 12:22:32.000000 napari-bacseg-1.0.8/src/_dev/update_img_metadata.py
--rw-rw-rw-   0        0        0     6859 2023-02-24 14:19:52.000000 napari-bacseg-1.0.8/src/_dev/video_iamges.py
--rw-rw-rw-   0        0        0     7767 2023-03-13 16:18:11.000000 napari-bacseg-1.0.8/src/_dev/zooniverse.py
--rw-rw-rw-   0        0        0     5624 2023-02-24 14:21:12.000000 napari-bacseg-1.0.8/src/_dev/zooniverse_move.py
--rw-rw-rw-   0        0        0     5742 2023-03-15 10:15:29.000000 napari-bacseg-1.0.8/src/_dev/zooniverse_move_titrations.py
--rw-rw-rw-   0        0        0    30267 2023-03-13 16:29:04.000000 napari-bacseg-1.0.8/src/_dev/zooniverse_titration_upload.py
--rw-rw-rw-   0        0        0     7503 2023-03-13 17:00:21.000000 napari-bacseg-1.0.8/src/_dev/zooniverse_titrations.py
--rw-rw-rw-   0        0        0    30267 2023-03-13 16:09:34.000000 napari-bacseg-1.0.8/src/_dev/zooniverse_upload.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:28:01.912045 napari-bacseg-1.0.8/src/napari_bacseg/
--rw-rw-rw-   0        0        0      155 2023-06-14 08:26:42.000000 napari-bacseg-1.0.8/src/napari_bacseg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:28:01.939970 napari-bacseg-1.0.8/src/napari_bacseg/_tests/
--rw-rw-rw-   0        0        0        0 2023-02-24 11:00:35.000000 napari-bacseg-1.0.8/src/napari_bacseg/_tests/__init__.py
--rw-rw-rw-   0        0        0    26817 2023-06-13 13:36:57.000000 napari-bacseg-1.0.8/src/napari_bacseg/_tests/test_bacseg.py
--rw-rw-rw-   0        0        0     1276 2023-02-27 13:15:54.000000 napari-bacseg-1.0.8/src/napari_bacseg/_tests/test_widget.py
--rw-rw-rw-   0        0        0    90731 2023-06-13 16:07:22.000000 napari-bacseg-1.0.8/src/napari_bacseg/_utils.py
--rw-rw-rw-   0        0        0    14723 2023-06-13 08:44:12.000000 napari-bacseg-1.0.8/src/napari_bacseg/_utils_cellpose.py
--rw-rw-rw-   0        0        0    17465 2023-02-27 13:15:54.000000 napari-bacseg-1.0.8/src/napari_bacseg/_utils_colicoords.py
--rw-rw-rw-   0        0        0    20495 2023-05-03 08:53:54.000000 napari-bacseg-1.0.8/src/napari_bacseg/_utils_database.py
--rw-rw-rw-   0        0        0    47487 2023-06-13 09:49:45.000000 napari-bacseg-1.0.8/src/napari_bacseg/_utils_database_IO.py
--rw-rw-rw-   0        0        0     1670 2023-06-13 13:50:19.000000 napari-bacseg-1.0.8/src/napari_bacseg/_utils_imagej.py
--rw-rw-rw-   0        0        0    40215 2023-06-13 08:44:13.000000 napari-bacseg-1.0.8/src/napari_bacseg/_utils_interface_events.py
--rw-rw-rw-   0        0        0     6485 2023-06-13 08:44:12.000000 napari-bacseg-1.0.8/src/napari_bacseg/_utils_json.py
--rw-rw-rw-   0        0        0    34168 2023-03-07 17:38:57.000000 napari-bacseg-1.0.8/src/napari_bacseg/_utils_oufti.py
--rw-rw-rw-   0        0        0     2132 2023-02-27 13:15:54.000000 napari-bacseg-1.0.8/src/napari_bacseg/_utils_refine.py
--rw-rw-rw-   0        0        0    22517 2023-06-09 14:18:42.000000 napari-bacseg-1.0.8/src/napari_bacseg/_utils_statistics.py
--rw-rw-rw-   0        0        0     7837 2023-06-09 14:18:42.000000 napari-bacseg-1.0.8/src/napari_bacseg/_utils_tiler.py
--rw-rw-rw-   0        0        0      164 2023-06-14 08:28:01.000000 napari-bacseg-1.0.8/src/napari_bacseg/_version.py
--rw-rw-rw-   0        0        0    84663 2023-06-14 08:24:43.000000 napari-bacseg-1.0.8/src/napari_bacseg/_widget.py
--rw-rw-rw-   0        0        0   173126 2023-06-14 08:14:23.000000 napari-bacseg-1.0.8/src/napari_bacseg/bacseg_ui.py
--rw-rw-rw-   0        0        0   172600 2023-06-14 08:13:43.000000 napari-bacseg-1.0.8/src/napari_bacseg/bacseg_ui.ui
--rw-rw-rw-   0        0        0      271 2023-02-27 13:15:54.000000 napari-bacseg-1.0.8/src/napari_bacseg/gapseq_ui.py
--rw-rw-rw-   0        0        0      501 2023-03-07 17:38:57.000000 napari-bacseg-1.0.8/src/napari_bacseg/napari.yaml
--rw-rw-rw-   0        0        0      271 2023-02-27 13:15:54.000000 napari-bacseg-1.0.8/src/napari_bacseg/napari_ui.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:28:01.931023 napari-bacseg-1.0.8/src/napari_bacseg.egg-info/
--rw-rw-rw-   0        0        0     4732 2023-06-14 08:28:01.000000 napari-bacseg-1.0.8/src/napari_bacseg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3322 2023-06-14 08:28:01.000000 napari-bacseg-1.0.8/src/napari_bacseg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 08:28:01.000000 napari-bacseg-1.0.8/src/napari_bacseg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-06-14 08:28:01.000000 napari-bacseg-1.0.8/src/napari_bacseg.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      352 2023-06-14 08:28:01.000000 napari-bacseg-1.0.8/src/napari_bacseg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-06-14 08:28:01.000000 napari-bacseg-1.0.8/src/napari_bacseg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      644 2023-02-24 11:00:35.000000 napari-bacseg-1.0.8/tox.ini
+drwxrwxrwx   0        0        0        0 2023-07-17 09:49:27.766365 napari-bacseg-1.0.9/
+drwxrwxrwx   0        0        0        0 2023-07-17 09:49:27.375889 napari-bacseg-1.0.9/.github/
+drwxrwxrwx   0        0        0        0 2023-07-17 09:49:27.407021 napari-bacseg-1.0.9/.github/workflows/
+-rw-rw-rw-   0        0        0     2904 2023-02-24 11:00:35.000000 napari-bacseg-1.0.9/.github/workflows/test_and_deploy.yml
+-rw-rw-rw-   0        0        0     1239 2023-03-08 16:30:28.000000 napari-bacseg-1.0.9/.gitignore
+drwxrwxrwx   0        0        0        0 2023-07-17 09:49:27.407021 napari-bacseg-1.0.9/.napari-hub/
+-rw-rw-rw-   0        0        0      472 2023-02-24 11:00:35.000000 napari-bacseg-1.0.9/.napari-hub/DESCRIPTION.md
+-rw-rw-rw-   0        0        0      551 2023-02-24 11:00:35.000000 napari-bacseg-1.0.9/.napari-hub/config.yml
+-rw-rw-rw-   0        0        0     1211 2023-02-24 11:01:10.000000 napari-bacseg-1.0.9/.pre-commit-config.yaml
+-rw-rw-rw-   0        0        0     1515 2023-02-24 11:00:35.000000 napari-bacseg-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0      101 2023-02-24 11:00:35.000000 napari-bacseg-1.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     4732 2023-07-17 09:49:27.766365 napari-bacseg-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3859 2023-02-27 13:15:54.000000 napari-bacseg-1.0.9/README.md
+-rw-rw-rw-   0        0        0      271 2023-02-27 13:15:54.000000 napari-bacseg-1.0.9/bacseg_ui.py
+-rw-rw-rw-   0        0        0      988 2023-07-17 09:48:13.000000 napari-bacseg-1.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0     2060 2023-07-17 09:49:27.766365 napari-bacseg-1.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-17 09:49:27.375889 napari-bacseg-1.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-07-17 09:49:27.672519 napari-bacseg-1.0.9/src/_dev/
+-rw-rw-rw-   0        0        0      560 2022-10-16 10:26:58.000000 napari-bacseg-1.0.9/src/_dev/Export Masks to AKSEG v5 dev.py
+-rw-rw-rw-   0        0        0     8279 2023-02-24 14:29:04.000000 napari-bacseg-1.0.9/src/_dev/ScanR dev.py
+-rw-rw-rw-   0        0        0      482 2022-05-26 11:42:59.000000 napari-bacseg-1.0.9/src/_dev/Troodos dev.py
+-rw-rw-rw-   0        0        0        0 2022-04-28 17:23:51.000000 napari-bacseg-1.0.9/src/_dev/__init__.py
+-rw-rw-rw-   0        0        0     1878 2023-02-24 12:15:54.000000 napari-bacseg-1.0.9/src/_dev/akseg_db_stats.py
+-rw-rw-rw-   0        0        0    11262 2023-02-24 14:19:52.000000 napari-bacseg-1.0.9/src/_dev/akseg_dev.py
+-rw-rw-rw-   0        0        0     4463 2023-02-24 14:19:52.000000 napari-bacseg-1.0.9/src/_dev/akseg_dev2.py
+-rw-rw-rw-   0        0        0    10114 2023-02-24 14:36:34.000000 napari-bacseg-1.0.9/src/_dev/akseg_txt_metadata.py
+-rw-rw-rw-   0        0        0    10960 2023-02-24 14:19:52.000000 napari-bacseg-1.0.9/src/_dev/align_alex_datadump.py
+-rw-rw-rw-   0        0        0    28052 2023-02-24 14:19:52.000000 napari-bacseg-1.0.9/src/_dev/alison_datadump.py
+-rw-rw-rw-   0        0        0     4168 2023-02-24 14:19:11.000000 napari-bacseg-1.0.9/src/_dev/autocontast_dev.py
+-rw-rw-rw-   0        0        0      454 2023-02-24 14:19:52.000000 napari-bacseg-1.0.9/src/_dev/cellposedev.py
+-rw-rw-rw-   0        0        0      367 2022-09-22 16:01:43.000000 napari-bacseg-1.0.9/src/_dev/cellposeshapely.py
+-rw-rw-rw-   0        0        0     1279 2023-03-27 16:45:42.000000 napari-bacseg-1.0.9/src/_dev/chatGPT_midlines.py
+-rw-rw-rw-   0        0        0     6105 2023-05-05 10:49:23.000000 napari-bacseg-1.0.9/src/_dev/check_AluGasketv12_DFP.py
+-rw-rw-rw-   0        0        0     6452 2023-02-24 14:19:52.000000 napari-bacseg-1.0.9/src/_dev/check_metadata.py
+-rw-rw-rw-   0        0        0     1650 2023-02-24 14:19:11.000000 napari-bacseg-1.0.9/src/_dev/colicoords_cellldist_dev.py
+-rw-rw-rw-   0        0        0     3442 2023-02-24 14:19:11.000000 napari-bacseg-1.0.9/src/_dev/colicoords_ldist_dev.py
+-rw-rw-rw-   0        0        0    11185 2023-02-24 14:36:34.000000 napari-bacseg-1.0.9/src/_dev/database_dev.py
+-rw-rw-rw-   0        0        0     1023 2023-03-23 14:05:20.000000 napari-bacseg-1.0.9/src/_dev/deepsegmattest.py
+-rw-rw-rw-   0        0        0      666 2023-03-22 14:37:10.000000 napari-bacseg-1.0.9/src/_dev/edit_database_columns.py
+-rw-rw-rw-   0        0        0     1701 2023-02-24 12:15:54.000000 napari-bacseg-1.0.9/src/_dev/fits_dev.py
+-rw-rw-rw-   0        0        0     7216 2023-02-24 14:19:52.000000 napari-bacseg-1.0.9/src/_dev/fix_alison_missing_file_list.py
+-rw-rw-rw-   0        0        0     1126 2023-02-24 14:19:52.000000 napari-bacseg-1.0.9/src/_dev/generate_scanr_movie.py
+-rw-rw-rw-   0        0        0    24393 2023-02-24 14:19:52.000000 napari-bacseg-1.0.9/src/_dev/get_akseg_stats.py
+-rw-rw-rw-   0        0        0     2623 2022-11-14 15:25:24.000000 napari-bacseg-1.0.9/src/_dev/get_species_info.py
+-rw-rw-rw-   0        0        0     1983 2023-06-14 13:14:31.000000 napari-bacseg-1.0.9/src/_dev/imagej_dev.py
+-rw-rw-rw-   0        0        0     5034 2023-06-13 08:40:50.000000 napari-bacseg-1.0.9/src/_dev/json_nuclei_dev.py
+-rw-rw-rw-   0        0        0     4255 2023-02-24 14:19:52.000000 napari-bacseg-1.0.9/src/_dev/luke__script.py
+-rw-rw-rw-   0        0        0     5550 2023-02-24 14:21:12.000000 napari-bacseg-1.0.9/src/_dev/matplotlib_Events.py
+-rw-rw-rw-   0        0        0    40825 2023-03-22 17:47:52.000000 napari-bacseg-1.0.9/src/_dev/move_AluGasketDFP.py
+-rw-rw-rw-   0        0        0    44028 2023-04-04 10:28:53.000000 napari-bacseg-1.0.9/src/_dev/move_AluGasketDFP_poster.py
+-rw-rw-rw-   0        0        0    48241 2023-04-26 15:22:38.000000 napari-bacseg-1.0.9/src/_dev/move_AluGasketv12_DFP.py
+-rw-rw-rw-   0        0        0    46551 2023-05-05 08:15:07.000000 napari-bacseg-1.0.9/src/_dev/move_AluGasketv12_DFP_Titration.py
+-rw-rw-rw-   0        0        0    35330 2023-03-13 15:20:23.000000 napari-bacseg-1.0.9/src/_dev/move_conor_nim_dfp_data.py
+-rw-rw-rw-   0        0        0    34295 2023-03-08 10:06:11.000000 napari-bacseg-1.0.9/src/_dev/move_pillar_data.py
+-rw-rw-rw-   0        0        0    37169 2023-02-24 14:19:52.000000 napari-bacseg-1.0.9/src/_dev/move_pillar_zstack_data.py
+-rw-rw-rw-   0        0        0    57720 2023-02-24 14:29:03.000000 napari-bacseg-1.0.9/src/_dev/move_unlearning_files.py
+-rw-rw-rw-   0        0        0      686 2023-02-14 15:45:10.000000 napari-bacseg-1.0.9/src/_dev/new_metadata2.pickle.py
+-rw-rw-rw-   0        0        0     5989 2023-02-24 14:29:03.000000 napari-bacseg-1.0.9/src/_dev/new_read_akseg_directory.py
+-rw-rw-rw-   0        0        0     7222 2023-02-24 14:19:52.000000 napari-bacseg-1.0.9/src/_dev/nim_dev.py
+-rw-rw-rw-   0        0        0     3173 2023-02-24 14:19:52.000000 napari-bacseg-1.0.9/src/_dev/omnipose_dev.py
+-rw-rw-rw-   0        0        0     4398 2023-02-24 14:29:04.000000 napari-bacseg-1.0.9/src/_dev/omnipose_midlines.py
+-rw-rw-rw-   0        0        0     3032 2023-02-24 14:29:04.000000 napari-bacseg-1.0.9/src/_dev/omnipose_train.py
+-rw-rw-rw-   0        0        0    33520 2023-02-24 14:29:03.000000 napari-bacseg-1.0.9/src/_dev/oufti_dilate.py
+-rw-rw-rw-   0        0        0    37571 2023-03-06 10:55:01.000000 napari-bacseg-1.0.9/src/_dev/oufti_dilate_with_midlines.py
+-rw-rw-rw-   0        0        0     4449 2023-05-04 09:42:23.000000 napari-bacseg-1.0.9/src/_dev/pandas_speed.py
+-rw-rw-rw-   0        0        0    32011 2023-02-24 14:19:52.000000 napari-bacseg-1.0.9/src/_dev/process_alex_datadump.py
+-rw-rw-rw-   0        0        0    32643 2023-02-24 14:19:52.000000 napari-bacseg-1.0.9/src/_dev/process_alex_datadump_clinical.py
+-rw-rw-rw-   0        0        0    28804 2023-02-24 14:19:52.000000 napari-bacseg-1.0.9/src/_dev/process_conor_datadump.py
+-rw-rw-rw-   0        0        0    30160 2023-02-24 14:19:52.000000 napari-bacseg-1.0.9/src/_dev/process_gramstain_datadump.py
+-rw-rw-rw-   0        0        0      576 2022-08-16 09:34:20.000000 napari-bacseg-1.0.9/src/_dev/read_non_tif.py
+-rw-rw-rw-   0        0        0    15266 2023-07-14 15:28:28.000000 napari-bacseg-1.0.9/src/_dev/read_trillian.py
+-rw-rw-rw-   0        0        0     7794 2023-02-24 14:19:52.000000 napari-bacseg-1.0.9/src/_dev/rebuild_usermeta.py
+-rw-rw-rw-   0        0        0    10440 2023-02-24 14:19:52.000000 napari-bacseg-1.0.9/src/_dev/rebuild_usermeta_2.py
+-rw-rw-rw-   0        0        0     3034 2023-03-23 13:58:59.000000 napari-bacseg-1.0.9/src/_dev/recreate_user_metadata.py
+-rw-rw-rw-   0        0        0     2117 2023-04-20 14:14:30.000000 napari-bacseg-1.0.9/src/_dev/scalebar_dev.py
+-rw-rw-rw-   0        0        0    25122 2023-02-24 14:19:52.000000 napari-bacseg-1.0.9/src/_dev/sort_midlines.py
+-rw-rw-rw-   0        0        0     9633 2023-02-24 14:19:52.000000 napari-bacseg-1.0.9/src/_dev/stelios_stats.py
+-rw-rw-rw-   0        0        0      644 2023-02-24 14:19:52.000000 napari-bacseg-1.0.9/src/_dev/tile_meta_check.py
+-rw-rw-rw-   0        0        0     1615 2022-07-22 11:43:30.000000 napari-bacseg-1.0.9/src/_dev/tiler_dev.py
+-rw-rw-rw-   0        0        0     3064 2023-02-24 14:29:04.000000 napari-bacseg-1.0.9/src/_dev/updade_akseg_metadata.py
+-rw-rw-rw-   0        0        0     2057 2023-02-24 12:22:32.000000 napari-bacseg-1.0.9/src/_dev/update_img_metadata.py
+-rw-rw-rw-   0        0        0     6859 2023-02-24 14:19:52.000000 napari-bacseg-1.0.9/src/_dev/video_iamges.py
+-rw-rw-rw-   0        0        0     7767 2023-03-13 16:18:11.000000 napari-bacseg-1.0.9/src/_dev/zooniverse.py
+-rw-rw-rw-   0        0        0     5624 2023-02-24 14:21:12.000000 napari-bacseg-1.0.9/src/_dev/zooniverse_move.py
+-rw-rw-rw-   0        0        0     5742 2023-03-15 10:15:29.000000 napari-bacseg-1.0.9/src/_dev/zooniverse_move_titrations.py
+-rw-rw-rw-   0        0        0    30267 2023-03-13 16:29:04.000000 napari-bacseg-1.0.9/src/_dev/zooniverse_titration_upload.py
+-rw-rw-rw-   0        0        0     7503 2023-03-13 17:00:21.000000 napari-bacseg-1.0.9/src/_dev/zooniverse_titrations.py
+-rw-rw-rw-   0        0        0    30267 2023-03-13 16:09:34.000000 napari-bacseg-1.0.9/src/_dev/zooniverse_upload.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:49:27.735118 napari-bacseg-1.0.9/src/napari_bacseg/
+-rw-rw-rw-   0        0        0      155 2023-07-17 09:48:13.000000 napari-bacseg-1.0.9/src/napari_bacseg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:49:27.766365 napari-bacseg-1.0.9/src/napari_bacseg/_tests/
+-rw-rw-rw-   0        0        0        0 2023-02-24 11:00:35.000000 napari-bacseg-1.0.9/src/napari_bacseg/_tests/__init__.py
+-rw-rw-rw-   0        0        0    26817 2023-06-13 13:36:57.000000 napari-bacseg-1.0.9/src/napari_bacseg/_tests/test_bacseg.py
+-rw-rw-rw-   0        0        0     1276 2023-02-27 13:15:54.000000 napari-bacseg-1.0.9/src/napari_bacseg/_tests/test_widget.py
+-rw-rw-rw-   0        0        0    99818 2023-07-17 09:44:21.000000 napari-bacseg-1.0.9/src/napari_bacseg/_utils.py
+-rw-rw-rw-   0        0        0    14723 2023-06-13 08:44:12.000000 napari-bacseg-1.0.9/src/napari_bacseg/_utils_cellpose.py
+-rw-rw-rw-   0        0        0    17465 2023-02-27 13:15:54.000000 napari-bacseg-1.0.9/src/napari_bacseg/_utils_colicoords.py
+-rw-rw-rw-   0        0        0    20495 2023-05-03 08:53:54.000000 napari-bacseg-1.0.9/src/napari_bacseg/_utils_database.py
+-rw-rw-rw-   0        0        0    47487 2023-06-13 09:49:45.000000 napari-bacseg-1.0.9/src/napari_bacseg/_utils_database_IO.py
+-rw-rw-rw-   0        0        0     1670 2023-06-13 13:50:19.000000 napari-bacseg-1.0.9/src/napari_bacseg/_utils_imagej.py
+-rw-rw-rw-   0        0        0    40215 2023-06-13 08:44:13.000000 napari-bacseg-1.0.9/src/napari_bacseg/_utils_interface_events.py
+-rw-rw-rw-   0        0        0     6485 2023-06-13 08:44:12.000000 napari-bacseg-1.0.9/src/napari_bacseg/_utils_json.py
+-rw-rw-rw-   0        0        0    34168 2023-03-07 17:38:57.000000 napari-bacseg-1.0.9/src/napari_bacseg/_utils_oufti.py
+-rw-rw-rw-   0        0        0     2132 2023-02-27 13:15:54.000000 napari-bacseg-1.0.9/src/napari_bacseg/_utils_refine.py
+-rw-rw-rw-   0        0        0    22517 2023-06-09 14:18:42.000000 napari-bacseg-1.0.9/src/napari_bacseg/_utils_statistics.py
+-rw-rw-rw-   0        0        0     7837 2023-06-09 14:18:42.000000 napari-bacseg-1.0.9/src/napari_bacseg/_utils_tiler.py
+-rw-rw-rw-   0        0        0    13358 2023-07-17 09:44:19.000000 napari-bacseg-1.0.9/src/napari_bacseg/_utils_zeiss.py
+-rw-rw-rw-   0        0        0      164 2023-07-17 09:49:26.000000 napari-bacseg-1.0.9/src/napari_bacseg/_version.py
+-rw-rw-rw-   0        0        0   101226 2023-07-17 09:44:21.000000 napari-bacseg-1.0.9/src/napari_bacseg/_widget.py
+-rw-rw-rw-   0        0        0   188399 2023-07-17 09:44:24.000000 napari-bacseg-1.0.9/src/napari_bacseg/bacseg_ui.py
+-rw-rw-rw-   0        0        0   172734 2023-07-14 14:10:02.000000 napari-bacseg-1.0.9/src/napari_bacseg/bacseg_ui.ui
+-rw-rw-rw-   0        0        0      271 2023-02-27 13:15:54.000000 napari-bacseg-1.0.9/src/napari_bacseg/gapseq_ui.py
+-rw-rw-rw-   0        0        0      501 2023-03-07 17:38:57.000000 napari-bacseg-1.0.9/src/napari_bacseg/napari.yaml
+-rw-rw-rw-   0        0        0      271 2023-02-27 13:15:54.000000 napari-bacseg-1.0.9/src/napari_bacseg/napari_ui.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:49:27.750743 napari-bacseg-1.0.9/src/napari_bacseg.egg-info/
+-rw-rw-rw-   0        0        0     4732 2023-07-17 09:49:27.000000 napari-bacseg-1.0.9/src/napari_bacseg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3382 2023-07-17 09:49:27.000000 napari-bacseg-1.0.9/src/napari_bacseg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 09:49:27.000000 napari-bacseg-1.0.9/src/napari_bacseg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-07-17 09:49:27.000000 napari-bacseg-1.0.9/src/napari_bacseg.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      373 2023-07-17 09:49:27.000000 napari-bacseg-1.0.9/src/napari_bacseg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-07-17 09:49:27.000000 napari-bacseg-1.0.9/src/napari_bacseg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      644 2023-02-24 11:00:35.000000 napari-bacseg-1.0.9/tox.ini
```

### Comparing `napari-bacseg-1.0.8/.github/workflows/test_and_deploy.yml` & `napari-bacseg-1.0.9/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/.gitignore` & `napari-bacseg-1.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/.napari-hub/config.yml` & `napari-bacseg-1.0.9/.napari-hub/config.yml`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/.pre-commit-config.yaml` & `napari-bacseg-1.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/LICENSE` & `napari-bacseg-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/PKG-INFO` & `napari-bacseg-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-bacseg
-Version: 1.0.8
+Version: 1.0.9
 Summary: Bacterial segmentation and analysis platform than can inport/export files in multiple formats. Integrating many tools such as Cellpose, ColiCoords, Oufti/MicrobeTracker.
 Home-page: https://github.com/piedrro/napari-bacseg
 Author: Piers Turner
 Author-email: Piers Turner <piers.turner@physics.ox.ac.uk>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/piedrro/napari-bacseg
 Project-URL: Bug Tracker, https://github.com/piedrro/napari-bacseg/issues
```

### Comparing `napari-bacseg-1.0.8/README.md` & `napari-bacseg-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/pyproject.toml` & `napari-bacseg-1.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 [tool.isort]
 profile = "black"
 line_length = 79
 
 [project]
 name = "napari-bacseg"
-version = "1.0.8"
+version = "1.0.9"
 authors = [
   { name="Piers Turner", email="piers.turner@physics.ox.ac.uk"},
 ]
 description = "Bacterial segmentation and analysis platform than can inport/export files in multiple formats. Integrating many tools such as Cellpose, ColiCoords, Oufti/MicrobeTracker."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `napari-bacseg-1.0.8/setup.cfg` & `napari-bacseg-1.0.9/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -85,44 +85,45 @@
 00000540: 7065 6e70 7978 6c0d 0a09 7368 6170 656c  penpyxl...shapel
 00000550: 790d 0a09 636f 6c69 636f 6f72 6473 0d0a  y...colicoords..
 00000560: 0973 6369 6b69 742d 696d 6167 650d 0a09  .scikit-image...
 00000570: 7368 6170 656c 790d 0a09 7073 7574 696c  shapely...psutil
 00000580: 0d0a 0978 6d6c 746f 6469 6374 0d0a 0961  ...xmltodict...a
 00000590: 7374 726f 7079 0d0a 0974 696c 6572 0d0a  stropy...tiler..
 000005a0: 0969 6d61 6765 696f 2d66 666d 7065 670d  .imageio-ffmpeg.
-000005b0: 0a09 6d61 7470 6c6f 746c 6962 0d0a 7079  ..matplotlib..py
-000005c0: 7468 6f6e 5f72 6571 7569 7265 7320 3d20  thon_requires = 
-000005d0: 3e3d 332e 390d 0a69 6e63 6c75 6465 5f70  >=3.9..include_p
-000005e0: 6163 6b61 6765 5f64 6174 6120 3d20 5472  ackage_data = Tr
-000005f0: 7565 0d0a 7061 636b 6167 655f 6469 7220  ue..package_dir 
-00000600: 3d20 0d0a 093d 7372 630d 0a73 6574 7570  = ...=src..setup
-00000610: 5f72 6571 7569 7265 7320 3d20 7365 7475  _requires = setu
-00000620: 7074 6f6f 6c73 5f73 636d 0d0a 0d0a 5b6f  ptools_scm....[o
-00000630: 7074 696f 6e73 2e70 6163 6b61 6765 732e  ptions.packages.
-00000640: 6669 6e64 5d0d 0a77 6865 7265 203d 2073  find]..where = s
-00000650: 7263 0d0a 0d0a 5b6f 7074 696f 6e73 2e65  rc....[options.e
-00000660: 6e74 7279 5f70 6f69 6e74 735d 0d0a 6e61  ntry_points]..na
-00000670: 7061 7269 2e6d 616e 6966 6573 7420 3d20  pari.manifest = 
-00000680: 0d0a 096e 6170 6172 692d 6261 6373 6567  ...napari-bacseg
-00000690: 203d 206e 6170 6172 695f 6261 6373 6567   = napari_bacseg
-000006a0: 3a6e 6170 6172 692e 7961 6d6c 0d0a 0d0a  :napari.yaml....
-000006b0: 5b6f 7074 696f 6e73 2e65 7874 7261 735f  [options.extras_
-000006c0: 7265 7175 6972 655d 0d0a 7465 7374 696e  require]..testin
-000006d0: 6720 3d20 0d0a 0974 6f78 0d0a 0970 7974  g = ...tox...pyt
-000006e0: 6573 7420 2023 2068 7474 7073 3a2f 2f64  est  # https://d
-000006f0: 6f63 732e 7079 7465 7374 2e6f 7267 2f65  ocs.pytest.org/e
-00000700: 6e2f 6c61 7465 7374 2f63 6f6e 7465 6e74  n/latest/content
-00000710: 732e 6874 6d6c 0d0a 0970 7974 6573 742d  s.html...pytest-
-00000720: 636f 7620 2023 2068 7474 7073 3a2f 2f70  cov  # https://p
-00000730: 7974 6573 742d 636f 762e 7265 6164 7468  ytest-cov.readth
-00000740: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
-00000750: 7374 2f0d 0a09 7079 7465 7374 2d71 7420  st/...pytest-qt 
-00000760: 2023 2068 7474 7073 3a2f 2f70 7974 6573   # https://pytes
-00000770: 742d 7174 2e72 6561 6474 6865 646f 6373  t-qt.readthedocs
-00000780: 2e69 6f2f 656e 2f6c 6174 6573 742f 0d0a  .io/en/latest/..
-00000790: 096e 6170 6172 690d 0a09 7079 7174 350d  .napari...pyqt5.
-000007a0: 0a0d 0a5b 6f70 7469 6f6e 732e 7061 636b  ...[options.pack
-000007b0: 6167 655f 6461 7461 5d0d 0a2a 203d 202a  age_data]..* = *
-000007c0: 2e79 616d 6c0d 0a0d 0a5b 6567 675f 696e  .yaml....[egg_in
-000007d0: 666f 5d0d 0a74 6167 5f62 7569 6c64 203d  fo]..tag_build =
-000007e0: 200d 0a74 6167 5f64 6174 6520 3d20 300d   ..tag_date = 0.
-000007f0: 0a0d 0a                                  ...
+000005b0: 0a09 6d61 7470 6c6f 746c 6962 0d0a 0961  ..matplotlib...a
+000005c0: 6963 7370 796c 6962 637a 690d 0a09 637a  icspylibczi...cz
+000005d0: 6966 696c 650d 0a70 7974 686f 6e5f 7265  ifile..python_re
+000005e0: 7175 6972 6573 203d 203e 3d33 2e39 0d0a  quires = >=3.9..
+000005f0: 696e 636c 7564 655f 7061 636b 6167 655f  include_package_
+00000600: 6461 7461 203d 2054 7275 650d 0a70 6163  data = True..pac
+00000610: 6b61 6765 5f64 6972 203d 200d 0a09 3d73  kage_dir = ...=s
+00000620: 7263 0d0a 7365 7475 705f 7265 7175 6972  rc..setup_requir
+00000630: 6573 203d 2073 6574 7570 746f 6f6c 735f  es = setuptools_
+00000640: 7363 6d0d 0a0d 0a5b 6f70 7469 6f6e 732e  scm....[options.
+00000650: 7061 636b 6167 6573 2e66 696e 645d 0d0a  packages.find]..
+00000660: 7768 6572 6520 3d20 7372 630d 0a0d 0a5b  where = src....[
+00000670: 6f70 7469 6f6e 732e 656e 7472 795f 706f  options.entry_po
+00000680: 696e 7473 5d0d 0a6e 6170 6172 692e 6d61  ints]..napari.ma
+00000690: 6e69 6665 7374 203d 200d 0a09 6e61 7061  nifest = ...napa
+000006a0: 7269 2d62 6163 7365 6720 3d20 6e61 7061  ri-bacseg = napa
+000006b0: 7269 5f62 6163 7365 673a 6e61 7061 7269  ri_bacseg:napari
+000006c0: 2e79 616d 6c0d 0a0d 0a5b 6f70 7469 6f6e  .yaml....[option
+000006d0: 732e 6578 7472 6173 5f72 6571 7569 7265  s.extras_require
+000006e0: 5d0d 0a74 6573 7469 6e67 203d 200d 0a09  ]..testing = ...
+000006f0: 746f 780d 0a09 7079 7465 7374 2020 2320  tox...pytest  # 
+00000700: 6874 7470 733a 2f2f 646f 6373 2e70 7974  https://docs.pyt
+00000710: 6573 742e 6f72 672f 656e 2f6c 6174 6573  est.org/en/lates
+00000720: 742f 636f 6e74 656e 7473 2e68 746d 6c0d  t/contents.html.
+00000730: 0a09 7079 7465 7374 2d63 6f76 2020 2320  ..pytest-cov  # 
+00000740: 6874 7470 733a 2f2f 7079 7465 7374 2d63  https://pytest-c
+00000750: 6f76 2e72 6561 6474 6865 646f 6373 2e69  ov.readthedocs.i
+00000760: 6f2f 656e 2f6c 6174 6573 742f 0d0a 0970  o/en/latest/...p
+00000770: 7974 6573 742d 7174 2020 2320 6874 7470  ytest-qt  # http
+00000780: 733a 2f2f 7079 7465 7374 2d71 742e 7265  s://pytest-qt.re
+00000790: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
+000007a0: 6c61 7465 7374 2f0d 0a09 6e61 7061 7269  latest/...napari
+000007b0: 0d0a 0970 7971 7435 0d0a 0d0a 5b6f 7074  ...pyqt5....[opt
+000007c0: 696f 6e73 2e70 6163 6b61 6765 5f64 6174  ions.package_dat
+000007d0: 615d 0d0a 2a20 3d20 2a2e 7961 6d6c 0d0a  a]..* = *.yaml..
+000007e0: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
+000007f0: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
+00000800: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
```

### Comparing `napari-bacseg-1.0.8/src/_dev/Export Masks to AKSEG v5 dev.py` & `napari-bacseg-1.0.9/src/_dev/Export Masks to AKSEG v5 dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/ScanR dev.py` & `napari-bacseg-1.0.9/src/_dev/ScanR dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/akseg_db_stats.py` & `napari-bacseg-1.0.9/src/_dev/akseg_db_stats.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/akseg_dev.py` & `napari-bacseg-1.0.9/src/_dev/akseg_dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/akseg_dev2.py` & `napari-bacseg-1.0.9/src/_dev/akseg_dev2.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/akseg_txt_metadata.py` & `napari-bacseg-1.0.9/src/_dev/akseg_txt_metadata.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/align_alex_datadump.py` & `napari-bacseg-1.0.9/src/_dev/align_alex_datadump.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/alison_datadump.py` & `napari-bacseg-1.0.9/src/_dev/alison_datadump.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/autocontast_dev.py` & `napari-bacseg-1.0.9/src/_dev/autocontast_dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/chatGPT_midlines.py` & `napari-bacseg-1.0.9/src/_dev/chatGPT_midlines.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/check_AluGasketv12_DFP.py` & `napari-bacseg-1.0.9/src/_dev/check_AluGasketv12_DFP.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/check_metadata.py` & `napari-bacseg-1.0.9/src/_dev/check_metadata.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/colicoords_cellldist_dev.py` & `napari-bacseg-1.0.9/src/_dev/colicoords_cellldist_dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/colicoords_ldist_dev.py` & `napari-bacseg-1.0.9/src/_dev/colicoords_ldist_dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/database_dev.py` & `napari-bacseg-1.0.9/src/_dev/database_dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/deepsegmattest.py` & `napari-bacseg-1.0.9/src/_dev/deepsegmattest.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/edit_database_columns.py` & `napari-bacseg-1.0.9/src/_dev/edit_database_columns.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/fits_dev.py` & `napari-bacseg-1.0.9/src/_dev/fits_dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/fix_alison_missing_file_list.py` & `napari-bacseg-1.0.9/src/_dev/fix_alison_missing_file_list.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/generate_scanr_movie.py` & `napari-bacseg-1.0.9/src/_dev/generate_scanr_movie.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/get_akseg_stats.py` & `napari-bacseg-1.0.9/src/_dev/get_akseg_stats.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/get_species_info.py` & `napari-bacseg-1.0.9/src/_dev/get_species_info.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/imagej_dev.py` & `napari-bacseg-1.0.9/src/_dev/imagej_dev.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 
 
 def read_imagej_file(path, image, widget_notifications=True):
     
     contours = []
     mask = np.zeros(image.shape[-2:])
     
-    
-
     # reads overlays sequentially and then converts them to openCV contours
     try:
         for roi in roiread(path):
             coordinates = roi.integer_coordinates
 
             top = roi.top
             left = roi.left
```

### Comparing `napari-bacseg-1.0.8/src/_dev/json_nuclei_dev.py` & `napari-bacseg-1.0.9/src/_dev/json_nuclei_dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/luke__script.py` & `napari-bacseg-1.0.9/src/_dev/luke__script.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/matplotlib_Events.py` & `napari-bacseg-1.0.9/src/_dev/matplotlib_Events.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/move_AluGasketDFP.py` & `napari-bacseg-1.0.9/src/_dev/move_AluGasketDFP.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/move_AluGasketDFP_poster.py` & `napari-bacseg-1.0.9/src/_dev/move_AluGasketDFP_poster.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/move_AluGasketv12_DFP.py` & `napari-bacseg-1.0.9/src/_dev/move_AluGasketv12_DFP.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/move_AluGasketv12_DFP_Titration.py` & `napari-bacseg-1.0.9/src/_dev/move_AluGasketv12_DFP_Titration.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/move_conor_nim_dfp_data.py` & `napari-bacseg-1.0.9/src/_dev/move_conor_nim_dfp_data.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/move_pillar_data.py` & `napari-bacseg-1.0.9/src/_dev/move_pillar_data.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/move_pillar_zstack_data.py` & `napari-bacseg-1.0.9/src/_dev/move_pillar_zstack_data.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/move_unlearning_files.py` & `napari-bacseg-1.0.9/src/_dev/move_unlearning_files.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/new_metadata2.pickle.py` & `napari-bacseg-1.0.9/src/_dev/new_metadata2.pickle.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/new_read_akseg_directory.py` & `napari-bacseg-1.0.9/src/_dev/new_read_akseg_directory.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/nim_dev.py` & `napari-bacseg-1.0.9/src/_dev/nim_dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/omnipose_dev.py` & `napari-bacseg-1.0.9/src/_dev/omnipose_dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/omnipose_midlines.py` & `napari-bacseg-1.0.9/src/_dev/omnipose_midlines.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/omnipose_train.py` & `napari-bacseg-1.0.9/src/_dev/omnipose_train.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/oufti_dilate.py` & `napari-bacseg-1.0.9/src/_dev/oufti_dilate.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/oufti_dilate_with_midlines.py` & `napari-bacseg-1.0.9/src/_dev/oufti_dilate_with_midlines.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/pandas_speed.py` & `napari-bacseg-1.0.9/src/_dev/pandas_speed.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/process_alex_datadump.py` & `napari-bacseg-1.0.9/src/_dev/process_alex_datadump.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/process_alex_datadump_clinical.py` & `napari-bacseg-1.0.9/src/_dev/process_alex_datadump_clinical.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/process_conor_datadump.py` & `napari-bacseg-1.0.9/src/_dev/process_conor_datadump.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/process_gramstain_datadump.py` & `napari-bacseg-1.0.9/src/_dev/process_gramstain_datadump.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/read_non_tif.py` & `napari-bacseg-1.0.9/src/_dev/read_non_tif.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/rebuild_usermeta.py` & `napari-bacseg-1.0.9/src/_dev/rebuild_usermeta.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/rebuild_usermeta_2.py` & `napari-bacseg-1.0.9/src/_dev/rebuild_usermeta_2.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/recreate_user_metadata.py` & `napari-bacseg-1.0.9/src/_dev/recreate_user_metadata.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/scalebar_dev.py` & `napari-bacseg-1.0.9/src/_dev/scalebar_dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/sort_midlines.py` & `napari-bacseg-1.0.9/src/_dev/sort_midlines.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/stelios_stats.py` & `napari-bacseg-1.0.9/src/_dev/stelios_stats.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/tile_meta_check.py` & `napari-bacseg-1.0.9/src/_dev/tile_meta_check.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/tiler_dev.py` & `napari-bacseg-1.0.9/src/_dev/tiler_dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/updade_akseg_metadata.py` & `napari-bacseg-1.0.9/src/_dev/updade_akseg_metadata.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/update_img_metadata.py` & `napari-bacseg-1.0.9/src/_dev/update_img_metadata.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/video_iamges.py` & `napari-bacseg-1.0.9/src/_dev/video_iamges.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/zooniverse.py` & `napari-bacseg-1.0.9/src/_dev/zooniverse.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/zooniverse_move.py` & `napari-bacseg-1.0.9/src/_dev/zooniverse_move.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/zooniverse_move_titrations.py` & `napari-bacseg-1.0.9/src/_dev/zooniverse_move_titrations.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/zooniverse_titration_upload.py` & `napari-bacseg-1.0.9/src/_dev/zooniverse_titration_upload.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/zooniverse_titrations.py` & `napari-bacseg-1.0.9/src/_dev/zooniverse_titrations.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/_dev/zooniverse_upload.py` & `napari-bacseg-1.0.9/src/_dev/zooniverse_upload.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/napari_bacseg/_tests/test_bacseg.py` & `napari-bacseg-1.0.9/src/napari_bacseg/_tests/test_bacseg.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/napari_bacseg/_tests/test_widget.py` & `napari-bacseg-1.0.9/src/napari_bacseg/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/napari_bacseg/_utils.py` & `napari-bacseg-1.0.9/src/napari_bacseg/_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import copy
 import hashlib
 import json
 import os
 
 # from napari_bacseg._utils_cellpose import export_cellpose
 # from napari_bacseg._utils_oufti import  export_oufti
 # from napari_bacseg._utils_imagej import export_imagej
@@ -20,15 +21,15 @@
 from astropy.io import fits
 from glob2 import glob
 from napari.utils.notifications import show_info
 
 # from napari_bacseg._utils_imagej import read_imagej_file
 from skimage import exposure
 from skimage.registration import phase_cross_correlation
-import copy
+
 
 def normalize99(X):
     """normalize image so 0.0 is 0.01st percentile and 1.0 is 99.99th percentile"""
 
     if np.max(X) > 0:
         X = X.copy()
         v_min, v_max = np.percentile(X[X != 0], (0.1, 99.9))
@@ -58,43 +59,57 @@
 
                 if type(image_list) == dict:
                     image_list = [image_list]
 
                 for i in range(len(image_list)):
                     img = image_list[i]
 
-                    objective_id = int(img["ObjectiveSettings"]["@ID"].split(":")[-1])
-                    objective_dat = dat["Instrument"]["Objective"][objective_id]
-                    objective_mag = float(objective_dat["@NominalMagnification"])
+                    objective_id = int(
+                        img["ObjectiveSettings"]["@ID"].split(":")[-1]
+                    )
+                    objective_dat = dat["Instrument"]["Objective"][
+                        objective_id
+                    ]
+                    objective_mag = float(
+                        objective_dat["@NominalMagnification"]
+                    )
                     objective_na = float(objective_dat["@LensNA"])
 
                     pixel_size = float(img["Pixels"]["@PhysicalSizeX"])
 
                     position_index = i
                     microscope = "ScanR"
                     light_source = "LED"
 
                     channel_dict = {}
 
                     for j in range(len(img["Pixels"]["Channel"])):
                         channel_data = img["Pixels"]["Channel"][j]
 
-                        channel_dict[j] = dict(modality=channel_data["@IlluminationType"], channel=channel_data["@Name"], mode=channel_data["@AcquisitionMode"], well=
-                        channel_data["@ID"].split("W")[1].split("P")[0], )
+                        channel_dict[j] = dict(
+                            modality=channel_data["@IlluminationType"],
+                            channel=channel_data["@Name"],
+                            mode=channel_data["@AcquisitionMode"],
+                            well=channel_data["@ID"]
+                            .split("W")[1]
+                            .split("P")[0],
+                        )
 
                     primary_channel = ""
 
                     for j in range(len(img["Pixels"]["TiffData"])):
                         num_channels = img["Pixels"]["@SizeC"]
                         num_zstack = img["Pixels"]["@SizeZ"]
 
                         tiff_data = img["Pixels"]["TiffData"][j]
 
                         file_name = tiff_data["UUID"]["@FileName"]
-                        file_path = os.path.abspath(path.replace(os.path.basename(path), file_name))
+                        file_path = os.path.abspath(
+                            path.replace(os.path.basename(path), file_name)
+                        )
 
                         try:
                             plane_data = img["Pixels"]["Plane"][j]
                             exposure_time = plane_data["@ExposureTime"]
                             posX = float(plane_data["@PositionX"])
                             posY = float(plane_data["@PositionY"])
                             posZ = float(plane_data["@PositionZ"])
@@ -117,16 +132,33 @@
                             time_index = None
                             z_index = None
                             channel_dat = None
                             modality = None
                             channel = None
                             well_index = None
 
-                        files[
-                            file_path] = dict(file_name=file_name, well_index=well_index, position_index=position_index, channel_index=channel_index, time_index=time_index, z_index=z_index, microscope=microscope, light_source=light_source, channel=channel, modality=modality, pixel_size=pixel_size, objective_magnification=objective_mag, objective_na=objective_na, exposure_time=exposure_time, posX=posX, posY=posY, posZ=posZ, )
+                        files[file_path] = dict(
+                            file_name=file_name,
+                            well_index=well_index,
+                            position_index=position_index,
+                            channel_index=channel_index,
+                            time_index=time_index,
+                            z_index=z_index,
+                            microscope=microscope,
+                            light_source=light_source,
+                            channel=channel,
+                            modality=modality,
+                            pixel_size=pixel_size,
+                            objective_magnification=objective_mag,
+                            objective_na=objective_na,
+                            exposure_time=exposure_time,
+                            posX=posX,
+                            posY=posY,
+                            posZ=posZ,
+                        )
     except:
         print(traceback.format_exc())
 
     return files
 
 
 def read_scanr_directory(self, path):
@@ -138,29 +170,39 @@
 
         if len(path) == 1:
             path = os.path.abspath(path[0])
 
             if os.path.isfile(path) == True:
                 selected_paths = [path]
                 image_path = os.path.abspath(path)
-                file_directory = os.path.abspath(image_path.split(image_path.split("\\")[-1])[0])
+                file_directory = os.path.abspath(
+                    image_path.split(image_path.split("\\")[-1])[0]
+                )
                 file_paths = glob(file_directory + r"*\*.tif")
 
             else:
                 file_paths = glob(path + r"*\**\*.tif", recursive=True)
                 selected_paths = []
         else:
             selected_paths = [os.path.abspath(path) for path in path]
             image_path = os.path.abspath(path[0])
-            file_directory = os.path.abspath(image_path.split(image_path.split("\\")[-1])[0])
+            file_directory = os.path.abspath(
+                image_path.split(image_path.split("\\")[-1])[0]
+            )
             file_paths = glob(file_directory + r"*\*.tif")
 
-        scanR_meta_files = [path.replace(os.path.basename(path), "") for path in file_paths]
+        scanR_meta_files = [
+            path.replace(os.path.basename(path), "") for path in file_paths
+        ]
         scanR_meta_files = np.unique(scanR_meta_files).tolist()
-        scanR_meta_files = [glob(path + "*.ome.xml")[0] for path in scanR_meta_files if len(glob(path + "*.ome.xml")) > 0]
+        scanR_meta_files = [
+            glob(path + "*.ome.xml")[0]
+            for path in scanR_meta_files
+            if len(glob(path + "*.ome.xml")) > 0
+        ]
 
         file_info = read_xml(scanR_meta_files)
 
         files = []
 
         for path in file_paths:
             try:
@@ -199,39 +241,55 @@
             if int(import_limit) > num_measurements:
                 import_limit = num_measurements
 
         acquisitions = files.position_index.unique()[: int(import_limit)]
 
         files = files[files["position_index"] <= acquisitions[-1]]
 
-        measurements = files.groupby(by=["parent_folder", "position_index", "time_index", "z_index"])
+        measurements = files.groupby(
+            by=["parent_folder", "position_index", "time_index", "z_index"]
+        )
 
         if selected_paths != []:
             filtered_measurements = []
 
             for i in range(len(measurements)):
-                measurement = measurements.get_group(list(measurements.groups)[i])
+                measurement = measurements.get_group(
+                    list(measurements.groups)[i]
+                )
                 measurement_paths = measurement["path"].tolist()
 
-                selected_paths = [os.path.abspath(path) for path in selected_paths]
-                measurement_paths = [os.path.abspath(path) for path in measurement_paths]
+                selected_paths = [
+                    os.path.abspath(path) for path in selected_paths
+                ]
+                measurement_paths = [
+                    os.path.abspath(path) for path in measurement_paths
+                ]
 
                 if not set(selected_paths).isdisjoint(measurement_paths):
                     filtered_measurements.append(measurement)
 
             filtered_measurements = pd.concat(filtered_measurements)
 
-            measurements = filtered_measurements.groupby(by=["folder", "position_index", "time_index", "z_index"])
+            measurements = filtered_measurements.groupby(
+                by=["folder", "position_index", "time_index", "z_index"]
+            )
 
         channels = files["channel"].drop_duplicates().to_list()
 
         channel_num = str(len(files["channel"].unique()))
 
         if self.widget_notifications:
-            show_info("Found " + str(len(measurements)) + " measurments in ScanR Folder(s) with " + channel_num + " channels.")
+            show_info(
+                "Found "
+                + str(len(measurements))
+                + " measurments in ScanR Folder(s) with "
+                + channel_num
+                + " channels."
+            )
 
     except:
         measurements, file_paths, channels = None, None, None
         print(traceback.format_exc())
 
     return measurements, file_paths, channels
 
@@ -263,30 +321,39 @@
 
             try:
                 progress_callback.emit(progress)
             except:
                 pass
 
             if self.widget_notifications:
-                show_info("loading image[" + channel + "] " + str(i + 1) + " of " + str(len(measurements)))
+                show_info(
+                    "loading image["
+                    + channel
+                    + "] "
+                    + str(i + 1)
+                    + " of "
+                    + str(len(measurements))
+                )
 
             if channel in measurement_channels:
                 dat = measurement[measurement["channel"] == channel]
 
                 path = dat["path"].item()
                 laser = "LED"
                 folder = dat["folder"].item()
                 parent_folder = dat["parent_folder"].item()
                 modality = dat["modality"].item()
 
                 import_precision = self.import_precision.currentText()
                 multiframe_mode = self.import_multiframe_mode.currentIndex()
                 crop_mode = self.import_crop_mode.currentIndex()
 
-                img, meta = read_image_file(path, import_precision, multiframe_mode, crop_mode)
+                img, meta = read_image_file(
+                    path, import_precision, multiframe_mode, crop_mode
+                )
 
                 contrast_limit, alpha, beta, gamma = autocontrast_values(img)
 
                 self.active_import_mode = "ScanR"
 
                 meta["image_name"] = os.path.basename(path)
                 meta["image_path"] = path
@@ -333,26 +400,31 @@
                 meta["contrast_beta"] = None
                 meta["contrast_gamma"] = None
                 meta["dims"] = [img.shape[-1], img.shape[-2]]
                 meta["crop"] = [0, img.shape[-2], 0, img.shape[-1]]
                 meta["light_source"] = channel
 
             if channel not in scanr_images:
-                scanr_images[channel] = dict(images=[img], masks=[], nmasks=[], classes=[], metadata={i: meta}, )
+                scanr_images[channel] = dict(
+                    images=[img],
+                    masks=[],
+                    nmasks=[],
+                    classes=[],
+                    metadata={i: meta},
+                )
             else:
                 scanr_images[channel]["images"].append(img)
                 scanr_images[channel]["metadata"][i] = meta
 
     imported_data = dict(imported_images=scanr_images)
 
     return imported_data
 
 
 def import_imagej(self, progress_callback, paths):
-
     if isinstance(paths, list) == False:
         paths = [paths]
 
     if len(paths) == 1:
         paths = os.path.abspath(paths[0])
 
         if os.path.isfile(paths) == True:
@@ -377,42 +449,50 @@
         progress = int(((i + 1) / len(file_paths)) * 100)
         try:
             progress_callback.emit(progress)
         except:
             pass
 
         if self.widget_notifications:
-            show_info("loading image " + str(i + 1) + " of " + str(len(file_paths)))
+            show_info(
+                "loading image " + str(i + 1) + " of " + str(len(file_paths))
+            )
 
         paths = file_paths[i]
         paths = os.path.abspath(paths)
 
         import_precision = self.import_precision.currentText()
         multiframe_mode = self.import_multiframe_mode.currentIndex()
         crop_mode = self.import_crop_mode.currentIndex()
 
-        image_list, meta = read_image_file(paths, import_precision, multiframe_mode, crop_mode)
+        image_list, meta = read_image_file(
+            paths, import_precision, multiframe_mode, crop_mode
+        )
 
         akseg_hash = get_hash(img_path=paths)
 
         from napari_bacseg._utils_imagej import read_imagej_file
 
         file_name = os.path.basename(paths)
 
         for index, frame in enumerate(image_list):
-
             contrast_limit = np.percentile(frame, (1, 99))
-            contrast_limit = [int(contrast_limit[0] * 0.5), int(contrast_limit[1] * 2), ]
+            contrast_limit = [
+                int(contrast_limit[0] * 0.5),
+                int(contrast_limit[1] * 2),
+            ]
 
             mask = read_imagej_file(paths, frame)
 
             self.active_import_mode = "imagej"
 
             if len(image_list) > 1:
-                frame_name = file_name.replace(".", "_") + "_" + str(index) + ".tif"
+                frame_name = (
+                    file_name.replace(".", "_") + "_" + str(index) + ".tif"
+                )
             else:
                 frame_name = copy.deepcopy(file_name)
 
             frame_meta = copy.deepcopy(meta)
 
             frame_meta["akseg_hash"] = akseg_hash
             frame_meta["image_name"] = frame_name
@@ -430,15 +510,21 @@
             frame_meta["crop"] = [0, frame.shape[-2], 0, frame.shape[-1]]
 
             images.append(frame)
             masks.append(mask)
             metadata[img_index] = frame_meta
 
             if imported_images == {}:
-                imported_images["Image"] = dict(images=[frame], masks=[mask], nmasks=[], classes=[], metadata={img_index: frame_meta}, )
+                imported_images["Image"] = dict(
+                    images=[frame],
+                    masks=[mask],
+                    nmasks=[],
+                    classes=[],
+                    metadata={img_index: frame_meta},
+                )
             else:
                 imported_images["Image"]["images"].append(frame)
                 imported_images["Image"]["masks"].append(mask)
                 imported_images["Image"]["metadata"][img_index] = frame_meta
 
             img_index += 1
 
@@ -447,15 +533,14 @@
     for i in range(len(imported_images["Image"]["images"])):
         print(i, imported_images["Image"]["metadata"][i]["image_name"], i)
 
     return imported_data
 
 
 def read_nim_directory(self, path):
-
     if isinstance(path, list) == False:
         path = [path]
 
     if len(path) == 1:
         path = os.path.abspath(path[0])
 
         if os.path.isfile(path) == True:
@@ -466,15 +551,27 @@
     else:
         file_paths = path
 
     file_paths = [file for file in file_paths if file.split(".")[-1] == "tif"]
 
     file_names = [path.split("\\")[-1] for path in file_paths]
 
-    files = pd.DataFrame(columns=["path", "file_name", "folder", "parent_folder", "posX", "posY", "posZ", "laser", "timestamp", ])
+    files = pd.DataFrame(
+        columns=[
+            "path",
+            "file_name",
+            "folder",
+            "parent_folder",
+            "posX",
+            "posY",
+            "posZ",
+            "laser",
+            "timestamp",
+        ]
+    )
 
     for i in range(len(file_paths)):
         try:
             path = file_paths[i]
             path = os.path.abspath(path)
 
             file_name = path.split("\\")[-1]
@@ -497,37 +594,53 @@
                 timestamp = metadata["timestamp_us"]
 
                 posX, posY, posZ = metadata["StagePos_um"]
 
                 if True in laseractive:
                     laseractive = np.array(laseractive, dtype=bool)
                     laserpowers = np.array(laserpowers, dtype=float)
-                    laserwavelength_nm = np.array(laserwavelength_nm, dtype=str)
+                    laserwavelength_nm = np.array(
+                        laserwavelength_nm, dtype=str
+                    )
 
                     # finds maximum active power
                     power = laserpowers[laseractive == True].max()
 
                     laser_index = np.where(laserpowers == power)
 
                     laser = laserwavelength_nm[laser_index][0]
                 else:
                     laser = "White Light"
 
                 file_name = path.split("\\")[-1]
 
                 data = [path, file_name, posX, posY, posZ, laser, timestamp]
 
-                files.loc[len(files)] = [path, file_name, folder, parent_folder, posX, posY, posZ, laser, timestamp, ]
+                files.loc[len(files)] = [
+                    path,
+                    file_name,
+                    folder,
+                    parent_folder,
+                    posX,
+                    posY,
+                    posZ,
+                    laser,
+                    timestamp,
+                ]
 
         except:
             pass
 
-    files[["posX", "posY", "posZ"]] = files[["posX", "posY", "posZ"]].round(decimals=0)
-
-    files = files.sort_values(by=["timestamp", "posX", "posY", "laser"], ascending=True)
+    files[["posX", "posY", "posZ"]] = files[["posX", "posY", "posZ"]].round(
+        decimals=0
+    )
+
+    files = files.sort_values(
+        by=["timestamp", "posX", "posY", "laser"], ascending=True
+    )
     files = files.reset_index(drop=True)
     files["aquisition"] = 0
 
     positions = files[["posX", "posY"]].drop_duplicates()
     channels = files["laser"].drop_duplicates().to_list()
 
     acquisition = 0
@@ -574,15 +687,21 @@
 
     measurements = files.groupby(by=["aquisition"])
     channels = files["laser"].drop_duplicates().to_list()
 
     channel_num = str(len(files["laser"].unique()))
 
     if self.widget_notifications:
-        show_info("Found " + str(len(measurements)) + " measurments in NIM Folder with " + channel_num + " channels.")
+        show_info(
+            "Found "
+            + str(len(measurements))
+            + " measurments in NIM Folder with "
+            + channel_num
+            + " channels."
+        )
 
     return measurements, file_paths, channels
 
 
 def get_folder(files):
     folder = ""
     parent_folder = ""
@@ -603,24 +722,27 @@
         folder = paths[0].split("\\")[-2]
         parent_folder = paths[0].split("\\")[-3]
 
     return folder, parent_folder
 
 
 def read_image_file(path, precision="native", multiframe_mode=0, crop_mode=0):
-
     image_name = os.path.basename(path)
 
     if os.path.splitext(image_name)[1] == ".fits":
         with fits.open(path, ignore_missing_simple=True) as hdul:
             image = hdul[0].data
             try:
                 metadata = dict(hdul[0].header)
 
-                unserializable_keys = [key for key, value in metadata.items() if type(value) not in [bool, int, float, str]]
+                unserializable_keys = [
+                    key
+                    for key, value in metadata.items()
+                    if type(value) not in [bool, int, float, str]
+                ]
 
                 for key in unserializable_keys:
                     metadata.pop(key)
 
             except:
                 metadata = {}
     else:
@@ -662,15 +784,14 @@
         metadata["dims"] = [image[0].shape[-1], image[0].shape[-2]]
         metadata["crop"] = [0, image[0].shape[-2], 0, image[0].shape[-1]]
 
     return image, metadata
 
 
 def get_frame(img, multiframe_mode):
-
     if len(img.shape) > 2:
         if multiframe_mode == 0:
             img = img[0, :, :]
 
         elif multiframe_mode == 1:
             img = np.max(img, axis=0)
 
@@ -686,22 +807,21 @@
     if type(img) != list:
         img = [img]
 
     return img
 
 
 def crop_image(img, crop_mode=0):
-
     if crop_mode != 0:
         if len(img.shape) > 2:
             imgL = img[:, :, : img.shape[-1] // 2]
-            imgR = img[:, :, img.shape[-1] // 2:]
+            imgR = img[:, :, img.shape[-1] // 2 :]
         else:
             imgL = img[:, : img.shape[-1] // 2]
-            imgR = img[:, img.shape[-1] // 2:]
+            imgR = img[:, img.shape[-1] // 2 :]
 
         if crop_mode == 1:
             img = imgL
         if crop_mode == 2:
             img = imgR
 
         if crop_mode == 3:
@@ -710,115 +830,135 @@
             else:
                 img = imgR
 
     return img
 
 
 def rescale_image(image, precision="int16"):
-
-    precision_dict = {"int8": np.uint8, "int16": np.uint16, "int32": np.uint32, "native": image[0].dtype, }
+    precision_dict = {
+        "int8": np.uint8,
+        "int16": np.uint16,
+        "int32": np.uint32,
+        "native": image[0].dtype,
+    }
 
     dtype = precision_dict[precision]
 
     if "int" in str(dtype):
         max_value = np.iinfo(dtype).max - 1
     else:
         max_value = np.finfo(dtype).max - 1
 
     if precision != "native":
-
         for i, img in enumerate(image):
             img = ((img - np.min(img)) / np.max(img)) * max_value
             img = img.astype(dtype)
             image[i] = img
 
     return image
 
 
 def read_nim_images(self, progress_callback, measurements, channels):
-
     nim_images = {}
     img_shape = (100, 100)
     num_frames = 1
     img_type = np.uint16
     iter = 0
 
     img_index = {}
 
     for i in range(len(measurements)):
-
         measurement = measurements.get_group(list(measurements.groups)[i])
         measurement_channels = measurement["laser"].tolist()
 
         for j in range(len(channels)):
-
             channel = channels[j]
 
             if channel not in img_index.keys():
                 img_index[channel] = 0
 
             iter += 1
             progress = int((iter / (len(measurements) * len(channels))) * 100)
 
             try:
                 progress_callback.emit(progress)
             except:
                 pass
 
             if self.widget_notifications:
-                show_info("loading image[" + channel + "] " + str(i + 1) + " of " + str(len(measurements)))
+                show_info(
+                    "loading image["
+                    + channel
+                    + "] "
+                    + str(i + 1)
+                    + " of "
+                    + str(len(measurements))
+                )
 
             if channel in measurement_channels:
-
                 dat = measurement[measurement["laser"] == channel]
 
                 path = dat["path"].item()
                 laser = dat["laser"].item()
                 folder = dat["folder"].item()
                 parent_folder = dat["parent_folder"].item()
 
                 import_precision = self.import_precision.currentText()
                 multiframe_mode = self.import_multiframe_mode.currentIndex()
                 crop_mode = self.import_crop_mode.currentIndex()
 
-                image_list, meta = read_image_file(path, import_precision, multiframe_mode, crop_mode)
+                image_list, meta = read_image_file(
+                    path, import_precision, multiframe_mode, crop_mode
+                )
 
                 num_frames = len(image_list)
 
                 akseg_hash = get_hash(img_path=path)
 
                 file_name = os.path.basename(path)
 
                 for index, frame in enumerate(image_list):
-
                     frame_name = copy.deepcopy(file_name)
                     frame_meta = copy.deepcopy(meta)
 
                     contrast_limit = np.percentile(frame, (1, 99))
-                    contrast_limit = [int(contrast_limit[0] * 0.5), int(contrast_limit[1] * 2), ]
+                    contrast_limit = [
+                        int(contrast_limit[0] * 0.5),
+                        int(contrast_limit[1] * 2),
+                    ]
 
                     self.active_import_mode = "nim"
 
                     if len(image_list) > 1:
-                        frame_name = frame_name.replace(".", "_") + "_" + str(index) + ".tif"
+                        frame_name = (
+                            frame_name.replace(".", "_")
+                            + "_"
+                            + str(index)
+                            + ".tif"
+                        )
 
                     self.active_import_mode = "NIM"
 
                     frame_meta["image_name"] = frame_name
                     frame_meta["image_path"] = path
                     frame_meta["folder"] = folder
                     frame_meta["parent_folder"] = parent_folder
                     frame_meta["akseg_hash"] = akseg_hash
                     frame_meta["import_mode"] = "NIM"
                     frame_meta["contrast_limit"] = contrast_limit
                     frame_meta["contrast_alpha"] = 0
                     frame_meta["contrast_beta"] = 0
                     frame_meta["contrast_gamma"] = 0
                     frame_meta["dims"] = [frame.shape[-1], frame.shape[-2]]
-                    frame_meta["crop"] = [0, frame.shape[-2], 0, frame.shape[-1]]
+                    frame_meta["crop"] = [
+                        0,
+                        frame.shape[-2],
+                        0,
+                        frame.shape[-1],
+                    ]
 
                     if frame_meta["InstrumentSerial"] == "6D699GN6":
                         frame_meta["microscope"] = "BIO-NIM"
                     elif frame_meta["InstrumentSerial"] == "2EC5XTUC":
                         frame_meta["microscope"] = "JR-NIM"
                     else:
                         frame_meta["microscope"] = None
@@ -838,27 +978,35 @@
                     img_shape = frame.shape
                     img_type = np.array(frame).dtype
 
                     image_path = frame_meta["image_path"]
 
                     if "pos_" in image_path:
                         frame_meta["folder"] = image_path.split("\\")[-4]
-                        frame_meta["parent_folder"] = image_path.split("\\")[-5]
+                        frame_meta["parent_folder"] = image_path.split("\\")[
+                            -5
+                        ]
 
                     if channel not in nim_images:
-                        nim_images[channel] = dict(images=[frame], masks=[], nmasks=[], classes=[], metadata={img_index[channel]: frame_meta}, )
+                        nim_images[channel] = dict(
+                            images=[frame],
+                            masks=[],
+                            nmasks=[],
+                            classes=[],
+                            metadata={img_index[channel]: frame_meta},
+                        )
                     else:
                         nim_images[channel]["images"].append(frame)
-                        nim_images[channel]["metadata"][img_index[channel]] = frame_meta
+                        nim_images[channel]["metadata"][
+                            img_index[channel]
+                        ] = frame_meta
 
                     img_index[channel] += 1
             else:
-
                 for index in range(num_frames):
-
                     frame = np.zeros(img_shape, dtype=img_type)
                     frame_meta = {}
 
                     self.active_import_mode = "NIM"
 
                     frame_meta["image_name"] = "missing image channel"
                     frame_meta["image_path"] = "missing image channel"
@@ -868,33 +1016,46 @@
                     frame_meta["fov_mode"] = None
                     frame_meta["import_mode"] = "NIM"
                     frame_meta["contrast_limit"] = None
                     frame_meta["contrast_alpha"] = None
                     frame_meta["contrast_beta"] = None
                     frame_meta["contrast_gamma"] = None
                     frame_meta["dims"] = [frame.shape[-1], frame.shape[-2]]
-                    frame_meta["crop"] = [0, frame.shape[-2], 0, frame.shape[-1]]
+                    frame_meta["crop"] = [
+                        0,
+                        frame.shape[-2],
+                        0,
+                        frame.shape[-1],
+                    ]
                     frame_meta["light_source"] = channel
 
                     if channel not in nim_images:
-                        nim_images[channel] = dict(images=[frame], masks=[], nmasks=[], classes=[], metadata={img_index[channel]: frame_meta}, )
+                        nim_images[channel] = dict(
+                            images=[frame],
+                            masks=[],
+                            nmasks=[],
+                            classes=[],
+                            metadata={img_index[channel]: frame_meta},
+                        )
                     else:
                         nim_images[channel]["images"].append(frame)
-                        nim_images[channel]["metadata"][img_index[channel]] = frame_meta
+                        nim_images[channel]["metadata"][
+                            img_index[channel]
+                        ] = frame_meta
 
                     img_index[channel] += 1
 
     imported_data = dict(imported_images=nim_images)
 
     return imported_data
 
 
 def get_brightest_fov(image):
     imageL = image[0, :, : image.shape[2] // 2]
-    imageR = image[0, :, image.shape[2] // 2:]
+    imageR = image[0, :, image.shape[2] // 2 :]
 
     if np.mean(imageL) > np.mean(imageR):
         image = image[:, :, : image.shape[2] // 2]
     else:
         image = image[:, :, : image.shape[2] // 2]
 
     return image
@@ -919,15 +1080,15 @@
             img = np.mean(img, axis=0).astype(np.uint16)
 
     return img
 
 
 def get_fov(img, channel_mode):
     imgL = img[:, : img.shape[1] // 2]
-    imgR = img[:, img.shape[1] // 2:]
+    imgR = img[:, img.shape[1] // 2 :]
 
     if channel_mode == 0:
         if np.mean(imgL) > np.mean(imgR):
             img = imgL
         else:
             img = imgR
     if channel_mode == 1:
@@ -1031,35 +1192,44 @@
             image_paths = image_paths[: int(import_limit)]
 
         for i in range(len(image_paths)):
             progress = int(((i + 1) / len(image_paths)) * 100)
             progress_callback.emit(progress)
 
             if self.widget_notifications:
-                show_info("loading image " + str(i + 1) + " of " + str(len(image_paths)))
+                show_info(
+                    "loading image "
+                    + str(i + 1)
+                    + " of "
+                    + str(len(image_paths))
+                )
 
             image_path = os.path.abspath(image_paths[i])
             mask_path = image_path.replace("\\images\\", "\\masks\\")
 
             image_name = image_path.split("\\")[-1]
             mask_name = mask_path.split("\\")[-1]
 
             import_precision = self.import_precision.currentText()
             multiframe_mode = self.import_multiframe_mode.currentIndex()
             crop_mode = self.import_crop_mode.currentIndex()
 
-            image, meta = read_image_file(path, import_precision, multiframe_mode)
+            image, meta = read_image_file(
+                path, import_precision, multiframe_mode
+            )
 
             crop_mode = self.import_crop_mode.currentIndex()
             image = crop_image(image, crop_mode)
 
             if os.path.exists(mask_path):
                 mask = tifffile.imread(mask_path)
                 mask = crop_image(mask, crop_mode)
-                assert (len(mask.shape) < 3), "Can only import single channel masks"
+                assert (
+                    len(mask.shape) < 3
+                ), "Can only import single channel masks"
 
             else:
                 mask_name = None
                 mask_path = None
                 mask = np.zeros(image.shape, dtype=np.uint16)
 
             contrast_limit, alpha, beta, gamma = autocontrast_values(image)
@@ -1081,15 +1251,21 @@
             meta["dims"] = [image.shape[-1], image.shape[-2]]
             meta["crop"] = [0, image.shape[-2], 0, image.shape[-1]]
 
             images.append(image)
             metadata[i] = meta
 
             if imported_images == {}:
-                imported_images["Image"] = dict(images=[image], masks=[mask], nmasks=[], classes=[], metadata={i: meta}, )
+                imported_images["Image"] = dict(
+                    images=[image],
+                    masks=[mask],
+                    nmasks=[],
+                    classes=[],
+                    metadata={i: meta},
+                )
             else:
                 imported_images["Image"]["images"].append(image)
                 imported_images["Image"]["masks"].append(mask)
                 imported_images["Image"]["metadata"][i] = meta
 
     imported_data = dict(imported_images=imported_images)
 
@@ -1121,36 +1297,51 @@
             image_paths = image_paths[: int(import_limit)]
 
         for i in range(len(image_paths)):
             progress = int(((i + 1) / len(image_paths)) * 100)
             progress_callback.emit(progress)
 
             if self.widget_notifications:
-                show_info("loading image " + str(i + 1) + " of " + str(len(image_paths)))
+                show_info(
+                    "loading image "
+                    + str(i + 1)
+                    + " of "
+                    + str(len(image_paths))
+                )
 
             image_path = os.path.abspath(image_paths[i])
-            json_path = image_path.replace("\\images\\", "\\json\\").replace(".tif", ".txt")
+            json_path = image_path.replace("\\images\\", "\\json\\").replace(
+                ".tif", ".txt"
+            )
 
             import_precision = self.import_precision.currentText()
-            image, meta_stack = read_image_file(path, import_precision, multiframe_mode=0)
+            image, meta_stack = read_image_file(
+                path, import_precision, multiframe_mode=0
+            )
 
             crop_mode = self.import_crop_mode.currentIndex()
             image = crop_image(image, crop_mode)
 
             if os.path.exists(json_path):
                 from napari_bacseg._utils_json import import_coco_json
 
                 mask, nmask, label = import_coco_json(json_path)
                 mask = crop_image(mask, crop_mode)
                 label = crop_image(label, crop_mode)
 
             else:
-                label = np.zeros((image.shape[0], image.shape[1]), dtype=np.uint16)
-                mask = np.zeros((image.shape[0], image.shape[1]), dtype=np.uint16)
-                nmask = np.zeros((image.shape[0], image.shape[1]), dtype=np.uint16)
+                label = np.zeros(
+                    (image.shape[0], image.shape[1]), dtype=np.uint16
+                )
+                mask = np.zeros(
+                    (image.shape[0], image.shape[1]), dtype=np.uint16
+                )
+                nmask = np.zeros(
+                    (image.shape[0], image.shape[1]), dtype=np.uint16
+                )
 
             for j, channel in enumerate(meta_stack["channels"]):
                 img = image[j, :, :]
 
                 contrast_limit, alpha, beta, gamma = autocontrast_values(img)
 
                 self.active_import_mode = "BacSeg"
@@ -1161,15 +1352,21 @@
                 meta["contrast_alpha"] = alpha
                 meta["contrast_beta"] = beta
                 meta["contrast_gamma"] = gamma
                 meta["dims"] = [img.shape[0], img.shape[1]]
                 meta["crop"] = [0, img.shape[1], 0, img.shape[0]]
 
                 if channel not in imported_images.keys():
-                    imported_images[channel] = dict(images=[img], masks=[mask], nmasks=[], classes=[label], metadata={i: meta}, )
+                    imported_images[channel] = dict(
+                        images=[img],
+                        masks=[mask],
+                        nmasks=[],
+                        classes=[label],
+                        metadata={i: meta},
+                    )
                 else:
                     imported_images[channel]["images"].append(img)
                     imported_images[channel]["masks"].append(mask)
                     imported_images[channel]["nmasks"].append(nmask)
                     imported_images[channel]["classes"].append(label)
                     imported_images[channel]["metadata"][i] = meta
 
@@ -1178,67 +1375,75 @@
 
     imported_data = dict(imported_images=imported_images, akmeta=akmeta)
 
     return imported_data
 
 
 def import_images(self, progress_callback, file_paths):
-
     if os.path.isdir(file_paths[0]):
         file_paths = glob(file_paths[0] + r"**\*", recursive=True)
 
     image_formats = ["tif", "png", "jpeg", "fits"]
 
-    file_paths = [path for path in file_paths if path.split(".")[-1] in image_formats]
+    file_paths = [
+        path for path in file_paths if path.split(".")[-1] in image_formats
+    ]
 
     import_limit = self.import_limit.currentText()
 
     if import_limit != "None" and len(file_paths) > int(import_limit):
         file_paths = file_paths[: int(import_limit)]
 
     images = []
     metadata = {}
     imported_images = {}
 
     img_index = 0
 
     for i in range(len(file_paths)):
-
         progress = int(((i + 1) / len(file_paths)) * 100)
 
         try:
             progress_callback.emit(progress)
         except:
             pass
 
         if self.widget_notifications:
-            show_info("loading image " + str(i + 1) + " of " + str(len(file_paths)))
+            show_info(
+                "loading image " + str(i + 1) + " of " + str(len(file_paths))
+            )
 
         file_path = os.path.abspath(file_paths[i])
         file_name = os.path.basename(file_path)
 
         import_precision = self.import_precision.currentText()
         multiframe_mode = self.import_multiframe_mode.currentIndex()
         crop_mode = self.import_crop_mode.currentIndex()
 
-        image_list, meta = read_image_file(file_path, import_precision, multiframe_mode, crop_mode)
+        image_list, meta = read_image_file(
+            file_path, import_precision, multiframe_mode, crop_mode
+        )
 
         akseg_hash = get_hash(img_path=file_path)
 
         file_name = os.path.basename(file_path)
 
         for index, frame in enumerate(image_list):
-
             contrast_limit = np.percentile(frame, (1, 99))
-            contrast_limit = [int(contrast_limit[0] * 0.5), int(contrast_limit[1] * 2), ]
+            contrast_limit = [
+                int(contrast_limit[0] * 0.5),
+                int(contrast_limit[1] * 2),
+            ]
 
             self.active_import_mode = "image"
 
             if len(image_list) > 1:
-                frame_name = file_name.replace(".", "_") + "_" + str(index) + ".tif"
+                frame_name = (
+                    file_name.replace(".", "_") + "_" + str(index) + ".tif"
+                )
             else:
                 frame_name = copy.deepcopy(file_name)
 
             frame_meta = copy.deepcopy(meta)
 
             frame_meta["akseg_hash"] = akseg_hash
             frame_meta["image_name"] = frame_name
@@ -1255,15 +1460,21 @@
             frame_meta["dims"] = [frame.shape[-1], frame.shape[-2]]
             frame_meta["crop"] = [0, frame.shape[-2], 0, frame.shape[-1]]
 
             images.append(frame)
             metadata[i] = frame_meta
 
             if imported_images == {}:
-                imported_images["Image"] = dict(images=[frame], masks=[], nmasks=[], classes=[], metadata={img_index: frame_meta}, )
+                imported_images["Image"] = dict(
+                    images=[frame],
+                    masks=[],
+                    nmasks=[],
+                    classes=[],
+                    metadata={img_index: frame_meta},
+                )
             else:
                 imported_images["Image"]["images"].append(frame)
                 imported_images["Image"]["metadata"][img_index] = frame_meta
 
             img_index += 1
 
     imported_data = dict(imported_images=imported_images)
@@ -1273,29 +1484,33 @@
 
 def import_cellpose(self, progress_callback, file_paths):
     if os.path.isdir(file_paths[0]):
         file_paths = glob(file_paths[0] + r"**\*", recursive=True)
 
     image_formats = ["npy"]
 
-    file_paths = [path for path in file_paths if path.split(".")[-1] in image_formats]
+    file_paths = [
+        path for path in file_paths if path.split(".")[-1] in image_formats
+    ]
 
     import_limit = self.import_limit.currentText()
 
     if import_limit != "None" and len(file_paths) > int(import_limit):
         file_paths = file_paths[: int(import_limit)]
 
     imported_images = {}
 
     for i in range(len(file_paths)):
         progress = int(((i + 1) / len(file_paths)) * 100)
         progress_callback.emit(progress)
 
         if self.widget_notifications:
-            show_info("loading image " + str(i + 1) + " of " + str(len(file_paths)))
+            show_info(
+                "loading image " + str(i + 1) + " of " + str(len(file_paths))
+            )
 
         file_path = os.path.abspath(file_paths[i])
         file_name = file_path.split("\\")[-1]
 
         dat = np.load(file_path, allow_pickle=True).item()
 
         mask = dat["masks"]
@@ -1304,15 +1519,17 @@
         image_path = file_path.replace("_seg.npy", ".tif")
 
         if os.path.exists(image_path):
             image_name = image_path.split("\\")[-1]
 
             import_precision = self.import_precision.currentText()
             multiframe_mode = self.import_multiframe_mode.currentIndex()
-            img, meta = read_image_file(image_path, import_precision, multiframe_mode)
+            img, meta = read_image_file(
+                image_path, import_precision, multiframe_mode
+            )
 
             crop_mode = self.import_crop_mode.currentIndex()
             img = crop_image(img, crop_mode)
             mask = crop_image(mask, crop_mode)
 
             contrast_limit, alpha, beta, gamma = autocontrast_values(img)
 
@@ -1339,19 +1556,41 @@
             contrast_limit, alpha, beta, gamma = autocontrast_values(image)
 
             self.active_import_mode = "cellpose"
 
             folder = os.path.abspath(file_path).split("\\")[-2]
             parent_folder = os.path.abspath(file_path).split("\\")[-3]
 
-            meta = dict(image_name=file_name, image_path=file_path, mask_name=file_name, mask_path=file_path, label_name=None, label_path=None, folder=folder, parent_folder=parent_folder, contrast_limit=contrast_limit, contrast_alpha=alpha, contrast_beta=beta, contrast_gamma=gamma, akseg_hash=get_hash(img_path=file_path), import_mode="cellpose", dims=[
-                image.shape[0], image.shape[1]], crop=[0, image.shape[1], 0, image.shape[0]], )
+            meta = dict(
+                image_name=file_name,
+                image_path=file_path,
+                mask_name=file_name,
+                mask_path=file_path,
+                label_name=None,
+                label_path=None,
+                folder=folder,
+                parent_folder=parent_folder,
+                contrast_limit=contrast_limit,
+                contrast_alpha=alpha,
+                contrast_beta=beta,
+                contrast_gamma=gamma,
+                akseg_hash=get_hash(img_path=file_path),
+                import_mode="cellpose",
+                dims=[image.shape[0], image.shape[1]],
+                crop=[0, image.shape[1], 0, image.shape[0]],
+            )
 
         if imported_images == {}:
-            imported_images["Image"] = dict(images=[img], masks=[mask], nmasks=[], classes=[], metadata={i: meta}, )
+            imported_images["Image"] = dict(
+                images=[img],
+                masks=[mask],
+                nmasks=[],
+                classes=[],
+                metadata={i: meta},
+            )
         else:
             imported_images["Image"]["images"].append(img)
             imported_images["Image"]["masks"].append(mask)
             imported_images["Image"]["metadata"][i] = meta
 
     imported_data = dict(imported_images=imported_images)
 
@@ -1360,24 +1599,28 @@
 
 def import_oufti(self, progress_callback, file_paths):
     if os.path.isdir(file_paths[0]):
         file_paths = glob(file_paths[0] + r"**\*", recursive=True)
 
     image_formats = ["mat"]
 
-    file_paths = [path for path in file_paths if path.split(".")[-1] in image_formats]
+    file_paths = [
+        path for path in file_paths if path.split(".")[-1] in image_formats
+    ]
 
     file_path = os.path.abspath(file_paths[0])
     parent_dir = file_path.replace(file_path.split("\\")[-1], "")
 
     mat_paths = file_paths
     image_paths = glob(parent_dir + r"**\*", recursive=True)
 
     image_formats = ["tif"]
-    image_paths = [path for path in image_paths if path.split(".")[-1] in image_formats]
+    image_paths = [
+        path for path in image_paths if path.split(".")[-1] in image_formats
+    ]
 
     mat_files = [path.split("\\")[-1] for path in mat_paths]
     image_files = [path.split("\\")[-1] for path in image_paths]
 
     matching_image_paths = []
     matching_mat_paths = []
 
@@ -1404,15 +1647,17 @@
             image_files = [matching_image_paths[index]]
             mat_files = [matching_mat_paths[index]]
 
         else:
             if self.widget_notifications:
                 show_info("Matching image/mesh files could not be found")
             self.viewer.text_overlay.visible = True
-            self.viewer.text_overlay.text = ("Matching image/mesh files could not be found")
+            self.viewer.text_overlay.text = (
+                "Matching image/mesh files could not be found"
+            )
 
     else:
         image_files = matching_image_paths
         mat_files = matching_mat_paths
 
     import_limit = self.import_limit.currentText()
 
@@ -1423,15 +1668,20 @@
 
     for i in range(len(mat_files)):
         try:
             progress = int(((i + 1) / len(mat_files)) * 100)
             progress_callback.emit(progress)
 
             if self.widget_notifications:
-                show_info("loading image " + str(i + 1) + " of " + str(len(mat_files)))
+                show_info(
+                    "loading image "
+                    + str(i + 1)
+                    + " of "
+                    + str(len(mat_files))
+                )
 
             mat_path = mat_files[i]
             image_path = image_files[i]
 
             image_name = image_path.split("\\")[-1]
             mat_name = mat_path.split("\\")[-1]
 
@@ -1457,15 +1707,21 @@
             meta["contrast_alpha"] = alpha
             meta["contrast_beta"] = beta
             meta["contrast_gamma"] = gamma
             meta["dims"] = [image.shape[-1], image.shape[-2]]
             meta["crop"] = [0, image.shape[-2], 0, image.shape[-1]]
 
             if imported_images == {}:
-                imported_images["Image"] = dict(images=[image], masks=[mask], nmasks=[], classes=[], metadata={i: meta}, )
+                imported_images["Image"] = dict(
+                    images=[image],
+                    masks=[mask],
+                    nmasks=[],
+                    classes=[],
+                    metadata={i: meta},
+                )
             else:
                 imported_images["Image"]["images"].append(image)
                 imported_images["Image"]["masks"].append(mask)
                 imported_images["Image"]["metadata"][i] = meta
 
         except:
             pass
@@ -1475,15 +1731,17 @@
     return imported_data
 
 
 def import_mat_data(self, image_path, mat_path):
     import_precision = self.import_precision.currentText()
     multiframe_mode = self.import_multiframe_mode.currentIndex()
     crop_mode = self.import_crop_mode.currentIndex()
-    image, meta = read_image_file(image_path, import_precision, multiframe_mode)
+    image, meta = read_image_file(
+        image_path, import_precision, multiframe_mode
+    )
 
     mat_data = mat4py.loadmat(mat_path)
 
     mat_data = mat_data["cellList"]
 
     contours = []
 
@@ -1500,34 +1758,41 @@
 
         cv2.drawContours(mask, [cnt], -1, i + 1, -1)
 
     return image, mask, meta
 
 
 def unstack_images(stack, axis=0):
-    images = [np.squeeze(e, axis) for e in np.split(stack, stack.shape[axis], axis=axis)]
+    images = [
+        np.squeeze(e, axis)
+        for e in np.split(stack, stack.shape[axis], axis=axis)
+    ]
 
     return images
 
 
-def append_image_stacks(current_metadata, new_metadata, current_image_stack, new_image_stack):
+def append_image_stacks(
+    current_metadata, new_metadata, current_image_stack, new_image_stack
+):
     current_image_stack = unstack_images(current_image_stack)
 
     new_image_stack = unstack_images(new_image_stack)
 
     appended_image_stack = current_image_stack + new_image_stack
 
     appended_metadata = current_metadata
 
     for key, value in new_metadata.items():
         new_key = max(appended_metadata.keys()) + 1
 
         appended_metadata[new_key] = value
 
-    appended_image_stack, appended_metadata = stack_images(appended_image_stack, appended_metadata)
+    appended_image_stack, appended_metadata = stack_images(
+        appended_image_stack, appended_metadata
+    )
 
     return appended_image_stack, appended_metadata
 
 
 def append_metadata(current_metadata, new_metadata):
     appended_metadata = current_metadata
 
@@ -1536,23 +1801,27 @@
 
         appended_metadata[new_key] = value
 
         return appended_metadata
 
 
 def read_ak_metadata(self):
-    meta_path = os.path.join(self.database_path, "Metadata", "AKSEG Metadata.xlsx")
+    meta_path = os.path.join(
+        self.database_path, "Metadata", "AKSEG Metadata.xlsx"
+    )
 
     ak_meta = pd.read_excel(meta_path)
 
     user_initials = list(ak_meta["User Initials"].dropna())
     microscope = list(ak_meta["Microscope"].dropna())
     modality = list(ak_meta["Image Modality"].dropna())
 
-    ak_meta = dict(user_initials=user_initials, microscope=microscope, modality=modality)
+    ak_meta = dict(
+        user_initials=user_initials, microscope=microscope, modality=modality
+    )
 
     return ak_meta
 
 
 def get_hash(img_path=None, img=None):
     if img is not None:
         img_path = tempfile.TemporaryFile(suffix=".tif").name
@@ -1563,15 +1832,20 @@
 
         hash_code = hashlib.sha256(bytes).hexdigest()
 
         return hash_code
 
 
 def align_image_channels(self):
-    layer_names = [layer.name for layer in self.viewer.layers if layer.name not in ["Segmentations", "Nucleoid", "Classes", "center_lines"]]
+    layer_names = [
+        layer.name
+        for layer in self.viewer.layers
+        if layer.name
+        not in ["Segmentations", "Nucleoid", "Classes", "center_lines"]
+    ]
 
     if self.import_align.isChecked() and len(layer_names) > 1:
         primary_image = layer_names[-1]
 
         layer_names.remove(primary_image)
 
         dim_range = int(self.viewer.dims.range[0][1])
@@ -1579,15 +1853,17 @@
         for i in range(dim_range):
             img = self.viewer.layers[primary_image].data[i, :, :]
 
             for layer in layer_names:
                 shifted_img = self.viewer.layers[layer].data[i, :, :]
 
                 try:
-                    shift, error, diffphase = phase_cross_correlation(img, shifted_img, upsample_factor=100)
+                    shift, error, diffphase = phase_cross_correlation(
+                        img, shifted_img, upsample_factor=100
+                    )
                     shifted_img = scipy.ndimage.shift(shifted_img, shift)
 
                 except:
                     pass
 
                 self.viewer.layers[layer].data[i, :, :] = shifted_img
 
@@ -1633,15 +1909,19 @@
                 label_id = np.unique(label[cnt_mask == 255])[0]
 
                 if label_id in export_labels:
                     new_mask_id = np.max(np.unique(export_mask)) + 1
                     export_mask[cnt_mask == 255] = new_mask_id
                     export_label[cnt_mask == 255] = label_id
 
-                    cnt, _ = cv2.findContours(cnt_mask.astype(np.uint8), cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_NONE, )
+                    cnt, _ = cv2.findContours(
+                        cnt_mask.astype(np.uint8),
+                        cv2.RETR_EXTERNAL,
+                        cv2.CHAIN_APPROX_NONE,
+                    )
 
                     contours.append(cnt[0])
 
         export_mask_stack[i, :, :][y1:y2, x1:x2] = export_mask
         export_label_stack[i, :, :][y1:y2, x1:x2] = export_label
         export_contours[i] = contours
 
@@ -1650,15 +1930,17 @@
 
 def import_JSON(self, progress_callback, file_paths):
     if os.path.isdir(file_paths[0]):
         file_paths = glob(file_paths[0] + r"**\*", recursive=True)
 
     image_formats = ["txt"]
 
-    json_paths = [path for path in file_paths if path.split(".")[-1] in image_formats]
+    json_paths = [
+        path for path in file_paths if path.split(".")[-1] in image_formats
+    ]
 
     file_path = os.path.abspath(file_paths[0])
     parent_dir = file_path.replace(file_path.split("\\")[-1], "")
 
     image_paths = glob(parent_dir + "*.tif", recursive=True)
 
     json_files = [path.split("\\")[-1] for path in json_paths]
@@ -1697,15 +1979,17 @@
             json_files = [matching_json_paths[index]]
 
         else:
             if self.widget_notifications:
                 show_info("Matching image/mesh files could not be found")
 
             self.viewer.text_overlay.visible = True
-            self.viewer.text_overlay.text = ("Matching image/mesh files could not be found")
+            self.viewer.text_overlay.text = (
+                "Matching image/mesh files could not be found"
+            )
 
     else:
         image_files = matching_image_paths
         json_files = matching_json_paths
 
     imported_images = {}
 
@@ -1714,26 +1998,33 @@
 
     for i in range(len(json_files)):
         try:
             progress = int(((i + 1) / len(json_files)) * 100)
             progress_callback.emit(progress)
 
             if self.widget_notifications:
-                show_info("loading image " + str(i + 1) + " of " + str(len(json_files)))
+                show_info(
+                    "loading image "
+                    + str(i + 1)
+                    + " of "
+                    + str(len(json_files))
+                )
 
             json_path = json_files[i]
             image_path = image_files[i]
 
             image_name = image_path.split("\\")[-1]
             json_name = json_path.split("\\")[-1]
 
             import_precision = self.import_precision.currentText()
             multiframe_mode = self.import_multiframe_mode.currentIndex()
             crop_mode = self.import_crop_mode.currentIndex()
-            image, meta = read_image_file(image_path, import_precision, multiframe_mode)
+            image, meta = read_image_file(
+                image_path, import_precision, multiframe_mode
+            )
 
             from napari_bacseg._utils_json import import_coco_json
 
             mask, nmask, labels = import_coco_json(json_path)
 
             crop_mode = self.import_crop_mode.currentIndex()
             image = crop_image(image, crop_mode)
@@ -1757,15 +2048,21 @@
             meta["contrast_alpha"] = alpha
             meta["contrast_beta"] = beta
             meta["contrast_gamma"] = gamma
             meta["dims"] = [image.shape[-1], image.shape[-2]]
             meta["crop"] = [0, image.shape[-2], 0, image.shape[-1]]
 
             if imported_images == {}:
-                imported_images["Image"] = dict(images=[image], masks=[mask], nmasks=[nmask], classes=[labels], metadata={i: meta}, )
+                imported_images["Image"] = dict(
+                    images=[image],
+                    masks=[mask],
+                    nmasks=[nmask],
+                    classes=[labels],
+                    metadata={i: meta},
+                )
             else:
                 imported_images["Image"]["images"].append(image)
                 imported_images["Image"]["masks"].append(mask)
                 imported_images["Image"]["nmasks"].append(nmask)
                 imported_images["Image"]["classes"].append(labels)
                 imported_images["Image"]["metadata"][i] = meta
 
@@ -1802,15 +2099,15 @@
     for i in a:
         b.append(b[-1] + i)
     return np.array(b)
 
 
 def autocontrast_values(image, clip_hist_percent=0.001):
     # calculate histogram
-    hist, bin_edges = np.histogram(image, bins=(2 ** 16) - 1)
+    hist, bin_edges = np.histogram(image, bins=(2**16) - 1)
     hist_size = len(hist)
 
     # calculate cumulative distribution from the histogram
     accumulator = cumsum(hist)
 
     # Locate points to clip
     maximum = accumulator[-1]
@@ -1866,20 +2163,29 @@
         import_folder = file_paths
 
     if os.path.isfile(file_paths[0]):
         file_paths = os.path.abspath(file_paths[0])
         import_folder = file_paths.replace(file_paths.split("\\")[-1], "")
 
     import_folder = os.path.abspath(import_folder)
-    mask_paths = glob(import_folder + r"**\**\*" + file_extension, recursive=True)
+    mask_paths = glob(
+        import_folder + r"**\**\*" + file_extension, recursive=True
+    )
 
     mask_files = [path.split("\\")[-1] for path in mask_paths]
-    mask_search = [file.split(file.split(".")[-1])[0][:-1] for file in mask_files]
-
-    layer_names = [layer.name for layer in self.viewer.layers if layer.name not in ["Segmentations", "Nucleoid", "Classes", "center_lines"]]
+    mask_search = [
+        file.split(file.split(".")[-1])[0][:-1] for file in mask_files
+    ]
+
+    layer_names = [
+        layer.name
+        for layer in self.viewer.layers
+        if layer.name
+        not in ["Segmentations", "Nucleoid", "Classes", "center_lines"]
+    ]
 
     matching_masks = []
 
     for layer in layer_names:
         image_stack = self.viewer.layers[layer].data
         meta_stack = self.viewer.layers[layer].metadata
 
@@ -1972,28 +2278,32 @@
                 label_id = np.unique(label[cnt_mask == 255])[0]
 
                 if label_id in export_labels:
                     new_mask_id = np.max(np.unique(export_mask)) + 1
                     export_mask[cnt_mask == 255] = new_mask_id
                     export_label[cnt_mask == 255] = label_id
 
-                    cnt, _ = cv2.findContours(cnt_mask.astype(np.uint8), cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_NONE, )
+                    cnt, _ = cv2.findContours(
+                        cnt_mask.astype(np.uint8),
+                        cv2.RETR_EXTERNAL,
+                        cv2.CHAIN_APPROX_NONE,
+                    )
 
                     contours.append(cnt[0])
 
         except:
             pass
 
     return contours
 
 
 def automatic_brightness_and_contrast(image, clip_hist_percent=0.1):
     if np.max(image) > 0:
         # Calculate grayscale histogram
-        hist = cv2.calcHist([image], [0], None, [2 ** 16], [0, 2 ** 16])
+        hist = cv2.calcHist([image], [0], None, [2**16], [0, 2**16])
         hist_size = len(hist)
 
         # Calculate cumulative distribution from the histogram
         accumulator = []
         accumulator.append(float(hist[0]))
         for index in range(1, hist_size):
             accumulator.append(accumulator[index - 1] + float(hist[index]))
@@ -2018,15 +2328,24 @@
         beta = -minimum_gray * alpha
 
         image = cv2.convertScaleAbs(image, alpha=alpha, beta=beta)
 
     return image
 
 
-def add_scale_bar(image, pixel_resolution=100, pixel_resolution_units="nm", scalebar_size=20, scalebar_size_units="um", scalebar_colour="white", scalebar_thickness=10, scalebar_margin=10, ):
+def add_scale_bar(
+    image,
+    pixel_resolution=100,
+    pixel_resolution_units="nm",
+    scalebar_size=20,
+    scalebar_size_units="um",
+    scalebar_colour="white",
+    scalebar_thickness=10,
+    scalebar_margin=10,
+):
     try:
         if float(pixel_resolution) > 0 and float(scalebar_size) > 0:
             h, w = image.shape
 
             pixel_resolution = float(pixel_resolution)
             scalebar_size = float(scalebar_size)
 
@@ -2038,39 +2357,70 @@
                 rescaled_pixel_resolution = pixel_resolution
 
             if scalebar_size_units != "nm":
                 rescaled_scalebar_size = scalebar_size * 1000
             else:
                 rescaled_scalebar_size = scalebar_size
 
-            scalebar_len = int(rescaled_scalebar_size / rescaled_pixel_resolution)
+            scalebar_len = int(
+                rescaled_scalebar_size / rescaled_pixel_resolution
+            )
 
             if scalebar_len > 0 and scalebar_len < w:
                 if scalebar_colour == "White":
                     bit_depth = str(image.dtype)
                     bit_depth = int(bit_depth.replace("uint", ""))
-                    colour = (2 ** bit_depth) - 1
+                    colour = (2**bit_depth) - 1
                 else:
                     colour = 0
 
-                scalebar_pos = (w - scalebar_margin - scalebar_len, h - scalebar_margin - int(scalebar_thickness),)  # Position of the scale bar in the image (in pixels)
-
-                image = cv2.rectangle(image, scalebar_pos, (scalebar_pos[0] + scalebar_len, scalebar_pos[1] + int(scalebar_thickness),), colour, -1, )
+                scalebar_pos = (
+                    w - scalebar_margin - scalebar_len,
+                    h - scalebar_margin - int(scalebar_thickness),
+                )  # Position of the scale bar in the image (in pixels)
+
+                image = cv2.rectangle(
+                    image,
+                    scalebar_pos,
+                    (
+                        scalebar_pos[0] + scalebar_len,
+                        scalebar_pos[1] + int(scalebar_thickness),
+                    ),
+                    colour,
+                    -1,
+                )
 
             else:
-                show_info(f"{int(scalebar_size)} ({scalebar_size_units}) Scale bar is too large for the {(rescaled_pixel_resolution / 1000) * w}x{(rescaled_pixel_resolution / 1000) * h} (um) image")
+                show_info(
+                    f"{int(scalebar_size)} ({scalebar_size_units}) Scale bar is too large for the {(rescaled_pixel_resolution / 1000) * w}x{(rescaled_pixel_resolution / 1000) * h} (um) image"
+                )
 
     except:
         print(traceback.format_exc())
 
     return image
 
 
-def generate_export_image(self, export_channel, dim, normalize=False, invert=False, autocontrast=False, scalebar=False, cropzoom=False, mask_background=False, ):
-    layer_names = [layer.name for layer in self.viewer.layers if layer.name not in ["Segmentations", "Nucleoid", "Classes", "center_lines"]]
+def generate_export_image(
+    self,
+    export_channel,
+    dim,
+    normalize=False,
+    invert=False,
+    autocontrast=False,
+    scalebar=False,
+    cropzoom=False,
+    mask_background=False,
+):
+    layer_names = [
+        layer.name
+        for layer in self.viewer.layers
+        if layer.name
+        not in ["Segmentations", "Nucleoid", "Classes", "center_lines"]
+    ]
 
     layer_names.reverse()
 
     if export_channel == "All Channels (Stack)":
         mode = "stack"
     elif export_channel == "First Three Channels (RGB)":
         mode = "rgb"
@@ -2092,27 +2442,27 @@
     metadata = metadata[dim[0]]
 
     if cropzoom:
         layer = self.viewer.layers[layer_names[0]]
         crop = layer.corner_pixels.T
         y_range = crop[-2]
         x_range = crop[-1]
-        mask = mask[y_range[0]: y_range[1], x_range[0]: x_range[1]]
-        nmask = nmask[y_range[0]: y_range[1], x_range[0]: x_range[1]]
-        label = label[y_range[0]: y_range[1], x_range[0]: x_range[1]]
+        mask = mask[y_range[0] : y_range[1], x_range[0] : x_range[1]]
+        nmask = nmask[y_range[0] : y_range[1], x_range[0] : x_range[1]]
+        label = label[y_range[0] : y_range[1], x_range[0] : x_range[1]]
 
     image = []
 
     for layer in layer_names:
         img = self.viewer.layers[layer].data.copy()
 
         img = img[dim]
 
         if cropzoom:
-            img = img[y_range[0]: y_range[1], x_range[0]: x_range[1]]
+            img = img[y_range[0] : y_range[1], x_range[0] : x_range[1]]
 
         if mask_background:
             img[mask == 0] = 0
 
         if invert:
             img = cv2.bitwise_not(img)
 
@@ -2120,89 +2470,118 @@
             img = normalize99(img)
 
         if autocontrast:
             img = automatic_brightness_and_contrast(img)
 
         if scalebar:
             pixel_resolution = self.export_scalebar_resolution.text()
-            pixel_resolution_units = (self.export_scalebar_resolution_units.currentText())
+            pixel_resolution_units = (
+                self.export_scalebar_resolution_units.currentText()
+            )
             scalebar_size = self.export_scalebar_size.text()
             scalebar_size_units = self.export_scalebar_size_units.currentText()
             scalebar_colour = self.export_scalebar_colour.currentText()
             scalebar_thickness = self.export_scalebar_thickness.currentText()
 
-            img = add_scale_bar(img, pixel_resolution=pixel_resolution, pixel_resolution_units=pixel_resolution_units, scalebar_size=scalebar_size, scalebar_size_units=scalebar_size_units, scalebar_colour=scalebar_colour, scalebar_thickness=scalebar_thickness, )
+            img = add_scale_bar(
+                img,
+                pixel_resolution=pixel_resolution,
+                pixel_resolution_units=pixel_resolution_units,
+                scalebar_size=scalebar_size,
+                scalebar_size_units=scalebar_size_units,
+                scalebar_colour=scalebar_colour,
+                scalebar_thickness=scalebar_thickness,
+            )
 
         image.append(img)
 
     if mode == "rgb":
         while len(image) < 3:
             blank = np.zeros(img.shape, dtype=img.dtype)
 
             if scalebar:
-                blank = add_scale_bar(blank, pixel_resolution=pixel_resolution, pixel_resolution_units=pixel_resolution_units, scalebar_size=scalebar_size, scalebar_size_units=scalebar_size_units, scalebar_colour=scalebar_colour, scalebar_thickness=scalebar_thickness, )
+                blank = add_scale_bar(
+                    blank,
+                    pixel_resolution=pixel_resolution,
+                    pixel_resolution_units=pixel_resolution_units,
+                    scalebar_size=scalebar_size,
+                    scalebar_size_units=scalebar_size_units,
+                    scalebar_colour=scalebar_colour,
+                    scalebar_thickness=scalebar_thickness,
+                )
 
             image.append(blank)
 
     if mode == "rgb":
         image = np.stack(image, axis=-1)
 
         image = rescale01(image)
-        image = image * (2 ** 16 - 1)
+        image = image * (2**16 - 1)
         image = image.astype(np.uint16)
 
     elif mode == "stack":
         image = np.stack(image, axis=0)
     else:
         image = image[0]
 
     return image, mask, nmask, label, metadata, mode
 
 
 def export_stacks(self, progress_callback, mode):
-
     try:
-
-        layer_names = [layer.name for layer in self.viewer.layers if layer.name not in ["Segmentations", "Nucleoid", "Classes", "center_lines"]]
+        layer_names = [
+            layer.name
+            for layer in self.viewer.layers
+            if layer.name
+            not in ["Segmentations", "Nucleoid", "Classes", "center_lines"]
+        ]
 
         export_stack_channel = self.export_stack_channel.currentText()
         export_stack_mode = self.export_stack_mode.currentText()
         export_stack_modifier = self.export_stack_modifier.text()
 
         if mode == "active":
             export_channels = [self.export_stack_channel.currentText()]
         else:
-            export_channels = [layer.name for layer in self.viewer.layers if layer.name not in ["Segmentations", "Nucleoid", "Classes", "center_lines"]]
+            export_channels = [
+                layer.name
+                for layer in self.viewer.layers
+                if layer.name
+                not in ["Segmentations", "Nucleoid", "Classes", "center_lines"]
+            ]
 
         overwrite = self.export_stack_overwrite_setting.isChecked()
         export_images = self.export_stack_image_setting.isChecked()
 
         normalise = self.export_normalise.isChecked()
         invert = self.export_invert.isChecked()
         autocontrast = self.export_autocontrast.isChecked()
         scalebar = self.export_scalebar.isChecked()
         cropzoom = self.export_cropzoom.isChecked()
         mask_background = self.export_mask_background.isChecked()
 
         for channel in export_channels:
-
             image_stack = []
             mask_stack = []
 
             dims = self.viewer.layers[channel].data.shape[0]
 
             for dim in range(dims):
-
-                progress_callback.emit(int((dim / (dims-1)) * 100))
+                progress_callback.emit(int((dim / (dims - 1)) * 100))
 
                 image, mask, nmask, label, meta, mode = generate_export_image(
-                    self, channel, (dim,),
-                    normalise, invert, autocontrast,
+                    self,
+                    channel,
+                    (dim,),
+                    normalise,
+                    invert,
+                    autocontrast,
                     scalebar,
-                    cropzoom, mask_background,
+                    cropzoom,
+                    mask_background,
                 )
 
                 if len(image.shape) > 2:
                     image = image[0]
                     mask = mask[0]
 
                 image_stack.append(image)
@@ -2217,28 +2596,40 @@
                 image_path = meta["image_path"]
             if "path" in meta.keys():
                 image_path = meta["path"]
 
             file_name, file_extension = os.path.splitext(file_name)
 
             file_name = file_name + export_stack_modifier + ".tif"
-            image_path = image_path.replace(image_path.split("\\")[-1], file_name)
-
-            if (self.export_stack_location.currentText() == "Import Directory" and file_name != None and image_path != None):
-                export_path = os.path.abspath(image_path.replace(file_name, ""))
+            image_path = image_path.replace(
+                image_path.split("\\")[-1], file_name
+            )
+
+            if (
+                self.export_stack_location.currentText() == "Import Directory"
+                and file_name != None
+                and image_path != None
+            ):
+                export_path = os.path.abspath(
+                    image_path.replace(file_name, "")
+                )
 
-            elif self.export_stack_location.currentText() == "Select Directory":
+            elif (
+                self.export_stack_location.currentText() == "Select Directory"
+            ):
                 export_path = os.path.abspath(self.export_directory)
 
             else:
                 export_path = None
 
             if os.path.isdir(export_path) != True:
                 if self.widget_notifications:
-                    show_info("Directory does not exist, try selecting a directory instead!")
+                    show_info(
+                        "Directory does not exist, try selecting a directory instead!"
+                    )
 
             else:
                 y1, y2, x1, x2 = meta["crop"]
 
                 if len(image.shape) > 2:
                     image = image[:, y1:y2, x1:x2]
                     mask = mask[:, y1:y2, x1:x2]
@@ -2249,28 +2640,28 @@
                 if os.path.isdir(export_path) == False:
                     os.makedirs(file_path)
 
                 file_path = export_path + "\\" + file_name
 
                 if os.path.isfile(file_path) == True and overwrite == False:
                     if self.widget_notifications:
-                        show_info(file_name + " already exists, BacSeg will not overwrite files!")
+                        show_info(
+                            file_name
+                            + " already exists, BacSeg will not overwrite files!"
+                        )
 
                 else:
-
                     if export_stack_mode == "Export .tif Images":
                         tifffile.imwrite(file_path, image_stack, metadata=meta)
 
                     if export_stack_mode == "Export .tif Masks":
                         tifffile.imwrite(file_path, mask_stack, metadata=meta)
 
     except:
         print(traceback.format_exc())
-        pass
-
 
 
 def export_files(self, progress_callback, mode):
     desktop = os.path.expanduser("~/Desktop")
 
     overwrite = self.export_overwrite_setting.isChecked()
     export_images = self.export_image_setting.isChecked()
@@ -2303,15 +2694,25 @@
             if len(viewer_dims) == 2:
                 for tile_index in range(*viewer_dims[1]):
                     dim_list.append((image_index, tile_index))
             else:
                 dim_list.append((image_index,))
 
     for i, dim in enumerate(dim_list):
-        image, mask, nmask, label, meta, mode = generate_export_image(self, export_channel, dim, normalise, invert, autocontrast, scalebar, cropzoom, mask_background, )
+        image, mask, nmask, label, meta, mode = generate_export_image(
+            self,
+            export_channel,
+            dim,
+            normalise,
+            invert,
+            autocontrast,
+            scalebar,
+            cropzoom,
+            mask_background,
+        )
         contours = get_contours_from_mask(mask, label, export_labels)
 
         if "midlines" in meta.keys():
             midlines = meta["midlines"].copy()
         else:
             midlines = None
 
@@ -2329,26 +2730,32 @@
 
         if len(dim) == 2:
             file_name = file_name + f"_{dim}"
 
         file_name = file_name + export_modifier + ".tif"
         image_path = image_path.replace(image_path.split("\\")[-1], file_name)
 
-        if (self.export_location.currentText() == "Import Directory" and file_name != None and image_path != None):
+        if (
+            self.export_location.currentText() == "Import Directory"
+            and file_name != None
+            and image_path != None
+        ):
             export_path = os.path.abspath(image_path.replace(file_name, ""))
 
         elif self.export_location.currentText() == "Select Directory":
             export_path = os.path.abspath(self.export_directory)
 
         else:
             export_path = None
 
         if os.path.isdir(export_path) != True:
             if self.widget_notifications:
-                show_info("Directory does not exist, try selecting a directory instead!")
+                show_info(
+                    "Directory does not exist, try selecting a directory instead!"
+                )
 
         else:
             y1, y2, x1, x2 = meta["crop"]
 
             if len(image.shape) > 2:
                 image = image[:, y1:y2, x1:x2]
             else:
@@ -2360,24 +2767,30 @@
             if os.path.isdir(export_path) == False:
                 os.makedirs(file_path)
 
             file_path = export_path + "\\" + file_name
 
             if os.path.isfile(file_path) == True and overwrite == False:
                 if self.widget_notifications:
-                    show_info(file_name + " already exists, BacSeg will not overwrite files!")
+                    show_info(
+                        file_name
+                        + " already exists, BacSeg will not overwrite files!"
+                    )
 
             else:
                 if self.export_mode.currentText() == "Export .tif Images":
                     tifffile.imwrite(file_path, image, metadata=meta)
 
                 if self.export_mode.currentText() == "Export .tif Masks":
                     tifffile.imwrite(file_path, mask, metadata=meta)
 
-                if (self.export_mode.currentText() == "Export .tif Images and Masks"):
+                if (
+                    self.export_mode.currentText()
+                    == "Export .tif Images and Masks"
+                ):
                     image_path = os.path.abspath(export_path + "\\images")
                     mask_path = os.path.abspath(export_path + "\\masks")
 
                     if not os.path.exists(image_path):
                         os.makedirs(image_path)
 
                     if not os.path.exists(mask_path):
@@ -2398,42 +2811,55 @@
                         tifffile.imwrite(file_path, image, metadata=meta)
 
                 if self.export_mode.currentText() == "Export Oufti":
                     try:
                         with warnings.catch_warnings():
                             warnings.filterwarnings("ignore")
 
-                            from napari_bacseg._utils_oufti import (export_oufti, get_oufti_data, )
-
-                            oufti_data = get_oufti_data(self, image, mask, midlines)
+                            from napari_bacseg._utils_oufti import (
+                                export_oufti,
+                                get_oufti_data,
+                            )
+
+                            oufti_data = get_oufti_data(
+                                self, image, mask, midlines
+                            )
 
                             if "midlines" in meta.keys():
                                 meta.pop("midlines")
 
                             export_oufti(image, oufti_data, file_path)
 
                             if export_images:
-                                tifffile.imwrite(file_path, image, metadata=meta)
+                                tifffile.imwrite(
+                                    file_path, image, metadata=meta
+                                )
 
                     except:
-                        raise Exception("BacSeg can't load Cellpose and OUFTI dependencies simultaneously. Restart BacSeg, reload images/masks, then export Oufti")
+                        raise Exception(
+                            "BacSeg can't load Cellpose and OUFTI dependencies simultaneously. Restart BacSeg, reload images/masks, then export Oufti"
+                        )
 
                 if self.export_mode.currentText() == "Export ImageJ":
                     from napari_bacseg._utils_imagej import export_imagej
 
                     if mode == "rgb":
                         if self.widget_notifications:
-                            show_info("ImageJ can't handle RGB images with annotations, export as image stack instead...")
+                            show_info(
+                                "ImageJ can't handle RGB images with annotations, export as image stack instead..."
+                            )
 
                     export_imagej(image, contours, meta, file_path)
 
                 if self.export_mode.currentText() == "Export JSON":
                     from napari_bacseg._utils_json import export_coco_json
 
-                    export_coco_json(file_name, image, mask, nmask, label, file_path)
+                    export_coco_json(
+                        file_name, image, mask, nmask, label, file_path
+                    )
 
                     if export_images:
                         tifffile.imwrite(file_path, image, metadata=meta)
 
                 if self.export_mode.currentText() == "Export CSV":
                     export_csv(image, contours, meta, file_path)
 
@@ -2462,63 +2888,102 @@
 
         for i in range(len(contours)):
             try:
                 cnt = contours[i]
                 cnt = np.vstack(cnt).squeeze().astype(str)
 
                 if len(cnt.shape) < max_length:
-                    cnt = np.pad(cnt, ((0, max_length - cnt.shape[0]), (0, 0)), "constant", constant_values="", )
+                    cnt = np.pad(
+                        cnt,
+                        ((0, max_length - cnt.shape[0]), (0, 0)),
+                        "constant",
+                        constant_values="",
+                    )
 
                 processed_contours.append(cnt)
 
             except:
                 pass
 
         try:
             file_extension = file_path.split(".")[-1]
             file_path = file_path.replace(file_extension, "csv")
 
             processed_contours = np.hstack(processed_contours)
-            headers = np.array([[f"x[{str(x)}]", f"y[{str((x))}]"] for x in range(processed_contours.shape[-1] // 2)]).flatten()
-
-            pd.DataFrame(processed_contours, columns=headers).to_csv(file_path, index=False, header=True)
+            headers = np.array(
+                [
+                    [f"x[{str(x)}]", f"y[{str((x))}]"]
+                    for x in range(processed_contours.shape[-1] // 2)
+                ]
+            ).flatten()
+
+            pd.DataFrame(processed_contours, columns=headers).to_csv(
+                file_path, index=False, header=True
+            )
 
         except:
             print(traceback.format_exc())
 
 
 def _manualImport(self):
     try:
-        if (self.viewer.layers.index("Segmentations") != len(self.viewer.layers) - 1):
+        if (
+            self.viewer.layers.index("Segmentations")
+            != len(self.viewer.layers) - 1
+        ):
             # reshapes masks to be same shape as active image
             self.active_layer = self.viewer.layers[-1]
 
             if self.active_layer.metadata == {}:
                 active_image = self.active_layer.data
 
                 if len(active_image.shape) < 3:
                     active_image = np.expand_dims(active_image, axis=0)
                     self.active_layer.data = active_image
 
                 if self.classLayer.data.shape != self.active_layer.data.shape:
-                    self.classLayer.data = np.zeros(active_image.shape, np.uint16)
+                    self.classLayer.data = np.zeros(
+                        active_image.shape, np.uint16
+                    )
 
                 if self.segLayer.data.shape != self.active_layer.data.shape:
-                    self.segLayer.data = np.zeros(active_image.shape, np.uint16)
+                    self.segLayer.data = np.zeros(
+                        active_image.shape, np.uint16
+                    )
 
                 image_name = str(self.viewer.layers[-1]) + ".tif"
 
                 meta = {}
                 for i in range(active_image.shape[0]):
                     img = active_image[i, :, :]
 
-                    contrast_limit, alpha, beta, gamma = autocontrast_values(img, clip_hist_percent=1)
-
-                    img_meta = dict(image_name=image_name, image_path="Unknown", mask_name=None, mask_path=None, label_name=None, label_path=None, folder=None, parent_folder=None, contrast_limit=contrast_limit, contrast_alpha=alpha, contrast_beta=beta, contrast_gamma=gamma, akseg_hash=None, import_mode="manual", dims=[
-                        img.shape[1], img.shape[0]], crop=[0, img.shape[0], 0, img.shape[1]], frame=i, frames=active_image.shape[0], )
+                    contrast_limit, alpha, beta, gamma = autocontrast_values(
+                        img, clip_hist_percent=1
+                    )
+
+                    img_meta = dict(
+                        image_name=image_name,
+                        image_path="Unknown",
+                        mask_name=None,
+                        mask_path=None,
+                        label_name=None,
+                        label_path=None,
+                        folder=None,
+                        parent_folder=None,
+                        contrast_limit=contrast_limit,
+                        contrast_alpha=alpha,
+                        contrast_beta=beta,
+                        contrast_gamma=gamma,
+                        akseg_hash=None,
+                        import_mode="manual",
+                        dims=[img.shape[1], img.shape[0]],
+                        crop=[0, img.shape[0], 0, img.shape[1]],
+                        frame=i,
+                        frames=active_image.shape[0],
+                    )
 
                     meta[i] = img_meta
 
                 self.active_layer.metadata = meta
                 self.segLayer.metadata = meta
                 self.classLayer.metadata = meta
```

### Comparing `napari-bacseg-1.0.8/src/napari_bacseg/_utils_cellpose.py` & `napari-bacseg-1.0.9/src/napari_bacseg/_utils_cellpose.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/napari_bacseg/_utils_colicoords.py` & `napari-bacseg-1.0.9/src/napari_bacseg/_utils_colicoords.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/napari_bacseg/_utils_database.py` & `napari-bacseg-1.0.9/src/napari_bacseg/_utils_database.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/napari_bacseg/_utils_database_IO.py` & `napari-bacseg-1.0.9/src/napari_bacseg/_utils_database_IO.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/napari_bacseg/_utils_imagej.py` & `napari-bacseg-1.0.9/src/napari_bacseg/_utils_imagej.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/napari_bacseg/_utils_interface_events.py` & `napari-bacseg-1.0.9/src/napari_bacseg/_utils_interface_events.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/napari_bacseg/_utils_json.py` & `napari-bacseg-1.0.9/src/napari_bacseg/_utils_json.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/napari_bacseg/_utils_oufti.py` & `napari-bacseg-1.0.9/src/napari_bacseg/_utils_oufti.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/napari_bacseg/_utils_refine.py` & `napari-bacseg-1.0.9/src/napari_bacseg/_utils_refine.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/napari_bacseg/_utils_statistics.py` & `napari-bacseg-1.0.9/src/napari_bacseg/_utils_statistics.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/napari_bacseg/_utils_tiler.py` & `napari-bacseg-1.0.9/src/napari_bacseg/_utils_tiler.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.8/src/napari_bacseg/_widget.py` & `napari-bacseg-1.0.9/src/napari_bacseg/_widget.py`

 * *Files 27% similar despite different names*

```diff
@@ -17,15 +17,30 @@
 
 import cv2
 import napari
 import numpy as np
 from napari.utils.notifications import show_info
 from PyQt5.QtCore import pyqtSignal, pyqtSlot
 from qtpy.QtCore import QObject, QRunnable, QThreadPool
-from qtpy.QtWidgets import (QCheckBox, QComboBox, QFileDialog, QFormLayout, QHBoxLayout, QLabel, QLineEdit, QProgressBar, QPushButton, QRadioButton, QSlider, QTabWidget, QVBoxLayout, QWidget, )
+from qtpy.QtWidgets import (
+    QCheckBox,
+    QComboBox,
+    QFileDialog,
+    QFormLayout,
+    QHBoxLayout,
+    QLabel,
+    QLineEdit,
+    QProgressBar,
+    QPushButton,
+    QRadioButton,
+    QSlider,
+    QTabWidget,
+    QVBoxLayout,
+    QWidget,
+)
 
 import napari_bacseg._utils
 from napari_bacseg._utils import align_image_channels, unstack_images
 
 os.environ["QT_AUTO_SCREEN_SCALE_FACTOR"] = "1"
 
 
@@ -91,15 +106,17 @@
         try:
             result = self.fn(*self.args, **self.kwargs)
         except:
             traceback.print_exc()
             exctype, value = sys.exc_info()[:2]
             self.signals.error.emit((exctype, value, traceback.format_exc()))
         else:
-            self.signals.result.emit(result)  # Return the result of the processing
+            self.signals.result.emit(
+                result
+            )  # Return the result of the processing
         finally:
             self.signals.finished.emit()  # Done
 
     def result(self):
         return self.fn(*self.args, **self.kwargs)
 
 
@@ -140,20 +157,53 @@
     def __init__(self, viewer: napari.Viewer):
         """Initialize widget with two layer combo boxes and a run button"""
 
         super().__init__()
 
         # import functions
         from napari_bacseg._utils import _manualImport, stack_images
-        from napari_bacseg._utils_cellpose import (_initialise_cellpose_model, _select_cellpose_save_directory, _select_cellpose_save_path, _select_custom_cellpose_model, train_cellpose_model, )
-        from napari_bacseg._utils_database import (_create_bacseg_database, _load_bacseg_database, _populateUSERMETA, _show_database_controls, populate_upload_combos, update_database_metadata, )
-        from napari_bacseg._utils_interface_events import (_copymasktoall, _delete_active_image, _deleteallmasks, _doubeClickEvents, _imageControls, _modify_channel_changed, _modifyMode, _segmentationEvents, _viewerControls, )
-        from napari_bacseg._utils_oufti import (_update_active_midlines, centre_oufti_midlines, generate_midlines, midline_edit_toggle, update_midlines, )
+        from napari_bacseg._utils_cellpose import (
+            _initialise_cellpose_model,
+            _select_cellpose_save_directory,
+            _select_cellpose_save_path,
+            _select_custom_cellpose_model,
+            train_cellpose_model,
+        )
+        from napari_bacseg._utils_database import (
+            _create_bacseg_database,
+            _load_bacseg_database,
+            _populateUSERMETA,
+            _show_database_controls,
+            populate_upload_combos,
+            update_database_metadata,
+        )
+        from napari_bacseg._utils_interface_events import (
+            _copymasktoall,
+            _delete_active_image,
+            _deleteallmasks,
+            _doubeClickEvents,
+            _imageControls,
+            _modify_channel_changed,
+            _modifyMode,
+            _segmentationEvents,
+            _viewerControls,
+        )
+        from napari_bacseg._utils_oufti import (
+            _update_active_midlines,
+            centre_oufti_midlines,
+            generate_midlines,
+            midline_edit_toggle,
+            update_midlines,
+        )
         from napari_bacseg._utils_statistics import _compute_simple_cell_stats
-        from napari_bacseg._utils_tiler import (fold_images, unfold_images, update_image_folds, )
+        from napari_bacseg._utils_tiler import (
+            fold_images,
+            unfold_images,
+            update_image_folds,
+        )
         from napari_bacseg.bacseg_ui import Ui_tab_widget
 
         self.populate_upload_combos = self.wrapper(populate_upload_combos)
         self.update_database_metadata = self.wrapper(update_database_metadata)
         self.stack_image = self.wrapper(stack_images)
         self._modifyMode = self.wrapper(_modifyMode)
         self._viewerControls = self.wrapper(_viewerControls)
@@ -162,31 +212,41 @@
         self._delete_active_image = self.wrapper(_delete_active_image)
         self._populateUSERMETA = self.wrapper(_populateUSERMETA)
         self._imageControls = self.wrapper(_imageControls)
         self._segmentationEvents = self.wrapper(_segmentationEvents)
         self._modify_channel_changed = self.wrapper(_modify_channel_changed)
         self._manualImport = self.wrapper(_manualImport)
         self.train_cellpose_model = self.wrapper(train_cellpose_model)
-        self._initialise_cellpose_model = self.wrapper(_initialise_cellpose_model)
-        self._select_custom_cellpose_model = self.wrapper(_select_custom_cellpose_model)
-        self._select_cellpose_save_directory = self.wrapper(_select_cellpose_save_directory)
-        self._select_cellpose_save_path = self.wrapper(_select_cellpose_save_path)
+        self._initialise_cellpose_model = self.wrapper(
+            _initialise_cellpose_model
+        )
+        self._select_custom_cellpose_model = self.wrapper(
+            _select_custom_cellpose_model
+        )
+        self._select_cellpose_save_directory = self.wrapper(
+            _select_cellpose_save_directory
+        )
+        self._select_cellpose_save_path = self.wrapper(
+            _select_cellpose_save_path
+        )
         self.unfold_images = self.wrapper(unfold_images)
         self.fold_images = self.wrapper(fold_images)
         self.update_image_folds = self.wrapper(update_image_folds)
         self.midline_edit_toggle = self.wrapper(midline_edit_toggle)
         self.centre_oufti_midlines = self.wrapper(centre_oufti_midlines)
         self.generate_midlines = self.wrapper(generate_midlines)
         self.update_midlines = self.wrapper(update_midlines)
         self._update_active_midlines = self.wrapper(_update_active_midlines)
         self._create_bacseg_database = self.wrapper(_create_bacseg_database)
         self._load_bacseg_database = self.wrapper(_load_bacseg_database)
         self._show_database_controls = self.wrapper(_show_database_controls)
         self._doubeClickEvents = self.wrapper(_doubeClickEvents)
-        self._compute_simple_cell_stats = self.wrapper(_compute_simple_cell_stats)
+        self._compute_simple_cell_stats = self.wrapper(
+            _compute_simple_cell_stats
+        )
 
         application_path = os.path.dirname(sys.executable)
         self.viewer = viewer
         self.setLayout(QVBoxLayout())
 
         # ui_path = os.path.abspath(r"C:\napari-bacseg\src\napari_bacseg\bacseg_ui.ui")
         # self.bacseg_ui = uic.loadUi(ui_path)
@@ -207,131 +267,217 @@
         self.active_import_mode = ""
         self.import_mode = self.findChild(QComboBox, "import_mode")
         self.import_filemode = self.findChild(QComboBox, "import_filemode")
         self.import_precision = self.findChild(QComboBox, "import_precision")
         self.import_import = self.findChild(QPushButton, "import_import")
         self.import_limit = self.findChild(QComboBox, "import_limit")
         self.import_limit_label = self.findChild(QLabel, "import_limit_label")
-        self.import_append_mode = self.findChild(QComboBox, "import_append_mode")
+        self.import_append_mode = self.findChild(
+            QComboBox, "import_append_mode"
+        )
 
         # self.clear_previous = self.findChild(QCheckBox, "import_clear_previous")
         self.autocontrast = self.findChild(QCheckBox, "import_auto_contrast")
-        self.import_multiframe_mode = self.findChild(QComboBox, "import_multiframe_mode")
+        self.import_multiframe_mode = self.findChild(
+            QComboBox, "import_multiframe_mode"
+        )
         self.import_crop_mode = self.findChild(QComboBox, "import_crop_mode")
         self.channel_mode = self.findChild(QComboBox, "nim_channel_mode")
-        self.import_progressbar = self.findChild(QProgressBar, "import_progressbar")
+        self.import_progressbar = self.findChild(
+            QProgressBar, "import_progressbar"
+        )
         self.import_align = self.findChild(QCheckBox, "import_align")
         self.label_modality = self.findChild(QComboBox, "label_modality")
         self.label_stain = self.findChild(QComboBox, "label_stain")
-        self.label_stain_target = self.findChild(QComboBox, "label_stain_target")
+        self.label_stain_target = self.findChild(
+            QComboBox, "label_stain_target"
+        )
         self.label_overwrite = self.findChild(QPushButton, "label_overwrite")
-        self.label_light_source = self.findChild(QComboBox, "label_light_source")
+        self.label_light_source = self.findChild(
+            QComboBox, "label_light_source"
+        )
 
         # view tab controls + variables from Qt Desinger References
         self.unfold_tile_size = self.findChild(QComboBox, "unfold_tile_size")
-        self.unfold_tile_overlap = self.findChild(QComboBox, "unfold_tile_overlap")
+        self.unfold_tile_overlap = self.findChild(
+            QComboBox, "unfold_tile_overlap"
+        )
         self.unfold_mode = self.findChild(QComboBox, "unfold_mode")
         self.fold = self.findChild(QPushButton, "fold")
         self.unfold = self.findChild(QPushButton, "unfold")
-        self.unfold_progressbar = self.findChild(QPushButton, "unfold_progressbar")
+        self.unfold_progressbar = self.findChild(
+            QPushButton, "unfold_progressbar"
+        )
         self.alignment_channel = self.findChild(QComboBox, "alignment_channel")
-        self.align_active_image = self.findChild(QPushButton, "align_active_image")
+        self.align_active_image = self.findChild(
+            QPushButton, "align_active_image"
+        )
         self.align_all_images = self.findChild(QPushButton, "align_all_images")
 
         self.overlay_filename = self.findChild(QCheckBox, "overlay_filename")
         self.overlay_folder = self.findChild(QCheckBox, "overlay_folder")
-        self.overlay_microscope = self.findChild(QCheckBox, "overlay_microscope")
-        self.overlay_datemodified = self.findChild(QCheckBox, "overlay_datemodified")
+        self.overlay_microscope = self.findChild(
+            QCheckBox, "overlay_microscope"
+        )
+        self.overlay_datemodified = self.findChild(
+            QCheckBox, "overlay_datemodified"
+        )
         self.overlay_content = self.findChild(QCheckBox, "overlay_content")
         self.overlay_phenotype = self.findChild(QCheckBox, "overlay_phenotype")
         self.overlay_strain = self.findChild(QCheckBox, "overlay_strain")
-        self.overlay_staintarget = self.findChild(QCheckBox, "overlay_staintarget")
-        self.overlay_antibiotic = self.findChild(QCheckBox, "overlay_antibiotic")
+        self.overlay_staintarget = self.findChild(
+            QCheckBox, "overlay_staintarget"
+        )
+        self.overlay_antibiotic = self.findChild(
+            QCheckBox, "overlay_antibiotic"
+        )
         self.overlay_stain = self.findChild(QCheckBox, "overlay_stain")
         self.overlay_modality = self.findChild(QCheckBox, "overlay_modality")
-        self.overlay_lightsource = self.findChild(QCheckBox, "overlay_lightsource")
+        self.overlay_lightsource = self.findChild(
+            QCheckBox, "overlay_lightsource"
+        )
         self.overlay_focus = self.findChild(QCheckBox, "overlay_focus")
         self.overlay_debris = self.findChild(QCheckBox, "overlay_debris")
         self.overlay_laplacian = self.findChild(QCheckBox, "overlay_laplacian")
         self.overlay_range = self.findChild(QCheckBox, "overlay_range")
 
-        self.zoom_magnification = self.findChild(QComboBox, "zoom_magnification")
+        self.zoom_magnification = self.findChild(
+            QComboBox, "zoom_magnification"
+        )
         self.zoom_apply = self.findChild(QPushButton, "zoom_apply")
 
         # cellpose controls + variables from Qt Desinger References
         self.cellpose_segmentation = False
         self.cellpose_model = None
         self.cellpose_custom_model_path = ""
         self.cellpose_train_model_path = ""
         self.cellpose_log_file = None
-        self.cellpose_select_custom_model = self.findChild(QPushButton, "cellpose_select_custom_model")
+        self.cellpose_select_custom_model = self.findChild(
+            QPushButton, "cellpose_select_custom_model"
+        )
         self.cellpose_segmodel = self.findChild(QComboBox, "cellpose_segmodel")
-        self.cellpose_trainmodel = self.findChild(QComboBox, "cellpose_trainmodel")
-        self.cellpose_segchannel = self.findChild(QComboBox, "cellpose_segchannel")
-        self.cellpose_flowthresh = self.findChild(QSlider, "cellpose_flowthresh")
-        self.cellpose_flowthresh_label = self.findChild(QLabel, "cellpose_flowthresh_label")
-        self.cellpose_maskthresh = self.findChild(QSlider, "cellpose_maskthresh")
-        self.cellpose_maskthresh_label = self.findChild(QLabel, "cellpose_maskthresh_label")
+        self.cellpose_trainmodel = self.findChild(
+            QComboBox, "cellpose_trainmodel"
+        )
+        self.cellpose_segchannel = self.findChild(
+            QComboBox, "cellpose_segchannel"
+        )
+        self.cellpose_flowthresh = self.findChild(
+            QSlider, "cellpose_flowthresh"
+        )
+        self.cellpose_flowthresh_label = self.findChild(
+            QLabel, "cellpose_flowthresh_label"
+        )
+        self.cellpose_maskthresh = self.findChild(
+            QSlider, "cellpose_maskthresh"
+        )
+        self.cellpose_maskthresh_label = self.findChild(
+            QLabel, "cellpose_maskthresh_label"
+        )
         self.cellpose_minsize = self.findChild(QSlider, "cellpose_minsize")
-        self.cellpose_minsize_label = self.findChild(QLabel, "cellpose_minsize_label")
+        self.cellpose_minsize_label = self.findChild(
+            QLabel, "cellpose_minsize_label"
+        )
         self.cellpose_diameter = self.findChild(QSlider, "cellpose_diameter")
-        self.cellpose_diameter_label = self.findChild(QLabel, "cellpose_diameter_label")
-        self.cellpose_segment_active = self.findChild(QPushButton, "cellpose_segment_active")
-        self.cellpose_segment_all = self.findChild(QPushButton, "cellpose_segment_all")
-        self.cellpose_clear_previous = self.findChild(QCheckBox, "cellpose_clear_previous")
+        self.cellpose_diameter_label = self.findChild(
+            QLabel, "cellpose_diameter_label"
+        )
+        self.cellpose_segment_active = self.findChild(
+            QPushButton, "cellpose_segment_active"
+        )
+        self.cellpose_segment_all = self.findChild(
+            QPushButton, "cellpose_segment_all"
+        )
+        self.cellpose_clear_previous = self.findChild(
+            QCheckBox, "cellpose_clear_previous"
+        )
         self.cellpose_usegpu = self.findChild(QCheckBox, "cellpose_usegpu")
-        self.cellpose_resetimage = self.findChild(QCheckBox, "cellpose_resetimage")
-        self.cellpose_progressbar = self.findChild(QProgressBar, "cellpose_progressbar")
-        self.cellpose_train_model = self.findChild(QPushButton, "cellpose_train_model")
-        self.cellpose_save_dir = self.findChild(QPushButton, "cellpose_save_dir")
-        self.cellpose_trainchannel = self.findChild(QComboBox, "cellpose_trainchannel")
+        self.cellpose_resetimage = self.findChild(
+            QCheckBox, "cellpose_resetimage"
+        )
+        self.cellpose_progressbar = self.findChild(
+            QProgressBar, "cellpose_progressbar"
+        )
+        self.cellpose_train_model = self.findChild(
+            QPushButton, "cellpose_train_model"
+        )
+        self.cellpose_save_dir = self.findChild(
+            QPushButton, "cellpose_save_dir"
+        )
+        self.cellpose_trainchannel = self.findChild(
+            QComboBox, "cellpose_trainchannel"
+        )
         self.cellpose_nepochs = self.findChild(QComboBox, "cellpose_nepochs")
-        self.cellpose_batchsize = self.findChild(QComboBox, "cellpose_batchsize")
-        self.cellpose_min_seg_size = self.findChild(QComboBox, "cellpose_min_seg_size")
+        self.cellpose_batchsize = self.findChild(
+            QComboBox, "cellpose_batchsize"
+        )
+        self.cellpose_min_seg_size = self.findChild(
+            QComboBox, "cellpose_min_seg_size"
+        )
         self.cellpose_seg_mode = self.findChild(QComboBox, "cellpose_seg_mode")
 
         # modify tab controls + variables from Qt Desinger References
         self.interface_mode = "panzoom"
         self.segmentation_mode = "add"
         self.class_mode = "single"
         self.class_colour = 1
         self.modify_panzoom = self.findChild(QPushButton, "modify_panzoom")
         self.modify_segment = self.findChild(QPushButton, "modify_segment")
         self.modify_classify = self.findChild(QPushButton, "modify_classify")
         self.modify_refine = self.findChild(QPushButton, "modify_refine")
         self.refine_channel = self.findChild(QComboBox, "refine_channel")
         self.refine_all = self.findChild(QPushButton, "refine_all")
-        self.modify_copymasktoall = self.findChild(QPushButton, "modify_copymasktoall")
-        self.modify_deleteallmasks = self.findChild(QPushButton, "modify_deleteallmasks")
-        self.modify_deleteactivemasks = self.findChild(QPushButton, "modify_deleteactivemasks")
-        self.modify_deleteactiveimage = self.findChild(QPushButton, "modify_deleteactiveimage")
-        self.modify_deleteotherimages = self.findChild(QPushButton, "modify_deleteotherimages")
-        self.modify_progressbar = self.findChild(QProgressBar, "modify_progressbar")
+        self.modify_copymasktoall = self.findChild(
+            QPushButton, "modify_copymasktoall"
+        )
+        self.modify_deleteallmasks = self.findChild(
+            QPushButton, "modify_deleteallmasks"
+        )
+        self.modify_deleteactivemasks = self.findChild(
+            QPushButton, "modify_deleteactivemasks"
+        )
+        self.modify_deleteactiveimage = self.findChild(
+            QPushButton, "modify_deleteactiveimage"
+        )
+        self.modify_deleteotherimages = self.findChild(
+            QPushButton, "modify_deleteotherimages"
+        )
+        self.modify_progressbar = self.findChild(
+            QProgressBar, "modify_progressbar"
+        )
         self.modify_channel = self.findChild(QComboBox, "modify_channel")
 
-        self.modify_auto_panzoom = self.findChild(QCheckBox, "modify_auto_panzoom")
+        self.modify_auto_panzoom = self.findChild(
+            QCheckBox, "modify_auto_panzoom"
+        )
         self.modify_add = self.findChild(QPushButton, "modify_add")
         self.modify_extend = self.findChild(QPushButton, "modify_extend")
         self.modify_split = self.findChild(QPushButton, "modify_split")
         self.modify_join = self.findChild(QPushButton, "modify_join")
         self.modify_delete = self.findChild(QPushButton, "modify_delete")
         self.classify_single = self.findChild(QPushButton, "classify_single")
-        self.classify_dividing = self.findChild(QPushButton, "classify_dividing")
+        self.classify_dividing = self.findChild(
+            QPushButton, "classify_dividing"
+        )
         self.classify_divided = self.findChild(QPushButton, "classify_divided")
-        self.classify_vertical = self.findChild(QPushButton, "classify_vertical")
+        self.classify_vertical = self.findChild(
+            QPushButton, "classify_vertical"
+        )
         self.classify_broken = self.findChild(QPushButton, "classify_broken")
         self.classify_edge = self.findChild(QPushButton, "classify_edge")
         self.modify_viewmasks = self.findChild(QCheckBox, "modify_viewmasks")
         self.modify_viewlabels = self.findChild(QCheckBox, "modify_viewlabels")
         self.find_next = self.findChild(QPushButton, "find_next")
         self.find_previous = self.findChild(QPushButton, "find_previous")
         self.find_criterion = self.findChild(QComboBox, "find_criterion")
         self.find_mode = self.findChild(QComboBox, "find_mode")
         self.scalebar_show = self.findChild(QCheckBox, "scalebar_show")
-        self.scalebar_resolution = self.findChild(QLineEdit, "scalebar_resolution")
+        self.scalebar_resolution = self.findChild(
+            QLineEdit, "scalebar_resolution"
+        )
         self.scalebar_units = self.findChild(QComboBox, "scalebar_units")
 
         self.set_quality_mode = self.findChild(QComboBox, "set_quality_mode")
         self.set_focus_0 = self.findChild(QPushButton, "set_focus_0")
         self.set_focus_1 = self.findChild(QPushButton, "set_focus_1")
         self.set_focus_2 = self.findChild(QPushButton, "set_focus_2")
         self.set_focus_3 = self.findChild(QPushButton, "set_focus_3")
@@ -344,135 +490,284 @@
         self.set_debris_4 = self.findChild(QPushButton, "set_debris_4")
         self.set_debris_5 = self.findChild(QPushButton, "set_debris_5")
 
         # upload tab controls from Qt Desinger References
         self.database_path = ""
         self.user_metadata_keys = 6
 
-        self.metadata_columns = ["date_uploaded", "date_created", "date_modified", "file_name", "channel", "file_list", "channel_list", "segmentation_file", "segmentation_channel", "akseg_hash",
-            "user_initial", "content", "microscope", "modality", "source", "strain", "phenotype", "stain", "stain_target", "antibiotic", "treatment time (mins)", "antibiotic concentration",
-            "mounting method", "protocol", "folder", "parent_folder", "num_segmentations", "image_laplacian", "image_focus", "image_debris", "segmented", "labelled", "segmentation_curated",
-            "label_curated", "posX", "posY", "posZ", "image_load_path", "image_save_path", "mask_load_path", "mask_save_path", "label_load_path", "label_save_path", ]
+        self.metadata_columns = [
+            "date_uploaded",
+            "date_created",
+            "date_modified",
+            "file_name",
+            "channel",
+            "file_list",
+            "channel_list",
+            "segmentation_file",
+            "segmentation_channel",
+            "akseg_hash",
+            "user_initial",
+            "content",
+            "microscope",
+            "modality",
+            "source",
+            "strain",
+            "phenotype",
+            "stain",
+            "stain_target",
+            "antibiotic",
+            "treatment time (mins)",
+            "antibiotic concentration",
+            "mounting method",
+            "protocol",
+            "folder",
+            "parent_folder",
+            "num_segmentations",
+            "image_laplacian",
+            "image_focus",
+            "image_debris",
+            "segmented",
+            "labelled",
+            "segmentation_curated",
+            "label_curated",
+            "posX",
+            "posY",
+            "posZ",
+            "image_load_path",
+            "image_save_path",
+            "mask_load_path",
+            "mask_save_path",
+            "label_load_path",
+            "label_save_path",
+        ]
 
         user_key_list = np.arange(1, self.user_metadata_keys + 1).tolist()
         user_key_list.reverse()
 
         for key in user_key_list:
             user_key = f"user_meta{key}"
             self.metadata_columns.insert(22, str(user_key))
-            setattr(self, f"upload_usermeta{key}", self.findChild(QComboBox, f"upload_usermeta{key}"), )
+            setattr(
+                self,
+                f"upload_usermeta{key}",
+                self.findChild(QComboBox, f"upload_usermeta{key}"),
+            )
 
         self.upload_initial = self.findChild(QComboBox, "upload_initial")
         self.upload_content = self.findChild(QComboBox, "upload_content")
         self.upload_microscope = self.findChild(QComboBox, "upload_microscope")
         self.upload_antibiotic = self.findChild(QComboBox, "upload_antibiotic")
         self.upload_phenotype = self.findChild(QComboBox, "upload_phenotype")
         self.upload_strain = self.findChild(QComboBox, "upload_strain")
-        self.upload_abxconcentration = self.findChild(QComboBox, "upload_abxconcentration")
-        self.upload_treatmenttime = self.findChild(QComboBox, "upload_treatmenttime")
+        self.upload_abxconcentration = self.findChild(
+            QComboBox, "upload_abxconcentration"
+        )
+        self.upload_treatmenttime = self.findChild(
+            QComboBox, "upload_treatmenttime"
+        )
         self.upload_mount = self.findChild(QComboBox, "upload_mount")
         self.upload_protocol = self.findChild(QComboBox, "upload_protocol")
-        self.upload_overwrite_images = self.findChild(QCheckBox, "upload_overwrite_images")
-        self.upload_overwrite_masks = self.findChild(QCheckBox, "upload_overwrite_masks")
-        self.overwrite_selected_metadata = self.findChild(QCheckBox, "overwrite_selected_metadata")
-        self.overwrite_all_metadata = self.findChild(QCheckBox, "overwrite_all_metadata")
+        self.upload_overwrite_images = self.findChild(
+            QCheckBox, "upload_overwrite_images"
+        )
+        self.upload_overwrite_masks = self.findChild(
+            QCheckBox, "upload_overwrite_masks"
+        )
+        self.overwrite_selected_metadata = self.findChild(
+            QCheckBox, "overwrite_selected_metadata"
+        )
+        self.overwrite_all_metadata = self.findChild(
+            QCheckBox, "overwrite_all_metadata"
+        )
         self.upload_all = self.findChild(QPushButton, "upload_all")
         self.upload_active = self.findChild(QPushButton, "upload_active")
-        self.database_download = self.findChild(QPushButton, "database_download")
-        self.database_download_limit = self.findChild(QComboBox, "database_download_limit")
+        self.database_download = self.findChild(
+            QPushButton, "database_download"
+        )
+        self.database_download_limit = self.findChild(
+            QComboBox, "database_download_limit"
+        )
         self.create_database = self.findChild(QPushButton, "create_database")
         self.load_database = self.findChild(QPushButton, "load_database")
-        self.display_database_path = self.findChild(QLineEdit, "display_database_path")
-        self.upload_progressbar = self.findChild(QProgressBar, "upload_progressbar")
+        self.display_database_path = self.findChild(
+            QLineEdit, "display_database_path"
+        )
+        self.upload_progressbar = self.findChild(
+            QProgressBar, "upload_progressbar"
+        )
         self.upload_tab = self.findChild(QWidget, "upload_tab")
-        self.upload_segmentation_combo = self.findChild(QComboBox, "upload_segmentation_combo")
-        self.upload_label_combo = self.findChild(QComboBox, "upload_label_combo")
-        self.download_sort_order_1 = self.findChild(QComboBox, "download_sort_order_1")
-        self.download_sort_order_2 = self.findChild(QComboBox, "download_sort_order_2")
-        self.download_sort_direction_1 = self.findChild(QComboBox, "download_sort_direction_1")
-        self.download_sort_direction_2 = self.findChild(QComboBox, "download_sort_direction_2")
+        self.upload_segmentation_combo = self.findChild(
+            QComboBox, "upload_segmentation_combo"
+        )
+        self.upload_label_combo = self.findChild(
+            QComboBox, "upload_label_combo"
+        )
+        self.download_sort_order_1 = self.findChild(
+            QComboBox, "download_sort_order_1"
+        )
+        self.download_sort_order_2 = self.findChild(
+            QComboBox, "download_sort_order_2"
+        )
+        self.download_sort_direction_1 = self.findChild(
+            QComboBox, "download_sort_direction_1"
+        )
+        self.download_sort_direction_2 = self.findChild(
+            QComboBox, "download_sort_direction_2"
+        )
         self.update_metadata = self.findChild(QPushButton, "update_metadata")
-        self.upload_images_setting = self.findChild(QCheckBox, "upload_images_setting")
-        self.upload_segmentations_setting = self.findChild(QCheckBox, "upload_segmentations_setting")
-        self.upload_metadata_setting = self.findChild(QCheckBox, "upload_metadata_setting")
-
-        self.image_metadata_controls = self.findChild(QFormLayout, "image_metadata_controls")
+        self.upload_images_setting = self.findChild(
+            QCheckBox, "upload_images_setting"
+        )
+        self.upload_segmentations_setting = self.findChild(
+            QCheckBox, "upload_segmentations_setting"
+        )
+        self.upload_metadata_setting = self.findChild(
+            QCheckBox, "upload_metadata_setting"
+        )
+
+        self.image_metadata_controls = self.findChild(
+            QFormLayout, "image_metadata_controls"
+        )
 
         self._show_database_controls(False)
 
         # oufti tab controls
-        self.oufti_generate_all_midlines = self.findChild(QPushButton, "oufti_generate_all_midlines")
-        self.oufti_generate_active_midlines = self.findChild(QPushButton, "oufti_generate_active_midlines")
-        self.oufti_panzoom_mode = self.findChild(QRadioButton, "oufti_panzoom_mode")
+        self.oufti_generate_all_midlines = self.findChild(
+            QPushButton, "oufti_generate_all_midlines"
+        )
+        self.oufti_generate_active_midlines = self.findChild(
+            QPushButton, "oufti_generate_active_midlines"
+        )
+        self.oufti_panzoom_mode = self.findChild(
+            QRadioButton, "oufti_panzoom_mode"
+        )
         self.oufti_edit_mode = self.findChild(QRadioButton, "oufti_edit_mode")
-        self.oufti_midline_vertexes = self.findChild(QComboBox, "oufti_midline_vertexes")
-        self.oufti_centre_all_midlines = self.findChild(QPushButton, "oufti_centre_all_midlines")
-        self.oufti_centre_active_midlines = self.findChild(QPushButton, "oufti_centre_active_midlines")
+        self.oufti_midline_vertexes = self.findChild(
+            QComboBox, "oufti_midline_vertexes"
+        )
+        self.oufti_centre_all_midlines = self.findChild(
+            QPushButton, "oufti_centre_all_midlines"
+        )
+        self.oufti_centre_active_midlines = self.findChild(
+            QPushButton, "oufti_centre_active_midlines"
+        )
         self.oufti_mesh_length = self.findChild(QComboBox, "oufti_mesh_length")
-        self.oufti_mesh_dilation = self.findChild(QComboBox, "oufti_mesh_dilation")
+        self.oufti_mesh_dilation = self.findChild(
+            QComboBox, "oufti_mesh_dilation"
+        )
 
         # export tab controls from Qt Desinger References
         self.export_channel = self.findChild(QComboBox, "export_channel")
         self.export_mode = self.findChild(QComboBox, "export_mode")
         self.export_location = self.findChild(QComboBox, "export_location")
         self.export_modifier = self.findChild(QLineEdit, "export_modifier")
         self.export_single = self.findChild(QCheckBox, "export_single")
         self.export_dividing = self.findChild(QCheckBox, "export_dividing")
         self.export_divided = self.findChild(QCheckBox, "export_divided")
         self.export_vertical = self.findChild(QCheckBox, "export_vertical")
         self.export_broken = self.findChild(QCheckBox, "export_broken")
         self.export_edge = self.findChild(QCheckBox, "export_edge")
-        self.export_statistics_multithreaded = self.findChild(QCheckBox, "export_statistics_multithreaded")
+        self.export_statistics_multithreaded = self.findChild(
+            QCheckBox, "export_statistics_multithreaded"
+        )
         self.export_active = self.findChild(QPushButton, "export_active")
         self.export_all = self.findChild(QPushButton, "export_all")
         self.export_normalise = self.findChild(QCheckBox, "export_normalise")
         self.export_invert = self.findChild(QCheckBox, "export_invert")
         self.export_scalebar = self.findChild(QCheckBox, "export_scalebar")
-        self.export_scalebar_resolution = self.findChild(QLineEdit, "export_scalebar_resolution")
-        self.export_scalebar_resolution_units = self.findChild(QComboBox, "export_scalebar_resolution_units")
-        self.export_scalebar_size = self.findChild(QLineEdit, "export_scalebar_size")
-        self.export_scalebar_size_units = self.findChild(QComboBox, "export_scalebar_size_units")
-        self.export_scalebar_colour = self.findChild(QComboBox, "export_scalebar_colour")
-        self.export_scalebar_thickness = self.findChild(QComboBox, "export_scalebar_thickness")
+        self.export_scalebar_resolution = self.findChild(
+            QLineEdit, "export_scalebar_resolution"
+        )
+        self.export_scalebar_resolution_units = self.findChild(
+            QComboBox, "export_scalebar_resolution_units"
+        )
+        self.export_scalebar_size = self.findChild(
+            QLineEdit, "export_scalebar_size"
+        )
+        self.export_scalebar_size_units = self.findChild(
+            QComboBox, "export_scalebar_size_units"
+        )
+        self.export_scalebar_colour = self.findChild(
+            QComboBox, "export_scalebar_colour"
+        )
+        self.export_scalebar_thickness = self.findChild(
+            QComboBox, "export_scalebar_thickness"
+        )
         self.export_cropzoom = self.findChild(QCheckBox, "export_crop_zoom")
-        self.export_mask_background = self.findChild(QCheckBox, "export_mask_background")
-
-        self.export_stack_channel = self.findChild(QComboBox, "export_stack_channel")
+        self.export_mask_background = self.findChild(
+            QCheckBox, "export_mask_background"
+        )
+
+        self.export_stack_channel = self.findChild(
+            QComboBox, "export_stack_channel"
+        )
         self.export_stack_mode = self.findChild(QComboBox, "export_stack_mode")
-        self.export_stack_location = self.findChild(QComboBox, "export_stack_location")
-        self.export_stack_modifier = self.findChild(QLineEdit, "export_stack_modifier")
-        self.export_stack_image_setting = self.findChild(QCheckBox, "export_stack_image_setting")
-        self.export_stack_overwrite_setting = self.findChild(QCheckBox, "export_stack_overwrite_setting")
-        self.export_stack_active = self.findChild(QPushButton, "export_stack_active")
+        self.export_stack_location = self.findChild(
+            QComboBox, "export_stack_location"
+        )
+        self.export_stack_modifier = self.findChild(
+            QLineEdit, "export_stack_modifier"
+        )
+        self.export_stack_image_setting = self.findChild(
+            QCheckBox, "export_stack_image_setting"
+        )
+        self.export_stack_overwrite_setting = self.findChild(
+            QCheckBox, "export_stack_overwrite_setting"
+        )
+        self.export_stack_active = self.findChild(
+            QPushButton, "export_stack_active"
+        )
         self.export_stack_all = self.findChild(QPushButton, "export_stack_all")
 
-        self.export_autocontrast = self.findChild(QCheckBox, "export_autocontrast")
-        self.export_statistics_pixelsize = self.findChild(QLineEdit, "export_statistics_pixelsize")
-        self.export_statistics_active = self.findChild(QPushButton, "export_statistics_active")
-        self.export_statistics_all = self.findChild(QPushButton, "export_statistics_all")
-        self.export_colicoords_mode = self.findChild(QComboBox, "export_colicoords_mode")
-        self.export_progressbar = self.findChild(QProgressBar, "export_progressbar")
-        self.export_image_setting = self.findChild(QCheckBox, "export_image_setting")
-        self.export_overwrite_setting = self.findChild(QCheckBox, "export_overwrite_setting")
+        self.export_autocontrast = self.findChild(
+            QCheckBox, "export_autocontrast"
+        )
+        self.export_statistics_pixelsize = self.findChild(
+            QLineEdit, "export_statistics_pixelsize"
+        )
+        self.export_statistics_active = self.findChild(
+            QPushButton, "export_statistics_active"
+        )
+        self.export_statistics_all = self.findChild(
+            QPushButton, "export_statistics_all"
+        )
+        self.export_colicoords_mode = self.findChild(
+            QComboBox, "export_colicoords_mode"
+        )
+        self.export_progressbar = self.findChild(
+            QProgressBar, "export_progressbar"
+        )
+        self.export_image_setting = self.findChild(
+            QCheckBox, "export_image_setting"
+        )
+        self.export_overwrite_setting = self.findChild(
+            QCheckBox, "export_overwrite_setting"
+        )
         self.export_directory = ""
 
         # import events
         self.autocontrast.stateChanged.connect(self._autoContrast)
         self.import_import.clicked.connect(self._importDialog)
         self.label_overwrite.clicked.connect(self.overwrite_channel_info)
-        self.import_mode.currentIndexChanged.connect(self._set_available_multiframe_modes)
+        self.import_mode.currentIndexChanged.connect(
+            self._set_available_multiframe_modes
+        )
 
         # view events
         self.fold.clicked.connect(self.fold_images)
         self.unfold.clicked.connect(self.unfold_images)
         self.tiler_object = None
         self.tile_dict = {"Segmentations": [], "Classes": [], "Nucleoid": []}
         self.unfolded = False
-        self.align_active_image.clicked.connect(partial(self._align_images, mode="active"))
-        self.align_all_images.clicked.connect(partial(self._align_images, mode="all"))
+        self.align_active_image.clicked.connect(
+            partial(self._align_images, mode="active")
+        )
+        self.align_all_images.clicked.connect(
+            partial(self._align_images, mode="all")
+        )
         self.scalebar_show.stateChanged.connect(self._updateScaleBar)
         self.scalebar_resolution.textChanged.connect(self._updateScaleBar)
         self.scalebar_units.currentTextChanged.connect(self._updateScaleBar)
         self.overlay_filename.stateChanged.connect(self._updateFileName)
         self.overlay_folder.stateChanged.connect(self._updateFileName)
         self.overlay_microscope.stateChanged.connect(self._updateFileName)
         self.overlay_datemodified.stateChanged.connect(self._updateFileName)
@@ -487,85 +782,159 @@
         self.overlay_focus.stateChanged.connect(self._updateFileName)
         self.overlay_debris.stateChanged.connect(self._updateFileName)
         self.overlay_laplacian.stateChanged.connect(self._updateFileName)
         self.overlay_range.stateChanged.connect(self._updateFileName)
         self.zoom_apply.clicked.connect(self._applyZoom)
 
         # cellpose events
-        self.cellpose_flowthresh.valueChanged.connect(lambda: self._updateSliderLabel("cellpose_flowthresh", "cellpose_flowthresh_label"))
-        self.cellpose_maskthresh.valueChanged.connect(lambda: self._updateSliderLabel("cellpose_maskthresh", "cellpose_maskthresh_label"))
-        self.cellpose_minsize.valueChanged.connect(lambda: self._updateSliderLabel("cellpose_minsize", "cellpose_minsize_label"))
-        self.cellpose_diameter.valueChanged.connect(lambda: self._updateSliderLabel("cellpose_diameter", "cellpose_diameter_label"))
-
-        self.cellpose_select_custom_model.clicked.connect(self._select_custom_cellpose_model)
-        self.cellpose_save_dir.clicked.connect(self._select_cellpose_save_directory)
+        self.cellpose_flowthresh.valueChanged.connect(
+            lambda: self._updateSliderLabel(
+                "cellpose_flowthresh", "cellpose_flowthresh_label"
+            )
+        )
+        self.cellpose_maskthresh.valueChanged.connect(
+            lambda: self._updateSliderLabel(
+                "cellpose_maskthresh", "cellpose_maskthresh_label"
+            )
+        )
+        self.cellpose_minsize.valueChanged.connect(
+            lambda: self._updateSliderLabel(
+                "cellpose_minsize", "cellpose_minsize_label"
+            )
+        )
+        self.cellpose_diameter.valueChanged.connect(
+            lambda: self._updateSliderLabel(
+                "cellpose_diameter", "cellpose_diameter_label"
+            )
+        )
+
+        self.cellpose_select_custom_model.clicked.connect(
+            self._select_custom_cellpose_model
+        )
+        self.cellpose_save_dir.clicked.connect(
+            self._select_cellpose_save_directory
+        )
         self.cellpose_segment_all.clicked.connect(self._segmentAll)
         self.cellpose_segment_active.clicked.connect(self._segmentActive)
         self.cellpose_train_model.clicked.connect(self._trainCellpose)
-        self.cellpose_segchannel.currentTextChanged.connect(self._updateSegChannels)
+        self.cellpose_segchannel.currentTextChanged.connect(
+            self._updateSegChannels
+        )
 
         # modify tab events
         self.modify_panzoom.clicked.connect(self._modifyMode(mode="panzoom"))
         self.modify_segment.clicked.connect(self._modifyMode(mode="segment"))
         self.modify_classify.clicked.connect(self._modifyMode(mode="classify"))
         self.modify_refine.clicked.connect(self._modifyMode(mode="refine"))
         self.modify_add.clicked.connect(self._modifyMode(mode="add"))
         self.modify_extend.clicked.connect(self._modifyMode(mode="extend"))
         self.modify_join.clicked.connect(self._modifyMode(mode="join"))
         self.modify_split.clicked.connect(self._modifyMode(mode="split"))
         self.modify_delete.clicked.connect(self._modifyMode(mode="delete"))
         self.classify_single.clicked.connect(self._modifyMode(mode="single"))
-        self.classify_dividing.clicked.connect(self._modifyMode(mode="dividing"))
+        self.classify_dividing.clicked.connect(
+            self._modifyMode(mode="dividing")
+        )
         self.classify_divided.clicked.connect(self._modifyMode(mode="divided"))
-        self.classify_vertical.clicked.connect(self._modifyMode(mode="vertical"))
+        self.classify_vertical.clicked.connect(
+            self._modifyMode(mode="vertical")
+        )
         self.classify_broken.clicked.connect(self._modifyMode(mode="broken"))
         self.classify_edge.clicked.connect(self._modifyMode(mode="edge"))
 
         self.viewer.bind_key(key="b", func=self.set_blurred, overwrite=True)
-        self.set_focus_1.clicked.connect(partial(self.set_image_quality, mode="focus", value=1))
-        self.set_focus_2.clicked.connect(partial(self.set_image_quality, mode="focus", value=2))
-        self.set_focus_3.clicked.connect(partial(self.set_image_quality, mode="focus", value=3))
-        self.set_focus_4.clicked.connect(partial(self.set_image_quality, mode="focus", value=4))
-        self.set_focus_5.clicked.connect(partial(self.set_image_quality, mode="focus", value=5))
+        self.set_focus_1.clicked.connect(
+            partial(self.set_image_quality, mode="focus", value=1)
+        )
+        self.set_focus_2.clicked.connect(
+            partial(self.set_image_quality, mode="focus", value=2)
+        )
+        self.set_focus_3.clicked.connect(
+            partial(self.set_image_quality, mode="focus", value=3)
+        )
+        self.set_focus_4.clicked.connect(
+            partial(self.set_image_quality, mode="focus", value=4)
+        )
+        self.set_focus_5.clicked.connect(
+            partial(self.set_image_quality, mode="focus", value=5)
+        )
         self.viewer.bind_key(key="f", func=self.set_focused, overwrite=True)
 
-        self.set_debris_1.clicked.connect(partial(self.set_image_quality, mode="debris", value=1))
-        self.set_debris_2.clicked.connect(partial(self.set_image_quality, mode="debris", value=2))
-        self.set_debris_3.clicked.connect(partial(self.set_image_quality, mode="debris", value=3))
-        self.set_debris_4.clicked.connect(partial(self.set_image_quality, mode="debris", value=4))
-        self.set_debris_5.clicked.connect(partial(self.set_image_quality, mode="debris", value=5))
-
-        self.modify_viewmasks.stateChanged.connect(self._viewerControls("viewmasks"))
-        self.modify_viewlabels.stateChanged.connect(self._viewerControls("viewlabels"))
+        self.set_debris_1.clicked.connect(
+            partial(self.set_image_quality, mode="debris", value=1)
+        )
+        self.set_debris_2.clicked.connect(
+            partial(self.set_image_quality, mode="debris", value=2)
+        )
+        self.set_debris_3.clicked.connect(
+            partial(self.set_image_quality, mode="debris", value=3)
+        )
+        self.set_debris_4.clicked.connect(
+            partial(self.set_image_quality, mode="debris", value=4)
+        )
+        self.set_debris_5.clicked.connect(
+            partial(self.set_image_quality, mode="debris", value=5)
+        )
+
+        self.modify_viewmasks.stateChanged.connect(
+            self._viewerControls("viewmasks")
+        )
+        self.modify_viewlabels.stateChanged.connect(
+            self._viewerControls("viewlabels")
+        )
         self.refine_all.clicked.connect(self._refine_bacseg)
         self.modify_copymasktoall.clicked.connect(self._copymasktoall)
-        self.modify_deleteallmasks.clicked.connect(self._deleteallmasks(mode="all"))
-        self.modify_deleteactivemasks.clicked.connect(self._deleteallmasks(mode="active"))
-        self.modify_deleteactiveimage.clicked.connect(self._delete_active_image(mode="active"))
-        self.modify_deleteotherimages.clicked.connect(self._delete_active_image(mode="other"))
+        self.modify_deleteallmasks.clicked.connect(
+            self._deleteallmasks(mode="all")
+        )
+        self.modify_deleteactivemasks.clicked.connect(
+            self._deleteallmasks(mode="active")
+        )
+        self.modify_deleteactiveimage.clicked.connect(
+            self._delete_active_image(mode="active")
+        )
+        self.modify_deleteotherimages.clicked.connect(
+            self._delete_active_image(mode="other")
+        )
         self.find_next.clicked.connect(self._sort_cells("next"))
         self.find_previous.clicked.connect(self._sort_cells("previous"))
-        self.modify_channel.currentTextChanged.connect(self._modify_channel_changed)
+        self.modify_channel.currentTextChanged.connect(
+            self._modify_channel_changed
+        )
 
         # export events
         self.export_active.clicked.connect(self._export("active"))
         self.export_all.clicked.connect(self._export("all"))
         self.export_stack_active.clicked.connect(self._export_stack("active"))
         self.export_stack_all.clicked.connect(self._export_stack("all"))
-        self.export_statistics_active.clicked.connect(self._export_statistics("active"))
-        self.export_statistics_all.clicked.connect(self._export_statistics("all"))
+        self.export_statistics_active.clicked.connect(
+            self._export_statistics("active")
+        )
+        self.export_statistics_all.clicked.connect(
+            self._export_statistics("all")
+        )
 
         # oufti events
-        self.oufti_generate_all_midlines.clicked.connect(self.generate_midlines(mode="all"))
-        self.oufti_generate_active_midlines.clicked.connect(self.generate_midlines(mode="active"))
-        self.viewer.bind_key(key="m", func=self.midline_edit_toggle, overwrite=True)
+        self.oufti_generate_all_midlines.clicked.connect(
+            self.generate_midlines(mode="all")
+        )
+        self.oufti_generate_active_midlines.clicked.connect(
+            self.generate_midlines(mode="active")
+        )
+        self.viewer.bind_key(
+            key="m", func=self.midline_edit_toggle, overwrite=True
+        )
         self.oufti_edit_mode.clicked.connect(self.midline_edit_toggle)
         self.oufti_panzoom_mode.clicked.connect(self.midline_edit_toggle)
-        self.oufti_centre_all_midlines.clicked.connect(self.centre_oufti_midlines(mode="all"))
-        self.oufti_centre_active_midlines.clicked.connect(self.centre_oufti_midlines(mode="active"))
+        self.oufti_centre_all_midlines.clicked.connect(
+            self.centre_oufti_midlines(mode="all")
+        )
+        self.oufti_centre_active_midlines.clicked.connect(
+            self.centre_oufti_midlines(mode="active")
+        )
 
         # upload tab events
         self.upload_all.clicked.connect(self._uploadDatabase(mode="all"))
         self.upload_active.clicked.connect(self._uploadDatabase(mode="active"))
         self.database_download.clicked.connect(self._downloadDatabase)
         self.create_database.clicked.connect(self._create_bacseg_database)
         self.load_database.clicked.connect(self._load_bacseg_database)
@@ -574,172 +943,351 @@
         self.update_metadata.clicked.connect(self.update_database_metadata)
 
         # viewer event that call updateFileName when the slider is modified
         self.contours = []
         self.viewer.dims.events.current_step.connect(self._sliderEvent)
 
         # self.segImage = self.viewer.add_image(np.zeros((1,100,100),dtype=np.uint16),name="Image")
-        self.class_colours = {1: (255 / 255, 255 / 255, 255 / 255, 1), 2: (0 / 255, 255 / 255, 0 / 255, 1), 3: (0 / 255, 170 / 255, 255 / 255, 1), 4: (170 / 255, 0 / 255, 255 / 255, 1), 5: (
-        255 / 255, 170 / 255, 0 / 255, 1), 6: (255 / 255, 0 / 255, 0 / 255, 1), }
-
-        self.classLayer = self.viewer.add_labels(np.zeros((1, 100, 100), dtype=np.uint16), opacity=0.25, name="Classes", color=self.class_colours, metadata={0: {"image_name": ""}}, visible=False, )
-        self.nucLayer = self.viewer.add_labels(np.zeros((1, 100, 100), dtype=np.uint16), opacity=1, name="Nucleoid", metadata={0: {"image_name": ""}}, )
-        self.segLayer = self.viewer.add_labels(np.zeros((1, 100, 100), dtype=np.uint16), opacity=1, name="Segmentations", metadata={0: {"image_name": ""}}, )
+        self.class_colours = {
+            1: (255 / 255, 255 / 255, 255 / 255, 1),
+            2: (0 / 255, 255 / 255, 0 / 255, 1),
+            3: (0 / 255, 170 / 255, 255 / 255, 1),
+            4: (170 / 255, 0 / 255, 255 / 255, 1),
+            5: (255 / 255, 170 / 255, 0 / 255, 1),
+            6: (255 / 255, 0 / 255, 0 / 255, 1),
+        }
+
+        self.classLayer = self.viewer.add_labels(
+            np.zeros((1, 100, 100), dtype=np.uint16),
+            opacity=0.25,
+            name="Classes",
+            color=self.class_colours,
+            metadata={0: {"image_name": ""}},
+            visible=False,
+        )
+        self.nucLayer = self.viewer.add_labels(
+            np.zeros((1, 100, 100), dtype=np.uint16),
+            opacity=1,
+            name="Nucleoid",
+            metadata={0: {"image_name": ""}},
+        )
+        self.segLayer = self.viewer.add_labels(
+            np.zeros((1, 100, 100), dtype=np.uint16),
+            opacity=1,
+            name="Segmentations",
+            metadata={0: {"image_name": ""}},
+        )
 
         self.segLayer.contour = 1
 
         # keyboard events, only triggered when viewer is not empty (an image is loaded/active)
-        self.viewer.bind_key(key="a", func=self._modifyMode(mode="add"), overwrite=True)
-        self.viewer.bind_key(key="e", func=self._modifyMode(mode="extend"), overwrite=True)
-        self.viewer.bind_key(key="j", func=self._modifyMode(mode="join"), overwrite=True)
-        self.viewer.bind_key(key="s", func=self._modifyMode(mode="split"), overwrite=True)
-        self.viewer.bind_key(key="d", func=self._modifyMode(mode="delete"), overwrite=True)
-        self.viewer.bind_key(key="r", func=self._modifyMode(mode="refine"), overwrite=True)
-        self.viewer.bind_key(key="k", func=self._modifyMode(mode="clicktozoom"), overwrite=True)
-        self.viewer.bind_key(key="Control-1", func=self._modifyMode(mode="single"), overwrite=True, )
-        self.viewer.bind_key(key="Control-2", func=self._modifyMode(mode="dividing"), overwrite=True, )
-        self.viewer.bind_key(key="Control-3", func=self._modifyMode(mode="divided"), overwrite=True, )
-        self.viewer.bind_key(key="Control-4", func=self._modifyMode(mode="vertical"), overwrite=True, )
-        self.viewer.bind_key(key="Control-5", func=self._modifyMode(mode="broken"), overwrite=True, )
-        self.viewer.bind_key(key="Control-6", func=self._modifyMode(mode="edge"), overwrite=True)
-        self.viewer.bind_key(key="F1", func=self._modifyMode(mode="panzoom"), overwrite=True)
-        self.viewer.bind_key(key="F2", func=self._modifyMode(mode="segment"), overwrite=True)
-        self.viewer.bind_key(key="F3", func=self._modifyMode(mode="classify"), overwrite=True)
-        self.viewer.bind_key(key="h", func=self._viewerControls("h"), overwrite=True)
-        self.viewer.bind_key(key="i", func=self._viewerControls("i"), overwrite=True)
-        self.viewer.bind_key(key="o", func=self._viewerControls("o"), overwrite=True)
-        self.viewer.bind_key(key="x", func=self._viewerControls("x"), overwrite=True)
-        self.viewer.bind_key(key="z", func=self._viewerControls("z"), overwrite=True)
-        self.viewer.bind_key(key="c", func=self._viewerControls("c"), overwrite=True)
-        self.viewer.bind_key(key="Right", func=self._imageControls("Right"), overwrite=True)
-        self.viewer.bind_key(key="Left", func=self._imageControls("Left"), overwrite=True)
-        self.viewer.bind_key(key="u", func=self._imageControls("Upload"), overwrite=True)
-        self.viewer.bind_key(key="Control-d", func=self._deleteallmasks(mode="active"), overwrite=True, )
-        self.viewer.bind_key(key="Control-Shift-d", func=self._deleteallmasks(mode="all"), overwrite=True, )
-        self.viewer.bind_key(key="Control-i", func=self._delete_active_image(mode="active"), overwrite=True, )
-        self.viewer.bind_key(key="Control-Shift-i", func=self._delete_active_image(mode="other"), overwrite=True, )
-
-        self.viewer.bind_key(key="Control-l", func=self._downloadDatabase(), overwrite=True)
-        self.viewer.bind_key(key="Control-u", func=self._uploadDatabase(mode="active"), overwrite=True, )
-        self.viewer.bind_key(key="Control-Shift-u", func=self._uploadDatabase(mode="all"), overwrite=True, )
+        self.viewer.bind_key(
+            key="a", func=self._modifyMode(mode="add"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="e", func=self._modifyMode(mode="extend"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="j", func=self._modifyMode(mode="join"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="s", func=self._modifyMode(mode="split"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="d", func=self._modifyMode(mode="delete"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="r", func=self._modifyMode(mode="refine"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="k", func=self._modifyMode(mode="clicktozoom"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="Control-1",
+            func=self._modifyMode(mode="single"),
+            overwrite=True,
+        )
+        self.viewer.bind_key(
+            key="Control-2",
+            func=self._modifyMode(mode="dividing"),
+            overwrite=True,
+        )
+        self.viewer.bind_key(
+            key="Control-3",
+            func=self._modifyMode(mode="divided"),
+            overwrite=True,
+        )
+        self.viewer.bind_key(
+            key="Control-4",
+            func=self._modifyMode(mode="vertical"),
+            overwrite=True,
+        )
+        self.viewer.bind_key(
+            key="Control-5",
+            func=self._modifyMode(mode="broken"),
+            overwrite=True,
+        )
+        self.viewer.bind_key(
+            key="Control-6", func=self._modifyMode(mode="edge"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="F1", func=self._modifyMode(mode="panzoom"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="F2", func=self._modifyMode(mode="segment"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="F3", func=self._modifyMode(mode="classify"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="h", func=self._viewerControls("h"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="i", func=self._viewerControls("i"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="o", func=self._viewerControls("o"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="x", func=self._viewerControls("x"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="z", func=self._viewerControls("z"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="c", func=self._viewerControls("c"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="Right", func=self._imageControls("Right"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="Left", func=self._imageControls("Left"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="u", func=self._imageControls("Upload"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="Control-d",
+            func=self._deleteallmasks(mode="active"),
+            overwrite=True,
+        )
+        self.viewer.bind_key(
+            key="Control-Shift-d",
+            func=self._deleteallmasks(mode="all"),
+            overwrite=True,
+        )
+        self.viewer.bind_key(
+            key="Control-i",
+            func=self._delete_active_image(mode="active"),
+            overwrite=True,
+        )
+        self.viewer.bind_key(
+            key="Control-Shift-i",
+            func=self._delete_active_image(mode="other"),
+            overwrite=True,
+        )
+
+        self.viewer.bind_key(
+            key="Control-l", func=self._downloadDatabase(), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="Control-u",
+            func=self._uploadDatabase(mode="active"),
+            overwrite=True,
+        )
+        self.viewer.bind_key(
+            key="Control-Shift-u",
+            func=self._uploadDatabase(mode="all"),
+            overwrite=True,
+        )
         #
-        self.viewer.bind_key(key="Control-Left", func=self._manual_align_channels("left", mode="active"), overwrite=True, )
-        self.viewer.bind_key(key="Control-Right", func=self._manual_align_channels("right", mode="active"), overwrite=True, )
-        self.viewer.bind_key(key="Control-Up", func=self._manual_align_channels("up", mode="active"), overwrite=True, )
-        self.viewer.bind_key(key="Control-Down", func=self._manual_align_channels("down", mode="active"), overwrite=True, )
-
-        self.viewer.bind_key(key="Alt-Left", func=self._manual_align_channels("left", mode="all"), overwrite=True, )
-        self.viewer.bind_key(key="Alt-Right", func=self._manual_align_channels("right", mode="all"), overwrite=True, )
-        self.viewer.bind_key(key="Alt-Up", func=self._manual_align_channels("up", mode="all"), overwrite=True, )
-        self.viewer.bind_key(key="Alt-Down", func=self._manual_align_channels("down", mode="all"), overwrite=True, )
-
-        self.import_filemode.currentIndexChanged.connect(self.update_import_limit)
+        self.viewer.bind_key(
+            key="Control-Left",
+            func=self._manual_align_channels("left", mode="active"),
+            overwrite=True,
+        )
+        self.viewer.bind_key(
+            key="Control-Right",
+            func=self._manual_align_channels("right", mode="active"),
+            overwrite=True,
+        )
+        self.viewer.bind_key(
+            key="Control-Up",
+            func=self._manual_align_channels("up", mode="active"),
+            overwrite=True,
+        )
+        self.viewer.bind_key(
+            key="Control-Down",
+            func=self._manual_align_channels("down", mode="active"),
+            overwrite=True,
+        )
+
+        self.viewer.bind_key(
+            key="Alt-Left",
+            func=self._manual_align_channels("left", mode="all"),
+            overwrite=True,
+        )
+        self.viewer.bind_key(
+            key="Alt-Right",
+            func=self._manual_align_channels("right", mode="all"),
+            overwrite=True,
+        )
+        self.viewer.bind_key(
+            key="Alt-Up",
+            func=self._manual_align_channels("up", mode="all"),
+            overwrite=True,
+        )
+        self.viewer.bind_key(
+            key="Alt-Down",
+            func=self._manual_align_channels("down", mode="all"),
+            overwrite=True,
+        )
+
+        self.import_filemode.currentIndexChanged.connect(
+            self.update_import_limit
+        )
+        self.import_mode.currentIndexChanged.connect(self.update_import_limit)
         self.update_import_limit()
 
         # mouse events
         self.segLayer.mouse_drag_callbacks.append(self._segmentationEvents)
         self.nucLayer.mouse_drag_callbacks.append(self._segmentationEvents)
 
         # self.segLayer.mouse_move_callbac1ks.append(self._zoomEvents)
-        self.segLayer.mouse_double_click_callbacks.append(self._doubeClickEvents)
+        self.segLayer.mouse_double_click_callbacks.append(
+            self._doubeClickEvents
+        )
 
         # viewer events
         self.viewer.layers.events.inserted.connect(self._manualImport)
-        self.viewer.layers.events.removed.connect(self._updateSegmentationCombo)
-        self.viewer.layers.selection.events.changed.connect(self._updateFileName)
+        self.viewer.layers.events.removed.connect(
+            self._updateSegmentationCombo
+        )
+        self.viewer.layers.selection.events.changed.connect(
+            self._updateFileName
+        )
 
         self.threadpool = QThreadPool()  # self.load_dev_data()
 
         self.widget_notifications = True
 
     def _set_available_multiframe_modes(self):
-
-        multiframe_items = [self.import_multiframe_mode.itemText(i) for i in range(self.import_multiframe_mode.count())]
+        multiframe_items = [
+            self.import_multiframe_mode.itemText(i)
+            for i in range(self.import_multiframe_mode.count())
+        ]
         mode = self.import_mode.currentText()
 
         if mode in ["Images", "NanoImager Data", "ImageJ files(s)"]:
-            if 'Keep All Frames (BETA)' not in multiframe_items:
-                self.import_multiframe_mode.addItem('Keep All Frames (BETA)')
+            if "Keep All Frames (BETA)" not in multiframe_items:
+                self.import_multiframe_mode.addItem("Keep All Frames (BETA)")
         else:
-            if 'Keep All Frames (BETA)' in multiframe_items:
-                self.import_multiframe_mode.removeItem(multiframe_items.index('Keep All Frames (BETA)'))
+            if "Keep All Frames (BETA)" in multiframe_items:
+                self.import_multiframe_mode.removeItem(
+                    multiframe_items.index("Keep All Frames (BETA)")
+                )
 
     def _applyZoom(self):
         try:
             import re
 
             magnification = self.zoom_magnification.currentText()
             pixel_resolution = float(self.scalebar_resolution.text())
-            magnification = (magnification.lower().replace("x", "").replace("%", ""))
+            magnification = (
+                magnification.lower().replace("x", "").replace("%", "")
+            )
 
             magnification = re.findall(r"\b\d+\b", magnification)[0]
 
             if magnification.isdigit():
                 magnification = int(magnification)
 
                 if magnification == 0:
                     self.viewer.reset_view()
                 elif magnification > 0:
                     magnification = 1 + magnification / 100
 
-                    self.viewer.camera.zoom = magnification * (1 / pixel_resolution)
+                    self.viewer.camera.zoom = magnification * (
+                        1 / pixel_resolution
+                    )
 
         except:
             print(traceback.format_exc())
 
     def _align_images(self, viewer=None, mode="active"):
         import scipy
         from skimage.registration import phase_cross_correlation
 
         try:
-            layer_names = [layer.name for layer in self.viewer.layers if layer.name not in ["Segmentations", "Nucleoid", "Classes", "center_lines"]]
+            layer_names = [
+                layer.name
+                for layer in self.viewer.layers
+                if layer.name
+                not in ["Segmentations", "Nucleoid", "Classes", "center_lines"]
+            ]
 
             if len(layer_names) > 2:
                 num_images = self.viewer.layers[layer_names[0]].data.shape[0]
 
                 if mode == "active":
                     fov_list = [self.viewer.dims.current_step[0]]
                 else:
                     fov_list = range(num_images)
 
                 alignment_channel = self.alignment_channel.currentText()
                 current_fov = self.viewer.dims.current_step[0]
 
-                target_channels = [layer for layer in layer_names if layer != alignment_channel]
+                target_channels = [
+                    layer
+                    for layer in layer_names
+                    if layer != alignment_channel
+                ]
 
                 for channel in target_channels:
                     image_stack = self.viewer.layers[channel].data.copy()
-                    target_image_stack = self.viewer.layers[alignment_channel].data.copy()
+                    target_image_stack = self.viewer.layers[
+                        alignment_channel
+                    ].data.copy()
 
                     for fov in fov_list:
                         target_image = image_stack[fov, :, :]
                         alignment_image = target_image_stack[fov, :, :]
 
-                        shift, error, diffphase = phase_cross_correlation(alignment_image, target_image, upsample_factor=100)
+                        shift, error, diffphase = phase_cross_correlation(
+                            alignment_image, target_image, upsample_factor=100
+                        )
 
                         shifted_img = scipy.ndimage.shift(target_image, shift)
 
                         image_stack[fov, :, :] = shifted_img
 
                     self.viewer.layers[channel].data = image_stack
 
-                show_info(f"{len(fov_list)} Image(s) aligned to channel: " + alignment_channel)
+                show_info(
+                    f"{len(fov_list)} Image(s) aligned to channel: "
+                    + alignment_channel
+                )
 
         except:
             pass
 
     def set_blurred(self, viewer=None):
         self.set_image_quality(mode="focus", value=1)
 
     def set_focused(self, viewer=None):
         self.set_image_quality(mode="focus", value=5)
 
     def set_image_quality(self, mode="", value=""):
         try:
-            layer_names = [layer.name for layer in self.viewer.layers if layer.name not in ["Segmentations", "Nucleoid", "Classes", "center_lines"]]
+            layer_names = [
+                layer.name
+                for layer in self.viewer.layers
+                if layer.name
+                not in ["Segmentations", "Nucleoid", "Classes", "center_lines"]
+            ]
 
             update_mode = self.set_quality_mode.currentIndex()
 
             if len(layer_names) > 0:
                 current_fov = self.viewer.dims.current_step[0]
                 n_frames = self.viewer.dims.nsteps[0]
                 active_layer = self.viewer.layers.selection.active.name
@@ -782,21 +1330,28 @@
         except:
             pass
 
         return func
 
     def overwrite_channel_info(self):
         all_layers = [layer.name for layer in self.viewer.layers]
-        selected_layers = [layer.name for layer in self.viewer.layers.selection]
+        selected_layers = [
+            layer.name for layer in self.viewer.layers.selection
+        ]
 
         if len(selected_layers) == 1:
             selected_layer = selected_layers[0]
             all_layers.pop(all_layers.index(selected_layer))
 
-            if selected_layer not in ["Segmentations", "Nucleoid", "Classes", "center_lines", ]:
+            if selected_layer not in [
+                "Segmentations",
+                "Nucleoid",
+                "Classes",
+                "center_lines",
+            ]:
                 metadata = self.viewer.layers[selected_layer].metadata.copy()
 
                 label_modality = self.label_modality.currentText()
                 label_light_source = self.label_light_source.currentText()
                 label_stain = self.label_stain.currentText()
                 label_stain_target = self.label_stain_target.currentText()
 
@@ -836,63 +1391,99 @@
             colicoords_channel = colicoords_channel.replace("Mask + ", "")
 
             if pixel_size <= 0:
                 pixel_size = 1
 
             desktop = os.path.expanduser("~/Desktop")
 
-            path = QFileDialog.getExistingDirectory(self, "Select Directory", desktop)
+            path = QFileDialog.getExistingDirectory(
+                self, "Select Directory", desktop
+            )
 
             colicoords_dir = os.path.join(tempfile.gettempdir(), "colicoords")
 
             if os.path.isdir(colicoords_dir) != True:
                 os.mkdir(colicoords_dir)
             else:
                 shutil.rmtree(colicoords_dir)
                 os.mkdir(colicoords_dir)
 
             if os.path.isdir(path):
                 path = os.path.abspath(path)
 
-                from napari_bacseg._utils_statistics import (get_cell_statistics, process_cell_statistics, )
+                from napari_bacseg._utils_statistics import (
+                    get_cell_statistics,
+                    process_cell_statistics,
+                )
 
                 self.get_cell_statistics = self.wrapper(get_cell_statistics)
-                self.process_cell_statistics = self.wrapper(process_cell_statistics)
-
-                worker = Worker(self.get_cell_statistics, mode=mode, pixel_size=pixel_size, colicoords_dir=colicoords_dir, )
-                worker.signals.progress.connect(partial(self._Progresbar, progressbar="export"))
-                worker.signals.result.connect(self.process_cell_statistics(path=path))
+                self.process_cell_statistics = self.wrapper(
+                    process_cell_statistics
+                )
+
+                worker = Worker(
+                    self.get_cell_statistics,
+                    mode=mode,
+                    pixel_size=pixel_size,
+                    colicoords_dir=colicoords_dir,
+                )
+                worker.signals.progress.connect(
+                    partial(self._Progresbar, progressbar="export")
+                )
+                worker.signals.result.connect(
+                    self.process_cell_statistics(path=path)
+                )
                 self.threadpool.start(worker)
                 cell_data = worker.result()
 
                 if self.export_colicoords_mode.currentIndex() != 0:
                     from napari_bacseg._utils_colicoords import run_colicoords
 
                     self.run_colicoords = self.wrapper(run_colicoords)
 
-                    worker = Worker(self.run_colicoords, cell_data=cell_data, colicoords_channel=colicoords_channel, pixel_size=pixel_size, statistics=True, multithreaded=multithreaded, )
-
-                    worker.signals.progress.connect(partial(self._Progresbar, progressbar="export"))
-                    worker.signals.result.connect(self.process_cell_statistics(path=path))
+                    worker = Worker(
+                        self.run_colicoords,
+                        cell_data=cell_data,
+                        colicoords_channel=colicoords_channel,
+                        pixel_size=pixel_size,
+                        statistics=True,
+                        multithreaded=multithreaded,
+                    )
+
+                    worker.signals.progress.connect(
+                        partial(self._Progresbar, progressbar="export")
+                    )
+                    worker.signals.result.connect(
+                        self.process_cell_statistics(path=path)
+                    )
                     self.threadpool.start(worker)
 
         return _event
 
     def update_import_limit(self):
-        if self.import_filemode.currentIndex() == 0:
-            self.import_limit.setEnabled(False)
-            self.import_limit.setCurrentIndex(6)
-            self.import_limit.hide()
-            self.import_limit_label.hide()
-        else:
+        if (
+            self.import_filemode.currentIndex() == 1
+            or self.import_mode.currentText() == "Zeiss (.czi) Data"
+        ):
             self.import_limit.setEnabled(True)
             self.import_limit.setCurrentIndex(0)
             self.import_limit.show()
             self.import_limit_label.show()
 
+            if self.import_mode.currentText() == "Zeiss (.czi) Data":
+                self.import_limit_label.setText("Import Limit (FOV)")
+            else:
+                self.import_limit_label.setText("Import Limit (Files)")
+
+        else:
+            self.import_limit.setEnabled(False)
+            self.import_limit.setCurrentIndex(6)
+            self.import_limit.hide()
+            self.import_limit_label.hide()
+
     def _sort_cells(self, order):
         def _event(viewer):
             if self.unfolded == True:
                 self.fold_images()
 
             try:
                 current_fov = self.viewer.dims.current_step[0]
@@ -911,34 +1502,49 @@
                     criterion = meta["simple_cell_stats"]["cell_area"]
                 if find_criterion == "Cell Solidity":
                     criterion = meta["simple_cell_stats"]["cell_solidity"]
                 if find_criterion == "Cell Aspect Ratio":
                     criterion = meta["simple_cell_stats"]["cell_aspect_ratio"]
 
                 if find_mode == "Ascending":
-                    criterion, cell_centre, cell_zoom = zip(*sorted(zip(criterion, cell_centre, cell_zoom), key=lambda x: x[0], ))
+                    criterion, cell_centre, cell_zoom = zip(
+                        *sorted(
+                            zip(criterion, cell_centre, cell_zoom),
+                            key=lambda x: x[0],
+                        )
+                    )
                 else:
-                    criterion, cell_centre, cell_zoom = zip(*sorted(zip(criterion, cell_centre, cell_zoom), key=lambda x: x[0], reverse=True, ))
-
-                current_position = tuple(np.array(self.viewer.camera.center).round())
+                    criterion, cell_centre, cell_zoom = zip(
+                        *sorted(
+                            zip(criterion, cell_centre, cell_zoom),
+                            key=lambda x: x[0],
+                            reverse=True,
+                        )
+                    )
+
+                current_position = tuple(
+                    np.array(self.viewer.camera.center).round()
+                )
 
                 if current_position not in cell_centre:
                     self.viewer.camera.center = cell_centre[0]
                     self.viewer.camera.zoom = cell_zoom[0]
 
                 else:
                     current_index = cell_centre.index(current_position)
 
                     if order == "next":
                         new_index = current_index + 1
 
                     if order == "previous":
                         new_index = current_index - 1
 
-                    new_index = max(current_fov, min(new_index, len(cell_centre) - 1))
+                    new_index = max(
+                        current_fov, min(new_index, len(cell_centre) - 1)
+                    )
 
                     self.viewer.camera.center = cell_centre[new_index]
                     self.viewer.camera.zoom = cell_zoom[new_index]
 
             except:
                 pass
 
@@ -963,15 +1569,19 @@
             elif key == "right":
                 shift_vector = [0.0, 1.0]
             else:
                 shift_vector = [0.0, 0.0]
 
             shift_image = False
             if active_layer != None:
-                if active_layer.name not in ["Segmentations", "Classes", "center_lines", ]:
+                if active_layer.name not in [
+                    "Segmentations",
+                    "Classes",
+                    "center_lines",
+                ]:
                     shift_image = True
 
             if shift_image is True:
                 if mode == "active":
                     image_stack = active_layer.data.copy()
                     image = image_stack[current_fov, :, :]
                     image = shift(image, shift=shift_vector)
@@ -1019,90 +1629,146 @@
 
         channel = self.refine_channel.currentText()
         colicoords_channel = channel.replace("Mask + ", "")
 
         mask_stack = self.segLayer.data
         mask = mask_stack[current_fov, :, :].copy()
 
-        from napari_bacseg._utils_colicoords import (process_colicoords, run_colicoords, )
+        from napari_bacseg._utils_colicoords import (
+            process_colicoords,
+            run_colicoords,
+        )
         from napari_bacseg._utils_statistics import get_cell_statistics
 
         self.get_cell_statistics = self.wrapper(get_cell_statistics)
         self.run_colicoords = self.wrapper(run_colicoords)
         self.process_colicoords = self.wrapper(process_colicoords)
 
         colicoords_dir = os.path.join(tempfile.gettempdir(), "colicoords")
 
-        worker = Worker(self.get_cell_statistics, mode="active", pixel_size=pixel_size, colicoords_dir=colicoords_dir, )
+        worker = Worker(
+            self.get_cell_statistics,
+            mode="active",
+            pixel_size=pixel_size,
+            colicoords_dir=colicoords_dir,
+        )
 
         self.threadpool.start(worker)
         cell_data = worker.result()
 
-        worker = Worker(self.run_colicoords, cell_data=cell_data, colicoords_channel=colicoords_channel, pixel_size=pixel_size, multithreaded=True, )
-
-        worker.signals.progress.connect(partial(self._Progresbar, progressbar="modify"))
+        worker = Worker(
+            self.run_colicoords,
+            cell_data=cell_data,
+            colicoords_channel=colicoords_channel,
+            pixel_size=pixel_size,
+            multithreaded=True,
+        )
+
+        worker.signals.progress.connect(
+            partial(self._Progresbar, progressbar="modify")
+        )
         worker.signals.result.connect(self.process_colicoords)
         self.threadpool.start(worker)
 
     def _uploadDatabase(self, viewer=None, mode=""):
         def _event(viewer):
             try:
-                if (self.database_path != "" and os.path.exists(self.database_path) == True):
+                if (
+                    self.database_path != ""
+                    and os.path.exists(self.database_path) == True
+                ):
                     if self.unfolded == True:
                         self.fold_images()
 
-                    if self.upload_initial.currentText() in ["", "Required for upload", ]:
+                    if self.upload_initial.currentText() in [
+                        "",
+                        "Required for upload",
+                    ]:
                         show_info("Please select the user initial.")
                     else:
-                        from napari_bacseg._utils_database_IO import (_upload_bacseg_database, )
-
-                        self._upload_bacseg_database = self.wrapper(_upload_bacseg_database)
-
-                        worker = Worker(self._upload_bacseg_database, mode=mode)
-                        worker.signals.progress.connect(partial(self._Progresbar, progressbar="database"))
+                        from napari_bacseg._utils_database_IO import (
+                            _upload_bacseg_database,
+                        )
+
+                        self._upload_bacseg_database = self.wrapper(
+                            _upload_bacseg_database
+                        )
+
+                        worker = Worker(
+                            self._upload_bacseg_database, mode=mode
+                        )
+                        worker.signals.progress.connect(
+                            partial(self._Progresbar, progressbar="database")
+                        )
                         self.threadpool.start(worker)
             except:
                 pass
 
         return _event
 
     def _downloadDatabase(self, viewer=None):
         try:
-            if (self.database_path != "" and os.path.exists(self.database_path) == True):
+            if (
+                self.database_path != ""
+                and os.path.exists(self.database_path) == True
+            ):
                 if self.unfolded == True:
                     self.fold_images()
 
-                if self.upload_initial.currentText() in ["", "Required for upload", ]:
+                if self.upload_initial.currentText() in [
+                    "",
+                    "Required for upload",
+                ]:
                     show_info("Please select the user initial.")
 
                 else:
-                    from napari_bacseg._utils_database_IO import (get_filtered_database_metadata, read_bacseg_images, )
-
-                    self.get_filtered_database_metadata = self.wrapper(get_filtered_database_metadata)
+                    from napari_bacseg._utils_database_IO import (
+                        get_filtered_database_metadata,
+                        read_bacseg_images,
+                    )
+
+                    self.get_filtered_database_metadata = self.wrapper(
+                        get_filtered_database_metadata
+                    )
                     self.read_bacseg_images = self.wrapper(read_bacseg_images)
 
                     self.active_import_mode = "BacSeg"
 
-                    (measurements, file_paths, channels,) = self.get_filtered_database_metadata()
+                    (
+                        measurements,
+                        file_paths,
+                        channels,
+                    ) = self.get_filtered_database_metadata()
 
                     if len(file_paths) == 0:
                         if self.widget_notifications:
                             show_info("no matching database files found")
 
                     else:
-                        worker = Worker(self.read_bacseg_images, measurements=measurements, channels=channels, )
+                        worker = Worker(
+                            self.read_bacseg_images,
+                            measurements=measurements,
+                            channels=channels,
+                        )
                         worker.signals.result.connect(self._process_import)
-                        worker.signals.progress.connect(partial(self._Progresbar, progressbar="database"))
+                        worker.signals.progress.connect(
+                            partial(self._Progresbar, progressbar="database")
+                        )
                         self.threadpool.start(worker)
 
         except:
             print(traceback.format_exc())
 
     def _updateSegChannels(self):
-        layer_names = [layer.name for layer in self.viewer.layers if layer.name not in ["Segmentations", "Nucleoid", "Classes", "center_lines"]]
+        layer_names = [
+            layer.name
+            for layer in self.viewer.layers
+            if layer.name
+            not in ["Segmentations", "Nucleoid", "Classes", "center_lines"]
+        ]
 
         segChannel = self.cellpose_segchannel.currentText()
 
         self.export_channel.setCurrentText(segChannel)
 
     def _Progresbar(self, progress, progressbar):
         if progressbar == "import":
@@ -1137,199 +1803,311 @@
             file_extension = "*.tif *.png *.jpeg *.fits"
         if import_mode == "Cellpose (.npy) Segmentation(s)":
             file_extension = "*.npy"
         if import_mode == "Oufti (.mat) Segmentation(s)":
             file_extension = "*.mat"
         if import_mode == "JSON (.txt) Segmentation(s)":
             file_extension = "*.txt"
+        if import_mode == "Zeiss (.czi) Data":
+            file_extension = "*.czi"
 
         desktop = os.path.expanduser("~/Desktop")
 
         if type(paths) is not list:
             if import_filemode == "Import File(s)":
-                paths, _ = QFileDialog.getOpenFileNames(self, "Open Files", desktop, f"Files ({file_extension})")
+                paths, _ = QFileDialog.getOpenFileNames(
+                    self, "Open Files", desktop, f"Files ({file_extension})"
+                )
 
             if import_filemode == "Import Directory":
-                path = QFileDialog.getExistingDirectory(self, "Select Directory", desktop)
+                path = QFileDialog.getExistingDirectory(
+                    self, "Select Directory", desktop
+                )
 
                 paths = [path]
 
         if "" in paths or paths == [] or type(paths) is not list:
             if self.widget_notifications:
                 show_info("No file/folder selected")
 
         else:
             if import_mode == "Images":
-                self.import_images = self.wrapper(napari_bacseg._utils.import_images)
+                self.import_images = self.wrapper(
+                    napari_bacseg._utils.import_images
+                )
 
                 worker = Worker(self.import_images, file_paths=paths)
                 worker.signals.result.connect(self._process_import)
-                worker.signals.progress.connect(partial(self._Progresbar, progressbar="import"))
+                worker.signals.progress.connect(
+                    partial(self._Progresbar, progressbar="import")
+                )
                 self.threadpool.start(worker)
 
             if import_mode == "NanoImager Data":
-                self.read_nim_directory = self.wrapper(napari_bacseg._utils.read_nim_directory)
-                self.read_nim_images = self.wrapper(napari_bacseg._utils.read_nim_images)
-
-                measurements, file_paths, channels = self.read_nim_directory(paths)
-
-                worker = Worker(self.read_nim_images, measurements=measurements, channels=channels, )
+                self.read_nim_directory = self.wrapper(
+                    napari_bacseg._utils.read_nim_directory
+                )
+                self.read_nim_images = self.wrapper(
+                    napari_bacseg._utils.read_nim_images
+                )
+
+                measurements, file_paths, channels = self.read_nim_directory(
+                    paths
+                )
+
+                worker = Worker(
+                    self.read_nim_images,
+                    measurements=measurements,
+                    channels=channels,
+                )
                 worker.signals.result.connect(self._process_import)
-                worker.signals.progress.connect(partial(self._Progresbar, progressbar="import"))
+                worker.signals.progress.connect(
+                    partial(self._Progresbar, progressbar="import")
+                )
                 self.threadpool.start(worker)
 
             if import_mode == "Mask (.tif) Segmentation(s)":
-                self.import_masks = self.wrapper(napari_bacseg._utils.import_masks)
+                self.import_masks = self.wrapper(
+                    napari_bacseg._utils.import_masks
+                )
                 self.import_masks(paths, file_extension=".tif")
                 self._autoClassify()
 
             if import_mode == "Cellpose (.npy) Segmentation(s)":
-                self.import_masks = self.wrapper(napari_bacseg._utils.import_masks)
+                self.import_masks = self.wrapper(
+                    napari_bacseg._utils.import_masks
+                )
                 self.import_masks(paths, file_extension=".npy")
                 self._autoClassify()
 
             if import_mode == "Oufti (.mat) Segmentation(s)":
-                self.import_masks = self.wrapper(napari_bacseg._utils.import_masks)
+                self.import_masks = self.wrapper(
+                    napari_bacseg._utils.import_masks
+                )
                 self.import_masks(paths, file_extension=".mat")
                 self._autoClassify()
 
             if import_mode == "JSON (.txt) Segmentation(s)":
-                self.import_masks = self.wrapper(napari_bacseg._utils.import_masks)
+                self.import_masks = self.wrapper(
+                    napari_bacseg._utils.import_masks
+                )
                 self.import_masks(paths, file_extension=".txt")
                 self._autoClassify()
 
             if import_mode == "ImageJ files(s)":
-                self.import_imagej = self.wrapper(napari_bacseg._utils.import_imagej)
+                self.import_imagej = self.wrapper(
+                    napari_bacseg._utils.import_imagej
+                )
 
                 worker = Worker(self.import_imagej, paths=paths)
                 worker.signals.result.connect(self._process_import)
-                worker.signals.progress.connect(partial(self._Progresbar, progressbar="import"))
+                worker.signals.progress.connect(
+                    partial(self._Progresbar, progressbar="import")
+                )
                 self.threadpool.start(worker)
 
             if import_mode == "ScanR Data":
-                from napari_bacseg._utils import (read_scanr_directory, read_scanr_images, )
+                from napari_bacseg._utils import (
+                    read_scanr_directory,
+                    read_scanr_images,
+                )
 
                 self.read_scanr_images = self.wrapper(read_scanr_images)
 
-                measurements, file_paths, channels = read_scanr_directory(self, paths)
-
-                worker = Worker(self.read_scanr_images, measurements=measurements, channels=channels, )
+                measurements, file_paths, channels = read_scanr_directory(
+                    self, paths
+                )
+
+                worker = Worker(
+                    self.read_scanr_images,
+                    measurements=measurements,
+                    channels=channels,
+                )
                 worker.signals.result.connect(self._process_import)
-                worker.signals.progress.connect(partial(self._Progresbar, progressbar="import"))
+                worker.signals.progress.connect(
+                    partial(self._Progresbar, progressbar="import")
+                )
                 self.threadpool.start(worker)
 
+            if import_mode == "Zeiss (.czi) Data":
+                try:
+                    from napari_bacseg._utils_zeiss import (
+                        get_zeiss_measurements,
+                        read_zeiss_image_files,
+                    )
+
+                    self.get_zeiss_measurements = self.wrapper(
+                        get_zeiss_measurements
+                    )
+                    self.read_zeiss_image_files = self.wrapper(
+                        read_zeiss_image_files
+                    )
+
+                    (
+                        zeiss_measurements,
+                        channel_names,
+                        num_measurements,
+                    ) = get_zeiss_measurements(self, paths)
+
+                    worker = Worker(
+                        self.read_zeiss_image_files,
+                        zeiss_measurements=zeiss_measurements,
+                        channel_names=channel_names,
+                        num_measurements=num_measurements,
+                    )
+                    worker.signals.result.connect(self._process_import)
+                    worker.signals.progress.connect(
+                        partial(self._Progresbar, progressbar="import")
+                    )
+                    self.threadpool.start(worker)
+
+                except:
+                    print(traceback.format_exc())
+
     def _export_stack(self, mode, viewer=None):
         def _event(viewer):
             execute_export = True
 
             if self.export_location.currentIndex() == 1:
                 desktop = os.path.expanduser("~/Desktop")
-                self.export_directory = QFileDialog.getExistingDirectory(self, "Select Directory", desktop)
+                self.export_directory = QFileDialog.getExistingDirectory(
+                    self, "Select Directory", desktop
+                )
 
                 if self.export_directory == "":
                     execute_export = False
 
             if execute_export == True:
-                self.export_stacks = self.wrapper(napari_bacseg._utils.export_stacks)
+                self.export_stacks = self.wrapper(
+                    napari_bacseg._utils.export_stacks
+                )
 
                 worker = Worker(self.export_stacks, mode=mode)
-                worker.signals.progress.connect(partial(self._Progresbar, progressbar="export"))
+                worker.signals.progress.connect(
+                    partial(self._Progresbar, progressbar="export")
+                )
                 self.threadpool.start(worker)
 
         return _event
 
     def _export(self, mode, viewer=None):
         def _event(viewer):
             # if self.unfolded == True:
             #     self.fold_images()
 
             execute_export = True
 
             if self.export_location.currentIndex() == 1:
                 desktop = os.path.expanduser("~/Desktop")
-                self.export_directory = QFileDialog.getExistingDirectory(self, "Select Directory", desktop)
+                self.export_directory = QFileDialog.getExistingDirectory(
+                    self, "Select Directory", desktop
+                )
 
                 if self.export_directory == "":
                     execute_export = False
 
             if execute_export == True:
-                self.export_files = self.wrapper(napari_bacseg._utils.export_files)
+                self.export_files = self.wrapper(
+                    napari_bacseg._utils.export_files
+                )
 
                 worker = Worker(self.export_files, mode=mode)
-                worker.signals.progress.connect(partial(self._Progresbar, progressbar="export"))
+                worker.signals.progress.connect(
+                    partial(self._Progresbar, progressbar="export")
+                )
                 self.threadpool.start(worker)
 
         return _event
 
     def _trainCellpose(self):
         if self.unfolded == True:
             self.fold_images()
 
         from napari_bacseg._utils_cellpose import train_cellpose_model
 
         self.train_cellpose_model = self.wrapper(train_cellpose_model)
 
         worker = Worker(self.train_cellpose_model)
-        worker.signals.progress.connect(partial(self._Progresbar, progressbar="cellpose_train"))
+        worker.signals.progress.connect(
+            partial(self._Progresbar, progressbar="cellpose_train")
+        )
         self.threadpool.start(worker)
 
     def _segmentActive(self):
         if self.unfolded == True:
             self.fold_images()
 
-        from napari_bacseg._utils_cellpose import (_process_cellpose, _run_cellpose, )
+        from napari_bacseg._utils_cellpose import (
+            _process_cellpose,
+            _run_cellpose,
+        )
 
         self._run_cellpose = self.wrapper(_run_cellpose)
         self._process_cellpose = self.wrapper(_process_cellpose)
 
         current_fov = self.viewer.dims.current_step[0]
         chanel = self.cellpose_segchannel.currentText()
 
         images = self.viewer.layers[chanel].data
 
         image = [images[current_fov, :, :]]
 
         worker = Worker(self._run_cellpose, images=image)
         worker.signals.result.connect(self._process_cellpose)
-        worker.signals.progress.connect(partial(self._Progresbar, progressbar="cellpose"))
+        worker.signals.progress.connect(
+            partial(self._Progresbar, progressbar="cellpose")
+        )
         self.threadpool.start(worker)
 
     def _segmentAll(self):
         if self.unfolded == True:
             self.fold_images()
 
-        from napari_bacseg._utils_cellpose import (_process_cellpose, _run_cellpose, )
+        from napari_bacseg._utils_cellpose import (
+            _process_cellpose,
+            _run_cellpose,
+        )
 
         self._run_cellpose = self.wrapper(_run_cellpose)
         self._process_cellpose = self.wrapper(_process_cellpose)
 
         channel = self.cellpose_segchannel.currentText()
 
         images = self.viewer.layers[channel].data
 
         images = unstack_images(images)
 
         worker = Worker(self._run_cellpose, images=images)
         worker.signals.result.connect(self._process_cellpose)
-        worker.signals.progress.connect(partial(self._Progresbar, progressbar="cellpose"))
+        worker.signals.progress.connect(
+            partial(self._Progresbar, progressbar="cellpose")
+        )
         self.threadpool.start(worker)
 
     def _updateSliderLabel(self, slider_name, label_name):
         self.slider = self.findChild(QSlider, slider_name)
         self.label = self.findChild(QLabel, label_name)
 
         slider_value = self.slider.value()
 
-        if (slider_name == "cellpose_flowthresh" or slider_name == "cellpose_maskthresh"):
+        if (
+            slider_name == "cellpose_flowthresh"
+            or slider_name == "cellpose_maskthresh"
+        ):
             self.label.setText(str(slider_value / 100))
         else:
             self.label.setText(str(slider_value))
 
     def _updateSegmentationCombo(self):
-        layer_names = [layer.name for layer in self.viewer.layers if layer.name not in ["Segmentations", "Nucleoid", "Classes", "center_lines"]]
+        layer_names = [
+            layer.name
+            for layer in self.viewer.layers
+            if layer.name
+            not in ["Segmentations", "Nucleoid", "Classes", "center_lines"]
+        ]
 
         self.cellpose_segchannel.clear()
         self.cellpose_segchannel.addItems(layer_names)
 
         self.cellpose_trainchannel.clear()
         self.cellpose_trainchannel.addItems(layer_names)
 
@@ -1340,24 +2118,28 @@
         self.alignment_channel.addItems(layer_names)
 
         self.export_stack_channel.clear()
         self.export_stack_channel.addItems(layer_names)
 
         self.export_channel.clear()
         export_layers = layer_names
-        export_layers.extend(["All Channels (Stack)", "First Three Channels (RGB)"])
+        export_layers.extend(
+            ["All Channels (Stack)", "First Three Channels (RGB)"]
+        )
         self.export_channel.addItems(export_layers)
 
         self.refine_channel.clear()
         refine_layers = ["Mask + " + layer for layer in layer_names]
         self.refine_channel.addItems(["Mask"] + refine_layers)
 
         self.export_colicoords_mode.clear()
         refine_layers = ["Mask + " + layer for layer in layer_names]
-        self.export_colicoords_mode.addItems(["None (OpenCV Stats)", "Mask"] + refine_layers)
+        self.export_colicoords_mode.addItems(
+            ["None (OpenCV Stats)", "Mask"] + refine_layers
+        )
 
     def _sliderEvent(self, current_step):
         try:
             active_layer = self.viewer.layers.selection.active
 
             crop = active_layer.corner_pixels.T
 
@@ -1377,93 +2159,176 @@
         try:
             if self.scalebar_show.isChecked() and len(layer_names) > 0:
                 pixel_resolution = float(self.scalebar_resolution.text())
                 scalebar_units = self.scalebar_units.currentText()
 
                 if pixel_resolution > 0:
                     for layer in layer_names:
-                        self.viewer.layers[layer].scale = [1, pixel_resolution, pixel_resolution, ]
+                        self.viewer.layers[layer].scale = [
+                            1,
+                            pixel_resolution,
+                            pixel_resolution,
+                        ]
 
                         self.viewer.scale_bar.visible = True
                         self.viewer.scale_bar.unit = scalebar_units
                         self.viewer.reset_view()
 
             else:
                 self.viewer.scale_bar.visible = False
 
         except:
             self.viewer.scale_bar.visible = False
 
     def _autoContrast(self):
         try:
             if self.autocontrast.isChecked():
-                layer_names = [layer.name for layer in self.viewer.layers if layer.name not in ["Segmentations", "Nucleoid", "Classes", "center_lines", ]]
+                layer_names = [
+                    layer.name
+                    for layer in self.viewer.layers
+                    if layer.name
+                    not in [
+                        "Segmentations",
+                        "Nucleoid",
+                        "Classes",
+                        "center_lines",
+                    ]
+                ]
 
                 if len(layer_names) != 0:
                     active_layer = layer_names[-1]
 
-                    image_dims = tuple(list(self.viewer.dims.current_step[:-2]) + [...])
-
-                    image = (self.viewer.layers[str(active_layer)].data[image_dims].copy())
-
-                    crop = self.viewer.layers[str(active_layer)].corner_pixels[:, -2:]
+                    image_dims = tuple(
+                        list(self.viewer.dims.current_step[:-2]) + [...]
+                    )
+
+                    image = (
+                        self.viewer.layers[str(active_layer)]
+                        .data[image_dims]
+                        .copy()
+                    )
+
+                    crop = self.viewer.layers[str(active_layer)].corner_pixels[
+                        :, -2:
+                    ]
 
                     [[y1, x1], [y2, x2]] = crop
 
                     image_crop = image[y1:y2, x1:x2]
 
-                    contrast_limit = np.percentile(image_crop[image_crop != 0], (1, 99))
-                    contrast_limit = [int(contrast_limit[0] * 0.5), int(contrast_limit[1] * 2), ]
+                    contrast_limit = np.percentile(
+                        image_crop[image_crop != 0], (1, 99)
+                    )
+                    contrast_limit = [
+                        int(contrast_limit[0] * 0.5),
+                        int(contrast_limit[1] * 2),
+                    ]
 
                     if contrast_limit[1] > contrast_limit[0]:
-                        self.viewer.layers[str(active_layer)].contrast_limits = contrast_limit
+                        self.viewer.layers[
+                            str(active_layer)
+                        ].contrast_limits = contrast_limit
 
         except:
             pass
 
     def _updateFileName(self):
         try:
             current_fov = self.viewer.dims.current_step[0]
             active_layer = self.viewer.layers.selection.active
 
             image = self.viewer.layers[str(active_layer)].data[current_fov]
-            metadata = self.viewer.layers[str(active_layer)].metadata[current_fov]
+            metadata = self.viewer.layers[str(active_layer)].metadata[
+                current_fov
+            ]
 
             viewer_text = ""
 
             # print(metadata['image_name'])
 
-            if (self.overlay_filename.isChecked() and "image_name" in metadata.keys()):
+            if (
+                self.overlay_filename.isChecked()
+                and "image_name" in metadata.keys()
+            ):
                 viewer_text = f"File Name: {metadata['image_name']}"
             if self.overlay_folder.isChecked() and "folder" in metadata.keys():
                 viewer_text = viewer_text + f"\nFolder: {metadata['folder']}"
-            if (self.overlay_microscope.isChecked() and "microscope" in metadata.keys()):
-                viewer_text = (viewer_text + f"\nMicroscope: {metadata['microscope']}")
-            if (self.overlay_datemodified.isChecked() and "date_modified" in metadata.keys()):
-                viewer_text = (viewer_text + f"\nDate Modified: {metadata['date_modified']}")
-            if (self.overlay_content.isChecked() and "content" in metadata.keys()):
+            if (
+                self.overlay_microscope.isChecked()
+                and "microscope" in metadata.keys()
+            ):
+                viewer_text = (
+                    viewer_text + f"\nMicroscope: {metadata['microscope']}"
+                )
+            if (
+                self.overlay_datemodified.isChecked()
+                and "date_modified" in metadata.keys()
+            ):
+                viewer_text = (
+                    viewer_text
+                    + f"\nDate Modified: {metadata['date_modified']}"
+                )
+            if (
+                self.overlay_content.isChecked()
+                and "content" in metadata.keys()
+            ):
                 viewer_text = viewer_text + f"\nContent: {metadata['content']}"
             if self.overlay_strain.isChecked() and "strain" in metadata.keys():
                 viewer_text = viewer_text + f"\nStrain: {metadata['strain']}"
-            if (self.overlay_phenotype.isChecked() and "phenotype" in metadata.keys()):
-                viewer_text = (viewer_text + f"\nPhenotype: {metadata['phenotype']}")
-            if (self.overlay_antibiotic.isChecked() and "antibiotic" in metadata.keys()):
-                viewer_text = (viewer_text + f"\nAntibiotic: {metadata['antibiotic']}")
+            if (
+                self.overlay_phenotype.isChecked()
+                and "phenotype" in metadata.keys()
+            ):
+                viewer_text = (
+                    viewer_text + f"\nPhenotype: {metadata['phenotype']}"
+                )
+            if (
+                self.overlay_antibiotic.isChecked()
+                and "antibiotic" in metadata.keys()
+            ):
+                viewer_text = (
+                    viewer_text + f"\nAntibiotic: {metadata['antibiotic']}"
+                )
             if self.overlay_stain.isChecked() and "stain" in metadata.keys():
                 viewer_text = viewer_text + f"\nStain: {metadata['stain']}"
-            if (self.overlay_staintarget.isChecked() and "stain_target" in metadata.keys()):
-                viewer_text = (viewer_text + f"\nStain Target: {metadata['stain_target']}")
-            if (self.overlay_modality.isChecked() and "modality" in metadata.keys()):
-                viewer_text = (viewer_text + f"\nModality: {metadata['modality']}")
-            if (self.overlay_lightsource.isChecked() and "source" in metadata.keys()):
-                viewer_text = (viewer_text + f"\nLight Source: {metadata['source']}")
-            if (self.overlay_focus.isChecked() and "image_focus" in metadata.keys()):
-                viewer_text = (viewer_text + f"\nImage Focus: {metadata['image_focus']}")
-            if (self.overlay_debris.isChecked() and "image_debris" in metadata.keys()):
-                viewer_text = (viewer_text + f"\nImage Debris: {metadata['image_debris']}")
+            if (
+                self.overlay_staintarget.isChecked()
+                and "stain_target" in metadata.keys()
+            ):
+                viewer_text = (
+                    viewer_text + f"\nStain Target: {metadata['stain_target']}"
+                )
+            if (
+                self.overlay_modality.isChecked()
+                and "modality" in metadata.keys()
+            ):
+                viewer_text = (
+                    viewer_text + f"\nModality: {metadata['modality']}"
+                )
+            if (
+                self.overlay_lightsource.isChecked()
+                and "source" in metadata.keys()
+            ):
+                viewer_text = (
+                    viewer_text + f"\nLight Source: {metadata['source']}"
+                )
+            if (
+                self.overlay_focus.isChecked()
+                and "image_focus" in metadata.keys()
+            ):
+                viewer_text = (
+                    viewer_text + f"\nImage Focus: {metadata['image_focus']}"
+                )
+            if (
+                self.overlay_debris.isChecked()
+                and "image_debris" in metadata.keys()
+            ):
+                viewer_text = (
+                    viewer_text + f"\nImage Debris: {metadata['image_debris']}"
+                )
             if self.overlay_laplacian.isChecked():
                 image_laplacian = np.mean(cv2.Laplacian(image, cv2.CV_64F))
                 viewer_text = viewer_text + f"\nLaplacian: {image_laplacian}"
             if self.overlay_range.isChecked():
                 image_range = np.max(image) - np.min(image)
                 viewer_text = viewer_text + f"\nRange: {image_range}"
 
@@ -1473,15 +2338,20 @@
             else:
                 self.viewer.text_overlay.visible = False
 
         except:
             pass
 
     def _process_import(self, imported_data, rearrange=True):
-        layer_names = [layer.name for layer in self.viewer.layers if layer.name not in ["Segmentations", "Nucleoid", "Classes", "center_lines"]]
+        layer_names = [
+            layer.name
+            for layer in self.viewer.layers
+            if layer.name
+            not in ["Segmentations", "Nucleoid", "Classes", "center_lines"]
+        ]
 
         append_mode = self.import_append_mode.currentIndex()
 
         if append_mode == 0:
             # removes all layers (except segmentation layer)
             for layer_name in layer_names:
                 self.viewer.layers.remove(self.viewer.layers[layer_name])
@@ -1491,15 +2361,14 @@
             self.classLayer.data = np.zeros((1, 100, 100), dtype=np.uint16)
 
         imported_images = imported_data["imported_images"]
 
         self.viewer.dims.set_current_step(0, 0)
 
         for layer_name, layer_data in imported_images.items():
-
             images = layer_data["images"]
             masks = layer_data["masks"]
             classes = layer_data["classes"]
             metadata = layer_data["metadata"]
 
             # for i in range(len(images)):
             #     print(metadata[i]["image_name"])
@@ -1513,96 +2382,179 @@
 
             new_image_stack, new_metadata = stack_images(images, metadata)
             new_mask_stack, new_metadata = stack_images(masks, metadata)
             new_nmask_stack, new_metadata = stack_images(nmasks, metadata)
             new_class_stack, new_metadata = stack_images(classes, metadata)
 
             if len(new_mask_stack) == 0:
-                new_mask_stack = np.zeros(new_image_stack.shape, dtype=np.uint16)
+                new_mask_stack = np.zeros(
+                    new_image_stack.shape, dtype=np.uint16
+                )
 
             if len(new_nmask_stack) == 0:
-                new_nmask_stack = np.zeros(new_image_stack.shape, dtype=np.uint16)
+                new_nmask_stack = np.zeros(
+                    new_image_stack.shape, dtype=np.uint16
+                )
 
             if len(new_class_stack) == 0:
-                new_class_stack = np.zeros(new_image_stack.shape, dtype=np.uint16)
+                new_class_stack = np.zeros(
+                    new_image_stack.shape, dtype=np.uint16
+                )
 
             colormap = "gray"
 
             if layer_name == "405":
                 colormap = "green"
             if layer_name == "532":
                 colormap = "red"
             if layer_name == "Cy3":
                 colormap = "red"
             if layer_name == "DAPI":
                 colormap = "green"
 
-            if (append_mode == 1 and layer_name in layer_names):
-
+            if append_mode == 1 and layer_name in layer_names:
                 current_image_stack = self.viewer.layers[layer_name].data
                 current_metadata = self.viewer.layers[layer_name].metadata
                 current_mask_stack = self.segLayer.data
                 current_nmask_stack = self.nucLayer.data
                 current_class_stack = self.classLayer.data
 
                 if len(current_image_stack) == 0:
-                    setattr(self, layer_name, self.viewer.add_image(new_image_stack, name=layer_name, colormap=colormap, gamma=0.8, metadata=new_metadata, ), )
+                    setattr(
+                        self,
+                        layer_name,
+                        self.viewer.add_image(
+                            new_image_stack,
+                            name=layer_name,
+                            colormap=colormap,
+                            gamma=0.8,
+                            metadata=new_metadata,
+                        ),
+                    )
 
                     image_layer = getattr(self, layer_name)
-                    image_layer.mouse_drag_callbacks.append(self._segmentationEvents)
-                    image_layer.mouse_double_click_callbacks.append(self._doubeClickEvents)
+                    image_layer.mouse_drag_callbacks.append(
+                        self._segmentationEvents
+                    )
+                    image_layer.mouse_double_click_callbacks.append(
+                        self._doubeClickEvents
+                    )
 
                     self.segLayer.data = new_mask_stack
                     self.nucLayer.data = new_nmask_stack
                     self.classLayer.data = new_class_stack
                     self.segLayer.metadata = new_metadata
 
                 else:
                     from napari_bacseg._utils import append_image_stacks
 
-                    (appended_image_stack, appended_metadata,) = append_image_stacks(current_metadata, new_metadata, current_image_stack, new_image_stack, )
-
-                    (appended_mask_stack, appended_metadata,) = append_image_stacks(current_metadata, new_metadata, current_mask_stack, new_mask_stack, )
-
-                    (appended_nmask_stack, appended_metadata,) = append_image_stacks(current_metadata, new_metadata, current_nmask_stack, new_nmask_stack, )
-
-                    (appended_class_stack, appended_metadata,) = append_image_stacks(current_metadata, new_metadata, current_class_stack, new_class_stack, )
+                    (
+                        appended_image_stack,
+                        appended_metadata,
+                    ) = append_image_stacks(
+                        current_metadata,
+                        new_metadata,
+                        current_image_stack,
+                        new_image_stack,
+                    )
+
+                    (
+                        appended_mask_stack,
+                        appended_metadata,
+                    ) = append_image_stacks(
+                        current_metadata,
+                        new_metadata,
+                        current_mask_stack,
+                        new_mask_stack,
+                    )
+
+                    (
+                        appended_nmask_stack,
+                        appended_metadata,
+                    ) = append_image_stacks(
+                        current_metadata,
+                        new_metadata,
+                        current_nmask_stack,
+                        new_nmask_stack,
+                    )
+
+                    (
+                        appended_class_stack,
+                        appended_metadata,
+                    ) = append_image_stacks(
+                        current_metadata,
+                        new_metadata,
+                        current_class_stack,
+                        new_class_stack,
+                    )
 
                     self.viewer.layers.remove(self.viewer.layers[layer_name])
 
-                    setattr(self, layer_name, self.viewer.add_image(appended_image_stack, name=layer_name, colormap=colormap, gamma=0.8, metadata=appended_metadata, ), )
+                    setattr(
+                        self,
+                        layer_name,
+                        self.viewer.add_image(
+                            appended_image_stack,
+                            name=layer_name,
+                            colormap=colormap,
+                            gamma=0.8,
+                            metadata=appended_metadata,
+                        ),
+                    )
 
                     image_layer = getattr(self, layer_name)
-                    image_layer.mouse_drag_callbacks.append(self._segmentationEvents)
-                    image_layer.mouse_double_click_callbacks.append(self._doubeClickEvents)
+                    image_layer.mouse_drag_callbacks.append(
+                        self._segmentationEvents
+                    )
+                    image_layer.mouse_double_click_callbacks.append(
+                        self._doubeClickEvents
+                    )
 
                     self.segLayer.data = appended_mask_stack
                     self.nucLayer.data = appended_nmask_stack
                     self.classLayer.data = appended_class_stack
                     self.segLayer.metadata = appended_metadata
 
             else:
-
                 if append_mode == 2:
                     if layer_name in layer_names:
                         import re
-                        channel_indeces = [int(re.findall(r"\[(\d+)\]",layer)[-1]) for layer in layer_names if bool(re.search(r'\[\d+\]', layer)) == True]
+
+                        channel_indeces = [
+                            int(re.findall(r"\[(\d+)\]", layer)[-1])
+                            for layer in layer_names
+                            if bool(re.search(r"\[\d+\]", layer)) == True
+                        ]
 
                         if len(channel_indeces) == 0:
                             new_index = 1
                         else:
                             new_index = max(channel_indeces) + 1
 
                         layer_name = layer_name + f" [{new_index}]"
 
-                setattr(self, layer_name, self.viewer.add_image(new_image_stack, name=layer_name, colormap=colormap, gamma=0.8, metadata=new_metadata, ), )
+                setattr(
+                    self,
+                    layer_name,
+                    self.viewer.add_image(
+                        new_image_stack,
+                        name=layer_name,
+                        colormap=colormap,
+                        gamma=0.8,
+                        metadata=new_metadata,
+                    ),
+                )
 
                 image_layer = getattr(self, layer_name)
-                image_layer.mouse_drag_callbacks.append(self._segmentationEvents)
-                image_layer.mouse_double_click_callbacks.append(self._doubeClickEvents)
+                image_layer.mouse_drag_callbacks.append(
+                    self._segmentationEvents
+                )
+                image_layer.mouse_double_click_callbacks.append(
+                    self._doubeClickEvents
+                )
 
                 self.segLayer.data = new_mask_stack
                 self.nucLayer.data = new_nmask_stack
                 self.classLayer.data = new_class_stack
                 self.segLayer.metadata = new_metadata
 
         # sets labels such that only label contours are shown
@@ -1620,17 +2572,27 @@
         self._autoClassify()
         align_image_channels(self)
         self._autoContrast()
         self._updateScaleBar()
 
     def _reorderLayers(self):
         try:
-            layer_names = [layer.name for layer in self.viewer.layers if layer.name in ["Segmentations", "Nucleoid", "Classes", "center_lines"]]
-
-            for layer in ["center_lines", "Classes", "Nucleoid", "Segmentations", ]:
+            layer_names = [
+                layer.name
+                for layer in self.viewer.layers
+                if layer.name
+                in ["Segmentations", "Nucleoid", "Classes", "center_lines"]
+            ]
+
+            for layer in [
+                "center_lines",
+                "Classes",
+                "Nucleoid",
+                "Segmentations",
+            ]:
                 if layer in layer_names:
                     layer_index = self.viewer.layers.index(layer)
                     self.viewer.layers.move(layer_index, -1)
 
         except:
             pass
 
@@ -1649,21 +2611,30 @@
                 label = np.zeros(label.shape, dtype=np.uint16)
 
                 for mask_id in mask_ids:
                     if mask_id != 0:
                         cnt_mask = np.zeros(label.shape, dtype=np.uint8)
                         cnt_mask[mask == mask_id] = 255
 
-                        cnt, _ = cv2.findContours(cnt_mask.astype(np.uint8), cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_NONE, )
+                        cnt, _ = cv2.findContours(
+                            cnt_mask.astype(np.uint8),
+                            cv2.RETR_EXTERNAL,
+                            cv2.CHAIN_APPROX_NONE,
+                        )
 
                         x, y, w, h = cv2.boundingRect(cnt[0])
                         y1, y2, x1, x2 = y, (y + h), x, (x + w)
 
                         # appends contour to list if the bounding coordinates are along the edge of the image
-                        if (y1 > 0 and y2 < cnt_mask.shape[0] and x1 > 0 and x2 < cnt_mask.shape[1]):
+                        if (
+                            y1 > 0
+                            and y2 < cnt_mask.shape[0]
+                            and x1 > 0
+                            and x2 < cnt_mask.shape[1]
+                        ):
                             label[mask == mask_id] = 1
 
                         else:
                             label[mask == mask_id] = 6
 
             label_stack[i, :, :] = label
```

### Comparing `napari-bacseg-1.0.8/src/napari_bacseg/bacseg_ui.py` & `napari-bacseg-1.0.9/src/napari_bacseg/bacseg_ui.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-# -*- coding: utf-8 -*-
-
 # Form implementation generated from reading ui file 'bacseg_ui.ui'
 #
 # Created by: PyQt5 UI code generator 5.15.9
 #
 # WARNING: Any manual changes made to this file will be lost when pyuic5 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt5 import QtCore, QtGui, QtWidgets
 
 
-class Ui_tab_widget(object):
+class Ui_tab_widget:
     def setupUi(self, tab_widget):
         tab_widget.setObjectName("tab_widget")
         tab_widget.setEnabled(True)
         tab_widget.resize(681, 1133)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        sizePolicy = QtWidgets.QSizePolicy(
+            QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum
+        )
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(100)
-        sizePolicy.setHeightForWidth(tab_widget.sizePolicy().hasHeightForWidth())
+        sizePolicy.setHeightForWidth(
+            tab_widget.sizePolicy().hasHeightForWidth()
+        )
         tab_widget.setSizePolicy(sizePolicy)
         tab_widget.setMinimumSize(QtCore.QSize(200, 0))
         tab_widget.setMaximumSize(QtCore.QSize(1000, 16777215))
         font = QtGui.QFont()
         font.setPointSize(10)
         tab_widget.setFont(font)
         tab_widget.setTabPosition(QtWidgets.QTabWidget.North)
@@ -44,127 +46,192 @@
         font.setBold(True)
         font.setWeight(75)
         self.label_37.setFont(font)
         self.label_37.setObjectName("label_37")
         self.verticalLayout.addWidget(self.label_37)
         self.formLayout_8 = QtWidgets.QFormLayout()
         self.formLayout_8.setObjectName("formLayout_8")
-        spacerItem = QtWidgets.QSpacerItem(334, 5, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
-        self.formLayout_8.setItem(2, QtWidgets.QFormLayout.FieldRole, spacerItem)
+        spacerItem = QtWidgets.QSpacerItem(
+            334,
+            5,
+            QtWidgets.QSizePolicy.Minimum,
+            QtWidgets.QSizePolicy.Minimum,
+        )
+        self.formLayout_8.setItem(
+            2, QtWidgets.QFormLayout.FieldRole, spacerItem
+        )
         self.label_51 = QtWidgets.QLabel(self.import_tab)
         self.label_51.setObjectName("label_51")
-        self.formLayout_8.setWidget(3, QtWidgets.QFormLayout.LabelRole, self.label_51)
+        self.formLayout_8.setWidget(
+            3, QtWidgets.QFormLayout.LabelRole, self.label_51
+        )
         self.import_filemode = QtWidgets.QComboBox(self.import_tab)
         self.import_filemode.setObjectName("import_filemode")
         self.import_filemode.addItem("")
         self.import_filemode.addItem("")
-        self.formLayout_8.setWidget(3, QtWidgets.QFormLayout.FieldRole, self.import_filemode)
+        self.formLayout_8.setWidget(
+            3, QtWidgets.QFormLayout.FieldRole, self.import_filemode
+        )
         self.import_limit_label = QtWidgets.QLabel(self.import_tab)
         self.import_limit_label.setObjectName("import_limit_label")
-        self.formLayout_8.setWidget(4, QtWidgets.QFormLayout.LabelRole, self.import_limit_label)
+        self.formLayout_8.setWidget(
+            4, QtWidgets.QFormLayout.LabelRole, self.import_limit_label
+        )
         self.import_limit = QtWidgets.QComboBox(self.import_tab)
         self.import_limit.setObjectName("import_limit")
         self.import_limit.addItem("")
         self.import_limit.addItem("")
         self.import_limit.addItem("")
         self.import_limit.addItem("")
         self.import_limit.addItem("")
         self.import_limit.addItem("")
         self.import_limit.addItem("")
-        self.formLayout_8.setWidget(4, QtWidgets.QFormLayout.FieldRole, self.import_limit)
-        spacerItem1 = QtWidgets.QSpacerItem(334, 5, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
-        self.formLayout_8.setItem(5, QtWidgets.QFormLayout.FieldRole, spacerItem1)
+        self.formLayout_8.setWidget(
+            4, QtWidgets.QFormLayout.FieldRole, self.import_limit
+        )
+        spacerItem1 = QtWidgets.QSpacerItem(
+            334,
+            5,
+            QtWidgets.QSizePolicy.Minimum,
+            QtWidgets.QSizePolicy.Minimum,
+        )
+        self.formLayout_8.setItem(
+            5, QtWidgets.QFormLayout.FieldRole, spacerItem1
+        )
         self.label_30 = QtWidgets.QLabel(self.import_tab)
         self.label_30.setObjectName("label_30")
-        self.formLayout_8.setWidget(6, QtWidgets.QFormLayout.LabelRole, self.label_30)
+        self.formLayout_8.setWidget(
+            6, QtWidgets.QFormLayout.LabelRole, self.label_30
+        )
         self.import_multiframe_mode = QtWidgets.QComboBox(self.import_tab)
         self.import_multiframe_mode.setObjectName("import_multiframe_mode")
         self.import_multiframe_mode.addItem("")
         self.import_multiframe_mode.addItem("")
         self.import_multiframe_mode.addItem("")
         self.import_multiframe_mode.addItem("")
         self.import_multiframe_mode.addItem("")
-        self.formLayout_8.setWidget(6, QtWidgets.QFormLayout.FieldRole, self.import_multiframe_mode)
+        self.formLayout_8.setWidget(
+            6, QtWidgets.QFormLayout.FieldRole, self.import_multiframe_mode
+        )
         self.label_22 = QtWidgets.QLabel(self.import_tab)
         self.label_22.setObjectName("label_22")
-        self.formLayout_8.setWidget(7, QtWidgets.QFormLayout.LabelRole, self.label_22)
+        self.formLayout_8.setWidget(
+            7, QtWidgets.QFormLayout.LabelRole, self.label_22
+        )
         self.import_crop_mode = QtWidgets.QComboBox(self.import_tab)
         self.import_crop_mode.setObjectName("import_crop_mode")
         self.import_crop_mode.addItem("")
         self.import_crop_mode.addItem("")
         self.import_crop_mode.addItem("")
         self.import_crop_mode.addItem("")
-        self.formLayout_8.setWidget(7, QtWidgets.QFormLayout.FieldRole, self.import_crop_mode)
+        self.formLayout_8.setWidget(
+            7, QtWidgets.QFormLayout.FieldRole, self.import_crop_mode
+        )
         self.label_21 = QtWidgets.QLabel(self.import_tab)
         self.label_21.setObjectName("label_21")
-        self.formLayout_8.setWidget(8, QtWidgets.QFormLayout.LabelRole, self.label_21)
+        self.formLayout_8.setWidget(
+            8, QtWidgets.QFormLayout.LabelRole, self.label_21
+        )
         self.import_precision = QtWidgets.QComboBox(self.import_tab)
         self.import_precision.setObjectName("import_precision")
         self.import_precision.addItem("")
         self.import_precision.addItem("")
         self.import_precision.addItem("")
         self.import_precision.addItem("")
-        self.formLayout_8.setWidget(8, QtWidgets.QFormLayout.FieldRole, self.import_precision)
+        self.formLayout_8.setWidget(
+            8, QtWidgets.QFormLayout.FieldRole, self.import_precision
+        )
         self.import_mode = QtWidgets.QComboBox(self.import_tab)
         self.import_mode.setObjectName("import_mode")
         self.import_mode.addItem("")
         self.import_mode.addItem("")
         self.import_mode.addItem("")
         self.import_mode.addItem("")
         self.import_mode.addItem("")
         self.import_mode.addItem("")
         self.import_mode.addItem("")
         self.import_mode.addItem("")
-        self.formLayout_8.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.import_mode)
+        self.import_mode.addItem("")
+        self.formLayout_8.setWidget(
+            0, QtWidgets.QFormLayout.FieldRole, self.import_mode
+        )
         self.label_27 = QtWidgets.QLabel(self.import_tab)
         self.label_27.setObjectName("label_27")
-        self.formLayout_8.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_27)
-        spacerItem2 = QtWidgets.QSpacerItem(20, 5, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
-        self.formLayout_8.setItem(9, QtWidgets.QFormLayout.FieldRole, spacerItem2)
+        self.formLayout_8.setWidget(
+            0, QtWidgets.QFormLayout.LabelRole, self.label_27
+        )
+        spacerItem2 = QtWidgets.QSpacerItem(
+            20, 5, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum
+        )
+        self.formLayout_8.setItem(
+            9, QtWidgets.QFormLayout.FieldRole, spacerItem2
+        )
         self.label_105 = QtWidgets.QLabel(self.import_tab)
         self.label_105.setObjectName("label_105")
-        self.formLayout_8.setWidget(10, QtWidgets.QFormLayout.LabelRole, self.label_105)
+        self.formLayout_8.setWidget(
+            10, QtWidgets.QFormLayout.LabelRole, self.label_105
+        )
         self.import_append_mode = QtWidgets.QComboBox(self.import_tab)
         self.import_append_mode.setObjectName("import_append_mode")
         self.import_append_mode.addItem("")
         self.import_append_mode.addItem("")
         self.import_append_mode.addItem("")
-        self.formLayout_8.setWidget(10, QtWidgets.QFormLayout.FieldRole, self.import_append_mode)
+        self.formLayout_8.setWidget(
+            10, QtWidgets.QFormLayout.FieldRole, self.import_append_mode
+        )
         self.verticalLayout.addLayout(self.formLayout_8)
-        spacerItem3 = QtWidgets.QSpacerItem(334, 50, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        spacerItem3 = QtWidgets.QSpacerItem(
+            334,
+            50,
+            QtWidgets.QSizePolicy.Minimum,
+            QtWidgets.QSizePolicy.Minimum,
+        )
         self.verticalLayout.addItem(spacerItem3)
         self.import_align = QtWidgets.QCheckBox(self.import_tab)
         self.import_align.setChecked(False)
         self.import_align.setObjectName("import_align")
         self.verticalLayout.addWidget(self.import_align)
         self.import_import = QtWidgets.QPushButton(self.import_tab)
         self.import_import.setObjectName("import_import")
         self.verticalLayout.addWidget(self.import_import)
         self.formLayout_14 = QtWidgets.QFormLayout()
         self.formLayout_14.setObjectName("formLayout_14")
         self.label_36 = QtWidgets.QLabel(self.import_tab)
         self.label_36.setObjectName("label_36")
-        self.formLayout_14.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_36)
+        self.formLayout_14.setWidget(
+            0, QtWidgets.QFormLayout.LabelRole, self.label_36
+        )
         self.import_progressbar = QtWidgets.QProgressBar(self.import_tab)
         self.import_progressbar.setProperty("value", 0)
         self.import_progressbar.setObjectName("import_progressbar")
-        self.formLayout_14.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.import_progressbar)
+        self.formLayout_14.setWidget(
+            0, QtWidgets.QFormLayout.FieldRole, self.import_progressbar
+        )
         self.verticalLayout.addLayout(self.formLayout_14)
-        spacerItem4 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        spacerItem4 = QtWidgets.QSpacerItem(
+            20,
+            40,
+            QtWidgets.QSizePolicy.Minimum,
+            QtWidgets.QSizePolicy.Expanding,
+        )
         self.verticalLayout.addItem(spacerItem4)
         tab_widget.addTab(self.import_tab, "")
         self.tab = QtWidgets.QWidget()
         self.tab.setObjectName("tab")
         self.verticalLayout_5 = QtWidgets.QVBoxLayout(self.tab)
         self.verticalLayout_5.setObjectName("verticalLayout_5")
         self.zoom_ = QtWidgets.QTabWidget(self.tab)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Preferred)
+        sizePolicy = QtWidgets.QSizePolicy(
+            QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Preferred
+        )
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
-        sizePolicy.setHeightForWidth(self.zoom_.sizePolicy().hasHeightForWidth())
+        sizePolicy.setHeightForWidth(
+            self.zoom_.sizePolicy().hasHeightForWidth()
+        )
         self.zoom_.setSizePolicy(sizePolicy)
         self.zoom_.setObjectName("zoom_")
         self.tab_16 = QtWidgets.QWidget()
         self.tab_16.setObjectName("tab_16")
         self.verticalLayout_23 = QtWidgets.QVBoxLayout(self.tab_16)
         self.verticalLayout_23.setObjectName("verticalLayout_23")
         self.label_60 = QtWidgets.QLabel(self.tab_16)
@@ -175,15 +242,20 @@
         self.label_60.setFont(font)
         self.label_60.setObjectName("label_60")
         self.verticalLayout_23.addWidget(self.label_60)
         self.import_auto_contrast = QtWidgets.QCheckBox(self.tab_16)
         self.import_auto_contrast.setChecked(True)
         self.import_auto_contrast.setObjectName("import_auto_contrast")
         self.verticalLayout_23.addWidget(self.import_auto_contrast)
-        spacerItem5 = QtWidgets.QSpacerItem(20, 1, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        spacerItem5 = QtWidgets.QSpacerItem(
+            20,
+            1,
+            QtWidgets.QSizePolicy.Minimum,
+            QtWidgets.QSizePolicy.Expanding,
+        )
         self.verticalLayout_23.addItem(spacerItem5)
         self.line_29 = QtWidgets.QFrame(self.tab_16)
         self.line_29.setFrameShape(QtWidgets.QFrame.HLine)
         self.line_29.setFrameShadow(QtWidgets.QFrame.Sunken)
         self.line_29.setObjectName("line_29")
         self.verticalLayout_23.addWidget(self.line_29)
         self.label_38 = QtWidgets.QLabel(self.tab_16)
@@ -199,15 +271,20 @@
         self.modify_viewlabels = QtWidgets.QCheckBox(self.tab_16)
         self.modify_viewlabels.setObjectName("modify_viewlabels")
         self.gridLayout_6.addWidget(self.modify_viewlabels, 1, 1, 1, 1)
         self.modify_viewmasks = QtWidgets.QCheckBox(self.tab_16)
         self.modify_viewmasks.setObjectName("modify_viewmasks")
         self.gridLayout_6.addWidget(self.modify_viewmasks, 1, 0, 1, 1)
         self.verticalLayout_23.addLayout(self.gridLayout_6)
-        spacerItem6 = QtWidgets.QSpacerItem(20, 1, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        spacerItem6 = QtWidgets.QSpacerItem(
+            20,
+            1,
+            QtWidgets.QSizePolicy.Minimum,
+            QtWidgets.QSizePolicy.Expanding,
+        )
         self.verticalLayout_23.addItem(spacerItem6)
         self.zoom_.addTab(self.tab_16, "")
         self.tab_7 = QtWidgets.QWidget()
         self.tab_7.setObjectName("tab_7")
         self.verticalLayout_21 = QtWidgets.QVBoxLayout(self.tab_7)
         self.verticalLayout_21.setObjectName("verticalLayout_21")
         self.line_26 = QtWidgets.QFrame(self.tab_7)
@@ -238,15 +315,20 @@
         self.scalebar_units.addItem("")
         self.scalebar_units.addItem("")
         self.gridLayout_20.addWidget(self.scalebar_units, 0, 2, 1, 1)
         self.label_48 = QtWidgets.QLabel(self.tab_7)
         self.label_48.setObjectName("label_48")
         self.gridLayout_20.addWidget(self.label_48, 0, 0, 1, 1)
         self.verticalLayout_21.addLayout(self.gridLayout_20)
-        spacerItem7 = QtWidgets.QSpacerItem(20, 1, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        spacerItem7 = QtWidgets.QSpacerItem(
+            20,
+            1,
+            QtWidgets.QSizePolicy.Minimum,
+            QtWidgets.QSizePolicy.Expanding,
+        )
         self.verticalLayout_21.addItem(spacerItem7)
         self.zoom_.addTab(self.tab_7, "")
         self.tab_15 = QtWidgets.QWidget()
         self.tab_15.setObjectName("tab_15")
         self.verticalLayout_22 = QtWidgets.QVBoxLayout(self.tab_15)
         self.verticalLayout_22.setObjectName("verticalLayout_22")
         self.line_27 = QtWidgets.QFrame(self.tab_15)
@@ -316,15 +398,17 @@
         self.overlay_debris = QtWidgets.QCheckBox(self.tab_15)
         self.overlay_debris.setObjectName("overlay_debris")
         self.gridLayout_30.addWidget(self.overlay_debris, 0, 1, 1, 1)
         self.overlay_range = QtWidgets.QCheckBox(self.tab_15)
         self.overlay_range.setObjectName("overlay_range")
         self.gridLayout_30.addWidget(self.overlay_range, 0, 3, 1, 1)
         self.verticalLayout_22.addLayout(self.gridLayout_30)
-        spacerItem8 = QtWidgets.QSpacerItem(20, 1, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        spacerItem8 = QtWidgets.QSpacerItem(
+            20, 1, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum
+        )
         self.verticalLayout_22.addItem(spacerItem8)
         self.zoom_.addTab(self.tab_15, "")
         self.tab_17 = QtWidgets.QWidget()
         self.tab_17.setObjectName("tab_17")
         self.verticalLayout_24 = QtWidgets.QVBoxLayout(self.tab_17)
         self.verticalLayout_24.setObjectName("verticalLayout_24")
         self.line_28 = QtWidgets.QFrame(self.tab_17)
@@ -349,46 +433,63 @@
         self.fold.setObjectName("fold")
         self.gridLayout_8.addWidget(self.fold, 0, 1, 1, 1)
         self.verticalLayout_24.addLayout(self.gridLayout_8)
         self.formLayout_3 = QtWidgets.QFormLayout()
         self.formLayout_3.setObjectName("formLayout_3")
         self.label_58 = QtWidgets.QLabel(self.tab_17)
         self.label_58.setObjectName("label_58")
-        self.formLayout_3.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.label_58)
+        self.formLayout_3.setWidget(
+            1, QtWidgets.QFormLayout.LabelRole, self.label_58
+        )
         self.unfold_tile_size = QtWidgets.QComboBox(self.tab_17)
         self.unfold_tile_size.setEditable(True)
         self.unfold_tile_size.setObjectName("unfold_tile_size")
         self.unfold_tile_size.addItem("")
         self.unfold_tile_size.addItem("")
         self.unfold_tile_size.addItem("")
         self.unfold_tile_size.addItem("")
         self.unfold_tile_size.addItem("")
-        self.formLayout_3.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.unfold_tile_size)
+        self.formLayout_3.setWidget(
+            1, QtWidgets.QFormLayout.FieldRole, self.unfold_tile_size
+        )
         self.label_59 = QtWidgets.QLabel(self.tab_17)
         self.label_59.setObjectName("label_59")
-        self.formLayout_3.setWidget(2, QtWidgets.QFormLayout.LabelRole, self.label_59)
+        self.formLayout_3.setWidget(
+            2, QtWidgets.QFormLayout.LabelRole, self.label_59
+        )
         self.unfold_tile_overlap = QtWidgets.QComboBox(self.tab_17)
         self.unfold_tile_overlap.setEditable(True)
         self.unfold_tile_overlap.setObjectName("unfold_tile_overlap")
         self.unfold_tile_overlap.addItem("")
         self.unfold_tile_overlap.addItem("")
         self.unfold_tile_overlap.addItem("")
         self.unfold_tile_overlap.addItem("")
         self.unfold_tile_overlap.addItem("")
-        self.formLayout_3.setWidget(2, QtWidgets.QFormLayout.FieldRole, self.unfold_tile_overlap)
+        self.formLayout_3.setWidget(
+            2, QtWidgets.QFormLayout.FieldRole, self.unfold_tile_overlap
+        )
         self.label_62 = QtWidgets.QLabel(self.tab_17)
         self.label_62.setObjectName("label_62")
-        self.formLayout_3.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_62)
+        self.formLayout_3.setWidget(
+            0, QtWidgets.QFormLayout.LabelRole, self.label_62
+        )
         self.unfold_mode = QtWidgets.QComboBox(self.tab_17)
         self.unfold_mode.setObjectName("unfold_mode")
         self.unfold_mode.addItem("")
         self.unfold_mode.addItem("")
-        self.formLayout_3.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.unfold_mode)
+        self.formLayout_3.setWidget(
+            0, QtWidgets.QFormLayout.FieldRole, self.unfold_mode
+        )
         self.verticalLayout_24.addLayout(self.formLayout_3)
-        spacerItem9 = QtWidgets.QSpacerItem(20, 1, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        spacerItem9 = QtWidgets.QSpacerItem(
+            20,
+            1,
+            QtWidgets.QSizePolicy.Minimum,
+            QtWidgets.QSizePolicy.Expanding,
+        )
         self.verticalLayout_24.addItem(spacerItem9)
         self.zoom_.addTab(self.tab_17, "")
         self.tab_5 = QtWidgets.QWidget()
         self.tab_5.setObjectName("tab_5")
         self.verticalLayout_20 = QtWidgets.QVBoxLayout(self.tab_5)
         self.verticalLayout_20.setObjectName("verticalLayout_20")
         self.line_30 = QtWidgets.QFrame(self.tab_5)
@@ -404,172 +505,246 @@
         self.label_86.setFont(font)
         self.label_86.setObjectName("label_86")
         self.verticalLayout_20.addWidget(self.label_86)
         self.formLayout_20 = QtWidgets.QFormLayout()
         self.formLayout_20.setObjectName("formLayout_20")
         self.label_93 = QtWidgets.QLabel(self.tab_5)
         self.label_93.setObjectName("label_93")
-        self.formLayout_20.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_93)
+        self.formLayout_20.setWidget(
+            0, QtWidgets.QFormLayout.LabelRole, self.label_93
+        )
         self.zoom_magnification = QtWidgets.QComboBox(self.tab_5)
         self.zoom_magnification.setEditable(True)
         self.zoom_magnification.setObjectName("zoom_magnification")
         self.zoom_magnification.addItem("")
         self.zoom_magnification.addItem("")
         self.zoom_magnification.addItem("")
         self.zoom_magnification.addItem("")
         self.zoom_magnification.addItem("")
         self.zoom_magnification.addItem("")
         self.zoom_magnification.addItem("")
         self.zoom_magnification.addItem("")
         self.zoom_magnification.addItem("")
         self.zoom_magnification.addItem("")
         self.zoom_magnification.addItem("")
-        self.formLayout_20.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.zoom_magnification)
+        self.formLayout_20.setWidget(
+            0, QtWidgets.QFormLayout.FieldRole, self.zoom_magnification
+        )
         self.verticalLayout_20.addLayout(self.formLayout_20)
         self.zoom_apply = QtWidgets.QPushButton(self.tab_5)
         self.zoom_apply.setObjectName("zoom_apply")
         self.verticalLayout_20.addWidget(self.zoom_apply)
-        spacerItem10 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        spacerItem10 = QtWidgets.QSpacerItem(
+            20,
+            40,
+            QtWidgets.QSizePolicy.Minimum,
+            QtWidgets.QSizePolicy.Expanding,
+        )
         self.verticalLayout_20.addItem(spacerItem10)
         self.zoom_.addTab(self.tab_5, "")
         self.verticalLayout_5.addWidget(self.zoom_)
-        spacerItem11 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        spacerItem11 = QtWidgets.QSpacerItem(
+            20,
+            40,
+            QtWidgets.QSizePolicy.Minimum,
+            QtWidgets.QSizePolicy.Expanding,
+        )
         self.verticalLayout_5.addItem(spacerItem11)
         tab_widget.addTab(self.tab, "")
         self.segement_tab = QtWidgets.QWidget()
         self.segement_tab.setObjectName("segement_tab")
         self.verticalLayout_2 = QtWidgets.QVBoxLayout(self.segement_tab)
         self.verticalLayout_2.setObjectName("verticalLayout_2")
         self.line_12 = QtWidgets.QFrame(self.segement_tab)
         self.line_12.setFrameShape(QtWidgets.QFrame.HLine)
         self.line_12.setFrameShadow(QtWidgets.QFrame.Sunken)
         self.line_12.setObjectName("line_12")
         self.verticalLayout_2.addWidget(self.line_12)
-        self.cellpose_select_custom_model = QtWidgets.QPushButton(self.segement_tab)
-        self.cellpose_select_custom_model.setObjectName("cellpose_select_custom_model")
+        self.cellpose_select_custom_model = QtWidgets.QPushButton(
+            self.segement_tab
+        )
+        self.cellpose_select_custom_model.setObjectName(
+            "cellpose_select_custom_model"
+        )
         self.verticalLayout_2.addWidget(self.cellpose_select_custom_model)
-        spacerItem12 = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        spacerItem12 = QtWidgets.QSpacerItem(
+            20,
+            10,
+            QtWidgets.QSizePolicy.Minimum,
+            QtWidgets.QSizePolicy.Minimum,
+        )
         self.verticalLayout_2.addItem(spacerItem12)
         self.tabWidget_3 = QtWidgets.QTabWidget(self.segement_tab)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Preferred)
+        sizePolicy = QtWidgets.QSizePolicy(
+            QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Preferred
+        )
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
-        sizePolicy.setHeightForWidth(self.tabWidget_3.sizePolicy().hasHeightForWidth())
+        sizePolicy.setHeightForWidth(
+            self.tabWidget_3.sizePolicy().hasHeightForWidth()
+        )
         self.tabWidget_3.setSizePolicy(sizePolicy)
         self.tabWidget_3.setObjectName("tabWidget_3")
         self.tab_6 = QtWidgets.QWidget()
         self.tab_6.setObjectName("tab_6")
         self.verticalLayout_10 = QtWidgets.QVBoxLayout(self.tab_6)
         self.verticalLayout_10.setObjectName("verticalLayout_10")
         self.formLayout_12 = QtWidgets.QFormLayout()
         self.formLayout_12.setObjectName("formLayout_12")
         self.label_97 = QtWidgets.QLabel(self.tab_6)
         self.label_97.setObjectName("label_97")
-        self.formLayout_12.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_97)
+        self.formLayout_12.setWidget(
+            0, QtWidgets.QFormLayout.LabelRole, self.label_97
+        )
         self.label_2 = QtWidgets.QLabel(self.tab_6)
         self.label_2.setObjectName("label_2")
-        self.formLayout_12.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.label_2)
+        self.formLayout_12.setWidget(
+            1, QtWidgets.QFormLayout.LabelRole, self.label_2
+        )
         self.cellpose_segchannel = QtWidgets.QComboBox(self.tab_6)
         self.cellpose_segchannel.setObjectName("cellpose_segchannel")
-        self.formLayout_12.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.cellpose_segchannel)
+        self.formLayout_12.setWidget(
+            1, QtWidgets.QFormLayout.FieldRole, self.cellpose_segchannel
+        )
         self.label = QtWidgets.QLabel(self.tab_6)
         self.label.setObjectName("label")
-        self.formLayout_12.setWidget(2, QtWidgets.QFormLayout.LabelRole, self.label)
+        self.formLayout_12.setWidget(
+            2, QtWidgets.QFormLayout.LabelRole, self.label
+        )
         self.cellpose_segmodel = QtWidgets.QComboBox(self.tab_6)
         self.cellpose_segmodel.setObjectName("cellpose_segmodel")
         self.cellpose_segmodel.addItem("")
         self.cellpose_segmodel.addItem("")
         self.cellpose_segmodel.addItem("")
         self.cellpose_segmodel.addItem("")
         self.cellpose_segmodel.addItem("")
         self.cellpose_segmodel.addItem("")
         self.cellpose_segmodel.addItem("")
-        self.formLayout_12.setWidget(2, QtWidgets.QFormLayout.FieldRole, self.cellpose_segmodel)
+        self.formLayout_12.setWidget(
+            2, QtWidgets.QFormLayout.FieldRole, self.cellpose_segmodel
+        )
         self.cellpose_seg_mode = QtWidgets.QComboBox(self.tab_6)
         self.cellpose_seg_mode.setObjectName("cellpose_seg_mode")
         self.cellpose_seg_mode.addItem("")
         self.cellpose_seg_mode.addItem("")
-        self.formLayout_12.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.cellpose_seg_mode)
+        self.formLayout_12.setWidget(
+            0, QtWidgets.QFormLayout.FieldRole, self.cellpose_seg_mode
+        )
         self.verticalLayout_10.addLayout(self.formLayout_12)
-        spacerItem13 = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        spacerItem13 = QtWidgets.QSpacerItem(
+            20,
+            10,
+            QtWidgets.QSizePolicy.Minimum,
+            QtWidgets.QSizePolicy.Minimum,
+        )
         self.verticalLayout_10.addItem(spacerItem13)
         self.cellpose_segment_active = QtWidgets.QPushButton(self.tab_6)
         self.cellpose_segment_active.setObjectName("cellpose_segment_active")
         self.verticalLayout_10.addWidget(self.cellpose_segment_active)
         self.cellpose_segment_all = QtWidgets.QPushButton(self.tab_6)
         self.cellpose_segment_all.setObjectName("cellpose_segment_all")
         self.verticalLayout_10.addWidget(self.cellpose_segment_all)
-        spacerItem14 = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        spacerItem14 = QtWidgets.QSpacerItem(
+            20,
+            10,
+            QtWidgets.QSizePolicy.Minimum,
+            QtWidgets.QSizePolicy.Minimum,
+        )
         self.verticalLayout_10.addItem(spacerItem14)
         self.formLayout_13 = QtWidgets.QFormLayout()
         self.formLayout_13.setObjectName("formLayout_13")
         self.cellpose_progressbar = QtWidgets.QProgressBar(self.tab_6)
         self.cellpose_progressbar.setMaximumSize(QtCore.QSize(16777215, 20))
         self.cellpose_progressbar.setProperty("value", 0)
         self.cellpose_progressbar.setObjectName("cellpose_progressbar")
-        self.formLayout_13.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.cellpose_progressbar)
+        self.formLayout_13.setWidget(
+            0, QtWidgets.QFormLayout.FieldRole, self.cellpose_progressbar
+        )
         self.label_35 = QtWidgets.QLabel(self.tab_6)
         self.label_35.setObjectName("label_35")
-        self.formLayout_13.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_35)
+        self.formLayout_13.setWidget(
+            0, QtWidgets.QFormLayout.LabelRole, self.label_35
+        )
         self.verticalLayout_10.addLayout(self.formLayout_13)
         self.tabWidget_3.addTab(self.tab_6, "")
         self.tab_11 = QtWidgets.QWidget()
         self.tab_11.setObjectName("tab_11")
         self.verticalLayout_13 = QtWidgets.QVBoxLayout(self.tab_11)
         self.verticalLayout_13.setObjectName("verticalLayout_13")
         self.formLayout_15 = QtWidgets.QFormLayout()
         self.formLayout_15.setObjectName("formLayout_15")
         self.label_8 = QtWidgets.QLabel(self.tab_11)
         self.label_8.setObjectName("label_8")
-        self.formLayout_15.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_8)
+        self.formLayout_15.setWidget(
+            0, QtWidgets.QFormLayout.LabelRole, self.label_8
+        )
         self.cellpose_trainchannel = QtWidgets.QComboBox(self.tab_11)
         self.cellpose_trainchannel.setObjectName("cellpose_trainchannel")
-        self.formLayout_15.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.cellpose_trainchannel)
+        self.formLayout_15.setWidget(
+            0, QtWidgets.QFormLayout.FieldRole, self.cellpose_trainchannel
+        )
         self.label_9 = QtWidgets.QLabel(self.tab_11)
         self.label_9.setObjectName("label_9")
-        self.formLayout_15.setWidget(2, QtWidgets.QFormLayout.LabelRole, self.label_9)
+        self.formLayout_15.setWidget(
+            2, QtWidgets.QFormLayout.LabelRole, self.label_9
+        )
         self.cellpose_nepochs = QtWidgets.QComboBox(self.tab_11)
         self.cellpose_nepochs.setEditable(True)
         self.cellpose_nepochs.setObjectName("cellpose_nepochs")
         self.cellpose_nepochs.addItem("")
         self.cellpose_nepochs.addItem("")
         self.cellpose_nepochs.addItem("")
         self.cellpose_nepochs.addItem("")
         self.cellpose_nepochs.addItem("")
         self.cellpose_nepochs.addItem("")
-        self.formLayout_15.setWidget(2, QtWidgets.QFormLayout.FieldRole, self.cellpose_nepochs)
+        self.formLayout_15.setWidget(
+            2, QtWidgets.QFormLayout.FieldRole, self.cellpose_nepochs
+        )
         self.label_10 = QtWidgets.QLabel(self.tab_11)
         self.label_10.setObjectName("label_10")
-        self.formLayout_15.setWidget(3, QtWidgets.QFormLayout.LabelRole, self.label_10)
+        self.formLayout_15.setWidget(
+            3, QtWidgets.QFormLayout.LabelRole, self.label_10
+        )
         self.cellpose_batchsize = QtWidgets.QComboBox(self.tab_11)
         self.cellpose_batchsize.setEditable(True)
         self.cellpose_batchsize.setObjectName("cellpose_batchsize")
         self.cellpose_batchsize.addItem("")
         self.cellpose_batchsize.addItem("")
         self.cellpose_batchsize.addItem("")
         self.cellpose_batchsize.addItem("")
         self.cellpose_batchsize.addItem("")
         self.cellpose_batchsize.addItem("")
         self.cellpose_batchsize.addItem("")
-        self.formLayout_15.setWidget(3, QtWidgets.QFormLayout.FieldRole, self.cellpose_batchsize)
+        self.formLayout_15.setWidget(
+            3, QtWidgets.QFormLayout.FieldRole, self.cellpose_batchsize
+        )
         self.label_11 = QtWidgets.QLabel(self.tab_11)
         self.label_11.setObjectName("label_11")
-        self.formLayout_15.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.label_11)
+        self.formLayout_15.setWidget(
+            1, QtWidgets.QFormLayout.LabelRole, self.label_11
+        )
         self.cellpose_trainmodel = QtWidgets.QComboBox(self.tab_11)
         self.cellpose_trainmodel.setObjectName("cellpose_trainmodel")
         self.cellpose_trainmodel.addItem("")
         self.cellpose_trainmodel.addItem("")
         self.cellpose_trainmodel.addItem("")
         self.cellpose_trainmodel.addItem("")
         self.cellpose_trainmodel.addItem("")
         self.cellpose_trainmodel.addItem("")
         self.cellpose_trainmodel.addItem("")
-        self.formLayout_15.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.cellpose_trainmodel)
+        self.formLayout_15.setWidget(
+            1, QtWidgets.QFormLayout.FieldRole, self.cellpose_trainmodel
+        )
         self.verticalLayout_13.addLayout(self.formLayout_15)
-        spacerItem15 = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        spacerItem15 = QtWidgets.QSpacerItem(
+            20,
+            10,
+            QtWidgets.QSizePolicy.Minimum,
+            QtWidgets.QSizePolicy.Expanding,
+        )
         self.verticalLayout_13.addItem(spacerItem15)
         self.cellpose_save_dir = QtWidgets.QPushButton(self.tab_11)
         self.cellpose_save_dir.setObjectName("cellpose_save_dir")
         self.verticalLayout_13.addWidget(self.cellpose_save_dir)
         self.cellpose_train_model = QtWidgets.QPushButton(self.tab_11)
         self.cellpose_train_model.setObjectName("cellpose_train_model")
         self.verticalLayout_13.addWidget(self.cellpose_train_model)
@@ -586,36 +761,46 @@
         self.label_94.setFont(font)
         self.label_94.setObjectName("label_94")
         self.verticalLayout_14.addWidget(self.label_94)
         self.gridLayout_2 = QtWidgets.QGridLayout()
         self.gridLayout_2.setObjectName("gridLayout_2")
         self.cellpose_flowthresh_label = QtWidgets.QLabel(self.tab_12)
         self.cellpose_flowthresh_label.setMinimumSize(QtCore.QSize(28, 22))
-        self.cellpose_flowthresh_label.setObjectName("cellpose_flowthresh_label")
-        self.gridLayout_2.addWidget(self.cellpose_flowthresh_label, 0, 2, 1, 1, QtCore.Qt.AlignLeft)
+        self.cellpose_flowthresh_label.setObjectName(
+            "cellpose_flowthresh_label"
+        )
+        self.gridLayout_2.addWidget(
+            self.cellpose_flowthresh_label, 0, 2, 1, 1, QtCore.Qt.AlignLeft
+        )
         self.cellpose_flowthresh = QtWidgets.QSlider(self.tab_12)
         self.cellpose_flowthresh.setMaximum(100)
         self.cellpose_flowthresh.setSingleStep(10)
         self.cellpose_flowthresh.setPageStep(10)
         self.cellpose_flowthresh.setSliderPosition(90)
         self.cellpose_flowthresh.setOrientation(QtCore.Qt.Horizontal)
         self.cellpose_flowthresh.setObjectName("cellpose_flowthresh")
         self.gridLayout_2.addWidget(self.cellpose_flowthresh, 0, 1, 1, 1)
         self.label_3 = QtWidgets.QLabel(self.tab_12)
         self.label_3.setObjectName("label_3")
         self.gridLayout_2.addWidget(self.label_3, 0, 0, 1, 1)
         self.cellpose_maskthresh_label = QtWidgets.QLabel(self.tab_12)
         self.cellpose_maskthresh_label.setMinimumSize(QtCore.QSize(28, 22))
-        self.cellpose_maskthresh_label.setObjectName("cellpose_maskthresh_label")
-        self.gridLayout_2.addWidget(self.cellpose_maskthresh_label, 1, 2, 1, 1, QtCore.Qt.AlignLeft)
+        self.cellpose_maskthresh_label.setObjectName(
+            "cellpose_maskthresh_label"
+        )
+        self.gridLayout_2.addWidget(
+            self.cellpose_maskthresh_label, 1, 2, 1, 1, QtCore.Qt.AlignLeft
+        )
         self.cellpose_minsize_label = QtWidgets.QLabel(self.tab_12)
         self.cellpose_minsize_label.setMinimumSize(QtCore.QSize(24, 22))
         self.cellpose_minsize_label.setMaximumSize(QtCore.QSize(24, 16777215))
         self.cellpose_minsize_label.setObjectName("cellpose_minsize_label")
-        self.gridLayout_2.addWidget(self.cellpose_minsize_label, 2, 2, 1, 1, QtCore.Qt.AlignLeft)
+        self.gridLayout_2.addWidget(
+            self.cellpose_minsize_label, 2, 2, 1, 1, QtCore.Qt.AlignLeft
+        )
         self.label_5 = QtWidgets.QLabel(self.tab_12)
         self.label_5.setObjectName("label_5")
         self.gridLayout_2.addWidget(self.label_5, 1, 0, 1, 1)
         self.label_6 = QtWidgets.QLabel(self.tab_12)
         self.label_6.setObjectName("label_6")
         self.gridLayout_2.addWidget(self.label_6, 2, 0, 1, 1)
         self.cellpose_minsize = QtWidgets.QSlider(self.tab_12)
@@ -644,39 +829,53 @@
         self.label_4 = QtWidgets.QLabel(self.tab_12)
         self.label_4.setObjectName("label_4")
         self.gridLayout_2.addWidget(self.label_4, 3, 0, 1, 1)
         self.cellpose_diameter_label = QtWidgets.QLabel(self.tab_12)
         self.cellpose_diameter_label.setObjectName("cellpose_diameter_label")
         self.gridLayout_2.addWidget(self.cellpose_diameter_label, 3, 2, 1, 1)
         self.verticalLayout_14.addLayout(self.gridLayout_2)
-        spacerItem16 = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        spacerItem16 = QtWidgets.QSpacerItem(
+            20,
+            10,
+            QtWidgets.QSizePolicy.Minimum,
+            QtWidgets.QSizePolicy.Expanding,
+        )
         self.verticalLayout_14.addItem(spacerItem16)
         self.label_95 = QtWidgets.QLabel(self.tab_12)
         font = QtGui.QFont()
         font.setPointSize(10)
         font.setBold(True)
         font.setWeight(75)
         self.label_95.setFont(font)
         self.label_95.setObjectName("label_95")
         self.verticalLayout_14.addWidget(self.label_95)
         self.formLayout_21 = QtWidgets.QFormLayout()
         self.formLayout_21.setObjectName("formLayout_21")
         self.label_96 = QtWidgets.QLabel(self.tab_12)
         self.label_96.setObjectName("label_96")
-        self.formLayout_21.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_96)
+        self.formLayout_21.setWidget(
+            0, QtWidgets.QFormLayout.LabelRole, self.label_96
+        )
         self.cellpose_min_seg_size = QtWidgets.QComboBox(self.tab_12)
         self.cellpose_min_seg_size.setEditable(True)
         self.cellpose_min_seg_size.setObjectName("cellpose_min_seg_size")
         self.cellpose_min_seg_size.addItem("")
         self.cellpose_min_seg_size.addItem("")
         self.cellpose_min_seg_size.addItem("")
         self.cellpose_min_seg_size.addItem("")
-        self.formLayout_21.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.cellpose_min_seg_size)
+        self.formLayout_21.setWidget(
+            0, QtWidgets.QFormLayout.FieldRole, self.cellpose_min_seg_size
+        )
         self.verticalLayout_14.addLayout(self.formLayout_21)
-        spacerItem17 = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        spacerItem17 = QtWidgets.QSpacerItem(
+            20,
+            10,
+            QtWidgets.QSizePolicy.Minimum,
+            QtWidgets.QSizePolicy.Expanding,
+        )
         self.verticalLayout_14.addItem(spacerItem17)
         self.cellpose_clear_previous = QtWidgets.QCheckBox(self.tab_12)
         self.cellpose_clear_previous.setChecked(True)
         self.cellpose_clear_previous.setObjectName("cellpose_clear_previous")
         self.verticalLayout_14.addWidget(self.cellpose_clear_previous)
         self.cellpose_usegpu = QtWidgets.QCheckBox(self.tab_12)
         self.cellpose_usegpu.setChecked(True)
@@ -689,15 +888,20 @@
         self.tabWidget_3.addTab(self.tab_12, "")
         self.verticalLayout_2.addWidget(self.tabWidget_3)
         self.line_6 = QtWidgets.QFrame(self.segement_tab)
         self.line_6.setFrameShape(QtWidgets.QFrame.HLine)
         self.line_6.setFrameShadow(QtWidgets.QFrame.Sunken)
         self.line_6.setObjectName("line_6")
         self.verticalLayout_2.addWidget(self.line_6)
-        spacerItem18 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        spacerItem18 = QtWidgets.QSpacerItem(
+            20,
+            40,
+            QtWidgets.QSizePolicy.Minimum,
+            QtWidgets.QSizePolicy.Expanding,
+        )
         self.verticalLayout_2.addItem(spacerItem18)
         tab_widget.addTab(self.segement_tab, "")
         self.tab_3 = QtWidgets.QWidget()
         self.tab_3.setEnabled(True)
         self.tab_3.setObjectName("tab_3")
         self.verticalLayout_3 = QtWidgets.QVBoxLayout(self.tab_3)
         self.verticalLayout_3.setObjectName("verticalLayout_3")
@@ -722,32 +926,46 @@
         self.modify_classify = QtWidgets.QPushButton(self.tab_3)
         self.modify_classify.setObjectName("modify_classify")
         self.gridLayout_3.addWidget(self.modify_classify, 0, 3, 1, 1)
         self.modify_segment = QtWidgets.QPushButton(self.tab_3)
         self.modify_segment.setObjectName("modify_segment")
         self.gridLayout_3.addWidget(self.modify_segment, 0, 1, 1, 1)
         self.verticalLayout_3.addLayout(self.gridLayout_3)
-        spacerItem19 = QtWidgets.QSpacerItem(334, 14, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        spacerItem19 = QtWidgets.QSpacerItem(
+            334,
+            14,
+            QtWidgets.QSizePolicy.Minimum,
+            QtWidgets.QSizePolicy.Minimum,
+        )
         self.verticalLayout_3.addItem(spacerItem19)
         self.formLayout_22 = QtWidgets.QFormLayout()
         self.formLayout_22.setObjectName("formLayout_22")
         self.label_98 = QtWidgets.QLabel(self.tab_3)
         self.label_98.setObjectName("label_98")
-        self.formLayout_22.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_98)
+        self.formLayout_22.setWidget(
+            0, QtWidgets.QFormLayout.LabelRole, self.label_98
+        )
         self.modify_channel = QtWidgets.QComboBox(self.tab_3)
         self.modify_channel.setObjectName("modify_channel")
         self.modify_channel.addItem("")
         self.modify_channel.addItem("")
-        self.formLayout_22.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.modify_channel)
+        self.formLayout_22.setWidget(
+            0, QtWidgets.QFormLayout.FieldRole, self.modify_channel
+        )
         self.verticalLayout_3.addLayout(self.formLayout_22)
         self.modify_auto_panzoom = QtWidgets.QCheckBox(self.tab_3)
         self.modify_auto_panzoom.setChecked(True)
         self.modify_auto_panzoom.setObjectName("modify_auto_panzoom")
         self.verticalLayout_3.addWidget(self.modify_auto_panzoom)
-        spacerItem20 = QtWidgets.QSpacerItem(334, 14, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        spacerItem20 = QtWidgets.QSpacerItem(
+            334,
+            14,
+            QtWidgets.QSizePolicy.Minimum,
+            QtWidgets.QSizePolicy.Minimum,
+        )
         self.verticalLayout_3.addItem(spacerItem20)
         self.line_18 = QtWidgets.QFrame(self.tab_3)
         self.line_18.setFrameShape(QtWidgets.QFrame.HLine)
         self.line_18.setFrameShadow(QtWidgets.QFrame.Sunken)
         self.line_18.setObjectName("line_18")
         self.verticalLayout_3.addWidget(self.line_18)
         self.label_16 = QtWidgets.QLabel(self.tab_3)
@@ -775,15 +993,20 @@
         self.modify_split = QtWidgets.QPushButton(self.tab_3)
         self.modify_split.setObjectName("modify_split")
         self.gridLayout_4.addWidget(self.modify_split, 1, 0, 1, 1)
         self.modify_extend = QtWidgets.QPushButton(self.tab_3)
         self.modify_extend.setObjectName("modify_extend")
         self.gridLayout_4.addWidget(self.modify_extend, 0, 1, 1, 1)
         self.verticalLayout_3.addLayout(self.gridLayout_4)
-        spacerItem21 = QtWidgets.QSpacerItem(334, 14, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        spacerItem21 = QtWidgets.QSpacerItem(
+            334,
+            14,
+            QtWidgets.QSizePolicy.Minimum,
+            QtWidgets.QSizePolicy.Minimum,
+        )
         self.verticalLayout_3.addItem(spacerItem21)
         self.line_19 = QtWidgets.QFrame(self.tab_3)
         self.line_19.setFrameShape(QtWidgets.QFrame.HLine)
         self.line_19.setFrameShadow(QtWidgets.QFrame.Sunken)
         self.line_19.setObjectName("line_19")
         self.verticalLayout_3.addWidget(self.line_19)
         self.label_28 = QtWidgets.QLabel(self.tab_3)
@@ -801,16 +1024,15 @@
         self.classify_edge.setObjectName("classify_edge")
         self.gridLayout_5.addWidget(self.classify_edge, 1, 2, 1, 1)
         self.classify_divided = QtWidgets.QPushButton(self.tab_3)
         self.classify_divided.setStyleSheet("color: rgb(0, 170, 255);")
         self.classify_divided.setObjectName("classify_divided")
         self.gridLayout_5.addWidget(self.classify_divided, 0, 2, 1, 1)
         self.classify_dividing = QtWidgets.QPushButton(self.tab_3)
-        self.classify_dividing.setStyleSheet("\n"
-"color: rgb(0, 255, 0);")
+        self.classify_dividing.setStyleSheet("\n" "color: rgb(0, 255, 0);")
         self.classify_dividing.setObjectName("classify_dividing")
         self.gridLayout_5.addWidget(self.classify_dividing, 0, 1, 1, 1)
         self.classify_vertical = QtWidgets.QPushButton(self.tab_3)
         self.classify_vertical.setStyleSheet("color:rgb(170, 0, 255)")
         self.classify_vertical.setObjectName("classify_vertical")
         self.gridLayout_5.addWidget(self.classify_vertical, 1, 0, 1, 1)
         self.classify_broken = QtWidgets.QPushButton(self.tab_3)
@@ -818,15 +1040,20 @@
         self.classify_broken.setObjectName("classify_broken")
         self.gridLayout_5.addWidget(self.classify_broken, 1, 1, 1, 1)
         self.classify_single = QtWidgets.QPushButton(self.tab_3)
         self.classify_single.setStyleSheet("color: rgb(255, 255, 255);")
         self.classify_single.setObjectName("classify_single")
         self.gridLayout_5.addWidget(self.classify_single, 0, 0, 1, 1)
         self.verticalLayout_3.addLayout(self.gridLayout_5)
-        spacerItem22 = QtWidgets.QSpacerItem(334, 14, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        spacerItem22 = QtWidgets.QSpacerItem(
+            334,
+            14,
+            QtWidgets.QSizePolicy.Minimum,
+            QtWidgets.QSizePolicy.Minimum,
+        )
         self.verticalLayout_3.addItem(spacerItem22)
         self.line_21 = QtWidgets.QFrame(self.tab_3)
         self.line_21.setFrameShape(QtWidgets.QFrame.HLine)
         self.line_21.setFrameShadow(QtWidgets.QFrame.Sunken)
         self.line_21.setObjectName("line_21")
         self.verticalLayout_3.addWidget(self.line_21)
         self.label_14 = QtWidgets.QLabel(self.tab_3)
@@ -837,30 +1064,38 @@
         self.label_14.setFont(font)
         self.label_14.setObjectName("label_14")
         self.verticalLayout_3.addWidget(self.label_14)
         self.formLayout_17 = QtWidgets.QFormLayout()
         self.formLayout_17.setObjectName("formLayout_17")
         self.label_18 = QtWidgets.QLabel(self.tab_3)
         self.label_18.setObjectName("label_18")
-        self.formLayout_17.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_18)
+        self.formLayout_17.setWidget(
+            0, QtWidgets.QFormLayout.LabelRole, self.label_18
+        )
         self.set_quality_mode = QtWidgets.QComboBox(self.tab_3)
         self.set_quality_mode.setObjectName("set_quality_mode")
         self.set_quality_mode.addItem("")
         self.set_quality_mode.addItem("")
         self.set_quality_mode.addItem("")
         self.set_quality_mode.addItem("")
-        self.formLayout_17.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.set_quality_mode)
+        self.formLayout_17.setWidget(
+            0, QtWidgets.QFormLayout.FieldRole, self.set_quality_mode
+        )
         self.verticalLayout_3.addLayout(self.formLayout_17)
         self.gridLayout_21 = QtWidgets.QGridLayout()
         self.gridLayout_21.setObjectName("gridLayout_21")
         self.label_34 = QtWidgets.QLabel(self.tab_3)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Maximum)
+        sizePolicy = QtWidgets.QSizePolicy(
+            QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Maximum
+        )
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
-        sizePolicy.setHeightForWidth(self.label_34.sizePolicy().hasHeightForWidth())
+        sizePolicy.setHeightForWidth(
+            self.label_34.sizePolicy().hasHeightForWidth()
+        )
         self.label_34.setSizePolicy(sizePolicy)
         self.label_34.setMinimumSize(QtCore.QSize(50, 0))
         font = QtGui.QFont()
         font.setPointSize(10)
         font.setBold(True)
         font.setWeight(75)
         self.label_34.setFont(font)
@@ -887,18 +1122,22 @@
         self.set_debris_2 = QtWidgets.QPushButton(self.tab_3)
         self.set_debris_2.setObjectName("set_debris_2")
         self.gridLayout_22.addWidget(self.set_debris_2, 0, 2, 1, 1)
         self.set_debris_3 = QtWidgets.QPushButton(self.tab_3)
         self.set_debris_3.setObjectName("set_debris_3")
         self.gridLayout_22.addWidget(self.set_debris_3, 0, 3, 1, 1)
         self.label_39 = QtWidgets.QLabel(self.tab_3)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Maximum)
+        sizePolicy = QtWidgets.QSizePolicy(
+            QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Maximum
+        )
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
-        sizePolicy.setHeightForWidth(self.label_39.sizePolicy().hasHeightForWidth())
+        sizePolicy.setHeightForWidth(
+            self.label_39.sizePolicy().hasHeightForWidth()
+        )
         self.label_39.setSizePolicy(sizePolicy)
         self.label_39.setMinimumSize(QtCore.QSize(50, 0))
         font = QtGui.QFont()
         font.setPointSize(10)
         font.setBold(True)
         font.setWeight(75)
         self.label_39.setFont(font)
@@ -910,15 +1149,20 @@
         self.set_debris_4 = QtWidgets.QPushButton(self.tab_3)
         self.set_debris_4.setObjectName("set_debris_4")
         self.gridLayout_22.addWidget(self.set_debris_4, 0, 4, 1, 1)
         self.set_debris_5 = QtWidgets.QPushButton(self.tab_3)
         self.set_debris_5.setObjectName("set_debris_5")
         self.gridLayout_22.addWidget(self.set_debris_5, 0, 5, 1, 1)
         self.verticalLayout_3.addLayout(self.gridLayout_22)
-        spacerItem23 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        spacerItem23 = QtWidgets.QSpacerItem(
+            20,
+            40,
+            QtWidgets.QSizePolicy.Minimum,
+            QtWidgets.QSizePolicy.Expanding,
+        )
         self.verticalLayout_3.addItem(spacerItem23)
         tab_widget.addTab(self.tab_3, "")
         self.tab_2 = QtWidgets.QWidget()
         self.tab_2.setObjectName("tab_2")
         self.verticalLayout_7 = QtWidgets.QVBoxLayout(self.tab_2)
         self.verticalLayout_7.setObjectName("verticalLayout_7")
         self.label_29 = QtWidgets.QLabel(self.tab_2)
@@ -934,97 +1178,138 @@
         self.oufti_panzoom_mode = QtWidgets.QRadioButton(self.tab_2)
         self.oufti_panzoom_mode.setObjectName("oufti_panzoom_mode")
         self.gridLayout_10.addWidget(self.oufti_panzoom_mode, 0, 0, 1, 1)
         self.oufti_edit_mode = QtWidgets.QRadioButton(self.tab_2)
         self.oufti_edit_mode.setObjectName("oufti_edit_mode")
         self.gridLayout_10.addWidget(self.oufti_edit_mode, 0, 1, 1, 1)
         self.verticalLayout_7.addLayout(self.gridLayout_10)
-        spacerItem24 = QtWidgets.QSpacerItem(360, 13, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        spacerItem24 = QtWidgets.QSpacerItem(
+            360,
+            13,
+            QtWidgets.QSizePolicy.Minimum,
+            QtWidgets.QSizePolicy.Minimum,
+        )
         self.verticalLayout_7.addItem(spacerItem24)
         self.label_20 = QtWidgets.QLabel(self.tab_2)
         font = QtGui.QFont()
         font.setPointSize(10)
         font.setBold(True)
         font.setWeight(75)
         self.label_20.setFont(font)
         self.label_20.setObjectName("label_20")
         self.verticalLayout_7.addWidget(self.label_20)
         self.formLayout_4 = QtWidgets.QFormLayout()
         self.formLayout_4.setObjectName("formLayout_4")
         self.label_25 = QtWidgets.QLabel(self.tab_2)
         self.label_25.setObjectName("label_25")
-        self.formLayout_4.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_25)
+        self.formLayout_4.setWidget(
+            0, QtWidgets.QFormLayout.LabelRole, self.label_25
+        )
         self.oufti_midline_vertexes = QtWidgets.QComboBox(self.tab_2)
         self.oufti_midline_vertexes.setObjectName("oufti_midline_vertexes")
         self.oufti_midline_vertexes.addItem("")
         self.oufti_midline_vertexes.addItem("")
         self.oufti_midline_vertexes.addItem("")
         self.oufti_midline_vertexes.addItem("")
         self.oufti_midline_vertexes.addItem("")
         self.oufti_midline_vertexes.addItem("")
-        self.formLayout_4.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.oufti_midline_vertexes)
+        self.formLayout_4.setWidget(
+            0, QtWidgets.QFormLayout.FieldRole, self.oufti_midline_vertexes
+        )
         self.verticalLayout_7.addLayout(self.formLayout_4)
         self.gridLayout_16 = QtWidgets.QGridLayout()
         self.gridLayout_16.setObjectName("gridLayout_16")
         self.oufti_generate_active_midlines = QtWidgets.QPushButton(self.tab_2)
-        self.oufti_generate_active_midlines.setObjectName("oufti_generate_active_midlines")
-        self.gridLayout_16.addWidget(self.oufti_generate_active_midlines, 0, 0, 1, 1)
+        self.oufti_generate_active_midlines.setObjectName(
+            "oufti_generate_active_midlines"
+        )
+        self.gridLayout_16.addWidget(
+            self.oufti_generate_active_midlines, 0, 0, 1, 1
+        )
         self.gridLayout_17 = QtWidgets.QGridLayout()
         self.gridLayout_17.setObjectName("gridLayout_17")
         self.oufti_generate_all_midlines = QtWidgets.QPushButton(self.tab_2)
-        self.oufti_generate_all_midlines.setObjectName("oufti_generate_all_midlines")
-        self.gridLayout_17.addWidget(self.oufti_generate_all_midlines, 0, 0, 1, 1)
+        self.oufti_generate_all_midlines.setObjectName(
+            "oufti_generate_all_midlines"
+        )
+        self.gridLayout_17.addWidget(
+            self.oufti_generate_all_midlines, 0, 0, 1, 1
+        )
         self.gridLayout_16.addLayout(self.gridLayout_17, 0, 1, 1, 1)
         self.verticalLayout_7.addLayout(self.gridLayout_16)
-        spacerItem25 = QtWidgets.QSpacerItem(360, 13, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        spacerItem25 = QtWidgets.QSpacerItem(
+            360,
+            13,
+            QtWidgets.QSizePolicy.Minimum,
+            QtWidgets.QSizePolicy.Minimum,
+        )
         self.verticalLayout_7.addItem(spacerItem25)
         self.label_63 = QtWidgets.QLabel(self.tab_2)
         font = QtGui.QFont()
         font.setPointSize(10)
         font.setBold(True)
         font.setWeight(75)
         self.label_63.setFont(font)
         self.label_63.setObjectName("label_63")
         self.verticalLayout_7.addWidget(self.label_63)
         self.gridLayout_15 = QtWidgets.QGridLayout()
         self.gridLayout_15.setObjectName("gridLayout_15")
         self.oufti_centre_active_midlines = QtWidgets.QPushButton(self.tab_2)
-        self.oufti_centre_active_midlines.setObjectName("oufti_centre_active_midlines")
-        self.gridLayout_15.addWidget(self.oufti_centre_active_midlines, 0, 0, 1, 1)
+        self.oufti_centre_active_midlines.setObjectName(
+            "oufti_centre_active_midlines"
+        )
+        self.gridLayout_15.addWidget(
+            self.oufti_centre_active_midlines, 0, 0, 1, 1
+        )
         self.oufti_centre_all_midlines = QtWidgets.QPushButton(self.tab_2)
-        self.oufti_centre_all_midlines.setObjectName("oufti_centre_all_midlines")
-        self.gridLayout_15.addWidget(self.oufti_centre_all_midlines, 0, 1, 1, 1)
+        self.oufti_centre_all_midlines.setObjectName(
+            "oufti_centre_all_midlines"
+        )
+        self.gridLayout_15.addWidget(
+            self.oufti_centre_all_midlines, 0, 1, 1, 1
+        )
         self.verticalLayout_7.addLayout(self.gridLayout_15)
-        spacerItem26 = QtWidgets.QSpacerItem(360, 13, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        spacerItem26 = QtWidgets.QSpacerItem(
+            360,
+            13,
+            QtWidgets.QSizePolicy.Minimum,
+            QtWidgets.QSizePolicy.Minimum,
+        )
         self.verticalLayout_7.addItem(spacerItem26)
         self.label_61 = QtWidgets.QLabel(self.tab_2)
         font = QtGui.QFont()
         font.setPointSize(10)
         font.setBold(True)
         font.setWeight(75)
         self.label_61.setFont(font)
         self.label_61.setObjectName("label_61")
         self.verticalLayout_7.addWidget(self.label_61)
         self.formLayout_7 = QtWidgets.QFormLayout()
         self.formLayout_7.setObjectName("formLayout_7")
         self.label_64 = QtWidgets.QLabel(self.tab_2)
         self.label_64.setObjectName("label_64")
-        self.formLayout_7.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_64)
+        self.formLayout_7.setWidget(
+            0, QtWidgets.QFormLayout.LabelRole, self.label_64
+        )
         self.oufti_mesh_length = QtWidgets.QComboBox(self.tab_2)
         self.oufti_mesh_length.setObjectName("oufti_mesh_length")
         self.oufti_mesh_length.addItem("")
         self.oufti_mesh_length.addItem("")
         self.oufti_mesh_length.addItem("")
         self.oufti_mesh_length.addItem("")
         self.oufti_mesh_length.addItem("")
         self.oufti_mesh_length.addItem("")
-        self.formLayout_7.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.oufti_mesh_length)
+        self.formLayout_7.setWidget(
+            0, QtWidgets.QFormLayout.FieldRole, self.oufti_mesh_length
+        )
         self.label_13 = QtWidgets.QLabel(self.tab_2)
         self.label_13.setObjectName("label_13")
-        self.formLayout_7.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.label_13)
+        self.formLayout_7.setWidget(
+            1, QtWidgets.QFormLayout.LabelRole, self.label_13
+        )
         self.oufti_mesh_dilation = QtWidgets.QComboBox(self.tab_2)
         self.oufti_mesh_dilation.setEditable(True)
         self.oufti_mesh_dilation.setObjectName("oufti_mesh_dilation")
         self.oufti_mesh_dilation.addItem("")
         self.oufti_mesh_dilation.addItem("")
         self.oufti_mesh_dilation.addItem("")
         self.oufti_mesh_dilation.addItem("")
@@ -1033,17 +1318,24 @@
         self.oufti_mesh_dilation.addItem("")
         self.oufti_mesh_dilation.addItem("")
         self.oufti_mesh_dilation.addItem("")
         self.oufti_mesh_dilation.addItem("")
         self.oufti_mesh_dilation.addItem("")
         self.oufti_mesh_dilation.addItem("")
         self.oufti_mesh_dilation.addItem("")
-        self.formLayout_7.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.oufti_mesh_dilation)
+        self.formLayout_7.setWidget(
+            1, QtWidgets.QFormLayout.FieldRole, self.oufti_mesh_dilation
+        )
         self.verticalLayout_7.addLayout(self.formLayout_7)
-        spacerItem27 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        spacerItem27 = QtWidgets.QSpacerItem(
+            20,
+            40,
+            QtWidgets.QSizePolicy.Minimum,
+            QtWidgets.QSizePolicy.Expanding,
+        )
         self.verticalLayout_7.addItem(spacerItem27)
         tab_widget.addTab(self.tab_2, "")
         self.upload_tab = QtWidgets.QWidget()
         self.upload_tab.setEnabled(True)
         self.upload_tab.setObjectName("upload_tab")
         self.verticalLayout_4 = QtWidgets.QVBoxLayout(self.upload_tab)
         self.verticalLayout_4.setObjectName("verticalLayout_4")
@@ -1068,30 +1360,47 @@
         self.load_database = QtWidgets.QPushButton(self.upload_tab)
         self.load_database.setObjectName("load_database")
         self.gridLayout_13.addWidget(self.load_database, 0, 1, 1, 1)
         self.verticalLayout_4.addLayout(self.gridLayout_13)
         self.formLayout_9 = QtWidgets.QFormLayout()
         self.formLayout_9.setObjectName("formLayout_9")
         self.display_database_path_label = QtWidgets.QLabel(self.upload_tab)
-        self.display_database_path_label.setObjectName("display_database_path_label")
-        self.formLayout_9.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.display_database_path_label)
+        self.display_database_path_label.setObjectName(
+            "display_database_path_label"
+        )
+        self.formLayout_9.setWidget(
+            0,
+            QtWidgets.QFormLayout.LabelRole,
+            self.display_database_path_label,
+        )
         self.display_database_path = QtWidgets.QLineEdit(self.upload_tab)
         self.display_database_path.setAlignment(QtCore.Qt.AlignCenter)
         self.display_database_path.setReadOnly(True)
         self.display_database_path.setClearButtonEnabled(False)
         self.display_database_path.setObjectName("display_database_path")
-        self.formLayout_9.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.display_database_path)
+        self.formLayout_9.setWidget(
+            0, QtWidgets.QFormLayout.FieldRole, self.display_database_path
+        )
         self.verticalLayout_4.addLayout(self.formLayout_9)
-        spacerItem28 = QtWidgets.QSpacerItem(435, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        spacerItem28 = QtWidgets.QSpacerItem(
+            435,
+            20,
+            QtWidgets.QSizePolicy.Minimum,
+            QtWidgets.QSizePolicy.Minimum,
+        )
         self.verticalLayout_4.addItem(spacerItem28)
         self.metadata_controls = QtWidgets.QTabWidget(self.upload_tab)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Preferred)
+        sizePolicy = QtWidgets.QSizePolicy(
+            QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Preferred
+        )
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
-        sizePolicy.setHeightForWidth(self.metadata_controls.sizePolicy().hasHeightForWidth())
+        sizePolicy.setHeightForWidth(
+            self.metadata_controls.sizePolicy().hasHeightForWidth()
+        )
         self.metadata_controls.setSizePolicy(sizePolicy)
         font = QtGui.QFont()
         font.setPointSize(10)
         font.setBold(False)
         font.setWeight(50)
         self.metadata_controls.setFont(font)
         self.metadata_controls.setObjectName("metadata_controls")
@@ -1099,129 +1408,179 @@
         self.experiment_metadata.setObjectName("experiment_metadata")
         self.verticalLayout_9 = QtWidgets.QVBoxLayout(self.experiment_metadata)
         self.verticalLayout_9.setObjectName("verticalLayout_9")
         self.image_metadata_controls = QtWidgets.QFormLayout()
         self.image_metadata_controls.setObjectName("image_metadata_controls")
         self.label_65 = QtWidgets.QLabel(self.experiment_metadata)
         self.label_65.setObjectName("label_65")
-        self.image_metadata_controls.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_65)
+        self.image_metadata_controls.setWidget(
+            0, QtWidgets.QFormLayout.LabelRole, self.label_65
+        )
         self.upload_initial = QtWidgets.QComboBox(self.experiment_metadata)
         self.upload_initial.setEnabled(True)
         self.upload_initial.setStyleSheet("background-color: rgb(191, 0, 0);")
         self.upload_initial.setEditable(True)
         self.upload_initial.setObjectName("upload_initial")
         self.upload_initial.addItem("")
-        self.image_metadata_controls.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.upload_initial)
+        self.image_metadata_controls.setWidget(
+            0, QtWidgets.QFormLayout.FieldRole, self.upload_initial
+        )
         self.label_74 = QtWidgets.QLabel(self.experiment_metadata)
         self.label_74.setObjectName("label_74")
-        self.image_metadata_controls.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.label_74)
+        self.image_metadata_controls.setWidget(
+            1, QtWidgets.QFormLayout.LabelRole, self.label_74
+        )
         self.upload_content = QtWidgets.QComboBox(self.experiment_metadata)
         self.upload_content.setEnabled(True)
         self.upload_content.setStyleSheet("background-color: rgb(191, 0, 0);")
         self.upload_content.setEditable(True)
         self.upload_content.setObjectName("upload_content")
         self.upload_content.addItem("")
-        self.image_metadata_controls.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.upload_content)
+        self.image_metadata_controls.setWidget(
+            1, QtWidgets.QFormLayout.FieldRole, self.upload_content
+        )
         self.label_75 = QtWidgets.QLabel(self.experiment_metadata)
         self.label_75.setObjectName("label_75")
-        self.image_metadata_controls.setWidget(2, QtWidgets.QFormLayout.LabelRole, self.label_75)
+        self.image_metadata_controls.setWidget(
+            2, QtWidgets.QFormLayout.LabelRole, self.label_75
+        )
         self.upload_microscope = QtWidgets.QComboBox(self.experiment_metadata)
         self.upload_microscope.setEnabled(True)
-        self.upload_microscope.setStyleSheet("background-color: rgb(191, 0, 0);")
+        self.upload_microscope.setStyleSheet(
+            "background-color: rgb(191, 0, 0);"
+        )
         self.upload_microscope.setEditable(True)
         self.upload_microscope.setObjectName("upload_microscope")
         self.upload_microscope.addItem("")
-        self.image_metadata_controls.setWidget(2, QtWidgets.QFormLayout.FieldRole, self.upload_microscope)
+        self.image_metadata_controls.setWidget(
+            2, QtWidgets.QFormLayout.FieldRole, self.upload_microscope
+        )
         self.label_76 = QtWidgets.QLabel(self.experiment_metadata)
         self.label_76.setObjectName("label_76")
-        self.image_metadata_controls.setWidget(5, QtWidgets.QFormLayout.LabelRole, self.label_76)
+        self.image_metadata_controls.setWidget(
+            5, QtWidgets.QFormLayout.LabelRole, self.label_76
+        )
         self.upload_antibiotic = QtWidgets.QComboBox(self.experiment_metadata)
         self.upload_antibiotic.setEnabled(True)
         self.upload_antibiotic.setEditable(True)
         self.upload_antibiotic.setObjectName("upload_antibiotic")
-        self.image_metadata_controls.setWidget(5, QtWidgets.QFormLayout.FieldRole, self.upload_antibiotic)
+        self.image_metadata_controls.setWidget(
+            5, QtWidgets.QFormLayout.FieldRole, self.upload_antibiotic
+        )
         self.label_77 = QtWidgets.QLabel(self.experiment_metadata)
         self.label_77.setObjectName("label_77")
-        self.image_metadata_controls.setWidget(6, QtWidgets.QFormLayout.LabelRole, self.label_77)
-        self.upload_treatmenttime = QtWidgets.QComboBox(self.experiment_metadata)
+        self.image_metadata_controls.setWidget(
+            6, QtWidgets.QFormLayout.LabelRole, self.label_77
+        )
+        self.upload_treatmenttime = QtWidgets.QComboBox(
+            self.experiment_metadata
+        )
         self.upload_treatmenttime.setEnabled(True)
         self.upload_treatmenttime.setEditable(True)
         self.upload_treatmenttime.setObjectName("upload_treatmenttime")
         self.upload_treatmenttime.addItem("")
         self.upload_treatmenttime.setItemText(0, "")
-        self.image_metadata_controls.setWidget(6, QtWidgets.QFormLayout.FieldRole, self.upload_treatmenttime)
+        self.image_metadata_controls.setWidget(
+            6, QtWidgets.QFormLayout.FieldRole, self.upload_treatmenttime
+        )
         self.label_78 = QtWidgets.QLabel(self.experiment_metadata)
         self.label_78.setObjectName("label_78")
-        self.image_metadata_controls.setWidget(7, QtWidgets.QFormLayout.LabelRole, self.label_78)
-        self.upload_abxconcentration = QtWidgets.QComboBox(self.experiment_metadata)
+        self.image_metadata_controls.setWidget(
+            7, QtWidgets.QFormLayout.LabelRole, self.label_78
+        )
+        self.upload_abxconcentration = QtWidgets.QComboBox(
+            self.experiment_metadata
+        )
         self.upload_abxconcentration.setEnabled(True)
         self.upload_abxconcentration.setEditable(True)
         self.upload_abxconcentration.setObjectName("upload_abxconcentration")
-        self.image_metadata_controls.setWidget(7, QtWidgets.QFormLayout.FieldRole, self.upload_abxconcentration)
+        self.image_metadata_controls.setWidget(
+            7, QtWidgets.QFormLayout.FieldRole, self.upload_abxconcentration
+        )
         self.label_79 = QtWidgets.QLabel(self.experiment_metadata)
         self.label_79.setObjectName("label_79")
-        self.image_metadata_controls.setWidget(8, QtWidgets.QFormLayout.LabelRole, self.label_79)
+        self.image_metadata_controls.setWidget(
+            8, QtWidgets.QFormLayout.LabelRole, self.label_79
+        )
         self.upload_mount = QtWidgets.QComboBox(self.experiment_metadata)
         self.upload_mount.setEnabled(True)
         self.upload_mount.setEditable(True)
         self.upload_mount.setObjectName("upload_mount")
         self.upload_mount.addItem("")
         self.upload_mount.setItemText(0, "")
         self.upload_mount.addItem("")
         self.upload_mount.addItem("")
-        self.image_metadata_controls.setWidget(8, QtWidgets.QFormLayout.FieldRole, self.upload_mount)
+        self.image_metadata_controls.setWidget(
+            8, QtWidgets.QFormLayout.FieldRole, self.upload_mount
+        )
         self.label_80 = QtWidgets.QLabel(self.experiment_metadata)
         self.label_80.setObjectName("label_80")
-        self.image_metadata_controls.setWidget(9, QtWidgets.QFormLayout.LabelRole, self.label_80)
+        self.image_metadata_controls.setWidget(
+            9, QtWidgets.QFormLayout.LabelRole, self.label_80
+        )
         self.upload_protocol = QtWidgets.QComboBox(self.experiment_metadata)
         self.upload_protocol.setEnabled(True)
         self.upload_protocol.setEditable(True)
         self.upload_protocol.setObjectName("upload_protocol")
         self.upload_protocol.addItem("")
         self.upload_protocol.setItemText(0, "")
-        self.image_metadata_controls.setWidget(9, QtWidgets.QFormLayout.FieldRole, self.upload_protocol)
+        self.image_metadata_controls.setWidget(
+            9, QtWidgets.QFormLayout.FieldRole, self.upload_protocol
+        )
         self.upload_phenotype = QtWidgets.QComboBox(self.experiment_metadata)
         self.upload_phenotype.setEditable(True)
         self.upload_phenotype.setObjectName("upload_phenotype")
         self.upload_phenotype.addItem("")
         self.upload_phenotype.setItemText(0, "")
         self.upload_phenotype.addItem("")
         self.upload_phenotype.addItem("")
         self.upload_phenotype.addItem("")
         self.upload_phenotype.addItem("")
-        self.image_metadata_controls.setWidget(4, QtWidgets.QFormLayout.FieldRole, self.upload_phenotype)
+        self.image_metadata_controls.setWidget(
+            4, QtWidgets.QFormLayout.FieldRole, self.upload_phenotype
+        )
         self.label_41 = QtWidgets.QLabel(self.experiment_metadata)
         self.label_41.setObjectName("label_41")
-        self.image_metadata_controls.setWidget(4, QtWidgets.QFormLayout.LabelRole, self.label_41)
+        self.image_metadata_controls.setWidget(
+            4, QtWidgets.QFormLayout.LabelRole, self.label_41
+        )
         self.label_42 = QtWidgets.QLabel(self.experiment_metadata)
         self.label_42.setObjectName("label_42")
-        self.image_metadata_controls.setWidget(3, QtWidgets.QFormLayout.LabelRole, self.label_42)
+        self.image_metadata_controls.setWidget(
+            3, QtWidgets.QFormLayout.LabelRole, self.label_42
+        )
         self.upload_strain = QtWidgets.QComboBox(self.experiment_metadata)
         self.upload_strain.setEditable(True)
         self.upload_strain.setObjectName("upload_strain")
         self.upload_strain.addItem("")
         self.upload_strain.setItemText(0, "")
         self.upload_strain.addItem("")
-        self.image_metadata_controls.setWidget(3, QtWidgets.QFormLayout.FieldRole, self.upload_strain)
+        self.image_metadata_controls.setWidget(
+            3, QtWidgets.QFormLayout.FieldRole, self.upload_strain
+        )
         self.verticalLayout_9.addLayout(self.image_metadata_controls)
         self.metadata_controls.addTab(self.experiment_metadata, "")
         self.image_metadata = QtWidgets.QWidget()
         self.image_metadata.setObjectName("image_metadata")
         self.verticalLayout_8 = QtWidgets.QVBoxLayout(self.image_metadata)
         self.verticalLayout_8.setObjectName("verticalLayout_8")
         self.formLayout_10 = QtWidgets.QFormLayout()
         self.formLayout_10.setObjectName("formLayout_10")
         self.label_67 = QtWidgets.QLabel(self.image_metadata)
         self.label_67.setObjectName("label_67")
-        self.formLayout_10.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_67)
+        self.formLayout_10.setWidget(
+            0, QtWidgets.QFormLayout.LabelRole, self.label_67
+        )
         self.label_modality = QtWidgets.QComboBox(self.image_metadata)
         palette = QtGui.QPalette()
         brush = QtGui.QBrush(QtGui.QColor(0, 0, 0))
         brush.setStyle(QtCore.Qt.SolidPattern)
-        palette.setBrush(QtGui.QPalette.Active, QtGui.QPalette.WindowText, brush)
+        palette.setBrush(
+            QtGui.QPalette.Active, QtGui.QPalette.WindowText, brush
+        )
         brush = QtGui.QBrush(QtGui.QColor(191, 0, 0))
         brush.setStyle(QtCore.Qt.SolidPattern)
         palette.setBrush(QtGui.QPalette.Active, QtGui.QPalette.Button, brush)
         brush = QtGui.QBrush(QtGui.QColor(255, 127, 127))
         brush.setStyle(QtCore.Qt.SolidPattern)
         palette.setBrush(QtGui.QPalette.Active, QtGui.QPalette.Light, brush)
         brush = QtGui.QBrush(QtGui.QColor(255, 63, 63))
@@ -1234,362 +1593,496 @@
         brush.setStyle(QtCore.Qt.SolidPattern)
         palette.setBrush(QtGui.QPalette.Active, QtGui.QPalette.Mid, brush)
         brush = QtGui.QBrush(QtGui.QColor(0, 0, 0))
         brush.setStyle(QtCore.Qt.SolidPattern)
         palette.setBrush(QtGui.QPalette.Active, QtGui.QPalette.Text, brush)
         brush = QtGui.QBrush(QtGui.QColor(255, 255, 255))
         brush.setStyle(QtCore.Qt.SolidPattern)
-        palette.setBrush(QtGui.QPalette.Active, QtGui.QPalette.BrightText, brush)
+        palette.setBrush(
+            QtGui.QPalette.Active, QtGui.QPalette.BrightText, brush
+        )
         brush = QtGui.QBrush(QtGui.QColor(0, 0, 0))
         brush.setStyle(QtCore.Qt.SolidPattern)
-        palette.setBrush(QtGui.QPalette.Active, QtGui.QPalette.ButtonText, brush)
+        palette.setBrush(
+            QtGui.QPalette.Active, QtGui.QPalette.ButtonText, brush
+        )
         brush = QtGui.QBrush(QtGui.QColor(191, 0, 0))
         brush.setStyle(QtCore.Qt.SolidPattern)
         palette.setBrush(QtGui.QPalette.Active, QtGui.QPalette.Base, brush)
         brush = QtGui.QBrush(QtGui.QColor(191, 0, 0))
         brush.setStyle(QtCore.Qt.SolidPattern)
         palette.setBrush(QtGui.QPalette.Active, QtGui.QPalette.Window, brush)
         brush = QtGui.QBrush(QtGui.QColor(0, 0, 0))
         brush.setStyle(QtCore.Qt.SolidPattern)
         palette.setBrush(QtGui.QPalette.Active, QtGui.QPalette.Shadow, brush)
         brush = QtGui.QBrush(QtGui.QColor(255, 127, 127))
         brush.setStyle(QtCore.Qt.SolidPattern)
-        palette.setBrush(QtGui.QPalette.Active, QtGui.QPalette.AlternateBase, brush)
+        palette.setBrush(
+            QtGui.QPalette.Active, QtGui.QPalette.AlternateBase, brush
+        )
         brush = QtGui.QBrush(QtGui.QColor(255, 255, 220))
         brush.setStyle(QtCore.Qt.SolidPattern)
-        palette.setBrush(QtGui.QPalette.Active, QtGui.QPalette.ToolTipBase, brush)
+        palette.setBrush(
+            QtGui.QPalette.Active, QtGui.QPalette.ToolTipBase, brush
+        )
         brush = QtGui.QBrush(QtGui.QColor(0, 0, 0))
         brush.setStyle(QtCore.Qt.SolidPattern)
-        palette.setBrush(QtGui.QPalette.Active, QtGui.QPalette.ToolTipText, brush)
+        palette.setBrush(
+            QtGui.QPalette.Active, QtGui.QPalette.ToolTipText, brush
+        )
         brush = QtGui.QBrush(QtGui.QColor(0, 0, 0, 128))
         brush.setStyle(QtCore.Qt.SolidPattern)
-        palette.setBrush(QtGui.QPalette.Active, QtGui.QPalette.PlaceholderText, brush)
+        palette.setBrush(
+            QtGui.QPalette.Active, QtGui.QPalette.PlaceholderText, brush
+        )
         brush = QtGui.QBrush(QtGui.QColor(0, 0, 0))
         brush.setStyle(QtCore.Qt.SolidPattern)
-        palette.setBrush(QtGui.QPalette.Inactive, QtGui.QPalette.WindowText, brush)
+        palette.setBrush(
+            QtGui.QPalette.Inactive, QtGui.QPalette.WindowText, brush
+        )
         brush = QtGui.QBrush(QtGui.QColor(191, 0, 0))
         brush.setStyle(QtCore.Qt.SolidPattern)
         palette.setBrush(QtGui.QPalette.Inactive, QtGui.QPalette.Button, brush)
         brush = QtGui.QBrush(QtGui.QColor(255, 127, 127))
         brush.setStyle(QtCore.Qt.SolidPattern)
         palette.setBrush(QtGui.QPalette.Inactive, QtGui.QPalette.Light, brush)
         brush = QtGui.QBrush(QtGui.QColor(255, 63, 63))
         brush.setStyle(QtCore.Qt.SolidPattern)
-        palette.setBrush(QtGui.QPalette.Inactive, QtGui.QPalette.Midlight, brush)
+        palette.setBrush(
+            QtGui.QPalette.Inactive, QtGui.QPalette.Midlight, brush
+        )
         brush = QtGui.QBrush(QtGui.QColor(127, 0, 0))
         brush.setStyle(QtCore.Qt.SolidPattern)
         palette.setBrush(QtGui.QPalette.Inactive, QtGui.QPalette.Dark, brush)
         brush = QtGui.QBrush(QtGui.QColor(170, 0, 0))
         brush.setStyle(QtCore.Qt.SolidPattern)
         palette.setBrush(QtGui.QPalette.Inactive, QtGui.QPalette.Mid, brush)
         brush = QtGui.QBrush(QtGui.QColor(0, 0, 0))
         brush.setStyle(QtCore.Qt.SolidPattern)
         palette.setBrush(QtGui.QPalette.Inactive, QtGui.QPalette.Text, brush)
         brush = QtGui.QBrush(QtGui.QColor(255, 255, 255))
         brush.setStyle(QtCore.Qt.SolidPattern)
-        palette.setBrush(QtGui.QPalette.Inactive, QtGui.QPalette.BrightText, brush)
+        palette.setBrush(
+            QtGui.QPalette.Inactive, QtGui.QPalette.BrightText, brush
+        )
         brush = QtGui.QBrush(QtGui.QColor(0, 0, 0))
         brush.setStyle(QtCore.Qt.SolidPattern)
-        palette.setBrush(QtGui.QPalette.Inactive, QtGui.QPalette.ButtonText, brush)
+        palette.setBrush(
+            QtGui.QPalette.Inactive, QtGui.QPalette.ButtonText, brush
+        )
         brush = QtGui.QBrush(QtGui.QColor(191, 0, 0))
         brush.setStyle(QtCore.Qt.SolidPattern)
         palette.setBrush(QtGui.QPalette.Inactive, QtGui.QPalette.Base, brush)
         brush = QtGui.QBrush(QtGui.QColor(191, 0, 0))
         brush.setStyle(QtCore.Qt.SolidPattern)
         palette.setBrush(QtGui.QPalette.Inactive, QtGui.QPalette.Window, brush)
         brush = QtGui.QBrush(QtGui.QColor(0, 0, 0))
         brush.setStyle(QtCore.Qt.SolidPattern)
         palette.setBrush(QtGui.QPalette.Inactive, QtGui.QPalette.Shadow, brush)
         brush = QtGui.QBrush(QtGui.QColor(255, 127, 127))
         brush.setStyle(QtCore.Qt.SolidPattern)
-        palette.setBrush(QtGui.QPalette.Inactive, QtGui.QPalette.AlternateBase, brush)
+        palette.setBrush(
+            QtGui.QPalette.Inactive, QtGui.QPalette.AlternateBase, brush
+        )
         brush = QtGui.QBrush(QtGui.QColor(255, 255, 220))
         brush.setStyle(QtCore.Qt.SolidPattern)
-        palette.setBrush(QtGui.QPalette.Inactive, QtGui.QPalette.ToolTipBase, brush)
+        palette.setBrush(
+            QtGui.QPalette.Inactive, QtGui.QPalette.ToolTipBase, brush
+        )
         brush = QtGui.QBrush(QtGui.QColor(0, 0, 0))
         brush.setStyle(QtCore.Qt.SolidPattern)
-        palette.setBrush(QtGui.QPalette.Inactive, QtGui.QPalette.ToolTipText, brush)
+        palette.setBrush(
+            QtGui.QPalette.Inactive, QtGui.QPalette.ToolTipText, brush
+        )
         brush = QtGui.QBrush(QtGui.QColor(0, 0, 0, 128))
         brush.setStyle(QtCore.Qt.SolidPattern)
-        palette.setBrush(QtGui.QPalette.Inactive, QtGui.QPalette.PlaceholderText, brush)
+        palette.setBrush(
+            QtGui.QPalette.Inactive, QtGui.QPalette.PlaceholderText, brush
+        )
         brush = QtGui.QBrush(QtGui.QColor(127, 0, 0))
         brush.setStyle(QtCore.Qt.SolidPattern)
-        palette.setBrush(QtGui.QPalette.Disabled, QtGui.QPalette.WindowText, brush)
+        palette.setBrush(
+            QtGui.QPalette.Disabled, QtGui.QPalette.WindowText, brush
+        )
         brush = QtGui.QBrush(QtGui.QColor(191, 0, 0))
         brush.setStyle(QtCore.Qt.SolidPattern)
         palette.setBrush(QtGui.QPalette.Disabled, QtGui.QPalette.Button, brush)
         brush = QtGui.QBrush(QtGui.QColor(255, 127, 127))
         brush.setStyle(QtCore.Qt.SolidPattern)
         palette.setBrush(QtGui.QPalette.Disabled, QtGui.QPalette.Light, brush)
         brush = QtGui.QBrush(QtGui.QColor(255, 63, 63))
         brush.setStyle(QtCore.Qt.SolidPattern)
-        palette.setBrush(QtGui.QPalette.Disabled, QtGui.QPalette.Midlight, brush)
+        palette.setBrush(
+            QtGui.QPalette.Disabled, QtGui.QPalette.Midlight, brush
+        )
         brush = QtGui.QBrush(QtGui.QColor(127, 0, 0))
         brush.setStyle(QtCore.Qt.SolidPattern)
         palette.setBrush(QtGui.QPalette.Disabled, QtGui.QPalette.Dark, brush)
         brush = QtGui.QBrush(QtGui.QColor(170, 0, 0))
         brush.setStyle(QtCore.Qt.SolidPattern)
         palette.setBrush(QtGui.QPalette.Disabled, QtGui.QPalette.Mid, brush)
         brush = QtGui.QBrush(QtGui.QColor(127, 0, 0))
         brush.setStyle(QtCore.Qt.SolidPattern)
         palette.setBrush(QtGui.QPalette.Disabled, QtGui.QPalette.Text, brush)
         brush = QtGui.QBrush(QtGui.QColor(255, 255, 255))
         brush.setStyle(QtCore.Qt.SolidPattern)
-        palette.setBrush(QtGui.QPalette.Disabled, QtGui.QPalette.BrightText, brush)
+        palette.setBrush(
+            QtGui.QPalette.Disabled, QtGui.QPalette.BrightText, brush
+        )
         brush = QtGui.QBrush(QtGui.QColor(127, 0, 0))
         brush.setStyle(QtCore.Qt.SolidPattern)
-        palette.setBrush(QtGui.QPalette.Disabled, QtGui.QPalette.ButtonText, brush)
+        palette.setBrush(
+            QtGui.QPalette.Disabled, QtGui.QPalette.ButtonText, brush
+        )
         brush = QtGui.QBrush(QtGui.QColor(191, 0, 0))
         brush.setStyle(QtCore.Qt.SolidPattern)
         palette.setBrush(QtGui.QPalette.Disabled, QtGui.QPalette.Base, brush)
         brush = QtGui.QBrush(QtGui.QColor(191, 0, 0))
         brush.setStyle(QtCore.Qt.SolidPattern)
         palette.setBrush(QtGui.QPalette.Disabled, QtGui.QPalette.Window, brush)
         brush = QtGui.QBrush(QtGui.QColor(0, 0, 0))
         brush.setStyle(QtCore.Qt.SolidPattern)
         palette.setBrush(QtGui.QPalette.Disabled, QtGui.QPalette.Shadow, brush)
         brush = QtGui.QBrush(QtGui.QColor(255, 0, 0))
         brush.setStyle(QtCore.Qt.SolidPattern)
-        palette.setBrush(QtGui.QPalette.Disabled, QtGui.QPalette.AlternateBase, brush)
+        palette.setBrush(
+            QtGui.QPalette.Disabled, QtGui.QPalette.AlternateBase, brush
+        )
         brush = QtGui.QBrush(QtGui.QColor(255, 255, 220))
         brush.setStyle(QtCore.Qt.SolidPattern)
-        palette.setBrush(QtGui.QPalette.Disabled, QtGui.QPalette.ToolTipBase, brush)
+        palette.setBrush(
+            QtGui.QPalette.Disabled, QtGui.QPalette.ToolTipBase, brush
+        )
         brush = QtGui.QBrush(QtGui.QColor(0, 0, 0))
         brush.setStyle(QtCore.Qt.SolidPattern)
-        palette.setBrush(QtGui.QPalette.Disabled, QtGui.QPalette.ToolTipText, brush)
+        palette.setBrush(
+            QtGui.QPalette.Disabled, QtGui.QPalette.ToolTipText, brush
+        )
         brush = QtGui.QBrush(QtGui.QColor(0, 0, 0, 128))
         brush.setStyle(QtCore.Qt.SolidPattern)
-        palette.setBrush(QtGui.QPalette.Disabled, QtGui.QPalette.PlaceholderText, brush)
+        palette.setBrush(
+            QtGui.QPalette.Disabled, QtGui.QPalette.PlaceholderText, brush
+        )
         self.label_modality.setPalette(palette)
         self.label_modality.setStyleSheet("background-color: rgb(191, 0, 0);")
         self.label_modality.setEditable(True)
         self.label_modality.setObjectName("label_modality")
         self.label_modality.addItem("")
         self.label_modality.addItem("")
         self.label_modality.addItem("")
         self.label_modality.addItem("")
         self.label_modality.addItem("")
         self.label_modality.addItem("")
         self.label_modality.addItem("")
         self.label_modality.addItem("")
-        self.formLayout_10.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.label_modality)
+        self.formLayout_10.setWidget(
+            0, QtWidgets.QFormLayout.FieldRole, self.label_modality
+        )
         self.label_66 = QtWidgets.QLabel(self.image_metadata)
         self.label_66.setObjectName("label_66")
-        self.formLayout_10.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.label_66)
+        self.formLayout_10.setWidget(
+            1, QtWidgets.QFormLayout.LabelRole, self.label_66
+        )
         self.label_light_source = QtWidgets.QComboBox(self.image_metadata)
-        self.label_light_source.setStyleSheet("background-color: rgb(191, 0, 0);")
+        self.label_light_source.setStyleSheet(
+            "background-color: rgb(191, 0, 0);"
+        )
         self.label_light_source.setEditable(True)
         self.label_light_source.setObjectName("label_light_source")
         self.label_light_source.addItem("")
         self.label_light_source.addItem("")
         self.label_light_source.setItemText(1, "")
         self.label_light_source.addItem("")
         self.label_light_source.addItem("")
         self.label_light_source.addItem("")
         self.label_light_source.addItem("")
         self.label_light_source.addItem("")
         self.label_light_source.addItem("")
         self.label_light_source.addItem("")
-        self.formLayout_10.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.label_light_source)
+        self.formLayout_10.setWidget(
+            1, QtWidgets.QFormLayout.FieldRole, self.label_light_source
+        )
         self.label_68 = QtWidgets.QLabel(self.image_metadata)
         self.label_68.setObjectName("label_68")
-        self.formLayout_10.setWidget(2, QtWidgets.QFormLayout.LabelRole, self.label_68)
+        self.formLayout_10.setWidget(
+            2, QtWidgets.QFormLayout.LabelRole, self.label_68
+        )
         self.label_stain = QtWidgets.QComboBox(self.image_metadata)
         self.label_stain.setStyleSheet("background-color: rgb(191, 0, 0);")
         self.label_stain.setEditable(True)
         self.label_stain.setObjectName("label_stain")
         self.label_stain.addItem("")
         self.label_stain.addItem("")
         self.label_stain.setItemText(1, "")
         self.label_stain.addItem("")
         self.label_stain.addItem("")
         self.label_stain.addItem("")
         self.label_stain.addItem("")
         self.label_stain.addItem("")
         self.label_stain.addItem("")
         self.label_stain.addItem("")
-        self.formLayout_10.setWidget(2, QtWidgets.QFormLayout.FieldRole, self.label_stain)
+        self.formLayout_10.setWidget(
+            2, QtWidgets.QFormLayout.FieldRole, self.label_stain
+        )
         self.label_69 = QtWidgets.QLabel(self.image_metadata)
         self.label_69.setObjectName("label_69")
-        self.formLayout_10.setWidget(3, QtWidgets.QFormLayout.LabelRole, self.label_69)
+        self.formLayout_10.setWidget(
+            3, QtWidgets.QFormLayout.LabelRole, self.label_69
+        )
         self.label_stain_target = QtWidgets.QComboBox(self.image_metadata)
-        self.label_stain_target.setStyleSheet("background-color: rgb(191, 0, 0);")
+        self.label_stain_target.setStyleSheet(
+            "background-color: rgb(191, 0, 0);"
+        )
         self.label_stain_target.setEditable(True)
         self.label_stain_target.setObjectName("label_stain_target")
         self.label_stain_target.addItem("")
         self.label_stain_target.addItem("")
         self.label_stain_target.setItemText(1, "")
         self.label_stain_target.addItem("")
         self.label_stain_target.addItem("")
         self.label_stain_target.addItem("")
-        self.formLayout_10.setWidget(3, QtWidgets.QFormLayout.FieldRole, self.label_stain_target)
+        self.formLayout_10.setWidget(
+            3, QtWidgets.QFormLayout.FieldRole, self.label_stain_target
+        )
         self.verticalLayout_8.addLayout(self.formLayout_10)
         self.label_overwrite = QtWidgets.QPushButton(self.image_metadata)
         self.label_overwrite.setObjectName("label_overwrite")
         self.verticalLayout_8.addWidget(self.label_overwrite)
-        spacerItem29 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        spacerItem29 = QtWidgets.QSpacerItem(
+            20,
+            40,
+            QtWidgets.QSizePolicy.Minimum,
+            QtWidgets.QSizePolicy.Expanding,
+        )
         self.verticalLayout_8.addItem(spacerItem29)
         self.metadata_controls.addTab(self.image_metadata, "")
         self.user_metadata = QtWidgets.QWidget()
         self.user_metadata.setObjectName("user_metadata")
         self.verticalLayout_19 = QtWidgets.QVBoxLayout(self.user_metadata)
         self.verticalLayout_19.setObjectName("verticalLayout_19")
         self.formLayout_2 = QtWidgets.QFormLayout()
         self.formLayout_2.setObjectName("formLayout_2")
         self.label_81 = QtWidgets.QLabel(self.user_metadata)
         self.label_81.setObjectName("label_81")
-        self.formLayout_2.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_81)
+        self.formLayout_2.setWidget(
+            0, QtWidgets.QFormLayout.LabelRole, self.label_81
+        )
         self.upload_usermeta1 = QtWidgets.QComboBox(self.user_metadata)
         self.upload_usermeta1.setEnabled(True)
         self.upload_usermeta1.setEditable(True)
         self.upload_usermeta1.setObjectName("upload_usermeta1")
-        self.formLayout_2.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.upload_usermeta1)
+        self.formLayout_2.setWidget(
+            0, QtWidgets.QFormLayout.FieldRole, self.upload_usermeta1
+        )
         self.label_82 = QtWidgets.QLabel(self.user_metadata)
         self.label_82.setObjectName("label_82")
-        self.formLayout_2.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.label_82)
+        self.formLayout_2.setWidget(
+            1, QtWidgets.QFormLayout.LabelRole, self.label_82
+        )
         self.upload_usermeta2 = QtWidgets.QComboBox(self.user_metadata)
         self.upload_usermeta2.setEnabled(True)
         self.upload_usermeta2.setEditable(True)
         self.upload_usermeta2.setObjectName("upload_usermeta2")
-        self.formLayout_2.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.upload_usermeta2)
+        self.formLayout_2.setWidget(
+            1, QtWidgets.QFormLayout.FieldRole, self.upload_usermeta2
+        )
         self.label_83 = QtWidgets.QLabel(self.user_metadata)
         self.label_83.setObjectName("label_83")
-        self.formLayout_2.setWidget(2, QtWidgets.QFormLayout.LabelRole, self.label_83)
+        self.formLayout_2.setWidget(
+            2, QtWidgets.QFormLayout.LabelRole, self.label_83
+        )
         self.upload_usermeta3 = QtWidgets.QComboBox(self.user_metadata)
         self.upload_usermeta3.setEnabled(True)
         self.upload_usermeta3.setEditable(True)
         self.upload_usermeta3.setObjectName("upload_usermeta3")
-        self.formLayout_2.setWidget(2, QtWidgets.QFormLayout.FieldRole, self.upload_usermeta3)
+        self.formLayout_2.setWidget(
+            2, QtWidgets.QFormLayout.FieldRole, self.upload_usermeta3
+        )
         self.label_91 = QtWidgets.QLabel(self.user_metadata)
         self.label_91.setObjectName("label_91")
-        self.formLayout_2.setWidget(3, QtWidgets.QFormLayout.LabelRole, self.label_91)
+        self.formLayout_2.setWidget(
+            3, QtWidgets.QFormLayout.LabelRole, self.label_91
+        )
         self.upload_usermeta4 = QtWidgets.QComboBox(self.user_metadata)
         self.upload_usermeta4.setEnabled(True)
         self.upload_usermeta4.setEditable(True)
         self.upload_usermeta4.setObjectName("upload_usermeta4")
-        self.formLayout_2.setWidget(3, QtWidgets.QFormLayout.FieldRole, self.upload_usermeta4)
+        self.formLayout_2.setWidget(
+            3, QtWidgets.QFormLayout.FieldRole, self.upload_usermeta4
+        )
         self.upload_usermeta5 = QtWidgets.QComboBox(self.user_metadata)
         self.upload_usermeta5.setEnabled(True)
         self.upload_usermeta5.setEditable(True)
         self.upload_usermeta5.setObjectName("upload_usermeta5")
-        self.formLayout_2.setWidget(4, QtWidgets.QFormLayout.FieldRole, self.upload_usermeta5)
+        self.formLayout_2.setWidget(
+            4, QtWidgets.QFormLayout.FieldRole, self.upload_usermeta5
+        )
         self.label_90 = QtWidgets.QLabel(self.user_metadata)
         self.label_90.setObjectName("label_90")
-        self.formLayout_2.setWidget(4, QtWidgets.QFormLayout.LabelRole, self.label_90)
+        self.formLayout_2.setWidget(
+            4, QtWidgets.QFormLayout.LabelRole, self.label_90
+        )
         self.label_92 = QtWidgets.QLabel(self.user_metadata)
         self.label_92.setObjectName("label_92")
-        self.formLayout_2.setWidget(5, QtWidgets.QFormLayout.LabelRole, self.label_92)
+        self.formLayout_2.setWidget(
+            5, QtWidgets.QFormLayout.LabelRole, self.label_92
+        )
         self.upload_usermeta6 = QtWidgets.QComboBox(self.user_metadata)
         self.upload_usermeta6.setEnabled(True)
         self.upload_usermeta6.setEditable(True)
         self.upload_usermeta6.setObjectName("upload_usermeta6")
-        self.formLayout_2.setWidget(5, QtWidgets.QFormLayout.FieldRole, self.upload_usermeta6)
+        self.formLayout_2.setWidget(
+            5, QtWidgets.QFormLayout.FieldRole, self.upload_usermeta6
+        )
         self.verticalLayout_19.addLayout(self.formLayout_2)
-        spacerItem30 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        spacerItem30 = QtWidgets.QSpacerItem(
+            20,
+            40,
+            QtWidgets.QSizePolicy.Minimum,
+            QtWidgets.QSizePolicy.Expanding,
+        )
         self.verticalLayout_19.addItem(spacerItem30)
         self.metadata_controls.addTab(self.user_metadata, "")
         self.verticalLayout_4.addWidget(self.metadata_controls)
         self.update_metadata = QtWidgets.QPushButton(self.upload_tab)
         self.update_metadata.setObjectName("update_metadata")
         self.verticalLayout_4.addWidget(self.update_metadata)
-        spacerItem31 = QtWidgets.QSpacerItem(435, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        spacerItem31 = QtWidgets.QSpacerItem(
+            435,
+            20,
+            QtWidgets.QSizePolicy.Minimum,
+            QtWidgets.QSizePolicy.Minimum,
+        )
         self.verticalLayout_4.addItem(spacerItem31)
         self.label_87 = QtWidgets.QLabel(self.upload_tab)
         font = QtGui.QFont()
         font.setPointSize(10)
         font.setBold(True)
         font.setWeight(75)
         self.label_87.setFont(font)
         self.label_87.setObjectName("label_87")
         self.verticalLayout_4.addWidget(self.label_87)
         self.formLayout_16 = QtWidgets.QFormLayout()
         self.formLayout_16.setObjectName("formLayout_16")
         self.label_85 = QtWidgets.QLabel(self.upload_tab)
         self.label_85.setObjectName("label_85")
-        self.formLayout_16.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_85)
+        self.formLayout_16.setWidget(
+            0, QtWidgets.QFormLayout.LabelRole, self.label_85
+        )
         self.upload_segmentation_combo = QtWidgets.QComboBox(self.upload_tab)
-        self.upload_segmentation_combo.setObjectName("upload_segmentation_combo")
+        self.upload_segmentation_combo.setObjectName(
+            "upload_segmentation_combo"
+        )
         self.upload_segmentation_combo.addItem("")
         self.upload_segmentation_combo.setItemText(0, "")
         self.upload_segmentation_combo.addItem("")
         self.upload_segmentation_combo.addItem("")
         self.upload_segmentation_combo.addItem("")
-        self.formLayout_16.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.upload_segmentation_combo)
+        self.formLayout_16.setWidget(
+            0, QtWidgets.QFormLayout.FieldRole, self.upload_segmentation_combo
+        )
         self.label_84 = QtWidgets.QLabel(self.upload_tab)
         self.label_84.setObjectName("label_84")
-        self.formLayout_16.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.label_84)
+        self.formLayout_16.setWidget(
+            1, QtWidgets.QFormLayout.LabelRole, self.label_84
+        )
         self.upload_label_combo = QtWidgets.QComboBox(self.upload_tab)
         self.upload_label_combo.setObjectName("upload_label_combo")
         self.upload_label_combo.addItem("")
         self.upload_label_combo.setItemText(0, "")
         self.upload_label_combo.addItem("")
         self.upload_label_combo.addItem("")
         self.upload_label_combo.addItem("")
-        self.formLayout_16.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.upload_label_combo)
+        self.formLayout_16.setWidget(
+            1, QtWidgets.QFormLayout.FieldRole, self.upload_label_combo
+        )
         self.verticalLayout_4.addLayout(self.formLayout_16)
-        spacerItem32 = QtWidgets.QSpacerItem(435, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        spacerItem32 = QtWidgets.QSpacerItem(
+            435,
+            20,
+            QtWidgets.QSizePolicy.Minimum,
+            QtWidgets.QSizePolicy.Minimum,
+        )
         self.verticalLayout_4.addItem(spacerItem32)
         self.tabWidget_2 = QtWidgets.QTabWidget(self.upload_tab)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Preferred)
+        sizePolicy = QtWidgets.QSizePolicy(
+            QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Preferred
+        )
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
-        sizePolicy.setHeightForWidth(self.tabWidget_2.sizePolicy().hasHeightForWidth())
+        sizePolicy.setHeightForWidth(
+            self.tabWidget_2.sizePolicy().hasHeightForWidth()
+        )
         self.tabWidget_2.setSizePolicy(sizePolicy)
         self.tabWidget_2.setMaximumSize(QtCore.QSize(16777215, 500))
         self.tabWidget_2.setObjectName("tabWidget_2")
         self.tab_10 = QtWidgets.QWidget()
         self.tab_10.setObjectName("tab_10")
         self.verticalLayout_12 = QtWidgets.QVBoxLayout(self.tab_10)
         self.verticalLayout_12.setObjectName("verticalLayout_12")
         self.database_download_buttons_2 = QtWidgets.QGridLayout()
-        self.database_download_buttons_2.setObjectName("database_download_buttons_2")
+        self.database_download_buttons_2.setObjectName(
+            "database_download_buttons_2"
+        )
         self.download_sort_order_2 = QtWidgets.QComboBox(self.tab_10)
         self.download_sort_order_2.setObjectName("download_sort_order_2")
         self.download_sort_order_2.addItem("")
         self.download_sort_order_2.setItemText(0, "")
         self.download_sort_order_2.addItem("")
         self.download_sort_order_2.addItem("")
         self.download_sort_order_2.addItem("")
         self.download_sort_order_2.addItem("")
         self.download_sort_order_2.addItem("")
         self.download_sort_order_2.addItem("")
         self.download_sort_order_2.addItem("")
-        self.database_download_buttons_2.addWidget(self.download_sort_order_2, 1, 1, 1, 1)
+        self.database_download_buttons_2.addWidget(
+            self.download_sort_order_2, 1, 1, 1, 1
+        )
         self.label_15 = QtWidgets.QLabel(self.tab_10)
         self.label_15.setObjectName("label_15")
         self.database_download_buttons_2.addWidget(self.label_15, 0, 0, 1, 1)
         self.download_sort_direction_1 = QtWidgets.QComboBox(self.tab_10)
-        self.download_sort_direction_1.setObjectName("download_sort_direction_1")
+        self.download_sort_direction_1.setObjectName(
+            "download_sort_direction_1"
+        )
         self.download_sort_direction_1.addItem("")
         self.download_sort_direction_1.setItemText(0, "")
         self.download_sort_direction_1.addItem("")
         self.download_sort_direction_1.addItem("")
-        self.database_download_buttons_2.addWidget(self.download_sort_direction_1, 0, 2, 1, 1)
+        self.database_download_buttons_2.addWidget(
+            self.download_sort_direction_1, 0, 2, 1, 1
+        )
         self.download_sort_order_1 = QtWidgets.QComboBox(self.tab_10)
         self.download_sort_order_1.setObjectName("download_sort_order_1")
         self.download_sort_order_1.addItem("")
         self.download_sort_order_1.setItemText(0, "")
         self.download_sort_order_1.addItem("")
         self.download_sort_order_1.addItem("")
         self.download_sort_order_1.addItem("")
         self.download_sort_order_1.addItem("")
         self.download_sort_order_1.addItem("")
         self.download_sort_order_1.addItem("")
         self.download_sort_order_1.addItem("")
-        self.database_download_buttons_2.addWidget(self.download_sort_order_1, 0, 1, 1, 1)
+        self.database_download_buttons_2.addWidget(
+            self.download_sort_order_1, 0, 1, 1, 1
+        )
         self.label_23 = QtWidgets.QLabel(self.tab_10)
         self.label_23.setObjectName("label_23")
         self.database_download_buttons_2.addWidget(self.label_23, 1, 0, 1, 1)
         self.download_sort_direction_2 = QtWidgets.QComboBox(self.tab_10)
-        self.download_sort_direction_2.setObjectName("download_sort_direction_2")
+        self.download_sort_direction_2.setObjectName(
+            "download_sort_direction_2"
+        )
         self.download_sort_direction_2.addItem("")
         self.download_sort_direction_2.setItemText(0, "")
         self.download_sort_direction_2.addItem("")
         self.download_sort_direction_2.addItem("")
-        self.database_download_buttons_2.addWidget(self.download_sort_direction_2, 1, 2, 1, 1)
+        self.database_download_buttons_2.addWidget(
+            self.download_sort_direction_2, 1, 2, 1, 1
+        )
         self.verticalLayout_12.addLayout(self.database_download_buttons_2)
         self.gridLayout_23 = QtWidgets.QGridLayout()
         self.gridLayout_23.setObjectName("gridLayout_23")
         self.label_88 = QtWidgets.QLabel(self.tab_10)
         self.label_88.setObjectName("label_88")
         self.gridLayout_23.addWidget(self.label_88, 0, 0, 1, 1)
         self.database_download_limit = QtWidgets.QComboBox(self.tab_10)
@@ -1623,16 +2116,20 @@
         self.label_24.setFont(font)
         self.label_24.setObjectName("label_24")
         self.verticalLayout_11.addWidget(self.label_24)
         self.gridLayout_24 = QtWidgets.QGridLayout()
         self.gridLayout_24.setObjectName("gridLayout_24")
         self.upload_segmentations_setting = QtWidgets.QCheckBox(self.tab_4)
         self.upload_segmentations_setting.setChecked(True)
-        self.upload_segmentations_setting.setObjectName("upload_segmentations_setting")
-        self.gridLayout_24.addWidget(self.upload_segmentations_setting, 0, 1, 1, 1)
+        self.upload_segmentations_setting.setObjectName(
+            "upload_segmentations_setting"
+        )
+        self.gridLayout_24.addWidget(
+            self.upload_segmentations_setting, 0, 1, 1, 1
+        )
         self.upload_images_setting = QtWidgets.QCheckBox(self.tab_4)
         self.upload_images_setting.setChecked(True)
         self.upload_images_setting.setObjectName("upload_images_setting")
         self.gridLayout_24.addWidget(self.upload_images_setting, 0, 0, 1, 1)
         self.upload_metadata_setting = QtWidgets.QCheckBox(self.tab_4)
         self.upload_metadata_setting.setChecked(True)
         self.upload_metadata_setting.setObjectName("upload_metadata_setting")
@@ -1658,56 +2155,79 @@
         self.gridLayout_25.addWidget(self.upload_overwrite_images, 0, 0, 1, 1)
         self.overwrite_all_metadata = QtWidgets.QCheckBox(self.tab_4)
         self.overwrite_all_metadata.setEnabled(True)
         self.overwrite_all_metadata.setObjectName("overwrite_all_metadata")
         self.gridLayout_25.addWidget(self.overwrite_all_metadata, 1, 0, 1, 1)
         self.overwrite_selected_metadata = QtWidgets.QCheckBox(self.tab_4)
         self.overwrite_selected_metadata.setEnabled(True)
-        self.overwrite_selected_metadata.setObjectName("overwrite_selected_metadata")
-        self.gridLayout_25.addWidget(self.overwrite_selected_metadata, 1, 1, 1, 1)
+        self.overwrite_selected_metadata.setObjectName(
+            "overwrite_selected_metadata"
+        )
+        self.gridLayout_25.addWidget(
+            self.overwrite_selected_metadata, 1, 1, 1, 1
+        )
         self.verticalLayout_11.addLayout(self.gridLayout_25)
-        spacerItem33 = QtWidgets.QSpacerItem(435, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        spacerItem33 = QtWidgets.QSpacerItem(
+            435,
+            20,
+            QtWidgets.QSizePolicy.Minimum,
+            QtWidgets.QSizePolicy.Minimum,
+        )
         self.verticalLayout_11.addItem(spacerItem33)
         self.database_upload_buttons_2 = QtWidgets.QGridLayout()
-        self.database_upload_buttons_2.setObjectName("database_upload_buttons_2")
+        self.database_upload_buttons_2.setObjectName(
+            "database_upload_buttons_2"
+        )
         self.upload_all = QtWidgets.QPushButton(self.tab_4)
         self.upload_all.setEnabled(True)
         self.upload_all.setObjectName("upload_all")
         self.database_upload_buttons_2.addWidget(self.upload_all, 0, 1, 1, 1)
         self.upload_active = QtWidgets.QPushButton(self.tab_4)
         self.upload_active.setEnabled(True)
         self.upload_active.setObjectName("upload_active")
-        self.database_upload_buttons_2.addWidget(self.upload_active, 0, 0, 1, 1)
+        self.database_upload_buttons_2.addWidget(
+            self.upload_active, 0, 0, 1, 1
+        )
         self.verticalLayout_11.addLayout(self.database_upload_buttons_2)
         self.tabWidget_2.addTab(self.tab_4, "")
         self.verticalLayout_4.addWidget(self.tabWidget_2)
         self.gridLayout_18 = QtWidgets.QGridLayout()
         self.gridLayout_18.setObjectName("gridLayout_18")
         self.label_89 = QtWidgets.QLabel(self.upload_tab)
         self.label_89.setObjectName("label_89")
         self.gridLayout_18.addWidget(self.label_89, 0, 0, 1, 1)
         self.upload_progressbar = QtWidgets.QProgressBar(self.upload_tab)
         self.upload_progressbar.setEnabled(True)
         self.upload_progressbar.setProperty("value", 0)
         self.upload_progressbar.setObjectName("upload_progressbar")
         self.gridLayout_18.addWidget(self.upload_progressbar, 0, 1, 1, 1)
         self.verticalLayout_4.addLayout(self.gridLayout_18)
-        spacerItem34 = QtWidgets.QSpacerItem(20, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        spacerItem34 = QtWidgets.QSpacerItem(
+            20,
+            20,
+            QtWidgets.QSizePolicy.Minimum,
+            QtWidgets.QSizePolicy.Expanding,
+        )
         self.verticalLayout_4.addItem(spacerItem34)
         tab_widget.addTab(self.upload_tab, "")
         self.export_tab = QtWidgets.QWidget()
         self.export_tab.setEnabled(True)
         self.export_tab.setObjectName("export_tab")
         self.verticalLayout_6 = QtWidgets.QVBoxLayout(self.export_tab)
         self.verticalLayout_6.setObjectName("verticalLayout_6")
         self.tabWidget_4 = QtWidgets.QTabWidget(self.export_tab)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.MinimumExpanding, QtWidgets.QSizePolicy.Preferred)
+        sizePolicy = QtWidgets.QSizePolicy(
+            QtWidgets.QSizePolicy.MinimumExpanding,
+            QtWidgets.QSizePolicy.Preferred,
+        )
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
-        sizePolicy.setHeightForWidth(self.tabWidget_4.sizePolicy().hasHeightForWidth())
+        sizePolicy.setHeightForWidth(
+            self.tabWidget_4.sizePolicy().hasHeightForWidth()
+        )
         self.tabWidget_4.setSizePolicy(sizePolicy)
         self.tabWidget_4.setObjectName("tabWidget_4")
         self.tab_8 = QtWidgets.QWidget()
         self.tab_8.setObjectName("tab_8")
         self.verticalLayout_15 = QtWidgets.QVBoxLayout(self.tab_8)
         self.verticalLayout_15.setObjectName("verticalLayout_15")
         self.tabWidget = QtWidgets.QTabWidget(self.tab_8)
@@ -1724,55 +2244,76 @@
         self.export_mode.addItem("")
         self.export_mode.addItem("")
         self.export_mode.addItem("")
         self.export_mode.addItem("")
         self.export_mode.addItem("")
         self.export_mode.addItem("")
         self.export_mode.addItem("")
-        self.formLayout_6.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.export_mode)
+        self.formLayout_6.setWidget(
+            1, QtWidgets.QFormLayout.FieldRole, self.export_mode
+        )
         self.label_19 = QtWidgets.QLabel(self.tab_18)
         self.label_19.setObjectName("label_19")
-        self.formLayout_6.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.label_19)
+        self.formLayout_6.setWidget(
+            1, QtWidgets.QFormLayout.LabelRole, self.label_19
+        )
         self.export_location = QtWidgets.QComboBox(self.tab_18)
         self.export_location.setObjectName("export_location")
         self.export_location.addItem("")
         self.export_location.addItem("")
-        self.formLayout_6.setWidget(2, QtWidgets.QFormLayout.FieldRole, self.export_location)
+        self.formLayout_6.setWidget(
+            2, QtWidgets.QFormLayout.FieldRole, self.export_location
+        )
         self.label_44 = QtWidgets.QLabel(self.tab_18)
         self.label_44.setObjectName("label_44")
-        self.formLayout_6.setWidget(2, QtWidgets.QFormLayout.LabelRole, self.label_44)
+        self.formLayout_6.setWidget(
+            2, QtWidgets.QFormLayout.LabelRole, self.label_44
+        )
         self.export_channel = QtWidgets.QComboBox(self.tab_18)
         self.export_channel.setObjectName("export_channel")
         self.export_channel.addItem("")
         self.export_channel.addItem("")
-        self.formLayout_6.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.export_channel)
+        self.formLayout_6.setWidget(
+            0, QtWidgets.QFormLayout.FieldRole, self.export_channel
+        )
         self.label_45 = QtWidgets.QLabel(self.tab_18)
         self.label_45.setObjectName("label_45")
-        self.formLayout_6.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_45)
+        self.formLayout_6.setWidget(
+            0, QtWidgets.QFormLayout.LabelRole, self.label_45
+        )
         self.verticalLayout_26.addLayout(self.formLayout_6)
         self.formLayout_5 = QtWidgets.QFormLayout()
         self.formLayout_5.setObjectName("formLayout_5")
         self.label_26 = QtWidgets.QLabel(self.tab_18)
         self.label_26.setObjectName("label_26")
-        self.formLayout_5.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_26)
+        self.formLayout_5.setWidget(
+            0, QtWidgets.QFormLayout.LabelRole, self.label_26
+        )
         self.export_modifier = QtWidgets.QLineEdit(self.tab_18)
         self.export_modifier.setObjectName("export_modifier")
-        self.formLayout_5.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.export_modifier)
+        self.formLayout_5.setWidget(
+            0, QtWidgets.QFormLayout.FieldRole, self.export_modifier
+        )
         self.verticalLayout_26.addLayout(self.formLayout_5)
         self.gridLayout_32 = QtWidgets.QGridLayout()
         self.gridLayout_32.setObjectName("gridLayout_32")
         self.export_image_setting = QtWidgets.QCheckBox(self.tab_18)
         self.export_image_setting.setChecked(True)
         self.export_image_setting.setObjectName("export_image_setting")
         self.gridLayout_32.addWidget(self.export_image_setting, 0, 0, 1, 1)
         self.export_overwrite_setting = QtWidgets.QCheckBox(self.tab_18)
         self.export_overwrite_setting.setObjectName("export_overwrite_setting")
         self.gridLayout_32.addWidget(self.export_overwrite_setting, 0, 1, 1, 1)
         self.verticalLayout_26.addLayout(self.gridLayout_32)
-        spacerItem35 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        spacerItem35 = QtWidgets.QSpacerItem(
+            20,
+            40,
+            QtWidgets.QSizePolicy.Minimum,
+            QtWidgets.QSizePolicy.Expanding,
+        )
         self.verticalLayout_26.addItem(spacerItem35)
         self.export_active = QtWidgets.QPushButton(self.tab_18)
         self.export_active.setObjectName("export_active")
         self.verticalLayout_26.addWidget(self.export_active)
         self.export_all = QtWidgets.QPushButton(self.tab_18)
         self.export_all.setObjectName("export_all")
         self.verticalLayout_26.addWidget(self.export_all)
@@ -1781,55 +2322,84 @@
         self.tab_19.setObjectName("tab_19")
         self.verticalLayout_25 = QtWidgets.QVBoxLayout(self.tab_19)
         self.verticalLayout_25.setObjectName("verticalLayout_25")
         self.formLayout_23 = QtWidgets.QFormLayout()
         self.formLayout_23.setObjectName("formLayout_23")
         self.label_101 = QtWidgets.QLabel(self.tab_19)
         self.label_101.setObjectName("label_101")
-        self.formLayout_23.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_101)
+        self.formLayout_23.setWidget(
+            0, QtWidgets.QFormLayout.LabelRole, self.label_101
+        )
         self.export_stack_channel = QtWidgets.QComboBox(self.tab_19)
         self.export_stack_channel.setObjectName("export_stack_channel")
-        self.formLayout_23.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.export_stack_channel)
+        self.formLayout_23.setWidget(
+            0, QtWidgets.QFormLayout.FieldRole, self.export_stack_channel
+        )
         self.label_99 = QtWidgets.QLabel(self.tab_19)
         self.label_99.setObjectName("label_99")
-        self.formLayout_23.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.label_99)
+        self.formLayout_23.setWidget(
+            1, QtWidgets.QFormLayout.LabelRole, self.label_99
+        )
         self.export_stack_mode = QtWidgets.QComboBox(self.tab_19)
         self.export_stack_mode.setObjectName("export_stack_mode")
         self.export_stack_mode.addItem("")
         self.export_stack_mode.addItem("")
-        self.formLayout_23.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.export_stack_mode)
+        self.formLayout_23.setWidget(
+            1, QtWidgets.QFormLayout.FieldRole, self.export_stack_mode
+        )
         self.label_100 = QtWidgets.QLabel(self.tab_19)
         self.label_100.setObjectName("label_100")
-        self.formLayout_23.setWidget(2, QtWidgets.QFormLayout.LabelRole, self.label_100)
+        self.formLayout_23.setWidget(
+            2, QtWidgets.QFormLayout.LabelRole, self.label_100
+        )
         self.export_stack_location = QtWidgets.QComboBox(self.tab_19)
         self.export_stack_location.setObjectName("export_stack_location")
         self.export_stack_location.addItem("")
         self.export_stack_location.addItem("")
-        self.formLayout_23.setWidget(2, QtWidgets.QFormLayout.FieldRole, self.export_stack_location)
+        self.formLayout_23.setWidget(
+            2, QtWidgets.QFormLayout.FieldRole, self.export_stack_location
+        )
         self.verticalLayout_25.addLayout(self.formLayout_23)
         self.formLayout_25 = QtWidgets.QFormLayout()
         self.formLayout_25.setObjectName("formLayout_25")
         self.label_103 = QtWidgets.QLabel(self.tab_19)
         self.label_103.setObjectName("label_103")
-        self.formLayout_25.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_103)
+        self.formLayout_25.setWidget(
+            0, QtWidgets.QFormLayout.LabelRole, self.label_103
+        )
         self.export_stack_modifier = QtWidgets.QLineEdit(self.tab_19)
         self.export_stack_modifier.setObjectName("export_stack_modifier")
-        self.formLayout_25.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.export_stack_modifier)
+        self.formLayout_25.setWidget(
+            0, QtWidgets.QFormLayout.FieldRole, self.export_stack_modifier
+        )
         self.verticalLayout_25.addLayout(self.formLayout_25)
         self.gridLayout_33 = QtWidgets.QGridLayout()
         self.gridLayout_33.setObjectName("gridLayout_33")
         self.export_stack_image_setting = QtWidgets.QCheckBox(self.tab_19)
         self.export_stack_image_setting.setChecked(True)
-        self.export_stack_image_setting.setObjectName("export_stack_image_setting")
-        self.gridLayout_33.addWidget(self.export_stack_image_setting, 0, 0, 1, 1)
+        self.export_stack_image_setting.setObjectName(
+            "export_stack_image_setting"
+        )
+        self.gridLayout_33.addWidget(
+            self.export_stack_image_setting, 0, 0, 1, 1
+        )
         self.export_stack_overwrite_setting = QtWidgets.QCheckBox(self.tab_19)
-        self.export_stack_overwrite_setting.setObjectName("export_stack_overwrite_setting")
-        self.gridLayout_33.addWidget(self.export_stack_overwrite_setting, 0, 1, 1, 1)
+        self.export_stack_overwrite_setting.setObjectName(
+            "export_stack_overwrite_setting"
+        )
+        self.gridLayout_33.addWidget(
+            self.export_stack_overwrite_setting, 0, 1, 1, 1
+        )
         self.verticalLayout_25.addLayout(self.gridLayout_33)
-        spacerItem36 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        spacerItem36 = QtWidgets.QSpacerItem(
+            20,
+            40,
+            QtWidgets.QSizePolicy.Minimum,
+            QtWidgets.QSizePolicy.Expanding,
+        )
         self.verticalLayout_25.addItem(spacerItem36)
         self.export_stack_active = QtWidgets.QPushButton(self.tab_19)
         self.export_stack_active.setObjectName("export_stack_active")
         self.verticalLayout_25.addWidget(self.export_stack_active)
         self.export_stack_all = QtWidgets.QPushButton(self.tab_19)
         self.export_stack_all.setObjectName("export_stack_all")
         self.verticalLayout_25.addWidget(self.export_stack_all)
@@ -1869,77 +2439,115 @@
         self.export_edge.setObjectName("export_edge")
         self.gridLayout.addWidget(self.export_edge, 1, 2, 1, 1)
         self.export_broken = QtWidgets.QCheckBox(self.tab_20)
         self.export_broken.setChecked(True)
         self.export_broken.setObjectName("export_broken")
         self.gridLayout.addWidget(self.export_broken, 1, 1, 1, 1)
         self.verticalLayout_27.addLayout(self.gridLayout)
-        spacerItem37 = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        spacerItem37 = QtWidgets.QSpacerItem(
+            20,
+            10,
+            QtWidgets.QSizePolicy.Minimum,
+            QtWidgets.QSizePolicy.Expanding,
+        )
         self.verticalLayout_27.addItem(spacerItem37)
         self.label_49 = QtWidgets.QLabel(self.tab_20)
         font = QtGui.QFont()
         font.setPointSize(10)
         font.setBold(True)
         font.setWeight(75)
         self.label_49.setFont(font)
         self.label_49.setObjectName("label_49")
         self.verticalLayout_27.addWidget(self.label_49)
         self.gridLayout_27 = QtWidgets.QGridLayout()
         self.gridLayout_27.setObjectName("gridLayout_27")
-        self.export_scalebar_resolution_units = QtWidgets.QComboBox(self.tab_20)
-        self.export_scalebar_resolution_units.setMaximumSize(QtCore.QSize(200, 100))
-        self.export_scalebar_resolution_units.setObjectName("export_scalebar_resolution_units")
+        self.export_scalebar_resolution_units = QtWidgets.QComboBox(
+            self.tab_20
+        )
+        self.export_scalebar_resolution_units.setMaximumSize(
+            QtCore.QSize(200, 100)
+        )
+        self.export_scalebar_resolution_units.setObjectName(
+            "export_scalebar_resolution_units"
+        )
         self.export_scalebar_resolution_units.addItem("")
         self.export_scalebar_resolution_units.addItem("")
-        self.gridLayout_27.addWidget(self.export_scalebar_resolution_units, 0, 2, 1, 1)
+        self.gridLayout_27.addWidget(
+            self.export_scalebar_resolution_units, 0, 2, 1, 1
+        )
         self.label_50 = QtWidgets.QLabel(self.tab_20)
         self.label_50.setObjectName("label_50")
         self.gridLayout_27.addWidget(self.label_50, 0, 0, 1, 1)
         self.export_scalebar_resolution = QtWidgets.QLineEdit(self.tab_20)
-        self.export_scalebar_resolution.setMaximumSize(QtCore.QSize(200, 16777215))
-        self.export_scalebar_resolution.setObjectName("export_scalebar_resolution")
-        self.gridLayout_27.addWidget(self.export_scalebar_resolution, 0, 1, 1, 1)
+        self.export_scalebar_resolution.setMaximumSize(
+            QtCore.QSize(200, 16777215)
+        )
+        self.export_scalebar_resolution.setObjectName(
+            "export_scalebar_resolution"
+        )
+        self.gridLayout_27.addWidget(
+            self.export_scalebar_resolution, 0, 1, 1, 1
+        )
         self.label_55 = QtWidgets.QLabel(self.tab_20)
         self.label_55.setObjectName("label_55")
         self.gridLayout_27.addWidget(self.label_55, 1, 0, 1, 1)
         self.export_scalebar_size = QtWidgets.QLineEdit(self.tab_20)
         self.export_scalebar_size.setMaximumSize(QtCore.QSize(200, 16777215))
         self.export_scalebar_size.setObjectName("export_scalebar_size")
         self.gridLayout_27.addWidget(self.export_scalebar_size, 1, 1, 1, 1)
         self.export_scalebar_size_units = QtWidgets.QComboBox(self.tab_20)
         self.export_scalebar_size_units.setMaximumSize(QtCore.QSize(200, 100))
-        self.export_scalebar_size_units.setObjectName("export_scalebar_size_units")
+        self.export_scalebar_size_units.setObjectName(
+            "export_scalebar_size_units"
+        )
         self.export_scalebar_size_units.addItem("")
         self.export_scalebar_size_units.addItem("")
-        self.gridLayout_27.addWidget(self.export_scalebar_size_units, 1, 2, 1, 1)
+        self.gridLayout_27.addWidget(
+            self.export_scalebar_size_units, 1, 2, 1, 1
+        )
         self.verticalLayout_27.addLayout(self.gridLayout_27)
         self.formLayout_19 = QtWidgets.QFormLayout()
         self.formLayout_19.setObjectName("formLayout_19")
         self.label_71 = QtWidgets.QLabel(self.tab_20)
         self.label_71.setObjectName("label_71")
-        self.formLayout_19.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_71)
+        self.formLayout_19.setWidget(
+            0, QtWidgets.QFormLayout.LabelRole, self.label_71
+        )
         self.export_scalebar_colour = QtWidgets.QComboBox(self.tab_20)
         self.export_scalebar_colour.setObjectName("export_scalebar_colour")
         self.export_scalebar_colour.addItem("")
         self.export_scalebar_colour.addItem("")
-        self.formLayout_19.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.export_scalebar_colour)
+        self.formLayout_19.setWidget(
+            0, QtWidgets.QFormLayout.FieldRole, self.export_scalebar_colour
+        )
         self.label_72 = QtWidgets.QLabel(self.tab_20)
         self.label_72.setObjectName("label_72")
-        self.formLayout_19.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.label_72)
+        self.formLayout_19.setWidget(
+            1, QtWidgets.QFormLayout.LabelRole, self.label_72
+        )
         self.export_scalebar_thickness = QtWidgets.QComboBox(self.tab_20)
-        self.export_scalebar_thickness.setObjectName("export_scalebar_thickness")
+        self.export_scalebar_thickness.setObjectName(
+            "export_scalebar_thickness"
+        )
         self.export_scalebar_thickness.addItem("")
         self.export_scalebar_thickness.addItem("")
         self.export_scalebar_thickness.addItem("")
         self.export_scalebar_thickness.addItem("")
         self.export_scalebar_thickness.addItem("")
         self.export_scalebar_thickness.addItem("")
-        self.formLayout_19.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.export_scalebar_thickness)
+        self.formLayout_19.setWidget(
+            1, QtWidgets.QFormLayout.FieldRole, self.export_scalebar_thickness
+        )
         self.verticalLayout_27.addLayout(self.formLayout_19)
-        spacerItem38 = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        spacerItem38 = QtWidgets.QSpacerItem(
+            20,
+            10,
+            QtWidgets.QSizePolicy.Minimum,
+            QtWidgets.QSizePolicy.Expanding,
+        )
         self.verticalLayout_27.addItem(spacerItem38)
         self.label_12 = QtWidgets.QLabel(self.tab_20)
         font = QtGui.QFont()
         font.setPointSize(10)
         font.setBold(True)
         font.setWeight(75)
         self.label_12.setFont(font)
@@ -1964,15 +2572,20 @@
         self.gridLayout_19.addWidget(self.export_mask_background, 2, 1, 1, 1)
         self.export_crop_zoom = QtWidgets.QCheckBox(self.tab_20)
         self.export_crop_zoom.setObjectName("export_crop_zoom")
         self.gridLayout_19.addWidget(self.export_crop_zoom, 2, 2, 1, 1)
         self.verticalLayout_27.addLayout(self.gridLayout_19)
         self.tabWidget.addTab(self.tab_20, "")
         self.verticalLayout_15.addWidget(self.tabWidget)
-        spacerItem39 = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        spacerItem39 = QtWidgets.QSpacerItem(
+            20,
+            10,
+            QtWidgets.QSizePolicy.Minimum,
+            QtWidgets.QSizePolicy.Expanding,
+        )
         self.verticalLayout_15.addItem(spacerItem39)
         self.tabWidget_4.addTab(self.tab_8, "")
         self.tab_9 = QtWidgets.QWidget()
         self.tab_9.setObjectName("tab_9")
         self.verticalLayout_17 = QtWidgets.QVBoxLayout(self.tab_9)
         self.verticalLayout_17.setObjectName("verticalLayout_17")
         self.label_46 = QtWidgets.QLabel(self.tab_9)
@@ -1985,55 +2598,79 @@
         self.verticalLayout_17.addWidget(self.label_46)
         self.gridLayout_11 = QtWidgets.QGridLayout()
         self.gridLayout_11.setObjectName("gridLayout_11")
         self.label_54 = QtWidgets.QLabel(self.tab_9)
         self.label_54.setObjectName("label_54")
         self.gridLayout_11.addWidget(self.label_54, 1, 0, 1, 1)
         self.export_statistics_pixelsize = QtWidgets.QLineEdit(self.tab_9)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Fixed)
+        sizePolicy = QtWidgets.QSizePolicy(
+            QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Fixed
+        )
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
-        sizePolicy.setHeightForWidth(self.export_statistics_pixelsize.sizePolicy().hasHeightForWidth())
+        sizePolicy.setHeightForWidth(
+            self.export_statistics_pixelsize.sizePolicy().hasHeightForWidth()
+        )
         self.export_statistics_pixelsize.setSizePolicy(sizePolicy)
-        self.export_statistics_pixelsize.setObjectName("export_statistics_pixelsize")
-        self.gridLayout_11.addWidget(self.export_statistics_pixelsize, 0, 1, 1, 1)
+        self.export_statistics_pixelsize.setObjectName(
+            "export_statistics_pixelsize"
+        )
+        self.gridLayout_11.addWidget(
+            self.export_statistics_pixelsize, 0, 1, 1, 1
+        )
         self.export_colicoords_mode = QtWidgets.QComboBox(self.tab_9)
         self.export_colicoords_mode.setObjectName("export_colicoords_mode")
         self.export_colicoords_mode.addItem("")
         self.export_colicoords_mode.addItem("")
         self.gridLayout_11.addWidget(self.export_colicoords_mode, 1, 1, 1, 1)
         self.label_52 = QtWidgets.QLabel(self.tab_9)
         self.label_52.setObjectName("label_52")
         self.gridLayout_11.addWidget(self.label_52, 0, 0, 1, 1)
         self.verticalLayout_17.addLayout(self.gridLayout_11)
-        spacerItem40 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        spacerItem40 = QtWidgets.QSpacerItem(
+            20,
+            40,
+            QtWidgets.QSizePolicy.Minimum,
+            QtWidgets.QSizePolicy.Expanding,
+        )
         self.verticalLayout_17.addItem(spacerItem40)
         self.export_statistics_multithreaded = QtWidgets.QCheckBox(self.tab_9)
         self.export_statistics_multithreaded.setChecked(True)
-        self.export_statistics_multithreaded.setObjectName("export_statistics_multithreaded")
+        self.export_statistics_multithreaded.setObjectName(
+            "export_statistics_multithreaded"
+        )
         self.verticalLayout_17.addWidget(self.export_statistics_multithreaded)
         self.export_statistics_active = QtWidgets.QPushButton(self.tab_9)
         self.export_statistics_active.setObjectName("export_statistics_active")
         self.verticalLayout_17.addWidget(self.export_statistics_active)
         self.export_statistics_all = QtWidgets.QPushButton(self.tab_9)
         self.export_statistics_all.setObjectName("export_statistics_all")
         self.verticalLayout_17.addWidget(self.export_statistics_all)
         self.tabWidget_4.addTab(self.tab_9, "")
         self.verticalLayout_6.addWidget(self.tabWidget_4)
         self.formLayout_11 = QtWidgets.QFormLayout()
         self.formLayout_11.setObjectName("formLayout_11")
         self.label_33 = QtWidgets.QLabel(self.export_tab)
         self.label_33.setObjectName("label_33")
-        self.formLayout_11.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_33)
+        self.formLayout_11.setWidget(
+            0, QtWidgets.QFormLayout.LabelRole, self.label_33
+        )
         self.export_progressbar = QtWidgets.QProgressBar(self.export_tab)
         self.export_progressbar.setProperty("value", 0)
         self.export_progressbar.setObjectName("export_progressbar")
-        self.formLayout_11.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.export_progressbar)
+        self.formLayout_11.setWidget(
+            0, QtWidgets.QFormLayout.FieldRole, self.export_progressbar
+        )
         self.verticalLayout_6.addLayout(self.formLayout_11)
-        spacerItem41 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        spacerItem41 = QtWidgets.QSpacerItem(
+            20,
+            40,
+            QtWidgets.QSizePolicy.Minimum,
+            QtWidgets.QSizePolicy.Expanding,
+        )
         self.verticalLayout_6.addItem(spacerItem41)
         tab_widget.addTab(self.export_tab, "")
         self.tab_14 = QtWidgets.QWidget()
         self.tab_14.setObjectName("tab_14")
         self.verticalLayout_18 = QtWidgets.QVBoxLayout(self.tab_14)
         self.verticalLayout_18.setObjectName("verticalLayout_18")
         self.line_20 = QtWidgets.QFrame(self.tab_14)
@@ -2052,15 +2689,20 @@
         self.verticalLayout_18.addWidget(self.modify_deleteotherimages)
         self.modify_deleteactivemasks = QtWidgets.QPushButton(self.tab_14)
         self.modify_deleteactivemasks.setObjectName("modify_deleteactivemasks")
         self.verticalLayout_18.addWidget(self.modify_deleteactivemasks)
         self.modify_deleteallmasks = QtWidgets.QPushButton(self.tab_14)
         self.modify_deleteallmasks.setObjectName("modify_deleteallmasks")
         self.verticalLayout_18.addWidget(self.modify_deleteallmasks)
-        spacerItem42 = QtWidgets.QSpacerItem(20, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        spacerItem42 = QtWidgets.QSpacerItem(
+            20,
+            20,
+            QtWidgets.QSizePolicy.Minimum,
+            QtWidgets.QSizePolicy.Minimum,
+        )
         self.verticalLayout_18.addItem(spacerItem42)
         self.line_22 = QtWidgets.QFrame(self.tab_14)
         self.line_22.setFrameShape(QtWidgets.QFrame.HLine)
         self.line_22.setFrameShadow(QtWidgets.QFrame.Sunken)
         self.line_22.setObjectName("line_22")
         self.verticalLayout_18.addWidget(self.line_22)
         self.label_31 = QtWidgets.QLabel(self.tab_14)
@@ -2084,22 +2726,31 @@
         self.refine_all = QtWidgets.QPushButton(self.tab_14)
         self.refine_all.setObjectName("refine_all")
         self.verticalLayout_18.addWidget(self.refine_all)
         self.formLayout = QtWidgets.QFormLayout()
         self.formLayout.setObjectName("formLayout")
         self.label_17 = QtWidgets.QLabel(self.tab_14)
         self.label_17.setObjectName("label_17")
-        self.formLayout.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_17)
+        self.formLayout.setWidget(
+            0, QtWidgets.QFormLayout.LabelRole, self.label_17
+        )
         self.modify_progressbar = QtWidgets.QProgressBar(self.tab_14)
         self.modify_progressbar.setProperty("value", 0)
         self.modify_progressbar.setTextVisible(True)
         self.modify_progressbar.setObjectName("modify_progressbar")
-        self.formLayout.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.modify_progressbar)
+        self.formLayout.setWidget(
+            0, QtWidgets.QFormLayout.FieldRole, self.modify_progressbar
+        )
         self.verticalLayout_18.addLayout(self.formLayout)
-        spacerItem43 = QtWidgets.QSpacerItem(20, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        spacerItem43 = QtWidgets.QSpacerItem(
+            20,
+            20,
+            QtWidgets.QSizePolicy.Minimum,
+            QtWidgets.QSizePolicy.Minimum,
+        )
         self.verticalLayout_18.addItem(spacerItem43)
         self.line_23 = QtWidgets.QFrame(self.tab_14)
         self.line_23.setFrameShape(QtWidgets.QFrame.HLine)
         self.line_23.setFrameShadow(QtWidgets.QFrame.Sunken)
         self.line_23.setObjectName("line_23")
         self.verticalLayout_18.addWidget(self.line_23)
         self.label_56 = QtWidgets.QLabel(self.tab_14)
@@ -2126,43 +2777,57 @@
         self.find_criterion = QtWidgets.QComboBox(self.tab_14)
         self.find_criterion.setObjectName("find_criterion")
         self.find_criterion.addItem("")
         self.find_criterion.addItem("")
         self.find_criterion.addItem("")
         self.gridLayout_7.addWidget(self.find_criterion, 0, 0, 1, 1)
         self.verticalLayout_18.addLayout(self.gridLayout_7)
-        spacerItem44 = QtWidgets.QSpacerItem(20, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        spacerItem44 = QtWidgets.QSpacerItem(
+            20,
+            20,
+            QtWidgets.QSizePolicy.Minimum,
+            QtWidgets.QSizePolicy.Minimum,
+        )
         self.verticalLayout_18.addItem(spacerItem44)
         self.label_70 = QtWidgets.QLabel(self.tab_14)
         font = QtGui.QFont()
         font.setPointSize(10)
         font.setBold(True)
         font.setWeight(75)
         self.label_70.setFont(font)
         self.label_70.setObjectName("label_70")
         self.verticalLayout_18.addWidget(self.label_70)
         self.formLayout_18 = QtWidgets.QFormLayout()
         self.formLayout_18.setObjectName("formLayout_18")
         self.alignment_channel = QtWidgets.QComboBox(self.tab_14)
         self.alignment_channel.setObjectName("alignment_channel")
-        self.formLayout_18.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.alignment_channel)
+        self.formLayout_18.setWidget(
+            0, QtWidgets.QFormLayout.FieldRole, self.alignment_channel
+        )
         self.label_40 = QtWidgets.QLabel(self.tab_14)
         self.label_40.setObjectName("label_40")
-        self.formLayout_18.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_40)
+        self.formLayout_18.setWidget(
+            0, QtWidgets.QFormLayout.LabelRole, self.label_40
+        )
         self.verticalLayout_18.addLayout(self.formLayout_18)
         self.gridLayout_26 = QtWidgets.QGridLayout()
         self.gridLayout_26.setObjectName("gridLayout_26")
         self.align_active_image = QtWidgets.QPushButton(self.tab_14)
         self.align_active_image.setObjectName("align_active_image")
         self.gridLayout_26.addWidget(self.align_active_image, 0, 0, 1, 1)
         self.align_all_images = QtWidgets.QPushButton(self.tab_14)
         self.align_all_images.setObjectName("align_all_images")
         self.gridLayout_26.addWidget(self.align_all_images, 0, 1, 1, 1)
         self.verticalLayout_18.addLayout(self.gridLayout_26)
-        spacerItem45 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        spacerItem45 = QtWidgets.QSpacerItem(
+            20,
+            40,
+            QtWidgets.QSizePolicy.Minimum,
+            QtWidgets.QSizePolicy.Expanding,
+        )
         self.verticalLayout_18.addItem(spacerItem45)
         tab_widget.addTab(self.tab_14, "")
 
         self.retranslateUi(tab_widget)
         tab_widget.setCurrentIndex(0)
         self.import_limit.setCurrentIndex(6)
         self.import_precision.setCurrentIndex(1)
@@ -2187,141 +2852,272 @@
         self.export_scalebar_size_units.setCurrentIndex(1)
         self.export_scalebar_thickness.setCurrentIndex(3)
         QtCore.QMetaObject.connectSlotsByName(tab_widget)
 
     def retranslateUi(self, tab_widget):
         _translate = QtCore.QCoreApplication.translate
         tab_widget.setWindowTitle(_translate("tab_widget", "TabWidget"))
-        self.label_37.setText(_translate("tab_widget", "General Import Settings"))
+        self.label_37.setText(
+            _translate("tab_widget", "General Import Settings")
+        )
         self.label_51.setText(_translate("tab_widget", "Import File Mode"))
-        self.import_filemode.setItemText(0, _translate("tab_widget", "Import File(s)"))
-        self.import_filemode.setItemText(1, _translate("tab_widget", "Import Directory"))
-        self.import_limit_label.setText(_translate("tab_widget", "Import File Limit"))
+        self.import_filemode.setItemText(
+            0, _translate("tab_widget", "Import File(s)")
+        )
+        self.import_filemode.setItemText(
+            1, _translate("tab_widget", "Import Directory")
+        )
+        self.import_limit_label.setText(
+            _translate("tab_widget", "Import File Limit")
+        )
         self.import_limit.setItemText(0, _translate("tab_widget", "1"))
         self.import_limit.setItemText(1, _translate("tab_widget", "5"))
         self.import_limit.setItemText(2, _translate("tab_widget", "10"))
         self.import_limit.setItemText(3, _translate("tab_widget", "20"))
         self.import_limit.setItemText(4, _translate("tab_widget", "50"))
         self.import_limit.setItemText(5, _translate("tab_widget", "100"))
         self.import_limit.setItemText(6, _translate("tab_widget", "None"))
         self.label_30.setText(_translate("tab_widget", "Multi-Frame Mode"))
-        self.import_multiframe_mode.setItemText(0, _translate("tab_widget", "Keep Brightest Frame"))
-        self.import_multiframe_mode.setItemText(1, _translate("tab_widget", "Average Frames"))
-        self.import_multiframe_mode.setItemText(2, _translate("tab_widget", "Sum Frames"))
-        self.import_multiframe_mode.setItemText(3, _translate("tab_widget", "Keep First Frame"))
-        self.import_multiframe_mode.setItemText(4, _translate("tab_widget", "Keep All Frames (BETA)"))
+        self.import_multiframe_mode.setItemText(
+            0, _translate("tab_widget", "Keep Brightest Frame")
+        )
+        self.import_multiframe_mode.setItemText(
+            1, _translate("tab_widget", "Average Frames")
+        )
+        self.import_multiframe_mode.setItemText(
+            2, _translate("tab_widget", "Sum Frames")
+        )
+        self.import_multiframe_mode.setItemText(
+            3, _translate("tab_widget", "Keep First Frame")
+        )
+        self.import_multiframe_mode.setItemText(
+            4, _translate("tab_widget", "Keep All Frames (BETA)")
+        )
         self.label_22.setText(_translate("tab_widget", "Image Crop Mode"))
         self.import_crop_mode.setItemText(0, _translate("tab_widget", "None"))
-        self.import_crop_mode.setItemText(1, _translate("tab_widget", "Crop Left Half"))
-        self.import_crop_mode.setItemText(2, _translate("tab_widget", "Crop Right Half"))
-        self.import_crop_mode.setItemText(3, _translate("tab_widget", "Crop Brightest Half"))
+        self.import_crop_mode.setItemText(
+            1, _translate("tab_widget", "Crop Left Half")
+        )
+        self.import_crop_mode.setItemText(
+            2, _translate("tab_widget", "Crop Right Half")
+        )
+        self.import_crop_mode.setItemText(
+            3, _translate("tab_widget", "Crop Brightest Half")
+        )
         self.label_21.setText(_translate("tab_widget", "Import Precision"))
         self.import_precision.setItemText(0, _translate("tab_widget", "int8"))
         self.import_precision.setItemText(1, _translate("tab_widget", "int16"))
         self.import_precision.setItemText(2, _translate("tab_widget", "int32"))
-        self.import_precision.setItemText(3, _translate("tab_widget", "native"))
+        self.import_precision.setItemText(
+            3, _translate("tab_widget", "native")
+        )
         self.import_mode.setItemText(0, _translate("tab_widget", "Images"))
-        self.import_mode.setItemText(1, _translate("tab_widget", "NanoImager Data"))
+        self.import_mode.setItemText(
+            1, _translate("tab_widget", "NanoImager Data")
+        )
         self.import_mode.setItemText(2, _translate("tab_widget", "ScanR Data"))
-        self.import_mode.setItemText(3, _translate("tab_widget", "ImageJ files(s)"))
-        self.import_mode.setItemText(4, _translate("tab_widget", "Mask (.tif) Segmentation(s)"))
-        self.import_mode.setItemText(5, _translate("tab_widget", "Cellpose (.npy) Segmentation(s)"))
-        self.import_mode.setItemText(6, _translate("tab_widget", "Oufti (.mat) Segmentation(s)"))
-        self.import_mode.setItemText(7, _translate("tab_widget", "JSON (.txt) Segmentation(s)"))
+        self.import_mode.setItemText(
+            3, _translate("tab_widget", "Zeiss (.czi) Data")
+        )
+        self.import_mode.setItemText(
+            4, _translate("tab_widget", "ImageJ files(s)")
+        )
+        self.import_mode.setItemText(
+            5, _translate("tab_widget", "Mask (.tif) Segmentation(s)")
+        )
+        self.import_mode.setItemText(
+            6, _translate("tab_widget", "Cellpose (.npy) Segmentation(s)")
+        )
+        self.import_mode.setItemText(
+            7, _translate("tab_widget", "Oufti (.mat) Segmentation(s)")
+        )
+        self.import_mode.setItemText(
+            8, _translate("tab_widget", "JSON (.txt) Segmentation(s)")
+        )
         self.label_27.setText(_translate("tab_widget", "Import Mode"))
         self.label_105.setText(_translate("tab_widget", "Append Mode"))
-        self.import_append_mode.setItemText(0, _translate("tab_widget", "None (Clear Previous Images)"))
-        self.import_append_mode.setItemText(1, _translate("tab_widget", "Append Images"))
-        self.import_append_mode.setItemText(2, _translate("tab_widget", "Append Channels"))
-        self.import_align.setText(_translate("tab_widget", "Align Image Channels (Slow)"))
+        self.import_append_mode.setItemText(
+            0, _translate("tab_widget", "None (Clear Previous Images)")
+        )
+        self.import_append_mode.setItemText(
+            1, _translate("tab_widget", "Append Images")
+        )
+        self.import_append_mode.setItemText(
+            2, _translate("tab_widget", "Append Channels")
+        )
+        self.import_align.setText(
+            _translate("tab_widget", "Align Image Channels (Slow)")
+        )
         self.import_import.setText(_translate("tab_widget", "Import"))
         self.label_36.setText(_translate("tab_widget", "Progress"))
-        tab_widget.setTabText(tab_widget.indexOf(self.import_tab), _translate("tab_widget", "Import"))
-        self.label_60.setText(_translate("tab_widget", "Auto Contrast Adjustment"))
-        self.import_auto_contrast.setText(_translate("tab_widget", "Auto Contrast Adjustment"))
-        self.label_38.setText(_translate("tab_widget", "View Mask/Class Labels"))
-        self.modify_viewlabels.setText(_translate("tab_widget", "View Class Labels [x]"))
-        self.modify_viewmasks.setText(_translate("tab_widget", "View Masks [Z]"))
-        self.zoom_.setTabText(self.zoom_.indexOf(self.tab_16), _translate("tab_widget", "General"))
+        tab_widget.setTabText(
+            tab_widget.indexOf(self.import_tab),
+            _translate("tab_widget", "Import"),
+        )
+        self.label_60.setText(
+            _translate("tab_widget", "Auto Contrast Adjustment")
+        )
+        self.import_auto_contrast.setText(
+            _translate("tab_widget", "Auto Contrast Adjustment")
+        )
+        self.label_38.setText(
+            _translate("tab_widget", "View Mask/Class Labels")
+        )
+        self.modify_viewlabels.setText(
+            _translate("tab_widget", "View Class Labels [x]")
+        )
+        self.modify_viewmasks.setText(
+            _translate("tab_widget", "View Masks [Z]")
+        )
+        self.zoom_.setTabText(
+            self.zoom_.indexOf(self.tab_16),
+            _translate("tab_widget", "General"),
+        )
         self.label_47.setText(_translate("tab_widget", "Scale Bar Settings"))
         self.scalebar_show.setText(_translate("tab_widget", "Show Scale Bar"))
         self.scalebar_units.setItemText(0, _translate("tab_widget", "um"))
         self.scalebar_units.setItemText(1, _translate("tab_widget", "nm"))
-        self.label_48.setText(_translate("tab_widget", "Pixel Resolution (um)"))
-        self.zoom_.setTabText(self.zoom_.indexOf(self.tab_7), _translate("tab_widget", "Scale Bar"))
-        self.label_73.setText(_translate("tab_widget", "Information Overlay Settings"))
+        self.label_48.setText(
+            _translate("tab_widget", "Pixel Resolution (um)")
+        )
+        self.zoom_.setTabText(
+            self.zoom_.indexOf(self.tab_7),
+            _translate("tab_widget", "Scale Bar"),
+        )
+        self.label_73.setText(
+            _translate("tab_widget", "Information Overlay Settings")
+        )
         self.overlay_filename.setText(_translate("tab_widget", "File Name"))
         self.overlay_folder.setText(_translate("tab_widget", "Folder"))
         self.overlay_antibiotic.setText(_translate("tab_widget", "Antibiotic"))
         self.overlay_phenotype.setText(_translate("tab_widget", "Phenotype"))
         self.overlay_strain.setText(_translate("tab_widget", "Strain"))
         self.overlay_content.setText(_translate("tab_widget", "Content"))
         self.overlay_microscope.setText(_translate("tab_widget", "Microscope"))
-        self.overlay_datemodified.setText(_translate("tab_widget", "Date Modified"))
-        self.overlay_lightsource.setText(_translate("tab_widget", "Light Source"))
-        self.overlay_staintarget.setText(_translate("tab_widget", "Stain Target"))
+        self.overlay_datemodified.setText(
+            _translate("tab_widget", "Date Modified")
+        )
+        self.overlay_lightsource.setText(
+            _translate("tab_widget", "Light Source")
+        )
+        self.overlay_staintarget.setText(
+            _translate("tab_widget", "Stain Target")
+        )
         self.overlay_modality.setText(_translate("tab_widget", "Modality"))
         self.overlay_stain.setText(_translate("tab_widget", "Stain"))
         self.overlay_focus.setText(_translate("tab_widget", "Image Focus"))
-        self.overlay_laplacian.setText(_translate("tab_widget", "Image Laplacian"))
+        self.overlay_laplacian.setText(
+            _translate("tab_widget", "Image Laplacian")
+        )
         self.overlay_debris.setText(_translate("tab_widget", "Image Debris"))
         self.overlay_range.setText(_translate("tab_widget", "Image Range"))
-        self.zoom_.setTabText(self.zoom_.indexOf(self.tab_15), _translate("tab_widget", "Overlay"))
-        self.label_57.setText(_translate("tab_widget", "Unfold/Fold into Tiles"))
+        self.zoom_.setTabText(
+            self.zoom_.indexOf(self.tab_15),
+            _translate("tab_widget", "Overlay"),
+        )
+        self.label_57.setText(
+            _translate("tab_widget", "Unfold/Fold into Tiles")
+        )
         self.unfold.setText(_translate("tab_widget", "Unfold"))
         self.fold.setText(_translate("tab_widget", "Fold"))
         self.label_58.setText(_translate("tab_widget", "Tile Size (Pixels)"))
         self.unfold_tile_size.setItemText(0, _translate("tab_widget", "100"))
         self.unfold_tile_size.setItemText(1, _translate("tab_widget", "200"))
         self.unfold_tile_size.setItemText(2, _translate("tab_widget", "300"))
         self.unfold_tile_size.setItemText(3, _translate("tab_widget", "500"))
         self.unfold_tile_size.setItemText(4, _translate("tab_widget", "1000"))
-        self.label_59.setText(_translate("tab_widget", "Tile Overlap (Pixels)"))
+        self.label_59.setText(
+            _translate("tab_widget", "Tile Overlap (Pixels)")
+        )
         self.unfold_tile_overlap.setItemText(0, _translate("tab_widget", "10"))
         self.unfold_tile_overlap.setItemText(1, _translate("tab_widget", "20"))
         self.unfold_tile_overlap.setItemText(2, _translate("tab_widget", "30"))
         self.unfold_tile_overlap.setItemText(3, _translate("tab_widget", "50"))
-        self.unfold_tile_overlap.setItemText(4, _translate("tab_widget", "100"))
+        self.unfold_tile_overlap.setItemText(
+            4, _translate("tab_widget", "100")
+        )
         self.label_62.setText(_translate("tab_widget", "Mode"))
-        self.unfold_mode.setItemText(0, _translate("tab_widget", "Nested Tiles"))
-        self.unfold_mode.setItemText(1, _translate("tab_widget", "Smaller Images (Extra FOVs)"))
-        self.zoom_.setTabText(self.zoom_.indexOf(self.tab_17), _translate("tab_widget", "Fold/Unfold"))
-        self.label_86.setText(_translate("tab_widget", "Zoom in/out at Specific Intervals"))
+        self.unfold_mode.setItemText(
+            0, _translate("tab_widget", "Nested Tiles")
+        )
+        self.unfold_mode.setItemText(
+            1, _translate("tab_widget", "Smaller Images (Extra FOVs)")
+        )
+        self.zoom_.setTabText(
+            self.zoom_.indexOf(self.tab_17),
+            _translate("tab_widget", "Fold/Unfold"),
+        )
+        self.label_86.setText(
+            _translate("tab_widget", "Zoom in/out at Specific Intervals")
+        )
         self.label_93.setText(_translate("tab_widget", "Magnification (%)"))
-        self.zoom_magnification.setItemText(0, _translate("tab_widget", "0 (Home)"))
+        self.zoom_magnification.setItemText(
+            0, _translate("tab_widget", "0 (Home)")
+        )
         self.zoom_magnification.setItemText(1, _translate("tab_widget", "10"))
         self.zoom_magnification.setItemText(2, _translate("tab_widget", "20"))
         self.zoom_magnification.setItemText(3, _translate("tab_widget", "30"))
         self.zoom_magnification.setItemText(4, _translate("tab_widget", "40"))
         self.zoom_magnification.setItemText(5, _translate("tab_widget", "50"))
         self.zoom_magnification.setItemText(6, _translate("tab_widget", "100"))
         self.zoom_magnification.setItemText(7, _translate("tab_widget", "200"))
         self.zoom_magnification.setItemText(8, _translate("tab_widget", "300"))
         self.zoom_magnification.setItemText(9, _translate("tab_widget", "400"))
-        self.zoom_magnification.setItemText(10, _translate("tab_widget", "500"))
+        self.zoom_magnification.setItemText(
+            10, _translate("tab_widget", "500")
+        )
         self.zoom_apply.setText(_translate("tab_widget", "Apply Zoom"))
-        self.zoom_.setTabText(self.zoom_.indexOf(self.tab_5), _translate("tab_widget", "Zoom"))
-        tab_widget.setTabText(tab_widget.indexOf(self.tab), _translate("tab_widget", "View"))
-        self.cellpose_select_custom_model.setText(_translate("tab_widget", "Select Custom Cellpose Model"))
+        self.zoom_.setTabText(
+            self.zoom_.indexOf(self.tab_5), _translate("tab_widget", "Zoom")
+        )
+        tab_widget.setTabText(
+            tab_widget.indexOf(self.tab), _translate("tab_widget", "View")
+        )
+        self.cellpose_select_custom_model.setText(
+            _translate("tab_widget", "Select Custom Cellpose Model")
+        )
         self.label_97.setText(_translate("tab_widget", "Segmentation Mode"))
         self.label_2.setText(_translate("tab_widget", "Segmentation Channel"))
         self.label.setText(_translate("tab_widget", "Cellpose Model"))
         self.cellpose_segmodel.setItemText(0, _translate("tab_widget", "cyto"))
-        self.cellpose_segmodel.setItemText(1, _translate("tab_widget", "nuclei"))
-        self.cellpose_segmodel.setItemText(2, _translate("tab_widget", "tissuenet"))
-        self.cellpose_segmodel.setItemText(3, _translate("tab_widget", "livecell"))
-        self.cellpose_segmodel.setItemText(4, _translate("tab_widget", "cyto2"))
-        self.cellpose_segmodel.setItemText(5, _translate("tab_widget", "general"))
-        self.cellpose_segmodel.setItemText(6, _translate("tab_widget", "custom"))
-        self.cellpose_seg_mode.setItemText(0, _translate("tab_widget", "Cell Wall"))
-        self.cellpose_seg_mode.setItemText(1, _translate("tab_widget", "Nucleiod"))
-        self.cellpose_segment_active.setText(_translate("tab_widget", "Segment Active Image"))
-        self.cellpose_segment_all.setText(_translate("tab_widget", "Segment All Images"))
+        self.cellpose_segmodel.setItemText(
+            1, _translate("tab_widget", "nuclei")
+        )
+        self.cellpose_segmodel.setItemText(
+            2, _translate("tab_widget", "tissuenet")
+        )
+        self.cellpose_segmodel.setItemText(
+            3, _translate("tab_widget", "livecell")
+        )
+        self.cellpose_segmodel.setItemText(
+            4, _translate("tab_widget", "cyto2")
+        )
+        self.cellpose_segmodel.setItemText(
+            5, _translate("tab_widget", "general")
+        )
+        self.cellpose_segmodel.setItemText(
+            6, _translate("tab_widget", "custom")
+        )
+        self.cellpose_seg_mode.setItemText(
+            0, _translate("tab_widget", "Cell Wall")
+        )
+        self.cellpose_seg_mode.setItemText(
+            1, _translate("tab_widget", "Nucleiod")
+        )
+        self.cellpose_segment_active.setText(
+            _translate("tab_widget", "Segment Active Image")
+        )
+        self.cellpose_segment_all.setText(
+            _translate("tab_widget", "Segment All Images")
+        )
         self.label_35.setText(_translate("tab_widget", "Progress"))
-        self.tabWidget_3.setTabText(self.tabWidget_3.indexOf(self.tab_6), _translate("tab_widget", "Segment"))
+        self.tabWidget_3.setTabText(
+            self.tabWidget_3.indexOf(self.tab_6),
+            _translate("tab_widget", "Segment"),
+        )
         self.label_8.setText(_translate("tab_widget", "Train Channel"))
         self.label_9.setText(_translate("tab_widget", "N Epochs"))
         self.cellpose_nepochs.setItemText(0, _translate("tab_widget", "1"))
         self.cellpose_nepochs.setItemText(1, _translate("tab_widget", "5"))
         self.cellpose_nepochs.setItemText(2, _translate("tab_widget", "10"))
         self.cellpose_nepochs.setItemText(3, _translate("tab_widget", "100"))
         self.cellpose_nepochs.setItemText(4, _translate("tab_widget", "200"))
@@ -2330,348 +3126,791 @@
         self.cellpose_batchsize.setItemText(0, _translate("tab_widget", "5"))
         self.cellpose_batchsize.setItemText(1, _translate("tab_widget", "10"))
         self.cellpose_batchsize.setItemText(2, _translate("tab_widget", "20"))
         self.cellpose_batchsize.setItemText(3, _translate("tab_widget", "30"))
         self.cellpose_batchsize.setItemText(4, _translate("tab_widget", "40"))
         self.cellpose_batchsize.setItemText(5, _translate("tab_widget", "50"))
         self.cellpose_batchsize.setItemText(6, _translate("tab_widget", "100"))
-        self.label_11.setText(_translate("tab_widget", "Initial Model (Transfer Learning)"))
-        self.cellpose_trainmodel.setItemText(0, _translate("tab_widget", "cyto"))
-        self.cellpose_trainmodel.setItemText(1, _translate("tab_widget", "nuclei"))
-        self.cellpose_trainmodel.setItemText(2, _translate("tab_widget", "tissuenet"))
-        self.cellpose_trainmodel.setItemText(3, _translate("tab_widget", "livecell"))
-        self.cellpose_trainmodel.setItemText(4, _translate("tab_widget", "cyto2"))
-        self.cellpose_trainmodel.setItemText(5, _translate("tab_widget", "general"))
-        self.cellpose_trainmodel.setItemText(6, _translate("tab_widget", "custom"))
-        self.cellpose_save_dir.setText(_translate("tab_widget", "Select Save Directory"))
-        self.cellpose_train_model.setText(_translate("tab_widget", "Train Cellpose Model (All Images)"))
-        self.tabWidget_3.setTabText(self.tabWidget_3.indexOf(self.tab_11), _translate("tab_widget", "Train"))
+        self.label_11.setText(
+            _translate("tab_widget", "Initial Model (Transfer Learning)")
+        )
+        self.cellpose_trainmodel.setItemText(
+            0, _translate("tab_widget", "cyto")
+        )
+        self.cellpose_trainmodel.setItemText(
+            1, _translate("tab_widget", "nuclei")
+        )
+        self.cellpose_trainmodel.setItemText(
+            2, _translate("tab_widget", "tissuenet")
+        )
+        self.cellpose_trainmodel.setItemText(
+            3, _translate("tab_widget", "livecell")
+        )
+        self.cellpose_trainmodel.setItemText(
+            4, _translate("tab_widget", "cyto2")
+        )
+        self.cellpose_trainmodel.setItemText(
+            5, _translate("tab_widget", "general")
+        )
+        self.cellpose_trainmodel.setItemText(
+            6, _translate("tab_widget", "custom")
+        )
+        self.cellpose_save_dir.setText(
+            _translate("tab_widget", "Select Save Directory")
+        )
+        self.cellpose_train_model.setText(
+            _translate("tab_widget", "Train Cellpose Model (All Images)")
+        )
+        self.tabWidget_3.setTabText(
+            self.tabWidget_3.indexOf(self.tab_11),
+            _translate("tab_widget", "Train"),
+        )
         self.label_94.setText(_translate("tab_widget", "Cellpose Controls"))
         self.cellpose_flowthresh_label.setText(_translate("tab_widget", "0.9"))
         self.label_3.setText(_translate("tab_widget", "Flow Threshold"))
         self.cellpose_maskthresh_label.setText(_translate("tab_widget", "0.0"))
         self.cellpose_minsize_label.setText(_translate("tab_widget", "15"))
         self.label_5.setText(_translate("tab_widget", "Mask Threshold"))
         self.label_6.setText(_translate("tab_widget", "Min Size"))
         self.label_4.setText(_translate("tab_widget", "Diameter"))
         self.cellpose_diameter_label.setText(_translate("tab_widget", "15"))
-        self.label_95.setText(_translate("tab_widget", "Cellpose Post Processing"))
-        self.label_96.setText(_translate("tab_widget", "Min Segmentation Size (Pixels)"))
-        self.cellpose_min_seg_size.setCurrentText(_translate("tab_widget", "50"))
-        self.cellpose_min_seg_size.setItemText(0, _translate("tab_widget", "1"))
-        self.cellpose_min_seg_size.setItemText(1, _translate("tab_widget", "5"))
-        self.cellpose_min_seg_size.setItemText(2, _translate("tab_widget", "10"))
-        self.cellpose_min_seg_size.setItemText(3, _translate("tab_widget", "50"))
-        self.cellpose_clear_previous.setText(_translate("tab_widget", "Clear Previous Segmentations"))
-        self.cellpose_usegpu.setText(_translate("tab_widget", "Use GPU (if Availiable)"))
-        self.cellpose_resetimage.setText(_translate("tab_widget", "Reset Image View After Segmentation"))
-        self.tabWidget_3.setTabText(self.tabWidget_3.indexOf(self.tab_12), _translate("tab_widget", "Settings"))
-        tab_widget.setTabText(tab_widget.indexOf(self.segement_tab), _translate("tab_widget", "Segment"))
+        self.label_95.setText(
+            _translate("tab_widget", "Cellpose Post Processing")
+        )
+        self.label_96.setText(
+            _translate("tab_widget", "Min Segmentation Size (Pixels)")
+        )
+        self.cellpose_min_seg_size.setCurrentText(
+            _translate("tab_widget", "50")
+        )
+        self.cellpose_min_seg_size.setItemText(
+            0, _translate("tab_widget", "1")
+        )
+        self.cellpose_min_seg_size.setItemText(
+            1, _translate("tab_widget", "5")
+        )
+        self.cellpose_min_seg_size.setItemText(
+            2, _translate("tab_widget", "10")
+        )
+        self.cellpose_min_seg_size.setItemText(
+            3, _translate("tab_widget", "50")
+        )
+        self.cellpose_clear_previous.setText(
+            _translate("tab_widget", "Clear Previous Segmentations")
+        )
+        self.cellpose_usegpu.setText(
+            _translate("tab_widget", "Use GPU (if Availiable)")
+        )
+        self.cellpose_resetimage.setText(
+            _translate("tab_widget", "Reset Image View After Segmentation")
+        )
+        self.tabWidget_3.setTabText(
+            self.tabWidget_3.indexOf(self.tab_12),
+            _translate("tab_widget", "Settings"),
+        )
+        tab_widget.setTabText(
+            tab_widget.indexOf(self.segement_tab),
+            _translate("tab_widget", "Segment"),
+        )
         self.label_7.setText(_translate("tab_widget", "Interface Modes:"))
         self.modify_panzoom.setText(_translate("tab_widget", "Pan/Zoom [F1]"))
         self.modify_classify.setText(_translate("tab_widget", "Classify [F3]"))
         self.modify_segment.setText(_translate("tab_widget", "Segment [F2]"))
         self.label_98.setText(_translate("tab_widget", "Curate Channel"))
-        self.modify_channel.setItemText(0, _translate("tab_widget", "Segmentations (Cell Wall)"))
-        self.modify_channel.setItemText(1, _translate("tab_widget", "Nucleoid"))
-        self.modify_auto_panzoom.setText(_translate("tab_widget", "Auto select Pan/Zoom after interface event"))
+        self.modify_channel.setItemText(
+            0, _translate("tab_widget", "Segmentations (Cell Wall)")
+        )
+        self.modify_channel.setItemText(
+            1, _translate("tab_widget", "Nucleoid")
+        )
+        self.modify_auto_panzoom.setText(
+            _translate(
+                "tab_widget", "Auto select Pan/Zoom after interface event"
+            )
+        )
         self.label_16.setText(_translate("tab_widget", "Segmentation Modes:"))
         self.modify_refine.setText(_translate("tab_widget", "Refine [R]"))
         self.modify_join.setText(_translate("tab_widget", "Join [J]"))
         self.modify_add.setText(_translate("tab_widget", "Add [A]"))
         self.modify_delete.setText(_translate("tab_widget", "Delete [D]"))
         self.modify_split.setText(_translate("tab_widget", "Split [S]"))
         self.modify_extend.setText(_translate("tab_widget", "Extend [E]"))
-        self.label_28.setText(_translate("tab_widget", "Segmentation Classes:"))
+        self.label_28.setText(
+            _translate("tab_widget", "Segmentation Classes:")
+        )
         self.classify_edge.setText(_translate("tab_widget", "Edge [Ctrl+6]"))
-        self.classify_divided.setText(_translate("tab_widget", "Divided [Ctrl+3]"))
-        self.classify_dividing.setText(_translate("tab_widget", "Dividing [Ctrl+2]"))
-        self.classify_vertical.setText(_translate("tab_widget", "Vertical [Ctrl+4]"))
-        self.classify_broken.setText(_translate("tab_widget", "Broken [Ctrl+5]"))
-        self.classify_single.setText(_translate("tab_widget", "Single [Ctrl+1]"))
+        self.classify_divided.setText(
+            _translate("tab_widget", "Divided [Ctrl+3]")
+        )
+        self.classify_dividing.setText(
+            _translate("tab_widget", "Dividing [Ctrl+2]")
+        )
+        self.classify_vertical.setText(
+            _translate("tab_widget", "Vertical [Ctrl+4]")
+        )
+        self.classify_broken.setText(
+            _translate("tab_widget", "Broken [Ctrl+5]")
+        )
+        self.classify_single.setText(
+            _translate("tab_widget", "Single [Ctrl+1]")
+        )
         self.label_14.setText(_translate("tab_widget", "Image Quality Flags:"))
         self.label_18.setText(_translate("tab_widget", "Mode"))
-        self.set_quality_mode.setItemText(0, _translate("tab_widget", "Active Channel, Active Frame"))
-        self.set_quality_mode.setItemText(1, _translate("tab_widget", "All Channels, Active Frame"))
-        self.set_quality_mode.setItemText(2, _translate("tab_widget", "Active Channel, All Frames"))
-        self.set_quality_mode.setItemText(3, _translate("tab_widget", "All Channels, All Frames"))
+        self.set_quality_mode.setItemText(
+            0, _translate("tab_widget", "Active Channel, Active Frame")
+        )
+        self.set_quality_mode.setItemText(
+            1, _translate("tab_widget", "All Channels, Active Frame")
+        )
+        self.set_quality_mode.setItemText(
+            2, _translate("tab_widget", "Active Channel, All Frames")
+        )
+        self.set_quality_mode.setItemText(
+            3, _translate("tab_widget", "All Channels, All Frames")
+        )
         self.label_34.setText(_translate("tab_widget", "Focus"))
         self.set_focus_2.setText(_translate("tab_widget", "2"))
         self.set_focus_3.setText(_translate("tab_widget", "3"))
         self.set_focus_1.setText(_translate("tab_widget", "1"))
         self.set_focus_4.setText(_translate("tab_widget", "4"))
         self.set_focus_5.setText(_translate("tab_widget", "5"))
         self.set_debris_2.setText(_translate("tab_widget", "2"))
         self.set_debris_3.setText(_translate("tab_widget", "3"))
         self.label_39.setText(_translate("tab_widget", "Debris"))
         self.set_debris_1.setText(_translate("tab_widget", "1"))
         self.set_debris_4.setText(_translate("tab_widget", "4"))
         self.set_debris_5.setText(_translate("tab_widget", "5"))
-        tab_widget.setTabText(tab_widget.indexOf(self.tab_3), _translate("tab_widget", "Curate"))
-        self.label_29.setText(_translate("tab_widget", "Mideline View Mode Toggle [M]"))
+        tab_widget.setTabText(
+            tab_widget.indexOf(self.tab_3), _translate("tab_widget", "Curate")
+        )
+        self.label_29.setText(
+            _translate("tab_widget", "Mideline View Mode Toggle [M]")
+        )
         self.oufti_panzoom_mode.setText(_translate("tab_widget", "Pan/Zoom"))
         self.oufti_edit_mode.setText(_translate("tab_widget", "Edit Midlines"))
-        self.label_20.setText(_translate("tab_widget", "Generate Cell Midlines"))
+        self.label_20.setText(
+            _translate("tab_widget", "Generate Cell Midlines")
+        )
         self.label_25.setText(_translate("tab_widget", "Midline Vertices"))
-        self.oufti_midline_vertexes.setCurrentText(_translate("tab_widget", "5"))
-        self.oufti_midline_vertexes.setItemText(0, _translate("tab_widget", "5"))
-        self.oufti_midline_vertexes.setItemText(1, _translate("tab_widget", "6"))
-        self.oufti_midline_vertexes.setItemText(2, _translate("tab_widget", "7"))
-        self.oufti_midline_vertexes.setItemText(3, _translate("tab_widget", "8"))
-        self.oufti_midline_vertexes.setItemText(4, _translate("tab_widget", "9"))
-        self.oufti_midline_vertexes.setItemText(5, _translate("tab_widget", "10"))
-        self.oufti_generate_active_midlines.setText(_translate("tab_widget", "Generate Midlines (Active Image)"))
-        self.oufti_generate_all_midlines.setText(_translate("tab_widget", "Generate Midlines (All Images)"))
+        self.oufti_midline_vertexes.setCurrentText(
+            _translate("tab_widget", "5")
+        )
+        self.oufti_midline_vertexes.setItemText(
+            0, _translate("tab_widget", "5")
+        )
+        self.oufti_midline_vertexes.setItemText(
+            1, _translate("tab_widget", "6")
+        )
+        self.oufti_midline_vertexes.setItemText(
+            2, _translate("tab_widget", "7")
+        )
+        self.oufti_midline_vertexes.setItemText(
+            3, _translate("tab_widget", "8")
+        )
+        self.oufti_midline_vertexes.setItemText(
+            4, _translate("tab_widget", "9")
+        )
+        self.oufti_midline_vertexes.setItemText(
+            5, _translate("tab_widget", "10")
+        )
+        self.oufti_generate_active_midlines.setText(
+            _translate("tab_widget", "Generate Midlines (Active Image)")
+        )
+        self.oufti_generate_all_midlines.setText(
+            _translate("tab_widget", "Generate Midlines (All Images)")
+        )
         self.label_63.setText(_translate("tab_widget", "Midline Centering"))
-        self.oufti_centre_active_midlines.setText(_translate("tab_widget", "Centre Midlines (Active Image)"))
-        self.oufti_centre_all_midlines.setText(_translate("tab_widget", "Centre Midlines (All Images)"))
-        self.label_61.setText(_translate("tab_widget", "Oufti Export Settings"))
+        self.oufti_centre_active_midlines.setText(
+            _translate("tab_widget", "Centre Midlines (Active Image)")
+        )
+        self.oufti_centre_all_midlines.setText(
+            _translate("tab_widget", "Centre Midlines (All Images)")
+        )
+        self.label_61.setText(
+            _translate("tab_widget", "Oufti Export Settings")
+        )
         self.label_64.setText(_translate("tab_widget", "Target Mesh Length"))
         self.oufti_mesh_length.setItemText(0, _translate("tab_widget", "10"))
         self.oufti_mesh_length.setItemText(1, _translate("tab_widget", "20"))
         self.oufti_mesh_length.setItemText(2, _translate("tab_widget", "30"))
         self.oufti_mesh_length.setItemText(3, _translate("tab_widget", "40"))
         self.oufti_mesh_length.setItemText(4, _translate("tab_widget", "50"))
         self.oufti_mesh_length.setItemText(5, _translate("tab_widget", "100"))
-        self.label_13.setText(_translate("tab_widget", "Mesh Dilation (Pixels)"))
+        self.label_13.setText(
+            _translate("tab_widget", "Mesh Dilation (Pixels)")
+        )
         self.oufti_mesh_dilation.setCurrentText(_translate("tab_widget", "0"))
         self.oufti_mesh_dilation.setItemText(0, _translate("tab_widget", "-2"))
-        self.oufti_mesh_dilation.setItemText(1, _translate("tab_widget", "-1.5"))
+        self.oufti_mesh_dilation.setItemText(
+            1, _translate("tab_widget", "-1.5")
+        )
         self.oufti_mesh_dilation.setItemText(2, _translate("tab_widget", "-1"))
-        self.oufti_mesh_dilation.setItemText(3, _translate("tab_widget", "-0.5"))
-        self.oufti_mesh_dilation.setItemText(4, _translate("tab_widget", "-0.2"))
-        self.oufti_mesh_dilation.setItemText(5, _translate("tab_widget", "-0.1"))
+        self.oufti_mesh_dilation.setItemText(
+            3, _translate("tab_widget", "-0.5")
+        )
+        self.oufti_mesh_dilation.setItemText(
+            4, _translate("tab_widget", "-0.2")
+        )
+        self.oufti_mesh_dilation.setItemText(
+            5, _translate("tab_widget", "-0.1")
+        )
         self.oufti_mesh_dilation.setItemText(6, _translate("tab_widget", "0"))
-        self.oufti_mesh_dilation.setItemText(7, _translate("tab_widget", "0.1"))
-        self.oufti_mesh_dilation.setItemText(8, _translate("tab_widget", "0.2"))
-        self.oufti_mesh_dilation.setItemText(9, _translate("tab_widget", "0.5"))
+        self.oufti_mesh_dilation.setItemText(
+            7, _translate("tab_widget", "0.1")
+        )
+        self.oufti_mesh_dilation.setItemText(
+            8, _translate("tab_widget", "0.2")
+        )
+        self.oufti_mesh_dilation.setItemText(
+            9, _translate("tab_widget", "0.5")
+        )
         self.oufti_mesh_dilation.setItemText(10, _translate("tab_widget", "1"))
-        self.oufti_mesh_dilation.setItemText(11, _translate("tab_widget", "1.5"))
+        self.oufti_mesh_dilation.setItemText(
+            11, _translate("tab_widget", "1.5")
+        )
         self.oufti_mesh_dilation.setItemText(12, _translate("tab_widget", "2"))
-        tab_widget.setTabText(tab_widget.indexOf(self.tab_2), _translate("tab_widget", "Oufti"))
-        self.database_io_title.setText(_translate("tab_widget", "Database I/O"))
-        self.create_database.setText(_translate("tab_widget", "Create Database"))
+        tab_widget.setTabText(
+            tab_widget.indexOf(self.tab_2), _translate("tab_widget", "Oufti")
+        )
+        self.database_io_title.setText(
+            _translate("tab_widget", "Database I/O")
+        )
+        self.create_database.setText(
+            _translate("tab_widget", "Create Database")
+        )
         self.load_database.setText(_translate("tab_widget", "Load Database"))
-        self.display_database_path_label.setText(_translate("tab_widget", "Database Path"))
-        self.display_database_path.setText(_translate("tab_widget", "No database loaded"))
+        self.display_database_path_label.setText(
+            _translate("tab_widget", "Database Path")
+        )
+        self.display_database_path.setText(
+            _translate("tab_widget", "No database loaded")
+        )
         self.label_65.setText(_translate("tab_widget", "User Initial"))
-        self.upload_initial.setItemText(0, _translate("tab_widget", "Required for upload"))
+        self.upload_initial.setItemText(
+            0, _translate("tab_widget", "Required for upload")
+        )
         self.label_74.setText(_translate("tab_widget", "Image Content"))
-        self.upload_content.setItemText(0, _translate("tab_widget", "Required for upload"))
+        self.upload_content.setItemText(
+            0, _translate("tab_widget", "Required for upload")
+        )
         self.label_75.setText(_translate("tab_widget", "Microscope"))
-        self.upload_microscope.setItemText(0, _translate("tab_widget", "Required for upload"))
+        self.upload_microscope.setItemText(
+            0, _translate("tab_widget", "Required for upload")
+        )
         self.label_76.setText(_translate("tab_widget", "Antibiotic"))
-        self.label_77.setText(_translate("tab_widget", "Treatment Time (mins)"))
-        self.label_78.setText(_translate("tab_widget", "Antibiotic Concentration"))
+        self.label_77.setText(
+            _translate("tab_widget", "Treatment Time (mins)")
+        )
+        self.label_78.setText(
+            _translate("tab_widget", "Antibiotic Concentration")
+        )
         self.label_79.setText(_translate("tab_widget", "Mounting Method"))
         self.upload_mount.setItemText(1, _translate("tab_widget", "Agarose"))
         self.upload_mount.setItemText(2, _translate("tab_widget", "Chitosan"))
         self.label_80.setText(_translate("tab_widget", "Protocol"))
-        self.upload_phenotype.setItemText(1, _translate("tab_widget", "Untreated"))
-        self.upload_phenotype.setItemText(2, _translate("tab_widget", "Treated"))
-        self.upload_phenotype.setItemText(3, _translate("tab_widget", "Treated Sensitive"))
-        self.upload_phenotype.setItemText(4, _translate("tab_widget", "Treated Resistant"))
+        self.upload_phenotype.setItemText(
+            1, _translate("tab_widget", "Untreated")
+        )
+        self.upload_phenotype.setItemText(
+            2, _translate("tab_widget", "Treated")
+        )
+        self.upload_phenotype.setItemText(
+            3, _translate("tab_widget", "Treated Sensitive")
+        )
+        self.upload_phenotype.setItemText(
+            4, _translate("tab_widget", "Treated Resistant")
+        )
         self.label_41.setText(_translate("tab_widget", "Phenotype"))
         self.label_42.setText(_translate("tab_widget", "Strain"))
         self.upload_strain.setItemText(1, _translate("tab_widget", "MG1655"))
-        self.metadata_controls.setTabText(self.metadata_controls.indexOf(self.experiment_metadata), _translate("tab_widget", "Experiment Metadata"))
+        self.metadata_controls.setTabText(
+            self.metadata_controls.indexOf(self.experiment_metadata),
+            _translate("tab_widget", "Experiment Metadata"),
+        )
         self.label_67.setText(_translate("tab_widget", "Modality"))
-        self.label_modality.setItemText(0, _translate("tab_widget", "Required for upload"))
-        self.label_modality.setItemText(1, _translate("tab_widget", "Bright Field"))
-        self.label_modality.setItemText(2, _translate("tab_widget", "Dark Field"))
-        self.label_modality.setItemText(3, _translate("tab_widget", "Phase Contrast"))
-        self.label_modality.setItemText(4, _translate("tab_widget", "Fake Phase Contrast"))
-        self.label_modality.setItemText(5, _translate("tab_widget", "Epifluorescence"))
+        self.label_modality.setItemText(
+            0, _translate("tab_widget", "Required for upload")
+        )
+        self.label_modality.setItemText(
+            1, _translate("tab_widget", "Bright Field")
+        )
+        self.label_modality.setItemText(
+            2, _translate("tab_widget", "Dark Field")
+        )
+        self.label_modality.setItemText(
+            3, _translate("tab_widget", "Phase Contrast")
+        )
+        self.label_modality.setItemText(
+            4, _translate("tab_widget", "Fake Phase Contrast")
+        )
+        self.label_modality.setItemText(
+            5, _translate("tab_widget", "Epifluorescence")
+        )
         self.label_modality.setItemText(6, _translate("tab_widget", "HILO"))
         self.label_modality.setItemText(7, _translate("tab_widget", "TIRF"))
         self.label_66.setText(_translate("tab_widget", "Light Source"))
-        self.label_light_source.setItemText(0, _translate("tab_widget", "Required for upload"))
-        self.label_light_source.setItemText(2, _translate("tab_widget", "White Light"))
+        self.label_light_source.setItemText(
+            0, _translate("tab_widget", "Required for upload")
+        )
+        self.label_light_source.setItemText(
+            2, _translate("tab_widget", "White Light")
+        )
         self.label_light_source.setItemText(3, _translate("tab_widget", "LED"))
         self.label_light_source.setItemText(4, _translate("tab_widget", "405"))
         self.label_light_source.setItemText(5, _translate("tab_widget", "514"))
         self.label_light_source.setItemText(6, _translate("tab_widget", "473"))
         self.label_light_source.setItemText(7, _translate("tab_widget", "532"))
         self.label_light_source.setItemText(8, _translate("tab_widget", "640"))
         self.label_68.setText(_translate("tab_widget", "Stain"))
-        self.label_stain.setItemText(0, _translate("tab_widget", "Required for upload"))
+        self.label_stain.setItemText(
+            0, _translate("tab_widget", "Required for upload")
+        )
         self.label_stain.setItemText(2, _translate("tab_widget", "Nile Red"))
         self.label_stain.setItemText(3, _translate("tab_widget", "DAPI"))
         self.label_stain.setItemText(4, _translate("tab_widget", "Cy3"))
         self.label_stain.setItemText(5, _translate("tab_widget", "Cy5"))
         self.label_stain.setItemText(6, _translate("tab_widget", "WGA-488"))
         self.label_stain.setItemText(7, _translate("tab_widget", "WGA-647"))
         self.label_stain.setItemText(8, _translate("tab_widget", "FM4-64"))
         self.label_69.setText(_translate("tab_widget", "Stain Target"))
-        self.label_stain_target.setItemText(0, _translate("tab_widget", "Required for upload"))
-        self.label_stain_target.setItemText(2, _translate("tab_widget", "Membrane"))
-        self.label_stain_target.setItemText(3, _translate("tab_widget", "Ribosome"))
-        self.label_stain_target.setItemText(4, _translate("tab_widget", "Nucleoid"))
-        self.label_overwrite.setText(_translate("tab_widget", "Update Channel Info (Selected Channel)"))
-        self.metadata_controls.setTabText(self.metadata_controls.indexOf(self.image_metadata), _translate("tab_widget", "Image/Channel Metadata"))
+        self.label_stain_target.setItemText(
+            0, _translate("tab_widget", "Required for upload")
+        )
+        self.label_stain_target.setItemText(
+            2, _translate("tab_widget", "Membrane")
+        )
+        self.label_stain_target.setItemText(
+            3, _translate("tab_widget", "Ribosome")
+        )
+        self.label_stain_target.setItemText(
+            4, _translate("tab_widget", "Nucleoid")
+        )
+        self.label_overwrite.setText(
+            _translate("tab_widget", "Update Channel Info (Selected Channel)")
+        )
+        self.metadata_controls.setTabText(
+            self.metadata_controls.indexOf(self.image_metadata),
+            _translate("tab_widget", "Image/Channel Metadata"),
+        )
         self.label_81.setText(_translate("tab_widget", "User Meta #1"))
         self.label_82.setText(_translate("tab_widget", "User Meta #2"))
         self.label_83.setText(_translate("tab_widget", "User Meta #3"))
         self.label_91.setText(_translate("tab_widget", "User Meta #4"))
         self.label_90.setText(_translate("tab_widget", "User Meta #5"))
         self.label_92.setText(_translate("tab_widget", "User Meta #6"))
-        self.metadata_controls.setTabText(self.metadata_controls.indexOf(self.user_metadata), _translate("tab_widget", "User Metadata"))
-        self.update_metadata.setText(_translate("tab_widget", "Update Metadata Categories"))
-        self.label_87.setText(_translate("tab_widget", "Segmentation Metadata"))
+        self.metadata_controls.setTabText(
+            self.metadata_controls.indexOf(self.user_metadata),
+            _translate("tab_widget", "User Metadata"),
+        )
+        self.update_metadata.setText(
+            _translate("tab_widget", "Update Metadata Categories")
+        )
+        self.label_87.setText(
+            _translate("tab_widget", "Segmentation Metadata")
+        )
         self.label_85.setText(_translate("tab_widget", "Segmentation"))
-        self.upload_segmentation_combo.setItemText(1, _translate("tab_widget", "Not Segmented"))
-        self.upload_segmentation_combo.setItemText(2, _translate("tab_widget", "Segmented"))
-        self.upload_segmentation_combo.setItemText(3, _translate("tab_widget", "Curated Segmentations"))
+        self.upload_segmentation_combo.setItemText(
+            1, _translate("tab_widget", "Not Segmented")
+        )
+        self.upload_segmentation_combo.setItemText(
+            2, _translate("tab_widget", "Segmented")
+        )
+        self.upload_segmentation_combo.setItemText(
+            3, _translate("tab_widget", "Curated Segmentations")
+        )
         self.label_84.setText(_translate("tab_widget", "Labelled"))
-        self.upload_label_combo.setItemText(1, _translate("tab_widget", "Not Labelled"))
-        self.upload_label_combo.setItemText(2, _translate("tab_widget", "Labelled"))
-        self.upload_label_combo.setItemText(3, _translate("tab_widget", "Curated Labels"))
-        self.download_sort_order_2.setItemText(1, _translate("tab_widget", "Random"))
-        self.download_sort_order_2.setItemText(2, _translate("tab_widget", "Date Uploaded"))
-        self.download_sort_order_2.setItemText(3, _translate("tab_widget", "Date Modifed"))
-        self.download_sort_order_2.setItemText(4, _translate("tab_widget", "Image Laplacian"))
-        self.download_sort_order_2.setItemText(5, _translate("tab_widget", "Num Segmentations"))
-        self.download_sort_order_2.setItemText(6, _translate("tab_widget", "Image Focus"))
-        self.download_sort_order_2.setItemText(7, _translate("tab_widget", "Image Debris"))
+        self.upload_label_combo.setItemText(
+            1, _translate("tab_widget", "Not Labelled")
+        )
+        self.upload_label_combo.setItemText(
+            2, _translate("tab_widget", "Labelled")
+        )
+        self.upload_label_combo.setItemText(
+            3, _translate("tab_widget", "Curated Labels")
+        )
+        self.download_sort_order_2.setItemText(
+            1, _translate("tab_widget", "Random")
+        )
+        self.download_sort_order_2.setItemText(
+            2, _translate("tab_widget", "Date Uploaded")
+        )
+        self.download_sort_order_2.setItemText(
+            3, _translate("tab_widget", "Date Modifed")
+        )
+        self.download_sort_order_2.setItemText(
+            4, _translate("tab_widget", "Image Laplacian")
+        )
+        self.download_sort_order_2.setItemText(
+            5, _translate("tab_widget", "Num Segmentations")
+        )
+        self.download_sort_order_2.setItemText(
+            6, _translate("tab_widget", "Image Focus")
+        )
+        self.download_sort_order_2.setItemText(
+            7, _translate("tab_widget", "Image Debris")
+        )
         self.label_15.setText(_translate("tab_widget", "Primary Sort Order"))
-        self.download_sort_direction_1.setItemText(1, _translate("tab_widget", "Ascending"))
-        self.download_sort_direction_1.setItemText(2, _translate("tab_widget", "Descending"))
-        self.download_sort_order_1.setItemText(1, _translate("tab_widget", "Random"))
-        self.download_sort_order_1.setItemText(2, _translate("tab_widget", "Date Uploaded"))
-        self.download_sort_order_1.setItemText(3, _translate("tab_widget", "Date Modifed"))
-        self.download_sort_order_1.setItemText(4, _translate("tab_widget", "Image Laplacian"))
-        self.download_sort_order_1.setItemText(5, _translate("tab_widget", "Num Segmentations"))
-        self.download_sort_order_1.setItemText(6, _translate("tab_widget", "Image Focus"))
-        self.download_sort_order_1.setItemText(7, _translate("tab_widget", "Image Debris"))
+        self.download_sort_direction_1.setItemText(
+            1, _translate("tab_widget", "Ascending")
+        )
+        self.download_sort_direction_1.setItemText(
+            2, _translate("tab_widget", "Descending")
+        )
+        self.download_sort_order_1.setItemText(
+            1, _translate("tab_widget", "Random")
+        )
+        self.download_sort_order_1.setItemText(
+            2, _translate("tab_widget", "Date Uploaded")
+        )
+        self.download_sort_order_1.setItemText(
+            3, _translate("tab_widget", "Date Modifed")
+        )
+        self.download_sort_order_1.setItemText(
+            4, _translate("tab_widget", "Image Laplacian")
+        )
+        self.download_sort_order_1.setItemText(
+            5, _translate("tab_widget", "Num Segmentations")
+        )
+        self.download_sort_order_1.setItemText(
+            6, _translate("tab_widget", "Image Focus")
+        )
+        self.download_sort_order_1.setItemText(
+            7, _translate("tab_widget", "Image Debris")
+        )
         self.label_23.setText(_translate("tab_widget", "Secondary Sort Order"))
-        self.download_sort_direction_2.setItemText(1, _translate("tab_widget", "Ascending"))
-        self.download_sort_direction_2.setItemText(2, _translate("tab_widget", "Descending"))
+        self.download_sort_direction_2.setItemText(
+            1, _translate("tab_widget", "Ascending")
+        )
+        self.download_sort_direction_2.setItemText(
+            2, _translate("tab_widget", "Descending")
+        )
         self.label_88.setText(_translate("tab_widget", "Download Limit"))
-        self.database_download_limit.setItemText(0, _translate("tab_widget", "1"))
-        self.database_download_limit.setItemText(1, _translate("tab_widget", "5"))
-        self.database_download_limit.setItemText(2, _translate("tab_widget", "10"))
-        self.database_download_limit.setItemText(3, _translate("tab_widget", "20"))
-        self.database_download_limit.setItemText(4, _translate("tab_widget", "50"))
-        self.database_download_limit.setItemText(5, _translate("tab_widget", "100"))
-        self.database_download_limit.setItemText(6, _translate("tab_widget", "All"))
-        self.database_download.setText(_translate("tab_widget", "Download [Control-L]"))
-        self.tabWidget_2.setTabText(self.tabWidget_2.indexOf(self.tab_10), _translate("tab_widget", "Database Download"))
+        self.database_download_limit.setItemText(
+            0, _translate("tab_widget", "1")
+        )
+        self.database_download_limit.setItemText(
+            1, _translate("tab_widget", "5")
+        )
+        self.database_download_limit.setItemText(
+            2, _translate("tab_widget", "10")
+        )
+        self.database_download_limit.setItemText(
+            3, _translate("tab_widget", "20")
+        )
+        self.database_download_limit.setItemText(
+            4, _translate("tab_widget", "50")
+        )
+        self.database_download_limit.setItemText(
+            5, _translate("tab_widget", "100")
+        )
+        self.database_download_limit.setItemText(
+            6, _translate("tab_widget", "All")
+        )
+        self.database_download.setText(
+            _translate("tab_widget", "Download [Control-L]")
+        )
+        self.tabWidget_2.setTabText(
+            self.tabWidget_2.indexOf(self.tab_10),
+            _translate("tab_widget", "Database Download"),
+        )
         self.label_24.setText(_translate("tab_widget", "Upload Data"))
-        self.upload_segmentations_setting.setText(_translate("tab_widget", "Segmentations/labels"))
+        self.upload_segmentations_setting.setText(
+            _translate("tab_widget", "Segmentations/labels")
+        )
         self.upload_images_setting.setText(_translate("tab_widget", "Images"))
-        self.upload_metadata_setting.setText(_translate("tab_widget", "Metadata"))
+        self.upload_metadata_setting.setText(
+            _translate("tab_widget", "Metadata")
+        )
         self.label_32.setText(_translate("tab_widget", "Upload Settings"))
-        self.upload_overwrite_masks.setText(_translate("tab_widget", "Overwrite Masks/Labels"))
-        self.upload_overwrite_images.setText(_translate("tab_widget", "Overwrite Images"))
-        self.overwrite_all_metadata.setText(_translate("tab_widget", "Overwrite All Metadata"))
-        self.overwrite_selected_metadata.setText(_translate("tab_widget", "Overwrite Selected Metadata"))
-        self.upload_all.setText(_translate("tab_widget", "Upload All Images [Control-Shift-U]"))
-        self.upload_active.setText(_translate("tab_widget", "Upload Active Image [Control-U]"))
-        self.tabWidget_2.setTabText(self.tabWidget_2.indexOf(self.tab_4), _translate("tab_widget", "Database Upload"))
+        self.upload_overwrite_masks.setText(
+            _translate("tab_widget", "Overwrite Masks/Labels")
+        )
+        self.upload_overwrite_images.setText(
+            _translate("tab_widget", "Overwrite Images")
+        )
+        self.overwrite_all_metadata.setText(
+            _translate("tab_widget", "Overwrite All Metadata")
+        )
+        self.overwrite_selected_metadata.setText(
+            _translate("tab_widget", "Overwrite Selected Metadata")
+        )
+        self.upload_all.setText(
+            _translate("tab_widget", "Upload All Images [Control-Shift-U]")
+        )
+        self.upload_active.setText(
+            _translate("tab_widget", "Upload Active Image [Control-U]")
+        )
+        self.tabWidget_2.setTabText(
+            self.tabWidget_2.indexOf(self.tab_4),
+            _translate("tab_widget", "Database Upload"),
+        )
         self.label_89.setText(_translate("tab_widget", "Progress"))
-        tab_widget.setTabText(tab_widget.indexOf(self.upload_tab), _translate("tab_widget", "Database"))
-        self.export_mode.setItemText(0, _translate("tab_widget", "Export .tif Images"))
-        self.export_mode.setItemText(1, _translate("tab_widget", "Export .tif Masks"))
-        self.export_mode.setItemText(2, _translate("tab_widget", "Export .tif Images and Masks"))
-        self.export_mode.setItemText(3, _translate("tab_widget", "Export Cellpose"))
-        self.export_mode.setItemText(4, _translate("tab_widget", "Export Oufti"))
-        self.export_mode.setItemText(5, _translate("tab_widget", "Export ImageJ"))
-        self.export_mode.setItemText(6, _translate("tab_widget", "Export JSON"))
+        tab_widget.setTabText(
+            tab_widget.indexOf(self.upload_tab),
+            _translate("tab_widget", "Database"),
+        )
+        self.export_mode.setItemText(
+            0, _translate("tab_widget", "Export .tif Images")
+        )
+        self.export_mode.setItemText(
+            1, _translate("tab_widget", "Export .tif Masks")
+        )
+        self.export_mode.setItemText(
+            2, _translate("tab_widget", "Export .tif Images and Masks")
+        )
+        self.export_mode.setItemText(
+            3, _translate("tab_widget", "Export Cellpose")
+        )
+        self.export_mode.setItemText(
+            4, _translate("tab_widget", "Export Oufti")
+        )
+        self.export_mode.setItemText(
+            5, _translate("tab_widget", "Export ImageJ")
+        )
+        self.export_mode.setItemText(
+            6, _translate("tab_widget", "Export JSON")
+        )
         self.export_mode.setItemText(7, _translate("tab_widget", "Export CSV"))
         self.label_19.setText(_translate("tab_widget", "Export Mode"))
-        self.export_location.setItemText(0, _translate("tab_widget", "Import Directory"))
-        self.export_location.setItemText(1, _translate("tab_widget", "Select Directory"))
+        self.export_location.setItemText(
+            0, _translate("tab_widget", "Import Directory")
+        )
+        self.export_location.setItemText(
+            1, _translate("tab_widget", "Select Directory")
+        )
         self.label_44.setText(_translate("tab_widget", "Export Location"))
-        self.export_channel.setItemText(0, _translate("tab_widget", "All Channels (Stack)"))
-        self.export_channel.setItemText(1, _translate("tab_widget", "First Three Channels (RGB)"))
+        self.export_channel.setItemText(
+            0, _translate("tab_widget", "All Channels (Stack)")
+        )
+        self.export_channel.setItemText(
+            1, _translate("tab_widget", "First Three Channels (RGB)")
+        )
         self.label_45.setText(_translate("tab_widget", "Image Channel"))
         self.label_26.setText(_translate("tab_widget", "File Name Modifier"))
         self.export_modifier.setText(_translate("tab_widget", "_BacSeg"))
-        self.export_image_setting.setText(_translate("tab_widget", "Export Image Files"))
-        self.export_overwrite_setting.setText(_translate("tab_widget", "Overwrite Files"))
-        self.export_active.setText(_translate("tab_widget", "Export Image From Active Frame"))
-        self.export_all.setText(_translate("tab_widget", "Export Image From All Frames"))
-        self.tabWidget.setTabText(self.tabWidget.indexOf(self.tab_18), _translate("tab_widget", "Export Frames"))
+        self.export_image_setting.setText(
+            _translate("tab_widget", "Export Image Files")
+        )
+        self.export_overwrite_setting.setText(
+            _translate("tab_widget", "Overwrite Files")
+        )
+        self.export_active.setText(
+            _translate("tab_widget", "Export Image From Active Frame")
+        )
+        self.export_all.setText(
+            _translate("tab_widget", "Export Image From All Frames")
+        )
+        self.tabWidget.setTabText(
+            self.tabWidget.indexOf(self.tab_18),
+            _translate("tab_widget", "Export Frames"),
+        )
         self.label_101.setText(_translate("tab_widget", "Image Channel"))
         self.label_99.setText(_translate("tab_widget", "Export Mode"))
-        self.export_stack_mode.setItemText(0, _translate("tab_widget", "Export .tif Images"))
-        self.export_stack_mode.setItemText(1, _translate("tab_widget", "Export .tif Masks"))
+        self.export_stack_mode.setItemText(
+            0, _translate("tab_widget", "Export .tif Images")
+        )
+        self.export_stack_mode.setItemText(
+            1, _translate("tab_widget", "Export .tif Masks")
+        )
         self.label_100.setText(_translate("tab_widget", "Export Location"))
-        self.export_stack_location.setItemText(0, _translate("tab_widget", "Import Directory"))
-        self.export_stack_location.setItemText(1, _translate("tab_widget", "Select Directory"))
+        self.export_stack_location.setItemText(
+            0, _translate("tab_widget", "Import Directory")
+        )
+        self.export_stack_location.setItemText(
+            1, _translate("tab_widget", "Select Directory")
+        )
         self.label_103.setText(_translate("tab_widget", "File Name Modifier"))
         self.export_stack_modifier.setText(_translate("tab_widget", "_BacSeg"))
-        self.export_stack_image_setting.setText(_translate("tab_widget", "Export Image Files"))
-        self.export_stack_overwrite_setting.setText(_translate("tab_widget", "Overwrite Files"))
-        self.export_stack_active.setText(_translate("tab_widget", "Export Image Stack From Selected Channel"))
-        self.export_stack_all.setText(_translate("tab_widget", "Export Image Stack From All Channels"))
-        self.tabWidget.setTabText(self.tabWidget.indexOf(self.tab_19), _translate("tab_widget", "Export Stacks"))
+        self.export_stack_image_setting.setText(
+            _translate("tab_widget", "Export Image Files")
+        )
+        self.export_stack_overwrite_setting.setText(
+            _translate("tab_widget", "Overwrite Files")
+        )
+        self.export_stack_active.setText(
+            _translate(
+                "tab_widget", "Export Image Stack From Selected Channel"
+            )
+        )
+        self.export_stack_all.setText(
+            _translate("tab_widget", "Export Image Stack From All Channels")
+        )
+        self.tabWidget.setTabText(
+            self.tabWidget.indexOf(self.tab_19),
+            _translate("tab_widget", "Export Stacks"),
+        )
         self.label_43.setText(_translate("tab_widget", "Export Cell Settings"))
         self.export_single.setText(_translate("tab_widget", "Single"))
         self.export_vertical.setText(_translate("tab_widget", "Vertical"))
         self.export_divided.setText(_translate("tab_widget", "Divided"))
         self.export_dividing.setText(_translate("tab_widget", "Dividing"))
         self.export_edge.setText(_translate("tab_widget", "Edge"))
         self.export_broken.setText(_translate("tab_widget", "Broken"))
         self.label_49.setText(_translate("tab_widget", "Scale Bar Settings"))
-        self.export_scalebar_resolution_units.setItemText(0, _translate("tab_widget", "nm"))
-        self.export_scalebar_resolution_units.setItemText(1, _translate("tab_widget", "um"))
+        self.export_scalebar_resolution_units.setItemText(
+            0, _translate("tab_widget", "nm")
+        )
+        self.export_scalebar_resolution_units.setItemText(
+            1, _translate("tab_widget", "um")
+        )
         self.label_50.setText(_translate("tab_widget", "Pixel Resolution"))
-        self.export_scalebar_resolution.setText(_translate("tab_widget", "100"))
+        self.export_scalebar_resolution.setText(
+            _translate("tab_widget", "100")
+        )
         self.label_55.setText(_translate("tab_widget", "Scale Bar Size"))
         self.export_scalebar_size.setText(_translate("tab_widget", "20"))
-        self.export_scalebar_size_units.setItemText(0, _translate("tab_widget", "nm"))
-        self.export_scalebar_size_units.setItemText(1, _translate("tab_widget", "um"))
+        self.export_scalebar_size_units.setItemText(
+            0, _translate("tab_widget", "nm")
+        )
+        self.export_scalebar_size_units.setItemText(
+            1, _translate("tab_widget", "um")
+        )
         self.label_71.setText(_translate("tab_widget", "Scale Bar Colour"))
-        self.export_scalebar_colour.setItemText(0, _translate("tab_widget", "Black"))
-        self.export_scalebar_colour.setItemText(1, _translate("tab_widget", "White"))
-        self.label_72.setText(_translate("tab_widget", "Scale Bar Thickness (pixels)"))
-        self.export_scalebar_thickness.setItemText(0, _translate("tab_widget", "1"))
-        self.export_scalebar_thickness.setItemText(1, _translate("tab_widget", "2"))
-        self.export_scalebar_thickness.setItemText(2, _translate("tab_widget", "5"))
-        self.export_scalebar_thickness.setItemText(3, _translate("tab_widget", "10"))
-        self.export_scalebar_thickness.setItemText(4, _translate("tab_widget", "15"))
-        self.export_scalebar_thickness.setItemText(5, _translate("tab_widget", "20"))
+        self.export_scalebar_colour.setItemText(
+            0, _translate("tab_widget", "Black")
+        )
+        self.export_scalebar_colour.setItemText(
+            1, _translate("tab_widget", "White")
+        )
+        self.label_72.setText(
+            _translate("tab_widget", "Scale Bar Thickness (pixels)")
+        )
+        self.export_scalebar_thickness.setItemText(
+            0, _translate("tab_widget", "1")
+        )
+        self.export_scalebar_thickness.setItemText(
+            1, _translate("tab_widget", "2")
+        )
+        self.export_scalebar_thickness.setItemText(
+            2, _translate("tab_widget", "5")
+        )
+        self.export_scalebar_thickness.setItemText(
+            3, _translate("tab_widget", "10")
+        )
+        self.export_scalebar_thickness.setItemText(
+            4, _translate("tab_widget", "15")
+        )
+        self.export_scalebar_thickness.setItemText(
+            5, _translate("tab_widget", "20")
+        )
         self.label_12.setText(_translate("tab_widget", "Image Modifications"))
-        self.export_autocontrast.setText(_translate("tab_widget", "Auto Contrast"))
+        self.export_autocontrast.setText(
+            _translate("tab_widget", "Auto Contrast")
+        )
         self.export_normalise.setText(_translate("tab_widget", "Normalise"))
-        self.export_scalebar.setText(_translate("tab_widget", "Show Scale Bar"))
+        self.export_scalebar.setText(
+            _translate("tab_widget", "Show Scale Bar")
+        )
         self.export_invert.setText(_translate("tab_widget", "Invert "))
-        self.export_mask_background.setText(_translate("tab_widget", "Mask Background"))
-        self.export_crop_zoom.setText(_translate("tab_widget", "Crop to Current Zoom"))
-        self.tabWidget.setTabText(self.tabWidget.indexOf(self.tab_20), _translate("tab_widget", "Export Settings"))
-        self.tabWidget_4.setTabText(self.tabWidget_4.indexOf(self.tab_8), _translate("tab_widget", "Export Data"))
-        self.label_46.setText(_translate("tab_widget", "Export Cell Statistics"))
+        self.export_mask_background.setText(
+            _translate("tab_widget", "Mask Background")
+        )
+        self.export_crop_zoom.setText(
+            _translate("tab_widget", "Crop to Current Zoom")
+        )
+        self.tabWidget.setTabText(
+            self.tabWidget.indexOf(self.tab_20),
+            _translate("tab_widget", "Export Settings"),
+        )
+        self.tabWidget_4.setTabText(
+            self.tabWidget_4.indexOf(self.tab_8),
+            _translate("tab_widget", "Export Data"),
+        )
+        self.label_46.setText(
+            _translate("tab_widget", "Export Cell Statistics")
+        )
         self.label_54.setText(_translate("tab_widget", "ColiCoords Fit Mode"))
-        self.export_statistics_pixelsize.setText(_translate("tab_widget", "0.116999998688698"))
-        self.export_colicoords_mode.setItemText(0, _translate("tab_widget", "None (OpenCV Stats)"))
-        self.export_colicoords_mode.setItemText(1, _translate("tab_widget", "Mask"))
+        self.export_statistics_pixelsize.setText(
+            _translate("tab_widget", "0.116999998688698")
+        )
+        self.export_colicoords_mode.setItemText(
+            0, _translate("tab_widget", "None (OpenCV Stats)")
+        )
+        self.export_colicoords_mode.setItemText(
+            1, _translate("tab_widget", "Mask")
+        )
         self.label_52.setText(_translate("tab_widget", "Pixel Size (um)"))
-        self.export_statistics_multithreaded.setText(_translate("tab_widget", "Multithreaded Processing"))
-        self.export_statistics_active.setText(_translate("tab_widget", "Export Cell Statistics From Active Image"))
-        self.export_statistics_all.setText(_translate("tab_widget", "Export Cell Statistics From All Images"))
-        self.tabWidget_4.setTabText(self.tabWidget_4.indexOf(self.tab_9), _translate("tab_widget", "Export Statistics"))
+        self.export_statistics_multithreaded.setText(
+            _translate("tab_widget", "Multithreaded Processing")
+        )
+        self.export_statistics_active.setText(
+            _translate(
+                "tab_widget", "Export Cell Statistics From Active Image"
+            )
+        )
+        self.export_statistics_all.setText(
+            _translate("tab_widget", "Export Cell Statistics From All Images")
+        )
+        self.tabWidget_4.setTabText(
+            self.tabWidget_4.indexOf(self.tab_9),
+            _translate("tab_widget", "Export Statistics"),
+        )
         self.label_33.setText(_translate("tab_widget", "Progress "))
-        tab_widget.setTabText(tab_widget.indexOf(self.export_tab), _translate("tab_widget", "Export"))
-        self.modify_copymasktoall.setText(_translate("tab_widget", "Copy Mask From Active Image to All Images"))
-        self.modify_deleteactiveimage.setText(_translate("tab_widget", "Delete Active Image [Control-I]"))
-        self.modify_deleteotherimages.setText(_translate("tab_widget", "Delete All Images Except Active Image [Control-Shift-I]"))
-        self.modify_deleteactivemasks.setText(_translate("tab_widget", "Delete All Masks, Active Image [Control-D]"))
-        self.modify_deleteallmasks.setText(_translate("tab_widget", "Delete All Masks, All Images [Control-Shift-D]"))
-        self.label_31.setText(_translate("tab_widget", "Refine Settings (ColiCoords):"))
+        tab_widget.setTabText(
+            tab_widget.indexOf(self.export_tab),
+            _translate("tab_widget", "Export"),
+        )
+        self.modify_copymasktoall.setText(
+            _translate(
+                "tab_widget", "Copy Mask From Active Image to All Images"
+            )
+        )
+        self.modify_deleteactiveimage.setText(
+            _translate("tab_widget", "Delete Active Image [Control-I]")
+        )
+        self.modify_deleteotherimages.setText(
+            _translate(
+                "tab_widget",
+                "Delete All Images Except Active Image [Control-Shift-I]",
+            )
+        )
+        self.modify_deleteactivemasks.setText(
+            _translate(
+                "tab_widget", "Delete All Masks, Active Image [Control-D]"
+            )
+        )
+        self.modify_deleteallmasks.setText(
+            _translate(
+                "tab_widget", "Delete All Masks, All Images [Control-Shift-D]"
+            )
+        )
+        self.label_31.setText(
+            _translate("tab_widget", "Refine Settings (ColiCoords):")
+        )
         self.label_53.setText(_translate("tab_widget", "Refine Channel"))
         self.refine_channel.setItemText(0, _translate("tab_widget", "Mask"))
-        self.refine_all.setText(_translate("tab_widget", "Refine All Segmentations In Active Image"))
+        self.refine_all.setText(
+            _translate(
+                "tab_widget", "Refine All Segmentations In Active Image"
+            )
+        )
         self.label_17.setText(_translate("tab_widget", "Progress"))
         self.label_56.setText(_translate("tab_widget", "Find/Sort Cells"))
         self.find_previous.setText(_translate("tab_widget", "Find Previous"))
         self.find_mode.setItemText(0, _translate("tab_widget", "Ascending"))
         self.find_mode.setItemText(1, _translate("tab_widget", "Descending"))
         self.find_next.setText(_translate("tab_widget", "Find Next"))
-        self.find_criterion.setItemText(0, _translate("tab_widget", "Cell Area"))
-        self.find_criterion.setItemText(1, _translate("tab_widget", "Cell Solidity"))
-        self.find_criterion.setItemText(2, _translate("tab_widget", "Cell Aspect Ratio"))
-        self.label_70.setText(_translate("tab_widget", "Automatic Channel Alignment/Registration"))
+        self.find_criterion.setItemText(
+            0, _translate("tab_widget", "Cell Area")
+        )
+        self.find_criterion.setItemText(
+            1, _translate("tab_widget", "Cell Solidity")
+        )
+        self.find_criterion.setItemText(
+            2, _translate("tab_widget", "Cell Aspect Ratio")
+        )
+        self.label_70.setText(
+            _translate(
+                "tab_widget", "Automatic Channel Alignment/Registration"
+            )
+        )
         self.label_40.setText(_translate("tab_widget", "Reference Channel"))
-        self.align_active_image.setText(_translate("tab_widget", "Align Active Image"))
-        self.align_all_images.setText(_translate("tab_widget", "Align All Images"))
-        tab_widget.setTabText(tab_widget.indexOf(self.tab_14), _translate("tab_widget", "Utilities"))
+        self.align_active_image.setText(
+            _translate("tab_widget", "Align Active Image")
+        )
+        self.align_all_images.setText(
+            _translate("tab_widget", "Align All Images")
+        )
+        tab_widget.setTabText(
+            tab_widget.indexOf(self.tab_14),
+            _translate("tab_widget", "Utilities"),
+        )
```

### Comparing `napari-bacseg-1.0.8/src/napari_bacseg/bacseg_ui.ui` & `napari-bacseg-1.0.9/src/napari_bacseg/bacseg_ui.ui`

 * *Files 0% similar despite different names*

#### Comparing `napari-bacseg-1.0.8/src/napari_bacseg/bacseg_ui.ui` & `napari-bacseg-1.0.9/src/napari_bacseg/bacseg_ui.ui`

```diff
@@ -297,14 +297,19 @@
                 <item>
                   <property name="text">
                     <string>ScanR Data</string>
                   </property>
                 </item>
                 <item>
                   <property name="text">
+                    <string>Zeiss (.czi) Data</string>
+                  </property>
+                </item>
+                <item>
+                  <property name="text">
                     <string>ImageJ files(s)</string>
                   </property>
                 </item>
                 <item>
                   <property name="text">
                     <string>Mask (.tif) Segmentation(s)</string>
                   </property>
```

### Comparing `napari-bacseg-1.0.8/src/napari_bacseg.egg-info/PKG-INFO` & `napari-bacseg-1.0.9/src/napari_bacseg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-bacseg
-Version: 1.0.8
+Version: 1.0.9
 Summary: Bacterial segmentation and analysis platform than can inport/export files in multiple formats. Integrating many tools such as Cellpose, ColiCoords, Oufti/MicrobeTracker.
 Home-page: https://github.com/piedrro/napari-bacseg
 Author: Piers Turner
 Author-email: Piers Turner <piers.turner@physics.ox.ac.uk>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/piedrro/napari-bacseg
 Project-URL: Bug Tracker, https://github.com/piedrro/napari-bacseg/issues
```

### Comparing `napari-bacseg-1.0.8/src/napari_bacseg.egg-info/SOURCES.txt` & `napari-bacseg-1.0.9/src/napari_bacseg.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 src/_dev/oufti_dilate_with_midlines.py
 src/_dev/pandas_speed.py
 src/_dev/process_alex_datadump.py
 src/_dev/process_alex_datadump_clinical.py
 src/_dev/process_conor_datadump.py
 src/_dev/process_gramstain_datadump.py
 src/_dev/read_non_tif.py
+src/_dev/read_trillian.py
 src/_dev/rebuild_usermeta.py
 src/_dev/rebuild_usermeta_2.py
 src/_dev/recreate_user_metadata.py
 src/_dev/scalebar_dev.py
 src/_dev/sort_midlines.py
 src/_dev/stelios_stats.py
 src/_dev/tile_meta_check.py
@@ -88,14 +89,15 @@
 src/napari_bacseg/_utils_imagej.py
 src/napari_bacseg/_utils_interface_events.py
 src/napari_bacseg/_utils_json.py
 src/napari_bacseg/_utils_oufti.py
 src/napari_bacseg/_utils_refine.py
 src/napari_bacseg/_utils_statistics.py
 src/napari_bacseg/_utils_tiler.py
+src/napari_bacseg/_utils_zeiss.py
 src/napari_bacseg/_version.py
 src/napari_bacseg/_widget.py
 src/napari_bacseg/bacseg_ui.py
 src/napari_bacseg/bacseg_ui.ui
 src/napari_bacseg/gapseq_ui.py
 src/napari_bacseg/napari.yaml
 src/napari_bacseg/napari_ui.py
```

### Comparing `napari-bacseg-1.0.8/tox.ini` & `napari-bacseg-1.0.9/tox.ini`

 * *Files identical despite different names*

