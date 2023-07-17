# Comparing `tmp/power-grid-model-1.5.0rc9216009937633.tar.gz` & `tmp/power-grid-model-1.5.0rc9219310821193.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "power-grid-model-1.5.0rc9216009937633.tar", last modified: Thu Jul 13 13:12:09 2023, max compression
+gzip compressed data, was "power-grid-model-1.5.0rc9219310821193.tar", last modified: Mon Jul 17 07:40:08 2023, max compression
```

## Comparing `power-grid-model-1.5.0rc9216009937633.tar` & `power-grid-model-1.5.0rc9219310821193.tar`

### file list

```diff
@@ -1,588 +1,593 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.450212 power-grid-model-1.5.0rc9216009937633/
--rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-07-13 13:12:09.450212 power-grid-model-1.5.0rc9216009937633/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-13 13:11:16.000000 power-grid-model-1.5.0rc9216009937633/PYPI_VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.370208 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.370208 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.362207 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.374208 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/all_components.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.374208 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/input.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9795 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data_gen.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.374208 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/
--rw-r--r--   0 runner    (1001) docker     (123)    30276 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/input.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    17268 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/output.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/update.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/output.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/update.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9311 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/calculation_parameters.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.378208 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/component/
--rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/component/appliance.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/component/base.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9145 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7084 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch3.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/component/fault.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/component/line.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/component/link.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/component/load_gen.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/component/node.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/component/power_sensor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/component/sensor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/component/shunt.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/component/source.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    20677 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/component/three_winding_transformer.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer_utils.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/component/voltage_sensor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    15129 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/container.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/enum.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/exception.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    68835 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/main_model.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.378208 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/block_matrix.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8955 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_current_pf_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    41695 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_linear_se_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_pf_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/linear_pf_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/math_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    16065 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_pf_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    14236 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/short_circuit_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    16203 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/sparse_lu_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    20157 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/y_bus.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/power_grid_model.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/sparse_mapping.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11555 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/three_phase_tensor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/timer.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    30819 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/topology.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.378208 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model_c/
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model_c/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.378208 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model_c/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.382208 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/basics.h
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/buffer.h
--rw-r--r--   0 runner    (1001) docker     (123)    55882 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/dataset_definitions.h
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/handle.h
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/meta_data.h
--rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/model.h
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/options.h
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model_c/include/power_grid_model_c.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.382208 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model_c/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model_c/src/buffer.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    93852 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model_c/src/dataset_definitions.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model_c/src/handle.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model_c/src/handle.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model_c/src/meta_data.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model_c/src/model.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model_c/src/options.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model_c/src/options.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 13:12:09.450212 power-grid-model-1.5.0rc9216009937633/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.362207 power-grid-model-1.5.0rc9216009937633/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.382208 power-grid-model-1.5.0rc9216009937633/src/power_grid_model/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/src/power_grid_model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.386209 power-grid-model-1.5.0rc9216009937633/src/power_grid_model/core/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/src/power_grid_model/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/src/power_grid_model/core/data_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/src/power_grid_model/core/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/src/power_grid_model/core/index_integer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/src/power_grid_model/core/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    10645 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/src/power_grid_model/core/power_grid_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     9426 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/src/power_grid_model/core/power_grid_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    22015 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/src/power_grid_model/core/power_grid_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/src/power_grid_model/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/src/power_grid_model/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/src/power_grid_model/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    21661 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/src/power_grid_model/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.386209 power-grid-model-1.5.0rc9216009937633/src/power_grid_model/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/src/power_grid_model/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/src/power_grid_model/validation/assertions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15485 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/src/power_grid_model/validation/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    35027 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/src/power_grid_model/validation/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     8610 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/src/power_grid_model/validation/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    29999 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/src/power_grid_model/validation/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.382208 power-grid-model-1.5.0rc9216009937633/src/power_grid_model.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-07-13 13:12:09.000000 power-grid-model-1.5.0rc9216009937633/src/power_grid_model.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    35172 2023-07-13 13:12:09.000000 power-grid-model-1.5.0rc9216009937633/src/power_grid_model.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 13:12:09.000000 power-grid-model-1.5.0rc9216009937633/src/power_grid_model.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-13 13:12:09.000000 power-grid-model-1.5.0rc9216009937633/src/power_grid_model.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-13 13:12:09.000000 power-grid-model-1.5.0rc9216009937633/src/power_grid_model.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.370208 power-grid-model-1.5.0rc9216009937633/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.370208 power-grid-model-1.5.0rc9216009937633/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.370208 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.386209 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/1os2msr/
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/1os2msr/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/1os2msr/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/1os2msr/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/1os2msr/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/1os2msr/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/1os2msr/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.390209 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test/
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.390209 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.390209 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-dependent-cacheable/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-dependent-cacheable/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-dependent-cacheable/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.394209 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.394209 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-incomplete-input/
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-incomplete-input/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-incomplete-input/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.398209 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-independent-cacheable/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-independent-cacheable/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-independent-cacheable/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.398209 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.398209 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-newton/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-newton/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-newton/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-newton/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-newton/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-newton/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-newton/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-newton/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-newton/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.402209 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-i-n-optional/
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-i-n-optional/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-i-n-optional/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-i-n-optional/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-i-n-optional/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.402209 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/gaia-example/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/gaia-example/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/gaia-example/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/gaia-example/gaia_grid.gnf
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/gaia-example/gaia_grid.gnf.license
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/gaia-example/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/gaia-example/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/gaia-example/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/gaia-example/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.402209 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/multi-source-with-angle/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/multi-source-with-angle/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/multi-source-with-angle/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/multi-source-with-angle/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/multi-source-with-angle/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/multi-source-with-angle/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/multi-source-with-angle/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.366207 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.366207 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.366207 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.402209 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.406210 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/asym_load/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/asym_load/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/asym_load/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/asym_load/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.406210 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/line/
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/line/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/line/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/line/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/line/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/line/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.406210 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/node/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/node/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/node/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/node/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/node/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/node/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.410210 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/shunt/
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/shunt/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/shunt/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/shunt/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.410210 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/source/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/source/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/source/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/source/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/source/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/source/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.410210 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.414210 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/sym_load/
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/sym_load/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/sym_load/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/sym_load/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.414210 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/transformer/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    17633 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.366207 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.414210 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/basic-node/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/basic-node/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/basic-node/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/basic-node/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/basic-node/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/basic-node/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/basic-node/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/basic-node/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.414210 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/line/
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/line/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/line/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/line/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/line/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/line/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.418210 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/node/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/node/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/node/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/node/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/node/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/node/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.418210 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/shunt/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/shunt/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/shunt/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/shunt/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.418210 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/source/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/source/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/source/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/source/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/source/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/source/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.418210 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/sym_gen/
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/sym_gen/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/sym_gen/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/sym_gen/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.422211 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/sym_load/
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/sym_load/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/sym_load/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/sym_load/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.422211 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.422211 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/transformer/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    15639 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.366207 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/networks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.366207 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/networks/asymmetric/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.426211 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    15865 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.426211 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    10605 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.366207 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/networks/symmetric/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.426211 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     8702 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.426211 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.430211 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/r-state-estimation/
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/r-state-estimation/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/r-state-estimation/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/r-state-estimation/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/r-state-estimation/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/r-state-estimation/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/r-state-estimation/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.430211 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/three-winding-transformer/
--rw-r--r--   0 runner    (1001) docker     (123)    21196 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/three-winding-transformer/asym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/three-winding-transformer/asym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/three-winding-transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/three-winding-transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/three-winding-transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/three-winding-transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/three-winding-transformer/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/three-winding-transformer/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/three-winding-transformer/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/three-winding-transformer/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.430211 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/vision-example/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/vision-example/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/vision-example/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/vision-example/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/vision-example/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/vision-example/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/vision-example/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/vision-example/vision_grid.vnf
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/vision-example/vision_grid.vnf.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.434211 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/vision-validation-network/
--rw-r--r--   0 runner    (1001) docker     (123)    20486 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/vision-validation-network/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/vision-validation-network/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    30756 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/vision-validation-network/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/vision-validation-network/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/vision-validation-network/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/vision-validation-network/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/vision-validation-network/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/vision-validation-network/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    35119 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.370208 power-grid-model-1.5.0rc9216009937633/tests/data/short_circuit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.434211 power-grid-model-1.5.0rc9216009937633/tests/data/short_circuit/single_phase_to_ground/
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/short_circuit/single_phase_to_ground/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/short_circuit/single_phase_to_ground/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/short_circuit/single_phase_to_ground/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/short_circuit/single_phase_to_ground/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)   243263 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/short_circuit/single_phase_to_ground/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/short_circuit/single_phase_to_ground/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    24314 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/short_circuit/single_phase_to_ground/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/short_circuit/single_phase_to_ground/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.434211 power-grid-model-1.5.0rc9216009937633/tests/data/short_circuit/three_phase/
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/short_circuit/three_phase/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/short_circuit/three_phase/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/short_circuit/three_phase/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/short_circuit/three_phase/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    58928 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/short_circuit/three_phase/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/short_circuit/three_phase/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/short_circuit/three_phase/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/short_circuit/three_phase/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.438212 power-grid-model-1.5.0rc9216009937633/tests/data/short_circuit/two_phase/
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/short_circuit/two_phase/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/short_circuit/two_phase/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/short_circuit/two_phase/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/short_circuit/two_phase/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)   236282 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/short_circuit/two_phase/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/short_circuit/two_phase/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    24314 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/short_circuit/two_phase/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/short_circuit/two_phase/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.438212 power-grid-model-1.5.0rc9216009937633/tests/data/short_circuit/two_phase_to_ground/
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/short_circuit/two_phase_to_ground/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/short_circuit/two_phase_to_ground/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/short_circuit/two_phase_to_ground/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/short_circuit/two_phase_to_ground/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)   242819 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/short_circuit/two_phase_to_ground/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/short_circuit/two_phase_to_ground/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    24314 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/short_circuit/two_phase_to_ground/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/short_circuit/two_phase_to_ground/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.370208 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.442212 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/1os2msr/
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/1os2msr/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/1os2msr/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/1os2msr/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/1os2msr/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/1os2msr/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/1os2msr/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.442212 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/1os2msr-no-angle/
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/1os2msr-no-angle/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/1os2msr-no-angle/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/1os2msr-no-angle/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/1os2msr-no-angle/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/1os2msr-no-angle/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/1os2msr-no-angle/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.442212 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/distribution-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/distribution-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/distribution-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/distribution-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/distribution-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/distribution-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    19468 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/distribution-case/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/distribution-case/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/distribution-case/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/distribution-case/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.442212 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/dummy-test-sym/
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/dummy-test-sym/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/dummy-test-sym/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/dummy-test-sym/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/dummy-test-sym/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/dummy-test-sym/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/dummy-test-sym/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.446212 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/node-injection-sensor-and-zero-injection/
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/node-injection-sensor-and-zero-injection/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/node-injection-sensor-and-zero-injection/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.446212 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/residual-test/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/residual-test/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/residual-test/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/residual-test/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/residual-test/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/residual-test/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/residual-test/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.446212 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/single-line-load/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/single-line-load/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/single-line-load/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/single-line-load/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/single-line-load/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/single-line-load/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/single-line-load/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.446212 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/three_winding_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/three_winding_transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/three_winding_transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/three_winding_transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/three_winding_transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/three_winding_transformer/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/three_winding_transformer/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.450212 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/transmission-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/transmission-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    29158 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/transmission-case/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/transmission-case/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/transmission-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/transmission-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/transmission-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/transmission-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/transmission-case/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/transmission-case/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.450212 power-grid-model-1.5.0rc9216009937633/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/unit/test_0Z_model_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/unit/test_error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/unit/test_meta_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/unit/test_power_grid_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    20807 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/unit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:12:09.450212 power-grid-model-1.5.0rc9216009937633/tests/unit/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/unit/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/unit/validation/test_assertions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/unit/validation/test_batch_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/unit/validation/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    29354 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/unit/validation/test_input_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19701 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/unit/validation/test_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/unit/validation/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    24851 2023-07-13 13:11:12.000000 power-grid-model-1.5.0rc9216009937633/tests/unit/validation/test_validation_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.446553 power-grid-model-1.5.0rc9219310821193/
+-rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-07-17 07:40:08.446553 power-grid-model-1.5.0rc9219310821193/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-17 07:39:23.000000 power-grid-model-1.5.0rc9219310821193/PYPI_VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.366553 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.366553 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.358553 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.366553 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/all_components.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.366553 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/input.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9795 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data_gen.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.366553 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)    30276 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/input.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17268 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/output.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/update.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/output.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/update.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11542 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/calculation_parameters.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.370553 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/component/
+-rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/component/appliance.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/component/base.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9145 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7084 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch3.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/component/fault.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/component/line.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/component/link.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/component/load_gen.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/component/node.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/component/power_sensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/component/sensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/component/shunt.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/component/source.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20677 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/component/three_winding_transformer.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer_utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/component/voltage_sensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15129 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/container.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/enum.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/exception.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.370553 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/
+-rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/input.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15956 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/output.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/state.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/update.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    53503 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/main_model.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.370553 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/block_matrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8955 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_current_pf_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    41695 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_linear_se_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_pf_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/linear_pf_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/math_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16065 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_pf_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14236 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/short_circuit_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16203 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/sparse_lu_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20157 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/y_bus.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/power_grid_model.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/sparse_mapping.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11555 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/three_phase_tensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/timer.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    30819 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/topology.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.370553 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model_c/
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model_c/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.370553 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model_c/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.370553 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/basics.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/buffer.h
+-rw-r--r--   0 runner    (1001) docker     (123)    55882 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/dataset_definitions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/handle.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/meta_data.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/model.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/options.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model_c/include/power_grid_model_c.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.374553 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model_c/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model_c/src/buffer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    93852 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model_c/src/dataset_definitions.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model_c/src/handle.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model_c/src/handle.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model_c/src/meta_data.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model_c/src/model.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model_c/src/options.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model_c/src/options.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 07:40:08.446553 power-grid-model-1.5.0rc9219310821193/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.358553 power-grid-model-1.5.0rc9219310821193/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.374553 power-grid-model-1.5.0rc9219310821193/src/power_grid_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/src/power_grid_model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.374553 power-grid-model-1.5.0rc9219310821193/src/power_grid_model/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/src/power_grid_model/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/src/power_grid_model/core/data_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/src/power_grid_model/core/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/src/power_grid_model/core/index_integer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/src/power_grid_model/core/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10645 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/src/power_grid_model/core/power_grid_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9426 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/src/power_grid_model/core/power_grid_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22015 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/src/power_grid_model/core/power_grid_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/src/power_grid_model/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/src/power_grid_model/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/src/power_grid_model/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21661 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/src/power_grid_model/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.374553 power-grid-model-1.5.0rc9219310821193/src/power_grid_model/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/src/power_grid_model/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/src/power_grid_model/validation/assertions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15485 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/src/power_grid_model/validation/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35027 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/src/power_grid_model/validation/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8610 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/src/power_grid_model/validation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29999 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/src/power_grid_model/validation/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.374553 power-grid-model-1.5.0rc9219310821193/src/power_grid_model.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-07-17 07:40:08.000000 power-grid-model-1.5.0rc9219310821193/src/power_grid_model.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    35498 2023-07-17 07:40:08.000000 power-grid-model-1.5.0rc9219310821193/src/power_grid_model.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 07:40:08.000000 power-grid-model-1.5.0rc9219310821193/src/power_grid_model.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-17 07:40:08.000000 power-grid-model-1.5.0rc9219310821193/src/power_grid_model.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-17 07:40:08.000000 power-grid-model-1.5.0rc9219310821193/src/power_grid_model.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.362553 power-grid-model-1.5.0rc9219310821193/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.362553 power-grid-model-1.5.0rc9219310821193/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.362553 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.378553 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/1os2msr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/1os2msr/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/1os2msr/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/1os2msr/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/1os2msr/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/1os2msr/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/1os2msr/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.378553 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.378553 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.378553 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-dependent-cacheable/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-dependent-cacheable/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-dependent-cacheable/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.378553 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.382553 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-incomplete-input/
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-incomplete-input/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-incomplete-input/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.382553 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-independent-cacheable/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-independent-cacheable/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-independent-cacheable/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.386553 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.386553 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-newton/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-newton/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-newton/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-newton/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-newton/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-newton/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-newton/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-newton/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-newton/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.390553 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-i-n-optional/
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-i-n-optional/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-i-n-optional/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-i-n-optional/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-i-n-optional/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.390553 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/gaia-example/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/gaia-example/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/gaia-example/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/gaia-example/gaia_grid.gnf
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/gaia-example/gaia_grid.gnf.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/gaia-example/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/gaia-example/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/gaia-example/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/gaia-example/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.390553 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/multi-source-with-angle/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/multi-source-with-angle/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/multi-source-with-angle/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/multi-source-with-angle/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/multi-source-with-angle/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/multi-source-with-angle/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/multi-source-with-angle/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.362553 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.362553 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.362553 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.394553 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.394553 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/asym_load/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/asym_load/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/asym_load/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/asym_load/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.394553 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/line/
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/line/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/line/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/line/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/line/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/line/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.398553 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/node/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/node/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/node/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/node/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/node/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/node/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.398553 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/shunt/
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/shunt/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/shunt/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/shunt/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.398553 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/source/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/source/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/source/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/source/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/source/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.402553 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.402553 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/sym_load/
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/sym_load/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/sym_load/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/sym_load/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.406553 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/transformer/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    17633 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.362553 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.406553 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/basic-node/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/basic-node/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/basic-node/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/basic-node/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/basic-node/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/basic-node/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/basic-node/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/basic-node/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.406553 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/line/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/line/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/line/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/line/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/line/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/line/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.410553 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/node/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/node/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/node/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/node/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/node/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/node/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.410553 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/shunt/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/shunt/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/shunt/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/shunt/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.414553 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/source/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/source/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/source/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/source/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/source/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.414553 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/sym_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/sym_gen/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/sym_gen/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/sym_gen/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.414553 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/sym_load/
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/sym_load/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/sym_load/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/sym_load/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.418553 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.418553 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/transformer/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    15639 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.362553 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/networks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.362553 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/networks/asymmetric/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.422553 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    15865 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.422553 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10605 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.362553 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/networks/symmetric/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.426553 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     8702 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.426553 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.430553 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/r-state-estimation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/r-state-estimation/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/r-state-estimation/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/r-state-estimation/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/r-state-estimation/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/r-state-estimation/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/r-state-estimation/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.430553 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/three-winding-transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)    21196 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/three-winding-transformer/asym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/three-winding-transformer/asym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/three-winding-transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/three-winding-transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/three-winding-transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/three-winding-transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/three-winding-transformer/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/three-winding-transformer/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/three-winding-transformer/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/three-winding-transformer/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.430553 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/vision-example/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/vision-example/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/vision-example/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/vision-example/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/vision-example/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/vision-example/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/vision-example/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/vision-example/vision_grid.vnf
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/vision-example/vision_grid.vnf.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.434553 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/vision-validation-network/
+-rw-r--r--   0 runner    (1001) docker     (123)    20486 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/vision-validation-network/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/vision-validation-network/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    30756 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/vision-validation-network/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/vision-validation-network/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/vision-validation-network/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/vision-validation-network/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/vision-validation-network/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/vision-validation-network/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    35119 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.362553 power-grid-model-1.5.0rc9219310821193/tests/data/short_circuit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.434553 power-grid-model-1.5.0rc9219310821193/tests/data/short_circuit/single_phase_to_ground/
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/short_circuit/single_phase_to_ground/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/short_circuit/single_phase_to_ground/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/short_circuit/single_phase_to_ground/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/short_circuit/single_phase_to_ground/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)   243263 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/short_circuit/single_phase_to_ground/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/short_circuit/single_phase_to_ground/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    24314 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/short_circuit/single_phase_to_ground/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/short_circuit/single_phase_to_ground/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.434553 power-grid-model-1.5.0rc9219310821193/tests/data/short_circuit/three_phase/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/short_circuit/three_phase/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/short_circuit/three_phase/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/short_circuit/three_phase/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/short_circuit/three_phase/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    58928 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/short_circuit/three_phase/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/short_circuit/three_phase/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/short_circuit/three_phase/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/short_circuit/three_phase/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.434553 power-grid-model-1.5.0rc9219310821193/tests/data/short_circuit/two_phase/
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/short_circuit/two_phase/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/short_circuit/two_phase/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/short_circuit/two_phase/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/short_circuit/two_phase/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)   236282 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/short_circuit/two_phase/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/short_circuit/two_phase/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    24314 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/short_circuit/two_phase/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/short_circuit/two_phase/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.438553 power-grid-model-1.5.0rc9219310821193/tests/data/short_circuit/two_phase_to_ground/
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/short_circuit/two_phase_to_ground/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/short_circuit/two_phase_to_ground/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/short_circuit/two_phase_to_ground/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/short_circuit/two_phase_to_ground/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)   242819 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/short_circuit/two_phase_to_ground/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/short_circuit/two_phase_to_ground/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    24314 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/short_circuit/two_phase_to_ground/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/short_circuit/two_phase_to_ground/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.362553 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.438553 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/1os2msr/
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/1os2msr/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/1os2msr/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/1os2msr/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/1os2msr/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/1os2msr/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/1os2msr/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.438553 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/1os2msr-no-angle/
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/1os2msr-no-angle/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/1os2msr-no-angle/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/1os2msr-no-angle/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/1os2msr-no-angle/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/1os2msr-no-angle/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/1os2msr-no-angle/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.438553 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/distribution-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/distribution-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/distribution-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/distribution-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/distribution-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/distribution-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    19468 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/distribution-case/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/distribution-case/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/distribution-case/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/distribution-case/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.438553 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/dummy-test-sym/
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/dummy-test-sym/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/dummy-test-sym/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/dummy-test-sym/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/dummy-test-sym/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/dummy-test-sym/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/dummy-test-sym/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.442553 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/node-injection-sensor-and-zero-injection/
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/node-injection-sensor-and-zero-injection/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/node-injection-sensor-and-zero-injection/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.442553 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/residual-test/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/residual-test/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/residual-test/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/residual-test/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/residual-test/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/residual-test/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/residual-test/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.442553 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/single-line-load/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/single-line-load/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/single-line-load/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/single-line-load/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/single-line-load/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/single-line-load/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/single-line-load/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.442553 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/three_winding_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/three_winding_transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/three_winding_transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/three_winding_transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/three_winding_transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/three_winding_transformer/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/three_winding_transformer/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.442553 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/transmission-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/transmission-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    29158 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/transmission-case/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/transmission-case/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/transmission-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/transmission-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/transmission-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/transmission-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/transmission-case/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/transmission-case/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.442553 power-grid-model-1.5.0rc9219310821193/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/unit/test_0Z_model_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/unit/test_error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/unit/test_meta_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/unit/test_power_grid_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20807 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/unit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:08.446553 power-grid-model-1.5.0rc9219310821193/tests/unit/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/unit/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/unit/validation/test_assertions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/unit/validation/test_batch_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/unit/validation/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29354 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/unit/validation/test_input_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19701 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/unit/validation/test_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/unit/validation/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24851 2023-07-17 07:39:20.000000 power-grid-model-1.5.0rc9219310821193/tests/unit/validation/test_validation_functions.py
```

### Comparing `power-grid-model-1.5.0rc9216009937633/LICENSE` & `power-grid-model-1.5.0rc9219310821193/LICENSE`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/PKG-INFO` & `power-grid-model-1.5.0rc9219310821193/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: power-grid-model
-Version: 1.5.0rc9216009937633
+Version: 1.5.0rc9219310821193
 Summary: Python/C++ library for distribution power system analysis
 Author-email: Alliander Dynamic Grid Calculation <dynamic.grid.calculation@alliander.com>
 License: MPL-2.0
 Project-URL: Home-page, https://lfenergy.org/projects/power-grid-model/
 Project-URL: GitHub, https://github.com/PowerGridModel/power-grid-model
 Project-URL: Documentation, https://power-grid-model.readthedocs.io/en/stable/
 Project-URL: Mailing-list, https://lists.lfenergy.org/g/powergridmodel
```

### Comparing `power-grid-model-1.5.0rc9216009937633/README.md` & `power-grid-model-1.5.0rc9219310821193/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/CMakeLists.txt` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/all_components.hpp` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/all_components.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset.hpp` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/input.hpp` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/input.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data.hpp` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data_gen.hpp` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data_gen.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/input.hpp` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/input.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/output.hpp` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/output.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/update.hpp` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/update.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/output.hpp` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/output.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/update.hpp` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/update.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/calculation_parameters.hpp` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/calculation_parameters.hpp`

 * *Files 17% similar despite different names*

```diff
@@ -218,14 +218,58 @@
     std::vector<ComplexValue<sym>> i_fault;
     std::vector<ComplexValue<sym>> u_bus;
     std::vector<ComplexValue<sym>> i_branch_from;
     std::vector<ComplexValue<sym>> i_branch_to;
     std::vector<ComplexValue<sym>> i_source;
 };
 
+template <typename T>
+concept symmetric_math_output_type = std::same_as<T, MathOutput<true>> || std::same_as<T, ShortCircuitMathOutput<true>>;
+
+static_assert(symmetric_math_output_type<MathOutput<true>>);
+static_assert(!symmetric_math_output_type<MathOutput<false>>);
+static_assert(symmetric_math_output_type<ShortCircuitMathOutput<true>>);
+static_assert(!symmetric_math_output_type<ShortCircuitMathOutput<false>>);
+
+template <typename T>
+concept asymmetric_math_output_type =
+    std::same_as<T, MathOutput<false>> || std::same_as<T, ShortCircuitMathOutput<false>>;
+
+static_assert(!asymmetric_math_output_type<MathOutput<true>>);
+static_assert(asymmetric_math_output_type<MathOutput<false>>);
+static_assert(!asymmetric_math_output_type<ShortCircuitMathOutput<true>>);
+static_assert(asymmetric_math_output_type<ShortCircuitMathOutput<false>>);
+
+template <typename T>
+concept steady_state_math_output_type = std::same_as<T, MathOutput<true>> || std::same_as<T, MathOutput<false>>;
+
+static_assert(steady_state_math_output_type<MathOutput<true>>);
+static_assert(steady_state_math_output_type<MathOutput<false>>);
+static_assert(!steady_state_math_output_type<ShortCircuitMathOutput<true>>);
+static_assert(!steady_state_math_output_type<ShortCircuitMathOutput<false>>);
+
+template <typename T>
+concept short_circuit_math_output_type =
+    std::same_as<T, ShortCircuitMathOutput<true>> || std::same_as<T, ShortCircuitMathOutput<false>>;
+
+static_assert(!short_circuit_math_output_type<MathOutput<true>>);
+static_assert(!short_circuit_math_output_type<MathOutput<false>>);
+static_assert(short_circuit_math_output_type<ShortCircuitMathOutput<true>>);
+static_assert(short_circuit_math_output_type<ShortCircuitMathOutput<false>>);
+
+template <typename T>
+concept math_output_type = (symmetric_math_output_type<T> ||
+                            asymmetric_math_output_type<T>)&&(steady_state_math_output_type<T> ||
+                                                              short_circuit_math_output_type<T>);
+
+static_assert(math_output_type<MathOutput<true>>);
+static_assert(math_output_type<MathOutput<false>>);
+static_assert(math_output_type<ShortCircuitMathOutput<true>>);
+static_assert(math_output_type<ShortCircuitMathOutput<false>>);
+
 // component indices at physical model side
 // from, to node indices for branches
 // node1, node2, node3 indices for 3-way branches
 // node indices for source, load_gen, shunt
 struct ComponentTopology {
     Idx n_node;
     std::vector<BranchIdx> branch_node_idx;
```

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/component/appliance.hpp` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/component/appliance.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/component/base.hpp` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/component/base.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch.hpp` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch3.hpp` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch3.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/component/fault.hpp` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/component/fault.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/component/line.hpp` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/component/line.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/component/link.hpp` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/component/link.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/component/load_gen.hpp` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/component/load_gen.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/component/node.hpp` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/component/node.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/component/power_sensor.hpp` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/component/power_sensor.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/component/sensor.hpp` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/component/sensor.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/component/shunt.hpp` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/component/shunt.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/component/source.hpp` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/component/source.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/component/three_winding_transformer.hpp` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/component/three_winding_transformer.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer.hpp` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer_utils.hpp` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer_utils.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/component/voltage_sensor.hpp` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/component/voltage_sensor.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/container.hpp` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/container.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/enum.hpp` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/enum.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/exception.hpp` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/exception.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/main_model.hpp` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/main_model.hpp`

 * *Files 20% similar despite different names*

```diff
@@ -21,14 +21,19 @@
 #include "auxiliary/dataset.hpp"
 #include "auxiliary/input.hpp"
 #include "auxiliary/output.hpp"
 
 // math model include
 #include "math_solver/math_solver.hpp"
 
+// main model implementation
+#include "main_core/input.hpp"
+#include "main_core/output.hpp"
+#include "main_core/update.hpp"
+
 // threading
 #include <thread>
 
 namespace power_grid_model {
 
 // main model implementation template
 template <class T, class U>
@@ -36,14 +41,15 @@
 
 template <class... ExtraRetrievableType, class... ComponentType>
 class MainModelImpl<ExtraRetrievableTypes<ExtraRetrievableType...>, ComponentList<ComponentType...>> {
    private:
     // internal type traits
     // container class
     using ComponentContainer = Container<ExtraRetrievableTypes<ExtraRetrievableType...>, ComponentType...>;
+    using MainModelState = main_core::MainModelState<ComponentContainer>;
 
     // trait on type list
     // struct of entry
     // name of the component, and the index in the list
     struct ComponentEntry {
         char const* name;
         size_t index;
@@ -69,16 +75,16 @@
                                                         std::make_index_sequence<sizeof...(ComponentType)>>;
     static constexpr size_t n_types = AllComponents::n_types;
 
     // function pointer definition
     using InputFunc = void (*)(MainModelImpl& x, DataPointer<true> const& data_ptr, Idx position);
     using UpdateFunc = void (*)(MainModelImpl& x, DataPointer<true> const& data_ptr, Idx position,
                                 std::vector<Idx2D> const& sequence_idx);
-    template <bool sym>
-    using OutputFunc = void (*)(MainModelImpl& x, std::vector<MathOutput<sym>> const& math_output,
+    template <math_output_type MathOutputType>
+    using OutputFunc = void (*)(MainModelImpl& x, std::vector<MathOutputType> const& math_output,
                                 DataPointer<false> const& data_ptr, Idx position);
     using CheckUpdateFunc = bool (*)(ConstDataPointer const& component_update);
     using GetSeqIdxFunc = std::vector<Idx2D> (*)(MainModelImpl const& x, ConstDataPointer const& component_update);
     using GetIndexerFunc = void (*)(MainModelImpl const& x, ID const* id_begin, Idx size, Idx* indexer_begin);
 
    public:
     struct cached_update_t : std::true_type {};
@@ -109,15 +115,15 @@
     explicit MainModelImpl(double system_frequency) : system_frequency_{system_frequency} {
     }
 
     // get number
     template <class CompType>
     Idx component_count() const {
         assert(construction_complete_);
-        return components_.template size<CompType>();
+        return state_.components.template size<CompType>();
     }
 
     // all component count
     std::map<std::string, Idx> all_component_count() const {
         std::map<std::string, Idx> map;
         static constexpr std::array counter{&MainModelImpl::component_count<ComponentType>...};
         for (ComponentEntry const& entry : AllComponents::component_index_map) {
@@ -137,127 +143,31 @@
 
     // template to construct components
     // using forward interators
     // different selection based on component type
     template <std::derived_from<Base> CompType, std::forward_iterator ForwardIterator>
     void add_component(ForwardIterator begin, ForwardIterator end) {
         assert(!construction_complete_);
-        size_t size = std::distance(begin, end);
-        components_.template reserve<CompType>(size);
-        // loop to add component
-        for (auto it = begin; it != end; ++it) {
-            auto const& input = *it;
-            ID const id = input.id;
-            // construct based on type of component
-            if constexpr (std::derived_from<CompType, Node>) {
-                components_.template emplace<CompType>(id, input);
-            }
-            else if constexpr (std::derived_from<CompType, Branch>) {
-                double const u1 = components_.template get_item<Node>(input.from_node).u_rated();
-                double const u2 = components_.template get_item<Node>(input.to_node).u_rated();
-                // set system frequency for line
-                if constexpr (std::same_as<CompType, Line>) {
-                    components_.template emplace<CompType>(id, input, system_frequency_, u1, u2);
-                }
-                else {
-                    components_.template emplace<CompType>(id, input, u1, u2);
-                }
-            }
-            else if constexpr (std::derived_from<CompType, Branch3>) {
-                double const u1 = components_.template get_item<Node>(input.node_1).u_rated();
-                double const u2 = components_.template get_item<Node>(input.node_2).u_rated();
-                double const u3 = components_.template get_item<Node>(input.node_3).u_rated();
-                components_.template emplace<CompType>(id, input, u1, u2, u3);
-            }
-            else if constexpr (std::derived_from<CompType, Appliance>) {
-                double const u = components_.template get_item<Node>(input.node).u_rated();
-                components_.template emplace<CompType>(id, input, u);
-            }
-            else if constexpr (std::derived_from<CompType, GenericVoltageSensor>) {
-                double const u = components_.template get_item<Node>(input.measured_object).u_rated();
-                components_.template emplace<CompType>(id, input, u);
-            }
-            else if constexpr (std::derived_from<CompType, GenericPowerSensor>) {
-                // it is not allowed to place a sensor at a link
-                if (components_.get_idx_by_id(input.measured_object).group ==
-                    components_.template get_type_idx<Link>()) {
-                    throw InvalidMeasuredObject("Link", "PowerSensor");
-                }
-                ID const measured_object = input.measured_object;
-                // check correctness of measured component type based on measured terminal type
-                switch (input.measured_terminal_type) {
-                    using enum MeasuredTerminalType;
-
-                    case branch_from:
-                    case branch_to:
-                        components_.template get_item<Branch>(measured_object);
-                        break;
-                    case branch3_1:
-                    case branch3_2:
-                    case branch3_3:
-                        components_.template get_item<Branch3>(measured_object);
-                        break;
-                    case shunt:
-                        components_.template get_item<Shunt>(measured_object);
-                        break;
-                    case source:
-                        components_.template get_item<Source>(measured_object);
-                        break;
-                    case load:
-                        components_.template get_item<GenericLoad>(measured_object);
-                        break;
-                    case generator:
-                        components_.template get_item<GenericGenerator>(measured_object);
-                        break;
-                    case node:
-                        components_.template get_item<Node>(measured_object);
-                        break;
-                    default:
-                        throw MissingCaseForEnumError(std::string(GenericPowerSensor::name) + " item retrieval",
-                                                      input.measured_terminal_type);
-                }
-
-                components_.template emplace<CompType>(id, input);
-            }
-            else if constexpr (std::derived_from<CompType, Fault>) {
-                // check that fault object exists (currently, only faults at nodes are supported)
-                components_.template get_item<Node>(input.fault_object);
-                components_.template emplace<CompType>(id, input);
-            }
-        }
+        main_core::add_component<CompType>(state_, begin, end, system_frequency_);
     }
 
     // template to update components
     // using forward interators
     // different selection based on component type
     // if sequence_idx is given, it will be used to load the object instead of using IDs via hash map.
     template <class CompType, class CacheType, std::forward_iterator ForwardIterator>
     void update_component(ForwardIterator begin, ForwardIterator end, std::vector<Idx2D> const& sequence_idx = {}) {
         assert(construction_complete_);
-        bool const has_sequence_id = !sequence_idx.empty();
-        Idx seq = 0;
-        // loop to to update component
-        for (auto it = begin; it != end; ++it, ++seq) {
-            // get component
-            // either using ID via hash map
-            // either directly using sequence id
-            Idx2D const sequence_single =
-                has_sequence_id ? sequence_idx[seq] : components_.template get_idx_by_id<CompType>(it->id);
 
-            if constexpr (CacheType::value) {
-                components_.template cache_item<CompType>(sequence_single.pos);
-            }
+        UpdateChange changed = main_core::update_component<CompType, CacheType>(state_, begin, end, sequence_idx);
 
-            CompType& comp = components_.template get_item<CompType>(sequence_single);
-            // update, get changed variable
-            UpdateChange changed = comp.update(*it);
-            update_state(changed);
-            if constexpr (CacheType::value) {
-                cached_state_changes_ = cached_state_changes_ || changed;
-            }
+        // update, get changed variable
+        update_state(changed);
+        if constexpr (CacheType::value) {
+            cached_state_changes_ = cached_state_changes_ || changed;
         }
     }
 
     // helper function to update vectors of components
     template <class CompType, class CacheType>
     void update_component(std::vector<typename CompType::UpdateType> const& components) {
         update_component<CompType, CacheType>(components.cbegin(), components.cend());
@@ -290,132 +200,137 @@
                 update[entry.index](*this, found->second, pos, found_seq->second);
             }
         }
     }
 
     // restore the initial values of all components
     void restore_components() {
-        components_.restore_values();
+        state_.components.restore_values();
 
         update_state(cached_state_changes_);
         cached_state_changes_ = {};
     }
 
     // set complete construction
     // initialize internal arrays
     void set_construction_complete() {
         assert(!construction_complete_);
 #ifndef NDEBUG
         // set construction_complete for debug assertions
         construction_complete_ = true;
 #endif  // !NDEBUG
-        components_.set_construction_complete();
+        state_.components.set_construction_complete();
         // set component topo
         ComponentTopology comp_topo;
-        comp_topo.n_node = components_.template size<Node>();
+        comp_topo.n_node = state_.components.template size<Node>();
         // fill topology data
-        comp_topo.branch_node_idx.resize(components_.template size<Branch>());
-        std::transform(components_.template citer<Branch>().begin(), components_.template citer<Branch>().end(),
-                       comp_topo.branch_node_idx.begin(), [this](Branch const& branch) {
-                           return BranchIdx{components_.template get_seq<Node>(branch.from_node()),
-                                            components_.template get_seq<Node>(branch.to_node())};
-                       });
-        comp_topo.branch3_node_idx.resize(components_.template size<Branch3>());
-        std::transform(components_.template citer<Branch3>().begin(), components_.template citer<Branch3>().end(),
-                       comp_topo.branch3_node_idx.begin(), [this](Branch3 const& branch3) {
-                           return Branch3Idx{components_.template get_seq<Node>(branch3.node_1()),
-                                             components_.template get_seq<Node>(branch3.node_2()),
-                                             components_.template get_seq<Node>(branch3.node_3())};
-                       });
-        comp_topo.source_node_idx.resize(components_.template size<Source>());
-        std::transform(components_.template citer<Source>().begin(), components_.template citer<Source>().end(),
-                       comp_topo.source_node_idx.begin(), [this](Source const& source) {
-                           return components_.template get_seq<Node>(source.node());
-                       });
-        comp_topo.shunt_node_idx.resize(components_.template size<Shunt>());
-        std::transform(components_.template citer<Shunt>().begin(), components_.template citer<Shunt>().end(),
-                       comp_topo.shunt_node_idx.begin(), [this](Shunt const& shunt) {
-                           return components_.template get_seq<Node>(shunt.node());
-                       });
-        comp_topo.load_gen_node_idx.resize(components_.template size<GenericLoadGen>());
-        std::transform(components_.template citer<GenericLoadGen>().begin(),
-                       components_.template citer<GenericLoadGen>().end(), comp_topo.load_gen_node_idx.begin(),
+        comp_topo.branch_node_idx.resize(state_.components.template size<Branch>());
+        std::transform(state_.components.template citer<Branch>().begin(),
+                       state_.components.template citer<Branch>().end(), comp_topo.branch_node_idx.begin(),
+                       [this](Branch const& branch) {
+                           return BranchIdx{state_.components.template get_seq<Node>(branch.from_node()),
+                                            state_.components.template get_seq<Node>(branch.to_node())};
+                       });
+        comp_topo.branch3_node_idx.resize(state_.components.template size<Branch3>());
+        std::transform(state_.components.template citer<Branch3>().begin(),
+                       state_.components.template citer<Branch3>().end(), comp_topo.branch3_node_idx.begin(),
+                       [this](Branch3 const& branch3) {
+                           return Branch3Idx{state_.components.template get_seq<Node>(branch3.node_1()),
+                                             state_.components.template get_seq<Node>(branch3.node_2()),
+                                             state_.components.template get_seq<Node>(branch3.node_3())};
+                       });
+        comp_topo.source_node_idx.resize(state_.components.template size<Source>());
+        std::transform(state_.components.template citer<Source>().begin(),
+                       state_.components.template citer<Source>().end(), comp_topo.source_node_idx.begin(),
+                       [this](Source const& source) {
+                           return state_.components.template get_seq<Node>(source.node());
+                       });
+        comp_topo.shunt_node_idx.resize(state_.components.template size<Shunt>());
+        std::transform(state_.components.template citer<Shunt>().begin(),
+                       state_.components.template citer<Shunt>().end(), comp_topo.shunt_node_idx.begin(),
+                       [this](Shunt const& shunt) {
+                           return state_.components.template get_seq<Node>(shunt.node());
+                       });
+        comp_topo.load_gen_node_idx.resize(state_.components.template size<GenericLoadGen>());
+        std::transform(state_.components.template citer<GenericLoadGen>().begin(),
+                       state_.components.template citer<GenericLoadGen>().end(), comp_topo.load_gen_node_idx.begin(),
                        [this](GenericLoadGen const& load_gen) {
-                           return components_.template get_seq<Node>(load_gen.node());
+                           return state_.components.template get_seq<Node>(load_gen.node());
                        });
-        comp_topo.load_gen_type.resize(components_.template size<GenericLoadGen>());
-        std::transform(components_.template citer<GenericLoadGen>().begin(),
-                       components_.template citer<GenericLoadGen>().end(), comp_topo.load_gen_type.begin(),
+        comp_topo.load_gen_type.resize(state_.components.template size<GenericLoadGen>());
+        std::transform(state_.components.template citer<GenericLoadGen>().begin(),
+                       state_.components.template citer<GenericLoadGen>().end(), comp_topo.load_gen_type.begin(),
                        [](GenericLoadGen const& load_gen) {
                            return load_gen.type();
                        });
-        comp_topo.voltage_sensor_node_idx.resize(components_.template size<GenericVoltageSensor>());
-        std::transform(components_.template citer<GenericVoltageSensor>().begin(),
-                       components_.template citer<GenericVoltageSensor>().end(),
+        comp_topo.voltage_sensor_node_idx.resize(state_.components.template size<GenericVoltageSensor>());
+        std::transform(state_.components.template citer<GenericVoltageSensor>().begin(),
+                       state_.components.template citer<GenericVoltageSensor>().end(),
                        comp_topo.voltage_sensor_node_idx.begin(), [this](GenericVoltageSensor const& voltage_sensor) {
-                           return components_.template get_seq<Node>(voltage_sensor.measured_object());
-                       });
-        comp_topo.power_sensor_object_idx.resize(components_.template size<GenericPowerSensor>());
-        std::transform(components_.template citer<GenericPowerSensor>().begin(),
-                       components_.template citer<GenericPowerSensor>().end(),
-                       comp_topo.power_sensor_object_idx.begin(), [this](GenericPowerSensor const& power_sensor) {
-                           switch (power_sensor.get_terminal_type()) {
-                               using enum MeasuredTerminalType;
-
-                               case branch_from:
-                               case branch_to:
-                                   return components_.template get_seq<Branch>(power_sensor.measured_object());
-                               case source:
-                                   return components_.template get_seq<Source>(power_sensor.measured_object());
-                               case shunt:
-                                   return components_.template get_seq<Shunt>(power_sensor.measured_object());
-                               case load:
-                               case generator:
-                                   return components_.template get_seq<GenericLoadGen>(power_sensor.measured_object());
-                               case branch3_1:
-                               case branch3_2:
-                               case branch3_3:
-                                   return components_.template get_seq<Branch3>(power_sensor.measured_object());
-                               case node:
-                                   return components_.template get_seq<Node>(power_sensor.measured_object());
-                               default:
-                                   throw MissingCaseForEnumError("Power sensor idx to seq transformation",
-                                                                 power_sensor.get_terminal_type());
-                           }
+                           return state_.components.template get_seq<Node>(voltage_sensor.measured_object());
                        });
-        comp_topo.power_sensor_terminal_type.resize(components_.template size<GenericPowerSensor>());
-        std::transform(components_.template citer<GenericPowerSensor>().begin(),
-                       components_.template citer<GenericPowerSensor>().end(),
+        comp_topo.power_sensor_object_idx.resize(state_.components.template size<GenericPowerSensor>());
+        std::transform(
+            state_.components.template citer<GenericPowerSensor>().begin(),
+            state_.components.template citer<GenericPowerSensor>().end(), comp_topo.power_sensor_object_idx.begin(),
+            [this](GenericPowerSensor const& power_sensor) {
+                switch (power_sensor.get_terminal_type()) {
+                    using enum MeasuredTerminalType;
+
+                    case branch_from:
+                    case branch_to:
+                        return state_.components.template get_seq<Branch>(power_sensor.measured_object());
+                    case source:
+                        return state_.components.template get_seq<Source>(power_sensor.measured_object());
+                    case shunt:
+                        return state_.components.template get_seq<Shunt>(power_sensor.measured_object());
+                    case load:
+                    case generator:
+                        return state_.components.template get_seq<GenericLoadGen>(power_sensor.measured_object());
+                    case branch3_1:
+                    case branch3_2:
+                    case branch3_3:
+                        return state_.components.template get_seq<Branch3>(power_sensor.measured_object());
+                    case node:
+                        return state_.components.template get_seq<Node>(power_sensor.measured_object());
+                    default:
+                        throw MissingCaseForEnumError("Power sensor idx to seq transformation",
+                                                      power_sensor.get_terminal_type());
+                }
+            });
+        comp_topo.power_sensor_terminal_type.resize(state_.components.template size<GenericPowerSensor>());
+        std::transform(state_.components.template citer<GenericPowerSensor>().begin(),
+                       state_.components.template citer<GenericPowerSensor>().end(),
                        comp_topo.power_sensor_terminal_type.begin(), [](GenericPowerSensor const& power_sensor) {
                            return power_sensor.get_terminal_type();
                        });
-        comp_topo_ = std::make_shared<ComponentTopology const>(std::move(comp_topo));
+        state_.comp_topo = std::make_shared<ComponentTopology const>(std::move(comp_topo));
     }
 
     void reset_solvers() {
         assert(construction_complete_);
         is_topology_up_to_date_ = false;
         is_sym_parameter_up_to_date_ = false;
         is_asym_parameter_up_to_date_ = false;
         n_math_solvers_ = 0;
         sym_solvers_.clear();
         asym_solvers_.clear();
         math_topology_.clear();
-        comp_coup_.reset();
+        state_.comp_coup.reset();
     }
 
     /*
     the the sequence indexer given an input array of ID's for a given component type
     */
     void get_indexer(std::string const& component_type, ID const* id_begin, Idx size, Idx* indexer_begin) const {
         // static function array
         static constexpr std::array<GetIndexerFunc, n_types> get_indexer_func{
             [](MainModelImpl const& model, ID const* id_begin_, Idx size_, Idx* indexer_begin_) {
                 std::transform(id_begin_, id_begin_ + size_, indexer_begin_, [&model](ID id) {
-                    return model.components_.template get_idx_by_id<ComponentType>(id).pos;
+                    return model.state_.components.template get_idx_by_id<ComponentType>(id).pos;
                 });
             }...};
         // search component type name
         for (ComponentEntry const& entry : AllComponents::component_index_map) {
             if (entry.name == component_type) {
                 return get_indexer_func[entry.index](*this, id_begin, size, indexer_begin);
             }
@@ -489,15 +404,15 @@
                     return {};
                 }
                 // begin and end of the first batch
                 auto const [it_begin, it_end] = component_update.template get_iterators<UpdateType>(0);
                 // vector
                 std::vector<Idx2D> seq_idx(std::distance(it_begin, it_end));
                 std::transform(it_begin, it_end, seq_idx.begin(), [&model](UpdateType const& update) {
-                    return model.components_.template get_idx_by_id<ComponentType>(update.id);
+                    return model.state_.components.template get_idx_by_id<ComponentType>(update.id);
                 });
                 return seq_idx;
             }...};
 
         // fill in the map per component type
         std::map<std::string, std::vector<Idx2D>> sequence_idx_map;
         for (ComponentEntry const& entry : AllComponents::component_index_map) {
@@ -728,248 +643,63 @@
     BatchParameter calculate_state_estimation(double err_tol, Idx max_iter, CalculationMethod calculation_method,
                                               Dataset const& result_data, ConstDataset const& update_data,
                                               Idx threading = -1) {
         return batch_calculation_<sym, &MainModelImpl::calculate_state_estimation_<sym>>(
             err_tol, max_iter, calculation_method, result_data, update_data, threading);
     }
 
-    // output node
-    template <bool sym, std::same_as<Node> Component, std::forward_iterator ResIt>
-    ResIt output_result(std::vector<MathOutput<sym>> const& math_output, ResIt res_it) {
+    template <typename Component, math_output_type MathOutputType, std::forward_iterator ResIt>
+    ResIt output_result(std::vector<MathOutputType> const& math_output, ResIt res_it) {
         assert(construction_complete_);
-        return std::transform(components_.template citer<Component>().begin(),
-                              components_.template citer<Component>().end(), comp_coup_->node.cbegin(), res_it,
-                              [&math_output](Node const& node, Idx2D math_id) {
-                                  if (math_id.group == -1) {
-                                      return node.get_null_output<sym>();
-                                  }
-                                  return node.get_output<sym>(math_output[math_id.group].u[math_id.pos],
-                                                              math_output[math_id.group].bus_injection[math_id.pos]);
-                              });
+        return main_core::output_result<Component, ComponentContainer>(state_, math_output, res_it);
     }
 
-    // output branch
-    template <bool sym, std::derived_from<Branch> Component, std::forward_iterator ResIt>
-    ResIt output_result(std::vector<MathOutput<sym>> const& math_output, ResIt res_it) {
-        assert(construction_complete_);
-        return std::transform(components_.template citer<Component>().begin(),
-                              components_.template citer<Component>().end(),
-                              comp_coup_->branch.cbegin() + components_.template get_start_idx<Branch, Component>(),
-                              res_it, [&math_output](Branch const& branch, Idx2D math_id) {
-                                  if (math_id.group == -1) {
-                                      return branch.get_null_output<sym>();
-                                  }
-                                  return branch.get_output<sym>(math_output[math_id.group].branch[math_id.pos]);
-                              });
-    }
-
-    // output branch3
-    template <bool sym, std::derived_from<Branch3> Component, std::forward_iterator ResIt>
-    ResIt output_result(std::vector<MathOutput<sym>> const& math_output, ResIt res_it) {
-        assert(construction_complete_);
-        return std::transform(components_.template citer<Component>().begin(),
-                              components_.template citer<Component>().end(),
-                              comp_coup_->branch3.cbegin() + components_.template get_start_idx<Branch3, Component>(),
-                              res_it, [&math_output](Branch3 const& branch3, Idx2DBranch3 math_id) {
-                                  if (math_id.group == -1) {
-                                      return branch3.get_null_output<sym>();
-                                  }
-
-                                  return branch3.get_output<sym>(math_output[math_id.group].branch[math_id.pos[0]],
-                                                                 math_output[math_id.group].branch[math_id.pos[1]],
-                                                                 math_output[math_id.group].branch[math_id.pos[2]]);
-                              });
-    }
-
-    // output source, load_gen, shunt individually
-    template <bool sym, std::same_as<Appliance> Component, std::forward_iterator ResIt>
-    ResIt output_result(std::vector<MathOutput<sym>> const& math_output, ResIt res_it) {
-        assert(construction_complete_);
-        res_it = output_result<sym, Source>(math_output, res_it);
-        res_it = output_result<sym, GenericLoadGen>(math_output, res_it);
-        res_it = output_result<sym, Shunt>(math_output, res_it);
-        return res_it;
-    }
-
-    // output source
-    template <bool sym, std::same_as<Source> Component, std::forward_iterator ResIt>
-    ResIt output_result(std::vector<MathOutput<sym>> const& math_output, ResIt res_it) {
-        assert(construction_complete_);
-        return std::transform(components_.template citer<Component>().begin(),
-                              components_.template citer<Component>().end(), comp_coup_->source.cbegin(), res_it,
-                              [&math_output](Source const& source, Idx2D math_id) {
-                                  if (math_id.group == -1) {
-                                      return source.get_null_output<sym>();
-                                  }
-                                  return source.get_output<sym>(math_output[math_id.group].source[math_id.pos]);
-                              });
-    }
-
-    // output load gen
-    template <bool sym, std::derived_from<GenericLoadGen> Component, std::forward_iterator ResIt>
-    ResIt output_result(std::vector<MathOutput<sym>> const& math_output, ResIt res_it) {
-        assert(construction_complete_);
-        return std::transform(
-            components_.template citer<Component>().begin(), components_.template citer<Component>().end(),
-            comp_coup_->load_gen.cbegin() + components_.template get_start_idx<GenericLoadGen, Component>(), res_it,
-            [&math_output](GenericLoadGen const& load_gen, Idx2D math_id) {
-                if (math_id.group == -1) {
-                    return load_gen.get_null_output<sym>();
-                }
-                return load_gen.get_output<sym>(math_output[math_id.group].load_gen[math_id.pos]);
-            });
-    }
-
-    // output shunt
-    template <bool sym, std::same_as<Shunt> Component, std::forward_iterator ResIt>
-    ResIt output_result(std::vector<MathOutput<sym>> const& math_output, ResIt res_it) {
-        assert(construction_complete_);
-        return std::transform(components_.template citer<Component>().begin(),
-                              components_.template citer<Component>().end(), comp_coup_->shunt.cbegin(), res_it,
-                              [&math_output](Shunt const& shunt, Idx2D math_id) {
-                                  if (math_id.group == -1) {
-                                      return shunt.get_null_output<sym>();
-                                  }
-                                  return shunt.get_output<sym>(math_output[math_id.group].shunt[math_id.pos]);
-                              });
-    }
-
-    // output voltage sensor
-    template <bool sym, std::derived_from<GenericVoltageSensor> Component, std::forward_iterator ResIt>
-    ResIt output_result(std::vector<MathOutput<sym>> const& math_output, ResIt res_it) {
-        assert(construction_complete_);
-        return std::transform(
-            components_.template citer<Component>().begin(), components_.template citer<Component>().end(),
-            comp_topo_->voltage_sensor_node_idx.cbegin() +
-                components_.template get_start_idx<GenericVoltageSensor, Component>(),
-            res_it, [this, &math_output](GenericVoltageSensor const& voltage_sensor, Idx const node_seq) {
-                Idx2D const node_math_id = comp_coup_->node[node_seq];
-                if (node_math_id.group == -1) {
-                    return voltage_sensor.get_null_output<sym>();
-                }
-                return voltage_sensor.get_output<sym>(math_output[node_math_id.group].u[node_math_id.pos]);
-            });
-    }
-
-    // output power sensor
-    template <bool sym, std::derived_from<GenericPowerSensor> Component, std::forward_iterator ResIt>
-    ResIt output_result(std::vector<MathOutput<sym>> const& math_output, ResIt res_it) {
-        assert(construction_complete_);
-        return std::transform(
-            components_.template citer<Component>().begin(), components_.template citer<Component>().end(),
-            comp_topo_->power_sensor_object_idx.cbegin() +
-                components_.template get_start_idx<GenericPowerSensor, Component>(),
-            res_it, [this, &math_output](GenericPowerSensor const& power_sensor, Idx const obj_seq) {
-                auto const terminal_type = power_sensor.get_terminal_type();
-                Idx2D const obj_math_id = [&]() {
-                    switch (terminal_type) {
-                        using enum MeasuredTerminalType;
-
-                        case branch_from:
-                        case branch_to:
-                            return comp_coup_->branch[obj_seq];
-                        case source:
-                            return comp_coup_->source[obj_seq];
-                        case shunt:
-                            return comp_coup_->shunt[obj_seq];
-                        case load:
-                        case generator:
-                            return comp_coup_->load_gen[obj_seq];
-                        // from branch3, get relevant math object branch based on the measured side
-                        case branch3_1:
-                            return Idx2D{comp_coup_->branch3[obj_seq].group, comp_coup_->branch3[obj_seq].pos[0]};
-                        case branch3_2:
-                            return Idx2D{comp_coup_->branch3[obj_seq].group, comp_coup_->branch3[obj_seq].pos[1]};
-                        case branch3_3:
-                            return Idx2D{comp_coup_->branch3[obj_seq].group, comp_coup_->branch3[obj_seq].pos[2]};
-                        case node:
-                            return comp_coup_->node[obj_seq];
-                        default:
-                            throw MissingCaseForEnumError(std::string(GenericPowerSensor::name) + " output_result()",
-                                                          terminal_type);
-                    }
-                }();
-
-                if (obj_math_id.group == -1) {
-                    return power_sensor.get_null_output<sym>();
-                }
-
-                switch (terminal_type) {
-                    using enum MeasuredTerminalType;
-
-                    case branch_from:
-                    // all power sensors in branch3 are at from side in the mathematical model
-                    case branch3_1:
-                    case branch3_2:
-                    case branch3_3:
-                        return power_sensor.get_output<sym>(math_output[obj_math_id.group].branch[obj_math_id.pos].s_f);
-                    case branch_to:
-                        return power_sensor.get_output<sym>(math_output[obj_math_id.group].branch[obj_math_id.pos].s_t);
-                    case source:
-                        return power_sensor.get_output<sym>(math_output[obj_math_id.group].source[obj_math_id.pos].s);
-                    case shunt:
-                        return power_sensor.get_output<sym>(math_output[obj_math_id.group].shunt[obj_math_id.pos].s);
-                    case load:
-                    case generator:
-                        return power_sensor.get_output<sym>(math_output[obj_math_id.group].load_gen[obj_math_id.pos].s);
-                    case node:
-                        return power_sensor.get_output<sym>(
-                            math_output[obj_math_id.group].bus_injection[obj_math_id.pos]);
-                    default:
-                        throw MissingCaseForEnumError(std::string(GenericPowerSensor::name) + " output_result()",
-                                                      terminal_type);
-                }
-            });
-    }
-
-    // output fault
-    template <bool sym, class Component, class ResIt>
-    std::enable_if_t<
-        std::is_base_of_v<std::forward_iterator_tag, typename std::iterator_traits<ResIt>::iterator_category> &&
-            std::is_same_v<Fault, Component>,
-        ResIt>
-    output_result(std::vector<MathOutput<sym>> const& /* math_output */, ResIt res_it) {
-        assert(construction_complete_);
-        return std::transform(components_.template citer<Component>().begin(),
-                              components_.template citer<Component>().end(), comp_coup_->fault.cbegin(), res_it,
-                              [](Fault const& fault, Idx2D /* math_id */) {
-                                  return fault.get_output();
-                              });
-    }
-
-    template <bool sym>
-    void output_result(std::vector<MathOutput<sym>> const& math_output, Dataset const& result_data, Idx pos = 0) {
-        static constexpr std::array<OutputFunc<sym>, n_types> get_result{
-            [](MainModelImpl& model, std::vector<MathOutput<sym>> const& math_output_,
+    template <math_output_type MathOutputType>
+    void output_result(std::vector<MathOutputType> const& math_output, Dataset const& result_data, Idx pos = 0) {
+        static constexpr std::array<OutputFunc<MathOutputType>, n_types> get_result{
+            [](MainModelImpl& model, std::vector<MathOutputType> const& math_output_,
                DataPointer<false> const& data_ptr, Idx position) {
                 auto const begin =
-                    data_ptr.get_iterators<typename ComponentType::template OutputType<sym>>(position).first;
-                model.output_result<sym, ComponentType>(math_output_, begin);
+                    data_ptr
+                        .get_iterators<std::conditional_t<
+                            steady_state_math_output_type<MathOutputType>,
+                            typename ComponentType::template OutputType<symmetric_math_output_type<MathOutputType>>,
+                            typename ComponentType::ShortCircuitOutputType>>(position)
+                        .first;
+                model.output_result<ComponentType>(math_output_, begin);
             }...};
         for (ComponentEntry const& entry : AllComponents::component_index_map) {
             auto const found = result_data.find(entry.name);
             // skip if component does not exist
             if (found == result_data.cend()) {
                 continue;
             }
             // update
             get_result[entry.index](*this, math_output, found->second, pos);
         }
     }
 
+    template <bool sym, typename Component, std::forward_iterator ResIt>
+    ResIt output_result(std::vector<MathOutput<sym>> const& math_output, ResIt res_it) {
+        return output_result<Component, MathOutput<sym>, ResIt>(math_output, res_it);
+    }
+
+    template <bool sym>
+    void output_result(std::vector<MathOutput<sym>> const& math_output, Dataset const& result_data, Idx pos = 0) {
+        return output_result<MathOutput<sym>>(math_output, result_data, pos);
+    }
+
     CalculationInfo calculation_info() {
         return calculation_info_;
     }
 
    private:
     double system_frequency_;
-    ComponentContainer components_;
-    // calculation parameters
-    std::shared_ptr<ComponentTopology const> comp_topo_;
-    std::shared_ptr<ComponentToMathCoupling const> comp_coup_;
+
+    MainModelState state_;
     // math model
     std::vector<std::shared_ptr<MathModelTopology const>> math_topology_;
     std::vector<MathSolver<true>> sym_solvers_;
     std::vector<MathSolver<false>> asym_solvers_;
     Idx n_math_solvers_{0};
     bool is_topology_up_to_date_{false};
     bool is_sym_parameter_up_to_date_{false};
@@ -1003,45 +733,48 @@
 
     void rebuild_topology() {
         assert(construction_complete_);
         // clear old solvers
         reset_solvers();
         // get connection info
         ComponentConnections comp_conn;
-        comp_conn.branch_connected.resize(comp_topo_->branch_node_idx.size());
-        comp_conn.branch_phase_shift.resize(comp_topo_->branch_node_idx.size());
-        comp_conn.branch3_connected.resize(comp_topo_->branch3_node_idx.size());
-        comp_conn.branch3_phase_shift.resize(comp_topo_->branch3_node_idx.size());
-        comp_conn.source_connected.resize(comp_topo_->source_node_idx.size());
+        comp_conn.branch_connected.resize(state_.comp_topo->branch_node_idx.size());
+        comp_conn.branch_phase_shift.resize(state_.comp_topo->branch_node_idx.size());
+        comp_conn.branch3_connected.resize(state_.comp_topo->branch3_node_idx.size());
+        comp_conn.branch3_phase_shift.resize(state_.comp_topo->branch3_node_idx.size());
+        comp_conn.source_connected.resize(state_.comp_topo->source_node_idx.size());
         std::transform(
-            components_.template citer<Branch>().begin(), components_.template citer<Branch>().end(),
+            state_.components.template citer<Branch>().begin(), state_.components.template citer<Branch>().end(),
             comp_conn.branch_connected.begin(), [](Branch const& branch) {
                 return BranchConnected{static_cast<IntS>(branch.from_status()), static_cast<IntS>(branch.to_status())};
             });
-        std::transform(components_.template citer<Branch>().begin(), components_.template citer<Branch>().end(),
-                       comp_conn.branch_phase_shift.begin(), [](Branch const& branch) {
+        std::transform(state_.components.template citer<Branch>().begin(),
+                       state_.components.template citer<Branch>().end(), comp_conn.branch_phase_shift.begin(),
+                       [](Branch const& branch) {
                            return branch.phase_shift();
                        });
-        std::transform(components_.template citer<Branch3>().begin(), components_.template citer<Branch3>().end(),
-                       comp_conn.branch3_connected.begin(), [](Branch3 const& branch3) {
-                           return Branch3Connected{static_cast<IntS>(branch3.status_1()),
-                                                   static_cast<IntS>(branch3.status_2()),
-                                                   static_cast<IntS>(branch3.status_3())};
-                       });
-        std::transform(components_.template citer<Branch3>().begin(), components_.template citer<Branch3>().end(),
-                       comp_conn.branch3_phase_shift.begin(), [](Branch3 const& branch3) {
+        std::transform(
+            state_.components.template citer<Branch3>().begin(), state_.components.template citer<Branch3>().end(),
+            comp_conn.branch3_connected.begin(), [](Branch3 const& branch3) {
+                return Branch3Connected{static_cast<IntS>(branch3.status_1()), static_cast<IntS>(branch3.status_2()),
+                                        static_cast<IntS>(branch3.status_3())};
+            });
+        std::transform(state_.components.template citer<Branch3>().begin(),
+                       state_.components.template citer<Branch3>().end(), comp_conn.branch3_phase_shift.begin(),
+                       [](Branch3 const& branch3) {
                            return branch3.phase_shift();
                        });
-        std::transform(components_.template citer<Source>().begin(), components_.template citer<Source>().end(),
-                       comp_conn.source_connected.begin(), [](Source const& source) {
+        std::transform(state_.components.template citer<Source>().begin(),
+                       state_.components.template citer<Source>().end(), comp_conn.source_connected.begin(),
+                       [](Source const& source) {
                            return source.status();
                        });
         // re build
-        Topology topology{*comp_topo_, comp_conn};
-        std::tie(math_topology_, comp_coup_) = topology.build_topology();
+        Topology topology{*state_.comp_topo, comp_conn};
+        std::tie(math_topology_, state_.comp_coup) = topology.build_topology();
         n_math_solvers_ = (Idx)math_topology_.size();
         is_topology_up_to_date_ = true;
         is_sym_parameter_up_to_date_ = false;
         is_asym_parameter_up_to_date_ = false;
     }
 
     template <bool sym>
@@ -1049,54 +782,55 @@
         std::vector<MathModelParam<sym>> math_param(n_math_solvers_);
         for (Idx i = 0; i != n_math_solvers_; ++i) {
             math_param[i].branch_param.resize(math_topology_[i]->n_branch());
             math_param[i].shunt_param.resize(math_topology_[i]->n_shunt());
             math_param[i].source_param.resize(math_topology_[i]->n_source());
         }
         // loop all branch
-        for (Idx i = 0; i != (Idx)comp_topo_->branch_node_idx.size(); ++i) {
-            Idx2D const math_idx = comp_coup_->branch[i];
+        for (Idx i = 0; i != (Idx)state_.comp_topo->branch_node_idx.size(); ++i) {
+            Idx2D const math_idx = state_.comp_coup->branch[i];
             if (math_idx.group == -1) {
                 continue;
             }
             // assign parameters
             math_param[math_idx.group].branch_param[math_idx.pos] =
-                components_.template get_item_by_seq<Branch>(i).template calc_param<sym>();
+                state_.components.template get_item_by_seq<Branch>(i).template calc_param<sym>();
         }
         // loop all branch3
-        for (Idx i = 0; i != (Idx)comp_topo_->branch3_node_idx.size(); ++i) {
-            Idx2DBranch3 const math_idx = comp_coup_->branch3[i];
+        for (Idx i = 0; i != (Idx)state_.comp_topo->branch3_node_idx.size(); ++i) {
+            Idx2DBranch3 const math_idx = state_.comp_coup->branch3[i];
             if (math_idx.group == -1) {
                 continue;
             }
             // assign parameters, branch3 param consists of three branch parameters
-            auto const branch3_param = components_.template get_item_by_seq<Branch3>(i).template calc_param<sym>();
+            auto const branch3_param =
+                state_.components.template get_item_by_seq<Branch3>(i).template calc_param<sym>();
             for (size_t branch2 = 0; branch2 < 3; ++branch2) {
                 math_param[math_idx.group].branch_param[math_idx.pos[branch2]] = branch3_param[branch2];
             }
         }
         // loop all shunt
-        for (Idx i = 0; i != (Idx)comp_topo_->shunt_node_idx.size(); ++i) {
-            Idx2D const math_idx = comp_coup_->shunt[i];
+        for (Idx i = 0; i != (Idx)state_.comp_topo->shunt_node_idx.size(); ++i) {
+            Idx2D const math_idx = state_.comp_coup->shunt[i];
             if (math_idx.group == -1) {
                 continue;
             }
             // assign parameters
             math_param[math_idx.group].shunt_param[math_idx.pos] =
-                components_.template get_item_by_seq<Shunt>(i).template calc_param<sym>();
+                state_.components.template get_item_by_seq<Shunt>(i).template calc_param<sym>();
         }
         // loop all source
-        for (Idx i = 0; i != (Idx)comp_topo_->source_node_idx.size(); ++i) {
-            Idx2D const math_idx = comp_coup_->source[i];
+        for (Idx i = 0; i != (Idx)state_.comp_topo->source_node_idx.size(); ++i) {
+            Idx2D const math_idx = state_.comp_coup->source[i];
             if (math_idx.group == -1) {
                 continue;
             }
             // assign parameters
             math_param[math_idx.group].source_param[math_idx.pos] =
-                components_.template get_item_by_seq<Source>(i).template math_param<sym>();
+                state_.components.template get_item_by_seq<Source>(i).template math_param<sym>();
         }
         return math_param;
     }
 
     static constexpr auto include_all = [](Idx) {
         return true;
     };
@@ -1108,15 +842,15 @@
      * model and all of them are filled within the same function call (i.e. Notice that calc_input is a vector).
      *
      *  1. For each component, check if it should be included.
      *     By default, all component are included, except for some cases, like power sensors. For power sensors, the
      *     list of component contains all power sensors, but the preparation should only be done for one type of power
      *     sensors at a time. Therefore, `included` will be a lambda function, such as:
      *
-     *       [this](Idx i) { return comp_topo_->power_sensor_terminal_type[i] == MeasuredTerminalType::source; }
+     *       [this](Idx i) { return state_.comp_topo->power_sensor_terminal_type[i] == MeasuredTerminalType::source; }
      *
      *  2. Find the original component in the topology and retrieve its calculation parameters.
      *
      *  3. Fill the calculation parameters of the right math model.
      *
      *
      *  @tparam sym
@@ -1137,15 +871,15 @@
      * 	    The component type for which we are collecting calculation parameters
      *
      * @tparam PredicateIn
      * 	    The lambda function type. The actual type depends on the captured variables, and will be automatically
      * 	    deduced.
      *
      * @param component[in]
-     *      The vector of component math indices to consider (e.g. comp_coup_->source).
+     *      The vector of component math indices to consider (e.g. state_.comp_coup->source).
      *      When idx.group = -1, the original component is not assigned to a math model, so we can skip it.
      *
      * @param calc_input[out]
      *		Although this variable is called `input`, it is actually the output of this function, it stored the
      *		calculation parameters for each math model, for each component of type ComponentIn.
      *
      * @param include
@@ -1158,15 +892,15 @@
     void prepare_input(std::vector<Idx2D> const& components, std::vector<CalcStructOut>& calc_input,
                        PredicateIn include = include_all) {
         for (Idx i = 0, n = (Idx)components.size(); i != n; ++i) {
             if (include(i)) {
                 Idx2D const math_idx = components[i];
                 if (math_idx.group != -1) {
                     CalcParamOut const calc_param =
-                        components_.template get_item_by_seq<ComponentIn>(i).template calc_param<sym>();
+                        state_.components.template get_item_by_seq<ComponentIn>(i).template calc_param<sym>();
                     CalcStructOut& math_model_input = calc_input[math_idx.group];
                     std::vector<CalcParamOut>& math_model_input_vect = math_model_input.*comp_vect;
                     math_model_input_vect[math_idx.pos] = calc_param;
                 }
             }
         }
     }
@@ -1175,31 +909,31 @@
     void prepare_input_status(std::vector<Idx2D> const& objects, std::vector<StateEstimationInput<sym>>& input) {
         for (Idx i = 0, n = (Idx)objects.size(); i != n; ++i) {
             Idx2D const math_idx = objects[i];
             if (math_idx.group == -1) {
                 continue;
             }
             (input[math_idx.group].*component)[math_idx.pos] =
-                components_.template get_item_by_seq<Component>(i).status();
+                state_.components.template get_item_by_seq<Component>(i).status();
         }
     }
 
     template <bool sym>
     std::vector<PowerFlowInput<sym>> prepare_power_flow_input() {
         assert(is_topology_up_to_date_ && is_parameter_up_to_date<sym>());
         std::vector<PowerFlowInput<sym>> pf_input(n_math_solvers_);
         for (Idx i = 0; i != n_math_solvers_; ++i) {
             pf_input[i].s_injection.resize(math_topology_[i]->n_load_gen());
             pf_input[i].source.resize(math_topology_[i]->n_source());
         }
-        prepare_input<sym, PowerFlowInput<sym>, DoubleComplex, &PowerFlowInput<sym>::source, Source>(comp_coup_->source,
-                                                                                                     pf_input);
+        prepare_input<sym, PowerFlowInput<sym>, DoubleComplex, &PowerFlowInput<sym>::source, Source>(
+            state_.comp_coup->source, pf_input);
 
         prepare_input<sym, PowerFlowInput<sym>, ComplexValue<sym>, &PowerFlowInput<sym>::s_injection, GenericLoadGen>(
-            comp_coup_->load_gen, pf_input);
+            state_.comp_coup->load_gen, pf_input);
 
         return pf_input;
     }
 
     template <bool sym>
     std::vector<StateEstimationInput<sym>> prepare_state_estimation_input() {
         assert(is_topology_up_to_date_ && is_parameter_up_to_date<sym>());
@@ -1215,56 +949,57 @@
             se_input[i].measured_load_gen_power.resize(math_topology_[i]->n_load_gen_power_sensor());
             se_input[i].measured_shunt_power.resize(math_topology_[i]->n_shunt_power_power_sensor());
             se_input[i].measured_branch_from_power.resize(math_topology_[i]->n_branch_from_power_sensor());
             se_input[i].measured_branch_to_power.resize(math_topology_[i]->n_branch_to_power_sensor());
             se_input[i].measured_bus_injection.resize(math_topology_[i]->n_bus_power_sensor());
         }
 
-        prepare_input_status<sym, &StateEstimationInput<sym>::shunt_status, Shunt>(comp_coup_->shunt, se_input);
-        prepare_input_status<sym, &StateEstimationInput<sym>::load_gen_status, GenericLoadGen>(comp_coup_->load_gen,
-                                                                                               se_input);
-        prepare_input_status<sym, &StateEstimationInput<sym>::source_status, Source>(comp_coup_->source, se_input);
+        prepare_input_status<sym, &StateEstimationInput<sym>::shunt_status, Shunt>(state_.comp_coup->shunt, se_input);
+        prepare_input_status<sym, &StateEstimationInput<sym>::load_gen_status, GenericLoadGen>(
+            state_.comp_coup->load_gen, se_input);
+        prepare_input_status<sym, &StateEstimationInput<sym>::source_status, Source>(state_.comp_coup->source,
+                                                                                     se_input);
 
         prepare_input<sym, StateEstimationInput<sym>, SensorCalcParam<sym>,
-                      &StateEstimationInput<sym>::measured_voltage, GenericVoltageSensor>(comp_coup_->voltage_sensor,
-                                                                                          se_input);
+                      &StateEstimationInput<sym>::measured_voltage, GenericVoltageSensor>(
+            state_.comp_coup->voltage_sensor, se_input);
         prepare_input<sym, StateEstimationInput<sym>, SensorCalcParam<sym>,
                       &StateEstimationInput<sym>::measured_source_power, GenericPowerSensor>(
-            comp_coup_->power_sensor, se_input, [this](Idx i) {
-                return comp_topo_->power_sensor_terminal_type[i] == MeasuredTerminalType::source;
+            state_.comp_coup->power_sensor, se_input, [this](Idx i) {
+                return state_.comp_topo->power_sensor_terminal_type[i] == MeasuredTerminalType::source;
             });
         prepare_input<sym, StateEstimationInput<sym>, SensorCalcParam<sym>,
                       &StateEstimationInput<sym>::measured_load_gen_power, GenericPowerSensor>(
-            comp_coup_->power_sensor, se_input, [this](Idx i) {
-                return comp_topo_->power_sensor_terminal_type[i] == MeasuredTerminalType::load ||
-                       comp_topo_->power_sensor_terminal_type[i] == MeasuredTerminalType::generator;
+            state_.comp_coup->power_sensor, se_input, [this](Idx i) {
+                return state_.comp_topo->power_sensor_terminal_type[i] == MeasuredTerminalType::load ||
+                       state_.comp_topo->power_sensor_terminal_type[i] == MeasuredTerminalType::generator;
             });
         prepare_input<sym, StateEstimationInput<sym>, SensorCalcParam<sym>,
                       &StateEstimationInput<sym>::measured_shunt_power, GenericPowerSensor>(
-            comp_coup_->power_sensor, se_input, [this](Idx i) {
-                return comp_topo_->power_sensor_terminal_type[i] == MeasuredTerminalType::shunt;
+            state_.comp_coup->power_sensor, se_input, [this](Idx i) {
+                return state_.comp_topo->power_sensor_terminal_type[i] == MeasuredTerminalType::shunt;
             });
         prepare_input<sym, StateEstimationInput<sym>, SensorCalcParam<sym>,
                       &StateEstimationInput<sym>::measured_branch_from_power, GenericPowerSensor>(
-            comp_coup_->power_sensor, se_input, [this](Idx i) {
-                return comp_topo_->power_sensor_terminal_type[i] == MeasuredTerminalType::branch_from ||
+            state_.comp_coup->power_sensor, se_input, [this](Idx i) {
+                return state_.comp_topo->power_sensor_terminal_type[i] == MeasuredTerminalType::branch_from ||
                        // all branch3 sensors are at from side in the mathematical model
-                       comp_topo_->power_sensor_terminal_type[i] == MeasuredTerminalType::branch3_1 ||
-                       comp_topo_->power_sensor_terminal_type[i] == MeasuredTerminalType::branch3_2 ||
-                       comp_topo_->power_sensor_terminal_type[i] == MeasuredTerminalType::branch3_3;
+                       state_.comp_topo->power_sensor_terminal_type[i] == MeasuredTerminalType::branch3_1 ||
+                       state_.comp_topo->power_sensor_terminal_type[i] == MeasuredTerminalType::branch3_2 ||
+                       state_.comp_topo->power_sensor_terminal_type[i] == MeasuredTerminalType::branch3_3;
             });
         prepare_input<sym, StateEstimationInput<sym>, SensorCalcParam<sym>,
                       &StateEstimationInput<sym>::measured_branch_to_power, GenericPowerSensor>(
-            comp_coup_->power_sensor, se_input, [this](Idx i) {
-                return comp_topo_->power_sensor_terminal_type[i] == MeasuredTerminalType::branch_to;
+            state_.comp_coup->power_sensor, se_input, [this](Idx i) {
+                return state_.comp_topo->power_sensor_terminal_type[i] == MeasuredTerminalType::branch_to;
             });
         prepare_input<sym, StateEstimationInput<sym>, SensorCalcParam<sym>,
                       &StateEstimationInput<sym>::measured_bus_injection, GenericPowerSensor>(
-            comp_coup_->power_sensor, se_input, [this](Idx i) {
-                return comp_topo_->power_sensor_terminal_type[i] == MeasuredTerminalType::node;
+            state_.comp_coup->power_sensor, se_input, [this](Idx i) {
+                return state_.comp_topo->power_sensor_terminal_type[i] == MeasuredTerminalType::node;
             });
 
         return se_input;
     }
 
     template <bool sym>
     void prepare_solvers() {
```

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/block_matrix.hpp` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/block_matrix.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_current_pf_solver.hpp` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_current_pf_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_linear_se_solver.hpp` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_linear_se_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_pf_solver.hpp` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_pf_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/linear_pf_solver.hpp` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/linear_pf_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/math_solver.hpp` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/math_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_pf_solver.hpp` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_pf_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/short_circuit_solver.hpp` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/short_circuit_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/sparse_lu_solver.hpp` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/sparse_lu_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/y_bus.hpp` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/y_bus.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/power_grid_model.hpp` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/power_grid_model.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/sparse_mapping.hpp` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/sparse_mapping.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/three_phase_tensor.hpp` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/three_phase_tensor.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/timer.hpp` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/timer.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model/include/power_grid_model/topology.hpp` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model/include/power_grid_model/topology.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model_c/CMakeLists.txt` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model_c/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/basics.h` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/basics.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/buffer.h` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/buffer.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/dataset_definitions.h` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/dataset_definitions.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/handle.h` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/handle.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/meta_data.h` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/meta_data.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/model.h` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/model.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/options.h` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/options.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model_c/include/power_grid_model_c.h` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model_c/include/power_grid_model_c.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model_c/src/buffer.cpp` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model_c/src/buffer.cpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model_c/src/dataset_definitions.cpp` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model_c/src/dataset_definitions.cpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model_c/src/handle.cpp` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model_c/src/handle.cpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model_c/src/handle.hpp` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model_c/src/handle.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model_c/src/meta_data.cpp` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model_c/src/meta_data.cpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model_c/src/model.cpp` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model_c/src/model.cpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model_c/src/options.cpp` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model_c/src/options.cpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/power_grid_model_c/power_grid_model_c/src/options.hpp` & `power-grid-model-1.5.0rc9219310821193/power_grid_model_c/power_grid_model_c/src/options.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/pyproject.toml` & `power-grid-model-1.5.0rc9219310821193/pyproject.toml`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/setup.py` & `power-grid-model-1.5.0rc9219310821193/setup.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/src/power_grid_model/__init__.py` & `power-grid-model-1.5.0rc9219310821193/src/power_grid_model/__init__.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/src/power_grid_model/core/data_handling.py` & `power-grid-model-1.5.0rc9219310821193/src/power_grid_model/core/data_handling.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/src/power_grid_model/core/error_handling.py` & `power-grid-model-1.5.0rc9219310821193/src/power_grid_model/core/error_handling.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/src/power_grid_model/core/options.py` & `power-grid-model-1.5.0rc9219310821193/src/power_grid_model/core/options.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/src/power_grid_model/core/power_grid_core.py` & `power-grid-model-1.5.0rc9219310821193/src/power_grid_model/core/power_grid_core.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/src/power_grid_model/core/power_grid_meta.py` & `power-grid-model-1.5.0rc9219310821193/src/power_grid_model/core/power_grid_meta.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/src/power_grid_model/core/power_grid_model.py` & `power-grid-model-1.5.0rc9219310821193/src/power_grid_model/core/power_grid_model.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/src/power_grid_model/data_types.py` & `power-grid-model-1.5.0rc9219310821193/src/power_grid_model/data_types.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/src/power_grid_model/enum.py` & `power-grid-model-1.5.0rc9219310821193/src/power_grid_model/enum.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/src/power_grid_model/utils.py` & `power-grid-model-1.5.0rc9219310821193/src/power_grid_model/utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/src/power_grid_model/validation/__init__.py` & `power-grid-model-1.5.0rc9219310821193/src/power_grid_model/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/src/power_grid_model/validation/assertions.py` & `power-grid-model-1.5.0rc9219310821193/src/power_grid_model/validation/assertions.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/src/power_grid_model/validation/errors.py` & `power-grid-model-1.5.0rc9219310821193/src/power_grid_model/validation/errors.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/src/power_grid_model/validation/rules.py` & `power-grid-model-1.5.0rc9219310821193/src/power_grid_model/validation/rules.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/src/power_grid_model/validation/utils.py` & `power-grid-model-1.5.0rc9219310821193/src/power_grid_model/validation/utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/src/power_grid_model/validation/validation.py` & `power-grid-model-1.5.0rc9219310821193/src/power_grid_model/validation/validation.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/src/power_grid_model.egg-info/PKG-INFO` & `power-grid-model-1.5.0rc9219310821193/src/power_grid_model.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: power-grid-model
-Version: 1.5.0rc9216009937633
+Version: 1.5.0rc9219310821193
 Summary: Python/C++ library for distribution power system analysis
 Author-email: Alliander Dynamic Grid Calculation <dynamic.grid.calculation@alliander.com>
 License: MPL-2.0
 Project-URL: Home-page, https://lfenergy.org/projects/power-grid-model/
 Project-URL: GitHub, https://github.com/PowerGridModel/power-grid-model
 Project-URL: Documentation, https://power-grid-model.readthedocs.io/en/stable/
 Project-URL: Mailing-list, https://lists.lfenergy.org/g/powergridmodel
```

### Comparing `power-grid-model-1.5.0rc9216009937633/src/power_grid_model.egg-info/SOURCES.txt` & `power-grid-model-1.5.0rc9219310821193/src/power_grid_model.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,18 @@
 power_grid_model_c/power_grid_model/include/power_grid_model/component/sensor.hpp
 power_grid_model_c/power_grid_model/include/power_grid_model/component/shunt.hpp
 power_grid_model_c/power_grid_model/include/power_grid_model/component/source.hpp
 power_grid_model_c/power_grid_model/include/power_grid_model/component/three_winding_transformer.hpp
 power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer.hpp
 power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer_utils.hpp
 power_grid_model_c/power_grid_model/include/power_grid_model/component/voltage_sensor.hpp
+power_grid_model_c/power_grid_model/include/power_grid_model/main_core/input.hpp
+power_grid_model_c/power_grid_model/include/power_grid_model/main_core/output.hpp
+power_grid_model_c/power_grid_model/include/power_grid_model/main_core/state.hpp
+power_grid_model_c/power_grid_model/include/power_grid_model/main_core/update.hpp
 power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/block_matrix.hpp
 power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_current_pf_solver.hpp
 power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_linear_se_solver.hpp
 power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_pf_solver.hpp
 power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/linear_pf_solver.hpp
 power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/math_solver.hpp
 power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_pf_solver.hpp
```

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/1os2msr/input.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/1os2msr/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/1os2msr/sym_output.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/1os2msr/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test/input.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test/sym_output.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch/input.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-batch-newton/input.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-batch-newton/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-i-n-optional/input.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-i-n-optional/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/gaia-example/asym_output.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/gaia-example/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/gaia-example/gaia_grid.gnf` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/gaia-example/gaia_grid.gnf`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/gaia-example/input.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/gaia-example/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/multi-source-with-angle/input.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/multi-source-with-angle/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/README.md` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/asym_load/README.md` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/asym_load/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/line/README.md` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/line/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/line/input.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/line/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/node/README.md` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/node/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/node/input.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/node/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/shunt/README.md` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/shunt/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/source/README.md` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/source/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/source/input.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/source/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/README.md` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/sym_load/README.md` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/sym_load/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/transformer/README.md` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/transformer/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/line/README.md` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/line/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/line/input.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/line/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/node/input.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/node/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/source/input.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/source/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/sym_gen/README.md` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/sym_gen/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/sym_load/README.md` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/sym_load/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/README.md` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/transformer/README.md` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/transformer/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/README.md` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/README.md` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/README.md` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/README.md` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/r-state-estimation/input.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/r-state-estimation/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/r-state-estimation/sym_output.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/r-state-estimation/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/three-winding-transformer/asym_output_batch.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/three-winding-transformer/asym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/three-winding-transformer/input.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/three-winding-transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/three-winding-transformer/sym_output_batch.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/three-winding-transformer/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/three-winding-transformer/update_batch.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/three-winding-transformer/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/vision-example/asym_output.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/vision-example/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/vision-example/input.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/vision-example/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/vision-example/vision_grid.vnf` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/vision-example/vision_grid.vnf`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/vision-validation-network/asym_output.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/vision-validation-network/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/vision-validation-network/input.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/vision-validation-network/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/vision-validation-network/sym_output.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/vision-validation-network/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf` & `power-grid-model-1.5.0rc9219310821193/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/short_circuit/single_phase_to_ground/input.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/short_circuit/single_phase_to_ground/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/short_circuit/single_phase_to_ground/sc_output_batch.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/short_circuit/single_phase_to_ground/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/short_circuit/single_phase_to_ground/update_batch.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/short_circuit/single_phase_to_ground/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/short_circuit/three_phase/input.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/short_circuit/three_phase/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/short_circuit/three_phase/sc_output_batch.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/short_circuit/three_phase/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/short_circuit/three_phase/update_batch.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/short_circuit/three_phase/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/short_circuit/two_phase/input.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/short_circuit/two_phase/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/short_circuit/two_phase/sc_output_batch.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/short_circuit/two_phase/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/short_circuit/two_phase/update_batch.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/short_circuit/two_phase/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/short_circuit/two_phase_to_ground/input.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/short_circuit/two_phase_to_ground/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/short_circuit/two_phase_to_ground/sc_output_batch.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/short_circuit/two_phase_to_ground/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/short_circuit/two_phase_to_ground/update_batch.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/short_circuit/two_phase_to_ground/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/1os2msr/input.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/1os2msr/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/1os2msr/sym_output.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/1os2msr/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/1os2msr-no-angle/input.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/1os2msr-no-angle/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/1os2msr-no-angle/sym_output.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/1os2msr-no-angle/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/distribution-case/README.md` & `power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/distribution-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/distribution-case/input.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/distribution-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/distribution-case/sym_output_batch.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/distribution-case/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/distribution-case/update_batch.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/distribution-case/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/dummy-test-sym/input.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/dummy-test-sym/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/dummy-test-sym/sym_output.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/dummy-test-sym/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/single-line-load/input.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/single-line-load/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/single-line-load/sym_output.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/single-line-load/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/three_winding_transformer/input.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/three_winding_transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/three_winding_transformer/sym_output.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/three_winding_transformer/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/transmission-case/README.md` & `power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/transmission-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/transmission-case/asym_output.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/transmission-case/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/transmission-case/input.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/transmission-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/data/state_estimation/transmission-case/sym_output.json` & `power-grid-model-1.5.0rc9219310821193/tests/data/state_estimation/transmission-case/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/unit/test_0Z_model_validation.py` & `power-grid-model-1.5.0rc9219310821193/tests/unit/test_0Z_model_validation.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/unit/test_error_handling.py` & `power-grid-model-1.5.0rc9219310821193/tests/unit/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/unit/test_meta_data.py` & `power-grid-model-1.5.0rc9219310821193/tests/unit/test_meta_data.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/unit/test_power_grid_model.py` & `power-grid-model-1.5.0rc9219310821193/tests/unit/test_power_grid_model.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/unit/test_utils.py` & `power-grid-model-1.5.0rc9219310821193/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/unit/utils.py` & `power-grid-model-1.5.0rc9219310821193/tests/unit/utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/unit/validation/test_assertions.py` & `power-grid-model-1.5.0rc9219310821193/tests/unit/validation/test_assertions.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/unit/validation/test_batch_validation.py` & `power-grid-model-1.5.0rc9219310821193/tests/unit/validation/test_batch_validation.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/unit/validation/test_errors.py` & `power-grid-model-1.5.0rc9219310821193/tests/unit/validation/test_errors.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/unit/validation/test_input_validation.py` & `power-grid-model-1.5.0rc9219310821193/tests/unit/validation/test_input_validation.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/unit/validation/test_rules.py` & `power-grid-model-1.5.0rc9219310821193/tests/unit/validation/test_rules.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/unit/validation/test_utils.py` & `power-grid-model-1.5.0rc9219310821193/tests/unit/validation/test_utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9216009937633/tests/unit/validation/test_validation_functions.py` & `power-grid-model-1.5.0rc9219310821193/tests/unit/validation/test_validation_functions.py`

 * *Files identical despite different names*

