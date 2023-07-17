# Comparing `tmp/reservoirpy-0.3.8.tar.gz` & `tmp/reservoirpy-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reservoirpy-0.3.8.tar", last modified: Wed May 31 15:20:58 2023, max compression
+gzip compressed data, was "reservoirpy-0.3.9.tar", last modified: Mon Jul 17 10:03:38 2023, max compression
```

## Comparing `reservoirpy-0.3.8.tar` & `reservoirpy-0.3.9.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-05-31 15:20:58.217360 reservoirpy-0.3.8/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     1066 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/LICENSE
--rw-rw-r--   0 nathan    (1000) nathan    (1000)    12580 2023-05-31 15:20:58.217360 reservoirpy-0.3.8/PKG-INFO
--rw-rw-r--   0 nathan    (1000) nathan    (1000)    10961 2023-05-31 15:17:28.000000 reservoirpy-0.3.8/README.md
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      217 2023-03-20 16:00:23.000000 reservoirpy-0.3.8/pyproject.toml
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-05-31 15:20:58.209360 reservoirpy-0.3.8/reservoirpy/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      888 2023-03-17 08:49:21.000000 reservoirpy-0.3.8/reservoirpy/__init__.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)    24076 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/_base.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)       22 2023-05-31 15:17:28.000000 reservoirpy-0.3.8/reservoirpy/_version.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     3923 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/activationsfunc.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-05-31 15:20:58.209360 reservoirpy-0.3.8/reservoirpy/compat/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     5647 2023-03-17 08:48:30.000000 reservoirpy-0.3.8/reservoirpy/compat/__init__.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)    25130 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/compat/_base.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)    10288 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/compat/_esn.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)    17763 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/compat/_esn_online.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     7950 2023-03-17 08:48:30.000000 reservoirpy-0.3.8/reservoirpy/compat/regression_models.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-05-31 15:20:58.209360 reservoirpy-0.3.8/reservoirpy/compat/tests/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)       40 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/compat/tests/__init__.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     7040 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/compat/tests/test_esn.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     2288 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/compat/tests/test_esnonline.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     2301 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/compat/tests/test_load_from_previous_versions.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     2434 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/compat/tests/test_regression_models.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     3573 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/compat/tests/test_validation.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-05-31 15:20:58.213360 reservoirpy-0.3.8/reservoirpy/compat/utils/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)        0 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/compat/utils/__init__.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     4650 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/compat/utils/parallel.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     5534 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/compat/utils/save.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     6591 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/compat/utils/validation.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-05-31 15:20:58.213360 reservoirpy-0.3.8/reservoirpy/datasets/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     9167 2023-03-17 08:49:20.000000 reservoirpy-0.3.8/reservoirpy/datasets/__init__.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)    26022 2023-03-20 16:00:23.000000 reservoirpy-0.3.8/reservoirpy/datasets/_chaos.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     5451 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/datasets/_japanese_vowels.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      832 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/datasets/_seed.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      515 2023-03-17 08:48:30.000000 reservoirpy-0.3.8/reservoirpy/datasets/_utils.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-05-31 15:20:58.213360 reservoirpy-0.3.8/reservoirpy/datasets/tests/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)        0 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/datasets/tests/__init__.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     3958 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/datasets/tests/test_datasets.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-05-31 15:20:58.213360 reservoirpy-0.3.8/reservoirpy/experimental/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     1078 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/experimental/__init__.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     1658 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/experimental/add.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     3381 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/experimental/batchforce.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-05-31 15:20:58.213360 reservoirpy-0.3.8/reservoirpy/experimental/gpu/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)        0 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/experimental/gpu/__init__.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     1149 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/experimental/norm.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      937 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/experimental/randomchoice.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     1106 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/experimental/sklearn.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-05-31 15:20:58.213360 reservoirpy-0.3.8/reservoirpy/experimental/tests/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)       48 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/experimental/tests/__init__.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-05-31 15:20:58.213360 reservoirpy-0.3.8/reservoirpy/hyper/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      746 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/hyper/__init__.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)    11789 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/hyper/_hyperplot.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     6067 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/hyper/_hypersearch.py
--rwxrwxr-x   0 nathan    (1000) nathan    (1000)    32665 2023-05-31 15:17:24.000000 reservoirpy-0.3.8/reservoirpy/mat_gen.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)    38076 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/model.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)    40127 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/node.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-05-31 15:20:58.213360 reservoirpy-0.3.8/reservoirpy/nodes/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     2553 2023-03-17 08:49:21.000000 reservoirpy-0.3.8/reservoirpy/nodes/__init__.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     6113 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/nodes/activations.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     1963 2023-03-17 08:49:21.000000 reservoirpy-0.3.8/reservoirpy/nodes/concat.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)    12376 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/nodes/esn.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     2794 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/nodes/io.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-05-31 15:20:58.213360 reservoirpy-0.3.8/reservoirpy/nodes/readouts/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      136 2023-03-17 08:49:21.000000 reservoirpy-0.3.8/reservoirpy/nodes/readouts/__init__.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     3349 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/nodes/readouts/base.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     5785 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/nodes/readouts/force.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     4797 2023-03-17 08:49:21.000000 reservoirpy-0.3.8/reservoirpy/nodes/readouts/lms.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     6012 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/nodes/readouts/ridge.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     4437 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/nodes/readouts/rls.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-05-31 15:20:58.217360 reservoirpy-0.3.8/reservoirpy/nodes/reservoirs/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      299 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/nodes/reservoirs/__init__.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     8535 2023-05-31 15:17:28.000000 reservoirpy-0.3.8/reservoirpy/nodes/reservoirs/base.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)    18731 2023-05-31 15:17:28.000000 reservoirpy-0.3.8/reservoirpy/nodes/reservoirs/intrinsic_plasticity.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     6370 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/nodes/reservoirs/nvar.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)    14032 2023-05-31 15:17:28.000000 reservoirpy-0.3.8/reservoirpy/nodes/reservoirs/reservoir.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-05-31 15:20:58.217360 reservoirpy-0.3.8/reservoirpy/nodes/tests/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)       48 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/nodes/tests/__init__.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      493 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/nodes/tests/test_activations.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     1013 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/nodes/tests/test_concat.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     3706 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/nodes/tests/test_esn.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     5804 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/nodes/tests/test_force.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     2000 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/nodes/tests/test_intrinsic_plasticity.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      720 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/nodes/tests/test_io.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     3945 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/nodes/tests/test_lms.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     1053 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/nodes/tests/test_nvar.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     6889 2023-05-31 15:17:28.000000 reservoirpy-0.3.8/reservoirpy/nodes/tests/test_reservoir.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     3220 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/nodes/tests/test_ridge.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     4419 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/nodes/tests/test_rls.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     6038 2023-03-17 08:49:20.000000 reservoirpy-0.3.8/reservoirpy/observables.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)    13703 2023-04-15 10:20:03.000000 reservoirpy-0.3.8/reservoirpy/ops.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-05-31 15:20:58.217360 reservoirpy-0.3.8/reservoirpy/tests/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)       44 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/tests/__init__.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     8546 2023-03-17 08:48:30.000000 reservoirpy-0.3.8/reservoirpy/tests/dummy_nodes.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     2070 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/tests/test_activationsfunc.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)    10705 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/tests/test_base.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)    15591 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/tests/test_mat_gen.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)    14441 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/tests/test_model.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)    11827 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/tests/test_node.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     1819 2023-03-17 08:49:20.000000 reservoirpy-0.3.8/reservoirpy/tests/test_observables.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     2690 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/tests/test_ops.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     2398 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/type.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-05-31 15:20:58.217360 reservoirpy-0.3.8/reservoirpy/utils/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     1005 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/utils/__init__.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     8919 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/utils/graphflow.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     5618 2023-03-17 18:09:50.000000 reservoirpy-0.3.8/reservoirpy/utils/model_utils.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     2412 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/utils/parallel.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     2104 2023-03-20 16:00:23.000000 reservoirpy-0.3.8/reservoirpy/utils/random.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-05-31 15:20:58.217360 reservoirpy-0.3.8/reservoirpy/utils/tests/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)        0 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/utils/tests/__init__.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     1202 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/utils/tests/test_random.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     1417 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/utils/tests/test_utils.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     4891 2023-03-17 08:48:30.000000 reservoirpy-0.3.8/reservoirpy/utils/validation.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-05-31 15:20:58.209360 reservoirpy-0.3.8/reservoirpy.egg-info/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)    12580 2023-05-31 15:20:58.000000 reservoirpy-0.3.8/reservoirpy.egg-info/PKG-INFO
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     3313 2023-05-31 15:20:58.000000 reservoirpy-0.3.8/reservoirpy.egg-info/SOURCES.txt
--rw-rw-r--   0 nathan    (1000) nathan    (1000)        1 2023-05-31 15:20:58.000000 reservoirpy-0.3.8/reservoirpy.egg-info/dependency_links.txt
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      130 2023-05-31 15:20:58.000000 reservoirpy-0.3.8/reservoirpy.egg-info/requires.txt
--rw-rw-r--   0 nathan    (1000) nathan    (1000)       12 2023-05-31 15:20:58.000000 reservoirpy-0.3.8/reservoirpy.egg-info/top_level.txt
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      522 2023-05-31 15:20:58.217360 reservoirpy-0.3.8/setup.cfg
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     2633 2023-03-17 08:49:21.000000 reservoirpy-0.3.8/setup.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-17 10:03:38.491980 reservoirpy-0.3.9/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     1066 2023-02-05 11:29:19.000000 reservoirpy-0.3.9/LICENSE
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)    12580 2023-07-17 10:03:38.495980 reservoirpy-0.3.9/PKG-INFO
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)    10961 2023-07-17 09:42:22.000000 reservoirpy-0.3.9/README.md
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      217 2023-03-20 16:00:23.000000 reservoirpy-0.3.9/pyproject.toml
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-17 10:03:38.487980 reservoirpy-0.3.9/reservoirpy/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      888 2023-03-17 08:49:21.000000 reservoirpy-0.3.9/reservoirpy/__init__.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)    24076 2023-07-17 08:05:40.000000 reservoirpy-0.3.9/reservoirpy/_base.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)       22 2023-07-17 09:42:13.000000 reservoirpy-0.3.9/reservoirpy/_version.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     3923 2023-02-05 11:29:19.000000 reservoirpy-0.3.9/reservoirpy/activationsfunc.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-17 10:03:38.487980 reservoirpy-0.3.9/reservoirpy/compat/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     5647 2023-03-17 08:48:30.000000 reservoirpy-0.3.9/reservoirpy/compat/__init__.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)    25130 2023-07-17 08:05:40.000000 reservoirpy-0.3.9/reservoirpy/compat/_base.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)    10288 2023-02-05 11:29:19.000000 reservoirpy-0.3.9/reservoirpy/compat/_esn.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)    17763 2023-07-17 08:05:40.000000 reservoirpy-0.3.9/reservoirpy/compat/_esn_online.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     7950 2023-03-17 08:48:30.000000 reservoirpy-0.3.9/reservoirpy/compat/regression_models.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-17 10:03:38.487980 reservoirpy-0.3.9/reservoirpy/compat/tests/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)       40 2023-02-05 11:29:19.000000 reservoirpy-0.3.9/reservoirpy/compat/tests/__init__.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     7040 2023-07-17 08:05:40.000000 reservoirpy-0.3.9/reservoirpy/compat/tests/test_esn.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     2288 2023-02-05 11:29:19.000000 reservoirpy-0.3.9/reservoirpy/compat/tests/test_esnonline.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     2301 2023-07-17 08:05:40.000000 reservoirpy-0.3.9/reservoirpy/compat/tests/test_load_from_previous_versions.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     2434 2023-02-05 11:29:19.000000 reservoirpy-0.3.9/reservoirpy/compat/tests/test_regression_models.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     3573 2023-02-05 11:29:19.000000 reservoirpy-0.3.9/reservoirpy/compat/tests/test_validation.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-17 10:03:38.487980 reservoirpy-0.3.9/reservoirpy/compat/utils/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)        0 2023-02-05 11:29:19.000000 reservoirpy-0.3.9/reservoirpy/compat/utils/__init__.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     4650 2023-07-17 08:05:40.000000 reservoirpy-0.3.9/reservoirpy/compat/utils/parallel.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     5534 2023-07-17 08:05:40.000000 reservoirpy-0.3.9/reservoirpy/compat/utils/save.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     6591 2023-02-05 11:29:19.000000 reservoirpy-0.3.9/reservoirpy/compat/utils/validation.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-17 10:03:38.487980 reservoirpy-0.3.9/reservoirpy/datasets/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     9167 2023-03-17 08:49:20.000000 reservoirpy-0.3.9/reservoirpy/datasets/__init__.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)    26180 2023-07-17 08:37:53.000000 reservoirpy-0.3.9/reservoirpy/datasets/_chaos.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     5297 2023-07-17 09:34:23.000000 reservoirpy-0.3.9/reservoirpy/datasets/_japanese_vowels.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      832 2023-02-05 11:29:19.000000 reservoirpy-0.3.9/reservoirpy/datasets/_seed.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      515 2023-03-17 08:48:30.000000 reservoirpy-0.3.9/reservoirpy/datasets/_utils.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-17 10:03:38.487980 reservoirpy-0.3.9/reservoirpy/datasets/tests/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)        0 2023-02-05 11:29:19.000000 reservoirpy-0.3.9/reservoirpy/datasets/tests/__init__.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     3969 2023-07-17 08:45:22.000000 reservoirpy-0.3.9/reservoirpy/datasets/tests/test_datasets.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-17 10:03:38.487980 reservoirpy-0.3.9/reservoirpy/experimental/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     1078 2023-02-05 11:29:19.000000 reservoirpy-0.3.9/reservoirpy/experimental/__init__.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     1658 2023-02-05 11:29:19.000000 reservoirpy-0.3.9/reservoirpy/experimental/add.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     3381 2023-07-17 08:05:40.000000 reservoirpy-0.3.9/reservoirpy/experimental/batchforce.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-17 10:03:38.487980 reservoirpy-0.3.9/reservoirpy/experimental/gpu/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)        0 2023-02-05 11:29:19.000000 reservoirpy-0.3.9/reservoirpy/experimental/gpu/__init__.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     1149 2023-02-05 11:29:19.000000 reservoirpy-0.3.9/reservoirpy/experimental/norm.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      937 2023-02-05 11:29:19.000000 reservoirpy-0.3.9/reservoirpy/experimental/randomchoice.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     1106 2023-02-05 11:29:19.000000 reservoirpy-0.3.9/reservoirpy/experimental/sklearn.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-17 10:03:38.487980 reservoirpy-0.3.9/reservoirpy/experimental/tests/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)       48 2023-02-05 11:29:19.000000 reservoirpy-0.3.9/reservoirpy/experimental/tests/__init__.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-17 10:03:38.487980 reservoirpy-0.3.9/reservoirpy/hyper/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      746 2023-02-05 11:29:19.000000 reservoirpy-0.3.9/reservoirpy/hyper/__init__.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)    11789 2023-07-17 08:05:40.000000 reservoirpy-0.3.9/reservoirpy/hyper/_hyperplot.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     6067 2023-07-17 08:05:40.000000 reservoirpy-0.3.9/reservoirpy/hyper/_hypersearch.py
+-rwxrwxr-x   0 nathan    (1000) nathan    (1000)    32665 2023-07-17 08:05:40.000000 reservoirpy-0.3.9/reservoirpy/mat_gen.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)    38076 2023-07-17 08:05:40.000000 reservoirpy-0.3.9/reservoirpy/model.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)    40127 2023-07-17 08:05:40.000000 reservoirpy-0.3.9/reservoirpy/node.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-17 10:03:38.491980 reservoirpy-0.3.9/reservoirpy/nodes/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     2553 2023-03-17 08:49:21.000000 reservoirpy-0.3.9/reservoirpy/nodes/__init__.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     6113 2023-02-05 11:29:19.000000 reservoirpy-0.3.9/reservoirpy/nodes/activations.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     1963 2023-03-17 08:49:21.000000 reservoirpy-0.3.9/reservoirpy/nodes/concat.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)    12066 2023-07-17 09:58:39.000000 reservoirpy-0.3.9/reservoirpy/nodes/esn.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     2794 2023-02-05 11:29:19.000000 reservoirpy-0.3.9/reservoirpy/nodes/io.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-17 10:03:38.491980 reservoirpy-0.3.9/reservoirpy/nodes/readouts/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      136 2023-03-17 08:49:21.000000 reservoirpy-0.3.9/reservoirpy/nodes/readouts/__init__.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     3349 2023-07-17 08:05:40.000000 reservoirpy-0.3.9/reservoirpy/nodes/readouts/base.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     5785 2023-07-17 08:05:40.000000 reservoirpy-0.3.9/reservoirpy/nodes/readouts/force.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     4797 2023-03-17 08:49:21.000000 reservoirpy-0.3.9/reservoirpy/nodes/readouts/lms.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     6012 2023-07-17 08:05:40.000000 reservoirpy-0.3.9/reservoirpy/nodes/readouts/ridge.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     4437 2023-07-17 08:05:40.000000 reservoirpy-0.3.9/reservoirpy/nodes/readouts/rls.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-17 10:03:38.491980 reservoirpy-0.3.9/reservoirpy/nodes/reservoirs/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      299 2023-02-05 11:29:19.000000 reservoirpy-0.3.9/reservoirpy/nodes/reservoirs/__init__.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     8535 2023-07-17 08:05:40.000000 reservoirpy-0.3.9/reservoirpy/nodes/reservoirs/base.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)    18731 2023-07-17 08:05:40.000000 reservoirpy-0.3.9/reservoirpy/nodes/reservoirs/intrinsic_plasticity.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     6370 2023-02-05 11:29:19.000000 reservoirpy-0.3.9/reservoirpy/nodes/reservoirs/nvar.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)    14033 2023-07-17 09:23:32.000000 reservoirpy-0.3.9/reservoirpy/nodes/reservoirs/reservoir.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-17 10:03:38.491980 reservoirpy-0.3.9/reservoirpy/nodes/tests/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)       48 2023-02-05 11:29:19.000000 reservoirpy-0.3.9/reservoirpy/nodes/tests/__init__.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      493 2023-02-05 11:29:19.000000 reservoirpy-0.3.9/reservoirpy/nodes/tests/test_activations.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     1013 2023-07-17 08:05:40.000000 reservoirpy-0.3.9/reservoirpy/nodes/tests/test_concat.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     3792 2023-07-17 09:57:21.000000 reservoirpy-0.3.9/reservoirpy/nodes/tests/test_esn.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     5804 2023-07-17 08:05:40.000000 reservoirpy-0.3.9/reservoirpy/nodes/tests/test_force.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     2000 2023-07-17 08:05:40.000000 reservoirpy-0.3.9/reservoirpy/nodes/tests/test_intrinsic_plasticity.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      720 2023-02-05 11:29:19.000000 reservoirpy-0.3.9/reservoirpy/nodes/tests/test_io.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     3945 2023-07-17 08:05:40.000000 reservoirpy-0.3.9/reservoirpy/nodes/tests/test_lms.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     1053 2023-07-17 08:05:40.000000 reservoirpy-0.3.9/reservoirpy/nodes/tests/test_nvar.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     6889 2023-07-17 08:05:40.000000 reservoirpy-0.3.9/reservoirpy/nodes/tests/test_reservoir.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     3220 2023-07-17 08:05:40.000000 reservoirpy-0.3.9/reservoirpy/nodes/tests/test_ridge.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     4419 2023-07-17 08:05:40.000000 reservoirpy-0.3.9/reservoirpy/nodes/tests/test_rls.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     6071 2023-07-17 08:09:45.000000 reservoirpy-0.3.9/reservoirpy/observables.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)    13703 2023-04-15 10:20:03.000000 reservoirpy-0.3.9/reservoirpy/ops.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-17 10:03:38.491980 reservoirpy-0.3.9/reservoirpy/tests/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)       44 2023-02-05 11:29:19.000000 reservoirpy-0.3.9/reservoirpy/tests/__init__.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     8546 2023-03-17 08:48:30.000000 reservoirpy-0.3.9/reservoirpy/tests/dummy_nodes.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     2070 2023-02-05 11:29:19.000000 reservoirpy-0.3.9/reservoirpy/tests/test_activationsfunc.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)    10705 2023-07-17 08:05:40.000000 reservoirpy-0.3.9/reservoirpy/tests/test_base.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)    15591 2023-07-17 08:05:40.000000 reservoirpy-0.3.9/reservoirpy/tests/test_mat_gen.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)    14441 2023-07-17 08:05:40.000000 reservoirpy-0.3.9/reservoirpy/tests/test_model.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)    11827 2023-07-17 08:05:40.000000 reservoirpy-0.3.9/reservoirpy/tests/test_node.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     1819 2023-03-17 08:49:20.000000 reservoirpy-0.3.9/reservoirpy/tests/test_observables.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     2690 2023-07-17 08:05:40.000000 reservoirpy-0.3.9/reservoirpy/tests/test_ops.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     2398 2023-02-05 11:29:19.000000 reservoirpy-0.3.9/reservoirpy/type.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-17 10:03:38.491980 reservoirpy-0.3.9/reservoirpy/utils/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     1005 2023-02-05 11:29:19.000000 reservoirpy-0.3.9/reservoirpy/utils/__init__.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     9115 2023-07-17 08:09:45.000000 reservoirpy-0.3.9/reservoirpy/utils/graphflow.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     5618 2023-03-17 18:09:50.000000 reservoirpy-0.3.9/reservoirpy/utils/model_utils.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     2412 2023-07-17 08:05:40.000000 reservoirpy-0.3.9/reservoirpy/utils/parallel.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     2104 2023-03-20 16:00:23.000000 reservoirpy-0.3.9/reservoirpy/utils/random.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-17 10:03:38.491980 reservoirpy-0.3.9/reservoirpy/utils/tests/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)        0 2023-02-05 11:29:19.000000 reservoirpy-0.3.9/reservoirpy/utils/tests/__init__.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     1202 2023-07-17 08:05:40.000000 reservoirpy-0.3.9/reservoirpy/utils/tests/test_random.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     1417 2023-07-17 08:05:40.000000 reservoirpy-0.3.9/reservoirpy/utils/tests/test_utils.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     4891 2023-03-17 08:48:30.000000 reservoirpy-0.3.9/reservoirpy/utils/validation.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-17 10:03:38.487980 reservoirpy-0.3.9/reservoirpy.egg-info/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)    12580 2023-07-17 10:03:38.000000 reservoirpy-0.3.9/reservoirpy.egg-info/PKG-INFO
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     3313 2023-07-17 10:03:38.000000 reservoirpy-0.3.9/reservoirpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)        1 2023-07-17 10:03:38.000000 reservoirpy-0.3.9/reservoirpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      130 2023-07-17 10:03:38.000000 reservoirpy-0.3.9/reservoirpy.egg-info/requires.txt
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)       12 2023-07-17 10:03:38.000000 reservoirpy-0.3.9/reservoirpy.egg-info/top_level.txt
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      522 2023-07-17 10:03:38.495980 reservoirpy-0.3.9/setup.cfg
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     2633 2023-07-17 09:31:47.000000 reservoirpy-0.3.9/setup.py
```

### Comparing `reservoirpy-0.3.8/LICENSE` & `reservoirpy-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/PKG-INFO` & `reservoirpy-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: reservoirpy
-Version: 0.3.8
+Version: 0.3.9
 Summary: A simple and flexible code for Reservoir Computing architectures like Echo State Networks.
 Home-page: https://github.com/reservoirpy/reservoirpy
-Download-URL: https://github.com/reservoirpy/reservoirpy/v0.3.8.tar.gz
+Download-URL: https://github.com/reservoirpy/reservoirpy/v0.3.9.tar.gz
 Author: Xavier Hinaut
 Author-email: xavier.hinaut@inria.fr
 Maintainer: Xavier Hinaut, Nathan Trouvain
 Maintainer-email: xavier.hinaut@inria.fr, nathan.trouvain@inria.fr
 Project-URL: Bug Tracker, https://github.com/reservoirpy/reservoirpy/issues
 Project-URL: Documentation, https://reservoirpy.readthedocs.io/en/latest/index.html
 Project-URL: Source Code, https://github.com/reservoirpy/reservoirpy
@@ -40,15 +40,15 @@
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/reservoirpy)
 [![PyPI version](https://badge.fury.io/py/reservoirpy.svg)](https://badge.fury.io/py/reservoirpy)
 [![Documentation Status](https://readthedocs.org/projects/reservoirpy/badge/?version=latest)](https://reservoirpy.readthedocs.io/en/latest/?badge=latest)
 [![Testing](https://github.com/reservoirpy/reservoirpy/actions/workflows/test.yml/badge.svg?branch=master)](https://github.com/reservoirpy/reservoirpy/actions/workflows/test.yml)
 [![codecov](https://codecov.io/gh/reservoirpy/reservoirpy/branch/master/graph/badge.svg?token=JC8R1PB5EO)](https://codecov.io/gh/reservoirpy/reservoirpy)
 
-# ReservoirPy (v0.3.8) 🌀🧠
+# ReservoirPy (v0.3.9) 🌀🧠
 **Simple and flexible code for Reservoir Computing architectures like Echo State Networks (ESN).**
 
 [![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/reservoirpy/reservoirpy/HEAD)
 
 ```python
 from reservoirpy.nodes import Reservoir, Ridge, Input
```

### Comparing `reservoirpy-0.3.8/README.md` & `reservoirpy-0.3.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/reservoirpy)
 [![PyPI version](https://badge.fury.io/py/reservoirpy.svg)](https://badge.fury.io/py/reservoirpy)
 [![Documentation Status](https://readthedocs.org/projects/reservoirpy/badge/?version=latest)](https://reservoirpy.readthedocs.io/en/latest/?badge=latest)
 [![Testing](https://github.com/reservoirpy/reservoirpy/actions/workflows/test.yml/badge.svg?branch=master)](https://github.com/reservoirpy/reservoirpy/actions/workflows/test.yml)
 [![codecov](https://codecov.io/gh/reservoirpy/reservoirpy/branch/master/graph/badge.svg?token=JC8R1PB5EO)](https://codecov.io/gh/reservoirpy/reservoirpy)
 
-# ReservoirPy (v0.3.8) 🌀🧠
+# ReservoirPy (v0.3.9) 🌀🧠
 **Simple and flexible code for Reservoir Computing architectures like Echo State Networks (ESN).**
 
 [![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/reservoirpy/reservoirpy/HEAD)
 
 ```python
 from reservoirpy.nodes import Reservoir, Ridge, Input
```

### Comparing `reservoirpy-0.3.8/reservoirpy/__init__.py` & `reservoirpy-0.3.9/reservoirpy/__init__.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/_base.py` & `reservoirpy-0.3.9/reservoirpy/_base.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/activationsfunc.py` & `reservoirpy-0.3.9/reservoirpy/activationsfunc.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/compat/__init__.py` & `reservoirpy-0.3.9/reservoirpy/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/compat/_base.py` & `reservoirpy-0.3.9/reservoirpy/compat/_base.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/compat/_esn.py` & `reservoirpy-0.3.9/reservoirpy/compat/_esn.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/compat/_esn_online.py` & `reservoirpy-0.3.9/reservoirpy/compat/_esn_online.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/compat/regression_models.py` & `reservoirpy-0.3.9/reservoirpy/compat/regression_models.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/compat/tests/test_esn.py` & `reservoirpy-0.3.9/reservoirpy/compat/tests/test_esn.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/compat/tests/test_esnonline.py` & `reservoirpy-0.3.9/reservoirpy/compat/tests/test_esnonline.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/compat/tests/test_load_from_previous_versions.py` & `reservoirpy-0.3.9/reservoirpy/compat/tests/test_load_from_previous_versions.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/compat/tests/test_regression_models.py` & `reservoirpy-0.3.9/reservoirpy/compat/tests/test_regression_models.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/compat/tests/test_validation.py` & `reservoirpy-0.3.9/reservoirpy/compat/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/compat/utils/parallel.py` & `reservoirpy-0.3.9/reservoirpy/compat/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/compat/utils/save.py` & `reservoirpy-0.3.9/reservoirpy/compat/utils/save.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/compat/utils/validation.py` & `reservoirpy-0.3.9/reservoirpy/compat/utils/validation.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/datasets/__init__.py` & `reservoirpy-0.3.9/reservoirpy/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/datasets/_chaos.py` & `reservoirpy-0.3.9/reservoirpy/datasets/_chaos.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 
 
 def henon_map(
     n_timesteps: int,
     a: float = 1.4,
     b: float = 0.3,
     x0: Union[list, np.ndarray] = [0.0, 0.0],
+    **kwargs,
 ) -> np.ndarray:
     """Hénon map discrete timeseries [2]_ [3]_.
 
     .. math::
 
         x(n+1) &= 1 - ax(n)^2 + y(n)\\\\
         y(n+1) &= bx(n)
@@ -84,15 +85,15 @@
     for i in range(1, n_timesteps):
         states[i][0] = 1 - a * states[i - 1][0] ** 2 + states[i - 1][1]
         states[i][1] = b * states[i - 1][0]
 
     return states
 
 
-def logistic_map(n_timesteps: int, r: float = 3.9, x0: float = 0.5) -> np.ndarray:
+def logistic_map(n_timesteps: int, r: float = 3.9, x0: float = 0.5, **kwargs) -> np.ndarray:
     """Logistic map discrete timeseries [4]_ [5]_.
 
     .. math::
 
         x(n+1) = rx(n)(1-x(n))
 
     Parameters
@@ -183,32 +184,35 @@
            on Wikipedia.
     """
 
     def lorenz_diff(t, state):
         x, y, z = state
         return sigma * (y - x), x * (rho - z) - y, x * y - beta * z
 
-    t_eval = np.arange(0.0, n_timesteps * h, h)
+    t_max = n_timesteps * h
+
+    t_eval = np.linspace(0.0, t_max, n_timesteps)
 
     sol = solve_ivp(
-        lorenz_diff, y0=x0, t_span=(0.0, n_timesteps * h), t_eval=t_eval, **kwargs
+        lorenz_diff, y0=x0, t_span=(0.0, t_max), t_eval=t_eval, **kwargs
     )
 
     return sol.y.T
 
 
 def mackey_glass(
     n_timesteps: int,
     tau: int = 17,
     a: float = 0.2,
     b: float = 0.1,
     n: int = 10,
     x0: float = 1.2,
     h: float = 1.0,
     seed: Union[int, RandomState, Generator] = None,
+    **kwargs,
 ) -> np.ndarray:
     """Mackey-Glass timeseries [8]_ [9]_, computed from the Mackey-Glass
     delayed differential equation.
 
     .. math::
 
         \\frac{x}{t} = \\frac{ax(t-\\tau)}{1+x(t-\\tau)^n} - bx(t)
@@ -301,14 +305,15 @@
 def multiscroll(
     n_timesteps: int,
     a: float = 40.0,
     b: float = 3.0,
     c: float = 28.0,
     x0: Union[list, np.ndarray] = [-0.1, 0.5, -0.6],
     h: float = 0.01,
+    **kwargs,
 ) -> np.ndarray:
     """Double scroll attractor timeseries [10]_ [11]_,
     a particular case of multiscroll attractor timeseries.
 
     .. math::
 
         \\frac{\\mathrm{d}x}{\\mathrm{d}t} &= a(y - x) \\\\
@@ -351,21 +356,23 @@
     def multiscroll_diff(t, state):
         x, y, z = state
         dx = a * (y - x)
         dy = (c - a) * x - x * z + c * y
         dz = x * y - b * z
         return dx, dy, dz
 
-    t = np.arange(0.0, n_timesteps * h, h)
+    t_max = n_timesteps * h
+
+    t_eval = np.linspace(0.0, t_max, n_timesteps)
 
     sol = solve_ivp(
-        multiscroll_diff, y0=x0, t_span=(0.0, n_timesteps * h), dense_output=True
+        multiscroll_diff, y0=x0, t_span=(0.0, t_max), t_eval=t_eval, **kwargs
     )
 
-    return sol.sol(t).T
+    return sol.y.T
 
 
 def doublescroll(
     n_timesteps: int,
     r1: float = 1.2,
     r2: float = 3.44,
     r4: float = 0.193,
@@ -419,29 +426,31 @@
 
     .. [11] `Chen double scroll attractor
            <https://en.wikipedia.org/wiki/Multiscroll_attractor
            #Chen_attractor>`_
            on Wikipedia.
     """
 
-    def doublescroll(t, state):
+    def doublescroll_diff(t, state):
         V1, V2, i = state
 
         dV = V1 - V2
         factor = (dV / r2) + ir * np.sinh(beta * dV)
         dV1 = (V1 / r1) - factor
         dV2 = factor - i
         dI = V2 - r4 * i
 
         return dV1, dV2, dI
 
-    t_eval = np.arange(0.0, n_timesteps * h, h)
+    t_max = n_timesteps * h
+
+    t_eval = np.linspace(0.0, t_max, n_timesteps)
 
     sol = solve_ivp(
-        doublescroll, y0=x0, t_span=(0.0, n_timesteps * h), t_eval=t_eval, **kwargs
+        doublescroll_diff, y0=x0, t_span=(0.0, t_max), t_eval=t_eval, **kwargs
     )
 
     return sol.y.T
 
 
 def rabinovich_fabrikant(
     n_timesteps: int,
@@ -496,22 +505,20 @@
     def rabinovich_fabrikant_diff(t, state):
         x, y, z = state
         dx = y * (z - 1 + x**2) + gamma * x
         dy = x * (3 * z + 1 - x**2) + gamma * y
         dz = -2 * z * (alpha + x * y)
         return dx, dy, dz
 
-    t_eval = np.arange(0.0, n_timesteps * h, h)
+    t_max = n_timesteps * h
+
+    t_eval = np.linspace(0.0, t_max, n_timesteps)
 
     sol = solve_ivp(
-        rabinovich_fabrikant_diff,
-        y0=x0,
-        t_span=(0.0, n_timesteps * h),
-        t_eval=t_eval,
-        **kwargs,
+        rabinovich_fabrikant_diff, y0=x0, t_span=(0.0, t_max), t_eval=t_eval, **kwargs
     )
 
     return sol.y.T
 
 
 def narma(
     n_timesteps: int,
@@ -661,20 +668,22 @@
 
     def lorenz96_diff(t, state):
         ds = np.zeros(N)
         for i in range(N):
             ds[i] = (state[(i + 1) % N] - state[i - 2]) * state[i - 1] - state[i] + F
         return ds
 
-    t_eval = np.arange(0.0, (warmup + n_timesteps) * h, h)
+    t_max = (warmup + n_timesteps) * h
+
+    t_eval = np.linspace(0.0, t_max * h, n_timesteps)
 
     sol = solve_ivp(
         lorenz96_diff,
         y0=x0,
-        t_span=(0.0, (warmup + n_timesteps) * h),
+        t_span=(0.0, t_max * h),
         t_eval=t_eval,
         **kwargs,
     )
 
     return sol.y.T[warmup:]
 
 
@@ -733,18 +742,20 @@
     def rossler_diff(t, state):
         x, y, z = state
         dx = -y - z
         dy = x + a * y
         dz = b + z * (x - c)
         return dx, dy, dz
 
-    t_eval = np.arange(0.0, n_timesteps * h, h)
+    t_max = n_timesteps * h
+
+    t_eval = np.linspace(0.0, t_max, n_timesteps)
 
     sol = solve_ivp(
-        rossler_diff, y0=x0, t_span=(0.0, n_timesteps * h), t_eval=t_eval, **kwargs
+        rossler_diff, y0=x0, t_span=(0.0, t_max), t_eval=t_eval, **kwargs
     )
 
     return sol.y.T
 
 
 def _kuramoto_sivashinsky_etdrk4(v, *, g, E, E2, Q, f1, f2, f3):
     """A single step of EDTRK4 to solve Kuramoto-Sivashinsky equation.
```

### Comparing `reservoirpy-0.3.8/reservoirpy/datasets/_japanese_vowels.py` & `reservoirpy-0.3.9/reservoirpy/datasets/_japanese_vowels.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """Japanese vowels dataset."""
 # Author: Nathan Trouvain at 07/05/2022 <nathan.trouvain@inria.fr>
 # Licence: MIT License
 # Copyright: Xavier Hinaut (2018) <xavier.hinaut@inria.fr>
-from io import StringIO
-from pathlib import Path
+import io
+import zipfile
 from urllib.request import urlopen
 
-import joblib
 import numpy as np
 
 from .. import logger
 from ._utils import _get_data_folder
 
 SOURCE_URL = (
-    "https://archive.ics.uci.edu/ml/machine-learning-databases/JapaneseVowels-mld/"
+    "https://archive.ics.uci.edu/static/public/128/japanese+vowels.zip"
 )
 
 REMOTE_FILES = {
     "DESCR": "JapaneseVowels.data.html",
     "train": "ae.train",
     "test": "ae.test",
     "train_sizes": "size_ae.train",
@@ -27,63 +26,49 @@
 # class labels
 SPEAKERS = ["1", "2", "3", "4", "5", "6", "7", "8", "9"]
 
 ONE_HOT_SPEAKERS = np.eye(9)
 
 
 def _format_data(data, block_numbers, one_hot_encode):
-    """Load and parse data from downloaded binary files."""
+    """Load and parse data from downloaded files."""
 
     X = []
     Y = []
 
-    data = data.decode("utf-8").split("\n\n")[:-1]
+    data = data.split("\n\n")[:-1]
 
     block_cursor = 0
     speaker_cursor = 0
     for block in data:
 
         if block_cursor >= block_numbers[speaker_cursor]:
             block_cursor = 0
             speaker_cursor += 1
 
-        X.append(np.loadtxt(StringIO(block)))
+        X.append(np.loadtxt(io.StringIO(block)))
 
         if one_hot_encode:
             Y.append(ONE_HOT_SPEAKERS[speaker_cursor].reshape(1, -1))
         else:
             Y.append(np.array([SPEAKERS[speaker_cursor]]).reshape(1, 1))
 
         block_cursor += 1
 
     return X, Y
 
 
-def _download(data_folder, file_name, file_role):  # pragma: no cover
+def _download(data_folder):  # pragma: no cover
     """Download data from source into the reservoirpy data local directory."""
 
-    logger.info(f"Downloading {SOURCE_URL + file_name}.")
+    logger.info(f"Downloading {SOURCE_URL}.")
 
-    file_path = Path(file_name)
-
-    with urlopen(SOURCE_URL + file_name) as f:
-
-        # extract data block sizes integer lists
-        if file_role in ["train_sizes", "test_sizes"]:
-            data = [s for s in f.read().decode("utf-8").split(" ")]
-
-            # remove empty characters and spaces
-            data = [int(s) for s in filter(lambda s: s not in ["", "\n", " "], data)]
-
-        else:
-            data = f.read()
-
-        joblib.dump(data, data_folder / file_path, compress=6)
-
-    return data
+    with urlopen(SOURCE_URL) as zipresp:
+        with zipfile.ZipFile(io.BytesIO(zipresp.read())) as zfile:
+            zfile.extractall(data_folder)
 
 
 def _repeat_target(blocks, targets):
     """Repeat target label/vector along block's time axis."""
 
     repeated_targets = []
     for block, target in zip(blocks, targets):
@@ -113,15 +98,15 @@
     Samples per class (testing)     29-50 series of 7-29 timesteps
     Samples total                                              640
     Dimensionality                                              12
     Features                                                  real
     ============================   ===============================
 
     Data is downloaded from:
-    https://archive.ics.uci.edu/ml/machine-learning-databases/JapaneseVowels-mld/
+    https://doi.org/10.24432/C5NS47
 
     Parameters
     ----------
     one_hot_encode : bool, default to True
         If True, returns class label as a one-hot encoded vector.
     repeat_targets : bool, default to False
         If True, repeat the target label or vector along the time axis of the
@@ -144,22 +129,38 @@
            "Multidimensional Curve Classification Using Passing-Through Regions".
            Pattern Recognition Letters, Vol. 20, No. 11--13, pages 1103--1111.
 
     """
 
     data_folder = _get_data_folder(data_folder)
 
+    complete = True
+    for file_role, file_name in REMOTE_FILES.items():
+        if not (data_folder / file_name).exists():
+            complete = False
+            break
+
+    if reload or not complete:
+        _download(data_folder)
+
     data_files = {}
     for file_role, file_name in REMOTE_FILES.items():
-        file_path = Path(file_name)
 
-        if not (data_folder / file_path).exists() or reload:  # pragma: no cover
-            data_files[file_role] = _download(data_folder, file_name, file_role)
-        else:
-            data_files[file_role] = joblib.load(data_folder / file_path)
+        with open(data_folder / file_name, "r") as fp:
+
+            if file_role in ["train_sizes", "test_sizes"]:
+                data = fp.read().split(" ")
+                # remove empty characters and spaces
+                data = [int(s) for s in filter(lambda s: s not in ["", "\n", " "],
+                data)]
+
+            else:
+                data = fp.read()
+
+        data_files[file_role] = data
 
     X_train, Y_train = _format_data(
         data_files["train"], data_files["train_sizes"], one_hot_encode
     )
 
     X_test, Y_test = _format_data(
         data_files["test"], data_files["test_sizes"], one_hot_encode
```

### Comparing `reservoirpy-0.3.8/reservoirpy/datasets/_seed.py` & `reservoirpy-0.3.9/reservoirpy/datasets/_seed.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/datasets/_utils.py` & `reservoirpy-0.3.9/reservoirpy/datasets/_utils.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/datasets/tests/test_datasets.py` & `reservoirpy-0.3.9/reservoirpy/datasets/tests/test_datasets.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
     assert y.shape[0] == 200 - 5 - 10
     assert x.shape[0] == y.shape[0]
     assert xt.shape[0] == yt.shape[0] == 10
 
 
 def test_japanese_vowels():
 
-    X, Y, X_test, Y_test = datasets.japanese_vowels()
+    X, Y, X_test, Y_test = datasets.japanese_vowels(reload=True)
 
     assert len(X) == 270 == len(Y)
     assert len(X_test) == 370 == len(Y_test)
 
     assert Y[0].shape == (1, 9)
 
     X, Y, X_test, Y_test = datasets.japanese_vowels(repeat_targets=True)
```

### Comparing `reservoirpy-0.3.8/reservoirpy/experimental/__init__.py` & `reservoirpy-0.3.9/reservoirpy/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/experimental/add.py` & `reservoirpy-0.3.9/reservoirpy/experimental/add.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/experimental/batchforce.py` & `reservoirpy-0.3.9/reservoirpy/experimental/batchforce.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/experimental/norm.py` & `reservoirpy-0.3.9/reservoirpy/experimental/norm.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/experimental/randomchoice.py` & `reservoirpy-0.3.9/reservoirpy/experimental/randomchoice.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/experimental/sklearn.py` & `reservoirpy-0.3.9/reservoirpy/experimental/sklearn.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/hyper/__init__.py` & `reservoirpy-0.3.9/reservoirpy/hyper/__init__.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/hyper/_hyperplot.py` & `reservoirpy-0.3.9/reservoirpy/hyper/_hyperplot.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/hyper/_hypersearch.py` & `reservoirpy-0.3.9/reservoirpy/hyper/_hypersearch.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/mat_gen.py` & `reservoirpy-0.3.9/reservoirpy/mat_gen.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/model.py` & `reservoirpy-0.3.9/reservoirpy/model.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/node.py` & `reservoirpy-0.3.9/reservoirpy/node.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/nodes/__init__.py` & `reservoirpy-0.3.9/reservoirpy/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/nodes/activations.py` & `reservoirpy-0.3.9/reservoirpy/nodes/activations.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/nodes/concat.py` & `reservoirpy-0.3.9/reservoirpy/nodes/concat.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/nodes/esn.py` & `reservoirpy-0.3.9/reservoirpy/nodes/esn.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,28 @@
 from .reservoirs import NVAR, Reservoir
 
 _LEARNING_METHODS = {"ridge": Ridge}
 
 _RES_METHODS = {"reservoir": Reservoir, "nvar": NVAR}
 
 
+def _run_partial_fit_fn(esn, x, y, lock, warmup):
+    seq_len = len(x[list(x)[0]])
+    states = np.zeros((seq_len, esn.reservoir.output_dim))
+
+    for i, (x, forced_feedback, _) in enumerate(dispatch(x, y, shift_fb=True)):
+        esn._load_proxys()
+
+        with esn.readout.with_feedback(forced_feedback[esn.readout.name]):
+            states[i, :] = call(esn.reservoir, x[esn.reservoir.name])
+
+    esn._clean_proxys()
+    esn.readout.partial_fit(states, y[esn.readout.name], warmup=warmup, lock=lock)
+
+
 def _allocate_returned_states(model, inputs, return_states=None):
     """Create empty placeholders for model outputs."""
     seq_len = inputs[list(inputs.keys())[0]].shape[0]
     vulgar_names = {"reservoir": model.reservoir, "readout": model.readout}
 
     # pre-allocate states
     if return_states == "all":
@@ -316,40 +330,20 @@
             "sequential",
             "threading",
         ):
             lock = Manager().Lock()
         else:
             lock = None
 
-        def run_partial_fit_fn(x, y):
-            seq_len = len(x[list(x)[0]])
-            states = np.zeros((seq_len, self.reservoir.output_dim))
-
-            for i, (x, forced_feedback, _) in enumerate(dispatch(x, y, shift_fb=True)):
-                self._load_proxys()
-
-                with self.readout.with_feedback(forced_feedback[self.readout.name]):
-                    states[i, :] = call(self.reservoir, x[self.reservoir.name])
-
-            self._clean_proxys()
-
-            # Avoid any problem related to multiple
-            # writes from multiple processes
-            # if lock is not None:
-            # with lock:  # pragma: no cover
-            self.readout.partial_fit(states, y[self.readout.name], warmup=warmup, lock=lock)
-            # else:
-            #     self.readout.partial_fit(states, y[self.readout.name])
-
         backend = get_joblib_backend(workers=self.workers, backend=self.backend)
 
         seq = progress(X, f"Running {self.name}")
         with self.with_state(from_state, reset=reset, stateful=stateful):
             with Parallel(n_jobs=self.workers, backend=backend) as parallel:
-                parallel(delayed(run_partial_fit_fn)(x, y) for x, y in zip(seq, Y))
+                parallel(delayed(_run_partial_fit_fn)(self, x, y, lock, warmup) for x, y in zip(seq, Y))
 
             if verbosity():  # pragma: no cover
                 print(f"Fitting node {self.name}...")
 
             self.readout.fit()
 
         return self
```

### Comparing `reservoirpy-0.3.8/reservoirpy/nodes/io.py` & `reservoirpy-0.3.9/reservoirpy/nodes/io.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/nodes/readouts/base.py` & `reservoirpy-0.3.9/reservoirpy/nodes/readouts/base.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/nodes/readouts/force.py` & `reservoirpy-0.3.9/reservoirpy/nodes/readouts/force.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/nodes/readouts/lms.py` & `reservoirpy-0.3.9/reservoirpy/nodes/readouts/lms.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/nodes/readouts/ridge.py` & `reservoirpy-0.3.9/reservoirpy/nodes/readouts/ridge.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/nodes/readouts/rls.py` & `reservoirpy-0.3.9/reservoirpy/nodes/readouts/rls.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/nodes/reservoirs/base.py` & `reservoirpy-0.3.9/reservoirpy/nodes/reservoirs/base.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/nodes/reservoirs/intrinsic_plasticity.py` & `reservoirpy-0.3.9/reservoirpy/nodes/reservoirs/intrinsic_plasticity.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/nodes/reservoirs/nvar.py` & `reservoirpy-0.3.9/reservoirpy/nodes/reservoirs/nvar.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/nodes/reservoirs/reservoir.py` & `reservoirpy-0.3.9/reservoirpy/nodes/reservoirs/reservoir.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
     - **1.** Activation function is part of the neuron internal state
       (equation called ``internal``):
 
     .. math::
 
         \\mathbf{x}[t+1] = (1 - \\mathrm{lr}) * \\mathbf{x}[t] + \\mathrm{lr}
-         * (\\mathbf{W}_{in} \\cdot (\\mathbf{u}[t+1]+c_{in}*\\xi)
+         * f(\\mathbf{W}_{in} \\cdot (\\mathbf{u}[t+1]+c_{in}*\\xi)
           + \\mathbf{W} \\cdot \\mathbf{x}[t]
         + \\mathbf{W}_{fb} \\cdot (g(\\mathbf{y}[t])+c_{fb}*\\xi) + \\mathbf{b})
         + c * \\xi
 
     - **2.** Activation function is applied on emitted internal states
       (equation called ``external``):
```

### Comparing `reservoirpy-0.3.8/reservoirpy/nodes/tests/test_concat.py` & `reservoirpy-0.3.9/reservoirpy/nodes/tests/test_concat.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/nodes/tests/test_esn.py` & `reservoirpy-0.3.9/reservoirpy/nodes/tests/test_esn.py`

 * *Files 8% similar despite different names*

```diff
@@ -91,27 +91,28 @@
     assert esn.reservoir.Win.shape == (100, 10)
     assert esn.readout.Wout.shape == (100, 5)
     assert res.shape == (1, 5)
     assert esn.reservoir.Wfb is not None
     assert esn.reservoir.Wfb.shape == (100, 5)
 
 
-def test_esn_parallel_fit_reproducibility():
+@pytest.mark.parametrize("backend", ("loky", "multiprocessing", "threading"))
+def test_esn_parallel_fit_reproducibility(backend):
 
     for i in range(10):
         set_seed(45)
 
         esn = ESN(
             units=100,
             lr=0.8,
             sr=0.4,
             ridge=1e-5,
             feedback=True,
             workers=-1,
-            backend="loky",
+            backend=backend,
         )
 
         X, Y = np.ones((10, 100, 10)), np.ones((10, 100, 5))
         esn.fit(X, Y)
 
         assert esn.reservoir.W.shape == (100, 100)
         assert esn.reservoir.Win.shape == (100, 10)
```

### Comparing `reservoirpy-0.3.8/reservoirpy/nodes/tests/test_force.py` & `reservoirpy-0.3.9/reservoirpy/nodes/tests/test_force.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/nodes/tests/test_intrinsic_plasticity.py` & `reservoirpy-0.3.9/reservoirpy/nodes/tests/test_intrinsic_plasticity.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/nodes/tests/test_io.py` & `reservoirpy-0.3.9/reservoirpy/nodes/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/nodes/tests/test_lms.py` & `reservoirpy-0.3.9/reservoirpy/nodes/tests/test_lms.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/nodes/tests/test_nvar.py` & `reservoirpy-0.3.9/reservoirpy/nodes/tests/test_nvar.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/nodes/tests/test_reservoir.py` & `reservoirpy-0.3.9/reservoirpy/nodes/tests/test_reservoir.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/nodes/tests/test_ridge.py` & `reservoirpy-0.3.9/reservoirpy/nodes/tests/test_ridge.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/nodes/tests/test_rls.py` & `reservoirpy-0.3.9/reservoirpy/nodes/tests/test_rls.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/observables.py` & `reservoirpy-0.3.9/reservoirpy/observables.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         time.
     """
     if issparse(W):
         if maxiter is None:
             maxiter = W.shape[0] * 20
 
         return max(
-            abs(eigs(W, k=1, which="LM", maxiter=maxiter, return_eigenvectors=False))
+            abs(eigs(W, k=1, which="LM", maxiter=maxiter, return_eigenvectors=False, v0=np.ones(W.shape[0], W.dtype)))
         )
 
     return max(abs(linalg.eig(W)[0]))
 
 
 def mse(y_true: np.ndarray, y_pred: np.ndarray) -> float:
     """Mean squared error metric:
@@ -214,9 +214,9 @@
     -------
     float
         Coefficient of determination.
     """
     y_true_array, y_pred_array = _check_arrays(y_true, y_pred)
 
     d = (y_true_array - y_pred_array) ** 2
-    D = (y_true_array - y_pred_array.mean()) ** 2
+    D = (y_true_array - y_true_array.mean()) ** 2
     return 1 - np.sum(d) / np.sum(D)
```

### Comparing `reservoirpy-0.3.8/reservoirpy/ops.py` & `reservoirpy-0.3.9/reservoirpy/ops.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/tests/dummy_nodes.py` & `reservoirpy-0.3.9/reservoirpy/tests/dummy_nodes.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/tests/test_activationsfunc.py` & `reservoirpy-0.3.9/reservoirpy/tests/test_activationsfunc.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/tests/test_base.py` & `reservoirpy-0.3.9/reservoirpy/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/tests/test_mat_gen.py` & `reservoirpy-0.3.9/reservoirpy/tests/test_mat_gen.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/tests/test_model.py` & `reservoirpy-0.3.9/reservoirpy/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/tests/test_node.py` & `reservoirpy-0.3.9/reservoirpy/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/tests/test_observables.py` & `reservoirpy-0.3.9/reservoirpy/tests/test_observables.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/tests/test_ops.py` & `reservoirpy-0.3.9/reservoirpy/tests/test_ops.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/type.py` & `reservoirpy-0.3.9/reservoirpy/type.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/utils/__init__.py` & `reservoirpy-0.3.9/reservoirpy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/utils/graphflow.py` & `reservoirpy-0.3.9/reservoirpy/utils/graphflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 
 
 def find_parents_and_children(edges):
     """Returns two dicts linking nodes to their parents and children in the graph."""
     parents = defaultdict(list)
     children = defaultdict(list)
 
+    # Kludge to always have the parents and children in the same order at every run.
+    # TODO: refactor the graphflow part.
+    edges = sorted(list(edges), key=lambda x: x[0].name + x[1].name)
+
     for edge in edges:
         parent, child = edge
         parents[child] += [parent]
         children[parent] += [child]
 
     return parents, children
```

### Comparing `reservoirpy-0.3.8/reservoirpy/utils/model_utils.py` & `reservoirpy-0.3.9/reservoirpy/utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/utils/parallel.py` & `reservoirpy-0.3.9/reservoirpy/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/utils/random.py` & `reservoirpy-0.3.9/reservoirpy/utils/random.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/utils/tests/test_random.py` & `reservoirpy-0.3.9/reservoirpy/utils/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/utils/tests/test_utils.py` & `reservoirpy-0.3.9/reservoirpy/utils/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy/utils/validation.py` & `reservoirpy-0.3.9/reservoirpy/utils/validation.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/reservoirpy.egg-info/PKG-INFO` & `reservoirpy-0.3.9/reservoirpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: reservoirpy
-Version: 0.3.8
+Version: 0.3.9
 Summary: A simple and flexible code for Reservoir Computing architectures like Echo State Networks.
 Home-page: https://github.com/reservoirpy/reservoirpy
-Download-URL: https://github.com/reservoirpy/reservoirpy/v0.3.8.tar.gz
+Download-URL: https://github.com/reservoirpy/reservoirpy/v0.3.9.tar.gz
 Author: Xavier Hinaut
 Author-email: xavier.hinaut@inria.fr
 Maintainer: Xavier Hinaut, Nathan Trouvain
 Maintainer-email: xavier.hinaut@inria.fr, nathan.trouvain@inria.fr
 Project-URL: Bug Tracker, https://github.com/reservoirpy/reservoirpy/issues
 Project-URL: Documentation, https://reservoirpy.readthedocs.io/en/latest/index.html
 Project-URL: Source Code, https://github.com/reservoirpy/reservoirpy
@@ -40,15 +40,15 @@
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/reservoirpy)
 [![PyPI version](https://badge.fury.io/py/reservoirpy.svg)](https://badge.fury.io/py/reservoirpy)
 [![Documentation Status](https://readthedocs.org/projects/reservoirpy/badge/?version=latest)](https://reservoirpy.readthedocs.io/en/latest/?badge=latest)
 [![Testing](https://github.com/reservoirpy/reservoirpy/actions/workflows/test.yml/badge.svg?branch=master)](https://github.com/reservoirpy/reservoirpy/actions/workflows/test.yml)
 [![codecov](https://codecov.io/gh/reservoirpy/reservoirpy/branch/master/graph/badge.svg?token=JC8R1PB5EO)](https://codecov.io/gh/reservoirpy/reservoirpy)
 
-# ReservoirPy (v0.3.8) 🌀🧠
+# ReservoirPy (v0.3.9) 🌀🧠
 **Simple and flexible code for Reservoir Computing architectures like Echo State Networks (ESN).**
 
 [![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/reservoirpy/reservoirpy/HEAD)
 
 ```python
 from reservoirpy.nodes import Reservoir, Ridge, Input
```

### Comparing `reservoirpy-0.3.8/reservoirpy.egg-info/SOURCES.txt` & `reservoirpy-0.3.9/reservoirpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/setup.cfg` & `reservoirpy-0.3.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.8/setup.py` & `reservoirpy-0.3.9/setup.py`

 * *Files identical despite different names*

