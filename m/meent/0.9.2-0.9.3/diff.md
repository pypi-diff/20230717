# Comparing `tmp/meent-0.9.2.tar.gz` & `tmp/meent-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meent-0.9.2.tar", last modified: Tue May  2 14:35:52 2023, max compression
+gzip compressed data, was "meent-0.9.3.tar", last modified: Mon Jul 17 06:20:29 2023, max compression
```

## Comparing `meent-0.9.2.tar` & `meent-0.9.3.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:35:52.947544 meent-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-02 14:35:37.000000 meent-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-02 14:35:52.947544 meent-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-05-02 14:35:37.000000 meent-0.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:35:52.939544 meent-0.9.2/meent/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-02 14:35:37.000000 meent-0.9.2/meent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-05-02 14:35:37.000000 meent-0.9.2/meent/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:35:52.939544 meent-0.9.2/meent/nk_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:35:52.943544 meent-0.9.2/meent/nk_data/filmetrics/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-02 14:35:37.000000 meent-0.9.2/meent/nk_data/filmetrics/Al2O3.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-05-02 14:35:37.000000 meent-0.9.2/meent/nk_data/filmetrics/Si.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-02 14:35:37.000000 meent-0.9.2/meent/nk_data/filmetrics/Si3N4.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-05-02 14:35:37.000000 meent-0.9.2/meent/nk_data/filmetrics/SiO2.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:35:52.943544 meent-0.9.2/meent/nk_data/matlab/
--rw-r--r--   0 runner    (1001) docker     (123)    11222 2023-05-02 14:35:37.000000 meent-0.9.2/meent/nk_data/matlab/p_Si.mat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:35:52.943544 meent-0.9.2/meent/on_jax/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_jax/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:35:52.943544 meent-0.9.2/meent/on_jax/emsolver/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_jax/emsolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16856 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_jax/emsolver/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12769 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_jax/emsolver/convolution_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    38784 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_jax/emsolver/field_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_jax/emsolver/primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)    13965 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_jax/emsolver/rcwa.py
--rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_jax/emsolver/scattering_method.py
--rw-r--r--   0 runner    (1001) docker     (123)    10546 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_jax/emsolver/smm_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    14577 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_jax/emsolver/transfer_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_jax/mee.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:35:52.943544 meent-0.9.2/meent/on_jax/modeler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_jax/modeler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_jax/modeler/modeling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:35:52.943544 meent-0.9.2/meent/on_jax/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_jax/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_jax/optimizer/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_jax/optimizer/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:35:52.943544 meent-0.9.2/meent/on_numpy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_numpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:35:52.947544 meent-0.9.2/meent/on_numpy/emsolver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_numpy/emsolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14815 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_numpy/emsolver/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_numpy/emsolver/convolution_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    27387 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_numpy/emsolver/field_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_numpy/emsolver/rcwa.py
--rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_numpy/emsolver/scattering_method.py
--rw-r--r--   0 runner    (1001) docker     (123)    10530 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_numpy/emsolver/smm_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    12377 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_numpy/emsolver/transfer_method.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_numpy/mee.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:35:52.947544 meent-0.9.2/meent/on_numpy/modeler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_numpy/modeler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_numpy/modeler/modeling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:35:52.947544 meent-0.9.2/meent/on_torch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:35:52.947544 meent-0.9.2/meent/on_torch/emsolver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_torch/emsolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18368 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_torch/emsolver/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13557 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_torch/emsolver/convolution_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    29243 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_torch/emsolver/field_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_torch/emsolver/primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)    11858 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_torch/emsolver/rcwa.py
--rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_torch/emsolver/scattering_method.py
--rw-r--r--   0 runner    (1001) docker     (123)    10516 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_torch/emsolver/smm_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    14085 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_torch/emsolver/transfer_method.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_torch/mee.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:35:52.947544 meent-0.9.2/meent/on_torch/modeler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_torch/modeler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_torch/modeler/modeling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:35:52.947544 meent-0.9.2/meent/on_torch/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_torch/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_torch/optimizer/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_torch/optimizer/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:35:52.943544 meent-0.9.2/meent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-02 14:35:52.000000 meent-0.9.2/meent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-02 14:35:52.000000 meent-0.9.2/meent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 14:35:52.000000 meent-0.9.2/meent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-02 14:35:52.000000 meent-0.9.2/meent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-02 14:35:52.000000 meent-0.9.2/meent.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 14:35:52.947544 meent-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-02 14:35:37.000000 meent-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:20:29.113585 meent-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-17 06:20:15.000000 meent-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-17 06:20:29.113585 meent-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-07-17 06:20:15.000000 meent-0.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:20:29.105585 meent-0.9.3/meent/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-17 06:20:15.000000 meent-0.9.3/meent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-07-17 06:20:15.000000 meent-0.9.3/meent/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:20:29.105585 meent-0.9.3/meent/nk_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:20:29.105585 meent-0.9.3/meent/nk_data/filmetrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-17 06:20:15.000000 meent-0.9.3/meent/nk_data/filmetrics/Al2O3.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-07-17 06:20:15.000000 meent-0.9.3/meent/nk_data/filmetrics/Si.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-07-17 06:20:15.000000 meent-0.9.3/meent/nk_data/filmetrics/Si3N4.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-07-17 06:20:15.000000 meent-0.9.3/meent/nk_data/filmetrics/SiO2.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:20:29.105585 meent-0.9.3/meent/nk_data/matlab/
+-rw-r--r--   0 runner    (1001) docker     (123)    11222 2023-07-17 06:20:15.000000 meent-0.9.3/meent/nk_data/matlab/p_Si.mat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:20:29.105585 meent-0.9.3/meent/on_jax/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_jax/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:20:29.109585 meent-0.9.3/meent/on_jax/emsolver/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_jax/emsolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16856 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_jax/emsolver/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12769 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_jax/emsolver/convolution_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38784 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_jax/emsolver/field_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_jax/emsolver/primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14059 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_jax/emsolver/rcwa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_jax/emsolver/scattering_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10546 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_jax/emsolver/smm_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14577 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_jax/emsolver/transfer_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_jax/mee.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:20:29.109585 meent-0.9.3/meent/on_jax/modeler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_jax/modeler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_jax/modeler/modeling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:20:29.109585 meent-0.9.3/meent/on_jax/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_jax/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_jax/optimizer/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_jax/optimizer/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:20:29.109585 meent-0.9.3/meent/on_numpy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_numpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:20:29.109585 meent-0.9.3/meent/on_numpy/emsolver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_numpy/emsolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14816 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_numpy/emsolver/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_numpy/emsolver/convolution_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27387 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_numpy/emsolver/field_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_numpy/emsolver/rcwa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_numpy/emsolver/scattering_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10530 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_numpy/emsolver/smm_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12377 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_numpy/emsolver/transfer_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_numpy/mee.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:20:29.109585 meent-0.9.3/meent/on_numpy/modeler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_numpy/modeler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_numpy/modeler/modeling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:20:29.109585 meent-0.9.3/meent/on_torch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:20:29.113585 meent-0.9.3/meent/on_torch/emsolver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_torch/emsolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18452 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_torch/emsolver/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20183 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_torch/emsolver/convolution_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29243 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_torch/emsolver/field_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_torch/emsolver/primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11864 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_torch/emsolver/rcwa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_torch/emsolver/scattering_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10516 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_torch/emsolver/smm_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14085 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_torch/emsolver/transfer_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_torch/mee.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:20:29.113585 meent-0.9.3/meent/on_torch/modeler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_torch/modeler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15839 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_torch/modeler/modeling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:20:29.113585 meent-0.9.3/meent/on_torch/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_torch/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_torch/optimizer/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_torch/optimizer/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:20:29.105585 meent-0.9.3/meent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-17 06:20:29.000000 meent-0.9.3/meent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-07-17 06:20:29.000000 meent-0.9.3/meent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 06:20:29.000000 meent-0.9.3/meent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-17 06:20:29.000000 meent-0.9.3/meent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-17 06:20:29.000000 meent-0.9.3/meent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 06:20:29.113585 meent-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-17 06:20:15.000000 meent-0.9.3/setup.py
```

### Comparing `meent-0.9.2/LICENSE` & `meent-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `meent-0.9.2/README.md` & `meent-0.9.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 Jupyter notebooks are prepared in [tutorials](tutorials) to give a brief introduction.
 
 ## Citation
 To cite this repository:
 
 ```
 @software{Kim_Meent_Electromagnetic_simulation,
-  author = {Kim, Yongha and Kim, Sanmun and Lee, Jinmyoung and Jeong, Anthony Wonseok and Kim, Seolho},
+  author = {Kim, Yongha and Kim, Sanmun and Lee, Jinmyoung and Jung, Anthony W. and Kim, Seolho},
   license = {MIT},
   title = {{Meent:Electromagnetic simulation & optimization package in Python}},
   url = {https://github.com/kc-ml2/meent}
 }
 ```
 
 ## Reference
```

### Comparing `meent-0.9.2/meent/main.py` & `meent-0.9.3/meent/main.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.2/meent/nk_data/filmetrics/Al2O3.txt` & `meent-0.9.3/meent/nk_data/filmetrics/Al2O3.txt`

 * *Files identical despite different names*

### Comparing `meent-0.9.2/meent/nk_data/filmetrics/Si.txt` & `meent-0.9.3/meent/nk_data/filmetrics/Si.txt`

 * *Files identical despite different names*

### Comparing `meent-0.9.2/meent/nk_data/filmetrics/Si3N4.txt` & `meent-0.9.3/meent/nk_data/filmetrics/Si3N4.txt`

 * *Files identical despite different names*

### Comparing `meent-0.9.2/meent/nk_data/filmetrics/SiO2.txt` & `meent-0.9.3/meent/nk_data/filmetrics/SiO2.txt`

 * *Files identical despite different names*

### Comparing `meent-0.9.2/meent/nk_data/matlab/p_Si.mat` & `meent-0.9.3/meent/nk_data/matlab/p_Si.mat`

 * *Files identical despite different names*

### Comparing `meent-0.9.2/meent/on_jax/emsolver/_base.py` & `meent-0.9.3/meent/on_jax/emsolver/_base.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.2/meent/on_jax/emsolver/convolution_matrix.py` & `meent-0.9.3/meent/on_jax/emsolver/convolution_matrix.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.2/meent/on_jax/emsolver/field_distribution.py` & `meent-0.9.3/meent/on_jax/emsolver/field_distribution.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.2/meent/on_jax/emsolver/primitives.py` & `meent-0.9.3/meent/on_jax/emsolver/primitives.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.2/meent/on_jax/emsolver/rcwa.py` & `meent-0.9.3/meent/on_jax/emsolver/rcwa.py`

 * *Files 2% similar despite different names*

```diff
@@ -250,15 +250,16 @@
         print('gap(2-1): ', jnp.linalg.norm(field_cell2 - field_cell1))
         print('gap(0-2): ', jnp.linalg.norm(field_cell0 - field_cell2))
 
         return field_cell0, field_cell1, field_cell2
 
     @partial(jax.jit, static_argnums=(1, 2, 3, 4))
     @_BaseRCWA.jax_device_set
-    def conv_solve_field(self, res_x=20, res_y=20, res_z=20, field_algo=2):
+    def conv_solve_field(self, res_x=20, res_y=20, res_z=20, field_algo=2, **kwargs):
+        [setattr(self, k, v) for k, v in kwargs.items()]  # needed for optimization
 
         if self.fft_type == 1:
             print('CFT (fft_type=1) is not supported with JAX jit-compilation. Use conv_solve_field_no_jit.')
             return None, None, None
 
         de_ri, de_ti, _, _, _ = self._conv_solve()
         field_cell = self.calculate_field(res_x, res_y, res_z, field_algo=field_algo)
```

### Comparing `meent-0.9.2/meent/on_jax/emsolver/scattering_method.py` & `meent-0.9.3/meent/on_jax/emsolver/scattering_method.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.2/meent/on_jax/emsolver/smm_util.py` & `meent-0.9.3/meent/on_jax/emsolver/smm_util.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.2/meent/on_jax/emsolver/transfer_method.py` & `meent-0.9.3/meent/on_jax/emsolver/transfer_method.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.2/meent/on_jax/mee.py` & `meent-0.9.3/meent/on_jax/mee.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.2/meent/on_jax/modeler/modeling.py` & `meent-0.9.3/meent/on_jax/modeler/modeling.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.2/meent/on_jax/optimizer/loss.py` & `meent-0.9.3/meent/on_jax/optimizer/loss.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.2/meent/on_jax/optimizer/optimizer.py` & `meent-0.9.3/meent/on_jax/optimizer/optimizer.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.2/meent/on_numpy/emsolver/_base.py` & `meent-0.9.3/meent/on_numpy/emsolver/_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -226,14 +226,15 @@
                 E_conv_i = None
                 A = Kx ** 2 - E_conv
                 eigenvalues, W = np.linalg.eig(A)
                 eigenvalues += 0j  # to get positive square root
                 q = eigenvalues ** 0.5
                 Q = np.diag(q)
                 V = W @ Q
+
             elif self.pol == 1:
                 E_conv_i = np.linalg.inv(E_conv)
                 B = Kx @ E_conv_i @ Kx - np.eye(E_conv.shape[0], dtype=self.type_complex)
                 o_E_conv_i = np.linalg.inv(o_E_conv)
 
                 eigenvalues, W = np.linalg.eig(o_E_conv_i @ B)
                 eigenvalues += 0j  # to get positive square root
```

### Comparing `meent-0.9.2/meent/on_numpy/emsolver/convolution_matrix.py` & `meent-0.9.3/meent/on_numpy/emsolver/convolution_matrix.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.2/meent/on_numpy/emsolver/field_distribution.py` & `meent-0.9.3/meent/on_numpy/emsolver/field_distribution.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.2/meent/on_numpy/emsolver/rcwa.py` & `meent-0.9.3/meent/on_numpy/emsolver/rcwa.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.2/meent/on_numpy/emsolver/scattering_method.py` & `meent-0.9.3/meent/on_numpy/emsolver/scattering_method.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.2/meent/on_numpy/emsolver/smm_util.py` & `meent-0.9.3/meent/on_numpy/emsolver/smm_util.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.2/meent/on_numpy/emsolver/transfer_method.py` & `meent-0.9.3/meent/on_numpy/emsolver/transfer_method.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.2/meent/on_numpy/mee.py` & `meent-0.9.3/meent/on_numpy/mee.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.2/meent/on_numpy/modeler/modeling.py` & `meent-0.9.3/meent/on_numpy/modeler/modeling.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
         col_list = []
 
         for obj in obj_list:
             top_left, bottom_right, pmty = obj
             row_list.extend([top_left[0], bottom_right[0]])
             col_list.extend([top_left[1], bottom_right[1]])
 
+        # TODO: set seems not right for backprop
         row_list = list(set(row_list))
         col_list = list(set(col_list))
 
         row_list.sort()
         col_list.sort()
 
         if not row_list or row_list[-1] != period[0]:
```

### Comparing `meent-0.9.2/meent/on_torch/emsolver/_base.py` & `meent-0.9.3/meent/on_torch/emsolver/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,44 +67,46 @@
         elif device == 1:
             self._device = torch.device('cuda')
         elif type(device) is torch.device:
             self._device = device
         else:
             raise ValueError
 
-        try:
-            self._theta = self._theta.to(self.device)
-            self._phi = self._phi.to(self.device)
-            self._psi = self._psi.to(self.device)
-            self.thickness = self._thickness.to(self.device)
-        except AssertionError as e:
-            print(f'{e}. Get back to CPU')
-            self._device = torch.device('cpu')
+        # TODO: need this?
+        # try:
+        #     self._theta = self._theta.to(self.device)
+        #     self._phi = self._phi.to(self.device)
+        #     self._psi = self._psi.to(self.device)
+        #     self.thickness = self._thickness.to(self.device)
+        # except AssertionError as e:
+        #     print(f'{e}. Get back to CPU')
+        #     self._device = torch.device('cpu')
 
     @property
     def type_complex(self):
         return self._type_complex
 
     @type_complex.setter
     def type_complex(self, type_complex):
         if type_complex in (0, torch.complex128, np.complex128):
             self._type_complex = torch.complex128
         elif type_complex in (1, torch.complex64, np.complex64):
             self._type_complex = torch.complex64
         else:
             raise ValueError('type_complex')
 
-        self._type_float = torch.float64 if self.type_complex is not torch.complex64 else torch.float32
-        self._type_int = torch.int64 if self.type_complex is not torch.complex64 else torch.int32
-        self._theta = self._theta.to(self.type_float)
-        self._phi = self._phi.to(self.type_float)
-        self._psi = self._psi.to(self.type_float)
+        # TODO: need this?
+        # self._type_float = torch.float64 if self.type_complex is not torch.complex64 else torch.float32
+        # self._type_int = torch.int64 if self.type_complex is not torch.complex64 else torch.int32
+        # self._theta = self._theta.to(self.type_float)
+        # self._phi = self._phi.to(self.type_float)
+        # self._psi = self._psi.to(self.type_float)
 
-        self.fourier_order = self._fourier_order
-        self.thickness = self._thickness
+        # self.fourier_order = self._fourier_order
+        # self.thickness = self._thickness
 
     @property
     def type_float(self):
         return self._type_float
 
     @property
     def type_int(self):
```

### Comparing `meent-0.9.2/meent/on_torch/emsolver/convolution_matrix.py` & `meent-0.9.3/meent/on_torch/emsolver/convolution_matrix.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     x = []
     y = []
     cell_x = []
     cell_xy = []
 
     cell_next = torch.roll(cell, -1, dims=1)
 
-    for col in range(cell.shape[1]):
+    for col in torch.arange(cell.shape[1]):
         if not (cell[:, col] == cell_next[:, col]).all() or (col == cell.shape[1] - 1):
             x.append(step_x * (col + 1))
             cell_x.append(cell[:, col].reshape((1, -1)))
 
     cell_x = torch.cat(cell_x, dim=0).T
     cell_x_next = torch.roll(cell_x, -1, dims=0)
 
@@ -33,123 +33,162 @@
     x = torch.tensor(x, device=device).reshape((-1, 1)).type(type_complex)
     y = torch.tensor(y, device=device).reshape((-1, 1)).type(type_complex)
     cell_comp = torch.cat(cell_xy, dim=0)
 
     return cell_comp, x, y
 
 
-def fft_piecewise_constant(cell, fourier_order_x, fourier_order_y, device=torch.device('cpu'), type_complex=torch.complex128):
+# def fft_piecewise_constant(cell, fourier_order_x, fourier_order_y, device=torch.device('cpu'), type_complex=torch.complex128):
+#
+#     cell, x, y = cell_compression(cell, device=device, type_complex=type_complex)
+#
+#     # X axis
+#     cell_next_x = torch.roll(cell, -1, dims=1)
+#     cell_diff_x = cell_next_x - cell
+#     cell_diff_x = cell_diff_x.type(type_complex)
+#
+#     cell = cell.type(type_complex)
+#
+#     modes_x = torch.arange(-2 * fourier_order_x, 2 * fourier_order_x + 1, 1, device=device).type(type_complex)
+#
+#     f_coeffs_x = cell_diff_x @ torch.exp(-1j * 2 * torch.pi * x @ modes_x[None, :]).type(type_complex)
+#     c = f_coeffs_x.shape[1] // 2
+#
+#     x_next = torch.vstack((torch.roll(x, -1, dims=0)[:-1], torch.tensor([1], device=device))) - x
+#
+#     f_coeffs_x[:, c] = (cell @ torch.vstack((x[0], x_next[:-1]))).flatten()
+#     mask = torch.ones(f_coeffs_x.shape[1], device=device).type(torch.bool)
+#     mask[c] = False
+#     f_coeffs_x[:, mask] /= (1j * 2 * torch.pi * modes_x[mask])
+#
+#     # Y axis
+#     f_coeffs_x_next_y = torch.roll(f_coeffs_x, -1, dims=0)
+#     f_coeffs_x_diff_y = f_coeffs_x_next_y - f_coeffs_x
+#
+#     modes_y = torch.arange(-2 * fourier_order_y, 2 * fourier_order_y + 1, 1, device=device).type(type_complex)
+#
+#     f_coeffs_xy = f_coeffs_x_diff_y.T @ torch.exp(-1j * 2 * torch.pi * y @ modes_y[None, :])
+#     c = f_coeffs_xy.shape[1] // 2
+#
+#     y_next = torch.vstack((torch.roll(y, -1, dims=0)[:-1], torch.tensor([1], device=device))) - y
+#
+#     f_coeffs_xy[:, c] = f_coeffs_x.T @ torch.vstack((y[0], y_next[:-1])).flatten()
+#
+#     if c:
+#         mask = torch.ones(f_coeffs_xy.shape[1], device=device).type(torch.bool)
+#         mask[c] = False
+#         f_coeffs_xy[:, mask] /= (1j * 2 * torch.pi * modes_y[mask])
+#
+#     return f_coeffs_xy.T
+
+
+# def fft_piecewise_constant_vector(cell, x, y, fourier_order_x, fourier_order_y, device=torch.device('cpu'),
+#                                   type_complex=torch.complex128):
+#     # X axis
+#     cell_next_x = torch.roll(cell, -1, dims=1)
+#     cell_diff_x = cell_next_x - cell
+#     cell_diff_x = cell_diff_x.type(type_complex)
+#
+#     cell = cell.type(type_complex)
+#
+#     modes_x = torch.arange(-2 * fourier_order_x, 2 * fourier_order_x + 1, 1, device=device).type(type_complex)
+#
+#     f_coeffs_x = cell_diff_x @ torch.exp(-1j * 2 * torch.pi * x @ modes_x[None, :]).type(type_complex)
+#     c = f_coeffs_x.shape[1] // 2
+#
+#     x_next = torch.vstack((torch.roll(x, -1, dims=0)[:-1], torch.tensor([1], device=device))) - x
+#
+#     f_coeffs_x[:, c] = (cell @ torch.vstack((x[0], x_next[:-1]))).flatten()
+#     mask = torch.ones(f_coeffs_x.shape[1], device=device).type(torch.bool)
+#     mask[c] = False
+#     f_coeffs_x[:, mask] /= (1j * 2 * torch.pi * modes_x[mask])
+#
+#     # Y axis
+#     f_coeffs_x_next_y = torch.roll(f_coeffs_x, -1, dims=0)
+#     f_coeffs_x_diff_y = f_coeffs_x_next_y - f_coeffs_x
+#
+#     modes_y = torch.arange(-2 * fourier_order_y, 2 * fourier_order_y + 1, 1, device=device).type(type_complex)
+#
+#     f_coeffs_xy = f_coeffs_x_diff_y.T @ torch.exp(-1j * 2 * torch.pi * y @ modes_y[None, :])
+#     c = f_coeffs_xy.shape[1] // 2
+#
+#     y_next = torch.vstack((torch.roll(y, -1, dims=0)[:-1], torch.tensor([1], device=device))) - y
+#
+#     f_coeffs_xy[:, c] = f_coeffs_x.T @ torch.vstack((y[0], y_next[:-1])).flatten()
+#
+#     if c:
+#         mask = torch.ones(f_coeffs_xy.shape[1], device=device).type(torch.bool)
+#         mask[c] = False
+#         f_coeffs_xy[:, mask] /= (1j * 2 * torch.pi * modes_y[mask])
+#
+#     return f_coeffs_xy.T
 
-    cell, x, y = cell_compression(cell, device=device, type_complex=type_complex)
 
-    # X axis
-    cell_next_x = torch.roll(cell, -1, dims=1)
-    cell_diff_x = cell_next_x - cell
-    cell_diff_x = cell_diff_x.type(type_complex)
-
-    cell = cell.type(type_complex)
-
-    modes_x = torch.arange(-2 * fourier_order_x, 2 * fourier_order_x + 1, 1, device=device).type(type_complex)
-
-    f_coeffs_x = cell_diff_x @ torch.exp(-1j * 2 * torch.pi * x @ modes_x[None, :]).type(type_complex)
-    c = f_coeffs_x.shape[1] // 2
-
-    x_next = torch.vstack((torch.roll(x, -1, dims=0)[:-1], torch.tensor([1], device=device))) - x
-
-    f_coeffs_x[:, c] = (cell @ torch.vstack((x[0], x_next[:-1]))).flatten()
-    mask = torch.ones(f_coeffs_x.shape[1], device=device).type(torch.bool)
-    mask[c] = False
-    f_coeffs_x[:, mask] /= (1j * 2 * torch.pi * modes_x[mask])
-
-    # Y axis
-    f_coeffs_x_next_y = torch.roll(f_coeffs_x, -1, dims=0)
-    f_coeffs_x_diff_y = f_coeffs_x_next_y - f_coeffs_x
-
-    modes_y = torch.arange(-2 * fourier_order_y, 2 * fourier_order_y + 1, 1, device=device).type(type_complex)
-
-    f_coeffs_xy = f_coeffs_x_diff_y.T @ torch.exp(-1j * 2 * torch.pi * y @ modes_y[None, :])
-    c = f_coeffs_xy.shape[1] // 2
-
-    y_next = torch.vstack((torch.roll(y, -1, dims=0)[:-1], torch.tensor([1], device=device))) - y
-
-    f_coeffs_xy[:, c] = f_coeffs_x.T @ torch.vstack((y[0], y_next[:-1])).flatten()
-
-    if c:
-        mask = torch.ones(f_coeffs_xy.shape[1], device=device).type(torch.bool)
-        mask[c] = False
-        f_coeffs_xy[:, mask] /= (1j * 2 * torch.pi * modes_y[mask])
-
-    return f_coeffs_xy.T
+def fft_piecewise_constant(cell, x, y, fourier_order_x, fourier_order_y, device=torch.device('cpu'),
+                           type_complex=torch.complex128):
 
+    period_x, period_y = x[-1], y[-1]
 
-def fft_piecewise_constant_vector(cell, x, y, fourier_order_x, fourier_order_y, device=torch.device('cpu'),
-                                  type_complex=torch.complex128):
     # X axis
     cell_next_x = torch.roll(cell, -1, dims=1)
     cell_diff_x = cell_next_x - cell
     cell_diff_x = cell_diff_x.type(type_complex)
 
     cell = cell.type(type_complex)
 
     modes_x = torch.arange(-2 * fourier_order_x, 2 * fourier_order_x + 1, 1, device=device).type(type_complex)
 
-    f_coeffs_x = cell_diff_x @ torch.exp(-1j * 2 * torch.pi * x @ modes_x[None, :]).type(type_complex)
+    f_coeffs_x = cell_diff_x @ torch.exp(-1j * 2 * torch.pi * x @ modes_x[None, :] / period_x).type(type_complex)
     c = f_coeffs_x.shape[1] // 2
 
-    x_next = torch.vstack((torch.roll(x, -1, dims=0)[:-1], torch.tensor([1], device=device))) - x
+    x_next = torch.vstack((torch.roll(x, -1, dims=0)[:-1], torch.tensor([period_x], device=device))) - x
 
-    f_coeffs_x[:, c] = (cell @ torch.vstack((x[0], x_next[:-1]))).flatten()
+    f_coeffs_x[:, c] = (cell @ torch.vstack((x[0], x_next[:-1]))).flatten() / period_x
     mask = torch.ones(f_coeffs_x.shape[1], device=device).type(torch.bool)
     mask[c] = False
     f_coeffs_x[:, mask] /= (1j * 2 * torch.pi * modes_x[mask])
 
     # Y axis
     f_coeffs_x_next_y = torch.roll(f_coeffs_x, -1, dims=0)
     f_coeffs_x_diff_y = f_coeffs_x_next_y - f_coeffs_x
 
     modes_y = torch.arange(-2 * fourier_order_y, 2 * fourier_order_y + 1, 1, device=device).type(type_complex)
 
-    f_coeffs_xy = f_coeffs_x_diff_y.T @ torch.exp(-1j * 2 * torch.pi * y @ modes_y[None, :])
+    f_coeffs_xy = f_coeffs_x_diff_y.T @ torch.exp(-1j * 2 * torch.pi * y @ modes_y[None, :] / period_y)
     c = f_coeffs_xy.shape[1] // 2
 
-    y_next = torch.vstack((torch.roll(y, -1, dims=0)[:-1], torch.tensor([1], device=device))) - y
+    y_next = torch.vstack((torch.roll(y, -1, dims=0)[:-1], torch.tensor([period_y], device=device))) - y
 
-    f_coeffs_xy[:, c] = f_coeffs_x.T @ torch.vstack((y[0], y_next[:-1])).flatten()
+    f_coeffs_xy[:, c] = f_coeffs_x.T @ torch.vstack((y[0], y_next[:-1])).flatten() / period_y
 
     if c:
         mask = torch.ones(f_coeffs_xy.shape[1], device=device).type(torch.bool)
         mask[c] = False
         f_coeffs_xy[:, mask] /= (1j * 2 * torch.pi * modes_y[mask])
 
     return f_coeffs_xy.T
 
 
-def to_conv_mat_continuous_vector(ucell_info_list, fourier_order_x, fourier_order_y, device=torch.device('cpu'),
-                                  type_complex=torch.complex128):
+def to_conv_mat_vector(ucell_info_list, fourier_order_x, fourier_order_y, device=torch.device('cpu'),
+                       type_complex=torch.complex128):
     ff_x = 2 * fourier_order_x + 1
     ff_y = 2 * fourier_order_y + 1
 
-    e_conv_all = torch.zeros((len(ucell_info_list), ff_x * ff_y, ff_x * ff_y)).type(type_complex)
-    o_e_conv_all = torch.zeros((len(ucell_info_list), ff_x * ff_y, ff_x * ff_y)).type(type_complex)
+    e_conv_all = torch.zeros((len(ucell_info_list), ff_x * ff_y, ff_x * ff_y), device=device).type(type_complex)
+    o_e_conv_all = torch.zeros((len(ucell_info_list), ff_x * ff_y, ff_x * ff_y), device=device).type(type_complex)
 
     # 2D
-    for i, ucell_info in enumerate(ucell_info_list):
-        ucell_layer, x_list, y_list = ucell_info
-        ucell_layer = ucell_layer ** 2
-        # ucell_layer = torch.tensor(ucell_layer, dtype=type_complex) if type(ucell_layer) != torch.Tensor else ucell_layer
-        # x_list = torch.tensor(x_list, dtype=type_complex) if type(x_list) != torch.Tensor else x_list
-        # y_list = torch.tensor(y_list, dtype=type_complex) if type(y_list) != torch.Tensor else y_list
-
-        f_coeffs = fft_piecewise_constant_vector(ucell_layer, x_list, y_list,
-                                                 fourier_order_x, fourier_order_y, type_complex=type_complex)
-        o_f_coeffs = fft_piecewise_constant_vector(1/ucell_layer, x_list, y_list,
-                                                 fourier_order_x, fourier_order_y, type_complex=type_complex)
+    for i, (cell, x_list, y_list) in enumerate(ucell_info_list):
+
+        f_coeffs = fft_piecewise_constant(cell**2, x_list, y_list,
+                                          fourier_order_x, fourier_order_y, device=device, type_complex=type_complex)
+        o_f_coeffs = fft_piecewise_constant(1 / cell**2, x_list, y_list,
+                                            fourier_order_x, fourier_order_y, device=device, type_complex=type_complex)
 
-        center = torch.div(torch.tensor(f_coeffs.shape, device=device), 2, rounding_mode='trunc')
-        center = torch.tensor(center, device=device)
+        center = torch.tensor(f_coeffs.shape, device=device) // 2
 
         conv_idx_y = torch.arange(-ff_y + 1, ff_y, 1, device=device)
         conv_idx_y = circulant(conv_idx_y, device=device)
         conv_i = conv_idx_y.repeat_interleave(ff_x, dim=1)
         conv_i = conv_i.repeat_interleave(ff_x, dim=0)
 
         conv_idx_x = torch.arange(-ff_x + 1, ff_x, 1, device=device)
@@ -160,47 +199,142 @@
         o_e_conv = o_f_coeffs[center[0] + conv_i, center[1] + conv_j]
 
         e_conv_all[i] = e_conv
         o_e_conv_all[i] = o_e_conv
     return e_conv_all, o_e_conv_all
 
 
-def to_conv_mat_continuous(ucell, fourier_order_x, fourier_order_y, device=torch.device('cpu'),
-                           type_complex=torch.complex128):
+# def fs_rectangle(cx, cy, lx, ly, pmtvy, fourier_order, period):
+#     Px, Py = period
+#     fourier_x, fourier_y = fourier_order
+#     Nx_vector = torch.arange(-2 * fourier_x, 2 * fourier_x + 1, 1).type(torch.complex128)
+#     Ny_vector = torch.arange(-2 * fourier_y, 2 * fourier_y + 1, 1).type(torch.complex128)
+#
+#     # Nx_vector = torch.arange(-fourier_x, fourier_x + 1, 1).type(torch.complex128) * torch.cos(torch.tensor(torch.pi/4))
+#     # Ny_vector = torch.arange(-fourier_y, fourier_y + 1, 1).type(torch.complex128) * torch.sin(torch.tensor(torch.pi/4))
+#
+#     # c = n_index * lx * ly / Px / Py * torch.sinc(torch.pi * ly / Py * Ny_vector.reshape((-1, 1))) @ torch.sinc(torch.pi * lx / Px * Nx_vector.reshape((1, -1)))
+#     c = pmtvy * lx * ly / Px / Py * torch.sinc(ly / Py * Ny_vector.reshape((-1, 1))) @ torch.sinc(
+#         lx / Px * Nx_vector.reshape((1, -1)))
+#
+#     # c = c * (torch.exp(-1j * 2 * torch.pi * cy / Py * Ny_vector.reshape((-1, 1))) @ torch.exp(-1j * 2 * torch.pi * cx / Px * Nx_vector.reshape((1, -1))))
+#     c = c * (torch.exp(-1j * 2 * torch.pi * cy / Py * Ny_vector.reshape((-1, 1))) @ torch.exp(
+#         -1j * 2 * torch.pi * cx / Px * Nx_vector.reshape((1, -1))))
+#
+#     return c.T
+#
+#
+# def to_conv_mat_continuous_vector_sinc(ucell_info_list, fourier_order_x, fourier_order_y, device=torch.device('cpu'),
+#                                   type_complex=torch.complex128):
+#     ff_x = 2 * fourier_order_x + 1
+#     ff_y = 2 * fourier_order_y + 1
+#
+#     e_conv_all = torch.zeros((len(ucell_info_list), ff_x * ff_y, ff_x * ff_y)).type(type_complex)
+#     o_e_conv_all = torch.zeros((len(ucell_info_list), ff_x * ff_y, ff_x * ff_y)).type(type_complex)
+#
+#     # 2D
+#     for i, ucell_info in enumerate(ucell_info_list):
+#         ucell_layer, x_list, y_list = ucell_info
+#         ucell_layer = ucell_layer ** 2
+#         # ucell_layer = torch.tensor(ucell_layer, dtype=type_complex) if type(ucell_layer) != torch.Tensor else ucell_layer
+#         # x_list = torch.tensor(x_list, dtype=type_complex) if type(x_list) != torch.Tensor else x_list
+#         # y_list = torch.tensor(y_list, dtype=type_complex) if type(y_list) != torch.Tensor else y_list
+#
+#         f_coeffs = fft_piecewise_constant_vector(ucell_layer, x_list, y_list,
+#                                                  fourier_order_x, fourier_order_y, type_complex=type_complex)
+#         o_f_coeffs = fft_piecewise_constant_vector(1/ucell_layer, x_list, y_list,
+#                                                  fourier_order_x, fourier_order_y, type_complex=type_complex)
+#
+#         import seaborn as sns
+#         import matplotlib.pyplot as plt
+#         sns.heatmap(f_coeffs.detach().real)
+#         plt.show()
+#         sns.heatmap(o_f_coeffs.detach().real)
+#         plt.show()
+#
+#         sns.heatmap(f_coeffs.detach().imag)
+#         plt.show()
+#         sns.heatmap(o_f_coeffs.detach().imag)
+#         plt.show()
+#
+#         # f_coeffs = fs_rectangle()
+#
+#
+#         center = torch.tensor(f_coeffs.shape, device=device) // 2
+#         # center = torch.div(torch.tensor(f_coeffs.shape, device=device), 2, rounding_mode='trunc')
+#         # center = torch.tensor(center, device=device)
+#
+#         conv_idx_y = torch.arange(-ff_y + 1, ff_y, 1, device=device)
+#         conv_idx_y = circulant(conv_idx_y, device=device)
+#         conv_i = conv_idx_y.repeat_interleave(ff_x, dim=1)
+#         conv_i = conv_i.repeat_interleave(ff_x, dim=0)
+#
+#         conv_idx_x = torch.arange(-ff_x + 1, ff_x, 1, device=device)
+#         conv_idx_x = circulant(conv_idx_x, device=device)
+#         conv_j = conv_idx_x.repeat(ff_y, ff_y)
+#
+#         e_conv = f_coeffs[center[0] + conv_i, center[1] + conv_j]
+#         o_e_conv = o_f_coeffs[center[0] + conv_i, center[1] + conv_j]
+#
+#         e_conv_all[i] = e_conv
+#         o_e_conv_all[i] = o_e_conv
+#     return e_conv_all, o_e_conv_all
+
+
+def to_conv_mat_raster_continuous(ucell, fourier_order_x, fourier_order_y, device=torch.device('cpu'),
+                                  type_complex=torch.complex128):
     ucell_pmt = ucell ** 2
 
     if ucell_pmt.shape[1] == 1:  # 1D
         ff = 2 * fourier_order_x + 1
 
         e_conv_all = torch.zeros((ucell_pmt.shape[0], ff, ff), device=device).type(type_complex)
         o_e_conv_all = torch.zeros((ucell_pmt.shape[0], ff, ff), device=device).type(type_complex)
 
         for i, layer in enumerate(ucell_pmt):
-            f_coeffs = fft_piecewise_constant(layer, fourier_order_x, fourier_order_y, device=device, type_complex=type_complex)
-            o_f_coeffs = fft_piecewise_constant(1/layer, fourier_order_x, fourier_order_y, device=device, type_complex=type_complex)
-            center = torch.div(torch.tensor(f_coeffs.shape, device=device), 2, rounding_mode='trunc')
-            center = torch.tensor(center, device=device)
+
+            cell, x, y = cell_compression(layer, device=device, type_complex=type_complex)
+
+            # f_coeffs = fft_piecewise_constant(layer, fourier_order_x, fourier_order_y, device=device, type_complex=type_complex)
+            # o_f_coeffs = fft_piecewise_constant(1/layer, fourier_order_x, fourier_order_y, device=device, type_complex=type_complex)
+
+            f_coeffs = fft_piecewise_constant(cell, x, y, fourier_order_x, fourier_order_y, device=device, type_complex=type_complex)
+            o_f_coeffs = fft_piecewise_constant(1 / cell, x, y, fourier_order_x, fourier_order_y, device=device, type_complex=type_complex)
+
+
+            center = torch.tensor(f_coeffs.shape, device=device) // 2
+            # center = torch.div(torch.tensor(f_coeffs.shape, device=device), 2, rounding_mode='trunc')
+            # center = torch.tensor(center, device=device)
             conv_idx = torch.arange(-ff + 1, ff, 1, device=device)
             conv_idx = circulant(conv_idx, device=device)
             e_conv = f_coeffs[center[0], center[1] + conv_idx]
             o_e_conv = o_f_coeffs[center[0], center[1] + conv_idx]
             e_conv_all[i] = e_conv
             o_e_conv_all[i] = o_e_conv
     else:  # 2D
         ff_x = 2 * fourier_order_x + 1
         ff_y = 2 * fourier_order_y + 1
 
         e_conv_all = torch.zeros((ucell_pmt.shape[0], ff_x * ff_y,  ff_x * ff_y), device=device).type(type_complex)
         o_e_conv_all = torch.zeros((ucell_pmt.shape[0], ff_x * ff_y,  ff_x * ff_y), device=device).type(type_complex)
 
         for i, layer in enumerate(ucell_pmt):
-            f_coeffs = fft_piecewise_constant(layer, fourier_order_x, fourier_order_y, device=device, type_complex=type_complex)
-            o_f_coeffs = fft_piecewise_constant(1/layer, fourier_order_x, fourier_order_y, device=device, type_complex=type_complex)
-            center = torch.div(torch.tensor(f_coeffs.shape, device=device), 2, rounding_mode='trunc')
-            center = torch.tensor(center, device=device)
+            cell, x, y = cell_compression(layer, device=device, type_complex=type_complex)
+
+            # f_coeffs = fft_piecewise_constant(layer, fourier_order_x, fourier_order_y, device=device, type_complex=type_complex)
+            # o_f_coeffs = fft_piecewise_constant(1/layer, fourier_order_x, fourier_order_y, device=device, type_complex=type_complex)
+
+            f_coeffs = fft_piecewise_constant(cell, x, y, fourier_order_x, fourier_order_y, device=device,
+                                              type_complex=type_complex)
+            o_f_coeffs = fft_piecewise_constant(1 / cell, x, y, fourier_order_x, fourier_order_y, device=device,
+                                                type_complex=type_complex)
+
+            center = torch.tensor(f_coeffs.shape, device=device) // 2
+            # center = torch.div(torch.tensor(f_coeffs.shape, device=device), 2, rounding_mode='trunc')
+            # center = torch.tensor(center, device=device)
 
             conv_idx_y = torch.arange(-ff_y + 1, ff_y, 1, device=device)
             conv_idx_y = circulant(conv_idx_y, device=device)
             conv_i = conv_idx_y.repeat_interleave(ff_x, dim=1)
             conv_i = conv_i.repeat_interleave(ff_x, dim=0)
 
             conv_idx_x = torch.arange(-ff_x + 1, ff_x, 1, device=device)
@@ -210,16 +344,16 @@
             e_conv = f_coeffs[center[0] + conv_i, center[1] + conv_j]
             o_e_conv = o_f_coeffs[center[0] + conv_i, center[1] + conv_j]
             e_conv_all[i] = e_conv
             o_e_conv_all[i] = o_e_conv
     return e_conv_all, o_e_conv_all
 
 
-def to_conv_mat_discrete(ucell, fourier_order_x, fourier_order_y, device=torch.device('cpu'), type_complex=torch.complex128,
-                         improve_dft=True):
+def to_conv_mat_raster_discrete(ucell, fourier_order_x, fourier_order_y, device=torch.device('cpu'), type_complex=torch.complex128,
+                                improve_dft=True):
     ucell_pmt = ucell ** 2
 
     if ucell_pmt.shape[1] == 1:  # 1D
         ff = 2 * fourier_order_x + 1
         e_conv_all = torch.zeros((ucell_pmt.shape[0], ff, ff), device=device).type(type_complex)
         o_e_conv_all = torch.zeros((ucell_pmt.shape[0], ff, ff), device=device).type(type_complex)
         if improve_dft:
@@ -228,16 +362,17 @@
             minimum_pattern_size = 2 * ff
 
         for i, layer in enumerate(ucell_pmt):
             n = minimum_pattern_size // layer.shape[1]
             layer = layer.repeat_interleave(n + 1, axis=1)
             f_coeffs = torch.fft.fftshift(torch.fft.fft(layer / layer.numel()))
             o_f_coeffs = torch.fft.fftshift(torch.fft.fft(1/layer / layer.numel()))
-            center = torch.div(torch.tensor(f_coeffs.shape, device=device), 2, rounding_mode='trunc')
-            center = torch.tensor(center, device=device)
+            center = torch.tensor(f_coeffs.shape, device=device) // 2
+            # center = torch.div(torch.tensor(f_coeffs.shape, device=device), 2, rounding_mode='trunc')
+            # center = torch.tensor(center, device=device)
             conv_idx = torch.arange(-ff + 1, ff, 1, device=device)
             conv_idx = circulant(conv_idx, device=device)
             e_conv = f_coeffs[center[0], center[1] + conv_idx]
             o_e_conv = o_f_coeffs[center[0], center[1] + conv_idx]
             e_conv_all[i] = e_conv
             o_e_conv_all[i] = o_e_conv
 
@@ -254,26 +389,30 @@
         else:
             minimum_pattern_size_y = 2 * ff_y
             minimum_pattern_size_x = 2 * ff_x
         # e.g., 8 bytes * (40*500) * (40*500) / 1E6 = 3200 MB = 3.2 GB
 
         for i, layer in enumerate(ucell_pmt):
             if layer.shape[0] < minimum_pattern_size_y:
-                n = torch.div(minimum_pattern_size_y, layer.shape[0], rounding_mode='trunc')
+                # n = torch.div(minimum_pattern_size_y, layer.shape[0], rounding_mode='trunc')
+                n = minimum_pattern_size_y // layer.shape[0]
                 n = torch.tensor(n, device=device)
+
                 layer = layer.repeat_interleave(n + 1, axis=0)
             if layer.shape[1] < minimum_pattern_size_x:
-                n = torch.div(minimum_pattern_size_x, layer.shape[1], rounding_mode='trunc')
+                # n = torch.div(minimum_pattern_size_x, layer.shape[1], rounding_mode='trunc')
+                n = minimum_pattern_size_x // layer.shape[1]
                 n = torch.tensor(n, device=device)
                 layer = layer.repeat_interleave(n + 1, axis=1)
 
             f_coeffs = torch.fft.fftshift(torch.fft.fft2(layer / layer.numel()))
             o_f_coeffs = torch.fft.fftshift(torch.fft.fft2(1/layer / layer.numel()))
-            center = torch.div(torch.tensor(f_coeffs.shape, device=device), 2, rounding_mode='trunc')
-            center = torch.tensor(center, device=device)
+            center = torch.tensor(f_coeffs.shape, device=device) // 2
+            # center = torch.div(torch.tensor(f_coeffs.shape, device=device), 2, rounding_mode='trunc')
+            # center = torch.tensor(center, device=device)
 
             conv_idx_y = torch.arange(-ff_y + 1, ff_y, 1, device=device)
             conv_idx_y = circulant(conv_idx_y, device=device)
             conv_i = conv_idx_y.repeat_interleave(ff_x, dim=1)
             conv_i = conv_i.repeat_interleave(ff_x, dim=0)
 
             conv_idx_x = torch.arange(-ff_x + 1, ff_x, 1, device=device)
```

### Comparing `meent-0.9.2/meent/on_torch/emsolver/field_distribution.py` & `meent-0.9.3/meent/on_torch/emsolver/field_distribution.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.2/meent/on_torch/emsolver/primitives.py` & `meent-0.9.3/meent/on_torch/emsolver/primitives.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.2/meent/on_torch/emsolver/rcwa.py` & `meent-0.9.3/meent/on_torch/emsolver/rcwa.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import time
 import torch
 
 import numpy as np
 
 from ._base import _BaseRCWA
-from .convolution_matrix import to_conv_mat_discrete, to_conv_mat_continuous, to_conv_mat_continuous_vector
+from .convolution_matrix import to_conv_mat_raster_discrete, to_conv_mat_raster_continuous, to_conv_mat_vector
 from .field_distribution import field_dist_1d_vanilla, field_dist_2d_vanilla, field_plot, field_dist_1d_conical_vanilla, \
     field_dist_1d_vectorized_ji, field_dist_1d_vectorized_kji, field_dist_1d_conical_vectorized_ji, \
     field_dist_1d_conical_vectorized_kji, field_dist_2d_vectorized_ji, field_dist_2d_vectorized_kji
 
 
 class RCWATorch(_BaseRCWA):
     def __init__(self,
@@ -100,24 +100,25 @@
 
         return de_ri, de_ti
 
     def conv_solve(self, **kwargs):
         [setattr(self, k, v) for k, v in kwargs.items()]  # needed for optimization
 
         if self.fft_type == 0:
-            E_conv_all, o_E_conv_all = to_conv_mat_discrete(self.ucell, self.fourier_order[0], self.fourier_order[1],
-                                                            device=self.device, type_complex=self.type_complex,
-                                                            improve_dft=self.improve_dft)
+            E_conv_all, o_E_conv_all = to_conv_mat_raster_discrete(self.ucell, self.fourier_order[0], self.fourier_order[1],
+                                                                   device=self.device, type_complex=self.type_complex,
+                                                                   improve_dft=self.improve_dft)
         elif self.fft_type == 1:
-            E_conv_all, o_E_conv_all = to_conv_mat_continuous(self.ucell, self.fourier_order[0], self.fourier_order[1],
-                                                              device=self.device, type_complex=self.type_complex)
+            E_conv_all, o_E_conv_all = to_conv_mat_raster_continuous(self.ucell, self.fourier_order[0], self.fourier_order[1],
+                                                                     device=self.device, type_complex=self.type_complex)
         elif self.fft_type == 2:
-            E_conv_all, o_E_conv_all = to_conv_mat_continuous_vector(self.ucell_info_list, self.fourier_order[0],
-                                                                     self.fourier_order[1],
-                                                                     type_complex=self.type_complex)
+            E_conv_all, o_E_conv_all = to_conv_mat_vector(self.ucell_info_list, self.fourier_order[0],
+                                                          self.fourier_order[1],
+                                                          type_complex=self.type_complex)
+
         else:
             raise ValueError
 
         de_ri, de_ti, layer_info_list, T1, kx_vector = self._solve(self.wavelength, E_conv_all, o_E_conv_all)
 
         self.layer_info_list = layer_info_list
         self.T1 = T1
```

### Comparing `meent-0.9.2/meent/on_torch/emsolver/scattering_method.py` & `meent-0.9.3/meent/on_torch/emsolver/scattering_method.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.2/meent/on_torch/emsolver/smm_util.py` & `meent-0.9.3/meent/on_torch/emsolver/smm_util.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.2/meent/on_torch/emsolver/transfer_method.py` & `meent-0.9.3/meent/on_torch/emsolver/transfer_method.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.2/meent/on_torch/optimizer/loss.py` & `meent-0.9.3/meent/on_torch/optimizer/loss.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.2/meent/on_torch/optimizer/optimizer.py` & `meent-0.9.3/meent/on_torch/optimizer/optimizer.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.2/meent.egg-info/SOURCES.txt` & `meent-0.9.3/meent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meent-0.9.2/setup.py` & `meent-0.9.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,15 +8,15 @@
             ],
     'pytorch': ['torch>=2.0.0',
                 'tqdm>=4.64.1',
                 ],
 }
 setup(
     name='meent',
-    version='0.9.2',
+    version='0.9.3',
     url='https://github.com/kc-ml2/meent',
     author='KC ML2',
     author_email='yongha@kc-ml2.com',
     packages=['meent'] + find_packages(include=['meent.*']),
     install_requires=[
         'numpy>=1.23.3',
         'scipy>=1.9.1',
```

