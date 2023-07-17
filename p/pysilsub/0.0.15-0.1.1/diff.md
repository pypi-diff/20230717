# Comparing `tmp/pysilsub-0.0.15.tar.gz` & `tmp/pysilsub-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysilsub-0.0.15.tar", last modified: Fri Mar 24 14:45:01 2023, max compression
+gzip compressed data, was "pysilsub-0.1.1.tar", last modified: Mon Jul 17 13:48:54 2023, max compression
```

## Comparing `pysilsub-0.0.15.tar` & `pysilsub-0.1.1.tar`

### file list

```diff
@@ -1,61 +1,60 @@
-drwxr-xr-x   0 jtm545     (502) staff       (20)        0 2023-03-24 14:45:01.814877 pysilsub-0.0.15/
--rw-r--r--   0 jtm545     (502) staff       (20)     1077 2021-09-20 16:47:32.000000 pysilsub-0.0.15/LICENSE
--rw-r--r--   0 jtm545     (502) staff       (20)       44 2022-07-10 22:02:47.000000 pysilsub-0.0.15/MANIFEST.in
--rw-r--r--   0 jtm545     (502) staff       (20)     4434 2023-03-24 14:45:01.814633 pysilsub-0.0.15/PKG-INFO
--rw-r--r--   0 jtm545     (502) staff       (20)     3655 2023-03-24 14:32:19.000000 pysilsub-0.0.15/README.md
--rw-r--r--   0 jtm545     (502) staff       (20)      117 2022-07-10 19:46:42.000000 pysilsub-0.0.15/pyproject.toml
-drwxr-xr-x   0 jtm545     (502) staff       (20)        0 2023-03-24 14:45:01.728518 pysilsub-0.0.15/pysilsub/
--rw-r--r--   0 jtm545     (502) staff       (20)     6148 2023-03-07 10:22:03.000000 pysilsub-0.0.15/pysilsub/.DS_Store
--rwxr-xr-x   0 jtm545     (502) staff       (20)     9449 2023-02-09 00:58:41.000000 pysilsub-0.0.15/pysilsub/CIE.py
--rw-r--r--   0 jtm545     (502) staff       (20)      557 2023-03-24 11:33:14.000000 pysilsub-0.0.15/pysilsub/__init__.py
--rw-r--r--   0 jtm545     (502) staff       (20)     4984 2022-09-22 22:21:15.000000 pysilsub-0.0.15/pysilsub/colorfuncs.py
--rw-r--r--   0 jtm545     (502) staff       (20)      669 2022-09-03 15:40:04.000000 pysilsub-0.0.15/pysilsub/config.py
-drwxr-xr-x   0 jtm545     (502) staff       (20)        0 2023-03-24 14:45:01.813071 pysilsub-0.0.15/pysilsub/data/
--rw-r--r--   0 jtm545     (502) staff       (20)     6148 2022-12-22 13:44:21.000000 pysilsub-0.0.15/pysilsub/data/.DS_Store
-drwxr-xr-x   0 jtm545     (502) staff       (20)        0 2023-03-24 14:45:01.814250 pysilsub-0.0.15/pysilsub/data/.ipynb_checkpoints/
--rw-r--r--   0 jtm545     (502) staff       (20)     8121 2023-02-05 07:15:22.000000 pysilsub-0.0.15/pysilsub/data/.ipynb_checkpoints/OneLight-checkpoint.json
--rw-r--r--   0 jtm545     (502) staff       (20)      643 2023-02-04 16:16:42.000000 pysilsub-0.0.15/pysilsub/data/.ipynb_checkpoints/ProPixx-checkpoint.json
--rw-r--r--   0 jtm545     (502) staff       (20)     1341 2022-12-22 13:47:16.000000 pysilsub-0.0.15/pysilsub/data/.ipynb_checkpoints/STLAB_1_York-checkpoint.json
--rw-r--r--   0 jtm545     (502) staff       (20)   972930 2022-02-05 19:47:42.000000 pysilsub-0.0.15/pysilsub/data/BCGAR.csv
--rw-r--r--   0 jtm545     (502) staff       (20)      580 2022-12-22 13:34:12.000000 pysilsub-0.0.15/pysilsub/data/BCGAR.json
--rw-r--r--   0 jtm545     (502) staff       (20)     4211 2023-01-05 12:50:57.000000 pysilsub-0.0.15/pysilsub/data/Biermann2011_eyelid_transmiattance.csv
--rw-r--r--   0 jtm545     (502) staff       (20)     9666 2022-09-04 15:14:13.000000 pysilsub-0.0.15/pysilsub/data/CIE170_2_chromaticity_coordinates.csv
--rw-r--r--   0 jtm545     (502) staff       (20)      694 2022-09-04 17:28:12.000000 pysilsub-0.0.15/pysilsub/data/CIEPO06_macula_density.csv
--rw-r--r--   0 jtm545     (502) staff       (20)     1636 2022-09-12 19:37:03.000000 pysilsub-0.0.15/pysilsub/data/CIEPO06_optical_density.csv
--rw-r--r--   0 jtm545     (502) staff       (20)    17844 2022-09-29 08:18:08.000000 pysilsub-0.0.15/pysilsub/data/CIES026.csv
--rw-r--r--   0 jtm545     (502) staff       (20)     5695 2022-09-04 15:11:09.000000 pysilsub-0.0.15/pysilsub/data/CIE_1924_photopic_vl.csv
--rw-r--r--   0 jtm545     (502) staff       (20)    13055 2022-09-04 15:09:06.000000 pysilsub-0.0.15/pysilsub/data/CIE_1931_2_deg_CMF.csv
--rw-r--r--   0 jtm545     (502) staff       (20)     9207 2022-09-04 15:07:34.000000 pysilsub-0.0.15/pysilsub/data/CIE_2006_10_deg_CMF.csv
--rw-r--r--   0 jtm545     (502) staff       (20)     2170 2022-09-04 17:37:27.000000 pysilsub-0.0.15/pysilsub/data/CIE_A_lms.csv
--rw-r--r--   0 jtm545     (502) staff       (20)    94466 2022-12-22 12:54:00.000000 pysilsub-0.0.15/pysilsub/data/LEDCube.csv
--rw-r--r--   0 jtm545     (502) staff       (20)     2261 2022-12-22 13:27:45.000000 pysilsub-0.0.15/pysilsub/data/LEDCube.json
--rw-r--r--   0 jtm545     (502) staff       (20) 10877349 2023-02-05 06:31:36.000000 pysilsub-0.0.15/pysilsub/data/OneLight.csv
--rw-r--r--   0 jtm545     (502) staff       (20)     8121 2023-02-05 07:15:22.000000 pysilsub-0.0.15/pysilsub/data/OneLight.json
--rw-r--r--   0 jtm545     (502) staff       (20)    21321 2023-01-05 12:51:58.000000 pysilsub-0.0.15/pysilsub/data/Prahl2012_bilurubin_absorption_spectrum.csv
--rw-r--r--   0 jtm545     (502) staff       (20)     6872 2023-01-04 12:30:01.000000 pysilsub-0.0.15/pysilsub/data/Prahl_Hgb.csv
--rw-r--r--   0 jtm545     (502) staff       (20)   369285 2023-02-04 16:40:16.000000 pysilsub-0.0.15/pysilsub/data/ProPixx.csv
--rw-r--r--   0 jtm545     (502) staff       (20)      575 2023-03-24 12:41:06.000000 pysilsub-0.0.15/pysilsub/data/ProPixx.json
--rw-r--r--   0 jtm545     (502) staff       (20)  4321088 2022-10-31 14:25:01.000000 pysilsub-0.0.15/pysilsub/data/STLAB_1_York.csv
--rw-r--r--   0 jtm545     (502) staff       (20)     1341 2022-12-22 13:47:16.000000 pysilsub-0.0.15/pysilsub/data/STLAB_1_York.json
--rw-r--r--   0 jtm545     (502) staff       (20)  4319151 2022-10-31 14:24:10.000000 pysilsub-0.0.15/pysilsub/data/STLAB_2_York.csv
--rw-r--r--   0 jtm545     (502) staff       (20)     1348 2022-12-22 14:14:46.000000 pysilsub-0.0.15/pysilsub/data/STLAB_2_York.json
--rwxrwxrwx   0 jtm545     (502) staff       (20)  2952100 2022-06-27 14:17:01.000000 pysilsub-0.0.15/pysilsub/data/STLAB_Oxford.csv
--rw-r--r--   0 jtm545     (502) staff       (20)     1125 2022-12-22 13:41:24.000000 pysilsub-0.0.15/pysilsub/data/STLAB_Oxford.json
--rw-r--r--   0 jtm545     (502) staff       (20)   264985 2022-07-04 11:46:56.000000 pysilsub-0.0.15/pysilsub/data/VirtualSky.csv
--rw-r--r--   0 jtm545     (502) staff       (20)      752 2023-01-03 20:03:44.000000 pysilsub-0.0.15/pysilsub/data/VirtualSky.json
--rw-r--r--   0 jtm545     (502) staff       (20)     7495 2022-09-17 11:57:08.000000 pysilsub-0.0.15/pysilsub/data/linCIE2008v10e_1.csv
--rw-r--r--   0 jtm545     (502) staff       (20)    19109 2023-01-03 15:43:09.000000 pysilsub-0.0.15/pysilsub/data/rodent_action_spectra.csv
--rw-r--r--   0 jtm545     (502) staff       (20)      236 2023-01-04 12:35:35.000000 pysilsub-0.0.15/pysilsub/data/vanKampen_Hgb.csv
--rwxr-xr-x   0 jtm545     (502) staff       (20)    37798 2023-03-24 12:40:45.000000 pysilsub-0.0.15/pysilsub/devices.py
--rw-r--r--   0 jtm545     (502) staff       (20)    11441 2023-03-24 12:17:27.000000 pysilsub-0.0.15/pysilsub/observers.py
--rw-r--r--   0 jtm545     (502) staff       (20)    42095 2023-03-24 14:17:29.000000 pysilsub-0.0.15/pysilsub/preceps.py
--rw-r--r--   0 jtm545     (502) staff       (20)    42426 2023-03-08 23:25:11.000000 pysilsub-0.0.15/pysilsub/problems.py
--rw-r--r--   0 jtm545     (502) staff       (20)     1569 2023-03-24 14:17:38.000000 pysilsub-0.0.15/pysilsub/waves.py
-drwxr-xr-x   0 jtm545     (502) staff       (20)        0 2023-03-24 14:45:01.729376 pysilsub-0.0.15/pysilsub.egg-info/
--rw-r--r--   0 jtm545     (502) staff       (20)     4434 2023-03-24 14:45:01.000000 pysilsub-0.0.15/pysilsub.egg-info/PKG-INFO
--rw-r--r--   0 jtm545     (502) staff       (20)     1619 2023-03-24 14:45:01.000000 pysilsub-0.0.15/pysilsub.egg-info/SOURCES.txt
--rw-r--r--   0 jtm545     (502) staff       (20)        1 2023-03-24 14:45:01.000000 pysilsub-0.0.15/pysilsub.egg-info/dependency_links.txt
--rw-r--r--   0 jtm545     (502) staff       (20)       65 2023-03-24 14:45:01.000000 pysilsub-0.0.15/pysilsub.egg-info/requires.txt
--rw-r--r--   0 jtm545     (502) staff       (20)        9 2023-03-24 14:45:01.000000 pysilsub-0.0.15/pysilsub.egg-info/top_level.txt
--rw-r--r--   0 jtm545     (502) staff       (20)       38 2023-03-24 14:45:01.814936 pysilsub-0.0.15/setup.cfg
--rw-r--r--   0 jtm545     (502) staff       (20)     1318 2023-03-24 14:44:22.000000 pysilsub-0.0.15/setup.py
+drwxr-xr-x   0 jtm545     (502) staff       (20)        0 2023-07-17 13:48:54.090700 pysilsub-0.1.1/
+-rw-r--r--   0 jtm545     (502) staff       (20)     1077 2021-09-20 16:47:32.000000 pysilsub-0.1.1/LICENSE
+-rw-r--r--   0 jtm545     (502) staff       (20)       44 2022-07-10 22:02:47.000000 pysilsub-0.1.1/MANIFEST.in
+-rw-r--r--   0 jtm545     (502) staff       (20)     4446 2023-07-17 13:48:54.090514 pysilsub-0.1.1/PKG-INFO
+-rw-r--r--   0 jtm545     (502) staff       (20)     3675 2023-07-17 13:03:04.000000 pysilsub-0.1.1/README.md
+-rw-r--r--   0 jtm545     (502) staff       (20)      117 2022-07-10 19:46:42.000000 pysilsub-0.1.1/pyproject.toml
+drwxr-xr-x   0 jtm545     (502) staff       (20)        0 2023-07-17 13:48:54.037741 pysilsub-0.1.1/pysilsub/
+-rw-r--r--   0 jtm545     (502) staff       (20)     6148 2023-05-23 17:44:32.000000 pysilsub-0.1.1/pysilsub/.DS_Store
+-rwxr-xr-x   0 jtm545     (502) staff       (20)     9449 2023-02-09 00:58:41.000000 pysilsub-0.1.1/pysilsub/CIE.py
+-rw-r--r--   0 jtm545     (502) staff       (20)      556 2023-03-28 05:02:27.000000 pysilsub-0.1.1/pysilsub/__init__.py
+-rw-r--r--   0 jtm545     (502) staff       (20)     4239 2023-05-15 10:07:46.000000 pysilsub-0.1.1/pysilsub/binocular.py
+-rw-r--r--   0 jtm545     (502) staff       (20)     4985 2023-04-20 09:27:22.000000 pysilsub-0.1.1/pysilsub/colorfuncs.py
+-rw-r--r--   0 jtm545     (502) staff       (20)      669 2022-09-03 15:40:04.000000 pysilsub-0.1.1/pysilsub/config.py
+drwxr-xr-x   0 jtm545     (502) staff       (20)        0 2023-07-17 13:48:54.089316 pysilsub-0.1.1/pysilsub/data/
+-rw-r--r--   0 jtm545     (502) staff       (20)     6148 2023-03-28 04:55:07.000000 pysilsub-0.1.1/pysilsub/data/.DS_Store
+drwxr-xr-x   0 jtm545     (502) staff       (20)        0 2023-07-17 13:48:54.090184 pysilsub-0.1.1/pysilsub/data/.ipynb_checkpoints/
+-rw-r--r--   0 jtm545     (502) staff       (20)     8121 2023-02-05 07:15:22.000000 pysilsub-0.1.1/pysilsub/data/.ipynb_checkpoints/OneLight-checkpoint.json
+-rw-r--r--   0 jtm545     (502) staff       (20)      643 2023-02-04 16:16:42.000000 pysilsub-0.1.1/pysilsub/data/.ipynb_checkpoints/ProPixx-checkpoint.json
+-rw-r--r--   0 jtm545     (502) staff       (20)     1341 2022-12-22 13:47:16.000000 pysilsub-0.1.1/pysilsub/data/.ipynb_checkpoints/STLAB_1_York-checkpoint.json
+-rw-r--r--   0 jtm545     (502) staff       (20)   972930 2022-02-05 19:47:42.000000 pysilsub-0.1.1/pysilsub/data/BCGAR.csv
+-rw-r--r--   0 jtm545     (502) staff       (20)      580 2022-12-22 13:34:12.000000 pysilsub-0.1.1/pysilsub/data/BCGAR.json
+-rw-r--r--   0 jtm545     (502) staff       (20)     4211 2023-01-05 12:50:57.000000 pysilsub-0.1.1/pysilsub/data/Biermann2011_eyelid_transmiattance.csv
+-rw-r--r--   0 jtm545     (502) staff       (20)     9666 2022-09-04 15:14:13.000000 pysilsub-0.1.1/pysilsub/data/CIE170_2_chromaticity_coordinates.csv
+-rw-r--r--   0 jtm545     (502) staff       (20)      694 2022-09-04 17:28:12.000000 pysilsub-0.1.1/pysilsub/data/CIEPO06_macula_density.csv
+-rw-r--r--   0 jtm545     (502) staff       (20)     1636 2022-09-12 19:37:03.000000 pysilsub-0.1.1/pysilsub/data/CIEPO06_optical_density.csv
+-rw-r--r--   0 jtm545     (502) staff       (20)    17844 2022-09-29 08:18:08.000000 pysilsub-0.1.1/pysilsub/data/CIES026.csv
+-rw-r--r--   0 jtm545     (502) staff       (20)     5695 2022-09-04 15:11:09.000000 pysilsub-0.1.1/pysilsub/data/CIE_1924_photopic_vl.csv
+-rw-r--r--   0 jtm545     (502) staff       (20)    13055 2022-09-04 15:09:06.000000 pysilsub-0.1.1/pysilsub/data/CIE_1931_2_deg_CMF.csv
+-rw-r--r--   0 jtm545     (502) staff       (20)     9207 2022-09-04 15:07:34.000000 pysilsub-0.1.1/pysilsub/data/CIE_2006_10_deg_CMF.csv
+-rw-r--r--   0 jtm545     (502) staff       (20)     2170 2022-09-04 17:37:27.000000 pysilsub-0.1.1/pysilsub/data/CIE_A_lms.csv
+-rw-r--r--   0 jtm545     (502) staff       (20)   488814 2023-03-25 19:44:06.000000 pysilsub-0.1.1/pysilsub/data/CRT.csv
+-rw-r--r--   0 jtm545     (502) staff       (20)      477 2023-03-25 19:51:31.000000 pysilsub-0.1.1/pysilsub/data/CRT.json
+-rw-r--r--   0 jtm545     (502) staff       (20) 10877349 2023-02-05 06:31:36.000000 pysilsub-0.1.1/pysilsub/data/OneLight.csv
+-rw-r--r--   0 jtm545     (502) staff       (20)     8121 2023-02-05 07:15:22.000000 pysilsub-0.1.1/pysilsub/data/OneLight.json
+-rw-r--r--   0 jtm545     (502) staff       (20)    21321 2023-01-05 12:51:58.000000 pysilsub-0.1.1/pysilsub/data/Prahl2012_bilurubin_absorption_spectrum.csv
+-rw-r--r--   0 jtm545     (502) staff       (20)     6872 2023-01-04 12:30:01.000000 pysilsub-0.1.1/pysilsub/data/Prahl_Hgb.csv
+-rw-r--r--   0 jtm545     (502) staff       (20)   369285 2023-02-04 16:40:16.000000 pysilsub-0.1.1/pysilsub/data/ProPixx.csv
+-rw-r--r--   0 jtm545     (502) staff       (20)      575 2023-03-31 19:13:06.000000 pysilsub-0.1.1/pysilsub/data/ProPixx.json
+-rw-r--r--   0 jtm545     (502) staff       (20)  4321088 2022-10-31 14:25:01.000000 pysilsub-0.1.1/pysilsub/data/STLAB_1_York.csv
+-rw-r--r--   0 jtm545     (502) staff       (20)     1341 2022-12-22 13:47:16.000000 pysilsub-0.1.1/pysilsub/data/STLAB_1_York.json
+-rw-r--r--   0 jtm545     (502) staff       (20)  4319151 2022-10-31 14:24:10.000000 pysilsub-0.1.1/pysilsub/data/STLAB_2_York.csv
+-rw-r--r--   0 jtm545     (502) staff       (20)     1348 2022-12-22 14:14:46.000000 pysilsub-0.1.1/pysilsub/data/STLAB_2_York.json
+-rw-r--r--   0 jtm545     (502) staff       (20)   264985 2022-07-04 11:46:56.000000 pysilsub-0.1.1/pysilsub/data/VirtualSky.csv
+-rw-r--r--   0 jtm545     (502) staff       (20)      752 2023-01-03 20:03:44.000000 pysilsub-0.1.1/pysilsub/data/VirtualSky.json
+-rw-r--r--   0 jtm545     (502) staff       (20)     7495 2022-09-17 11:57:08.000000 pysilsub-0.1.1/pysilsub/data/linCIE2008v10e_1.csv
+-rw-r--r--   0 jtm545     (502) staff       (20)    19109 2023-01-03 15:43:09.000000 pysilsub-0.1.1/pysilsub/data/rodent_action_spectra.csv
+-rw-r--r--   0 jtm545     (502) staff       (20)      236 2023-01-04 12:35:35.000000 pysilsub-0.1.1/pysilsub/data/vanKampen_Hgb.csv
+-rwxr-xr-x   0 jtm545     (502) staff       (20)    38223 2023-05-31 08:49:59.000000 pysilsub-0.1.1/pysilsub/devices.py
+-rw-r--r--   0 jtm545     (502) staff       (20)    11366 2023-03-31 19:25:14.000000 pysilsub-0.1.1/pysilsub/observers.py
+-rw-r--r--   0 jtm545     (502) staff       (20)    42131 2023-03-24 15:54:50.000000 pysilsub-0.1.1/pysilsub/preceps.py
+-rw-r--r--   0 jtm545     (502) staff       (20)    42848 2023-06-01 12:50:13.000000 pysilsub-0.1.1/pysilsub/problems.py
+-rw-r--r--   0 jtm545     (502) staff       (20)     1606 2023-03-24 17:47:39.000000 pysilsub-0.1.1/pysilsub/waves.py
+drwxr-xr-x   0 jtm545     (502) staff       (20)        0 2023-07-17 13:48:54.038514 pysilsub-0.1.1/pysilsub.egg-info/
+-rw-r--r--   0 jtm545     (502) staff       (20)     4446 2023-07-17 13:48:53.000000 pysilsub-0.1.1/pysilsub.egg-info/PKG-INFO
+-rw-r--r--   0 jtm545     (502) staff       (20)     1570 2023-07-17 13:48:53.000000 pysilsub-0.1.1/pysilsub.egg-info/SOURCES.txt
+-rw-r--r--   0 jtm545     (502) staff       (20)        1 2023-07-17 13:48:53.000000 pysilsub-0.1.1/pysilsub.egg-info/dependency_links.txt
+-rw-r--r--   0 jtm545     (502) staff       (20)       50 2023-07-17 13:48:53.000000 pysilsub-0.1.1/pysilsub.egg-info/requires.txt
+-rw-r--r--   0 jtm545     (502) staff       (20)        9 2023-07-17 13:48:53.000000 pysilsub-0.1.1/pysilsub.egg-info/top_level.txt
+-rw-r--r--   0 jtm545     (502) staff       (20)       38 2023-07-17 13:48:54.090749 pysilsub-0.1.1/setup.cfg
+-rw-r--r--   0 jtm545     (502) staff       (20)     1311 2023-07-17 13:37:37.000000 pysilsub-0.1.1/setup.py
```

### Comparing `pysilsub-0.0.15/LICENSE` & `pysilsub-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pysilsub-0.0.15/PKG-INFO` & `pysilsub-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 Metadata-Version: 2.1
 Name: pysilsub
-Version: 0.0.15
+Version: 0.1.1
 Summary: Software for performing silent substitution in Python.
 Home-page: https://github.com/PySilentSubstitution/pysilsub
 Author: Joel T. Martin
 Author-email: joel.t.martin36@gmail.com
 License: MIT
 Project-URL: Documentation, https://pysilentsubstitution.github.io/pysilsub/index.html
 Keywords: silent substitution,vision,psychology,perception,metamer,spectra,LED
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3.7
-Requires-Python: >=3.8, <3.11
+Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Welcome to PySilentSubstitution!
 ================================
 
-
-
 [![DOI](https://zenodo.org/badge/390693759.svg)](https://zenodo.org/badge/latestdoi/390693759) [![PyPI version](https://badge.fury.io/py/pysilsub.svg)](https://badge.fury.io/py/pysilsub) [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.0-4baaaa.svg)](./CODE_OF_CONDUCT.md)  [![PyPi license](https://badgen.net/pypi/license/pip/)](https://pypi.com/project/pip/) [![PyPI status](https://img.shields.io/pypi/status/ansicolortags.svg)](https://pypi.python.org/pypi/ansicolortags/) 
 
 <img src="https://github.com/PySilentSubstitution/pysilsub/blob/main/logo/photoreceptor_characters.png?raw=True" alt="photoreceptor-characters" width="200"/>
 
-*PySilSub* is a Python toolbox for performing the method of [silent substitution](https://pysilentsubstitution.github.io/pysilsub/01_background.html) in vision and circadian research.
+*PySilSub* is a Python toolbox for performing the method of [silent substitution](https://pysilentsubstitution.github.io/pysilsub/01_background.html) in vision and nonvisual photoreception research.
 
 **Note:** See also, [PyPlr](https://pyplr.github.io/cvd_pupillometry/index.html),
 a sister project offering a Python framework for researching the pupillary 
 light reflex with the Pupil Core eye tracking platform.
 
 With *PySilSub*, observer- and device-specific solutions to silent substitution 
 problems are found with linear algebra or numerical optimisation via a configurable, 
@@ -67,16 +65,16 @@
 # algebra.
 
 from pysilsub import problems
 
 ssp = problems.SilentSubstitutionProblem.from_package_data('STLAB_1_York')  # Load example data
 ssp.background = [.5] * ssp.nprimaries  # Specify background spectrum
 ssp.ignore = ['rh']  # Ignore rod photoreceptors
-ssp.silence = ['sc', 'mc', 'lc']  # Minimise cone contrast
-ssp.target = ['mel']  # Target melanopsin
+ssp.silence = ['mc', 'lc', 'mel']  # Silence L/M cones and melanopsin
+ssp.target = ['sc']  # Target S cones
 ssp.target_contrast = .45  # With 45% contrast 
 solution = ssp.linalg_solve()  # Solve with linear algebra
 fig = ssp.plot_solution(solution)  # Plot the solution
 ```
 
 <img src="https://raw.githubusercontent.com/PySilentSubstitution/pysilsub/main/img/example_2.svg" alt="Example 2" />
```

### Comparing `pysilsub-0.0.15/README.md` & `pysilsub-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Welcome to PySilentSubstitution!
 ================================
 
-
-
 [![DOI](https://zenodo.org/badge/390693759.svg)](https://zenodo.org/badge/latestdoi/390693759) [![PyPI version](https://badge.fury.io/py/pysilsub.svg)](https://badge.fury.io/py/pysilsub) [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.0-4baaaa.svg)](./CODE_OF_CONDUCT.md)  [![PyPi license](https://badgen.net/pypi/license/pip/)](https://pypi.com/project/pip/) [![PyPI status](https://img.shields.io/pypi/status/ansicolortags.svg)](https://pypi.python.org/pypi/ansicolortags/) 
 
 <img src="https://github.com/PySilentSubstitution/pysilsub/blob/main/logo/photoreceptor_characters.png?raw=True" alt="photoreceptor-characters" width="200"/>
 
-*PySilSub* is a Python toolbox for performing the method of [silent substitution](https://pysilentsubstitution.github.io/pysilsub/01_background.html) in vision and circadian research.
+*PySilSub* is a Python toolbox for performing the method of [silent substitution](https://pysilentsubstitution.github.io/pysilsub/01_background.html) in vision and nonvisual photoreception research.
 
 **Note:** See also, [PyPlr](https://pyplr.github.io/cvd_pupillometry/index.html),
 a sister project offering a Python framework for researching the pupillary 
 light reflex with the Pupil Core eye tracking platform.
 
 With *PySilSub*, observer- and device-specific solutions to silent substitution 
 problems are found with linear algebra or numerical optimisation via a configurable, 
@@ -48,16 +46,16 @@
 # algebra.
 
 from pysilsub import problems
 
 ssp = problems.SilentSubstitutionProblem.from_package_data('STLAB_1_York')  # Load example data
 ssp.background = [.5] * ssp.nprimaries  # Specify background spectrum
 ssp.ignore = ['rh']  # Ignore rod photoreceptors
-ssp.silence = ['sc', 'mc', 'lc']  # Minimise cone contrast
-ssp.target = ['mel']  # Target melanopsin
+ssp.silence = ['mc', 'lc', 'mel']  # Silence L/M cones and melanopsin
+ssp.target = ['sc']  # Target S cones
 ssp.target_contrast = .45  # With 45% contrast 
 solution = ssp.linalg_solve()  # Solve with linear algebra
 fig = ssp.plot_solution(solution)  # Plot the solution
 ```
 
 <img src="https://raw.githubusercontent.com/PySilentSubstitution/pysilsub/main/img/example_2.svg" alt="Example 2" />
```

### Comparing `pysilsub-0.0.15/pysilsub/CIE.py` & `pysilsub-0.1.1/pysilsub/CIE.py`

 * *Files identical despite different names*

### Comparing `pysilsub-0.0.15/pysilsub/__init__.py` & `pysilsub-0.1.1/pysilsub/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
      dealing with non-linearity in calibrated multiprimary light systems 
   2. Support for CIEPO06- and CIES026- compliant physiological observer models
   3. A problem interface for defining, solving, and visualsing silent 
      substitution problems
   3. Other features
 
 """
-__version__ = '0.0.14'
+__version__ = '0.1.0'
```

### Comparing `pysilsub-0.0.15/pysilsub/colorfuncs.py` & `pysilsub-0.1.1/pysilsub/colorfuncs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 ``pysilsub.colorfuncs``
-======================
+=======================
 
 Tools for navigating between colorspaces.
 
 Many have been translated from MATLAB's Psychtoolbox/PsychColormetric
 
 """
```

### Comparing `pysilsub-0.0.15/pysilsub/config.py` & `pysilsub-0.1.1/pysilsub/config.py`

 * *Files identical despite different names*

### Comparing `pysilsub-0.0.15/pysilsub/data/.ipynb_checkpoints/OneLight-checkpoint.json` & `pysilsub-0.1.1/pysilsub/data/.ipynb_checkpoints/OneLight-checkpoint.json`

 * *Files identical despite different names*

### Comparing `pysilsub-0.0.15/pysilsub/data/.ipynb_checkpoints/ProPixx-checkpoint.json` & `pysilsub-0.1.1/pysilsub/data/.ipynb_checkpoints/ProPixx-checkpoint.json`

 * *Files identical despite different names*

### Comparing `pysilsub-0.0.15/pysilsub/data/.ipynb_checkpoints/STLAB_1_York-checkpoint.json` & `pysilsub-0.1.1/pysilsub/data/.ipynb_checkpoints/STLAB_1_York-checkpoint.json`

 * *Files identical despite different names*

### Comparing `pysilsub-0.0.15/pysilsub/data/BCGAR.csv` & `pysilsub-0.1.1/pysilsub/data/BCGAR.csv`

 * *Files identical despite different names*

### Comparing `pysilsub-0.0.15/pysilsub/data/BCGAR.json` & `pysilsub-0.1.1/pysilsub/data/BCGAR.json`

 * *Files identical despite different names*

### Comparing `pysilsub-0.0.15/pysilsub/data/Biermann2011_eyelid_transmiattance.csv` & `pysilsub-0.1.1/pysilsub/data/Biermann2011_eyelid_transmiattance.csv`

 * *Files identical despite different names*

### Comparing `pysilsub-0.0.15/pysilsub/data/CIE170_2_chromaticity_coordinates.csv` & `pysilsub-0.1.1/pysilsub/data/CIE170_2_chromaticity_coordinates.csv`

 * *Files identical despite different names*

### Comparing `pysilsub-0.0.15/pysilsub/data/CIEPO06_macula_density.csv` & `pysilsub-0.1.1/pysilsub/data/CIEPO06_macula_density.csv`

 * *Files identical despite different names*

### Comparing `pysilsub-0.0.15/pysilsub/data/CIEPO06_optical_density.csv` & `pysilsub-0.1.1/pysilsub/data/CIEPO06_optical_density.csv`

 * *Files identical despite different names*

### Comparing `pysilsub-0.0.15/pysilsub/data/CIES026.csv` & `pysilsub-0.1.1/pysilsub/data/CIES026.csv`

 * *Files identical despite different names*

### Comparing `pysilsub-0.0.15/pysilsub/data/CIE_1924_photopic_vl.csv` & `pysilsub-0.1.1/pysilsub/data/CIE_1924_photopic_vl.csv`

 * *Files identical despite different names*

### Comparing `pysilsub-0.0.15/pysilsub/data/CIE_1931_2_deg_CMF.csv` & `pysilsub-0.1.1/pysilsub/data/CIE_1931_2_deg_CMF.csv`

 * *Files identical despite different names*

### Comparing `pysilsub-0.0.15/pysilsub/data/CIE_2006_10_deg_CMF.csv` & `pysilsub-0.1.1/pysilsub/data/CIE_2006_10_deg_CMF.csv`

 * *Files identical despite different names*

### Comparing `pysilsub-0.0.15/pysilsub/data/CIE_A_lms.csv` & `pysilsub-0.1.1/pysilsub/data/CIE_A_lms.csv`

 * *Files identical despite different names*

### Comparing `pysilsub-0.0.15/pysilsub/data/OneLight.csv` & `pysilsub-0.1.1/pysilsub/data/OneLight.csv`

 * *Files identical despite different names*

### Comparing `pysilsub-0.0.15/pysilsub/data/OneLight.json` & `pysilsub-0.1.1/pysilsub/data/OneLight.json`

 * *Files identical despite different names*

### Comparing `pysilsub-0.0.15/pysilsub/data/Prahl2012_bilurubin_absorption_spectrum.csv` & `pysilsub-0.1.1/pysilsub/data/Prahl2012_bilurubin_absorption_spectrum.csv`

 * *Files identical despite different names*

### Comparing `pysilsub-0.0.15/pysilsub/data/Prahl_Hgb.csv` & `pysilsub-0.1.1/pysilsub/data/Prahl_Hgb.csv`

 * *Files identical despite different names*

### Comparing `pysilsub-0.0.15/pysilsub/data/ProPixx.csv` & `pysilsub-0.1.1/pysilsub/data/ProPixx.csv`

 * *Files identical despite different names*

### Comparing `pysilsub-0.0.15/pysilsub/data/ProPixx.json` & `pysilsub-0.1.1/pysilsub/data/ProPixx.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'primary_colors'": "{insert: [(1, 'green'), (2, 'red')], delete: [1, 0]}"}*

```diff
@@ -6,17 +6,17 @@
         781,
         1
     ],
     "json_name": "ProPixx",
     "name": "ProPixx Projector",
     "notes": "VPixx ProPixx projector at the York Neuroimaging Center. Spectra were measured with an OceanOptics Jaz spectrometer using a long fiber optic cable.",
     "primary_colors": [
-        "red",
+        "blue",
         "green",
-        "blue"
+        "red"
     ],
     "primary_resolutions": [
         255,
         255,
         255
     ]
 }
```

### Comparing `pysilsub-0.0.15/pysilsub/data/STLAB_1_York.csv` & `pysilsub-0.1.1/pysilsub/data/STLAB_1_York.csv`

 * *Files identical despite different names*

### Comparing `pysilsub-0.0.15/pysilsub/data/STLAB_1_York.json` & `pysilsub-0.1.1/pysilsub/data/STLAB_1_York.json`

 * *Files identical despite different names*

### Comparing `pysilsub-0.0.15/pysilsub/data/STLAB_2_York.csv` & `pysilsub-0.1.1/pysilsub/data/STLAB_2_York.csv`

 * *Files identical despite different names*

### Comparing `pysilsub-0.0.15/pysilsub/data/STLAB_2_York.json` & `pysilsub-0.1.1/pysilsub/data/STLAB_2_York.json`

 * *Files identical despite different names*

### Comparing `pysilsub-0.0.15/pysilsub/data/VirtualSky.csv` & `pysilsub-0.1.1/pysilsub/data/VirtualSky.csv`

 * *Files identical despite different names*

### Comparing `pysilsub-0.0.15/pysilsub/data/VirtualSky.json` & `pysilsub-0.1.1/pysilsub/data/VirtualSky.json`

 * *Files identical despite different names*

### Comparing `pysilsub-0.0.15/pysilsub/data/linCIE2008v10e_1.csv` & `pysilsub-0.1.1/pysilsub/data/linCIE2008v10e_1.csv`

 * *Files identical despite different names*

### Comparing `pysilsub-0.0.15/pysilsub/data/rodent_action_spectra.csv` & `pysilsub-0.1.1/pysilsub/data/rodent_action_spectra.csv`

 * *Files identical despite different names*

### Comparing `pysilsub-0.0.15/pysilsub/devices.py` & `pysilsub-0.1.1/pysilsub/devices.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,21 +16,28 @@
 import importlib_resources
 import scipy
 import matplotlib.pyplot as plt
 import matplotlib as mpl
 import pandas as pd
 import numpy as np
 import numpy.typing as npt
-import colour
-
+try:
+    import colour
+except ImportError:
+    print('Failed to import "colour" package. Chromaticity plots will not be '
+          'as nice.')
+    
 from . import colorfuncs
 from . import CIE
 from . import observers
 
 
+plt.style.use('bmh')
+
+
 # Type aliases
 PrimaryInput = Union[int, float]
 PrimaryWeights = Sequence[float]
 PrimarySettings = Sequence[int]
 DeviceInput = Union[PrimarySettings, PrimaryWeights]
 PrimaryBounds = List[Tuple[float, float]]
 PrimaryColors = Union[Sequence[str], Sequence[Sequence[Union[int, float]]]]
@@ -113,15 +120,15 @@
         else:
             self.calibration = calibration
 
         self.primaries = (
             self.calibration.index.get_level_values(0).unique().tolist()
         )
         self.nprimaries = len(self.primaries)
-
+        
         self._assert_wavelengths_are_valid(calibration_wavelengths)
         self.calibration_wavelengths = calibration_wavelengths
 
         self._assert_resolutions_are_valid(primary_resolutions)
         self.primary_resolutions = primary_resolutions
 
         self._assert_colors_are_valid(primary_colors)
@@ -353,15 +360,15 @@
         """Check device input is sensible."""
         if len(multiprimary_input) != self.nprimaries:
             raise StimulationDeviceError(
                 "Number of primary inputs does not match number of device ",
                 "primaries.",
             )
 
-        for primary, primary_input in enumerate(multiprimary_input):
+        for primary, primary_input in zip(self.primaries, multiprimary_input):
             self._assert_primary_input_is_valid(primary, primary_input)
 
     def _assert_wavelengths_are_valid(
         self, wavelengths: Sequence[int | float]
     ) -> None:
         """Check wavelengths match those in the calibration file."""
         if not all(
@@ -493,17 +500,22 @@
         ax : matplotlib.axes.Axes
 
         """
         gamut = self._get_gamut()
         if ax is None:
             ax = plt.gca()
         if show_1931_horseshoe:
-            colour.plotting.plot_chromaticity_diagram_CIE1931(
-                axes=ax, title=False, standalone=False
-            )
+            try:
+                colour.plotting.plot_chromaticity_diagram_CIE1931(
+                    axes=ax, title=False, standalone=False
+                    )
+            except NameError:
+                print('Unable to display chromaticity horseshoe as the ',
+                      '"colour" package is not installed.')
+
         if show_CIE170_2_horseshoe:
             cie170_2 = CIE.get_CIE170_2_chromaticity_coordinates()
             cie_horse = ax.plot(
                 cie170_2["x"], cie170_2["y"], c="k", ls=":", label="CIE 170-2"
             )
 
         # Defaults plot kws
@@ -562,15 +574,15 @@
                 ylabel = "Power"
 
         # Plot defaults
         lw = kwargs.pop("lw", 0.5)
         legend = kwargs.pop("legend", True)
 
         # Plot spds
-        for primary, color in enumerate(self.primary_colors):
+        for primary, color in zip(self.primaries, self.primary_colors):
             self.calibration.loc[primary].T.plot(
                 c=color, lw=lw, ax=ax, legend=False
             )
 
         # Add legend
         if legend:
             handles = [
@@ -692,15 +704,15 @@
             Predicted spectra or spectrum for given device settings.
 
         """
         self._assert_multiprimary_input_is_valid(multiprimary_input)
         if name is None:
             name = 0
         spd = []
-        for primary, primary_input in enumerate(multiprimary_input):
+        for primary, primary_input in zip(self.primaries, multiprimary_input):
             spd.append(
                 self.predict_primary_spd(primary, primary_input, name=primary)
             )
         spd = pd.concat(spd, axis=1)
         if nosum:
             spd.columns.name = "Primary"
             return spd
@@ -959,15 +971,15 @@
 
             new_x = (new_x * self.primary_resolutions[primary]).astype("int")
 
             # Interpolate for full lookup table
             gamma_table.append(new_x)
 
         gamma_table = (
-            pd.DataFrame(gamma_table, columns=settings)
+            pd.DataFrame(gamma_table, columns=settings, index=self.primaries)
             .reindex(columns=range(0, max(self.primary_resolutions) + 1))
             .interpolate("linear", axis=1)
             .astype("int")
         )
 
         # TODO temp fix, make generic
         gamma_table = gamma_table.clip(0, 4095)
@@ -1082,15 +1094,15 @@
         list
             Gamma corrected multiprimary input values.
 
         """
         self._assert_multiprimary_input_is_valid(multiprimary_input)
         return [
             self.gamma_lookup(primary, primary_input)
-            for primary, primary_input in enumerate(multiprimary_input)
+            for primary, primary_input in zip(self.primaries, multiprimary_input)
         ]
 
     def s2w(self, settings: PrimarySettings) -> list[float]:
         """Convert settings to weights.
 
         Parameters
         ----------
```

### Comparing `pysilsub-0.0.15/pysilsub/observers.py` & `pysilsub-0.1.1/pysilsub/observers.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,17 @@
 import pandas as pd
 import matplotlib.pyplot as plt
 
 from . import CIE
 from . import preceps
 
 
+plt.style.use('bmh')
+
+
 class ObserverError(Exception):
     """Generic Python-exception-derived object.
 
     Raised programmatically by Observer class methods when arguments are
     incorrectly specified or when they do not agree with values of other.
     """
 
@@ -105,18 +108,15 @@
         return self._action_spectra
 
     @action_spectra.setter
     def action_spectra(self, action_spectra: pd.DataFrame) -> None:
         """Set the observer action spectra."""
         self._action_spectra = action_spectra
         self.photoreceptors = action_spectra.columns.to_list()
-        print(
-            "Assigned new (probably not suitable) colors for action spectra."
-        )
-        nreceptors = len(self.photoreceptors)
+        self.nreceptors = len(self.photoreceptors)
 
     def save_action_spectra(self, save_to: str = "."):
         """Save observer action spectra to csv.
 
         Parameters
         ----------
         save_to : str, optional
```

### Comparing `pysilsub-0.0.15/pysilsub/preceps.py` & `pysilsub-0.1.1/pysilsub/preceps.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 ``pysilsub.preceps``
 ====================
 
 Convenience functions for accessing prereceptoral filter functions.
 
 
 """
+from __future__ import annotations
+
 
 from typing import Optional, Union, Sequence
 
 import numpy as np
 import pandas as pd
 import importlib_resources
```

### Comparing `pysilsub-0.0.15/pysilsub/problems.py` & `pysilsub-0.1.1/pysilsub/problems.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,22 +14,27 @@
 
 import numpy as np
 import numpy.typing as npt
 import scipy
 import pandas as pd
 import matplotlib.pyplot as plt
 from matplotlib import animation
-import colour
+try:
+    import colour
+except ImportError:
+    print('Failed to import "colour" package. Chromaticity plots will not be '
+          'as nice.')
 
 from . import devices
 from . import colorfuncs
 from . import observers
 from . import CIE
 from . import waves
 
+plt.style.use('bmh')
 
 class SilSubProblemError(Exception):
     """Generic Python-exception-derived object.
 
     Raised programmatically by ``SilentSubstitutionProblem`` methods when
     arguments are incorrectly specified or when they do not agree with values
     of other .
@@ -564,16 +569,16 @@
     def print_problem(self) -> None:
         """Print the current problem definition."""
         self._assert_problem_is_valid()
         print(f"{'*'*60}\n{' Silent Substitution Problem ':*^60s}\n{'*'*60}")
         print(f"Device: {self.name}")
         print(f"Observer: {self.observer}")
         print(f"Ignoring: {self._ignore}")
-        print(f"Minimising: {self._silence}")
-        print(f"Modulating: {self._target}")
+        print(f"Silencing: {self._silence}")
+        print(f"Targeting: {self._target}")
         print(f"Target contrast: {self._target_contrast}")
         print(f"Background: {self._background}")
         print("\n")
 
     # Useful stuff now
     def initial_guess_x0(self) -> npt.NDArray:
         """Return an initial guess of the primary inputs for optimization.
@@ -656,21 +661,21 @@
             Photoreceptor contrasts.
 
         """
         bg_aopic, mod_aopic = self.aopic_calculator(x0)
 
         if contrast_statistic == "simple":
             return mod_aopic.sub(bg_aopic).div(bg_aopic)
-
-        max_aopic = pd.concat([bg_aopic, mod_aopic], axis=1).max(axis=1)
-        min_aopic = pd.concat([bg_aopic, mod_aopic], axis=1).min(axis=1)
-        if contrast_statistic == "weber":
-            return (max_aopic - min_aopic) / (max_aopic)
-        elif contrast_statistic == "michelson":
-            return (max_aopic - min_aopic) / (max_aopic + min_aopic)
+        else:
+            max_aopic = pd.concat([bg_aopic, mod_aopic], axis=1).max(axis=1)
+            min_aopic = pd.concat([bg_aopic, mod_aopic], axis=1).min(axis=1)
+            if contrast_statistic == "weber":
+                return (max_aopic - min_aopic) / (max_aopic)
+            elif contrast_statistic == "michelson":
+                return (max_aopic - min_aopic) / (max_aopic + min_aopic)
 
     def objective_function(self, x0: devices.PrimaryWeights) -> float:
         """Calculate contrast error on targeted photoreceptor(s).
 
         This happens in accordance with the problem definition.
 
         Parameters
@@ -1017,17 +1022,21 @@
         bg_xy, mod_xy = self.get_solution_xy(solution)
 
         # Make plot
         if ax is None:
             ax = plt.gca()
 
         # Plot solution on horseshoe
-        colour.plotting.plot_chromaticity_diagram_CIE1931(
-            axes=ax, title=False, standalone=False
-        )
+        try:
+            colour.plotting.plot_chromaticity_diagram_CIE1931(
+                axes=ax, title=False, standalone=False
+            )
+        except NameError:
+            print('Unable to display chromaticity horseshoe as the ',
+                  '"colour" package is not installed.')
 
         cie170_2 = CIE.get_CIE170_2_chromaticity_coordinates()
         ax.plot(cie170_2["x"], cie170_2["y"], c="k", ls=":", label="CIE 170-2")
         ax.legend()
         ax.set(title="CIE 1931 horseshoe", xlim=(-0.1, 0.9), ylim=(-0.1, 0.9))
 
         # Chromaticity
@@ -1047,15 +1056,15 @@
             c="k",
             marker="x",
             label="Modulation",
         )
         ax.legend()
         return ax
 
-    def plot_solution_aopic(self, solution, ax=None, **kwargs):
+    def plot_solution_aopic(self, solution, ax: plt.Axes = None, **kwargs):
         """Plot barchart of alphaopic irradiances .
 
         Parameters
         ----------
         solution : array_like
             The solution returned by one of the solvers.
         ax : plt.Axes, optional
@@ -1136,30 +1145,30 @@
         print(f"Modulation spectrum: {self.w2s(mod_weights)}")
 
     # TODO: polish
     def make_contrast_modulation(
         self,
         frequency: int | float,
         sampling_frequency: int,
-        target_contrast: float,
+        target_contrasts: list[float],
         phase: int | float = 0,
         duration: int | float = 1
         ):
         """Make a sinusoidal contrast modulation.
 
         Parameters
         ----------
         frequency : int | float
             Modulation frequency in Hz.
         sampling_frequency : int
             Sampling frequency of the modulation. This should not exceed the
             temporal resolution (spectral switching time) of the stimulation
             device.
-        target_contrast : float
-            Peak contrast of the modulation for targetted photoreceptor(s).
+        target_contrast : list(float)
+            Peak contrast of the modulation for targeted photoreceptor(s).
         phase : int | float, optional
             Phase offset. The default is 0. Use np.pi
         duration : int | float, optional
             Duration of the modulation. The default is 1.
 
         Returns
         -------
@@ -1172,48 +1181,49 @@
             sampling_frequency,
             phase,
             duration,
         )
 
         solutions = []
         for point in waveform:
-            contrast = point * target_contrast
+            contrast = [point * c for c in target_contrasts]
             self.target_contrast = contrast
             solutions.append(self.linalg_solve())
         return solutions
 
     # TODO: Fix
-    def plot_contrast_modulation(self, solutions: list, **kwargs):
+    def plot_contrast_modulation(self, solutions: list, ax: plt.Axes = None, **kwargs):
         """Plot photoreceptor contrast over time for a list of solutions.
 
         Parameters
         ----------
         solutions : list
             List of solutions returned by one of the solvers (one for each
             timepoint in the modulation).
 
         Returns
         -------
         fig : plt.Figure
             The plot.
 
         """
-        fig, ax = plt.subplots(1, 1, figsize=(3.54, 3.54))
+        if ax is None:
+            ax = plt.gca()
 
         # Calculate contrast for all photoreceptors
         contrasts = [self.get_photoreceptor_contrasts(s) for s in solutions]
         contrasts = pd.concat(contrasts, axis=1)
 
         # Plot
-        contrasts.T.plot(ax=ax, color=self.observer.photoreceptor_colors)
+        contrasts.T.plot(ax=ax, color=self.observer.photoreceptor_colors, **kwargs)
         ax.set_ylabel("Contrast")
         ax.set_title(self.name)
         ax.set_xlabel("Time point")
 
-        return fig
+        return ax
 
     def animate_solutions(self, solutions, save_to=None):
         """Something here.
 
         Parameters
         ----------
         solutions : TYPE
```

### Comparing `pysilsub-0.0.15/pysilsub/waves.py` & `pysilsub-0.1.1/pysilsub/waves.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 ==================
 
 Convenience functions for accessing prereceptoral filter functions.
 
 
 """
 
+from __future__ import annotations
+
+
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 
 
 def make_stimulus_waveform(
     frequency: int | float,
```

### Comparing `pysilsub-0.0.15/pysilsub.egg-info/PKG-INFO` & `pysilsub-0.1.1/pysilsub.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 Metadata-Version: 2.1
 Name: pysilsub
-Version: 0.0.15
+Version: 0.1.1
 Summary: Software for performing silent substitution in Python.
 Home-page: https://github.com/PySilentSubstitution/pysilsub
 Author: Joel T. Martin
 Author-email: joel.t.martin36@gmail.com
 License: MIT
 Project-URL: Documentation, https://pysilentsubstitution.github.io/pysilsub/index.html
 Keywords: silent substitution,vision,psychology,perception,metamer,spectra,LED
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3.7
-Requires-Python: >=3.8, <3.11
+Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Welcome to PySilentSubstitution!
 ================================
 
-
-
 [![DOI](https://zenodo.org/badge/390693759.svg)](https://zenodo.org/badge/latestdoi/390693759) [![PyPI version](https://badge.fury.io/py/pysilsub.svg)](https://badge.fury.io/py/pysilsub) [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.0-4baaaa.svg)](./CODE_OF_CONDUCT.md)  [![PyPi license](https://badgen.net/pypi/license/pip/)](https://pypi.com/project/pip/) [![PyPI status](https://img.shields.io/pypi/status/ansicolortags.svg)](https://pypi.python.org/pypi/ansicolortags/) 
 
 <img src="https://github.com/PySilentSubstitution/pysilsub/blob/main/logo/photoreceptor_characters.png?raw=True" alt="photoreceptor-characters" width="200"/>
 
-*PySilSub* is a Python toolbox for performing the method of [silent substitution](https://pysilentsubstitution.github.io/pysilsub/01_background.html) in vision and circadian research.
+*PySilSub* is a Python toolbox for performing the method of [silent substitution](https://pysilentsubstitution.github.io/pysilsub/01_background.html) in vision and nonvisual photoreception research.
 
 **Note:** See also, [PyPlr](https://pyplr.github.io/cvd_pupillometry/index.html),
 a sister project offering a Python framework for researching the pupillary 
 light reflex with the Pupil Core eye tracking platform.
 
 With *PySilSub*, observer- and device-specific solutions to silent substitution 
 problems are found with linear algebra or numerical optimisation via a configurable, 
@@ -67,16 +65,16 @@
 # algebra.
 
 from pysilsub import problems
 
 ssp = problems.SilentSubstitutionProblem.from_package_data('STLAB_1_York')  # Load example data
 ssp.background = [.5] * ssp.nprimaries  # Specify background spectrum
 ssp.ignore = ['rh']  # Ignore rod photoreceptors
-ssp.silence = ['sc', 'mc', 'lc']  # Minimise cone contrast
-ssp.target = ['mel']  # Target melanopsin
+ssp.silence = ['mc', 'lc', 'mel']  # Silence L/M cones and melanopsin
+ssp.target = ['sc']  # Target S cones
 ssp.target_contrast = .45  # With 45% contrast 
 solution = ssp.linalg_solve()  # Solve with linear algebra
 fig = ssp.plot_solution(solution)  # Plot the solution
 ```
 
 <img src="https://raw.githubusercontent.com/PySilentSubstitution/pysilsub/main/img/example_2.svg" alt="Example 2" />
```

### Comparing `pysilsub-0.0.15/pysilsub.egg-info/SOURCES.txt` & `pysilsub-0.1.1/pysilsub.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 pysilsub/.DS_Store
 pysilsub/CIE.py
 pysilsub/__init__.py
+pysilsub/binocular.py
 pysilsub/colorfuncs.py
 pysilsub/config.py
 pysilsub/devices.py
 pysilsub/observers.py
 pysilsub/preceps.py
 pysilsub/problems.py
 pysilsub/waves.py
@@ -26,28 +27,26 @@
 pysilsub/data/CIEPO06_macula_density.csv
 pysilsub/data/CIEPO06_optical_density.csv
 pysilsub/data/CIES026.csv
 pysilsub/data/CIE_1924_photopic_vl.csv
 pysilsub/data/CIE_1931_2_deg_CMF.csv
 pysilsub/data/CIE_2006_10_deg_CMF.csv
 pysilsub/data/CIE_A_lms.csv
-pysilsub/data/LEDCube.csv
-pysilsub/data/LEDCube.json
+pysilsub/data/CRT.csv
+pysilsub/data/CRT.json
 pysilsub/data/OneLight.csv
 pysilsub/data/OneLight.json
 pysilsub/data/Prahl2012_bilurubin_absorption_spectrum.csv
 pysilsub/data/Prahl_Hgb.csv
 pysilsub/data/ProPixx.csv
 pysilsub/data/ProPixx.json
 pysilsub/data/STLAB_1_York.csv
 pysilsub/data/STLAB_1_York.json
 pysilsub/data/STLAB_2_York.csv
 pysilsub/data/STLAB_2_York.json
-pysilsub/data/STLAB_Oxford.csv
-pysilsub/data/STLAB_Oxford.json
 pysilsub/data/VirtualSky.csv
 pysilsub/data/VirtualSky.json
 pysilsub/data/linCIE2008v10e_1.csv
 pysilsub/data/rodent_action_spectra.csv
 pysilsub/data/vanKampen_Hgb.csv
 pysilsub/data/.ipynb_checkpoints/OneLight-checkpoint.json
 pysilsub/data/.ipynb_checkpoints/ProPixx-checkpoint.json
```

### Comparing `pysilsub-0.0.15/setup.py` & `pysilsub-0.1.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,37 +3,37 @@
 import setuptools
 
 with open('./README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pysilsub', # Replace with your own username
-    version='0.0.15',
+    version='0.1.1',
     author='Joel T. Martin',
     author_email='joel.t.martin36@gmail.com',
     description='Software for performing silent substitution in Python.',
     license='MIT',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/PySilentSubstitution/pysilsub',
     keywords=['silent substitution', 'vision', 'psychology', 'perception', 'metamer', 'spectra', 'LED'],
     project_urls={
         'Documentation': 'https://pysilentsubstitution.github.io/pysilsub/index.html'},
-    python_requires='>=3.8, <3.11',
+    python_requires='>=3.8',
     install_requires=[
         'numpy',
         'scipy',
         'matplotlib',
         'pandas',
         'importlib-resources',
-        'colour-science'
+        #'colour-science'
         ],
     packages=setuptools.find_packages(),
     include_package_data=True,
     classifiers=[
           'Development Status :: 2 - Pre-Alpha',
           'Topic :: Scientific/Engineering :: Information Analysis',
           'License :: OSI Approved :: MIT License',
           'Intended Audience :: Science/Research',
-          'Programming Language :: Python :: 3.7'
+          'Programming Language :: Python :: 3.8'
           ]
       )
```

