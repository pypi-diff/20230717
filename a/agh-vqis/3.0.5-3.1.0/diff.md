# Comparing `tmp/agh_vqis-3.0.5.tar.gz` & `tmp/agh_vqis-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agh_vqis-3.0.5.tar", last modified: Wed Jul  5 07:22:50 2023, max compression
+gzip compressed data, was "agh_vqis-3.1.0.tar", last modified: Mon Jul 17 00:46:03 2023, max compression
```

## Comparing `agh_vqis-3.0.5.tar` & `agh_vqis-3.1.0.tar`

### file list

```diff
@@ -1,147 +1,147 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 07:22:50.725638 agh_vqis-3.0.5/
--rw-rw-rw-   0        0        0     2826 2023-01-28 21:45:19.000000 agh_vqis-3.0.5/LICENSE
--rw-rw-rw-   0        0        0    12782 2023-07-05 07:22:50.725638 agh_vqis-3.0.5/PKG-INFO
--rw-rw-rw-   0        0        0    11774 2023-07-05 07:22:06.000000 agh_vqis-3.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-05 07:22:50.429171 agh_vqis-3.0.5/agh_vqis.egg-info/
--rw-rw-rw-   0        0        0    12782 2023-07-05 07:22:50.000000 agh_vqis-3.0.5/agh_vqis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8111 2023-07-05 07:22:50.000000 agh_vqis-3.0.5/agh_vqis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 07:22:50.000000 agh_vqis-3.0.5/agh_vqis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      206 2023-07-05 07:22:50.000000 agh_vqis-3.0.5/agh_vqis.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-05 07:22:50.000000 agh_vqis-3.0.5/agh_vqis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       97 2023-01-28 21:02:34.000000 agh_vqis-3.0.5/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-07-05 07:22:50.390164 agh_vqis-3.0.5/python-cpbd/
-drwxrwxrwx   0        0        0        0 2023-07-05 07:22:50.433170 agh_vqis-3.0.5/python-cpbd/cpbd/
--rw-rw-rw-   0        0        0       49 2023-01-28 22:00:29.000000 agh_vqis-3.0.5/python-cpbd/cpbd/__init__.py
--rw-rw-rw-   0        0        0     7670 2023-01-28 22:00:29.000000 agh_vqis-3.0.5/python-cpbd/cpbd/compute.py
--rw-rw-rw-   0        0        0     1540 2023-01-28 22:00:29.000000 agh_vqis-3.0.5/python-cpbd/cpbd/octave.py
--rw-rw-rw-   0        0        0     1329 2023-07-05 07:22:50.728629 agh_vqis-3.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-05 07:22:50.391162 agh_vqis-3.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-07-05 07:22:50.438174 agh_vqis-3.0.5/src/agh_vqis/
--rw-rw-rw-   0        0        0      381 2023-07-05 07:22:17.000000 agh_vqis-3.0.5/src/agh_vqis/__init__.py
--rw-rw-rw-   0        0        0    22326 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/__main__.py
--rw-rw-rw-   0        0        0     1349 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/_logger.py
-drwxrwxrwx   0        0        0        0 2023-07-05 07:22:50.445245 agh_vqis-3.0.5/src/agh_vqis/binaries/
--rw-rw-rw-   0        0        0    97508 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/binaries/agh_vqis_binary_macosx_mt
--rwxrwxrwx   0        0        0   122077 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/binaries/agh_vqis_binary_win64_mt.exe
--rw-rw-rw-   0        0        0    66424 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/binaries/agh_vqis_binary_x86_mt
--rw-rw-rw-   0        0        0  2952245 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/binaries/cygwin1.dll
-drwxrwxrwx   0        0        0        0 2023-07-05 07:22:50.392161 agh_vqis-3.0.5/src/agh_vqis/models/
-drwxrwxrwx   0        0        0        0 2023-07-05 07:22:50.716622 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/
--rw-rw-rw-   0        0        0    21075 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Blockiness_1080p_1440p.xgb
--rw-rw-rw-   0        0        0    21723 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Blockiness_1080p_2160p.xgb
--rw-rw-rw-   0        0        0    14595 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Blockiness_1440p_2160p.xgb
--rw-rw-rw-   0        0        0    15027 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Blockiness_2160p_1440p.xgb
--rw-rw-rw-   0        0        0    32379 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Blur_1080p_1440p.xgb
--rw-rw-rw-   0        0        0    35763 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Blur_1080p_2160p.xgb
--rw-rw-rw-   0        0        0    34323 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Blur_1440p_1080p.xgb
--rw-rw-rw-   0        0        0    34323 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Blur_1440p_2160p.xgb
--rw-rw-rw-   0        0        0    37059 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Blur_2160p_1080p.xgb
--rw-rw-rw-   0        0        0    34035 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Blur_2160p_1440p.xgb
--rw-rw-rw-   0        0        0    29643 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Blur_240p_360p.xgb
--rw-rw-rw-   0        0        0    33747 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Blur_240p_480p.xgb
--rw-rw-rw-   0        0        0    28059 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Blur_360p_240p.xgb
--rw-rw-rw-   0        0        0    29787 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Blur_360p_480p.xgb
--rw-rw-rw-   0        0        0    33531 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Blur_360p_720p.xgb
--rw-rw-rw-   0        0        0    29355 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Blur_480p_240p.xgb
--rw-rw-rw-   0        0        0    26691 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Blur_480p_360p.xgb
--rw-rw-rw-   0        0        0    31803 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Blur_480p_720p.xgb
--rw-rw-rw-   0        0        0    37779 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Blur_720p_1080p.xgb
--rw-rw-rw-   0        0        0    30291 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Blur_720p_360p.xgb
--rw-rw-rw-   0        0        0    30795 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Blur_720p_480p.xgb
--rw-rw-rw-   0        0        0    27195 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_1440p.xgb
--rw-rw-rw-   0        0        0    26907 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_2160p.xgb
--rw-rw-rw-   0        0        0    38355 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_240p.xgb
--rw-rw-rw-   0        0        0    39075 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_360p.xgb
--rw-rw-rw-   0        0        0    37635 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_480p.xgb
--rw-rw-rw-   0        0        0    37059 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_720p.xgb
--rw-rw-rw-   0        0        0    26979 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_1080p.xgb
--rw-rw-rw-   0        0        0    27339 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_2160p.xgb
--rw-rw-rw-   0        0        0    38571 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_240p.xgb
--rw-rw-rw-   0        0        0    39219 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_360p.xgb
--rw-rw-rw-   0        0        0    37923 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_480p.xgb
--rw-rw-rw-   0        0        0    37995 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_720p.xgb
--rw-rw-rw-   0        0        0    27339 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_1080p.xgb
--rw-rw-rw-   0        0        0    27267 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_1440p.xgb
--rw-rw-rw-   0        0        0    38643 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_240p.xgb
--rw-rw-rw-   0        0        0    39363 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_360p.xgb
--rw-rw-rw-   0        0        0    38067 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_480p.xgb
--rw-rw-rw-   0        0        0    38211 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_720p.xgb
--rw-rw-rw-   0        0        0    36915 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_240p_1080p.xgb
--rw-rw-rw-   0        0        0    37851 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_240p_1440p.xgb
--rw-rw-rw-   0        0        0    37347 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_240p_2160p.xgb
--rw-rw-rw-   0        0        0    28779 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_240p_360p.xgb
--rw-rw-rw-   0        0        0    29715 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_240p_480p.xgb
--rw-rw-rw-   0        0        0    30219 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_240p_720p.xgb
--rw-rw-rw-   0        0        0    37779 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_360p_1080p.xgb
--rw-rw-rw-   0        0        0    38283 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_360p_1440p.xgb
--rw-rw-rw-   0        0        0    37563 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_360p_2160p.xgb
--rw-rw-rw-   0        0        0    27843 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_360p_240p.xgb
--rw-rw-rw-   0        0        0    27267 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_360p_480p.xgb
--rw-rw-rw-   0        0        0    27699 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_360p_720p.xgb
--rw-rw-rw-   0        0        0    37635 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_480p_1080p.xgb
--rw-rw-rw-   0        0        0    37275 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_480p_1440p.xgb
--rw-rw-rw-   0        0        0    37851 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_480p_2160p.xgb
--rw-rw-rw-   0        0        0    29283 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_480p_240p.xgb
--rw-rw-rw-   0        0        0    27483 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_480p_360p.xgb
--rw-rw-rw-   0        0        0    26979 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_480p_720p.xgb
--rw-rw-rw-   0        0        0    37347 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_720p_1080p.xgb
--rw-rw-rw-   0        0        0    38139 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_720p_1440p.xgb
--rw-rw-rw-   0        0        0    37779 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_720p_2160p.xgb
--rw-rw-rw-   0        0        0    29787 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_720p_240p.xgb
--rw-rw-rw-   0        0        0    27195 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_720p_360p.xgb
--rw-rw-rw-   0        0        0    27195 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_720p_480p.xgb
--rw-rw-rw-   0        0        0    17259 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_1440p.xgb
--rw-rw-rw-   0        0        0    17835 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_2160p.xgb
--rw-rw-rw-   0        0        0    27411 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_360p.xgb
--rw-rw-rw-   0        0        0    25179 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_480p.xgb
--rw-rw-rw-   0        0        0    22659 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_720p.xgb
--rw-rw-rw-   0        0        0    17259 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_1080p.xgb
--rw-rw-rw-   0        0        0    17187 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_2160p.xgb
--rw-rw-rw-   0        0        0    25395 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_480p.xgb
--rw-rw-rw-   0        0        0    23955 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_720p.xgb
--rw-rw-rw-   0        0        0    19491 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_1080p.xgb
--rw-rw-rw-   0        0        0    16827 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_1440p.xgb
--rw-rw-rw-   0        0        0    23667 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_720p.xgb
--rw-rw-rw-   0        0        0    19491 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_360p.xgb
--rw-rw-rw-   0        0        0    20571 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_480p.xgb
--rw-rw-rw-   0        0        0    22299 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_720p.xgb
--rw-rw-rw-   0        0        0    22155 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_1080p.xgb
--rw-rw-rw-   0        0        0    19059 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_240p.xgb
--rw-rw-rw-   0        0        0    18987 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_480p.xgb
--rw-rw-rw-   0        0        0    20571 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_720p.xgb
--rw-rw-rw-   0        0        0    23163 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_1080p.xgb
--rw-rw-rw-   0        0        0    22803 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_1440p.xgb
--rw-rw-rw-   0        0        0    22011 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_240p.xgb
--rw-rw-rw-   0        0        0    20283 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_360p.xgb
--rw-rw-rw-   0        0        0    18123 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_720p.xgb
--rw-rw-rw-   0        0        0    22947 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_1080p.xgb
--rw-rw-rw-   0        0        0    22803 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_1440p.xgb
--rw-rw-rw-   0        0        0    22587 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_2160p.xgb
--rw-rw-rw-   0        0        0    23955 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_240p.xgb
--rw-rw-rw-   0        0        0    21435 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_360p.xgb
--rw-rw-rw-   0        0        0    18699 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_480p.xgb
--rw-rw-rw-   0        0        0     4587 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Interlace_1080p_1440p.xgb
--rw-rw-rw-   0        0        0     5739 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Interlace_240p_360p.xgb
--rw-rw-rw-   0        0        0     6459 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Interlace_360p_240p.xgb
--rw-rw-rw-   0        0        0     5307 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Interlace_360p_480p.xgb
--rw-rw-rw-   0        0        0     5811 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Interlace_480p_360p.xgb
--rw-rw-rw-   0        0        0     4947 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Interlace_480p_720p.xgb
--rw-rw-rw-   0        0        0     5379 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Interlace_720p_1080p.xgb
--rw-rw-rw-   0        0        0     5163 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Interlace_720p_480p.xgb
--rw-rw-rw-   0        0        0    40443 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Noise_1080p_1440p.xgb
--rw-rw-rw-   0        0        0    43467 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Noise_1080p_2160p.xgb
--rw-rw-rw-   0        0        0    39435 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Noise_1440p_1080p.xgb
--rw-rw-rw-   0        0        0    42171 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Noise_1440p_2160p.xgb
--rw-rw-rw-   0        0        0    38787 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Noise_2160p_1440p.xgb
--rw-rw-rw-   0        0        0    42747 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Noise_240p_360p.xgb
--rw-rw-rw-   0        0        0    39939 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Noise_360p_240p.xgb
--rw-rw-rw-   0        0        0    41235 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Noise_360p_480p.xgb
--rw-rw-rw-   0        0        0    38931 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Noise_480p_360p.xgb
--rw-rw-rw-   0        0        0    40875 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Noise_480p_720p.xgb
--rw-rw-rw-   0        0        0    37923 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Noise_720p_480p.xgb
-drwxrwxrwx   0        0        0        0 2023-07-05 07:22:50.718627 agh_vqis-3.0.5/src/agh_vqis/models/ugc/
--rw-rw-rw-   0        0        0   594166 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/models/ugc/12k_all_set.json
-drwxrwxrwx   0        0        0        0 2023-07-05 07:22:50.723623 agh_vqis-3.0.5/src/agh_vqis/utils/
--rw-rw-rw-   0        0        0     5470 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/utils/helpers.py
--rw-rw-rw-   0        0        0      754 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/utils/resolution_cast.py
--rw-rw-rw-   0        0        0     5735 2023-06-21 16:42:58.000000 agh_vqis-3.0.5/src/agh_vqis/utils/ugc.py
+drwxrwxrwx   0        0        0        0 2023-07-17 00:46:03.870504 agh_vqis-3.1.0/
+-rw-rw-rw-   0        0        0     2826 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/LICENSE
+-rw-rw-rw-   0        0        0    13218 2023-07-17 00:46:03.870504 agh_vqis-3.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0    12210 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 00:46:03.184081 agh_vqis-3.1.0/agh_vqis.egg-info/
+-rw-rw-rw-   0        0        0    13218 2023-07-17 00:46:03.000000 agh_vqis-3.1.0/agh_vqis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8111 2023-07-17 00:46:03.000000 agh_vqis-3.1.0/agh_vqis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 00:46:03.000000 agh_vqis-3.1.0/agh_vqis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      206 2023-07-17 00:46:03.000000 agh_vqis-3.1.0/agh_vqis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-17 00:46:03.000000 agh_vqis-3.1.0/agh_vqis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       97 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-07-17 00:46:03.168754 agh_vqis-3.1.0/python-cpbd/
+drwxrwxrwx   0        0        0        0 2023-07-17 00:46:03.185292 agh_vqis-3.1.0/python-cpbd/cpbd/
+-rw-rw-rw-   0        0        0       49 2023-07-16 23:41:56.000000 agh_vqis-3.1.0/python-cpbd/cpbd/__init__.py
+-rw-rw-rw-   0        0        0     7670 2023-07-16 23:41:56.000000 agh_vqis-3.1.0/python-cpbd/cpbd/compute.py
+-rw-rw-rw-   0        0        0     1540 2023-07-16 23:41:56.000000 agh_vqis-3.1.0/python-cpbd/cpbd/octave.py
+-rw-rw-rw-   0        0        0     1329 2023-07-17 00:46:03.870504 agh_vqis-3.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-17 00:46:03.168754 agh_vqis-3.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-17 00:46:03.191438 agh_vqis-3.1.0/src/agh_vqis/
+-rw-rw-rw-   0        0        0      381 2023-07-17 00:45:08.000000 agh_vqis-3.1.0/src/agh_vqis/__init__.py
+-rw-rw-rw-   0        0        0    22456 2023-07-17 00:20:36.000000 agh_vqis-3.1.0/src/agh_vqis/__main__.py
+-rw-rw-rw-   0        0        0     1349 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/_logger.py
+drwxrwxrwx   0        0        0        0 2023-07-17 00:46:03.197525 agh_vqis-3.1.0/src/agh_vqis/binaries/
+-rw-rw-rw-   0        0        0    97508 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/binaries/agh_vqis_binary_macosx_mt
+-rwxrwxrwx   0        0        0   122077 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/binaries/agh_vqis_binary_win64_mt.exe
+-rw-rw-rw-   0        0        0    66424 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/binaries/agh_vqis_binary_x86_mt
+-rw-rw-rw-   0        0        0  2952245 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/binaries/cygwin1.dll
+drwxrwxrwx   0        0        0        0 2023-07-17 00:46:03.168754 agh_vqis-3.1.0/src/agh_vqis/models/
+drwxrwxrwx   0        0        0        0 2023-07-17 00:46:03.870504 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/
+-rw-rw-rw-   0        0        0    21075 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blockiness_1080p_1440p.xgb
+-rw-rw-rw-   0        0        0    21723 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blockiness_1080p_2160p.xgb
+-rw-rw-rw-   0        0        0    14595 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blockiness_1440p_2160p.xgb
+-rw-rw-rw-   0        0        0    15027 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blockiness_2160p_1440p.xgb
+-rw-rw-rw-   0        0        0    32379 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_1080p_1440p.xgb
+-rw-rw-rw-   0        0        0    35763 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_1080p_2160p.xgb
+-rw-rw-rw-   0        0        0    34323 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_1440p_1080p.xgb
+-rw-rw-rw-   0        0        0    34323 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_1440p_2160p.xgb
+-rw-rw-rw-   0        0        0    37059 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_2160p_1080p.xgb
+-rw-rw-rw-   0        0        0    34035 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_2160p_1440p.xgb
+-rw-rw-rw-   0        0        0    29643 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_240p_360p.xgb
+-rw-rw-rw-   0        0        0    33747 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_240p_480p.xgb
+-rw-rw-rw-   0        0        0    28059 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_360p_240p.xgb
+-rw-rw-rw-   0        0        0    29787 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_360p_480p.xgb
+-rw-rw-rw-   0        0        0    33531 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_360p_720p.xgb
+-rw-rw-rw-   0        0        0    29355 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_480p_240p.xgb
+-rw-rw-rw-   0        0        0    26691 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_480p_360p.xgb
+-rw-rw-rw-   0        0        0    31803 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_480p_720p.xgb
+-rw-rw-rw-   0        0        0    37779 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_720p_1080p.xgb
+-rw-rw-rw-   0        0        0    30291 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_720p_360p.xgb
+-rw-rw-rw-   0        0        0    30795 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_720p_480p.xgb
+-rw-rw-rw-   0        0        0    27195 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_1440p.xgb
+-rw-rw-rw-   0        0        0    26907 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_2160p.xgb
+-rw-rw-rw-   0        0        0    38355 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_240p.xgb
+-rw-rw-rw-   0        0        0    39075 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_360p.xgb
+-rw-rw-rw-   0        0        0    37635 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_480p.xgb
+-rw-rw-rw-   0        0        0    37059 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_720p.xgb
+-rw-rw-rw-   0        0        0    26979 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_1080p.xgb
+-rw-rw-rw-   0        0        0    27339 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_2160p.xgb
+-rw-rw-rw-   0        0        0    38571 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_240p.xgb
+-rw-rw-rw-   0        0        0    39219 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_360p.xgb
+-rw-rw-rw-   0        0        0    37923 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_480p.xgb
+-rw-rw-rw-   0        0        0    37995 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_720p.xgb
+-rw-rw-rw-   0        0        0    27339 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_1080p.xgb
+-rw-rw-rw-   0        0        0    27267 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_1440p.xgb
+-rw-rw-rw-   0        0        0    38643 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_240p.xgb
+-rw-rw-rw-   0        0        0    39363 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_360p.xgb
+-rw-rw-rw-   0        0        0    38067 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_480p.xgb
+-rw-rw-rw-   0        0        0    38211 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_720p.xgb
+-rw-rw-rw-   0        0        0    36915 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_1080p.xgb
+-rw-rw-rw-   0        0        0    37851 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_1440p.xgb
+-rw-rw-rw-   0        0        0    37347 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_2160p.xgb
+-rw-rw-rw-   0        0        0    28779 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_360p.xgb
+-rw-rw-rw-   0        0        0    29715 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_480p.xgb
+-rw-rw-rw-   0        0        0    30219 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_720p.xgb
+-rw-rw-rw-   0        0        0    37779 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_1080p.xgb
+-rw-rw-rw-   0        0        0    38283 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_1440p.xgb
+-rw-rw-rw-   0        0        0    37563 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_2160p.xgb
+-rw-rw-rw-   0        0        0    27843 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_240p.xgb
+-rw-rw-rw-   0        0        0    27267 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_480p.xgb
+-rw-rw-rw-   0        0        0    27699 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_720p.xgb
+-rw-rw-rw-   0        0        0    37635 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_1080p.xgb
+-rw-rw-rw-   0        0        0    37275 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_1440p.xgb
+-rw-rw-rw-   0        0        0    37851 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_2160p.xgb
+-rw-rw-rw-   0        0        0    29283 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_240p.xgb
+-rw-rw-rw-   0        0        0    27483 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_360p.xgb
+-rw-rw-rw-   0        0        0    26979 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_720p.xgb
+-rw-rw-rw-   0        0        0    37347 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_1080p.xgb
+-rw-rw-rw-   0        0        0    38139 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_1440p.xgb
+-rw-rw-rw-   0        0        0    37779 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_2160p.xgb
+-rw-rw-rw-   0        0        0    29787 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_240p.xgb
+-rw-rw-rw-   0        0        0    27195 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_360p.xgb
+-rw-rw-rw-   0        0        0    27195 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_480p.xgb
+-rw-rw-rw-   0        0        0    17259 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_1440p.xgb
+-rw-rw-rw-   0        0        0    17835 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_2160p.xgb
+-rw-rw-rw-   0        0        0    27411 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_360p.xgb
+-rw-rw-rw-   0        0        0    25179 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_480p.xgb
+-rw-rw-rw-   0        0        0    22659 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_720p.xgb
+-rw-rw-rw-   0        0        0    17259 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_1080p.xgb
+-rw-rw-rw-   0        0        0    17187 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_2160p.xgb
+-rw-rw-rw-   0        0        0    25395 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_480p.xgb
+-rw-rw-rw-   0        0        0    23955 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_720p.xgb
+-rw-rw-rw-   0        0        0    19491 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_1080p.xgb
+-rw-rw-rw-   0        0        0    16827 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_1440p.xgb
+-rw-rw-rw-   0        0        0    23667 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_720p.xgb
+-rw-rw-rw-   0        0        0    19491 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_360p.xgb
+-rw-rw-rw-   0        0        0    20571 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_480p.xgb
+-rw-rw-rw-   0        0        0    22299 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_720p.xgb
+-rw-rw-rw-   0        0        0    22155 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_1080p.xgb
+-rw-rw-rw-   0        0        0    19059 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_240p.xgb
+-rw-rw-rw-   0        0        0    18987 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_480p.xgb
+-rw-rw-rw-   0        0        0    20571 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_720p.xgb
+-rw-rw-rw-   0        0        0    23163 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_1080p.xgb
+-rw-rw-rw-   0        0        0    22803 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_1440p.xgb
+-rw-rw-rw-   0        0        0    22011 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_240p.xgb
+-rw-rw-rw-   0        0        0    20283 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_360p.xgb
+-rw-rw-rw-   0        0        0    18123 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_720p.xgb
+-rw-rw-rw-   0        0        0    22947 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_1080p.xgb
+-rw-rw-rw-   0        0        0    22803 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_1440p.xgb
+-rw-rw-rw-   0        0        0    22587 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_2160p.xgb
+-rw-rw-rw-   0        0        0    23955 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_240p.xgb
+-rw-rw-rw-   0        0        0    21435 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_360p.xgb
+-rw-rw-rw-   0        0        0    18699 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_480p.xgb
+-rw-rw-rw-   0        0        0     4587 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Interlace_1080p_1440p.xgb
+-rw-rw-rw-   0        0        0     5739 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Interlace_240p_360p.xgb
+-rw-rw-rw-   0        0        0     6459 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Interlace_360p_240p.xgb
+-rw-rw-rw-   0        0        0     5307 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Interlace_360p_480p.xgb
+-rw-rw-rw-   0        0        0     5811 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Interlace_480p_360p.xgb
+-rw-rw-rw-   0        0        0     4947 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Interlace_480p_720p.xgb
+-rw-rw-rw-   0        0        0     5379 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Interlace_720p_1080p.xgb
+-rw-rw-rw-   0        0        0     5163 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Interlace_720p_480p.xgb
+-rw-rw-rw-   0        0        0    40443 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Noise_1080p_1440p.xgb
+-rw-rw-rw-   0        0        0    43467 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Noise_1080p_2160p.xgb
+-rw-rw-rw-   0        0        0    39435 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Noise_1440p_1080p.xgb
+-rw-rw-rw-   0        0        0    42171 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Noise_1440p_2160p.xgb
+-rw-rw-rw-   0        0        0    38787 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Noise_2160p_1440p.xgb
+-rw-rw-rw-   0        0        0    42747 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Noise_240p_360p.xgb
+-rw-rw-rw-   0        0        0    39939 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Noise_360p_240p.xgb
+-rw-rw-rw-   0        0        0    41235 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Noise_360p_480p.xgb
+-rw-rw-rw-   0        0        0    38931 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Noise_480p_360p.xgb
+-rw-rw-rw-   0        0        0    40875 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Noise_480p_720p.xgb
+-rw-rw-rw-   0        0        0    37923 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Noise_720p_480p.xgb
+drwxrwxrwx   0        0        0        0 2023-07-17 00:46:03.870504 agh_vqis-3.1.0/src/agh_vqis/models/ugc/
+-rw-rw-rw-   0        0        0   594166 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/ugc/12k_all_set.json
+drwxrwxrwx   0        0        0        0 2023-07-17 00:46:03.870504 agh_vqis-3.1.0/src/agh_vqis/utils/
+-rw-rw-rw-   0        0        0     6043 2023-07-17 00:34:17.000000 agh_vqis-3.1.0/src/agh_vqis/utils/helpers.py
+-rw-rw-rw-   0        0        0      754 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/utils/resolution_cast.py
+-rw-rw-rw-   0        0        0     5735 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/utils/ugc.py
```

### Comparing `agh_vqis-3.0.5/LICENSE` & `agh_vqis-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/agh_vqis.egg-info/SOURCES.txt` & `agh_vqis-3.1.0/agh_vqis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/python-cpbd/cpbd/compute.py` & `agh_vqis-3.1.0/python-cpbd/cpbd/compute.py`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/python-cpbd/cpbd/octave.py` & `agh_vqis-3.1.0/python-cpbd/cpbd/octave.py`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/setup.cfg` & `agh_vqis-3.1.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 6768 5f76 7169 730d 0a76 6572   = agh_vqis..ver
-00000020: 7369 6f6e 203d 2033 2e30 2e35 0d0a 6175  sion = 3.0.5..au
-00000030: 7468 6f72 203d 204a 616b 7562 204e 6177  thor = Jakub Naw
-00000040: 61c5 8261 2c20 4669 6c69 7020 4b6f 7275  a..a, Filip Koru
-00000050: 730d 0a61 7574 686f 725f 656d 6169 6c20  s..author_email 
-00000060: 3d20 6a61 6b75 622e 6e61 7761 6c61 4061  = jakub.nawala@a
-00000070: 6768 2e65 6475 2e70 6c2c 2066 6b6f 7275  gh.edu.pl, fkoru
-00000080: 7340 7374 7564 656e 742e 6167 682e 6564  s@student.agh.ed
+00000020: 7369 6f6e 203d 2033 2e31 2e30 0d0a 6175  sion = 3.1.0..au
+00000030: 7468 6f72 203d 2046 696c 6970 204b 6f72  thor = Filip Kor
+00000040: 7573 2c20 4a61 6b75 6220 4e61 7761 c582  us, Jakub Nawa..
+00000050: 610d 0a61 7574 686f 725f 656d 6169 6c20  a..author_email 
+00000060: 3d20 666b 6f72 7573 4073 7475 6465 6e74  = fkorus@student
+00000070: 2e61 6768 2e65 6475 2e70 6c2c 206a 616b  .agh.edu.pl, jak
+00000080: 7562 2e6e 6177 616c 6140 6167 682e 6564  ub.nawala@agh.ed
 00000090: 752e 706c 0d0a 6465 7363 7269 7074 696f  u.pl..descriptio
 000000a0: 6e20 3d20 4120 5079 7468 6f6e 2077 7261  n = A Python wra
 000000b0: 7070 6572 2066 6f72 2031 3820 696d 6167  pper for 18 imag
 000000c0: 6520 7175 616c 6974 7920 696e 6469 6361  e quality indica
 000000d0: 746f 7273 2e0d 0a6c 6f6e 675f 6465 7363  tors...long_desc
 000000e0: 7269 7074 696f 6e20 3d20 6669 6c65 3a20  ription = file: 
 000000f0: 5245 4144 4d45 2e6d 640d 0a6c 6f6e 675f  README.md..long_
@@ -69,16 +69,16 @@
 00000440: 6369 6b69 742d 696d 6167 653e 3d30 2e31  cikit-image>=0.1
 00000450: 392e 320d 0a09 736c 6963 6572 6174 6f72  9.2...slicerator
 00000460: 3e3d 312e 312e 300d 0a09 7363 656e 6564  >=1.1.0...scened
 00000470: 6574 6563 743e 3d30 2e36 2e30 2e33 0d0a  etect>=0.6.0.3..
 00000480: 096f 7065 6e63 762d 7079 7468 6f6e 3e3d  .opencv-python>=
 00000490: 342e 362e 302e 3636 0d0a 0978 6762 6f6f  4.6.0.66...xgboo
 000004a0: 7374 3d3d 312e 372e 350d 0a09 7363 696b  st==1.7.5...scik
-000004b0: 6974 2d6c 6561 726e 3d3d 312e 302e 320d  it-learn==1.0.2.
-000004c0: 0a09 6176 3e3d 382e 302e 330d 0a09 6666  ..av>=8.0.3...ff
+000004b0: 6974 2d6c 6561 726e 3d3d 312e 322e 300d  it-learn==1.2.0.
+000004c0: 0a09 6176 3e3d 392e 302e 300d 0a09 6666  ..av>=9.0.0...ff
 000004d0: 6d70 6567 2d70 7974 686f 6e3e 3d30 2e32  mpeg-python>=0.2
 000004e0: 2e30 0d0a 0d0a 5b6f 7074 696f 6e73 2e70  .0....[options.p
 000004f0: 6163 6b61 6765 5f64 6174 615d 0d0a 2a20  ackage_data]..* 
 00000500: 3d20 2a0d 0a0d 0a5b 6567 675f 696e 666f  = *....[egg_info
 00000510: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
 00000520: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
 00000530: 0a                                       .
```

### Comparing `agh_vqis-3.0.5/src/agh_vqis/__main__.py` & `agh_vqis-3.1.0/src/agh_vqis/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -323,14 +323,18 @@
 
     if options is None:
         options = {}
 
     if args is None:
         args = parse_user_input(cli)
 
+    if not is_ffmpeg_installed():
+        logger.error(f'ffmpeg is not installed or an executable command')
+        return -1
+
     if not in_path.exists():
         logger.error(f'{str(in_path)} file does not exists')
         return -1
 
     mm_file_ext = in_path.suffix
     if mm_file_ext not in allowed_mm_file_extensions:
         logger.error(f'{mm_file_ext} file extension is not supported')
@@ -472,15 +476,15 @@
 
 def main():
     # TODO Implement user input processing interface that allows to choose individual VQIs from the 15 AGH VQIs in a
     #  user-friendly manner
     args = parse_user_input(True)
 
     in_path = args.path
-    in_path = in_path.absolute()
+    in_path = in_path.resolve()
     if not in_path.exists():
         raise FileNotFoundError(f"The path you specified ({in_path}) does not exist. Exiting.")
 
     if in_path.is_dir():
         logger.info(f"Processing a folder ({str(in_path)}) potentially containing a set of multimedia materials")
         status = process_folder_w_mm_files(in_path, cli=True, options={}, args=args)
     else:
```

### Comparing `agh_vqis-3.0.5/src/agh_vqis/_logger.py` & `agh_vqis-3.1.0/src/agh_vqis/_logger.py`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/binaries/agh_vqis_binary_macosx_mt` & `agh_vqis-3.1.0/src/agh_vqis/binaries/agh_vqis_binary_macosx_mt`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/binaries/agh_vqis_binary_win64_mt.exe` & `agh_vqis-3.1.0/src/agh_vqis/binaries/agh_vqis_binary_win64_mt.exe`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/binaries/agh_vqis_binary_x86_mt` & `agh_vqis-3.1.0/src/agh_vqis/binaries/agh_vqis_binary_x86_mt`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/binaries/cygwin1.dll` & `agh_vqis-3.1.0/src/agh_vqis/binaries/cygwin1.dll`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Blockiness_1080p_1440p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blockiness_1080p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Blockiness_1080p_2160p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blockiness_1080p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Blockiness_1440p_2160p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blockiness_1440p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Blockiness_2160p_1440p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blockiness_2160p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Blur_1080p_1440p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_1080p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Blur_1080p_2160p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_1080p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Blur_1440p_1080p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_1440p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Blur_1440p_2160p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_1440p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Blur_2160p_1080p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_2160p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Blur_2160p_1440p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_2160p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Blur_240p_360p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_240p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Blur_240p_480p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_240p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Blur_360p_240p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_360p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Blur_360p_480p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_360p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Blur_360p_720p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_360p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Blur_480p_240p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_480p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Blur_480p_360p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_480p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Blur_480p_720p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_480p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Blur_720p_1080p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_720p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Blur_720p_360p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_720p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Blur_720p_480p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_720p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_1440p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_2160p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_240p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_360p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_480p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_720p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_1080p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_2160p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_240p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_360p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_480p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_720p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_1080p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_1440p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_240p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_360p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_480p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_720p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_240p_1080p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_240p_1440p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_240p_2160p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_240p_360p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_240p_480p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_240p_720p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_360p_1080p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_360p_1440p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_360p_2160p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_360p_240p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_360p_480p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_360p_720p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_480p_1080p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_480p_1440p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_480p_2160p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_480p_240p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_480p_360p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_480p_720p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_720p_1080p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_720p_1440p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_720p_2160p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_720p_240p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_720p_360p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Contrast_720p_480p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_1440p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_2160p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_360p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_480p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_720p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_1080p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_2160p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_480p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_720p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_1080p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_1440p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_720p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_360p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_480p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_720p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_1080p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_240p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_480p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_720p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_1080p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_1440p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_240p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_360p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_720p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_1080p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_1440p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_2160p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_240p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_360p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_480p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Interlace_1080p_1440p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Interlace_1080p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Interlace_240p_360p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Interlace_240p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Interlace_360p_240p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Interlace_360p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Interlace_360p_480p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Interlace_360p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Interlace_480p_360p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Interlace_480p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Interlace_480p_720p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Interlace_480p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Interlace_720p_1080p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Interlace_720p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Interlace_720p_480p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Interlace_720p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Noise_1080p_1440p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Noise_1080p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Noise_1080p_2160p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Noise_1080p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Noise_1440p_1080p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Noise_1440p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Noise_1440p_2160p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Noise_1440p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Noise_2160p_1440p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Noise_2160p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Noise_240p_360p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Noise_240p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Noise_360p_240p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Noise_360p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Noise_360p_480p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Noise_360p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Noise_480p_360p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Noise_480p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Noise_480p_720p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Noise_480p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/resolution_cast/model_Noise_720p_480p.xgb` & `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Noise_720p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/models/ugc/12k_all_set.json` & `agh_vqis-3.1.0/src/agh_vqis/models/ugc/12k_all_set.json`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/utils/helpers.py` & `agh_vqis-3.1.0/src/agh_vqis/utils/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import platform
 import ffmpeg
 import os
 import shutil
 import uuid
 from pathlib import Path
 from enum import Enum
-from subprocess import PIPE, STDOUT, Popen
+from subprocess import PIPE, STDOUT, Popen, run, CalledProcessError
 
 
 class VQIs:
     blockiness = 'blockiness'
     SA = 'SA'
     letterbox = 'letterbox'
     pillarbox = 'pillarbox'
@@ -191,9 +191,25 @@
             logger.error(f"{str(sfs_call_elems[0])}\'s output: {sfs_stdout.decode('ascii')}")
         return -1
 
     if logger is not None:
         logger.debug(f"{sfs_call_elems[0]} was successfully executed")
 
 
+def is_ffmpeg_installed():
+    try:
+        # Check if 'ffmpeg' can be run as a command without raising an exception
+        run(['ffmpeg', '-version'], stdout=PIPE, stderr=PIPE, text=True)
+        return True
+    except FileNotFoundError:
+        # The 'ffmpeg' command was not found
+        return False
+    except CalledProcessError:
+        # 'ffmpeg' is installed but returned a non-zero exit code (possible on Linux)
+        return True
+    except Exception as e:
+        # Other exceptions might occur
+        return False
+
+
 def generate_uuid():
     return str(uuid.uuid4())
```

### Comparing `agh_vqis-3.0.5/src/agh_vqis/utils/resolution_cast.py` & `agh_vqis-3.1.0/src/agh_vqis/utils/resolution_cast.py`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.5/src/agh_vqis/utils/ugc.py` & `agh_vqis-3.1.0/src/agh_vqis/utils/ugc.py`

 * *Files identical despite different names*

