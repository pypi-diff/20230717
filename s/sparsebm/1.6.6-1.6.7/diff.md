# Comparing `tmp/sparsebm-1.6.6.tar.gz` & `tmp/sparsebm-1.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparsebm-1.6.6.tar", last modified: Mon Apr  3 19:08:39 2023, max compression
+gzip compressed data, was "sparsebm-1.6.7.tar", last modified: Mon Jul 17 13:49:14 2023, max compression
```

## Comparing `sparsebm-1.6.6.tar` & `sparsebm-1.6.7.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 19:08:39.602751 sparsebm-1.6.6/
--rw-rw-rw-   0 root         (0) root         (0)       88 2023-04-03 19:08:27.000000 sparsebm-1.6.6/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1264 2023-04-03 19:08:27.000000 sparsebm-1.6.6/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      540 2023-04-03 19:08:27.000000 sparsebm-1.6.6/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1249 2023-04-03 19:08:27.000000 sparsebm-1.6.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5326 2023-04-03 19:08:39.601751 sparsebm-1.6.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4313 2023-04-03 19:08:27.000000 sparsebm-1.6.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 19:08:39.581749 sparsebm-1.6.6/doc/
--rw-rw-rw-   0 root         (0) root         (0)      609 2023-04-03 19:08:27.000000 sparsebm-1.6.6/doc/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 19:08:39.587750 sparsebm-1.6.6/doc/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 19:08:39.587750 sparsebm-1.6.6/doc/source/_static/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-03 19:08:27.000000 sparsebm-1.6.6/doc/source/_static/.keep
--rw-rw-rw-   0 root         (0) root         (0)      107 2023-04-03 19:08:27.000000 sparsebm-1.6.6/doc/source/cari.rst
--rw-rw-rw-   0 root         (0) root         (0)      100 2023-04-03 19:08:27.000000 sparsebm-1.6.6/doc/source/class-description.rst
--rw-rw-rw-   0 root         (0) root         (0)      162 2023-04-03 19:08:27.000000 sparsebm-1.6.6/doc/source/cli-sparsebm.rst
--rw-rw-rw-   0 root         (0) root         (0)     6422 2023-04-03 19:08:27.000000 sparsebm-1.6.6/doc/source/conf.py
--rw-rw-rw-   0 root         (0) root         (0)       43 2023-04-03 19:08:27.000000 sparsebm-1.6.6/doc/source/experiments.rst
--rw-rw-rw-   0 root         (0) root         (0)       31 2023-04-03 19:08:27.000000 sparsebm-1.6.6/doc/source/getting-started.rst
--rw-rw-rw-   0 root         (0) root         (0)      674 2023-04-03 19:08:27.000000 sparsebm-1.6.6/doc/source/graph-gen-lbm.rst
--rw-rw-rw-   0 root         (0) root         (0)      740 2023-04-03 19:08:27.000000 sparsebm-1.6.6/doc/source/graph-gen-sbm.rst
--rw-rw-rw-   0 root         (0) root         (0)      107 2023-04-03 19:08:27.000000 sparsebm-1.6.6/doc/source/helper-functions.rst
--rw-rw-rw-   0 root         (0) root         (0)      261 2023-04-03 19:08:27.000000 sparsebm-1.6.6/doc/source/index.rst
--rw-rw-rw-   0 root         (0) root         (0)    43274 2023-04-03 19:08:27.000000 sparsebm-1.6.6/doc/source/lbm.png
--rw-rw-rw-   0 root         (0) root         (0)      394 2023-04-03 19:08:27.000000 sparsebm-1.6.6/doc/source/lbm.rst
--rw-rw-rw-   0 root         (0) root         (0)      935 2023-04-03 19:08:27.000000 sparsebm-1.6.6/doc/source/model-selection.rst
--rw-rw-rw-   0 root         (0) root         (0)    42028 2023-04-03 19:08:27.000000 sparsebm-1.6.6/doc/source/sbm.png
--rw-rw-rw-   0 root         (0) root         (0)     1369 2023-04-03 19:08:27.000000 sparsebm-1.6.6/doc/source/sbm.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 19:08:39.590750 sparsebm-1.6.6/examples/
--rw-rw-rw-   0 root         (0) root         (0)     1107 2023-04-03 19:08:27.000000 sparsebm-1.6.6/examples/README.md
--rw-rw-rw-   0 root         (0) root         (0)      601 2023-04-03 19:08:27.000000 sparsebm-1.6.6/examples/conf_sbm.json
--rw-rw-rw-   0 root         (0) root         (0)     6361 2023-04-03 19:08:27.000000 sparsebm-1.6.6/examples/lbm_in_colab.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     4120 2023-04-03 19:08:27.000000 sparsebm-1.6.6/examples/lbm_model_selection.py
--rw-rw-rw-   0 root         (0) root         (0)     3895 2023-04-03 19:08:27.000000 sparsebm-1.6.6/examples/lbm_random_init.py
--rw-rw-rw-   0 root         (0) root         (0)     5899 2023-04-03 19:08:27.000000 sparsebm-1.6.6/examples/sbm_in_colab.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     3233 2023-04-03 19:08:27.000000 sparsebm-1.6.6/examples/sbm_model_selection.py
--rw-rw-rw-   0 root         (0) root         (0)     3147 2023-04-03 19:08:27.000000 sparsebm-1.6.6/examples/sbm_random_init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 19:08:39.594750 sparsebm-1.6.6/experiments/
--rw-rw-rw-   0 root         (0) root         (0)     3344 2023-04-03 19:08:27.000000 sparsebm-1.6.6/experiments/README.md
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-03 19:08:27.000000 sparsebm-1.6.6/experiments/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12802 2023-04-03 19:08:27.000000 sparsebm-1.6.6/experiments/benchmark_libraries.py
--rw-rw-rw-   0 root         (0) root         (0)     3611 2023-04-03 19:08:27.000000 sparsebm-1.6.6/experiments/benchmark_libraries_results.py
--rw-rw-rw-   0 root         (0) root         (0)    22870 2023-04-03 19:08:27.000000 sparsebm-1.6.6/experiments/lbm_not_sparse.py
--rw-rw-rw-   0 root         (0) root         (0)     6045 2023-04-03 19:08:27.000000 sparsebm-1.6.6/experiments/sparse_size_fixed.py
--rw-rw-rw-   0 root         (0) root         (0)     2296 2023-04-03 19:08:27.000000 sparsebm-1.6.6/experiments/sparse_size_fixed_generate_data.py
--rw-rw-rw-   0 root         (0) root         (0)     3443 2023-04-03 19:08:27.000000 sparsebm-1.6.6/experiments/sparse_size_fixed_results.py
--rw-rw-rw-   0 root         (0) root         (0)     6807 2023-04-03 19:08:27.000000 sparsebm-1.6.6/experiments/sparse_sparsity_fixed.py
--rw-rw-rw-   0 root         (0) root         (0)     2203 2023-04-03 19:08:27.000000 sparsebm-1.6.6/experiments/sparse_sparsity_fixed_generate_data.py
--rw-rw-rw-   0 root         (0) root         (0)     2837 2023-04-03 19:08:27.000000 sparsebm-1.6.6/experiments/sparse_sparsity_fixed_results.py
--rw-rw-rw-   0 root         (0) root         (0)     1443 2023-04-03 19:08:27.000000 sparsebm-1.6.6/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-03 19:08:39.602751 sparsebm-1.6.6/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 19:08:39.597751 sparsebm-1.6.6/sparsebm/
--rw-rw-rw-   0 root         (0) root         (0)     2261 2023-04-03 19:08:27.000000 sparsebm-1.6.6/sparsebm/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7094 2023-04-03 19:08:27.000000 sparsebm-1.6.6/sparsebm/_datatypes.py
--rw-rw-rw-   0 root         (0) root         (0)    23420 2023-04-03 19:08:27.000000 sparsebm-1.6.6/sparsebm/_entry_point.py
--rw-rw-rw-   0 root         (0) root         (0)    14973 2023-04-03 19:08:27.000000 sparsebm-1.6.6/sparsebm/_graph_generator.py
--rw-rw-rw-   0 root         (0) root         (0)    26564 2023-04-03 19:08:27.000000 sparsebm-1.6.6/sparsebm/_lbm.py
--rw-rw-rw-   0 root         (0) root         (0)    24660 2023-04-03 19:08:27.000000 sparsebm-1.6.6/sparsebm/_model_selection.py
--rw-rw-rw-   0 root         (0) root         (0)    22753 2023-04-03 19:08:27.000000 sparsebm-1.6.6/sparsebm/_sbm.py
--rw-rw-rw-   0 root         (0) root         (0)    19734 2023-04-03 19:08:27.000000 sparsebm-1.6.6/sparsebm/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 19:08:39.599751 sparsebm-1.6.6/sparsebm.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5326 2023-04-03 19:08:39.000000 sparsebm-1.6.6/sparsebm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1576 2023-04-03 19:08:39.000000 sparsebm-1.6.6/sparsebm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-03 19:08:39.000000 sparsebm-1.6.6/sparsebm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2023-04-03 19:08:39.000000 sparsebm-1.6.6/sparsebm.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      162 2023-04-03 19:08:39.000000 sparsebm-1.6.6/sparsebm.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-04-03 19:08:39.000000 sparsebm-1.6.6/sparsebm.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 19:08:39.601751 sparsebm-1.6.6/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-03 19:08:27.000000 sparsebm-1.6.6/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      842 2023-04-03 19:08:27.000000 sparsebm-1.6.6/tests/test_generate_sbm.py
--rw-rw-rw-   0 root         (0) root         (0)     1283 2023-04-03 19:08:27.000000 sparsebm-1.6.6/tests/test_lbm.py
--rw-rw-rw-   0 root         (0) root         (0)     1143 2023-04-03 19:08:27.000000 sparsebm-1.6.6/tests/test_sbm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:49:14.890637 sparsebm-1.6.7/
+-rw-rw-rw-   0 root         (0) root         (0)       88 2023-07-17 13:49:05.000000 sparsebm-1.6.7/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1264 2023-07-17 13:49:05.000000 sparsebm-1.6.7/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      540 2023-07-17 13:49:05.000000 sparsebm-1.6.7/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1249 2023-07-17 13:49:05.000000 sparsebm-1.6.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5326 2023-07-17 13:49:14.890637 sparsebm-1.6.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4313 2023-07-17 13:49:05.000000 sparsebm-1.6.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:49:14.876637 sparsebm-1.6.7/doc/
+-rw-rw-rw-   0 root         (0) root         (0)      609 2023-07-17 13:49:05.000000 sparsebm-1.6.7/doc/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:49:14.880637 sparsebm-1.6.7/doc/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:49:14.880637 sparsebm-1.6.7/doc/source/_static/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-17 13:49:05.000000 sparsebm-1.6.7/doc/source/_static/.keep
+-rw-rw-rw-   0 root         (0) root         (0)      107 2023-07-17 13:49:05.000000 sparsebm-1.6.7/doc/source/cari.rst
+-rw-rw-rw-   0 root         (0) root         (0)      100 2023-07-17 13:49:05.000000 sparsebm-1.6.7/doc/source/class-description.rst
+-rw-rw-rw-   0 root         (0) root         (0)      162 2023-07-17 13:49:05.000000 sparsebm-1.6.7/doc/source/cli-sparsebm.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6422 2023-07-17 13:49:05.000000 sparsebm-1.6.7/doc/source/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)       43 2023-07-17 13:49:05.000000 sparsebm-1.6.7/doc/source/experiments.rst
+-rw-rw-rw-   0 root         (0) root         (0)       31 2023-07-17 13:49:05.000000 sparsebm-1.6.7/doc/source/getting-started.rst
+-rw-rw-rw-   0 root         (0) root         (0)      674 2023-07-17 13:49:05.000000 sparsebm-1.6.7/doc/source/graph-gen-lbm.rst
+-rw-rw-rw-   0 root         (0) root         (0)      740 2023-07-17 13:49:05.000000 sparsebm-1.6.7/doc/source/graph-gen-sbm.rst
+-rw-rw-rw-   0 root         (0) root         (0)      107 2023-07-17 13:49:05.000000 sparsebm-1.6.7/doc/source/helper-functions.rst
+-rw-rw-rw-   0 root         (0) root         (0)      261 2023-07-17 13:49:05.000000 sparsebm-1.6.7/doc/source/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)    43274 2023-07-17 13:49:05.000000 sparsebm-1.6.7/doc/source/lbm.png
+-rw-rw-rw-   0 root         (0) root         (0)      394 2023-07-17 13:49:05.000000 sparsebm-1.6.7/doc/source/lbm.rst
+-rw-rw-rw-   0 root         (0) root         (0)      935 2023-07-17 13:49:05.000000 sparsebm-1.6.7/doc/source/model-selection.rst
+-rw-rw-rw-   0 root         (0) root         (0)    42028 2023-07-17 13:49:05.000000 sparsebm-1.6.7/doc/source/sbm.png
+-rw-rw-rw-   0 root         (0) root         (0)     1369 2023-07-17 13:49:05.000000 sparsebm-1.6.7/doc/source/sbm.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:49:14.882637 sparsebm-1.6.7/examples/
+-rw-rw-rw-   0 root         (0) root         (0)     1107 2023-07-17 13:49:05.000000 sparsebm-1.6.7/examples/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      601 2023-07-17 13:49:05.000000 sparsebm-1.6.7/examples/conf_sbm.json
+-rw-rw-rw-   0 root         (0) root         (0)     9053 2023-07-17 13:49:05.000000 sparsebm-1.6.7/examples/lbm_in_colab.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     4120 2023-07-17 13:49:05.000000 sparsebm-1.6.7/examples/lbm_model_selection.py
+-rw-rw-rw-   0 root         (0) root         (0)     3895 2023-07-17 13:49:05.000000 sparsebm-1.6.7/examples/lbm_random_init.py
+-rw-rw-rw-   0 root         (0) root         (0)     8419 2023-07-17 13:49:05.000000 sparsebm-1.6.7/examples/sbm_in_colab.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     3233 2023-07-17 13:49:05.000000 sparsebm-1.6.7/examples/sbm_model_selection.py
+-rw-rw-rw-   0 root         (0) root         (0)     3147 2023-07-17 13:49:05.000000 sparsebm-1.6.7/examples/sbm_random_init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:49:14.884637 sparsebm-1.6.7/experiments/
+-rw-rw-rw-   0 root         (0) root         (0)     3344 2023-07-17 13:49:05.000000 sparsebm-1.6.7/experiments/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-17 13:49:05.000000 sparsebm-1.6.7/experiments/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12802 2023-07-17 13:49:05.000000 sparsebm-1.6.7/experiments/benchmark_libraries.py
+-rw-rw-rw-   0 root         (0) root         (0)     3611 2023-07-17 13:49:05.000000 sparsebm-1.6.7/experiments/benchmark_libraries_results.py
+-rw-rw-rw-   0 root         (0) root         (0)    22870 2023-07-17 13:49:05.000000 sparsebm-1.6.7/experiments/lbm_not_sparse.py
+-rw-rw-rw-   0 root         (0) root         (0)     6045 2023-07-17 13:49:05.000000 sparsebm-1.6.7/experiments/sparse_size_fixed.py
+-rw-rw-rw-   0 root         (0) root         (0)     2296 2023-07-17 13:49:05.000000 sparsebm-1.6.7/experiments/sparse_size_fixed_generate_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     3443 2023-07-17 13:49:05.000000 sparsebm-1.6.7/experiments/sparse_size_fixed_results.py
+-rw-rw-rw-   0 root         (0) root         (0)     6807 2023-07-17 13:49:05.000000 sparsebm-1.6.7/experiments/sparse_sparsity_fixed.py
+-rw-rw-rw-   0 root         (0) root         (0)     2203 2023-07-17 13:49:05.000000 sparsebm-1.6.7/experiments/sparse_sparsity_fixed_generate_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     2837 2023-07-17 13:49:05.000000 sparsebm-1.6.7/experiments/sparse_sparsity_fixed_results.py
+-rw-rw-rw-   0 root         (0) root         (0)     1454 2023-07-17 13:49:05.000000 sparsebm-1.6.7/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-17 13:49:14.890637 sparsebm-1.6.7/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:49:14.887637 sparsebm-1.6.7/sparsebm/
+-rw-rw-rw-   0 root         (0) root         (0)     2261 2023-07-17 13:49:05.000000 sparsebm-1.6.7/sparsebm/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7094 2023-07-17 13:49:05.000000 sparsebm-1.6.7/sparsebm/_datatypes.py
+-rw-rw-rw-   0 root         (0) root         (0)    23420 2023-07-17 13:49:05.000000 sparsebm-1.6.7/sparsebm/_entry_point.py
+-rw-rw-rw-   0 root         (0) root         (0)    14973 2023-07-17 13:49:05.000000 sparsebm-1.6.7/sparsebm/_graph_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)    26564 2023-07-17 13:49:05.000000 sparsebm-1.6.7/sparsebm/_lbm.py
+-rw-rw-rw-   0 root         (0) root         (0)    24660 2023-07-17 13:49:05.000000 sparsebm-1.6.7/sparsebm/_model_selection.py
+-rw-rw-rw-   0 root         (0) root         (0)    22753 2023-07-17 13:49:05.000000 sparsebm-1.6.7/sparsebm/_sbm.py
+-rw-rw-rw-   0 root         (0) root         (0)    19734 2023-07-17 13:49:05.000000 sparsebm-1.6.7/sparsebm/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:49:14.888637 sparsebm-1.6.7/sparsebm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5326 2023-07-17 13:49:14.000000 sparsebm-1.6.7/sparsebm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1576 2023-07-17 13:49:14.000000 sparsebm-1.6.7/sparsebm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 13:49:14.000000 sparsebm-1.6.7/sparsebm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2023-07-17 13:49:14.000000 sparsebm-1.6.7/sparsebm.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      171 2023-07-17 13:49:14.000000 sparsebm-1.6.7/sparsebm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-17 13:49:14.000000 sparsebm-1.6.7/sparsebm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:49:14.889637 sparsebm-1.6.7/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-17 13:49:05.000000 sparsebm-1.6.7/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      842 2023-07-17 13:49:05.000000 sparsebm-1.6.7/tests/test_generate_sbm.py
+-rw-rw-rw-   0 root         (0) root         (0)     1283 2023-07-17 13:49:05.000000 sparsebm-1.6.7/tests/test_lbm.py
+-rw-rw-rw-   0 root         (0) root         (0)     1143 2023-07-17 13:49:05.000000 sparsebm-1.6.7/tests/test_sbm.py
```

### Comparing `sparsebm-1.6.6/.gitlab-ci.yml` & `sparsebm-1.6.7/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `sparsebm-1.6.6/.pre-commit-config.yaml` & `sparsebm-1.6.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sparsebm-1.6.6/LICENSE` & `sparsebm-1.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sparsebm-1.6.6/PKG-INFO` & `sparsebm-1.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparsebm
-Version: 1.6.6
+Version: 1.6.7
 Summary: An implementation of Stochastic Bloc model and Latent Block model efficient with sparse matrices
 Author-email: Gabriel Frisch <gabriel.frisch@hds.utc.fr>, Jean-Benoist Leger <jbleger@hds.utc.fr>
 Maintainer-email: Jean-Benoist Leger <jbleger@hds.utc.fr>
 License: MIT License
 Project-URL: Repository, https://gitlab.com/jbleger/sparsebm
 Project-URL: Documentation, https://jbleger.gitlab.io/sparsebm
 Keywords: datamining,graph,LBM,SBM,variationnal,sparse
```

### Comparing `sparsebm-1.6.6/README.md` & `sparsebm-1.6.7/README.md`

 * *Files identical despite different names*

### Comparing `sparsebm-1.6.6/doc/Makefile` & `sparsebm-1.6.7/doc/Makefile`

 * *Files identical despite different names*

### Comparing `sparsebm-1.6.6/doc/source/conf.py` & `sparsebm-1.6.7/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `sparsebm-1.6.6/doc/source/graph-gen-lbm.rst` & `sparsebm-1.6.7/doc/source/graph-gen-lbm.rst`

 * *Files identical despite different names*

### Comparing `sparsebm-1.6.6/doc/source/graph-gen-sbm.rst` & `sparsebm-1.6.7/doc/source/graph-gen-sbm.rst`

 * *Files identical despite different names*

### Comparing `sparsebm-1.6.6/doc/source/lbm.png` & `sparsebm-1.6.7/doc/source/lbm.png`

 * *Files identical despite different names*

### Comparing `sparsebm-1.6.6/doc/source/model-selection.rst` & `sparsebm-1.6.7/doc/source/model-selection.rst`

 * *Files identical despite different names*

### Comparing `sparsebm-1.6.6/doc/source/sbm.png` & `sparsebm-1.6.7/doc/source/sbm.png`

 * *Files identical despite different names*

### Comparing `sparsebm-1.6.6/doc/source/sbm.rst` & `sparsebm-1.6.7/doc/source/sbm.rst`

 * *Files identical despite different names*

### Comparing `sparsebm-1.6.6/examples/README.md` & `sparsebm-1.6.7/examples/README.md`

 * *Files identical despite different names*

### Comparing `sparsebm-1.6.6/examples/conf_sbm.json` & `sparsebm-1.6.7/examples/conf_sbm.json`

 * *Files identical despite different names*

### Comparing `sparsebm-1.6.6/examples/lbm_model_selection.py` & `sparsebm-1.6.7/examples/lbm_model_selection.py`

 * *Files identical despite different names*

### Comparing `sparsebm-1.6.6/examples/lbm_random_init.py` & `sparsebm-1.6.7/examples/lbm_random_init.py`

 * *Files identical despite different names*

### Comparing `sparsebm-1.6.6/examples/sbm_model_selection.py` & `sparsebm-1.6.7/examples/sbm_model_selection.py`

 * *Files identical despite different names*

### Comparing `sparsebm-1.6.6/examples/sbm_random_init.py` & `sparsebm-1.6.7/examples/sbm_random_init.py`

 * *Files identical despite different names*

### Comparing `sparsebm-1.6.6/experiments/README.md` & `sparsebm-1.6.7/experiments/README.md`

 * *Files identical despite different names*

### Comparing `sparsebm-1.6.6/experiments/benchmark_libraries.py` & `sparsebm-1.6.7/experiments/benchmark_libraries.py`

 * *Files identical despite different names*

### Comparing `sparsebm-1.6.6/experiments/benchmark_libraries_results.py` & `sparsebm-1.6.7/experiments/benchmark_libraries_results.py`

 * *Files identical despite different names*

### Comparing `sparsebm-1.6.6/experiments/lbm_not_sparse.py` & `sparsebm-1.6.7/experiments/lbm_not_sparse.py`

 * *Files identical despite different names*

### Comparing `sparsebm-1.6.6/experiments/sparse_size_fixed.py` & `sparsebm-1.6.7/experiments/sparse_size_fixed.py`

 * *Files identical despite different names*

### Comparing `sparsebm-1.6.6/experiments/sparse_size_fixed_generate_data.py` & `sparsebm-1.6.7/experiments/sparse_size_fixed_generate_data.py`

 * *Files identical despite different names*

### Comparing `sparsebm-1.6.6/experiments/sparse_size_fixed_results.py` & `sparsebm-1.6.7/experiments/sparse_size_fixed_results.py`

 * *Files identical despite different names*

### Comparing `sparsebm-1.6.6/experiments/sparse_sparsity_fixed.py` & `sparsebm-1.6.7/experiments/sparse_sparsity_fixed.py`

 * *Files identical despite different names*

### Comparing `sparsebm-1.6.6/experiments/sparse_sparsity_fixed_generate_data.py` & `sparsebm-1.6.7/experiments/sparse_sparsity_fixed_generate_data.py`

 * *Files identical despite different names*

### Comparing `sparsebm-1.6.6/experiments/sparse_sparsity_fixed_results.py` & `sparsebm-1.6.7/experiments/sparse_sparsity_fixed_results.py`

 * *Files identical despite different names*

### Comparing `sparsebm-1.6.6/pyproject.toml` & `sparsebm-1.6.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -39,15 +39,15 @@
   "scikit-learn",
 ]
 
 [project.optional-dependencies]
 gpu = ["cupy"]
 tests = ["pytest"]
 experiments = ["rpy2"]
-build-doc = ["sphinx", "sphinx-argparse","m2r2","sphinx_rtd_theme"]
+build-doc = ["sphinx<7", "sphinx-argparse","m2r2","sphinx_rtd_theme","pandas"]
 
 [project.scripts]
 sparsebm = "sparsebm._entry_point:main"
 
 [project.urls]
 Repository = "https://gitlab.com/jbleger/sparsebm"
 Documentation = "https://jbleger.gitlab.io/sparsebm"
```

### Comparing `sparsebm-1.6.6/sparsebm/__init__.py` & `sparsebm-1.6.7/sparsebm/__init__.py`

 * *Files identical despite different names*

### Comparing `sparsebm-1.6.6/sparsebm/_datatypes.py` & `sparsebm-1.6.7/sparsebm/_datatypes.py`

 * *Files identical despite different names*

### Comparing `sparsebm-1.6.6/sparsebm/_entry_point.py` & `sparsebm-1.6.7/sparsebm/_entry_point.py`

 * *Files identical despite different names*

### Comparing `sparsebm-1.6.6/sparsebm/_graph_generator.py` & `sparsebm-1.6.7/sparsebm/_graph_generator.py`

 * *Files identical despite different names*

### Comparing `sparsebm-1.6.6/sparsebm/_lbm.py` & `sparsebm-1.6.7/sparsebm/_lbm.py`

 * *Files identical despite different names*

### Comparing `sparsebm-1.6.6/sparsebm/_model_selection.py` & `sparsebm-1.6.7/sparsebm/_model_selection.py`

 * *Files identical despite different names*

### Comparing `sparsebm-1.6.6/sparsebm/_sbm.py` & `sparsebm-1.6.7/sparsebm/_sbm.py`

 * *Files identical despite different names*

### Comparing `sparsebm-1.6.6/sparsebm/utils.py` & `sparsebm-1.6.7/sparsebm/utils.py`

 * *Files identical despite different names*

### Comparing `sparsebm-1.6.6/sparsebm.egg-info/PKG-INFO` & `sparsebm-1.6.7/sparsebm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparsebm
-Version: 1.6.6
+Version: 1.6.7
 Summary: An implementation of Stochastic Bloc model and Latent Block model efficient with sparse matrices
 Author-email: Gabriel Frisch <gabriel.frisch@hds.utc.fr>, Jean-Benoist Leger <jbleger@hds.utc.fr>
 Maintainer-email: Jean-Benoist Leger <jbleger@hds.utc.fr>
 License: MIT License
 Project-URL: Repository, https://gitlab.com/jbleger/sparsebm
 Project-URL: Documentation, https://jbleger.gitlab.io/sparsebm
 Keywords: datamining,graph,LBM,SBM,variationnal,sparse
```

### Comparing `sparsebm-1.6.6/sparsebm.egg-info/SOURCES.txt` & `sparsebm-1.6.7/sparsebm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sparsebm-1.6.6/tests/test_generate_sbm.py` & `sparsebm-1.6.7/tests/test_generate_sbm.py`

 * *Files identical despite different names*

### Comparing `sparsebm-1.6.6/tests/test_lbm.py` & `sparsebm-1.6.7/tests/test_lbm.py`

 * *Files identical despite different names*

### Comparing `sparsebm-1.6.6/tests/test_sbm.py` & `sparsebm-1.6.7/tests/test_sbm.py`

 * *Files identical despite different names*

