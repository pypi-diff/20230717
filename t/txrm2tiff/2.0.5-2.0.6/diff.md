# Comparing `tmp/txrm2tiff-2.0.5.tar.gz` & `tmp/txrm2tiff-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/rky95813/Documents/Eclipse2/txrm2tiff/dist/.tmp-m109fkua/txrm2tiff-2.0.5.tar", last modified: Wed Jul 12 14:48:02 2023, max compression
+gzip compressed data, was "/home/rky95813/Documents/Eclipse2/txrm2tiff/dist/.tmp-lchvb1le/txrm2tiff-2.0.6.tar", last modified: Mon Jul 17 14:01:02 2023, max compression
```

## Comparing `txrm2tiff-2.0.5.tar` & `txrm2tiff-2.0.6.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-12 14:48:02.000000 txrm2tiff-2.0.5/
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1290 2023-07-10 08:58:14.000000 txrm2tiff-2.0.5/.gitignore
-drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-12 14:48:01.000000 txrm2tiff-2.0.5/.settings/
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       64 2020-03-30 17:10:47.000000 txrm2tiff-2.0.5/.settings/org.eclipse.core.resources.prefs
-drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-12 14:48:01.000000 txrm2tiff-2.0.5/.vscode/
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      638 2021-03-02 11:54:13.000000 txrm2tiff-2.0.5/.vscode/launch.json
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      766 2023-05-30 18:11:44.000000 txrm2tiff-2.0.5/.vscode/settings.json
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1533 2020-03-30 17:10:47.000000 txrm2tiff-2.0.5/LICENSE
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     7445 2023-07-12 14:48:02.000000 txrm2tiff-2.0.5/PKG-INFO
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     6967 2021-11-26 16:04:02.000000 txrm2tiff-2.0.5/README.md
-drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-12 14:48:01.000000 txrm2tiff-2.0.5/conda/
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1473 2023-07-10 10:33:15.000000 txrm2tiff-2.0.5/conda/meta.yaml
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1536 2023-07-07 14:59:26.000000 txrm2tiff-2.0.5/pyproject.toml
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       38 2023-07-12 14:48:02.000000 txrm2tiff-2.0.5/setup.cfg
-drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-12 14:48:01.000000 txrm2tiff-2.0.5/src/
-drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-12 14:48:01.000000 txrm2tiff-2.0.5/src/txrm2tiff/
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      122 2023-05-30 10:44:58.000000 txrm2tiff-2.0.5/src/txrm2tiff/__init__.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     5966 2023-05-30 10:44:58.000000 txrm2tiff-2.0.5/src/txrm2tiff/__main__.py
-drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-12 14:48:02.000000 txrm2tiff-2.0.5/src/txrm2tiff/font/
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)    42884 2021-02-08 17:40:15.000000 txrm2tiff-2.0.5/src/txrm2tiff/font/CallingCode-Regular.otf
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1554 2021-02-08 17:40:15.000000 txrm2tiff-2.0.5/src/txrm2tiff/font/License.txt
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       89 2023-07-10 10:33:15.000000 txrm2tiff-2.0.5/src/txrm2tiff/info.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     6531 2023-05-30 10:44:58.000000 txrm2tiff-2.0.5/src/txrm2tiff/inspector.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     7057 2023-05-30 10:44:58.000000 txrm2tiff-2.0.5/src/txrm2tiff/main.py
-drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-12 14:48:02.000000 txrm2tiff-2.0.5/src/txrm2tiff/txrm/
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       28 2021-12-01 16:06:26.000000 txrm2tiff-2.0.5/src/txrm2tiff/txrm/__init__.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)    18841 2023-05-30 10:44:58.000000 txrm2tiff-2.0.5/src/txrm2tiff/txrm/abstract.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)    12824 2023-05-30 15:24:48.000000 txrm2tiff-2.0.5/src/txrm2tiff/txrm/annot_mixin.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1357 2021-12-14 13:07:27.000000 txrm2tiff-2.0.5/src/txrm2tiff/txrm/main.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     8432 2023-05-30 10:24:41.000000 txrm2tiff-2.0.5/src/txrm2tiff/txrm/ref_mixin.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     3080 2023-05-30 14:59:57.000000 txrm2tiff-2.0.5/src/txrm2tiff/txrm/save_mixin.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1623 2021-12-01 16:29:22.000000 txrm2tiff-2.0.5/src/txrm2tiff/txrm/shifts_mixin.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1560 2023-05-30 10:24:37.000000 txrm2tiff-2.0.5/src/txrm2tiff/txrm/txrm_property.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     3158 2023-05-30 10:24:41.000000 txrm2tiff-2.0.5/src/txrm2tiff/txrm/v3.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     2928 2023-05-30 10:24:41.000000 txrm2tiff-2.0.5/src/txrm2tiff/txrm/v5.py
-drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-12 14:48:02.000000 txrm2tiff-2.0.5/src/txrm2tiff/txrm_functions/
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       45 2021-11-26 16:04:02.000000 txrm2tiff-2.0.5/src/txrm2tiff/txrm_functions/__init__.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     4667 2023-05-30 10:44:58.000000 txrm2tiff-2.0.5/src/txrm2tiff/txrm_functions/general.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     2649 2021-12-01 16:08:13.000000 txrm2tiff-2.0.5/src/txrm2tiff/txrm_functions/images.py
-drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-12 14:48:02.000000 txrm2tiff-2.0.5/src/txrm2tiff/utils/
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)        0 2021-11-26 16:04:02.000000 txrm2tiff-2.0.5/src/txrm2tiff/utils/__init__.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     4619 2023-07-10 10:33:15.000000 txrm2tiff-2.0.5/src/txrm2tiff/utils/file_handler.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      415 2021-11-26 16:04:02.000000 txrm2tiff-2.0.5/src/txrm2tiff/utils/functions.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     6400 2023-05-30 10:44:58.000000 txrm2tiff-2.0.5/src/txrm2tiff/utils/image_processing.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      818 2021-11-26 16:04:02.000000 txrm2tiff-2.0.5/src/txrm2tiff/utils/logging.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     5618 2023-07-07 17:08:26.000000 txrm2tiff-2.0.5/src/txrm2tiff/utils/metadata.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     2570 2021-11-26 16:04:02.000000 txrm2tiff-2.0.5/src/txrm2tiff/utils/shortcut_creation.py
-drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-12 14:48:02.000000 txrm2tiff-2.0.5/src/txrm2tiff/xradia_properties/
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       50 2021-11-26 16:04:02.000000 txrm2tiff-2.0.5/src/txrm2tiff/xradia_properties/__init__.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1856 2023-05-30 10:24:41.000000 txrm2tiff-2.0.5/src/txrm2tiff/xradia_properties/enums.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     3334 2023-05-30 10:44:58.000000 txrm2tiff-2.0.5/src/txrm2tiff/xradia_properties/stream_dtypes.py
-drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-12 14:48:02.000000 txrm2tiff-2.0.5/src/txrm2tiff.egg-info/
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     7445 2023-07-12 14:48:01.000000 txrm2tiff-2.0.5/src/txrm2tiff.egg-info/PKG-INFO
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1853 2023-07-12 14:48:01.000000 txrm2tiff-2.0.5/src/txrm2tiff.egg-info/SOURCES.txt
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)        1 2023-07-12 14:48:01.000000 txrm2tiff-2.0.5/src/txrm2tiff.egg-info/dependency_links.txt
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       54 2023-07-12 14:48:01.000000 txrm2tiff-2.0.5/src/txrm2tiff.egg-info/entry_points.txt
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      170 2023-07-12 14:48:01.000000 txrm2tiff-2.0.5/src/txrm2tiff.egg-info/requires.txt
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       10 2023-07-12 14:48:01.000000 txrm2tiff-2.0.5/src/txrm2tiff.egg-info/top_level.txt
-drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-12 14:48:02.000000 txrm2tiff-2.0.5/tests/
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      193 2021-02-08 17:40:15.000000 txrm2tiff-2.0.5/tests/__init__.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)    11184 2023-05-30 10:44:58.000000 txrm2tiff-2.0.5/tests/test_abstract_txrm.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)    10711 2023-05-30 10:44:58.000000 txrm2tiff-2.0.5/tests/test_annotator.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     9650 2023-05-30 10:44:58.000000 txrm2tiff-2.0.5/tests/test_commandline_entrypoint.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     5655 2023-07-10 10:33:15.000000 txrm2tiff-2.0.5/tests/test_file_handler.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     5849 2023-05-30 10:44:58.000000 txrm2tiff-2.0.5/tests/test_image_processing.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     2777 2021-12-01 16:29:22.000000 txrm2tiff-2.0.5/tests/test_inspector.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)    14713 2023-05-30 10:44:58.000000 txrm2tiff-2.0.5/tests/test_main.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     4036 2023-05-30 10:24:41.000000 txrm2tiff-2.0.5/tests/test_metadata.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     3858 2023-07-07 17:26:47.000000 txrm2tiff-2.0.5/tests/test_referencer.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     9936 2023-05-30 16:23:06.000000 txrm2tiff-2.0.5/tests/test_saver.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1455 2021-12-01 16:07:16.000000 txrm2tiff-2.0.5/tests/test_setup_fuctions.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     2246 2021-12-01 16:29:22.000000 txrm2tiff-2.0.5/tests/test_shifts.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     5057 2021-12-01 16:07:23.000000 txrm2tiff-2.0.5/tests/test_txrm_functions.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     2682 2023-05-30 10:44:58.000000 txrm2tiff-2.0.5/tests/test_txrm_property.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     3709 2023-05-30 15:25:01.000000 txrm2tiff-2.0.5/tests/test_txrm_v5.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     6007 2023-05-30 15:10:23.000000 txrm2tiff-2.0.5/tests/test_txrmv3.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      834 2021-12-01 16:07:35.000000 txrm2tiff-2.0.5/tests/test_util_functions.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     7056 2021-12-14 13:07:27.000000 txrm2tiff-2.0.5/tests/test_with_files.py
+drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-17 14:01:02.000000 txrm2tiff-2.0.6/
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1290 2023-07-10 08:58:14.000000 txrm2tiff-2.0.6/.gitignore
+drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-17 14:01:01.000000 txrm2tiff-2.0.6/.settings/
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       64 2020-03-30 17:10:47.000000 txrm2tiff-2.0.6/.settings/org.eclipse.core.resources.prefs
+drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-17 14:01:01.000000 txrm2tiff-2.0.6/.vscode/
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      638 2021-03-02 11:54:13.000000 txrm2tiff-2.0.6/.vscode/launch.json
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      766 2023-05-30 18:11:44.000000 txrm2tiff-2.0.6/.vscode/settings.json
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1533 2020-03-30 17:10:47.000000 txrm2tiff-2.0.6/LICENSE
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     7445 2023-07-17 14:01:02.000000 txrm2tiff-2.0.6/PKG-INFO
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     6967 2021-11-26 16:04:02.000000 txrm2tiff-2.0.6/README.md
+drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-17 14:01:01.000000 txrm2tiff-2.0.6/conda/
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1473 2023-07-17 13:59:18.000000 txrm2tiff-2.0.6/conda/meta.yaml
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1536 2023-07-07 14:59:26.000000 txrm2tiff-2.0.6/pyproject.toml
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       38 2023-07-17 14:01:02.000000 txrm2tiff-2.0.6/setup.cfg
+drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-17 14:01:01.000000 txrm2tiff-2.0.6/src/
+drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-17 14:01:01.000000 txrm2tiff-2.0.6/src/txrm2tiff/
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      122 2023-05-30 10:44:58.000000 txrm2tiff-2.0.6/src/txrm2tiff/__init__.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     5966 2023-05-30 10:44:58.000000 txrm2tiff-2.0.6/src/txrm2tiff/__main__.py
+drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-17 14:01:01.000000 txrm2tiff-2.0.6/src/txrm2tiff/font/
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)    42884 2021-02-08 17:40:15.000000 txrm2tiff-2.0.6/src/txrm2tiff/font/CallingCode-Regular.otf
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1554 2021-02-08 17:40:15.000000 txrm2tiff-2.0.6/src/txrm2tiff/font/License.txt
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       89 2023-07-17 13:59:18.000000 txrm2tiff-2.0.6/src/txrm2tiff/info.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     6531 2023-05-30 10:44:58.000000 txrm2tiff-2.0.6/src/txrm2tiff/inspector.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     7057 2023-05-30 10:44:58.000000 txrm2tiff-2.0.6/src/txrm2tiff/main.py
+drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-17 14:01:01.000000 txrm2tiff-2.0.6/src/txrm2tiff/txrm/
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       28 2021-12-01 16:06:26.000000 txrm2tiff-2.0.6/src/txrm2tiff/txrm/__init__.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)    18841 2023-05-30 10:44:58.000000 txrm2tiff-2.0.6/src/txrm2tiff/txrm/abstract.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)    12824 2023-05-30 15:24:48.000000 txrm2tiff-2.0.6/src/txrm2tiff/txrm/annot_mixin.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1357 2021-12-14 13:07:27.000000 txrm2tiff-2.0.6/src/txrm2tiff/txrm/main.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     8432 2023-05-30 10:24:41.000000 txrm2tiff-2.0.6/src/txrm2tiff/txrm/ref_mixin.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     3080 2023-05-30 14:59:57.000000 txrm2tiff-2.0.6/src/txrm2tiff/txrm/save_mixin.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1623 2021-12-01 16:29:22.000000 txrm2tiff-2.0.6/src/txrm2tiff/txrm/shifts_mixin.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1560 2023-05-30 10:24:37.000000 txrm2tiff-2.0.6/src/txrm2tiff/txrm/txrm_property.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     3158 2023-05-30 10:24:41.000000 txrm2tiff-2.0.6/src/txrm2tiff/txrm/v3.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     2928 2023-05-30 10:24:41.000000 txrm2tiff-2.0.6/src/txrm2tiff/txrm/v5.py
+drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-17 14:01:01.000000 txrm2tiff-2.0.6/src/txrm2tiff/txrm_functions/
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       45 2021-11-26 16:04:02.000000 txrm2tiff-2.0.6/src/txrm2tiff/txrm_functions/__init__.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     4667 2023-05-30 10:44:58.000000 txrm2tiff-2.0.6/src/txrm2tiff/txrm_functions/general.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     2649 2021-12-01 16:08:13.000000 txrm2tiff-2.0.6/src/txrm2tiff/txrm_functions/images.py
+drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-17 14:01:01.000000 txrm2tiff-2.0.6/src/txrm2tiff/utils/
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)        0 2021-11-26 16:04:02.000000 txrm2tiff-2.0.6/src/txrm2tiff/utils/__init__.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     4715 2023-07-17 13:59:18.000000 txrm2tiff-2.0.6/src/txrm2tiff/utils/file_handler.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      415 2021-11-26 16:04:02.000000 txrm2tiff-2.0.6/src/txrm2tiff/utils/functions.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     6400 2023-05-30 10:44:58.000000 txrm2tiff-2.0.6/src/txrm2tiff/utils/image_processing.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      818 2021-11-26 16:04:02.000000 txrm2tiff-2.0.6/src/txrm2tiff/utils/logging.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     5618 2023-07-07 17:08:26.000000 txrm2tiff-2.0.6/src/txrm2tiff/utils/metadata.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     2570 2021-11-26 16:04:02.000000 txrm2tiff-2.0.6/src/txrm2tiff/utils/shortcut_creation.py
+drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-17 14:01:01.000000 txrm2tiff-2.0.6/src/txrm2tiff/xradia_properties/
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       50 2021-11-26 16:04:02.000000 txrm2tiff-2.0.6/src/txrm2tiff/xradia_properties/__init__.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1856 2023-05-30 10:24:41.000000 txrm2tiff-2.0.6/src/txrm2tiff/xradia_properties/enums.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     3334 2023-05-30 10:44:58.000000 txrm2tiff-2.0.6/src/txrm2tiff/xradia_properties/stream_dtypes.py
+drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-17 14:01:01.000000 txrm2tiff-2.0.6/src/txrm2tiff.egg-info/
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     7445 2023-07-17 14:01:01.000000 txrm2tiff-2.0.6/src/txrm2tiff.egg-info/PKG-INFO
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1853 2023-07-17 14:01:01.000000 txrm2tiff-2.0.6/src/txrm2tiff.egg-info/SOURCES.txt
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)        1 2023-07-17 14:01:01.000000 txrm2tiff-2.0.6/src/txrm2tiff.egg-info/dependency_links.txt
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       54 2023-07-17 14:01:01.000000 txrm2tiff-2.0.6/src/txrm2tiff.egg-info/entry_points.txt
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      170 2023-07-17 14:01:01.000000 txrm2tiff-2.0.6/src/txrm2tiff.egg-info/requires.txt
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       10 2023-07-17 14:01:01.000000 txrm2tiff-2.0.6/src/txrm2tiff.egg-info/top_level.txt
+drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-17 14:01:02.000000 txrm2tiff-2.0.6/tests/
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      193 2021-02-08 17:40:15.000000 txrm2tiff-2.0.6/tests/__init__.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)    11184 2023-05-30 10:44:58.000000 txrm2tiff-2.0.6/tests/test_abstract_txrm.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)    10711 2023-05-30 10:44:58.000000 txrm2tiff-2.0.6/tests/test_annotator.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     9650 2023-05-30 10:44:58.000000 txrm2tiff-2.0.6/tests/test_commandline_entrypoint.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     5721 2023-07-17 13:59:18.000000 txrm2tiff-2.0.6/tests/test_file_handler.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     5849 2023-05-30 10:44:58.000000 txrm2tiff-2.0.6/tests/test_image_processing.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     2777 2021-12-01 16:29:22.000000 txrm2tiff-2.0.6/tests/test_inspector.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)    14713 2023-05-30 10:44:58.000000 txrm2tiff-2.0.6/tests/test_main.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     4036 2023-05-30 10:24:41.000000 txrm2tiff-2.0.6/tests/test_metadata.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     3858 2023-07-07 17:26:47.000000 txrm2tiff-2.0.6/tests/test_referencer.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     9936 2023-05-30 16:23:06.000000 txrm2tiff-2.0.6/tests/test_saver.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1455 2021-12-01 16:07:16.000000 txrm2tiff-2.0.6/tests/test_setup_fuctions.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     2246 2021-12-01 16:29:22.000000 txrm2tiff-2.0.6/tests/test_shifts.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     5057 2021-12-01 16:07:23.000000 txrm2tiff-2.0.6/tests/test_txrm_functions.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     2682 2023-05-30 10:44:58.000000 txrm2tiff-2.0.6/tests/test_txrm_property.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     3709 2023-05-30 15:25:01.000000 txrm2tiff-2.0.6/tests/test_txrm_v5.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     6007 2023-05-30 15:10:23.000000 txrm2tiff-2.0.6/tests/test_txrmv3.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      834 2021-12-01 16:07:35.000000 txrm2tiff-2.0.6/tests/test_util_functions.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     7056 2021-12-14 13:07:27.000000 txrm2tiff-2.0.6/tests/test_with_files.py
```

### Comparing `txrm2tiff-2.0.5/.gitignore` & `txrm2tiff-2.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.5/.vscode/launch.json` & `txrm2tiff-2.0.6/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.5/.vscode/settings.json` & `txrm2tiff-2.0.6/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.5/LICENSE` & `txrm2tiff-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.5/PKG-INFO` & `txrm2tiff-2.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: txrm2tiff
-Version: 2.0.5
+Version: 2.0.6
 Summary: A converter for Zeiss txrm and xrm files, created by & for B24 of Diamond Light Source
 Author-email: Thomas Fish <thomas.fish@diamond.ac.uk>
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `txrm2tiff-2.0.5/README.md` & `txrm2tiff-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.5/conda/meta.yaml` & `txrm2tiff-2.0.6/conda/meta.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 {% set name = "txrm2tiff" %}
-{% set version = "2.0.5" %}
+{% set version = "2.0.6" %}
 
 package:
   name: {{ name|lower }}
   version: {{ version }}
 
 source:
   path: ../
```

### Comparing `txrm2tiff-2.0.5/pyproject.toml` & `txrm2tiff-2.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.5/src/txrm2tiff/__main__.py` & `txrm2tiff-2.0.6/src/txrm2tiff/__main__.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.5/src/txrm2tiff/font/CallingCode-Regular.otf` & `txrm2tiff-2.0.6/src/txrm2tiff/font/CallingCode-Regular.otf`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.5/src/txrm2tiff/font/License.txt` & `txrm2tiff-2.0.6/src/txrm2tiff/font/License.txt`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.5/src/txrm2tiff/inspector.py` & `txrm2tiff-2.0.6/src/txrm2tiff/inspector.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.5/src/txrm2tiff/main.py` & `txrm2tiff-2.0.6/src/txrm2tiff/main.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.5/src/txrm2tiff/txrm/abstract.py` & `txrm2tiff-2.0.6/src/txrm2tiff/txrm/abstract.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.5/src/txrm2tiff/txrm/annot_mixin.py` & `txrm2tiff-2.0.6/src/txrm2tiff/txrm/annot_mixin.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.5/src/txrm2tiff/txrm/main.py` & `txrm2tiff-2.0.6/src/txrm2tiff/txrm/main.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.5/src/txrm2tiff/txrm/ref_mixin.py` & `txrm2tiff-2.0.6/src/txrm2tiff/txrm/ref_mixin.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.5/src/txrm2tiff/txrm/save_mixin.py` & `txrm2tiff-2.0.6/src/txrm2tiff/txrm/save_mixin.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.5/src/txrm2tiff/txrm/shifts_mixin.py` & `txrm2tiff-2.0.6/src/txrm2tiff/txrm/shifts_mixin.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.5/src/txrm2tiff/txrm/txrm_property.py` & `txrm2tiff-2.0.6/src/txrm2tiff/txrm/txrm_property.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.5/src/txrm2tiff/txrm/v3.py` & `txrm2tiff-2.0.6/src/txrm2tiff/txrm/v3.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.5/src/txrm2tiff/txrm/v5.py` & `txrm2tiff-2.0.6/src/txrm2tiff/txrm/v5.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.5/src/txrm2tiff/txrm_functions/general.py` & `txrm2tiff-2.0.6/src/txrm2tiff/txrm_functions/general.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.5/src/txrm2tiff/txrm_functions/images.py` & `txrm2tiff-2.0.6/src/txrm2tiff/txrm_functions/images.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.5/src/txrm2tiff/utils/file_handler.py` & `txrm2tiff-2.0.6/src/txrm2tiff/utils/file_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,16 +69,16 @@
     if metadata is not None:
         meta_img = metadata.image()
         pixels = meta_img.Pixels
         pixels.set_PixelType(dtype_dict[image.dtype.name])
         meta_img.set_Name(filepath.name)
         resolution = [pixels.get_PhysicalSizeX(), pixels.get_PhysicalSizeY()]
         if None not in resolution:  # Check that both have values
-            resolution = [pixel_size * 1000 for pixel_size in resolution]
-            resolution_unit = "MICROMETER"  # NANOMETER isn't included in tifffile
+            resolution = [1.e7 / (pixel_size)  for pixel_size in resolution]  # Pixels per resolution unit (converted from nm to cm)
+            resolution_unit = tf.TIFF.RESUNIT.CENTIMETER  # Must use CENTIMETER for maximum compatibility
             if tf.__version__ >= "2022.7.28":
                 # 2022.7.28: Deprecate third resolution argument on write (use resolutionunit)
                 tiff_kwargs["resolutionunit"] = resolution_unit
             else:
                 resolution.append(resolution_unit)
             tiff_kwargs["resolution"] = tuple(resolution)
         metadata = metadata.to_xml().encode()
@@ -89,15 +89,15 @@
     )  # Check if data bigger than 4GB TIFF limit
 
     logging.info("Saving image as %s with %i frames", filepath.name, num_frames)
 
     if filepath.exists():
         logging.warning("Overwriting existing file %s", filepath)
 
-    with tf.TiffWriter(str(filepath), bigtiff=bigtiff, ome=False) as tif:
+    with tf.TiffWriter(str(filepath), bigtiff=bigtiff, ome=False, imagej=False) as tif:
         tif.write(
             image,
             photometric="MINISBLACK",
             description=metadata,
             metadata={"axes": "ZYX"},
             software=f"txrm2tiff {__version__}",
             **tiff_kwargs
```

### Comparing `txrm2tiff-2.0.5/src/txrm2tiff/utils/image_processing.py` & `txrm2tiff-2.0.6/src/txrm2tiff/utils/image_processing.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.5/src/txrm2tiff/utils/logging.py` & `txrm2tiff-2.0.6/src/txrm2tiff/utils/logging.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.5/src/txrm2tiff/utils/metadata.py` & `txrm2tiff-2.0.6/src/txrm2tiff/utils/metadata.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.5/src/txrm2tiff/utils/shortcut_creation.py` & `txrm2tiff-2.0.6/src/txrm2tiff/utils/shortcut_creation.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.5/src/txrm2tiff/xradia_properties/enums.py` & `txrm2tiff-2.0.6/src/txrm2tiff/xradia_properties/enums.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.5/src/txrm2tiff/xradia_properties/stream_dtypes.py` & `txrm2tiff-2.0.6/src/txrm2tiff/xradia_properties/stream_dtypes.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.5/src/txrm2tiff.egg-info/PKG-INFO` & `txrm2tiff-2.0.6/src/txrm2tiff.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: txrm2tiff
-Version: 2.0.5
+Version: 2.0.6
 Summary: A converter for Zeiss txrm and xrm files, created by & for B24 of Diamond Light Source
 Author-email: Thomas Fish <thomas.fish@diamond.ac.uk>
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `txrm2tiff-2.0.5/src/txrm2tiff.egg-info/SOURCES.txt` & `txrm2tiff-2.0.6/src/txrm2tiff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.5/tests/test_abstract_txrm.py` & `txrm2tiff-2.0.6/tests/test_abstract_txrm.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.5/tests/test_annotator.py` & `txrm2tiff-2.0.6/tests/test_annotator.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.5/tests/test_commandline_entrypoint.py` & `txrm2tiff-2.0.6/tests/test_commandline_entrypoint.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.5/tests/test_file_handler.py` & `txrm2tiff-2.0.6/tests/test_file_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -111,32 +111,32 @@
 
     def test_manual_save_sets_pixel_size(self):
         with TemporaryDirectory(
             prefix="saving_test_", dir=Path(__name__).parent
         ) as tmpdir:
             im_path = Path(tmpdir) / "saved.tiff"
             metadata = OMEXML()
-            pixel_size_xy = (5, 6)  #nm
+            pixel_size_xy = (1, 2)  # nm
             pixels = metadata.image().Pixels
             pixels.set_PhysicalSizeX(pixel_size_xy[0])
             pixels.set_PhysicalSizeY(pixel_size_xy[1])
             image = np.ones((5, 30, 35), dtype=np.float64)
             self.assertFalse(im_path.exists())
             manual_save(im_path, image, data_type=np.uint16, metadata=metadata)
             self.assertTrue(im_path.exists())
             with tf.TiffFile(im_path) as tiff:
                 saved_arr = tiff.asarray()
-                tif_tags = {}
-                for tag in tiff.pages[0].tags.values():
-                    name, value = tag.name, tag.value
-                    tif_tags[name] = value
+                x_resolution = tiff.pages[0].tags['XResolution'].value
+                y_resolution = tiff.pages[0].tags['YResolution'].value
+                resolution_unit = tiff.pages[0].tags['ResolutionUnit'].value
 
         assert_array_equal(saved_arr, image)
-        self.assertEqual(tif_tags["XResolution"][0], pixel_size_xy[0] * 1000)
-        self.assertEqual(tif_tags["YResolution"][0], pixel_size_xy[1] * 1000)
+        self.assertEqual(x_resolution, (int(1.e7), 1))
+        self.assertEqual(y_resolution, (int(5.e6), 1))
+        self.assertEqual(resolution_unit, int(tf.TIFF.RESUNIT.CENTIMETER))
 
 
     def test_manual_annotation_save(self):
         with TemporaryDirectory(
             prefix="annotation_saving_test_", dir=Path(__name__).parent
         ) as tmpdir:
             im_path = Path(tmpdir) / "saved.tiff"
```

### Comparing `txrm2tiff-2.0.5/tests/test_image_processing.py` & `txrm2tiff-2.0.6/tests/test_image_processing.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.5/tests/test_inspector.py` & `txrm2tiff-2.0.6/tests/test_inspector.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.5/tests/test_main.py` & `txrm2tiff-2.0.6/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.5/tests/test_metadata.py` & `txrm2tiff-2.0.6/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.5/tests/test_referencer.py` & `txrm2tiff-2.0.6/tests/test_referencer.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.5/tests/test_saver.py` & `txrm2tiff-2.0.6/tests/test_saver.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.5/tests/test_setup_fuctions.py` & `txrm2tiff-2.0.6/tests/test_setup_fuctions.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.5/tests/test_shifts.py` & `txrm2tiff-2.0.6/tests/test_shifts.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.5/tests/test_txrm_functions.py` & `txrm2tiff-2.0.6/tests/test_txrm_functions.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.5/tests/test_txrm_property.py` & `txrm2tiff-2.0.6/tests/test_txrm_property.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.5/tests/test_txrm_v5.py` & `txrm2tiff-2.0.6/tests/test_txrm_v5.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.5/tests/test_txrmv3.py` & `txrm2tiff-2.0.6/tests/test_txrmv3.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.5/tests/test_util_functions.py` & `txrm2tiff-2.0.6/tests/test_util_functions.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.5/tests/test_with_files.py` & `txrm2tiff-2.0.6/tests/test_with_files.py`

 * *Files identical despite different names*

