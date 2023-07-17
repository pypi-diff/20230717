# Comparing `tmp/genomap-1.2.1.tar.gz` & `tmp/genomap-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genomap-1.2.1.tar", last modified: Mon Jul 17 19:40:42 2023, max compression
+gzip compressed data, was "genomap-1.2.2.tar", last modified: Mon Jul 17 21:16:35 2023, max compression
```

## Comparing `genomap-1.2.1.tar` & `genomap-1.2.2.tar`

### file list

```diff
@@ -1,64 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:40:42.473471 genomap-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-07-17 19:35:42.000000 genomap-1.2.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-17 19:35:42.000000 genomap-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10426 2023-07-17 19:40:42.473471 genomap-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9992 2023-07-17 19:35:43.000000 genomap-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:40:42.445471 genomap-1.2.1/data/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-17 19:35:43.000000 genomap-1.2.1/data/TM_data.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:40:42.449471 genomap-1.2.1/genomap/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:40:42.449471 genomap-1.2.1/genomap/bregman_genomap/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/bregman_genomap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   125058 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/bregman_genomap/bregman_genomap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:40:42.453471 genomap-1.2.1/genomap/genoClassification/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/genoClassification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/genoClassification/genoClassification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:40:42.457471 genomap-1.2.1/genomap/genoDR/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/genoDR/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/genoDR/genoDimReduction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:40:42.457471 genomap-1.2.1/genomap/genoMOI/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/genoMOI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/genoMOI/genoMOI.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:40:42.457471 genomap-1.2.1/genomap/genoNetRegression/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/genoNetRegression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/genoNetRegression/genoNet_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:40:42.461471 genomap-1.2.1/genomap/genoRegression/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/genoRegression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/genoRegression/genoRegression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:40:42.461471 genomap-1.2.1/genomap/genoSig/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/genoSig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/genoSig/genoSig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:40:42.461471 genomap-1.2.1/genomap/genoTraj/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/genoTraj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/genoTraj/genoTraj.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:40:42.465471 genomap-1.2.1/genomap/genoVis/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/genoVis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/genoVis/genoVis.py
--rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/genomap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:40:42.465471 genomap-1.2.1/genomap/genomapOPT/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/genomapOPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/genomapOPT/genomapOPT.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:40:42.465471 genomap-1.2.1/genomap/genomapT/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/genomapT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/genomapT/genomapT.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:40:42.473471 genomap-1.2.1/genomap/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/utils/ConvDEC.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/utils/ConvIDEC.py
--rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/utils/FcDEC.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/utils/FcIDEC.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/utils/class_discriminative_opt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/utils/gTraj_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/utils/group_centroid_opt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/utils/util_Sig.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-17 19:35:43.000000 genomap-1.2.1/genomap/utils/utils_MOI.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:40:42.449471 genomap-1.2.1/genomap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10426 2023-07-17 19:40:42.000000 genomap-1.2.1/genomap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-17 19:40:42.000000 genomap-1.2.1/genomap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 19:40:42.000000 genomap-1.2.1/genomap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-17 19:40:42.000000 genomap-1.2.1/genomap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 19:40:42.000000 genomap-1.2.1/genomap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-17 19:35:43.000000 genomap-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 19:40:42.473471 genomap-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-17 19:35:43.000000 genomap-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:16:35.397071 genomap-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-07-17 21:12:42.000000 genomap-1.2.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-17 21:12:42.000000 genomap-1.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11484 2023-07-17 21:16:35.397071 genomap-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11050 2023-07-17 21:12:43.000000 genomap-1.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:16:35.385071 genomap-1.2.2/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-17 21:12:43.000000 genomap-1.2.2/data/TM_data.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:16:35.385071 genomap-1.2.2/genomap/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:16:35.385071 genomap-1.2.2/genomap/bregman_genomap/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/bregman_genomap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   125058 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/bregman_genomap/bregman_genomap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:16:35.385071 genomap-1.2.2/genomap/genoClassification/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/genoClassification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/genoClassification/genoClassification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:16:35.389071 genomap-1.2.2/genomap/genoDR/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/genoDR/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/genoDR/genoDimReduction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:16:35.389071 genomap-1.2.2/genomap/genoMOI/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/genoMOI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/genoMOI/genoMOI.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:16:35.389071 genomap-1.2.2/genomap/genoNetRegression/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/genoNetRegression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/genoNetRegression/genoNet_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:16:35.389071 genomap-1.2.2/genomap/genoRegression/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/genoRegression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/genoRegression/genoRegression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:16:35.389071 genomap-1.2.2/genomap/genoSig/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/genoSig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/genoSig/genoSig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:16:35.389071 genomap-1.2.2/genomap/genoTraj/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/genoTraj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/genoTraj/genoTraj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:16:35.389071 genomap-1.2.2/genomap/genoVis/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/genoVis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/genoVis/genoVis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/genomap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:16:35.393071 genomap-1.2.2/genomap/genomapOPT/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/genomapOPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/genomapOPT/genomapOPT.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:16:35.393071 genomap-1.2.2/genomap/genomapT/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/genomapT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/genomapT/genomapT.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:16:35.397071 genomap-1.2.2/genomap/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/utils/ConvDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/utils/ConvIDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/utils/FcDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/utils/FcIDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/utils/class_discriminative_opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/utils/gTraj_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/utils/group_centroid_opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/utils/util_Sig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/utils/util_genoClassReg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/utils/utils_MOI.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:16:35.385071 genomap-1.2.2/genomap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11484 2023-07-17 21:16:35.000000 genomap-1.2.2/genomap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-17 21:16:35.000000 genomap-1.2.2/genomap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 21:16:35.000000 genomap-1.2.2/genomap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-17 21:16:35.000000 genomap-1.2.2/genomap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 21:16:35.000000 genomap-1.2.2/genomap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-17 21:12:43.000000 genomap-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 21:16:35.397071 genomap-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-17 21:12:43.000000 genomap-1.2.2/setup.py
```

### Comparing `genomap-1.2.1/LICENSE.txt` & `genomap-1.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `genomap-1.2.1/PKG-INFO` & `genomap-1.2.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genomap
-Version: 1.2.1
+Version: 1.2.2
 Summary: Genomap converts tabular gene expression data into spatially meaningful images.
 Home-page: https://github.com/xinglab-ai/genomap
 Author: Md Tauhidul Islam
 Author-email: tauhid@stanford.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -33,195 +33,239 @@
 ## Example codes
 
 ### Example 1 - Construct a genomap
 
 ```python
 import pandas as pd # Please install pandas and matplotlib before you run this example
 import matplotlib.pyplot as plt
+import numpy as np
 import scipy
-import genomap as gp
+from genomap import construct_genomap
 
-data = pd.read_csv('TM_data.csv', header=None, delim_whitespace=False)
-colNum=31 # Column number of genomap
-rowNum=31 # Row number of genomap
+data = pd.read_csv('TM_data.csv', header=None,
+                   delim_whitespace=False)
+colNum=33 # Column number of genomap
+rowNum=33 # Row number of genomap
 
 dataNorm=scipy.stats.zscore(data,axis=0,ddof=1) # Normalization of the data
 
-genoMaps=gp.construct_genomap(dataNorm,rowNum,colNum) # Construction of genomaps
+genoMaps=construct_genomap(dataNorm,rowNum,colNum,epsilon=0.0,num_iter=200) # Construction of genomaps
 
-findI=genoMaps[0,:,:,:]
+findI=genoMaps[10,:,:,:]
 
 plt.figure(1) # Plot the first genomap
-plt.imshow(findI, origin = 'lower', extent = [0, 10, 0, 10], aspect = 1)
+plt.imshow(findI, origin = 'lower',  extent = [0, 10, 0, 10], aspect = 1)
 plt.title('Genomap of a cell from TM dataset')
+plt.show()
 ```
 
 ### Example 2 - Try genoVis for data visualization and clustering
 
 ```python
 import scipy.io as sio
 import numpy as np
-import metrics
-from genomap.genoVis import compute_genoVis
-from genomap.genoTraj import compute_genoTraj
-from genomap.genoMOI import compute_genoMOI
+import pandas as pd
+from genomap.genoVis import genoVis
+import matplotlib.pyplot as plt
+from sklearn.cluster import KMeans
+from sklearn.decomposition import PCA
+import phate
+import umap
 
 data = pd.read_csv('TM_data.csv', header=None,
                    delim_whitespace=False)
 data=data.values
 gt_data = sio.loadmat('GT_TM.mat')
 y = np.squeeze(gt_data['GT'])
 n_clusters = len(np.unique(y))
 
-resVis=compute_genoVis(data,n_clusters=n_clusters, colNum=33,rowNum=33)
-# Use resVis=compute_genoVis(data, colNum=32,rowNum=32), if you do not know the number
+
+resVis=genoVis(data,n_clusters=n_clusters, colNum=33,rowNum=33)
+# Use resVis=compute_genoVis(data, colNum=32,rowNum=32), if you dont know the number
 # of classes in the data
 
 resVisEmb=resVis[0] # Dimensionality reduction and visualization result
 clusIndex=resVis[1] # Clustering result
 
 plt.figure(figsize=(15, 10))
 plt.rcParams.update({'font.size': 28})    
-h1=plt.scatter(resVisEmb[:, 0], resVisEmb[:, 1], c=y,cmap='jet', marker='o', s=18)     
+h1=plt.scatter(resVisEmb[:, 0], resVisEmb[:, 1], c=y,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
 plt.xlabel('genoVis1')
 plt.ylabel('genoVis2')
 plt.tight_layout()
 plt.colorbar(h1)
 
-# Print clustering accuracy metrics
+import genomap.utils.metrics as metrics
 print('acc=%.4f, nmi=%.4f, ari=%.4f' % (metrics.acc(y, clusIndex), metrics.nmi(y, clusIndex), metrics.ari(y, clusIndex)))
 ```
 
 ### Example 3 - Try genoDR for dimensionality reduction
 
 ```python
 import scipy.io as sio
 import numpy as np
-from genoDimReduction import compute_genoDimReduction
+from genomap.genoDR import genoDR
 import matplotlib.pyplot as plt
 import umap
 
-dx = sio.loadmat('../data/reducedData_divseq.mat')
+dx = sio.loadmat('reducedData_divseq.mat')
 data=dx['X']
-gt_data = sio.loadmat('../data/GT_divseq.mat')
+gt_data = sio.loadmat('GT_divseq.mat')
 y = np.squeeze(gt_data['GT'])
 n_clusters = len(np.unique(y))
 
-resDR=compute_genoDimReduction(data,n_clusters=n_clusters, colNum=33,rowNum=33)
+resDR=genoDR(data,n_clusters=n_clusters, colNum=33,rowNum=33)
 #resDR=compute_genoDimReduction(data, colNum=33,rowNum=33) # if you dont know the number
 # of classes in the data
 embedding2D = umap.UMAP(n_neighbors=30,min_dist=0.3,n_epochs=200).fit_transform(resDR)
 
 plt.figure(figsize=(15, 10))
 plt.rcParams.update({'font.size': 28})    
 h1=plt.scatter(embedding2D[:, 0], embedding2D[:, 1], c=y,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
 plt.xlabel('genoVis1')
 plt.ylabel('genoVis2')
 plt.tight_layout()
 plt.colorbar(h1)
+plt.show()
 ```
 
 ### Example 4 - Try genoTraj for cell trajectory analysis
 
 ```python
+import scipy.io as sio
+import numpy as np
+import pandas as pd
+import matplotlib.pyplot as plt
+from sklearn.cluster import KMeans
+from sklearn.decomposition import PCA
+import phate
+import umap
+from genomap.genoTraj import genoTraj
+
 # Load data
 dx = sio.loadmat('organoidData.mat')
 data=dx['X3']
 gt_data = sio.loadmat('cellsPsudo.mat')
 Y_time = np.squeeze(gt_data['newGT'])
 
 # Apply genoTraj for embedding showing cell trajectories
-outGenoTraj=compute_genoTraj(data)
+outGenoTraj=genoTraj(data)
 
 plt.figure(figsize=(15, 10))
 plt.rcParams.update({'font.size': 28})    
 h1=plt.scatter(outGenoTraj[:, 0], outGenoTraj[:, 1], c=Y_time,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
 plt.xlabel('genoTraj1')
 plt.ylabel('genoTraj2')
 plt.tight_layout()
 plt.colorbar(h1)
+plt.show()
 
+# Comparison with PHATE
+pca = PCA(n_components=100)
+resPCA=pca.fit_transform(data)
+
+phate_op = phate.PHATE()
+res_phate = phate_op.fit_transform(resPCA)
+    
+    
+plt.figure(figsize=(15, 10))
+plt.rcParams.update({'font.size': 28})    
+h1=plt.scatter(res_phate[:, 0], res_phate[:, 1], c=Y_time,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
+plt.xlabel('PHATE1')
+plt.ylabel('PHATE2')
+plt.tight_layout()
+plt.colorbar(h1)
+plt.show()
 ```
 
 ### Example 5 - Try genoMOI for multi-omic data integration
 
 ```python
+import scanpy as sc
+import matplotlib.pyplot as plt
+from genomap.genoMOI import genoMOI
+import scipy.io as sio
+import numpy as np
+import pandas as pd
+import umap
+
 
-# Load datasets
+# Load five different pancreatic datasets
 dx = sio.loadmat('dataBaronX.mat')
 data=dx['dataBaron']
 dx = sio.loadmat('dataMuraroX.mat')
 data2=dx['dataMuraro']
 dx = sio.loadmat('dataScapleX.mat')
 data3=dx['dataScaple']
 dx = sio.loadmat('dataWangX.mat')
 data4=dx['dataWang']
 dx = sio.loadmat('dataXinX.mat')
 data5=dx['dataXin']
+
 # Load class and batch labels
 dx = sio.loadmat('classLabel.mat')
 y = np.squeeze(dx['classLabel'])
 dx = sio.loadmat('batchLabel.mat')
 ybatch = np.squeeze(dx['batchLabel'])
 
 # Apply genoMOI
-resVis=compute_genoMOI(data, data2, data3, data4, data5, colNum=44, rowNum=44)
+resVis=genoMOI(data, data2, data3, data4, data5, colNum=44, rowNum=44)
 
 # Visualize the integrated data using UMAP
-embedding = umap.UMAP(n_neighbors=30,min_dist=0.3,n_epochs=200).fit_transform(resVis) 
+embedding = umap.UMAP(n_neighbors=30,min_dist=0.3,n_epochs=200).fit_transform(resVis)
 
 plt.figure(figsize=(15, 10))
 plt.rcParams.update({'font.size': 28})    
-h1=plt.scatter(embedding[:, 0], embedding[:, 1], c=y,cmap='jet', marker='o', s=18)     
-plt.xlabel('UMAP')
-plt.ylabel('UMAP2')
+h1=plt.scatter(embedding[:, 0], embedding[:, 1], c=y,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
+plt.xlabel('genoVis1')
+plt.ylabel('genoVis2')
 plt.tight_layout()
 plt.colorbar(h1)
+plt.show()
 ```
 
 ### Example 6 - Try genoSig for finding gene signatures for cell/data classes
 
 ```python
 import numpy as np
 import scipy.io as sio
-from util_Sig import createGenomap_for_sig
+from genomap.utils.util_Sig import createGenomap_for_sig
 import pandas as pd
-from compute_genoSig import genoSig
+from genomap.genoSig import genoSig
 
 # Load data
-dx = sio.loadmat('../data/reducedData_divseq.mat')
+dx = sio.loadmat('reducedData_divseq.mat')
 data=dx['X']
 # Load data labels
-label = pd.read_csv('../data/groundTruth_divseq.csv',header=None)
+label = pd.read_csv('groundTruth_divseq.csv',header=None)
 # Load gene names corresponding to the columns of the data
 gene_names = ['Gene_' + str(i) for i in range(1, data.shape[1]+1)]
 gene_names=np.array(gene_names)
 
 # The cell classes for which gene signatures will be computed
 userPD = np.array(['DG'])
 
 colNum=32 # genomap column number
 rowNum=32 # genomap row number
 # Create genomaps
 genoMaps,gene_namesRe,T=createGenomap_for_sig(data,gene_names,rowNum,colNum)
 # compute the gene signatures
 result=genoSig(genoMaps,T,label,userPD,gene_namesRe, epochs=50)
 
-print(result.head())  
+print(result.head())
 ```
 
 ### Example 7 - Try genoClassification for tabular data classification
 
 ```python
 import pandas as pd
 import numpy as np
 import scipy.io as sio
-from genoClassification import genoClassification
-from util_genoClassReg import select_random_values
-
+from genomap.genoClassification import genoClassification
+from genomap.utils.util_genoClassReg import select_random_values
 
 # First, we load the TM data. Data should be in cells X genes format, 
 data = pd.read_csv('TM_data.csv', header=None,
                    delim_whitespace=False)
 
 # Creation of genomaps
 # Selection of row and column number of the genomaps 
@@ -230,15 +274,15 @@
 rowNum=33
 
 # Load ground truth cell labels of the TM dataset
 gt_data = sio.loadmat('GT_TM.mat')
 GT = np.squeeze(gt_data['GT'])
 GT=GT-1 # to ensure the labels begin with 0 to conform with PyTorch
 
-# Select 80% of data randomly for training and others for testing
+# Select 80% data randomly for training and others for testing
 indxTrain, indxTest= select_random_values(start=0, end=GT.shape[0], perc=0.8)
 groundTruthTest = GT[indxTest-1]
 
 training_data=data.values[indxTrain-1]
 training_labels=GT[indxTrain-1]
 test_data=data.values[indxTest-1]
 
@@ -250,38 +294,38 @@
 
 ### Example 8 - Try genoRegression for tabular data regression
 
 ```python
 import pandas as pd
 import numpy as np
 import scipy.io as sio
-from genoRegression import genoRegression
+from genomap.genoRegression import genoRegression
 from sklearn.metrics import mean_squared_error
-from util_genoClassReg import select_random_values
+from genomap.utils.util_genoClassReg import select_random_values
 
 # Load data and labels
-dx = sio.loadmat('../data/organoidData.mat')
+dx = sio.loadmat('organoidData.mat')
 data=dx['X3']
-gt_data = sio.loadmat('../data/GT_Org.mat')
+gt_data = sio.loadmat('GT_Org.mat')
 Y_time = np.squeeze(gt_data['GT'])
 Y_time = Y_time - 1 # to ensure the labels begin with 0 to conform with PyTorch
 
-# Select 80% of data randomly for training and others for testing
+# Select 80% data randomly for training and others for testing
 indxTrain, indxTest= select_random_values(start=0, end=Y_time.shape[0], perc=0.8)
 groundTruthTest = Y_time[indxTest-1]
 training_data=data[indxTrain-1]
 training_labels=Y_time[indxTrain-1]
 test_data=data[indxTest-1]
 
 # Run genoRegression
 est=genoRegression(training_data, training_labels, test_data, rowNum=40, colNum=40, epoch=200)
 
 # Calculate MSE
 mse = mean_squared_error(groundTruthTest, est)
-print(f'MSE: {mse}') 
+print(f'MSE: {mse}')
 ```
 
 # Citation
 
 If you use the genomap code, please cite our Nature Communications paper: https://www.nature.com/articles/s41467-023-36383-6
 
 Islam, M.T., Xing, L. Cartography of Genomic Interactions Enables Deep Analysis of Single-Cell Expression Data. Nat Commun 14, 679 (2023). https://doi.org/10.1038/s41467-023-36383-6
```

### Comparing `genomap-1.2.1/README.md` & `genomap-1.2.2/genomap.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: genomap
+Version: 1.2.2
+Summary: Genomap converts tabular gene expression data into spatially meaningful images.
+Home-page: https://github.com/xinglab-ai/genomap
+Author: Md Tauhidul Islam
+Author-email: tauhid@stanford.edu
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # Genomap creates images from gene expression data and offers high-performance dimensionality reduction and visualization, data clustering, classification and regression, gene signature extraction, multi-omics data integration, and trajectory analysis 
 
 Genomap is an entropy-based cartography strategy to contrive the high dimensional gene expression data into a configured image format with explicit integration of the genomic interactions. This unique cartography casts the gene-gene interactions into a spatial configuration and enables us to extract the deep genomic interaction features and discover underlying discriminative patterns of the data. For a wide variety of applications (cell clustering and recognition, gene signature extraction, single-cell data integration, cellular trajectory analysis, dimensionality reduction, and visualization), genomap drastically improves the accuracy of data analyses as compared to state-of-the-art techniques.
 
 ## How to use genomap
 
 The easiest way to start with genomap is to install it from pypi using 
@@ -20,195 +33,239 @@
 ## Example codes
 
 ### Example 1 - Construct a genomap
 
 ```python
 import pandas as pd # Please install pandas and matplotlib before you run this example
 import matplotlib.pyplot as plt
+import numpy as np
 import scipy
-import genomap as gp
+from genomap import construct_genomap
 
-data = pd.read_csv('TM_data.csv', header=None, delim_whitespace=False)
-colNum=31 # Column number of genomap
-rowNum=31 # Row number of genomap
+data = pd.read_csv('TM_data.csv', header=None,
+                   delim_whitespace=False)
+colNum=33 # Column number of genomap
+rowNum=33 # Row number of genomap
 
 dataNorm=scipy.stats.zscore(data,axis=0,ddof=1) # Normalization of the data
 
-genoMaps=gp.construct_genomap(dataNorm,rowNum,colNum) # Construction of genomaps
+genoMaps=construct_genomap(dataNorm,rowNum,colNum,epsilon=0.0,num_iter=200) # Construction of genomaps
 
-findI=genoMaps[0,:,:,:]
+findI=genoMaps[10,:,:,:]
 
 plt.figure(1) # Plot the first genomap
-plt.imshow(findI, origin = 'lower', extent = [0, 10, 0, 10], aspect = 1)
+plt.imshow(findI, origin = 'lower',  extent = [0, 10, 0, 10], aspect = 1)
 plt.title('Genomap of a cell from TM dataset')
+plt.show()
 ```
 
 ### Example 2 - Try genoVis for data visualization and clustering
 
 ```python
 import scipy.io as sio
 import numpy as np
-import metrics
-from genomap.genoVis import compute_genoVis
-from genomap.genoTraj import compute_genoTraj
-from genomap.genoMOI import compute_genoMOI
+import pandas as pd
+from genomap.genoVis import genoVis
+import matplotlib.pyplot as plt
+from sklearn.cluster import KMeans
+from sklearn.decomposition import PCA
+import phate
+import umap
 
 data = pd.read_csv('TM_data.csv', header=None,
                    delim_whitespace=False)
 data=data.values
 gt_data = sio.loadmat('GT_TM.mat')
 y = np.squeeze(gt_data['GT'])
 n_clusters = len(np.unique(y))
 
-resVis=compute_genoVis(data,n_clusters=n_clusters, colNum=33,rowNum=33)
-# Use resVis=compute_genoVis(data, colNum=32,rowNum=32), if you do not know the number
+
+resVis=genoVis(data,n_clusters=n_clusters, colNum=33,rowNum=33)
+# Use resVis=compute_genoVis(data, colNum=32,rowNum=32), if you dont know the number
 # of classes in the data
 
 resVisEmb=resVis[0] # Dimensionality reduction and visualization result
 clusIndex=resVis[1] # Clustering result
 
 plt.figure(figsize=(15, 10))
 plt.rcParams.update({'font.size': 28})    
-h1=plt.scatter(resVisEmb[:, 0], resVisEmb[:, 1], c=y,cmap='jet', marker='o', s=18)     
+h1=plt.scatter(resVisEmb[:, 0], resVisEmb[:, 1], c=y,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
 plt.xlabel('genoVis1')
 plt.ylabel('genoVis2')
 plt.tight_layout()
 plt.colorbar(h1)
 
-# Print clustering accuracy metrics
+import genomap.utils.metrics as metrics
 print('acc=%.4f, nmi=%.4f, ari=%.4f' % (metrics.acc(y, clusIndex), metrics.nmi(y, clusIndex), metrics.ari(y, clusIndex)))
 ```
 
 ### Example 3 - Try genoDR for dimensionality reduction
 
 ```python
 import scipy.io as sio
 import numpy as np
-from genoDimReduction import compute_genoDimReduction
+from genomap.genoDR import genoDR
 import matplotlib.pyplot as plt
 import umap
 
-dx = sio.loadmat('../data/reducedData_divseq.mat')
+dx = sio.loadmat('reducedData_divseq.mat')
 data=dx['X']
-gt_data = sio.loadmat('../data/GT_divseq.mat')
+gt_data = sio.loadmat('GT_divseq.mat')
 y = np.squeeze(gt_data['GT'])
 n_clusters = len(np.unique(y))
 
-resDR=compute_genoDimReduction(data,n_clusters=n_clusters, colNum=33,rowNum=33)
+resDR=genoDR(data,n_clusters=n_clusters, colNum=33,rowNum=33)
 #resDR=compute_genoDimReduction(data, colNum=33,rowNum=33) # if you dont know the number
 # of classes in the data
 embedding2D = umap.UMAP(n_neighbors=30,min_dist=0.3,n_epochs=200).fit_transform(resDR)
 
 plt.figure(figsize=(15, 10))
 plt.rcParams.update({'font.size': 28})    
 h1=plt.scatter(embedding2D[:, 0], embedding2D[:, 1], c=y,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
 plt.xlabel('genoVis1')
 plt.ylabel('genoVis2')
 plt.tight_layout()
 plt.colorbar(h1)
+plt.show()
 ```
 
 ### Example 4 - Try genoTraj for cell trajectory analysis
 
 ```python
+import scipy.io as sio
+import numpy as np
+import pandas as pd
+import matplotlib.pyplot as plt
+from sklearn.cluster import KMeans
+from sklearn.decomposition import PCA
+import phate
+import umap
+from genomap.genoTraj import genoTraj
+
 # Load data
 dx = sio.loadmat('organoidData.mat')
 data=dx['X3']
 gt_data = sio.loadmat('cellsPsudo.mat')
 Y_time = np.squeeze(gt_data['newGT'])
 
 # Apply genoTraj for embedding showing cell trajectories
-outGenoTraj=compute_genoTraj(data)
+outGenoTraj=genoTraj(data)
 
 plt.figure(figsize=(15, 10))
 plt.rcParams.update({'font.size': 28})    
 h1=plt.scatter(outGenoTraj[:, 0], outGenoTraj[:, 1], c=Y_time,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
 plt.xlabel('genoTraj1')
 plt.ylabel('genoTraj2')
 plt.tight_layout()
 plt.colorbar(h1)
+plt.show()
 
+# Comparison with PHATE
+pca = PCA(n_components=100)
+resPCA=pca.fit_transform(data)
+
+phate_op = phate.PHATE()
+res_phate = phate_op.fit_transform(resPCA)
+    
+    
+plt.figure(figsize=(15, 10))
+plt.rcParams.update({'font.size': 28})    
+h1=plt.scatter(res_phate[:, 0], res_phate[:, 1], c=Y_time,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
+plt.xlabel('PHATE1')
+plt.ylabel('PHATE2')
+plt.tight_layout()
+plt.colorbar(h1)
+plt.show()
 ```
 
 ### Example 5 - Try genoMOI for multi-omic data integration
 
 ```python
+import scanpy as sc
+import matplotlib.pyplot as plt
+from genomap.genoMOI import genoMOI
+import scipy.io as sio
+import numpy as np
+import pandas as pd
+import umap
+
 
-# Load datasets
+# Load five different pancreatic datasets
 dx = sio.loadmat('dataBaronX.mat')
 data=dx['dataBaron']
 dx = sio.loadmat('dataMuraroX.mat')
 data2=dx['dataMuraro']
 dx = sio.loadmat('dataScapleX.mat')
 data3=dx['dataScaple']
 dx = sio.loadmat('dataWangX.mat')
 data4=dx['dataWang']
 dx = sio.loadmat('dataXinX.mat')
 data5=dx['dataXin']
+
 # Load class and batch labels
 dx = sio.loadmat('classLabel.mat')
 y = np.squeeze(dx['classLabel'])
 dx = sio.loadmat('batchLabel.mat')
 ybatch = np.squeeze(dx['batchLabel'])
 
 # Apply genoMOI
-resVis=compute_genoMOI(data, data2, data3, data4, data5, colNum=44, rowNum=44)
+resVis=genoMOI(data, data2, data3, data4, data5, colNum=44, rowNum=44)
 
 # Visualize the integrated data using UMAP
-embedding = umap.UMAP(n_neighbors=30,min_dist=0.3,n_epochs=200).fit_transform(resVis) 
+embedding = umap.UMAP(n_neighbors=30,min_dist=0.3,n_epochs=200).fit_transform(resVis)
 
 plt.figure(figsize=(15, 10))
 plt.rcParams.update({'font.size': 28})    
-h1=plt.scatter(embedding[:, 0], embedding[:, 1], c=y,cmap='jet', marker='o', s=18)     
-plt.xlabel('UMAP')
-plt.ylabel('UMAP2')
+h1=plt.scatter(embedding[:, 0], embedding[:, 1], c=y,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
+plt.xlabel('genoVis1')
+plt.ylabel('genoVis2')
 plt.tight_layout()
 plt.colorbar(h1)
+plt.show()
 ```
 
 ### Example 6 - Try genoSig for finding gene signatures for cell/data classes
 
 ```python
 import numpy as np
 import scipy.io as sio
-from util_Sig import createGenomap_for_sig
+from genomap.utils.util_Sig import createGenomap_for_sig
 import pandas as pd
-from compute_genoSig import genoSig
+from genomap.genoSig import genoSig
 
 # Load data
-dx = sio.loadmat('../data/reducedData_divseq.mat')
+dx = sio.loadmat('reducedData_divseq.mat')
 data=dx['X']
 # Load data labels
-label = pd.read_csv('../data/groundTruth_divseq.csv',header=None)
+label = pd.read_csv('groundTruth_divseq.csv',header=None)
 # Load gene names corresponding to the columns of the data
 gene_names = ['Gene_' + str(i) for i in range(1, data.shape[1]+1)]
 gene_names=np.array(gene_names)
 
 # The cell classes for which gene signatures will be computed
 userPD = np.array(['DG'])
 
 colNum=32 # genomap column number
 rowNum=32 # genomap row number
 # Create genomaps
 genoMaps,gene_namesRe,T=createGenomap_for_sig(data,gene_names,rowNum,colNum)
 # compute the gene signatures
 result=genoSig(genoMaps,T,label,userPD,gene_namesRe, epochs=50)
 
-print(result.head())  
+print(result.head())
 ```
 
 ### Example 7 - Try genoClassification for tabular data classification
 
 ```python
 import pandas as pd
 import numpy as np
 import scipy.io as sio
-from genoClassification import genoClassification
-from util_genoClassReg import select_random_values
-
+from genomap.genoClassification import genoClassification
+from genomap.utils.util_genoClassReg import select_random_values
 
 # First, we load the TM data. Data should be in cells X genes format, 
 data = pd.read_csv('TM_data.csv', header=None,
                    delim_whitespace=False)
 
 # Creation of genomaps
 # Selection of row and column number of the genomaps 
@@ -217,15 +274,15 @@
 rowNum=33
 
 # Load ground truth cell labels of the TM dataset
 gt_data = sio.loadmat('GT_TM.mat')
 GT = np.squeeze(gt_data['GT'])
 GT=GT-1 # to ensure the labels begin with 0 to conform with PyTorch
 
-# Select 80% of data randomly for training and others for testing
+# Select 80% data randomly for training and others for testing
 indxTrain, indxTest= select_random_values(start=0, end=GT.shape[0], perc=0.8)
 groundTruthTest = GT[indxTest-1]
 
 training_data=data.values[indxTrain-1]
 training_labels=GT[indxTrain-1]
 test_data=data.values[indxTest-1]
 
@@ -237,38 +294,38 @@
 
 ### Example 8 - Try genoRegression for tabular data regression
 
 ```python
 import pandas as pd
 import numpy as np
 import scipy.io as sio
-from genoRegression import genoRegression
+from genomap.genoRegression import genoRegression
 from sklearn.metrics import mean_squared_error
-from util_genoClassReg import select_random_values
+from genomap.utils.util_genoClassReg import select_random_values
 
 # Load data and labels
-dx = sio.loadmat('../data/organoidData.mat')
+dx = sio.loadmat('organoidData.mat')
 data=dx['X3']
-gt_data = sio.loadmat('../data/GT_Org.mat')
+gt_data = sio.loadmat('GT_Org.mat')
 Y_time = np.squeeze(gt_data['GT'])
 Y_time = Y_time - 1 # to ensure the labels begin with 0 to conform with PyTorch
 
-# Select 80% of data randomly for training and others for testing
+# Select 80% data randomly for training and others for testing
 indxTrain, indxTest= select_random_values(start=0, end=Y_time.shape[0], perc=0.8)
 groundTruthTest = Y_time[indxTest-1]
 training_data=data[indxTrain-1]
 training_labels=Y_time[indxTrain-1]
 test_data=data[indxTest-1]
 
 # Run genoRegression
 est=genoRegression(training_data, training_labels, test_data, rowNum=40, colNum=40, epoch=200)
 
 # Calculate MSE
 mse = mean_squared_error(groundTruthTest, est)
-print(f'MSE: {mse}') 
+print(f'MSE: {mse}')
 ```
 
 # Citation
 
 If you use the genomap code, please cite our Nature Communications paper: https://www.nature.com/articles/s41467-023-36383-6
 
 Islam, M.T., Xing, L. Cartography of Genomic Interactions Enables Deep Analysis of Single-Cell Expression Data. Nat Commun 14, 679 (2023). https://doi.org/10.1038/s41467-023-36383-6
```

### Comparing `genomap-1.2.1/genomap/bregman_genomap/bregman_genomap.py` & `genomap-1.2.2/genomap/bregman_genomap/bregman_genomap.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.1/genomap/genoClassification/genoClassification.py` & `genomap-1.2.2/genomap/genoClassification/genoClassification.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.1/genomap/genoDR/genoDimReduction.py` & `genomap-1.2.2/genomap/genoDR/genoDimReduction.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.1/genomap/genoMOI/genoMOI.py` & `genomap-1.2.2/genomap/genoMOI/genoMOI.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.1/genomap/genoNetRegression/genoNet_regression.py` & `genomap-1.2.2/genomap/genoNetRegression/genoNet_regression.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.1/genomap/genoRegression/genoRegression.py` & `genomap-1.2.2/genomap/genoRegression/genoRegression.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.1/genomap/genoSig/genoSig.py` & `genomap-1.2.2/genomap/genoSig/genoSig.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.1/genomap/genoTraj/genoTraj.py` & `genomap-1.2.2/genomap/genoTraj/genoTraj.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.1/genomap/genoVis/genoVis.py` & `genomap-1.2.2/genomap/genoVis/genoVis.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.1/genomap/genomap.py` & `genomap-1.2.2/genomap/genomap.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.1/genomap/genomapOPT/genomapOPT.py` & `genomap-1.2.2/genomap/genomapOPT/genomapOPT.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.1/genomap/genomapT/genomapT.py` & `genomap-1.2.2/genomap/genomapT/genomapT.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.1/genomap/utils/ConvDEC.py` & `genomap-1.2.2/genomap/utils/ConvDEC.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.1/genomap/utils/ConvIDEC.py` & `genomap-1.2.2/genomap/utils/ConvIDEC.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.1/genomap/utils/FcDEC.py` & `genomap-1.2.2/genomap/utils/FcDEC.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.1/genomap/utils/FcIDEC.py` & `genomap-1.2.2/genomap/utils/FcIDEC.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.1/genomap/utils/class_discriminative_opt.py` & `genomap-1.2.2/genomap/utils/class_discriminative_opt.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.1/genomap/utils/gTraj_utils.py` & `genomap-1.2.2/genomap/utils/gTraj_utils.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.1/genomap/utils/group_centroid_opt.py` & `genomap-1.2.2/genomap/utils/group_centroid_opt.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.1/genomap/utils/metrics.py` & `genomap-1.2.2/genomap/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.1/genomap/utils/util_Sig.py` & `genomap-1.2.2/genomap/utils/util_Sig.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.1/genomap/utils/utils_MOI.py` & `genomap-1.2.2/genomap/utils/utils_MOI.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.1/genomap.egg-info/PKG-INFO` & `genomap-1.2.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: genomap
-Version: 1.2.1
-Summary: Genomap converts tabular gene expression data into spatially meaningful images.
-Home-page: https://github.com/xinglab-ai/genomap
-Author: Md Tauhidul Islam
-Author-email: tauhid@stanford.edu
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # Genomap creates images from gene expression data and offers high-performance dimensionality reduction and visualization, data clustering, classification and regression, gene signature extraction, multi-omics data integration, and trajectory analysis 
 
 Genomap is an entropy-based cartography strategy to contrive the high dimensional gene expression data into a configured image format with explicit integration of the genomic interactions. This unique cartography casts the gene-gene interactions into a spatial configuration and enables us to extract the deep genomic interaction features and discover underlying discriminative patterns of the data. For a wide variety of applications (cell clustering and recognition, gene signature extraction, single-cell data integration, cellular trajectory analysis, dimensionality reduction, and visualization), genomap drastically improves the accuracy of data analyses as compared to state-of-the-art techniques.
 
 ## How to use genomap
 
 The easiest way to start with genomap is to install it from pypi using 
@@ -33,195 +20,239 @@
 ## Example codes
 
 ### Example 1 - Construct a genomap
 
 ```python
 import pandas as pd # Please install pandas and matplotlib before you run this example
 import matplotlib.pyplot as plt
+import numpy as np
 import scipy
-import genomap as gp
+from genomap import construct_genomap
 
-data = pd.read_csv('TM_data.csv', header=None, delim_whitespace=False)
-colNum=31 # Column number of genomap
-rowNum=31 # Row number of genomap
+data = pd.read_csv('TM_data.csv', header=None,
+                   delim_whitespace=False)
+colNum=33 # Column number of genomap
+rowNum=33 # Row number of genomap
 
 dataNorm=scipy.stats.zscore(data,axis=0,ddof=1) # Normalization of the data
 
-genoMaps=gp.construct_genomap(dataNorm,rowNum,colNum) # Construction of genomaps
+genoMaps=construct_genomap(dataNorm,rowNum,colNum,epsilon=0.0,num_iter=200) # Construction of genomaps
 
-findI=genoMaps[0,:,:,:]
+findI=genoMaps[10,:,:,:]
 
 plt.figure(1) # Plot the first genomap
-plt.imshow(findI, origin = 'lower', extent = [0, 10, 0, 10], aspect = 1)
+plt.imshow(findI, origin = 'lower',  extent = [0, 10, 0, 10], aspect = 1)
 plt.title('Genomap of a cell from TM dataset')
+plt.show()
 ```
 
 ### Example 2 - Try genoVis for data visualization and clustering
 
 ```python
 import scipy.io as sio
 import numpy as np
-import metrics
-from genomap.genoVis import compute_genoVis
-from genomap.genoTraj import compute_genoTraj
-from genomap.genoMOI import compute_genoMOI
+import pandas as pd
+from genomap.genoVis import genoVis
+import matplotlib.pyplot as plt
+from sklearn.cluster import KMeans
+from sklearn.decomposition import PCA
+import phate
+import umap
 
 data = pd.read_csv('TM_data.csv', header=None,
                    delim_whitespace=False)
 data=data.values
 gt_data = sio.loadmat('GT_TM.mat')
 y = np.squeeze(gt_data['GT'])
 n_clusters = len(np.unique(y))
 
-resVis=compute_genoVis(data,n_clusters=n_clusters, colNum=33,rowNum=33)
-# Use resVis=compute_genoVis(data, colNum=32,rowNum=32), if you do not know the number
+
+resVis=genoVis(data,n_clusters=n_clusters, colNum=33,rowNum=33)
+# Use resVis=compute_genoVis(data, colNum=32,rowNum=32), if you dont know the number
 # of classes in the data
 
 resVisEmb=resVis[0] # Dimensionality reduction and visualization result
 clusIndex=resVis[1] # Clustering result
 
 plt.figure(figsize=(15, 10))
 plt.rcParams.update({'font.size': 28})    
-h1=plt.scatter(resVisEmb[:, 0], resVisEmb[:, 1], c=y,cmap='jet', marker='o', s=18)     
+h1=plt.scatter(resVisEmb[:, 0], resVisEmb[:, 1], c=y,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
 plt.xlabel('genoVis1')
 plt.ylabel('genoVis2')
 plt.tight_layout()
 plt.colorbar(h1)
 
-# Print clustering accuracy metrics
+import genomap.utils.metrics as metrics
 print('acc=%.4f, nmi=%.4f, ari=%.4f' % (metrics.acc(y, clusIndex), metrics.nmi(y, clusIndex), metrics.ari(y, clusIndex)))
 ```
 
 ### Example 3 - Try genoDR for dimensionality reduction
 
 ```python
 import scipy.io as sio
 import numpy as np
-from genoDimReduction import compute_genoDimReduction
+from genomap.genoDR import genoDR
 import matplotlib.pyplot as plt
 import umap
 
-dx = sio.loadmat('../data/reducedData_divseq.mat')
+dx = sio.loadmat('reducedData_divseq.mat')
 data=dx['X']
-gt_data = sio.loadmat('../data/GT_divseq.mat')
+gt_data = sio.loadmat('GT_divseq.mat')
 y = np.squeeze(gt_data['GT'])
 n_clusters = len(np.unique(y))
 
-resDR=compute_genoDimReduction(data,n_clusters=n_clusters, colNum=33,rowNum=33)
+resDR=genoDR(data,n_clusters=n_clusters, colNum=33,rowNum=33)
 #resDR=compute_genoDimReduction(data, colNum=33,rowNum=33) # if you dont know the number
 # of classes in the data
 embedding2D = umap.UMAP(n_neighbors=30,min_dist=0.3,n_epochs=200).fit_transform(resDR)
 
 plt.figure(figsize=(15, 10))
 plt.rcParams.update({'font.size': 28})    
 h1=plt.scatter(embedding2D[:, 0], embedding2D[:, 1], c=y,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
 plt.xlabel('genoVis1')
 plt.ylabel('genoVis2')
 plt.tight_layout()
 plt.colorbar(h1)
+plt.show()
 ```
 
 ### Example 4 - Try genoTraj for cell trajectory analysis
 
 ```python
+import scipy.io as sio
+import numpy as np
+import pandas as pd
+import matplotlib.pyplot as plt
+from sklearn.cluster import KMeans
+from sklearn.decomposition import PCA
+import phate
+import umap
+from genomap.genoTraj import genoTraj
+
 # Load data
 dx = sio.loadmat('organoidData.mat')
 data=dx['X3']
 gt_data = sio.loadmat('cellsPsudo.mat')
 Y_time = np.squeeze(gt_data['newGT'])
 
 # Apply genoTraj for embedding showing cell trajectories
-outGenoTraj=compute_genoTraj(data)
+outGenoTraj=genoTraj(data)
 
 plt.figure(figsize=(15, 10))
 plt.rcParams.update({'font.size': 28})    
 h1=plt.scatter(outGenoTraj[:, 0], outGenoTraj[:, 1], c=Y_time,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
 plt.xlabel('genoTraj1')
 plt.ylabel('genoTraj2')
 plt.tight_layout()
 plt.colorbar(h1)
+plt.show()
 
+# Comparison with PHATE
+pca = PCA(n_components=100)
+resPCA=pca.fit_transform(data)
+
+phate_op = phate.PHATE()
+res_phate = phate_op.fit_transform(resPCA)
+    
+    
+plt.figure(figsize=(15, 10))
+plt.rcParams.update({'font.size': 28})    
+h1=plt.scatter(res_phate[:, 0], res_phate[:, 1], c=Y_time,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
+plt.xlabel('PHATE1')
+plt.ylabel('PHATE2')
+plt.tight_layout()
+plt.colorbar(h1)
+plt.show()
 ```
 
 ### Example 5 - Try genoMOI for multi-omic data integration
 
 ```python
+import scanpy as sc
+import matplotlib.pyplot as plt
+from genomap.genoMOI import genoMOI
+import scipy.io as sio
+import numpy as np
+import pandas as pd
+import umap
+
 
-# Load datasets
+# Load five different pancreatic datasets
 dx = sio.loadmat('dataBaronX.mat')
 data=dx['dataBaron']
 dx = sio.loadmat('dataMuraroX.mat')
 data2=dx['dataMuraro']
 dx = sio.loadmat('dataScapleX.mat')
 data3=dx['dataScaple']
 dx = sio.loadmat('dataWangX.mat')
 data4=dx['dataWang']
 dx = sio.loadmat('dataXinX.mat')
 data5=dx['dataXin']
+
 # Load class and batch labels
 dx = sio.loadmat('classLabel.mat')
 y = np.squeeze(dx['classLabel'])
 dx = sio.loadmat('batchLabel.mat')
 ybatch = np.squeeze(dx['batchLabel'])
 
 # Apply genoMOI
-resVis=compute_genoMOI(data, data2, data3, data4, data5, colNum=44, rowNum=44)
+resVis=genoMOI(data, data2, data3, data4, data5, colNum=44, rowNum=44)
 
 # Visualize the integrated data using UMAP
-embedding = umap.UMAP(n_neighbors=30,min_dist=0.3,n_epochs=200).fit_transform(resVis) 
+embedding = umap.UMAP(n_neighbors=30,min_dist=0.3,n_epochs=200).fit_transform(resVis)
 
 plt.figure(figsize=(15, 10))
 plt.rcParams.update({'font.size': 28})    
-h1=plt.scatter(embedding[:, 0], embedding[:, 1], c=y,cmap='jet', marker='o', s=18)     
-plt.xlabel('UMAP')
-plt.ylabel('UMAP2')
+h1=plt.scatter(embedding[:, 0], embedding[:, 1], c=y,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
+plt.xlabel('genoVis1')
+plt.ylabel('genoVis2')
 plt.tight_layout()
 plt.colorbar(h1)
+plt.show()
 ```
 
 ### Example 6 - Try genoSig for finding gene signatures for cell/data classes
 
 ```python
 import numpy as np
 import scipy.io as sio
-from util_Sig import createGenomap_for_sig
+from genomap.utils.util_Sig import createGenomap_for_sig
 import pandas as pd
-from compute_genoSig import genoSig
+from genomap.genoSig import genoSig
 
 # Load data
-dx = sio.loadmat('../data/reducedData_divseq.mat')
+dx = sio.loadmat('reducedData_divseq.mat')
 data=dx['X']
 # Load data labels
-label = pd.read_csv('../data/groundTruth_divseq.csv',header=None)
+label = pd.read_csv('groundTruth_divseq.csv',header=None)
 # Load gene names corresponding to the columns of the data
 gene_names = ['Gene_' + str(i) for i in range(1, data.shape[1]+1)]
 gene_names=np.array(gene_names)
 
 # The cell classes for which gene signatures will be computed
 userPD = np.array(['DG'])
 
 colNum=32 # genomap column number
 rowNum=32 # genomap row number
 # Create genomaps
 genoMaps,gene_namesRe,T=createGenomap_for_sig(data,gene_names,rowNum,colNum)
 # compute the gene signatures
 result=genoSig(genoMaps,T,label,userPD,gene_namesRe, epochs=50)
 
-print(result.head())  
+print(result.head())
 ```
 
 ### Example 7 - Try genoClassification for tabular data classification
 
 ```python
 import pandas as pd
 import numpy as np
 import scipy.io as sio
-from genoClassification import genoClassification
-from util_genoClassReg import select_random_values
-
+from genomap.genoClassification import genoClassification
+from genomap.utils.util_genoClassReg import select_random_values
 
 # First, we load the TM data. Data should be in cells X genes format, 
 data = pd.read_csv('TM_data.csv', header=None,
                    delim_whitespace=False)
 
 # Creation of genomaps
 # Selection of row and column number of the genomaps 
@@ -230,15 +261,15 @@
 rowNum=33
 
 # Load ground truth cell labels of the TM dataset
 gt_data = sio.loadmat('GT_TM.mat')
 GT = np.squeeze(gt_data['GT'])
 GT=GT-1 # to ensure the labels begin with 0 to conform with PyTorch
 
-# Select 80% of data randomly for training and others for testing
+# Select 80% data randomly for training and others for testing
 indxTrain, indxTest= select_random_values(start=0, end=GT.shape[0], perc=0.8)
 groundTruthTest = GT[indxTest-1]
 
 training_data=data.values[indxTrain-1]
 training_labels=GT[indxTrain-1]
 test_data=data.values[indxTest-1]
 
@@ -250,38 +281,38 @@
 
 ### Example 8 - Try genoRegression for tabular data regression
 
 ```python
 import pandas as pd
 import numpy as np
 import scipy.io as sio
-from genoRegression import genoRegression
+from genomap.genoRegression import genoRegression
 from sklearn.metrics import mean_squared_error
-from util_genoClassReg import select_random_values
+from genomap.utils.util_genoClassReg import select_random_values
 
 # Load data and labels
-dx = sio.loadmat('../data/organoidData.mat')
+dx = sio.loadmat('organoidData.mat')
 data=dx['X3']
-gt_data = sio.loadmat('../data/GT_Org.mat')
+gt_data = sio.loadmat('GT_Org.mat')
 Y_time = np.squeeze(gt_data['GT'])
 Y_time = Y_time - 1 # to ensure the labels begin with 0 to conform with PyTorch
 
-# Select 80% of data randomly for training and others for testing
+# Select 80% data randomly for training and others for testing
 indxTrain, indxTest= select_random_values(start=0, end=Y_time.shape[0], perc=0.8)
 groundTruthTest = Y_time[indxTest-1]
 training_data=data[indxTrain-1]
 training_labels=Y_time[indxTrain-1]
 test_data=data[indxTest-1]
 
 # Run genoRegression
 est=genoRegression(training_data, training_labels, test_data, rowNum=40, colNum=40, epoch=200)
 
 # Calculate MSE
 mse = mean_squared_error(groundTruthTest, est)
-print(f'MSE: {mse}') 
+print(f'MSE: {mse}')
 ```
 
 # Citation
 
 If you use the genomap code, please cite our Nature Communications paper: https://www.nature.com/articles/s41467-023-36383-6
 
 Islam, M.T., Xing, L. Cartography of Genomic Interactions Enables Deep Analysis of Single-Cell Expression Data. Nat Commun 14, 679 (2023). https://doi.org/10.1038/s41467-023-36383-6
```

### Comparing `genomap-1.2.1/genomap.egg-info/SOURCES.txt` & `genomap-1.2.2/genomap.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -39,8 +39,9 @@
 genomap/utils/FcIDEC.py
 genomap/utils/__init__.py
 genomap/utils/class_discriminative_opt.py
 genomap/utils/gTraj_utils.py
 genomap/utils/group_centroid_opt.py
 genomap/utils/metrics.py
 genomap/utils/util_Sig.py
+genomap/utils/util_genoClassReg.py
 genomap/utils/utils_MOI.py
```

### Comparing `genomap-1.2.1/setup.py` & `genomap-1.2.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="genomap",
-    version="1.2.1",
+    version="1.2.2",
     author="Md Tauhidul Islam",
     author_email="tauhid@stanford.edu",
     description="Genomap converts tabular gene expression data into spatially meaningful images.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/xinglab-ai/genomap",
     classifiers=[
```

