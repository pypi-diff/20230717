# Comparing `tmp/clover-energy-5.0.8.tar.gz` & `tmp/clover-energy-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/bewinche/modelling/CLOVER/dist/.tmp-1d4azq4f/clover-energy-5.0.8.tar", last modified: Fri Jul 14 14:29:36 2023, max compression
+gzip compressed data, was "/home/bewinche/modelling/CLOVER/dist/.tmp-2oap2u4h/clover-energy-5.1.0.tar", last modified: Mon Jul 17 11:13:50 2023, max compression
```

## Comparing `clover-energy-5.0.8.tar` & `clover-energy-5.1.0.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1080 2023-06-30 07:49:00.000000 clover-energy-5.0.8/LICENSE
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)       47 2023-06-30 07:49:00.000000 clover-energy-5.0.8/MANIFEST.in
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    16573 2023-07-14 14:29:36.000000 clover-energy-5.0.8/PKG-INFO
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    15933 2023-06-30 07:49:00.000000 clover-energy-5.0.8/README.md
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      103 2023-06-30 07:49:00.000000 clover-energy-5.0.8/pyproject.toml
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1296 2023-07-14 14:29:36.000000 clover-energy-5.0.8/setup.cfg
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     2049 2023-07-13 13:38:08.000000 clover-energy-5.0.8/src/clover/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    45472 2023-07-14 14:26:32.000000 clover-energy-5.0.8/src/clover/__main__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    93443 2023-07-14 14:26:32.000000 clover-energy-5.0.8/src/clover/__utils__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    36337 2023-07-14 14:26:32.000000 clover-energy-5.0.8/src/clover/analysis.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     8337 2023-07-14 14:26:32.000000 clover-energy-5.0.8/src/clover/argparser.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/conversion/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      710 2023-07-13 13:38:08.000000 clover-energy-5.0.8/src/clover/conversion/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    26993 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/conversion/conversion.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/conversion/tests/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/conversion/tests/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/conversion/tests/unit/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/conversion/tests/unit/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)   103637 2023-07-14 14:26:32.000000 clover-energy-5.0.8/src/clover/fileparser.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/generation/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/generation/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    19640 2023-07-14 14:26:32.000000 clover-energy-5.0.8/src/clover/generation/__utils__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    19468 2023-07-14 14:26:32.000000 clover-energy-5.0.8/src/clover/generation/solar.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/generation/tests/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/generation/tests/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/generation/tests/component/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/generation/tests/component/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/generation/tests/unit/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/generation/tests/unit/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     4505 2023-07-14 14:26:32.000000 clover-energy-5.0.8/src/clover/generation/weather.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     3514 2023-07-14 14:26:32.000000 clover-energy-5.0.8/src/clover/generation/wind.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/impact/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1141 2023-07-13 13:38:08.000000 clover-energy-5.0.8/src/clover/impact/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     4199 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/impact/__utils__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    44081 2023-07-14 14:26:32.000000 clover-energy-5.0.8/src/clover/impact/finance.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    30818 2023-07-14 14:26:32.000000 clover-energy-5.0.8/src/clover/impact/ghgs.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/impact/tests/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/impact/tests/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/impact/tests/component/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/impact/tests/component/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/impact/tests/unit/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/impact/tests/unit/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/load/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      931 2023-07-13 13:38:08.000000 clover-energy-5.0.8/src/clover/load/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    39767 2023-07-11 16:32:53.000000 clover-energy-5.0.8/src/clover/load/load.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/load/tests/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/load/tests/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/load/tests/component/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/load/tests/component/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/mains_supply/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      774 2023-07-13 13:38:08.000000 clover-energy-5.0.8/src/clover/mains_supply/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     4473 2023-07-11 16:32:53.000000 clover-energy-5.0.8/src/clover/mains_supply/__utils__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     4578 2023-07-11 16:32:53.000000 clover-energy-5.0.8/src/clover/mains_supply/grid.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/mains_supply/tests/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/mains_supply/tests/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/mains_supply/tests/component/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/mains_supply/tests/component/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/mains_supply/tests/unit/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/mains_supply/tests/unit/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    11741 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/mains_supply/water_source.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/optimisation/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1069 2023-07-13 13:38:08.000000 clover-energy-5.0.8/src/clover/optimisation/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    43289 2023-07-14 14:26:32.000000 clover-energy-5.0.8/src/clover/optimisation/__utils__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    29242 2023-07-14 14:26:32.000000 clover-energy-5.0.8/src/clover/optimisation/appraisal.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    64522 2023-07-14 14:26:32.000000 clover-energy-5.0.8/src/clover/optimisation/optimisation.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    43497 2023-07-14 14:26:32.000000 clover-energy-5.0.8/src/clover/optimisation/single_line_simulation.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/optimisation/tests/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/optimisation/tests/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/optimisation/tests/component/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/optimisation/tests/component/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/optimisation/tests/unit/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/optimisation/tests/unit/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     8395 2023-07-14 14:26:32.000000 clover-energy-5.0.8/src/clover/printer.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/scripts/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/scripts/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1309 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/scripts/clover.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1202 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/scripts/clover_hpc_clover.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1298 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/scripts/clover_hpc_outbox_assembly.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1138 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/scripts/clover_new_location.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1360 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/scripts/clover_update_api_token.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     6682 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/scripts/hpc.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    10191 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/scripts/hpc_clover.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     4894 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/scripts/hpc_outbox_assembly.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    22944 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/scripts/hpc_utils.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    11904 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/scripts/new_location.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/scripts/tests/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/scripts/tests/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/scripts/tests/unit/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/scripts/tests/unit/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     3638 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/scripts/update_api_token.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/simulation/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1199 2023-07-13 13:38:08.000000 clover-energy-5.0.8/src/clover/simulation/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    20348 2023-07-14 14:26:32.000000 clover-energy-5.0.8/src/clover/simulation/__utils__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    12992 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/simulation/diesel.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    88163 2023-07-14 14:26:32.000000 clover-energy-5.0.8/src/clover/simulation/energy_system.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     2450 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/simulation/exchanger.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    24234 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/simulation/solar.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    30736 2023-07-14 14:26:32.000000 clover-energy-5.0.8/src/clover/simulation/storage.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    19002 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/simulation/storage_utils.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/simulation/tests/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/simulation/tests/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/simulation/tests/unit/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/simulation/tests/unit/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     5411 2023-07-11 16:48:20.000000 clover-energy-5.0.8/src/clover/simulation/transmission.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/src/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/src/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    56900 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/src/new_location.yaml
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/tests/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/tests/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/tests/integration/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/tests/integration/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/tests/unit/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:49:00.000000 clover-energy-5.0.8/src/clover/tests/unit/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover_energy.egg-info/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    16573 2023-07-14 14:29:35.000000 clover-energy-5.0.8/src/clover_energy.egg-info/PKG-INFO
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     3003 2023-07-14 14:29:35.000000 clover-energy-5.0.8/src/clover_energy.egg-info/SOURCES.txt
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)        1 2023-07-14 14:29:35.000000 clover-energy-5.0.8/src/clover_energy.egg-info/dependency_links.txt
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      299 2023-07-14 14:29:35.000000 clover-energy-5.0.8/src/clover_energy.egg-info/entry_points.txt
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      119 2023-07-14 14:29:35.000000 clover-energy-5.0.8/src/clover_energy.egg-info/requires.txt
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)        7 2023-07-14 14:29:35.000000 clover-energy-5.0.8/src/clover_energy.egg-info/top_level.txt
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-17 11:13:50.000000 clover-energy-5.1.0/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1080 2023-06-30 07:49:00.000000 clover-energy-5.1.0/LICENSE
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)       47 2023-06-30 07:49:00.000000 clover-energy-5.1.0/MANIFEST.in
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    16573 2023-07-17 11:13:50.000000 clover-energy-5.1.0/PKG-INFO
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    15933 2023-07-17 10:28:59.000000 clover-energy-5.1.0/README.md
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      103 2023-06-30 07:49:00.000000 clover-energy-5.1.0/pyproject.toml
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1296 2023-07-17 11:13:50.000000 clover-energy-5.1.0/setup.cfg
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-17 11:13:50.000000 clover-energy-5.1.0/src/
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-17 11:13:50.000000 clover-energy-5.1.0/src/clover/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     2049 2023-07-17 10:09:36.000000 clover-energy-5.1.0/src/clover/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    50963 2023-07-17 10:40:04.000000 clover-energy-5.1.0/src/clover/__main__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    97316 2023-07-17 10:36:50.000000 clover-energy-5.1.0/src/clover/__utils__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    36718 2023-07-17 10:36:50.000000 clover-energy-5.1.0/src/clover/analysis.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     8512 2023-07-17 10:36:50.000000 clover-energy-5.1.0/src/clover/argparser.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-17 11:13:50.000000 clover-energy-5.1.0/src/clover/conversion/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      710 2023-07-17 10:09:36.000000 clover-energy-5.1.0/src/clover/conversion/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    26993 2023-07-17 10:28:59.000000 clover-energy-5.1.0/src/clover/conversion/conversion.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-17 11:13:50.000000 clover-energy-5.1.0/src/clover/conversion/tests/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.0/src/clover/conversion/tests/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-17 11:13:50.000000 clover-energy-5.1.0/src/clover/conversion/tests/unit/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.0/src/clover/conversion/tests/unit/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)   107239 2023-07-17 10:36:50.000000 clover-energy-5.1.0/src/clover/fileparser.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-17 11:13:50.000000 clover-energy-5.1.0/src/clover/generation/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.0/src/clover/generation/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    20730 2023-07-17 10:36:50.000000 clover-energy-5.1.0/src/clover/generation/__utils__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    27727 2023-07-17 10:36:50.000000 clover-energy-5.1.0/src/clover/generation/solar.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-17 11:13:50.000000 clover-energy-5.1.0/src/clover/generation/tests/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.0/src/clover/generation/tests/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-17 11:13:50.000000 clover-energy-5.1.0/src/clover/generation/tests/component/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.0/src/clover/generation/tests/component/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-17 11:13:50.000000 clover-energy-5.1.0/src/clover/generation/tests/unit/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.0/src/clover/generation/tests/unit/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     4554 2023-07-17 10:36:50.000000 clover-energy-5.1.0/src/clover/generation/weather.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     3563 2023-07-17 10:36:50.000000 clover-energy-5.1.0/src/clover/generation/wind.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-17 11:13:50.000000 clover-energy-5.1.0/src/clover/impact/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1141 2023-07-17 10:09:36.000000 clover-energy-5.1.0/src/clover/impact/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     4199 2023-07-17 10:28:59.000000 clover-energy-5.1.0/src/clover/impact/__utils__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    44572 2023-07-17 10:36:50.000000 clover-energy-5.1.0/src/clover/impact/finance.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    31219 2023-07-17 10:36:50.000000 clover-energy-5.1.0/src/clover/impact/ghgs.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-17 11:13:50.000000 clover-energy-5.1.0/src/clover/impact/tests/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.0/src/clover/impact/tests/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-17 11:13:50.000000 clover-energy-5.1.0/src/clover/impact/tests/component/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.0/src/clover/impact/tests/component/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-17 11:13:50.000000 clover-energy-5.1.0/src/clover/impact/tests/unit/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.0/src/clover/impact/tests/unit/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-17 11:13:50.000000 clover-energy-5.1.0/src/clover/load/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      931 2023-07-17 10:09:36.000000 clover-energy-5.1.0/src/clover/load/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    39767 2023-07-17 10:28:59.000000 clover-energy-5.1.0/src/clover/load/load.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-17 11:13:50.000000 clover-energy-5.1.0/src/clover/load/tests/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.0/src/clover/load/tests/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-17 11:13:50.000000 clover-energy-5.1.0/src/clover/load/tests/component/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.0/src/clover/load/tests/component/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-17 11:13:50.000000 clover-energy-5.1.0/src/clover/mains_supply/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      774 2023-07-17 10:09:36.000000 clover-energy-5.1.0/src/clover/mains_supply/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     4473 2023-07-11 16:32:53.000000 clover-energy-5.1.0/src/clover/mains_supply/__utils__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     4578 2023-07-11 16:32:53.000000 clover-energy-5.1.0/src/clover/mains_supply/grid.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-17 11:13:50.000000 clover-energy-5.1.0/src/clover/mains_supply/tests/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.0/src/clover/mains_supply/tests/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-17 11:13:50.000000 clover-energy-5.1.0/src/clover/mains_supply/tests/component/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.0/src/clover/mains_supply/tests/component/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-17 11:13:50.000000 clover-energy-5.1.0/src/clover/mains_supply/tests/unit/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.0/src/clover/mains_supply/tests/unit/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    11741 2023-06-30 07:48:00.000000 clover-energy-5.1.0/src/clover/mains_supply/water_source.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-17 11:13:50.000000 clover-energy-5.1.0/src/clover/optimisation/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1069 2023-07-17 10:09:36.000000 clover-energy-5.1.0/src/clover/optimisation/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    43348 2023-07-17 10:36:50.000000 clover-energy-5.1.0/src/clover/optimisation/__utils__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    29385 2023-07-17 10:36:50.000000 clover-energy-5.1.0/src/clover/optimisation/appraisal.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    64706 2023-07-17 10:36:50.000000 clover-energy-5.1.0/src/clover/optimisation/optimisation.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    43556 2023-07-17 10:36:50.000000 clover-energy-5.1.0/src/clover/optimisation/single_line_simulation.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-17 11:13:50.000000 clover-energy-5.1.0/src/clover/optimisation/tests/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.0/src/clover/optimisation/tests/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-17 11:13:50.000000 clover-energy-5.1.0/src/clover/optimisation/tests/component/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.0/src/clover/optimisation/tests/component/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-17 11:13:50.000000 clover-energy-5.1.0/src/clover/optimisation/tests/unit/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.0/src/clover/optimisation/tests/unit/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     8754 2023-07-17 10:36:50.000000 clover-energy-5.1.0/src/clover/printer.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-17 11:13:50.000000 clover-energy-5.1.0/src/clover/scripts/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.0/src/clover/scripts/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1309 2023-06-30 07:48:00.000000 clover-energy-5.1.0/src/clover/scripts/clover.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1202 2023-06-30 07:48:00.000000 clover-energy-5.1.0/src/clover/scripts/clover_hpc_clover.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1298 2023-06-30 07:48:00.000000 clover-energy-5.1.0/src/clover/scripts/clover_hpc_outbox_assembly.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1138 2023-06-30 07:48:00.000000 clover-energy-5.1.0/src/clover/scripts/clover_new_location.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1360 2023-06-30 07:48:00.000000 clover-energy-5.1.0/src/clover/scripts/clover_update_api_token.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     6682 2023-07-17 10:09:36.000000 clover-energy-5.1.0/src/clover/scripts/hpc.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    10191 2023-06-30 07:48:00.000000 clover-energy-5.1.0/src/clover/scripts/hpc_clover.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     4894 2023-06-30 07:48:00.000000 clover-energy-5.1.0/src/clover/scripts/hpc_outbox_assembly.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    22944 2023-07-17 10:09:36.000000 clover-energy-5.1.0/src/clover/scripts/hpc_utils.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    11904 2023-06-30 07:48:00.000000 clover-energy-5.1.0/src/clover/scripts/new_location.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-17 11:13:50.000000 clover-energy-5.1.0/src/clover/scripts/tests/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.0/src/clover/scripts/tests/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-17 11:13:50.000000 clover-energy-5.1.0/src/clover/scripts/tests/unit/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.0/src/clover/scripts/tests/unit/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     3638 2023-06-30 07:48:00.000000 clover-energy-5.1.0/src/clover/scripts/update_api_token.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-17 11:13:50.000000 clover-energy-5.1.0/src/clover/simulation/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1199 2023-07-17 10:09:36.000000 clover-energy-5.1.0/src/clover/simulation/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    21928 2023-07-17 10:36:50.000000 clover-energy-5.1.0/src/clover/simulation/__utils__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    12992 2023-07-17 10:28:59.000000 clover-energy-5.1.0/src/clover/simulation/diesel.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    88978 2023-07-17 10:36:50.000000 clover-energy-5.1.0/src/clover/simulation/energy_system.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     2450 2023-06-30 07:48:00.000000 clover-energy-5.1.0/src/clover/simulation/exchanger.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    24234 2023-07-17 10:28:59.000000 clover-energy-5.1.0/src/clover/simulation/solar.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    31852 2023-07-17 10:36:50.000000 clover-energy-5.1.0/src/clover/simulation/storage.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    19002 2023-06-30 07:48:00.000000 clover-energy-5.1.0/src/clover/simulation/storage_utils.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-17 11:13:50.000000 clover-energy-5.1.0/src/clover/simulation/tests/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.0/src/clover/simulation/tests/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-17 11:13:50.000000 clover-energy-5.1.0/src/clover/simulation/tests/unit/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.0/src/clover/simulation/tests/unit/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     5411 2023-07-11 16:48:20.000000 clover-energy-5.1.0/src/clover/simulation/transmission.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-17 11:13:50.000000 clover-energy-5.1.0/src/clover/src/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.0/src/clover/src/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    56900 2023-07-17 10:28:59.000000 clover-energy-5.1.0/src/clover/src/new_location.yaml
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-17 11:13:50.000000 clover-energy-5.1.0/src/clover/tests/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.0/src/clover/tests/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-17 11:13:50.000000 clover-energy-5.1.0/src/clover/tests/integration/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.0/src/clover/tests/integration/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-17 11:13:50.000000 clover-energy-5.1.0/src/clover/tests/unit/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:49:00.000000 clover-energy-5.1.0/src/clover/tests/unit/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-17 11:13:50.000000 clover-energy-5.1.0/src/clover_energy.egg-info/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    16573 2023-07-17 11:13:50.000000 clover-energy-5.1.0/src/clover_energy.egg-info/PKG-INFO
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     3003 2023-07-17 11:13:50.000000 clover-energy-5.1.0/src/clover_energy.egg-info/SOURCES.txt
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)        1 2023-07-17 11:13:50.000000 clover-energy-5.1.0/src/clover_energy.egg-info/dependency_links.txt
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      299 2023-07-17 11:13:50.000000 clover-energy-5.1.0/src/clover_energy.egg-info/entry_points.txt
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      119 2023-07-17 11:13:50.000000 clover-energy-5.1.0/src/clover_energy.egg-info/requires.txt
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)        7 2023-07-17 11:13:50.000000 clover-energy-5.1.0/src/clover_energy.egg-info/top_level.txt
```

### Comparing `clover-energy-5.0.8/LICENSE` & `clover-energy-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.8/PKG-INFO` & `clover-energy-5.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clover-energy
-Version: 5.0.8
+Version: 5.1.0
 Summary: Continuous Lifetime Optimisation of Variable Electricity Resources
 Home-page: https://github.com/CLOVER-energy/CLOVER
 Author: Phil Sandwell, Ben Winchester and Hamish Beath
 Author-email: philip.sandwell@gmail.com,benedict.winchester@gmail.com,hamishbeath@outlook.com
 Project-URL: Bug Tracker, https://github.com/CLOVER-energy/CLOVER/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `clover-energy-5.0.8/README.md` & `clover-energy-5.1.0/README.md`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.8/setup.cfg` & `clover-energy-5.1.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = clover-energy
-version = 5.0.8
+version = 5.1.0
 author = Phil Sandwell, Ben Winchester and Hamish Beath
 author_email = philip.sandwell@gmail.com,benedict.winchester@gmail.com,hamishbeath@outlook.com
 description = Continuous Lifetime Optimisation of Variable Electricity Resources
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/CLOVER-energy/CLOVER
 project_urls =
```

### Comparing `clover-energy-5.0.8/src/clover/__init__.py` & `clover-energy-5.1.0/src/clover/__init__.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.8/src/clover/__main__.py` & `clover-energy-5.1.0/src/clover/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,24 +13,25 @@
 CLOVER (Continuous Lifetime Optimisation of Variable Electricity Resources) can evaluate
 and optimise minigrid systems, determining whether a demand is met whilst minimising
 environmental and economic impacts. The main flow of CLOVER can be executed by running
 the clover module from the command-line interface.
 
 """
 
-__version__ = "5.0.8"
+__version__ = "5.1.0"
 
+import collections
 import datetime
 import logging
 import math
 import os
 import sys
 
 from argparse import Namespace
-from typing import Any, Dict, List, Optional, Set, Tuple
+from typing import Any, DefaultDict, Dict, List, Optional, Set, Tuple
 
 import pandas as pd  # pylint: disable=import-error
 
 from tqdm import tqdm
 
 from . import analysis, argparser
 from .conversion.conversion import WaterSource
@@ -60,14 +61,15 @@
     ResourceType,
     SystemAppraisal,
     get_logger,
     InputFileError,
     LOCATIONS_FOLDER_NAME,
     LOGGER_DIRECTORY,
     OperatingMode,
+    ProgrammerJudgementFault,
     save_simulation,
 )
 from .simulation.__utils__ import check_scenario
 
 __all__ = ("main",)
 
 # Auto-generated-files directory:
@@ -608,91 +610,164 @@
         raise
 
     logger.info("All input files successfully parsed.")
     print(DONE)
 
     print("Generating necessary profiles", end="\n")
 
+    # Determine the capacities of the various PV panels that are to be considered.
+    pv_system_sizes: DefaultDict[str, float] = collections.defaultdict(float)
+    if parsed_args.pv_system_size is not None:
+        try:
+            pv_system_sizes.update(
+                {minigrid.pv_panel.name: float(parsed_args.pv_system_size)}
+            )
+        except ProgrammerJudgementFault:
+            # Multiple panels are specified in the file, process as a mapping.
+            try:
+                pv_system_sizes.update(
+                    {
+                        panel_size_entry.split("=")[0]: float(
+                            panel_size_entry.split("=")[1]
+                        )
+                        for panel_size_entry in parsed_args.pv_system_size.split(",")
+                    }
+                )
+            except IndexError:
+                logger.error(
+                    "If using multiple panels, ensure that their capacities are entered "
+                    "using a '<panel_name>=<capacity>,<panel_name>=<capacity>,...' format."
+                )
+                raise ValueError(
+                    "The command-line arguments were invalid. See "
+                    f"{os.path.join(LOGGER_DIRECTORY, LOGGER_NAME)}.log for details."
+                ) from None
+        except TypeError:
+            logger.error(
+                "Mismatch between command-line usage of `pv` argument. If considering only "
+                "one panel, '%s', the capacity of the panel in pv units must be specified "
+                "using `--pv-system-size <capacity>` or `-pv <capacity>`.",
+                minigrid.pv_panel,
+            )
+            raise ValueError(
+                "The command-line arguments were invalid. See "
+                f"{os.path.join(LOGGER_DIRECTORY, LOGGER_NAME)}.log for details."
+            ) from None
+
+        # Ensure that the capacities match the panels entered in the energy-system inputs.
+        if pv_system_sizes.keys() != {panel.name for panel in minigrid.pv_panels}:
+            logger.error(
+                "The panels provided in the minigrid inputs file do not match those "
+                "entered on the command-line interface. If specifying multiple panel "
+                "capacities to consider, the sizes of each of these panels must be "
+                "inputted on the command-line. Ensure that the panels that are in the "
+                "`energy_system_inputs.yaml` file match those provided on the command-line "
+                "interface."
+            )
+            raise InputFileError(
+                "energy system inputs",
+                "The panels provided in the minigrid inputs file do not match those "
+                "entered on the command-line interface.",
+            )
+
     # Determine the number of background tasks to carry out.
+    panels_to_fetch: Set[solar.PVPanel] = set(
+        minigrid.pv_panels + minigrid.pvt_panels  # type: ignore [operator]
+    )
     num_ninjas: int = (
-        1
+        len(panels_to_fetch)
         + (1 if any(scenario.pv_t for scenario in scenarios) else 0)
         + (
             1
             if any(scenario.desalination_scenario for scenario in scenarios) is not None
             else 0
         )
     )
 
+    # Ninja pause index:
+    #   Variable used to ensure that no short-burst errors occur when launching multiple
+    # renewables.ninja threads in quick succession.
+    ninja_pause_index: int = 0
+
     # Generate and save the wind data for each year as a background task.
     if any(scenario.pv_t for scenario in scenarios):
         logger.info("Beginning wind-data fetching.")
         wind_data_thread: Optional[wind.WindDataThread] = wind.WindDataThread(
             os.path.join(auto_generated_files_directory, "wind"),
             generation_inputs,
             location,
             f"{parsed_args.location}_{wind.WIND_LOGGER_NAME}",
+            ninja_pause_index,
             parsed_args.refetch,
             num_ninjas,
             parsed_args.verbose,
         )
         if wind_data_thread is None:
             raise InternalError("Wind data thread failed to successfully instantiate.")
         wind_data_thread.start()
         logger.info(
             "Wind-data thread successfully instantiated. See %s for details.",
             f"{os.path.join(LOGGER_DIRECTORY, wind.WIND_LOGGER_NAME)}.log",
         )
+        ninja_pause_index += 1
     else:
         wind_data_thread = None
 
     # Generate and save the weather data for each year as a background task.
     if any(scenario.desalination_scenario is not None for scenario in scenarios):
         # Set up the system to call renewables.ninja at a slower rate.
         logger.info("Begining weather-data fetching.")
         weather_data_thread: Optional[
             weather.WeatherDataThread
         ] = weather.WeatherDataThread(
             os.path.join(auto_generated_files_directory, "weather"),
             generation_inputs,
             location,
             f"{parsed_args.location}_{weather.WEATHER_LOGGER_NAME}",
+            ninja_pause_index,
             parsed_args.refetch,
             num_ninjas,
             parsed_args.verbose,
         )
         if weather_data_thread is None:
             raise InternalError(
                 "Weather data thread failed to successfully instantiate."
             )
         weather_data_thread.start()
         logger.info(
             "Weather-data thread successfully instantiated. See %s for details.",
             f"{os.path.join(LOGGER_DIRECTORY, weather.WEATHER_LOGGER_NAME)}.log",
         )
+        ninja_pause_index += 1
     else:
         weather_data_thread = None
 
     # Generate and save the solar data for each year as a background task.
     logger.info("Beginning solar-data fetching.")
-    solar_data_thread = solar.SolarDataThread(
-        os.path.join(auto_generated_files_directory, "solar"),
-        generation_inputs,
-        location,
-        f"{parsed_args.location}_{solar.SOLAR_LOGGER_NAME}{run_number_string}",
-        parsed_args.refetch,
-        minigrid.pv_panel,
-        num_ninjas,
-        parsed_args.verbose,
-    )
-    solar_data_thread.start()
-    logger.info(
-        "Solar-data thread successfully instantiated. See %s for details.",
-        f"{os.path.join(LOGGER_DIRECTORY, solar.SOLAR_LOGGER_NAME)}.log",
-    )
+    solar_data_threads: Dict[solar.PVPanel, solar.SolarDataThread] = {}
+    for pv_panel in panels_to_fetch:
+        solar_data_threads[pv_panel] = solar.SolarDataThread(
+            os.path.join(auto_generated_files_directory, "solar"),
+            generation_inputs,
+            location,
+            f"{parsed_args.location}_{solar.SOLAR_LOGGER_NAME}_"
+            f"{solar.get_profile_prefix(pv_panel)}_{run_number_string}",
+            ninja_pause_index,
+            parsed_args.refetch,
+            pv_panel,
+            num_ninjas,
+            parsed_args.verbose,
+        )
+        solar_data_threads[pv_panel].start()
+        ninja_pause_index += 1
+    if len(panels_to_fetch) >= 1:
+        logger.info(
+            "Solar-data threads successfully instantiated. See %s for details.",
+            f"{os.path.join(LOGGER_DIRECTORY, solar.SOLAR_LOGGER_NAME)}.log",
+        )
 
     # Generate and save the device-ownership profiles.
     logger.info("Processing device informaiton.")
     # load_logger = get_logger(load.LOAD_LOGGER_NAME)
 
     initial_electric_hourly_loads: Optional[Dict[str, pd.DataFrame]] = None
     total_electric_load: Optional[pd.DataFrame] = None
@@ -844,28 +919,33 @@
         logger.info("Grid-availability profiles successfully generated.")
 
     else:
         logger.info("Grid disabled, no grid profiles to be generated.")
 
     # Wait for all threads to finish before proceeding.
     logger.info("Waiting for all setup threads to finish before proceeding.")
-    solar_data_thread.join()
+    for thread in solar_data_threads.values():
+        thread.join()
     if weather_data_thread is not None:
         weather_data_thread.join()
     if wind_data_thread is not None:
         wind_data_thread.join()
     logger.info("All setup threads finished.")
 
     logger.info("Generating and saving total solar output file.")
-    total_solar_data = solar.total_solar_output(
-        os.path.join(auto_generated_files_directory, "solar"),
-        parsed_args.regenerate,
-        generation_inputs["start_year"],
-        location.max_years,
-    )
+    total_solar_data: Dict[str, pd.DataFrame] = {
+        pv_panel.name: solar.total_solar_output(
+            os.path.join(auto_generated_files_directory, "solar"),
+            parsed_args.regenerate,
+            generation_inputs["start_year"],
+            location.max_years,
+            pv_panel=pv_panel,
+        )
+        for pv_panel in (minigrid.pv_panels + minigrid.pvt_panels)  # type: ignore
+    }
     logger.info("Total solar output successfully computed and saved.")
 
     if any(scenario.desalination_scenario is not None for scenario in scenarios) or any(
         scenario.hot_water_scenario is not None for scenario in scenarios
     ):
         logger.info("Generating and saving total weather output file.")
         total_weather_data = (  # pylint: disable=unused-variable
@@ -919,18 +999,18 @@
         )
         raise
 
     # Remove the index from the file.
     kerosene_usage.reset_index(drop=True)
 
     # Determine whether any default sizes have been overrided.
-    overrided_default_sizes: bool = (
-        minigrid.pv_panel.pv_unit_overrided
-        if minigrid.pv_panel is not None
-        else False or minigrid.battery.storage_unit
+    overrided_default_sizes: bool = any(
+        pv_panel.pv_unit_overrided for pv_panel in minigrid.pv_panels
+    ) or (
+        minigrid.battery.storage_unit_overrided
         if minigrid.battery is not None
         else False
     )
 
     # Run a simulation or optimisation as appropriate.
     if operating_mode == OperatingMode.SIMULATION:
         print(
@@ -965,15 +1045,15 @@
         logger.info("Loading grid profile.")
         grid_profile = grid.load_grid_profile(
             auto_generated_files_directory, logger, scenario
         )
         logger.info("Grid '%s' profile successfully loaded.", scenario.grid_type)
 
         simulation_string: str = generate_simulation_string(
-            minigrid, overrided_default_sizes, parsed_args, scenario
+            minigrid, overrided_default_sizes, parsed_args, pv_system_sizes, scenario
         )
         print(f"Running a simulation with:\n{simulation_string}")
 
         for simulation_number, simulation in enumerate(
             tqdm(
                 simulations, desc="simulations", disable=disable_tqdm, unit="simulation"
             ),
@@ -995,29 +1075,40 @@
                     converters,
                     disable_tqdm,
                     parsed_args.storage_size,
                     grid_profile,
                     parsed_args.hot_water_pvt_system_size
                     if parsed_args.hot_water_pvt_system_size is not None
                     else 0,
-                    total_solar_data[solar.SolarDataType.TOTAL_IRRADIANCE.value],
+                    {
+                        key: value[solar.SolarDataType.TOTAL_IRRADIANCE.value]
+                        for key, value in total_solar_data.items()
+                    },
                     kerosene_usage,
                     location,
                     logger,
                     minigrid,
                     parsed_args.num_clean_water_tanks,
                     parsed_args.num_hot_water_tanks,
-                    total_solar_data[solar.SolarDataType.ELECTRICITY.value]
-                    * minigrid.pv_panel.pv_unit,
-                    parsed_args.pv_system_size
-                    if parsed_args.pv_system_size is not None
-                    else 0,
+                    {
+                        panel.name: total_solar_data[panel.name][
+                            solar.SolarDataType.ELECTRICITY.value
+                        ]
+                        * panel.pv_unit
+                        for panel in (minigrid.pv_panels + minigrid.pvt_panels)  # type: ignore
+                    },
+                    pv_system_sizes
+                    if pv_system_sizes is not None
+                    else collections.defaultdict(float),
                     scenario,
                     simulation,
-                    total_solar_data[solar.SolarDataType.TEMPERATURE.value],
+                    {
+                        key: value[solar.SolarDataType.TEMPERATURE.value]
+                        for key, value in total_solar_data.items()
+                    },
                     total_loads,
                     total_wind_data[wind.WindDataType.WIND_SPEED.value]
                     if total_wind_data is not None
                     else None,
                 )
             except Exception as e:
                 print(f"Beginning CLOVER simulation runs {'.' * 30}    {FAILED}")
@@ -1044,17 +1135,22 @@
             system_details.file_information = input_file_info
 
             # Compute the key results.
             key_results = analysis.get_key_results(  # type: ignore
                 grid_profile,
                 simulation.end_year - simulation.start_year,
                 system_performance_outputs,
-                total_solar_data[solar.SolarDataType.ELECTRICITY.value]
-                * minigrid.pv_panel.pv_unit
-                * scenario.pv,
+                {
+                    pv_panel.name: total_solar_data[pv_panel.name][
+                        solar.SolarDataType.ELECTRICITY.value
+                    ]
+                    * pv_panel.pv_unit
+                    * scenario.pv
+                    for pv_panel in (minigrid.pv_panels + minigrid.pvt_panels)  # type: ignore
+                },
             )
 
             if parsed_args.analyse:
                 if not parsed_args.skip_plots:
                     # Generate and save the various plots.
                     analysis.plot_outputs(  # type: ignore
                         grid_times[scenario.grid_type],
@@ -1117,15 +1213,14 @@
 
     if operating_mode == OperatingMode.OPTIMISATION:
         print(f"Beginning CLOVER optimisation runs {'.' * 28}    ", end="\n")
         optimisation_times: List[str] = []
 
         # Enforce that the optimisation inputs are set correctly before attempting an
         # optimisation.
-
         if optimisation_inputs is None:
             raise InputFileError(
                 "optimisation inputs",
                 "Optimisation inputs were not specified despite an optimisation being "
                 "called.",
             )
         if electric_yearly_load_statistics is None:
@@ -1141,14 +1236,25 @@
         ):
             raise InputFileError(
                 "optimisation inputs",
                 "An optimisation was requested that runs over the maximum lifetime of "
                 "the system.",
             )
 
+        if len(minigrid.pv_panels) > 1:
+            raise InputFileError(
+                "energy-system inputs",
+                "Optimisations can only be run with a single PV panel.",
+            )
+        if len(minigrid.pvt_panels) > 1:
+            raise InputFileError(
+                "energy-system inputs",
+                "Optimisations can only be run with a single PV-T panel.",
+            )
+
         for optimisation_number, optimisation in enumerate(
             tqdm(
                 optimisations,
                 desc="optimisations",
                 disable=disable_tqdm,
                 unit="optimisation",
             ),
@@ -1179,25 +1285,38 @@
                 time_delta, optimisation_results = multiple_optimisation_step(
                     conventional_cw_source_profiles,
                     converters,
                     disable_tqdm,
                     finance_inputs,
                     ghg_inputs,
                     grid_profile,
-                    total_solar_data[solar.SolarDataType.TOTAL_IRRADIANCE.value],
+                    {
+                        panel_name: solar_data[
+                            solar.SolarDataType.TOTAL_IRRADIANCE.value
+                        ]
+                        for panel_name, solar_data in total_solar_data.items()
+                    },
                     kerosene_usage,
                     location,
                     logger,
                     minigrid,
                     optimisation,
                     optimisation_inputs,
-                    total_solar_data[solar.SolarDataType.TEMPERATURE.value],
+                    {
+                        panel_name: solar_data[solar.SolarDataType.TEMPERATURE.value]
+                        for panel_name, solar_data in total_solar_data.items()
+                    },
                     total_loads,
-                    total_solar_data[solar.SolarDataType.ELECTRICITY.value]
-                    * minigrid.pv_panel.pv_unit,
+                    {
+                        pv_panel.name: total_solar_data[pv_panel.name][
+                            solar.SolarDataType.ELECTRICITY.value
+                        ]
+                        * minigrid.pv_panel.pv_unit
+                        for pv_panel in (minigrid.pv_panels + minigrid.pvt_panels)  # type: ignore
+                    },
                     total_wind_data[wind.WindDataType.WIND_SPEED.value]
                     if total_wind_data is not None
                     else None,
                     electric_yearly_load_statistics,
                 )
             except Exception as e:
                 print(f"Beginning CLOVER optimisation runs {'.' * 28}    {FAILED}")
```

### Comparing `clover-energy-5.0.8/src/clover/__utils__.py` & `clover-energy-5.1.0/src/clover/__utils__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,20 +14,21 @@
 
 The utility module contains functionality which is used by various scripts, modules, and
 components across CLOVER, as well as commonly-held variables to prevent dependency
 issues and increase the ease of code alterations.
 
 """
 
+import collections
 import dataclasses
 import enum
 import logging
 import os
 
-from typing import Any, Dict, List, Optional, Set, Union
+from typing import Any, DefaultDict, Dict, List, Optional, Set, Union
 
 import json
 import numpy as np  # pylint: disable=import-error
 import pandas as pd  # pylint: disable=import-error
 import scipy  # pylint: disable=import-error
 import yaml  # pylint: disable=import-error
 
@@ -882,15 +883,16 @@
 
 @dataclasses.dataclass
 class KeyResults:
     """
     Contains the key results from a simulation.
 
     .. attribute:: average_pv_generation
-        The average energy generated by the PV set up per day, measured in kWh/day.
+        The average energy generated by the PV set up per day, measured in kWh/day, for
+        each of the PV panel types installed.
 
     .. attribute:: blackouts
         The fraction of time for which blackouts occurred.
 
     .. attribute:: clean_water_blackouts
         The fraction of time for which the clean-water system experienced a blackout.
 
@@ -917,47 +919,47 @@
     average_daily_hw_pvt_generation: Optional[float] = None
     average_daily_hw_supplied: Optional[float] = None
     average_daily_pv_energy_supplied: Optional[float] = None
     average_daily_renewables_energy_supplied: Optional[float] = None
     average_daily_renewables_energy_used: Optional[float] = None
     average_daily_stored_energy_supplied: Optional[float] = None
     average_daily_unmet_energy: Optional[float] = None
-    average_pv_generation: Optional[float] = None
+    average_pv_generation: Optional[Dict[str, float]] = None
     average_pvt_electric_generation: Optional[float] = None
     blackouts: Optional[float] = None
     clean_water_blackouts: Optional[float] = None
     cumulative_cw_load: Optional[float] = None
     cumulative_cw_pvt_generation: Optional[float] = None
     cumulative_cw_supplied: Optional[float] = None
     cumulative_hw_load: Optional[float] = None
     cumulative_hw_pvt_generation: Optional[float] = None
     cumulative_hw_supplied: Optional[float] = None
-    cumulative_pv_generation: Optional[float] = None
+    cumulative_pv_generation: Optional[Dict[str, float]] = None
     diesel_times: Optional[float] = None
     grid_daily_hours: Optional[float] = None
     max_buffer_tank_temperature: Optional[float] = None
     max_cw_pvt_output_temperature: Optional[float] = None
     mean_buffer_tank_temperature: Optional[float] = None
     mean_cw_pvt_output_temperature: Optional[float] = None
     min_buffer_tank_temperature: Optional[float] = None
     min_cw_pvt_output_temperature: Optional[float] = None
 
     def to_dict(  # pylint: disable=too-many-branches, too-many-statements
         self,
-    ) -> Dict[str, float]:
+    ) -> Dict[str, Union[float, Dict[str, float]]]:
         """
         Returns the :class:`KeyResults` information as a `dict` ready for saving.
 
         Outputs:
             - A `dict` containing the information stored in the :class:`KeyResult`
               instance.
 
         """
 
-        data_dict: Dict[str, float] = {}
+        data_dict: Dict[str, Union[float, Dict[str, float]]] = {}
 
         if self.average_daily_cw_demand_covered is not None:
             data_dict["Average daily clean-water demand covered"] = round(
                 self.average_daily_cw_demand_covered, 3
             )
         if self.average_daily_cw_supplied is not None:
             data_dict["Average daily clean water supplied / litres"] = round(
@@ -1008,17 +1010,26 @@
                 self.average_daily_stored_energy_supplied, 3
             )
         if self.average_daily_unmet_energy is not None:
             data_dict["Average daily unmet energy / kWh"] = round(
                 self.average_daily_unmet_energy, 3
             )
         if self.average_pv_generation is not None:
-            data_dict["Average pv generation / kWh/day"] = round(
-                self.average_pv_generation, 3
-            )
+            # If only one panel, simply display this, otherwise, key by the panel name.
+            if len(self.average_pv_generation) == 1:
+                data_dict["Average pv generation / kWh/day"] = round(
+                    list(self.average_pv_generation.values())[0], 3
+                )
+            else:
+                data_dict["Average pv generation / kWh/day"] = {
+                    panel_name.capitalize().replace("_", " "): round(
+                        average_generation, 3
+                    )
+                    for panel_name, average_generation in self.average_pv_generation.items()
+                }
         if self.average_pvt_electric_generation is not None:
             data_dict["Average pv-t electric generation / kWh/day"] = round(
                 self.average_pvt_electric_generation, 3
             )
         if self.blackouts is not None:
             data_dict["Blackouts"] = round(self.blackouts, 3)
         if self.clean_water_blackouts is not None:
@@ -1038,17 +1049,27 @@
                 self.cumulative_cw_supplied, 3
             )
         if self.cumulative_hw_pvt_generation is not None:
             data_dict["Cumulative hot-water PV-T generation / kWh"] = round(
                 self.cumulative_hw_pvt_generation, 3
             )
         if self.cumulative_pv_generation is not None:
-            data_dict["Cumulative pv generation / kWh/kWp"] = round(
-                self.cumulative_pv_generation, 3
-            )
+            # If only one panel, simply display this, otherwise, key by the panel name.
+            if len(self.cumulative_pv_generation) == 1:
+                data_dict["Cumulative pv generation / kWh/kWp"] = round(
+                    list(self.cumulative_pv_generation.values())[0], 3
+                )
+            else:
+                data_dict["Cumulative pv generation / kWh/kWp"] = {
+                    panel_name.capitalize().replace("_", " "): round(
+                        cumulative_generation, 3
+                    )
+                    for panel_name, cumulative_generation in self.cumulative_pv_generation.items()
+                }
+
         if self.diesel_times is not None:
             data_dict[ColumnHeader.DIESEL_GENERATOR_TIMES.value] = round(
                 self.diesel_times, 3
             )
         if self.grid_daily_hours is not None:
             data_dict["Average grid availability / hours/day"] = round(
                 self.grid_daily_hours, 3
@@ -1074,15 +1095,25 @@
                 self.min_buffer_tank_temperature, 3
             )
         if self.min_cw_pvt_output_temperature is not None:
             data_dict["Minimum clean-water PV-T output temperature / degC"] = round(
                 self.min_cw_pvt_output_temperature, 3
             )
 
-        data_dict = {str(key): float(value) for key, value in data_dict.items()}
+        data_dict = {
+            str(key): (
+                float(value)
+                if not isinstance(value, dict)
+                else {
+                    str(sub_key): float(sub_value)
+                    for sub_key, sub_value in value.items()
+                }
+            )
+            for key, value in data_dict.items()
+        }
 
         return data_dict
 
 
 class ProgrammerJudgementFault(Exception):
     """
     Raised when a programmer judgement faul occurs.
@@ -2226,15 +2257,15 @@
 
     .. attribute:: final_num_clean_water_tanks
         The final number of clean-water tanks installed in the system.
 
     .. attribute:: final_num_hot_water_tanks
         The final number of hot-water tanks installed in the system.
 
-    .. attribute:: final_pv_size
+    .. attribute:: final_pv_sizes
         The final pv size of the system.
 
     .. attribute:: final_storage_size
         The final storage size of the system.
 
     .. attribute:: initial_converter_sizes:
         A mapping between the name of the various converters associated with the system
@@ -2251,15 +2282,15 @@
 
     .. attribute:: initial_num_clean_water_tanks
         The initial number of clean-water tanks installed in the system.
 
     .. attribute:: initial_num_hot_water_tanks
         The initial number of hot-water tanks installed in the system.
 
-    .. attribute:: initial_pv_size
+    .. attribute:: initial_pv_sizes
         The initial pv size of the system.
 
     .. attribute:: initial_storage_size
         The initial storage size of the system.
 
     .. attribute:: required_feedwater_sources
         The `list` of feedwater sources which were required to supply the desalination
@@ -2277,55 +2308,79 @@
     end_year: int = 0
     final_converter_sizes: Optional[Dict[str, int]] = None
     final_cw_pvt_size: Optional[float] = 0
     final_hw_pvt_size: Optional[float] = 0
     final_num_buffer_tanks: Optional[int] = 0
     final_num_clean_water_tanks: Optional[int] = 0
     final_num_hot_water_tanks: Optional[int] = 0
-    final_pv_size: float = 0
+    final_pv_sizes: Union[
+        Dict[str, float], DefaultDict[str, float]
+    ] = dataclasses.field(  # type: ignore [assignment]
+        default_factory=lambda: collections.defaultdict(float)
+    )
     final_storage_size: float = 0
     initial_converter_sizes: Optional[Dict[str, int]] = None
     initial_cw_pvt_size: Optional[float] = 0
     initial_hw_pvt_size: Optional[float] = 0
     initial_num_buffer_tanks: Optional[int] = 0
     initial_num_clean_water_tanks: Optional[int] = 0
     initial_num_hot_water_tanks: Optional[int] = 0
-    initial_pv_size: float = 0
+    initial_pv_sizes: Union[
+        Dict[str, float], DefaultDict[str, float]
+    ] = dataclasses.field(  # type: ignore [assignment]
+        default_factory=lambda: collections.defaultdict(float)
+    )
     initial_storage_size: float = 0
     required_feedwater_sources: Optional[List[str]] = None
     start_year: int = 0
     file_information: Optional[Dict[str, str]] = None
 
     def to_dict(
         self,
     ) -> Dict[
-        str, Optional[Union[int, float, str, Dict[str, str]]]
+        str, Optional[Union[int, float, str, Dict[str, str], Dict[str, float]]]
     ]:  # pylint: disable=too-many-branches
         """
         Returns a `dict` containing information the :class:`SystemDetails`' information.
 
         Outputs:
             A `dict` containing the information stored within the :class:`SystemDetails`
             instance.
 
         """
 
         system_details_as_dict: Dict[
-            str, Optional[Union[int, float, str, Dict[str, str]]]
+            str, Optional[Union[int, float, str, Dict[str, str], Dict[str, float]]]
         ] = {
             "diesel_capacity": round(self.diesel_capacity, 3),
             "end_year": round(self.end_year, 3),
-            "final_pv_size": round(self.final_pv_size, 3),
             "final_storage_size": round(self.final_storage_size, 3),
-            "initial_pv_size": round(self.initial_pv_size, 3),
             "initial_storage_size": round(self.initial_storage_size, 3),
             "input_files": self.file_information,
             "start_year": round(self.start_year, 3),
         }
 
+        # Add the PV sizes
+        if len(self.final_pv_sizes) > 1:
+            system_details_as_dict["final_pv_sizes"] = {
+                key: round(value, 3) for key, value in self.final_pv_sizes.items()
+            }
+        else:
+            system_details_as_dict["final_pv_size"] = round(
+                list(self.final_pv_sizes.values())[0], 3
+            )
+        if len(self.initial_pv_sizes) > 1:
+            system_details_as_dict["initial_pv_sizes"] = {
+                key: round(value, 3) for key, value in self.initial_pv_sizes.items()
+            }
+        else:
+            system_details_as_dict["initial_pv_size"] = round(
+                list(self.initial_pv_sizes.values())[0], 3
+            )
+
         if self.initial_converter_sizes is not None:
             system_details_as_dict.update(
                 {
                     f"intial_num_{key}": value
                     for key, value in self.initial_converter_sizes.items()
                 }
             )
@@ -2380,28 +2435,74 @@
             system_details_as_dict["required_feedwater_sources"] = ", ".join(
                 self.required_feedwater_sources
             )
 
         return system_details_as_dict
 
     @property
+    def initial_pv_size(self) -> float:
+        """
+        Returns the initial PV size if only one panel is present, otherwise an error.
+
+        Outputs:
+            The size of initial PV panels installed, if only one panel is present.
+
+        Raises:
+            - :class:`ProgrammerJudementFault`
+                Raised when multiple panels are present.
+
+        """
+
+        if len(self.initial_pv_sizes) > 1:
+            raise ProgrammerJudgementFault(
+                "__utils__.SystemDetails::initial_pv_size",
+                "Cannot fetch initial PV size if multiple panels. Use "
+                "`initial_pv_sizes` to access all.",
+            )
+
+        return list(self.initial_pv_sizes.values())[0]
+
+    @property
     def initial_pvt_size(self) -> float:
         """
         Returns the total size of the PV-T system initially installed.
 
         Outputs:
             - The total size of the PV-T system initially installed.
 
         """
 
         return (
             self.initial_cw_pvt_size if self.initial_cw_pvt_size is not None else 0
         ) + (self.initial_hw_pvt_size if self.initial_hw_pvt_size is not None else 0)
 
     @property
+    def final_pv_size(self) -> float:
+        """
+        Returns the final PV size if only one panel is present, otherwise an error.
+
+        Outputs:
+            The size of final PV panels installed, if only one panel is present.
+
+        Raises:
+            - :class:`ProgrammerJudementFault`
+                Raised when multiple panels are present.
+
+        """
+
+        if len(self.final_pv_sizes) > 1:
+            raise ProgrammerJudgementFault(
+                "__utils__.SystemDetails::initial_pv_size",
+                "Cannot fetch final PV size if multiple panels. Use `initial_pv_sizes` "
+                "to access all.",
+            )
+
+        return list(self.final_pv_sizes.values())[0]
+
+    @property
     def final_pvt_size(self) -> float:
         """
         Returns the total size of the PV-T system installed at the end of the iteration.
 
         Outputs:
             - The total size of the PV-T system installed at the end of the simulation.
```

### Comparing `clover-energy-5.0.8/src/clover/analysis.py` & `clover-energy-5.1.0/src/clover/analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,44 +68,52 @@
 SIMULATION_PLOTS_DIRECTORY: str = "simulation_{simulation_number}_plots"
 
 
 def get_key_results(
     grid_input_profile: pd.DataFrame,
     num_years: int,
     simulation_results: pd.DataFrame,
-    total_solar_output: pd.DataFrame,
+    total_solar_output: Dict[str, pd.DataFrame],
 ) -> KeyResults:
     """
     Computes the key results of the simulation.
 
         Inputs:
         - grid_input_profile:
             The relevant grid input profile for the simulation that was run.
         - num_years:
             The number of years for which the simulation was run.
         - simulation_results:
             The results of the simulation.
         - total_solar_output:
-            The total solar power produced by the PV installation.
+            The total solar power produced by the PV installation for each of the solar
+            PV panels installed.
 
     Outputs:
         - key_results:
             The key results of the simulation, wrapped in a :class:`KeyResults`
             instance.
 
     """
 
     key_results = KeyResults()
 
     # Compute the solar-generation results.
-    total_solar_generation: float = np.round(np.sum(total_solar_output))
-    key_results.cumulative_pv_generation = float(total_solar_generation)
-    key_results.average_pv_generation = float(
-        round(total_solar_generation / (20 * 365))
-    )
+    total_solar_generation: Dict[str, float] = {
+        panel_name: np.round(np.sum(solar_output))
+        for panel_name, solar_output in total_solar_output.items()
+    }
+    key_results.cumulative_pv_generation: Dict[str, float] = {
+        panel_name: float(solar_generation)
+        for panel_name, solar_generation in total_solar_generation.items()
+    }
+    key_results.average_pv_generation: Dict[str, float] = {
+        panel_name: float(round(solar_generation / (20 * 365)))
+        for panel_name, solar_generation in total_solar_generation.items()
+    }
 
     # Compute the grid results.
     if grid_input_profile is not None:
         key_results.grid_daily_hours = np.sum(
             grid_input_profile[: num_years * HOURS_PER_YEAR], axis=0
         ) / (365 * num_years)
```

### Comparing `clover-energy-5.0.8/src/clover/argparser.py` & `clover-energy-5.1.0/src/clover/argparser.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,22 @@
         )
 
 
 def parse_args(args: List[Any]) -> argparse.Namespace:
     """
     Parses command-line arguments into a :class:`argparse.NameSpace`.
 
+    Inputs:
+        - args:
+            The un-parsed command-line arguments.
+
+    Outputs:
+        - parsed_args:
+            The parsed command-line arguments.
+
     """
 
     parser = argparse.ArgumentParser()
 
     # Misc. arguments.
     # Fast mode:
     #   Used for debugging purposes to run with fsat models.
@@ -109,16 +117,17 @@
         "-o",
         type=str,
         help="The location of the output file in which simulation data will be saved.",
     )
     action_arguments.add_argument(
         "--pv-system-size",
         "-pv",
-        type=float,
-        help="The size of the PV system being modelled in PV panel units, defaulting "
+        type=str,
+        help="The size of the PV system(s) being modelled in PV panel units, "
+        "defaulting "
         "to kWp.",
     )
     action_arguments.add_argument(
         "--scenario",
         "-s",
         type=str,
         default=DEFAULT_SCENARIO,
```

### Comparing `clover-energy-5.0.8/src/clover/conversion/__init__.py` & `clover-energy-5.1.0/src/clover/conversion/__init__.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.8/src/clover/conversion/conversion.py` & `clover-energy-5.1.0/src/clover/conversion/conversion.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.8/src/clover/fileparser.py` & `clover-energy-5.1.0/src/clover/fileparser.py`

 * *Files 5% similar despite different names*

```diff
@@ -1246,20 +1246,20 @@
 def _parse_solar_inputs(  # pylint: disable=too-many-locals, too-many-statements
     debug: bool,
     energy_system_inputs: Dict[str, Any],
     inputs_directory_relative_path: str,
     logger: Logger,
     scenarios: List[Scenario],
 ) -> Tuple[
-    solar.PVPanel,
-    Dict[str, float],
-    Dict[str, float],
-    Optional[solar.HybridPVTPanel],
-    Optional[Dict[str, float]],
-    Optional[Dict[str, float]],
+    List[solar.PVPanel],
+    Dict[str, DefaultDict[str, float]],
+    Dict[str, DefaultDict[str, float]],
+    List[solar.HybridPVTPanel],
+    Optional[Dict[str, DefaultDict[str, float]]],
+    Optional[Dict[str, DefaultDict[str, float]]],
     str,
 ]:
     """
     Parses the solar inputs file.
 
     Inputs:
         - debug:
@@ -1272,24 +1272,36 @@
         - logger:
             The :class:`logging.Logger` to use for the run.
         - scenarios:
             The `list` of :class:`Scenario` instances available for the run.
 
     Outputs:
         A `tuple` containing:
-        - The :class:`solar.PVPanel` being used for the run;
-        - The pv-panel cost information;
-        - The pv-panel emissions information;
-        - The :class:`HybridPVTPanel` being used for the run, if relevant;
-        - The pv-t-panel cost information, if relevant;
-        - The pv-t-panel emissions information, if relevant;
+        - A `list` of the :class:`solar.PVPanel` instances being used for the run;
+        - The pv-panel cost information for each panel being considered;
+        - The pv-panel emissions information for each panel being considered;
+        - A `list` of the :class:`HybridPVTPanel` being used for the run, if relevant;
+        - The pv-t-panel cost information for each panel being considered, if relevant;
+        - The pv-t-panel emissions informatio for each panel being considered, if
+          relevant;
         - The relative path to the solar generation inputs filepath.
 
     """
 
+    # Raise an error if both `pv_panel` and `pv_panels` etc. have been used.
+    if "pv_panel" in energy_system_inputs and "pv_panels" in energy_system_inputs:
+        logger.error(
+            "Cannot use both 'pv_panel' and 'pv_panels' in energy-system inputs. Only "
+            "one is acceptable use."
+        )
+        raise InputFileError(
+            "energy-system inputs",
+            "Both 'pv_panel' and 'pv_panels' keywords were used.",
+        )
+
     # Parse the solar input information.
     solar_generation_inputs_filepath = os.path.join(
         inputs_directory_relative_path,
         SOLAR_INPUTS_FILE,
     )
     solar_generation_inputs = read_yaml(
         solar_generation_inputs_filepath,
@@ -1321,158 +1333,211 @@
                     solar_panels,
                     thermal_model,
                 )
             )
 
     # Determine the PV panel being modelled.
     try:
-        pv_panel: Union[solar.PVPanel, solar.SolarPanel] = [
+        pv_panels: List[Union[solar.PVPanel, solar.SolarPanel]] = [
             panel
             for panel in solar_panels
             if panel.panel_type == solar.SolarPanelType.PV  # type: ignore
-            and panel.name == energy_system_inputs["pv_panel"]
-        ][0]
+            and (
+                panel.name == energy_system_inputs.get("pv_panel", "")
+                or panel.name in energy_system_inputs.get("pv_panels", [])
+            )
+        ]
     except IndexError:
         logger.error(
-            "%sPV panel %s not found in pv panel inputs.%s",
+            "%sPV panel%s %s not found in pv panel inputs.%s",
             BColours.fail,
-            energy_system_inputs["pv_panel"],
+            "(s)" if "pv_panels" in energy_system_inputs else "",
+            energy_system_inputs.get(
+                "pv_panel", ", ".join(energy_system_inputs.get("pv_panels", []))
+            ),
             BColours.endc,
         )
         raise
 
-    if not isinstance(pv_panel, solar.PVPanel):
-        logger.error(
-            "%sThe PV panel selected is not a valid PV panel.%s",
-            BColours.fail,
-            BColours.endc,
-        )
-        raise InputFileError(
-            "solar inputs OR energy system inputs",
-            "The PV panel selected is not a valid PV panel.",
-        )
+    for pv_panel in pv_panels:
+        if not isinstance(pv_panel, solar.PVPanel):
+            logger.error(
+                "%sThe PV panel, %s, selected is not a valid PV panel.%s",
+                BColours.fail,
+                pv_panel.name,
+                BColours.endc,
+            )
+            raise InputFileError(
+                "solar inputs OR energy system inputs",
+                "The PV panel selected is not a valid PV panel.",
+            )
 
     # Determine the PV panel costs.
     try:
-        pv_panel_costs: Dict[str, float] = [
-            panel_data[COSTS]
-            for panel_data in solar_generation_inputs["panels"]
-            if panel_data[NAME] == pv_panel.name
-        ][0]
+        pv_panel_costs: Dict[str, DefaultDict[str, float]] = {
+            pv_panel.name: [
+                defaultdict(float, panel_data[COSTS])
+                for panel_data in solar_generation_inputs["panels"]
+                if panel_data[NAME] == pv_panel.name
+            ][0]
+            for pv_panel in pv_panels
+        }
     except (KeyError, IndexError):
         logger.error(
-            "%sFailed to determine costs for PV panel %s.%s",
+            "%sFailed to determine costs for PV panel%s %s.%s",
             BColours.fail,
-            energy_system_inputs["pv_panel"],
+            "(s)" if "pv_panels" in energy_system_inputs else "",
+            energy_system_inputs.get(
+                "pv_panel", ", ".join(energy_system_inputs.get("pv_panels", []))
+            ),
             BColours.endc,
         )
         raise
     logger.info("PV panel costs successfully determined.")
 
     # Determine the PV panel emissions.
     try:
-        pv_panel_emissions: Dict[str, float] = [
-            panel_data[EMISSIONS]
-            for panel_data in solar_generation_inputs["panels"]
-            if panel_data[NAME] == pv_panel.name
-        ][0]
+        pv_panel_emissions: Dict[str, Dict[str, float]] = {
+            pv_panel.name: [
+                defaultdict(float, panel_data[EMISSIONS])
+                for panel_data in solar_generation_inputs["panels"]
+                if panel_data[NAME] == pv_panel.name
+            ][0]
+            for pv_panel in pv_panels
+        }
     except (KeyError, IndexError):
         logger.error(
-            "%sFailed to determine emissions for PV panel %s.%s",
+            "%sFailed to determine emissions for PV panel%s %s.%s",
             BColours.fail,
-            energy_system_inputs["pv_panel"],
+            "(s)" if "pv_panels" in energy_system_inputs else "",
+            energy_system_inputs.get(
+                "pv_panel", ", ".join(energy_system_inputs.get("pv_panels", []))
+            ),
             BColours.endc,
         )
         raise
     logger.info("PV panel emissions successfully determined.")
 
     # Determine the PVT panel being modelled, if appropriate.
-    if "pvt_panel" in energy_system_inputs:
+    if "pvt_panel" in energy_system_inputs or "pvt_panels" in energy_system_inputs:
+        # Raise an error if both `pvt_panel` and `pvt_panels` etc. have been used.
+        if "pvt_panel" in energy_system_inputs and "pvt_panels" in energy_system_inputs:
+            logger.error(
+                "Cannot use both 'pvt_panel' and 'pvt_panels' in energy-system inputs. "
+                "Only one is acceptable use."
+            )
+            raise InputFileError(
+                "energy-system inputs",
+                "Both 'pvt_panel' and 'pvt_panels' keywords were used.",
+            )
+
         try:
-            pvt_panel: Optional[Union[solar.HybridPVTPanel, solar.SolarPanel]] = [
+            pvt_panels: List[Union[solar.HybridPVTPanel, solar.SolarPanel]] = [
                 panel
                 for panel in solar_panels
                 if panel.panel_type == solar.SolarPanelType.PV_T  # type: ignore
-                and panel.name == energy_system_inputs["pvt_panel"]
-            ][0]
+                and (
+                    panel.name == energy_system_inputs.get("pvt_panel", "")
+                    or panel.name in energy_system_inputs.get("pvt_panels", [])
+                )
+            ]
             logger.info("PV-T panel successfully determined.")
         except IndexError:
             logger.error(
-                "%sPV-T panel %s not found in pv panel inputs.%s",
+                "%sPV-T panel%s %s not found in pv panel inputs.%s",
                 BColours.fail,
-                energy_system_inputs["pvt_panel"],
+                "(s)" if "pvt_panels" in energy_system_inputs else "",
+                energy_system_inputs.get(
+                    "pvt_panel", ", ".join(energy_system_inputs.get("pvt_panels", []))
+                ),
                 BColours.endc,
             )
             raise
 
-        if pvt_panel is None:
+        if len(pvt_panels) == 0:
             logger.error(
                 "%sThe PV-T panel selected caused an internal error when determining "
                 "the relevant panel data.%s",
                 BColours.fail,
                 BColours.endc,
             )
             raise InternalError(
                 "The PV-T panel selected was found but the information concerning it "
                 "was not successfully parsed."
             )
-        if not isinstance(pvt_panel, solar.HybridPVTPanel):
-            logger.error(
-                "%sThe PV-T panel selected %s is not a valid PV-T panel.%s",
-                BColours.fail,
-                energy_system_inputs["pv_panel"],
-                BColours.endc,
-            )
-            raise InputFileError(
-                "solar inputs OR energy system inputs",
-                "The PV-T panel selected is not a valid HybridPVTPanel.",
-            )
+        for pvt_panel in pvt_panels:
+            if not isinstance(pvt_panel, solar.HybridPVTPanel):
+                logger.error(
+                    "%sThe PV-T panel selected %s is not a valid PV-T panel.%s",
+                    BColours.fail,
+                    pvt_panel.name,
+                    BColours.endc,
+                )
+                raise InputFileError(
+                    "solar inputs OR energy system inputs",
+                    "The PV-T panel selected is not a valid HybridPVTPanel.",
+                )
 
-        logger.info("PV-T panel successfully parsed: %s.", pvt_panel.name)
+        logger.info(
+            "PV-T panel(s) successfully parsed: %s.",
+            ", ".join({entry.name for entry in pvt_panels}),
+        )
 
         try:
-            pvt_panel_costs: Optional[Dict[str, float]] = [
-                panel_data[COSTS]
-                for panel_data in solar_generation_inputs["panels"]
-                if panel_data[NAME] == pvt_panel.name
-            ][0]
+            pvt_panel_costs: Optional[Dict[str, DefaultDict[str, float]]] = {
+                pvt_panel.name: [
+                    defaultdict(float, panel_data[COSTS])
+                    for panel_data in solar_generation_inputs["panels"]
+                    if panel_data[NAME] == pvt_panel.name
+                ][0]
+                for pvt_panel in pvt_panels
+            }
         except (KeyError, IndexError):
             logger.error(
-                "%sFailed to determine costs for PV-T panel %s.%s",
+                "%sFailed to determine costs for PV-T panel%s %s.%s",
                 BColours.fail,
-                energy_system_inputs["pvt_panel"],
+                "(s)" if "pvt_panels" in energy_system_inputs else "",
+                energy_system_inputs.get(
+                    "pvt_panel", ", ".join(energy_system_inputs.get("pvt_panels", []))
+                ),
                 BColours.endc,
             )
             raise
         logger.info("PV-T panel costs successfully determined.")
         try:
-            pvt_panel_emissions: Optional[Dict[str, float]] = [
-                panel_data[EMISSIONS]
-                for panel_data in solar_generation_inputs["panels"]
-                if panel_data[NAME] == pvt_panel.name
-            ][0]
+            pvt_panel_emissions: Optional[Dict[str, DefaultDict[str, float]]] = {
+                pvt_panel.name: [
+                    defaultdict(float, panel_data[EMISSIONS])
+                    for panel_data in solar_generation_inputs["panels"]
+                    if panel_data[NAME] == pvt_panel.name
+                ][0]
+                for pvt_panel in pvt_panels
+            }
         except (KeyError, IndexError):
             logger.error(
-                "%sFailed to determine emissions for PV-T panel %s.%s",
+                "%sFailed to determine emissions for PV-T panel%s %s.%s",
                 BColours.fail,
-                energy_system_inputs["pvt_panel"],
+                "(s)" if "pvt_panels" in energy_system_inputs else "",
+                energy_system_inputs.get(
+                    "pvt_panel", ", ".join(energy_system_inputs.get("pvt_panels", []))
+                ),
                 BColours.endc,
             )
             raise
         logger.info("PV-T panel emissions successfully determined.")
     else:
-        pvt_panel = None
+        pvt_panels = []
         pvt_panel_costs = None
         pvt_panel_emissions = None
 
     return (
-        pv_panel,
+        pv_panels,  # type: ignore
         pv_panel_costs,
         pv_panel_emissions,
-        pvt_panel,
+        pvt_panels,  # type: ignore
         pvt_panel_costs,
         pvt_panel_emissions,
         solar_generation_inputs_filepath,
     )
 
 
 def _parse_tank_inputs(  # pylint: disable=too-many-statements
@@ -1707,18 +1772,18 @@
     str,
     Optional[Dict[str, float]],
     Optional[Dict[str, float]],
     Optional[str],
     Optional[Dict[str, float]],
     Optional[Dict[str, float]],
     Minigrid,
-    Dict[str, float],
-    Dict[str, float],
-    Optional[Dict[str, float]],
-    Optional[Dict[str, float]],
+    Dict[str, DefaultDict[str, float]],
+    Dict[str, DefaultDict[str, float]],
+    Optional[Dict[str, DefaultDict[str, float]]],
+    Optional[Dict[str, DefaultDict[str, float]]],
     str,
     Optional[str],
     Dict[str, Dict[str, float]],
     Dict[str, Dict[str, float]],
     str,
     Dict[str, Transmitter],
 ]:
@@ -1756,14 +1821,15 @@
         - Hot-water tank emissions,
         - The :class:`Minigrid` to use for the run,
         - PV costs,
         - PV emissions,
         - PV-T costs,
         - PV-T emissions,
         - Solar inputs filepath,
+        - Solar panels,
         - Tank inputs filepath,
         - Transmission costs,
         - Transmission emissions,
         - Transmission inputs filepath,
         - Transmitters.
 
     """
@@ -1802,26 +1868,24 @@
         scenarios,
     )
     logger.info(
         "Diesel generator %sinformation successfully parsed.",
         "and water heater " if diesel_water_heater is not None else "",
     )
 
-    pv_panel: solar.PVPanel
-    pv_panel_costs: Dict[str, float]
-    pv_panel_emissions: Dict[str, float]
-    pvt_panel: Optional[solar.HybridPVTPanel]
-    pvt_panel_costs: Optional[Dict[str, float]]
-    pvt_panel_emissions: Optional[Dict[str, float]]
+    pv_panel_costs: Dict[str, DefaultDict[str, float]]
+    pv_panel_emissions: Dict[str, DefaultDict[str, float]]
+    pvt_panel_costs: Optional[Dict[str, DefaultDict[str, float]]]
+    pvt_panel_emissions: Optional[Dict[str, DefaultDict[str, float]]]
     solar_generation_inputs_filepath: str
     (
-        pv_panel,
+        pv_panels,
         pv_panel_costs,
         pv_panel_emissions,
-        pvt_panel,
+        pvt_panels,
         pvt_panel_costs,
         pvt_panel_emissions,
         solar_generation_inputs_filepath,
     ) = _parse_solar_inputs(
         debug,
         energy_system_inputs,
         inputs_directory_relative_path,
@@ -1956,16 +2020,16 @@
         electric_water_heater = None
 
     minigrid: Minigrid = Minigrid.from_dict(
         diesel_generator,
         diesel_water_heater,
         electric_water_heater,
         energy_system_inputs,
-        pv_panel,
-        pvt_panel,
+        pv_panels,
+        pvt_panels,
         battery_inputs,
         exchanger_inputs,
         tank_inputs,
         water_pump,
     )
 
     if (
@@ -2532,16 +2596,20 @@
         lambda: defaultdict(float)
     )
     ghg_inputs.update(ghg_data)  # type: ignore
     logger.info("GHG inputs successfully parsed.")
 
     # Update the finance and GHG inputs accordingly with the PV data.
     logger.info("Updating with PV impact data.")
-    finance_inputs[ImpactingComponent.PV.value] = defaultdict(float, pv_panel_costs)
-    ghg_inputs[ImpactingComponent.PV.value] = defaultdict(float, pv_panel_emissions)
+    finance_inputs[ImpactingComponent.PV.value] = defaultdict(
+        lambda: defaultdict(float), pv_panel_costs  # type: ignore [arg-type, return-value]
+    )
+    ghg_inputs[ImpactingComponent.PV.value] = defaultdict(
+        lambda: defaultdict(float), pv_panel_emissions  # type: ignore [arg-type, return-value]
+    )
     logger.info("PV impact data successfully updated.")
 
     # Update the impact inputs with the diesel data.
     if any(
         scenario.diesel_scenario.mode != DieselMode.DISABLED for scenario in scenarios
     ):
         logger.info("Updating with diesel impact data.")
@@ -2590,18 +2658,18 @@
     else:
         logger.info("No battery present, skipping impact data.")
 
     if minigrid.pvt_panel is not None and any(scenario.pv_t for scenario in scenarios):
         if pvt_panel_costs is None or pvt_panel_emissions is None:
             raise InternalError("Error processing PV-T panel cost and emissions.")
         finance_inputs[ImpactingComponent.PV_T.value] = defaultdict(
-            float, pvt_panel_costs
+            float, pvt_panel_costs  # type: ignore [arg-type]
         )
         ghg_inputs[ImpactingComponent.PV_T.value] = defaultdict(
-            float, pvt_panel_emissions
+            float, pvt_panel_emissions  # type: ignore [arg-type]
         )
     else:
         logger.info("PV-T disblaed in scenario file, skipping PV-T impact parsing.")
 
     # Add transmitter impacts.
     for converter in converters.values():
         logger.info("Updating with %s impact data.", converter.name)
```

### Comparing `clover-energy-5.0.8/src/clover/generation/__utils__.py` & `clover-energy-5.1.0/src/clover/generation/__utils__.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,21 +20,21 @@
 locally within CLOVER. The profiles that are fetched are determined by the information
 that is passed in to the module.
 
 """
 
 import enum
 import json
+import math
 import os
 import threading
 import time
 
 from json.decoder import JSONDecodeError
 from logging import Logger
-from math import ceil
 from typing import Any, Dict, Union
 
 import numpy as np  # pylint: disable=import-error
 import pandas as pd  # pylint: disable=import-error
 import requests  # pylint: disable=import-error
 
 from tqdm import tqdm  # pylint: disable=import-error
@@ -190,14 +190,15 @@
         logger.error(
             "%sFailed to parse renewables.ninja data. Check that you correctly specified "
             "your API key: %s%s",
             BColours.fail,
             str(e),
             BColours.endc,
         )
+        logger.info("Session text: %s", session_url.text)
         raise RenewablesNinjaError() from None
 
     data_frame: pd.DataFrame = pd.DataFrame(
         pd.read_json(json.dumps(parsed_response["data"]), orient="index")
     )
     data_frame = data_frame.reset_index(drop=True)
 
@@ -333,14 +334,22 @@
 
     .. attribute:: location
         The location currently being considered.
 
     .. attribute:: logger
         The :class:`logging.Logger` to use for the run.
 
+    .. attribute:: pause_time
+        A time in seconds for which to pause before launching to avoid renewables.ninja
+        returning errors due to a large number of threads being launched in a short
+        space of time.
+
+    .. attribute:: profile_prefix
+        A prefix to append to the filenames.
+
     .. attribute:: regenerate
         Whether the profiles are to be regenerated, i.e., re-fetched from the
         renewables.ninja API (True) or whether existing profiles should be used if
         present (False).
 
     """
 
@@ -349,32 +358,39 @@
 
     def __init__(
         self,
         auto_generated_files_directory: str,
         generation_inputs: Dict[str, Any],
         location: Location,
         logger_name: str,
+        pause_time: int,
         regenerate: bool,
         sleep_multiplier: int,
         verbose: bool,
         *,
         renewables_ninja_params: Dict[str, Any],
+        profile_prefix: str = "",
     ) -> None:
         """
         Instantiate a renewables-ninja-base-data thread.
 
         Inputs:
             - auto_generated_files_directory:
                 The directory in which CLOVER-generated files should be saved.
             - generation_inputs:
                 The generation inputs.
             - location:
                 The location currently being considerted.
             - logger_name:
                 The name to use for the logger.
+            - pause_time:
+                A time for which to pause before initialising data fetching to avoid
+                short-burst errors from renewables.ninja.
+            - profile_prefix:
+                A prefix to append to the output filenames.
             - regenerate:
                 Whether to regenerate the profiles.
             - renewables_ninja_params:
                 Additional parameters to use when calling the renewables.ninja API.
             - sleep_multiplier:
                 The multiplier to use when computing how long to sleep for, used when
                 multiple threads are executed in parallel.
@@ -386,14 +402,16 @@
         self.auto_generated_files_directory: str = auto_generated_files_directory
         self.generation_inputs: Dict[
             str, Union[bool, int, str, float]
         ] = generation_inputs
         self.location: Location = location
         self.logger: Logger = get_logger(logger_name, verbose)
         self.logger_name: str = logger_name
+        self.pause_time: int = pause_time
+        self.profile_prefix: str = profile_prefix
         self.regenerate: bool = regenerate
         self.renewables_ninja_params: Dict[str, Any] = renewables_ninja_params
         self.sleep_multiplier: int = sleep_multiplier
 
         super().__init__()
 
     def __init_subclass__(cls, profile_name: str, profile_key: str) -> None:
@@ -431,27 +449,33 @@
             )
 
         self.logger.info(
             "RenewablesNinja data thread instantiated for %s profiles.",
             self.profile_name,
         )
 
+        # To avoid a high burst of calls, a random sleep up to the sleep time is made.
+        time.sleep(self.pause_time)
+
         # A counter is used to keep track of calls to renewables.ninja to prevent
         # overloading.
         try:
             for year in tqdm(
                 range(
                     int(self.generation_inputs["start_year"]),
                     int(self.generation_inputs["end_year"]) + 1,
                 ),
-                desc=f"{self.profile_name} profiles",
+                desc=f"{self.profile_name} "
+                f"{self.profile_prefix[:-1].replace('_', ' ')} profiles",
                 unit="year",
             ):
                 # If the data file for the year already exists, skip.
-                filename = f"{self.profile_name}_generation_{year}.csv"
+                filename = (
+                    f"{self.profile_prefix}{self.profile_name}_generation_{year}.csv"
+                )
                 filepath = os.path.join(self.auto_generated_files_directory, filename)
 
                 if os.path.isfile(filepath) and not self.regenerate:
                     self.logger.info(
                         "Data file for year %s already exists, skipping.", year
                     )
                     continue
@@ -518,14 +542,15 @@
 def total_profile_output(
     generation_directory: str,
     regenerate: bool,
     start_year: int = 2007,
     num_years: int = 20,
     *,
     profile_name: str,
+    profile_prefix: str,
 ) -> pd.DataFrame:
     """
     Generates total output data by taking the input years and repeating them.
 
     Inputs:
         - generation_directory:
             The directory in which generated profiles are saved.
@@ -533,23 +558,25 @@
             Whether to regenerate the profiles.
         - start_year:
             The year for which to begin the simulation.
         - num_years:
             The number of year for which to run the simulation.
         - profile_name:
             The name to use for saving the profiles.
-    Outputs:
+
+                Outputs:
         .csv file for twenty years of PV output data
+
     """
 
     output = pd.DataFrame([])
 
     total_output_filename = os.path.join(
         generation_directory,
-        f"{profile_name}_generation_{num_years}_years.csv",
+        f"{profile_prefix}{profile_name}_generation_{num_years}_years.csv",
     )
 
     # If the total output file already exists then simply read this in.
     if os.path.isfile(total_output_filename) and not regenerate:
         with open(total_output_filename, "r") as f:
             total_output = pd.read_csv(f)
 
@@ -561,26 +588,26 @@
             leave=True,
             unit="year",
         ):
             iteration_year = start_year + year_index
             with open(
                 os.path.join(
                     generation_directory,
-                    f"{profile_name}_generation_{iteration_year}.csv",
+                    f"{profile_prefix}{profile_name}_generation_{iteration_year}.csv",
                 ),
                 "r",
             ) as f:
                 iteration_year_data = pd.read_csv(
                     f,
                 )
             output = pd.concat([output, iteration_year_data], ignore_index=True)
 
         # Repeat the initial data in consecutive periods
         total_output = pd.DataFrame([])
-        for _ in range(int(ceil(num_years / 10))):
+        for _ in range(int(math.ceil(num_years / 10))):
             total_output = pd.concat([total_output, output], ignore_index=True)
         with open(total_output_filename, "w") as f:
             total_output.to_csv(
                 f,  # type: ignore
                 index=False,
                 line_terminator="\n",
             )
```

### Comparing `clover-energy-5.0.8/src/clover/generation/solar.py` & `clover-energy-5.1.0/src/clover/generation/solar.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 for use locally within CLOVER.
 
 """
 
 import enum
 
 from logging import Logger
-from typing import Any, Dict, List, Optional, Tuple
+from typing import Any, Dict, List, Optional, Tuple, Union
 
 import pandas as pd  # pylint: disable=import-error
 
 # from sklearn.linear_model._coordinate_descent import Lasso
 
 from ..__utils__ import (
     BColours,
@@ -33,14 +33,15 @@
     Location,
     NAME,
     ProgrammerJudgementFault,
 )
 from .__utils__ import BaseRenewablesNinjaThread, SolarDataType, total_profile_output
 
 __all__ = (
+    "get_profile_prefix",
     "HybridPVTPanel",
     "PVPanel",
     "SolarDataThread",
     "SolarDataType",
     "SolarPanelType",
     "solar_degradation",
     "SOLAR_LOGGER_NAME",
@@ -48,23 +49,38 @@
 )
 
 
 # Default PV unit:
 #   The default PV unit size to use, measured in kWp.
 DEFAULT_PV_UNIT: float = 1  # [kWp]
 
+# Default tracking:
+#   The default keyword to use for fixed-mounted panels.
+_DEFAULT_TRACKING: str = "fixed"
+
 # Reference solar irradiance:
 #   The reference solar irradiance, used to compute fractional PV-T electric
 #   performance values.
 REFERENCE_SOLAR_IRRADIANCE: float = 1000  # [W/m^2]
 
 # Solar logger name:
 #   The name to use for the solar logger.
 SOLAR_LOGGER_NAME = "solar_generation"
 
+# Tracking map:
+#   Map used for determining the tracking state of the panels.
+_TRACKING_MAP: Dict[str, int] = {
+    _DEFAULT_TRACKING: 0,
+    "single": 1,
+    "single_axis": 1,
+    "azimuthal": 1,
+    "dual": 2,
+    "dual_axis": 2,
+}
+
 
 class SolarPanelType(enum.Enum):
     """
     Specifies the type of solar panel being considered.
 
     - PV:
         Denotes that a PV panel is being considered.
@@ -73,14 +89,57 @@
 
     """
 
     PV = "pv"
     PV_T = "pv_t"
 
 
+class Tracking(enum.Enum):
+    """
+    Specifies the tracking state of the panel being considered.
+
+    - FIXED:
+        Denotes that the panel is fixed in both its azimuthal orientation and tilt.
+    - SINGLE_AXIS:
+        Denotes that the panel is single-axis tracking, i.e., has a fixed tilt but its
+        azimuthal orietntation can change.
+    - DUAL_AXIS:
+        Denotes that the panel is dual-axis tracking, i.e., both its azimuthal
+        orientation and tilt can change.
+
+    """
+
+    FIXED: int = 0
+    SINGLE_AXIS: int = 1
+    DUAL_AXIS: int = 2
+
+    @classmethod
+    def from_text(cls, logger: Logger, text: str) -> Any:
+        """
+        Used to instntiate the :class:`Tracking` instance based on the input text.
+
+        Inputs:
+            - text:
+                The text describing the tracking from the input file.
+
+        """
+
+        try:
+            return cls(_TRACKING_MAP[text])
+        except KeyError as err:
+            logger.error(
+                "Input value of %s for tracking type is not valid. Valid tracking modes: %s",
+                text,
+                ", ".join([f"'{key}'" for key in _TRACKING_MAP]),
+            )
+            raise InputFileError(
+                "solar_generation_inputs", f"Tracking mode '{text}' is not valid."
+            ) from err
+
+
 class SolarPanel:  # pylint: disable=too-few-public-methods
     """
     Represents a solar panel being considered.
 
     .. attribute:: azimuthal_orientation
         The azimuthal orientation of the panel, defined in degrees from North.
 
@@ -115,23 +174,23 @@
 
     """
 
     panel_type: SolarPanelType
 
     def __init__(
         self,
-        azimuthal_orientation: float,
+        azimuthal_orientation: Optional[float],
         lifetime: int,
         name: str,
         pv_unit: float,
         pv_unit_overrided: bool,
         reference_efficiency: Optional[float],
         reference_temperature: Optional[float],
         thermal_coefficient: Optional[float],
-        tilt: float,
+        tilt: Optional[float],
     ) -> None:
         """
         Instantiate a :class:`SolarPanel` instance.
 
         Inputs:
             - azimuthal_orientation:
                 The azimuthal orientation of the :class:`SolarPanel`.
@@ -155,23 +214,23 @@
                 The thermal coefficient of the PV layer of the panel, if required,
                 otherwise `None`.
             - tilt:
                 The tilt of the panel in degrees above the horizontal.
 
         """
 
-        self.azimuthal_orientation: float = azimuthal_orientation
+        self.azimuthal_orientation: Optional[float] = azimuthal_orientation
         self.lifetime: int = lifetime
         self.name: str = name
         self.pv_unit: float = pv_unit
         self.pv_unit_overrided: bool = pv_unit_overrided
         self.reference_efficiency: Optional[float] = reference_efficiency
         self.reference_temperature: Optional[float] = reference_temperature
         self.thermal_coefficient: Optional[float] = thermal_coefficient
-        self.tilt: float = tilt
+        self.tilt: Optional[float] = tilt
 
     def __init_subclass__(cls, panel_type: SolarPanelType) -> None:
         """
         The init_subclass hook, run on instantiation of the :class:`SolarPanel`.
 
         Inputs:
             - panel_type:
@@ -189,16 +248,111 @@
 
 class PVPanel(
     SolarPanel, panel_type=SolarPanelType.PV
 ):  # pylint: disable=too-few-public-methods
     """
     Represents a photovoltaic panel.
 
+    .. attribute:: tracking
+        Whether the panel is tracking or not.
+
     """
 
+    def __init__(
+        self,
+        azimuthal_orientation: Optional[float],
+        lifetime: int,
+        name: str,
+        pv_unit: float,
+        pv_unit_overrided: bool,
+        reference_efficiency: Optional[float],
+        reference_temperature: Optional[float],
+        thermal_coefficient: Optional[float],
+        tilt: Optional[float],
+        tracking: Tracking,
+    ) -> None:
+        """
+        Instantiate a :class:`PVPanel` instance.
+
+        Inputs:
+            - azimuthal_orientation:
+                The azimuthal orientation of the :class:`PVPanel` or `None` if the panel
+                is either single- or dual-axis tracking.
+            - lifetime:
+                The lifetime of the :class:`PVPanel` in years.
+            - name:
+                The name to assign to the :class:`PVPanel` in order to uniquely
+                identify it.
+            - pv_unit:
+                The output power, in Watts, of the PV layer of the panel per unit panel
+                installed.
+            - pv_unit_overrided:
+                Whether this unit has been overrided from its default value (True) or
+                not (False).
+            - reference_efficiency:
+                The reference efficiency of the panel, if required, otherwise `None`.
+            - reference_temperature:
+                The temperature, in degrees Celcius, at which the reference efficiency
+                is defined, if required, otherwise `None`.
+            - thermal_coefficient:
+                The thermal coefficient of the PV layer of the panel, if required,
+                otherwise `None`.
+            - tilt:
+                The tilt of the panel in degrees above the horizontal, if specified, or
+                `None` if the panel is dual-axis tracking..
+            - tracking:
+                The state of the panel's tracking.
+
+        """
+
+        self.tracking = tracking
+
+        super().__init__(
+            azimuthal_orientation,
+            lifetime,
+            name,
+            pv_unit,
+            pv_unit_overrided,
+            reference_efficiency,
+            reference_temperature,
+            thermal_coefficient,
+            tilt,
+        )
+
+    def __hash__(self) -> int:
+        """
+        Return a unique identifier for the panel.
+
+        Because the solar panel instances are used for fetching weather data, panels
+        with unique tilt, azimuthal orientation, and tracking, need to be kept separate.
+
+        These parameters are hence used to determine the "unique" hash for the panel.
+
+        """
+
+        return hash(
+            self.tracking.value
+            + 3
+            * (
+                self.azimuthal_orientation
+                if self.azimuthal_orientation is not None
+                else 0
+            )
+            + 540 * (self.tilt if self.tilt is not None else 0)
+        )
+
+    def __eq__(self, other: Any) -> bool:
+        """Used to determine whether to instances are identical for creating a set."""
+
+        return (  # type: ignore[no-any-return]
+            self.tracking == other.tracking
+            and self.azimuthal_orientation == other.azimuthal_orientation
+            and self.tilt == other.tilt
+        )
+
     @classmethod
     def from_dict(cls, logger: Logger, solar_inputs: Dict[str, Any]) -> Any:
         """
         Instantiate a :class:`PVPanel` instance based on the input data.
 
         Inputs:
             - logger:
@@ -220,30 +374,47 @@
                 "`pv_unit` variable specified, using a pv unit of %s kWp", pv_unit
             )
         else:
             pv_unit = DEFAULT_PV_UNIT
             pv_unit_overrided = False
             logger.info("No `pv_unit` keyword specified, defaulting to %s kWp", pv_unit)
 
+        tracking: Tracking = Tracking.from_text(
+            logger, solar_inputs.get("tracking", _DEFAULT_TRACKING)
+        )
+
+        if tracking == Tracking.FIXED:
+            azimuthal_orientation: Optional[float] = solar_inputs[
+                "azimuthal_orientation"
+            ]
+        else:
+            azimuthal_orientation = None
+
+        if tracking != Tracking.DUAL_AXIS:
+            tilt: Optional[float] = solar_inputs["tilt"]
+        else:
+            tilt = None
+
         return cls(
-            solar_inputs["azimuthal_orientation"],
+            azimuthal_orientation,
             solar_inputs["lifetime"],
             solar_inputs[NAME],
             pv_unit,
             pv_unit_overrided,
             solar_inputs["reference_efficiency"]
             if "reference_efficiency" in solar_inputs
             else None,
             solar_inputs["reference_temperature"]
             if "reference_temperature" in solar_inputs
             else None,
             solar_inputs["thermal_coefficient"]
             if "thermal_coefficient" in solar_inputs
             else None,
-            solar_inputs["tilt"],
+            tilt,
+            tracking,
         )
 
 
 class HybridPVTPanel(SolarPanel, panel_type=SolarPanelType.PV_T):
     """
     Represents a PV-T panel.
 
@@ -378,14 +549,43 @@
             + f", thermal_coefficient={self.thermal_coefficient}"
             + f", thermal_model={self.thermal_model}"
             + f", thermal_unit={self.thermal_unit}"
             + f", tilt={self.tilt}"
             + ")"
         )
 
+    def __hash__(self) -> int:
+        """
+        Return a unique identifier for the panel.
+
+        Because the solar panel instances are used for fetching weather data, panels
+        with unique tilt, azimuthal orientation, and tracking, need to be kept separate.
+
+        These parameters are hence used to determine the "unique" hash for the panel.
+
+        """
+
+        return hash(
+            3
+            * (
+                self.azimuthal_orientation
+                if self.azimuthal_orientation is not None
+                else 0
+            )
+            + 540 * (self.tilt if self.tilt is not None else 0)
+        )
+
+    def __eq__(self, other: Any) -> bool:
+        """Used to determine whether to instances are identical for creating a set."""
+
+        return (  # type: ignore[no-any-return]
+            self.azimuthal_orientation == other.azimuthal_orientation
+            and self.tilt == other.tilt
+        )
+
     def calculate_performance(
         self,
         ambient_temperature: float,
         input_temperature: float,
         logger: Logger,
         mass_flow_rate: float,
         solar_irradiance: float,
@@ -483,14 +683,42 @@
                 str(e),
             )
             raise
 
         return fractional_electric_performance, output_temperature
 
 
+def get_profile_prefix(panel: Union[PVPanel, HybridPVTPanel]) -> str:
+    """
+    Determine the prefix to use for profile names based on the tracking and angles.
+
+    Inputs:
+        - panel:
+            The :class:`PVPanel` to determine the profile prefix for.
+
+    """
+
+    if isinstance(panel, HybridPVTPanel):
+        tracking = Tracking.DUAL_AXIS
+    else:
+        tracking = panel.tracking
+
+    if tracking == Tracking.SINGLE_AXIS:
+        return f"single_axis_tilt_{panel.tilt}_"
+    if tracking == Tracking.DUAL_AXIS:
+        return "dual_axis_"
+    if tracking == Tracking.FIXED:
+        return f"fixed_tilt_{panel.tilt}_azim_{panel.azimuthal_orientation}_"
+
+    raise ProgrammerJudgementFault(
+        "generation.solar::get_profile_prefix",
+        f"Code not written for switch for tracking value {tracking.value}",
+    )
+
+
 def solar_degradation(lifetime: int, num_years: int) -> pd.DataFrame:
     """
     Calculates the solar degredation.
 
     Inputs:
         - lifetime:
             The lifetime of the solar setup in years.
@@ -515,22 +743,32 @@
 
 class SolarDataThread(
     BaseRenewablesNinjaThread, profile_name="solar", profile_key="pv"
 ):
     """
     Class to use when calling the solar data thread.
 
+    Options which are not immediately obvious are documented here:
+    - tracking:
+        Used for specifying whether the panels are tracking. Available options:
+        - 0 -> The panels do not track the sun;
+        - 1 -> The panels are single-axis tracking, i.e., track azimuthally but have a
+            fixed tilt angle;
+        - 2 -> The panels are dual-axis tracking, i.e., track both azimuthally and with
+            their tilt.
+
     """
 
     def __init__(
         self,
         auto_generated_files_directory: str,
         generation_inputs: Dict[str, Any],
         location: Location,
         logger_name: str,
+        pause_time: int,
         regenerate: bool,
         pv_panel: PVPanel,
         sleep_multiplier: int = 1,
         verbose: bool = False,
     ):
         """
         Instantiate a :class:`SolarDataThread` instance.
@@ -541,31 +779,50 @@
         renewables_ninja_params = {
             "dataset": "merra2",
             "lat": float(location.latitude),
             "lon": float(location.longitude),
             "local_time": "false",
             "capacity": 1.0,
             "system_loss": 0,
-            "tracking": 0,
-            "tilt": pv_panel.tilt,
-            "azim": pv_panel.azimuthal_orientation,
+            "tracking": pv_panel.tracking.value,
             "raw": "true",
         }
+
+        renewables_ninja_params["azim"] = (
+            pv_panel.azimuthal_orientation
+            if pv_panel.azimuthal_orientation is not None
+            else "false"
+        )
+        renewables_ninja_params["tilt"] = (
+            pv_panel.tilt if pv_panel.tilt is not None else "false"
+        )
+
+        # Determine the prefix to use for the solar profiles dependent on tracking.
+        profile_prefix = get_profile_prefix(pv_panel)
+
         super().__init__(
             auto_generated_files_directory,
             generation_inputs,
             location,
             logger_name,
+            pause_time,
             regenerate,
             sleep_multiplier,
             verbose,
             renewables_ninja_params=renewables_ninja_params,
+            profile_prefix=profile_prefix,
         )
 
 
-def total_solar_output(*args, **kwargs) -> pd.DataFrame:  # type: ignore
+def total_solar_output(
+    *args, pv_panel: Union[PVPanel, HybridPVTPanel]
+) -> pd.DataFrame:  # type: ignore
     """
     Wrapper function to wrap the total solar output.
 
     """
 
-    return total_profile_output(*args, **kwargs, profile_name="solar")
+    return total_profile_output(
+        *args,
+        profile_name="solar",
+        profile_prefix=get_profile_prefix(pv_panel),
+    )
```

### Comparing `clover-energy-5.0.8/src/clover/generation/weather.py` & `clover-energy-5.1.0/src/clover/generation/weather.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,15 @@
 
     def __init__(
         self,
         auto_generated_files_directory: str,
         generation_inputs: Dict[str, Any],
         location: Location,
         logger_name: str,
+        pause_time: int,
         regenerate: bool,
         sleep_multiplier: int = 1,
         verbose: bool = False,
     ):
         """
         Instantiate a :class:`WeatherDataThread` instance.
 
@@ -120,14 +121,15 @@
             "var_cldtot": "true",
         }
         super().__init__(
             auto_generated_files_directory,
             generation_inputs,
             location,
             logger_name,
+            pause_time,
             regenerate,
             sleep_multiplier,
             verbose,
             renewables_ninja_params=renewables_ninja_params,
         )
```

### Comparing `clover-energy-5.0.8/src/clover/generation/wind.py` & `clover-energy-5.1.0/src/clover/generation/wind.py`

 * *Files 7% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 
     def __init__(
         self,
         auto_generated_files_directory: str,
         generation_inputs: Dict[str, Any],
         location: Location,
         logger_name: str,
+        pause_time: int,
         regenerate: bool,
         sleep_multiplier: int = 1,
         verbose: bool = False,
     ):
         """
         Instantiate a :class:`WindDataThread` instance.
 
@@ -77,14 +78,15 @@
             "raw": "true",
         }
         super().__init__(
             auto_generated_files_directory,
             generation_inputs,
             location,
             logger_name,
+            pause_time,
             regenerate,
             sleep_multiplier,
             verbose,
             renewables_ninja_params=renewables_ninja_params,
         )
```

### Comparing `clover-energy-5.0.8/src/clover/impact/__init__.py` & `clover-energy-5.1.0/src/clover/impact/__init__.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.8/src/clover/impact/__utils__.py` & `clover-energy-5.1.0/src/clover/impact/__utils__.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.8/src/clover/impact/finance.py` & `clover-energy-5.1.0/src/clover/impact/finance.py`

 * *Files 2% similar despite different names*

```diff
@@ -379,15 +379,15 @@
     return inverter_discounted_cost
 
 
 def _misc_costs(
     diesel_size: float,
     misc_capacity_cost: float,
     misc_fixed_cost: float,
-    pv_array_size: float,
+    pv_array_size: Dict[str, float],
 ) -> float:
     """
     Calculates cost of miscellaneous capacity-related costs
 
     Inputs:
         - diesel_size:
             Capacity of diesel generator being installed
@@ -400,15 +400,17 @@
             Capacity of PV being installed
 
     Outputs:
         The undiscounted cost.
 
     """
 
-    total_misc_capacity_cost = (pv_array_size + diesel_size) * misc_capacity_cost
+    total_misc_capacity_cost = (
+        sum(pv_array_size.values()) + diesel_size
+    ) * misc_capacity_cost
 
     return total_misc_capacity_cost + misc_fixed_cost
 
 
 ###############################
 # Externally facing functions #
 ###############################
@@ -419,15 +421,15 @@
     clean_water_tanks: float,
     converters: Dict[str, int],
     diesel_size: float,
     finance_inputs: Dict[str, Any],
     heat_exchangers: float,
     hot_water_tanks: float,
     logger: Logger,
-    pv_array_size: float,
+    pv_array_size: Dict[str, float],
     pvt_array_size: float,
     storage_size: float,
     installation_year: int = 0,
 ) -> float:
     """
     Calculates all equipment costs.
 
@@ -460,18 +462,19 @@
 
     Outputs:
         The combined undiscounted cost of the system equipment.
 
     """
 
     # Calculate the various system costs.
+    # compoennts.
     bos_cost = _component_cost(
         finance_inputs[ImpactingComponent.BOS.value][COST],
         finance_inputs[ImpactingComponent.BOS.value][COST_DECREASE],
-        pv_array_size,
+        sum(pv_array_size.values()),
         installation_year,
     )
 
     if ImpactingComponent.BUFFER_TANK.value not in finance_inputs and buffer_tanks > 0:
         logger.error(
             "%sNo buffer tank financial input information provided.%s",
             BColours.fail,
@@ -642,25 +645,33 @@
             finance_inputs[ImpactingComponent.HOT_WATER_TANK.value][INSTALLATION_COST],
             finance_inputs[ImpactingComponent.HOT_WATER_TANK.value][
                 INSTALLATION_COST_DECREASE
             ],
             installation_year,
         )
 
-    pv_cost = _component_cost(
-        finance_inputs[ImpactingComponent.PV.value][COST],
-        finance_inputs[ImpactingComponent.PV.value][COST_DECREASE],
-        pv_array_size,
-        installation_year,
+    pv_cost = sum(
+        _component_cost(
+            finance_inputs[ImpactingComponent.PV.value][panel_name][COST],
+            finance_inputs[ImpactingComponent.PV.value][panel_name][COST_DECREASE],
+            array_size,
+            installation_year,
+        )
+        for panel_name, array_size in pv_array_size.items()
     )
-    pv_installation_cost = _component_installation_cost(
-        pv_array_size,
-        finance_inputs[ImpactingComponent.PV.value][INSTALLATION_COST],
-        finance_inputs[ImpactingComponent.PV.value][INSTALLATION_COST_DECREASE],
-        installation_year,
+    pv_installation_cost = sum(
+        _component_installation_cost(
+            array_size,
+            finance_inputs[ImpactingComponent.PV.value][panel_name][INSTALLATION_COST],
+            finance_inputs[ImpactingComponent.PV.value][panel_name][
+                INSTALLATION_COST_DECREASE
+            ],
+            installation_year,
+        )
+        for panel_name, array_size in pv_array_size.items()
     )
 
     if ImpactingComponent.PV_T.value not in finance_inputs and pvt_array_size > 0:
         logger.error(
             "%sNo PV-T financial input information provided.%s",
             BColours.fail,
             BColours.endc,
@@ -672,15 +683,15 @@
         )
     pvt_cost: float = 0
     pvt_installation_cost: float = 0
     if pvt_array_size > 0:
         pvt_cost = _component_cost(
             finance_inputs[ImpactingComponent.PV_T.value][COST],
             finance_inputs[ImpactingComponent.PV_T.value][COST_DECREASE],
-            pv_array_size,
+            pvt_array_size,
             installation_year,
         )
         pvt_installation_cost = _component_installation_cost(
             pvt_array_size,
             finance_inputs[ImpactingComponent.PV_T.value][INSTALLATION_COST],
             finance_inputs[ImpactingComponent.PV_T.value][INSTALLATION_COST_DECREASE],
             installation_year,
@@ -921,15 +932,15 @@
     clean_water_tanks: int,
     converters: Dict[str, int],
     diesel_size: float,
     finance_inputs: Dict[str, Any],
     heat_exchangers: int,
     hot_water_tanks: int,
     logger: Logger,
-    pv_array_size: float,
+    pv_array_size: Dict[str, float],
     pvt_array_size: float,
     storage_size: float,
     installation_year: int = 0,
 ) -> float:
     """
     Calculates cost of all equipment costs
 
@@ -1077,15 +1088,15 @@
     clean_water_tanks: int,
     converters: Optional[Dict[str, int]],
     diesel_size: float,
     finance_inputs: Dict[str, Any],
     heat_exchangers: int,
     hot_water_tanks: int,
     logger: Logger,
-    pv_array_size: float,
+    pv_array_size: Dict[str, float],
     pvt_array_size: float,
     storage_size: float,
     *,
     start_year: int = 0,
     end_year: int = 20,
 ) -> float:
     """
@@ -1258,21 +1269,24 @@
             hot_water_tanks,
             finance_inputs,
             logger,
             start_year=start_year,
             end_year=end_year,
         )
 
-    pv_om = _component_om(
-        finance_inputs[ImpactingComponent.PV.value][OM],
-        pv_array_size,
-        finance_inputs,
-        logger,
-        start_year=start_year,
-        end_year=end_year,
+    pv_om = sum(
+        _component_om(
+            finance_inputs[ImpactingComponent.PV.value][panel_name][OM],
+            array_size,
+            finance_inputs,
+            logger,
+            start_year=start_year,
+            end_year=end_year,
+        )
+        for panel_name, array_size in pv_array_size.items()
     )
 
     if ImpactingComponent.PV_T.value not in finance_inputs and pvt_array_size > 0:
         logger.error(
             "%sNo PV-T financial input information provided.%s",
             BColours.fail,
             BColours.endc,
```

### Comparing `clover-energy-5.0.8/src/clover/impact/ghgs.py` & `clover-energy-5.1.0/src/clover/impact/ghgs.py`

 * *Files 5% similar despite different names*

```diff
@@ -187,15 +187,15 @@
     clean_water_tanks: int,
     converters: Dict[str, int],
     diesel_size: float,
     ghg_inputs: Dict[str, Any],
     heat_exchangers: int,
     hot_water_tanks: int,
     logger: Logger,
-    pv_array_size: float,
+    pv_array_size: Dict[str, float],
     pvt_array_size: float,
     storage_size: float,
     year: int = 0,
 ) -> float:
     """
     Calculates ghgs of all newly installed equipment
 
@@ -227,15 +227,15 @@
     Outputs:
         GHGs
 
     """
 
     # Calculate system ghgs.
     bos_ghgs = calculate_ghgs(
-        pv_array_size, ghg_inputs, ImpactingComponent.BOS.value, year
+        sum(pv_array_size.values()), ghg_inputs, ImpactingComponent.BOS.value, year
     )
 
     if ImpactingComponent.BUFFER_TANK.value not in ghg_inputs and buffer_tanks > 0:
         logger.error(
             "%sNo buffer-tank GHG input information provided.%s",
             BColours.fail,
             BColours.endc,
@@ -364,19 +364,25 @@
             ImpactingComponent.HOT_WATER_TANK.value,
             year,
         )
         hot_water_tank_installation_ghgs = calculate_installation_ghgs(
             hot_water_tanks, ghg_inputs, ImpactingComponent.HOT_WATER_TANK.value, year
         )
 
-    pv_ghgs = calculate_ghgs(
-        pv_array_size, ghg_inputs, ImpactingComponent.PV.value, year
+    pv_ghgs = sum(
+        calculate_ghgs(
+            array_size, ghg_inputs[ImpactingComponent.PV.value], panel_name, year
+        )
+        for panel_name, array_size in pv_array_size.items()
     )
-    pv_installation_ghgs = calculate_installation_ghgs(
-        pv_array_size, ghg_inputs, ImpactingComponent.PV.value, year
+    pv_installation_ghgs = sum(
+        calculate_installation_ghgs(
+            array_size, ghg_inputs[ImpactingComponent.PV.value], panel_name, year
+        )
+        for panel_name, array_size in pv_array_size.items()
     )
 
     if ImpactingComponent.PV_T.value not in ghg_inputs and pvt_array_size > 0:
         logger.error(
             "%sNo PV-T GHG input information provided.%s", BColours.fail, BColours.endc
         )
         raise InputFileError(
@@ -398,15 +404,17 @@
         )
 
     storage_ghgs = calculate_ghgs(
         storage_size, ghg_inputs, ImpactingComponent.STORAGE.value, year
     )
 
     # Calculate misc GHGs.
-    misc_ghgs = calculate_misc_ghgs(diesel_size + pv_array_size, ghg_inputs)
+    misc_ghgs = calculate_misc_ghgs(
+        diesel_size + sum(pv_array_size.values()), ghg_inputs
+    )
 
     return (
         bos_ghgs
         + buffer_tank_ghgs
         + buffer_tank_installation_ghgs
         + clean_water_tank_installation_ghgs
         + clean_water_tank_ghgs
@@ -814,15 +822,15 @@
     clean_water_tanks: int,
     converters: Optional[Dict[str, int]],
     diesel_size: float,
     ghg_inputs: Dict[str, Any],
     heat_exchangers: int,
     hot_water_tanks: int,
     logger: Logger,
-    pv_array_size: float,
+    pv_array_size: Dict[str, float],
     pvt_array_size: float,
     storage_size: float,
     start_year: int = 0,
     end_year: int = 20,
 ) -> float:
     """
     Calculates total O&M ghgs over the simulation period
@@ -975,16 +983,23 @@
             hot_water_tanks,
             ghg_inputs,
             ImpactingComponent.HOT_WATER_TANK.value,
             start_year,
             end_year,
         )
 
-    pv_om_ghgs = calculate_om_ghgs(
-        pv_array_size, ghg_inputs, ImpactingComponent.PV.value, start_year, end_year
+    pv_om_ghgs = sum(
+        calculate_om_ghgs(
+            array_size,
+            ghg_inputs[ImpactingComponent.PV.value],
+            panel_name,
+            start_year,
+            end_year,
+        )
+        for panel_name, array_size in pv_array_size.items()
     )
 
     if ImpactingComponent.PV_T.value not in ghg_inputs and pvt_array_size > 0:
         logger.error(
             "%sNo PV-T GHG input information provided.%s", BColours.fail, BColours.endc
         )
         raise InputFileError(
```

### Comparing `clover-energy-5.0.8/src/clover/load/__init__.py` & `clover-energy-5.1.0/src/clover/load/__init__.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.8/src/clover/load/load.py` & `clover-energy-5.1.0/src/clover/load/load.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.8/src/clover/mains_supply/__init__.py` & `clover-energy-5.1.0/src/clover/mains_supply/__init__.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.8/src/clover/mains_supply/__utils__.py` & `clover-energy-5.1.0/src/clover/mains_supply/__utils__.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.8/src/clover/mains_supply/grid.py` & `clover-energy-5.1.0/src/clover/mains_supply/grid.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.8/src/clover/mains_supply/water_source.py` & `clover-energy-5.1.0/src/clover/mains_supply/water_source.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.8/src/clover/optimisation/__init__.py` & `clover-energy-5.1.0/src/clover/optimisation/__init__.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.8/src/clover/optimisation/__utils__.py` & `clover-energy-5.1.0/src/clover/optimisation/__utils__.py`

 * *Files 0% similar despite different names*

```diff
@@ -940,25 +940,25 @@
 def recursive_iteration(  # pylint: disable=too-many-locals
     conventional_cw_source_profiles: Optional[Dict[WaterSource, pd.DataFrame]],
     disable_tqdm: bool,
     end_year: int,
     finance_inputs: Dict[str, Any],
     ghg_inputs: Dict[str, Any],
     grid_profile: Optional[pd.DataFrame],
-    irradiance_data: pd.Series,
+    irradiance_data: Dict[str, pd.Series],
     kerosene_usage: pd.DataFrame,
     location: Location,
     logger: Logger,
     minigrid: energy_system.Minigrid,
     optimisation: Optimisation,
     previous_system: Optional[SystemAppraisal],
     start_year: int,
-    temperature_data: pd.Series,
+    temperature_data: Dict[str, pd.Series],
     total_loads: Dict[ResourceType, Optional[pd.DataFrame]],
-    total_solar_pv_power_produced: pd.Series,
+    total_solar_pv_power_produced: Dict[str, pd.Series],
     wind_speed_data: Optional[pd.Series],
     yearly_electric_load_statistics: pd.DataFrame,
     *,
     component_sizes: Dict[
         Union[Converter, ImpactingComponent, RenewableEnergySource],
         Union[int, float],
     ],
@@ -1053,15 +1053,15 @@
             kerosene_usage,
             location,
             logger,
             minigrid,
             int(component_sizes[ImpactingComponent.CLEAN_WATER_TANK]),
             int(component_sizes[ImpactingComponent.HOT_WATER_TANK]),
             total_solar_pv_power_produced,
-            component_sizes[RenewableEnergySource.PV],
+            {minigrid.pv_panel.name: component_sizes[RenewableEnergySource.PV]},
             optimisation.scenario,
             Simulation(end_year, start_year),
             temperature_data,
             total_loads,
             wind_speed_data,
         )
```

### Comparing `clover-energy-5.0.8/src/clover/optimisation/appraisal.py` & `clover-energy-5.1.0/src/clover/optimisation/appraisal.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     electric_yearly_load_statistics: pd.DataFrame,
     end_year: int,
     ghg_inputs: Dict[str, Any],
     heat_exchanger_addition: int,
     hot_water_tank_addition: int,
     location: Location,
     logger: Logger,
-    pv_addition: float,
+    pv_addition: Dict[str, float],
     pvt_addition: float,
     scenario: Scenario,
     simulation_results: pd.DataFrame,
     start_year: int,
     storage_addition: float,
     system_details: SystemDetails,
 ) -> EnvironmentalAppraisal:
@@ -168,15 +168,15 @@
             system_details.initial_num_buffer_tanks
             if system_details.initial_num_buffer_tanks is not None
             else 0,
             system_details.initial_num_hot_water_tanks
             if system_details.initial_num_hot_water_tanks is not None
             else 0,
             logger,
-            system_details.initial_pv_size,
+            system_details.initial_pv_sizes,
             system_details.initial_pvt_size
             if system_details.initial_pvt_size is not None
             else 0,
             system_details.initial_storage_size,
             start_year,
             end_year,
         )
@@ -253,15 +253,15 @@
     converter_addition: Dict[str, int],
     diesel_addition: float,
     finance_inputs: Dict[str, Any],
     heat_exchanger_addition: int,
     hot_water_tank_addition: int,
     location: Location,
     logger: Logger,
-    pv_addition: float,
+    pv_addition: Dict[str, float],
     pvt_addition: float,
     scenario: Scenario,
     simulation_results: pd.DataFrame,
     storage_addition: float,
     system_details: SystemDetails,
     yearly_load_statistics: pd.DataFrame,
 ) -> FinancialAppraisal:
@@ -356,15 +356,15 @@
         system_details.initial_num_buffer_tanks
         if system_details.initial_num_buffer_tanks is not None
         else 0,
         system_details.initial_num_hot_water_tanks
         if system_details.initial_num_hot_water_tanks is not None
         else 0,
         logger,
-        system_details.initial_pv_size,
+        system_details.initial_pv_sizes,
         system_details.initial_pvt_size
         if system_details.initial_pvt_size is not None
         else 0,
         system_details.initial_storage_size,
         start_year=system_details.start_year,
         end_year=system_details.end_year,
     )
@@ -670,17 +670,19 @@
     hot_water_tank_addition: int = (
         system_details.initial_num_hot_water_tanks
         - previous_system.system_details.final_num_hot_water_tanks
         if system_details.initial_num_hot_water_tanks is not None
         and previous_system.system_details.final_num_hot_water_tanks is not None
         else 0
     )
-    pv_addition = (
-        system_details.initial_pv_size - previous_system.system_details.final_pv_size
-    )
+    pv_addition: Dict[str, float] = {
+        panel_name: initial_pv_size
+        - previous_system.system_details.final_pv_sizes[panel_name]
+        for panel_name, initial_pv_size in system_details.initial_pv_sizes.items()
+    }
     pvt_addition: float = (
         system_details.initial_pvt_size - previous_system.system_details.final_pvt_size
         if system_details.initial_pvt_size is not None
         and previous_system.system_details.final_pvt_size is not None
         else 0
     )
     storage_addition = (
```

### Comparing `clover-energy-5.0.8/src/clover/optimisation/optimisation.py` & `clover-energy-5.1.0/src/clover/optimisation/optimisation.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
     conventional_cw_source_profiles: Optional[Dict[WaterSource, pd.DataFrame]],
     converters: Dict[str, Converter],
     disable_tqdm: bool,
     end_year: int,
     finance_inputs: Dict[str, Any],
     ghg_inputs: Dict[str, Any],
     grid_profile: Optional[pd.DataFrame],
-    irradiance_data: pd.Series,
+    irradiance_data: Dict[str, pd.Series],
     kerosene_usage: pd.DataFrame,
     largest_converter_sizes: Dict[Converter, ConverterSize],
     largest_cw_tank_size: TankSize,
     largest_cw_pvt_system_size: SolarSystemSize,
     largest_hw_tank_size: TankSize,
     largest_hw_pvt_system_size: SolarSystemSize,
     largest_pv_system_size: SolarSystemSize,
@@ -128,17 +128,17 @@
     location: Location,
     logger: Logger,
     minigrid: energy_system.Minigrid,
     optimisation: Optimisation,
     previous_system: Optional[SystemAppraisal],
     start_year: int,
     system_appraisals: List[SystemAppraisal],
-    temperature_data: pd.Series,
+    temperature_data: Dict[str, pd.Series],
     total_loads: Dict[ResourceType, Optional[pd.DataFrame]],
-    total_solar_pv_power_produced: pd.Series,
+    total_solar_pv_power_produced: Dict[str, pd.Series],
     wind_speed_data: Optional[pd.Series],
     yearly_electric_load_statistics: pd.DataFrame,
 ) -> Dict[Criterion, SystemAppraisal]:
     """
     Finds the optimum system from a group of sufficient systems.
 
     This function determines the optimum system from s group of sufficient systems. It
@@ -330,28 +330,28 @@
     converters: Dict[str, Converter],
     disable_tqdm: bool,
     finance_inputs: Dict[str, Any],
     ghg_inputs: Dict[str, Any],
     grid_profile: Optional[pd.DataFrame],
     hw_pvt_system_size: SolarSystemSize,
     hw_tanks: TankSize,
-    irradiance_data: pd.Series,
+    irradiance_data: Dict[str, pd.Series],
     kerosene_usage: pd.DataFrame,
     location: Location,
     logger: Logger,
     minigrid: energy_system.Minigrid,
     optimisation: Optimisation,
     optimisation_parameters: OptimisationParameters,
     previous_system: Optional[SystemAppraisal],
     pv_sizes: SolarSystemSize,
     start_year: int,
     storage_sizes: StorageSystemSize,
-    temperature_data: pd.Series,
+    temperature_data: Dict[str, pd.Series],
     total_loads: Dict[ResourceType, Optional[pd.DataFrame]],
-    total_solar_pv_power_produced: pd.Series,
+    total_solar_pv_power_produced: Dict[str, pd.Series],
     wind_speed_data: Optional[pd.Series],
     yearly_electric_load_statistics: pd.DataFrame,
 ) -> Tuple[
     int,
     Dict[Converter, ConverterSize],
     SolarSystemSize,
     TankSize,
@@ -491,15 +491,15 @@
         kerosene_usage,
         location,
         logger,
         minigrid,
         cw_tanks.max,
         hw_tanks.max,
         total_solar_pv_power_produced,
-        pv_sizes.max,
+        {minigrid.pv_panel.name: pv_sizes.max},
         optimisation.scenario,
         Simulation(end_year, start_year),
         temperature_data,
         total_loads,
         wind_speed_data,
     )
 
@@ -597,15 +597,15 @@
             kerosene_usage,
             location,
             logger,
             minigrid,
             cw_tanks_max,
             hw_tanks_max,
             total_solar_pv_power_produced,
-            pv_size_max,
+            {minigrid.pv_panel.name: pv_size_max},
             optimisation.scenario,
             Simulation(end_year, start_year),
             temperature_data,
             total_loads,
             wind_speed_data,
         )
 
@@ -965,28 +965,28 @@
     converters: Dict[str, Converter],
     disable_tqdm: bool,
     finance_inputs: Dict[str, Any],
     ghg_inputs: Dict[str, Any],
     grid_profile: Optional[pd.DataFrame],
     hw_pvt_system_size: SolarSystemSize,
     hw_tanks: TankSize,
-    irradiance_data: pd.Series,
+    irradiance_data: Dict[str, pd.Series],
     kerosene_usage: pd.DataFrame,
     location: Location,
     logger: Logger,
     minigrid: energy_system.Minigrid,
     optimisation: Optimisation,
     optimisation_parameters: OptimisationParameters,
     previous_system: Optional[SystemAppraisal],
     pv_sizes: SolarSystemSize,
     start_year: int,
     storage_sizes: StorageSystemSize,
-    temperature_data: pd.Series,
+    temperature_data: Dict[str, pd.Series],
     total_loads: Dict[ResourceType, Optional[pd.DataFrame]],
-    total_solar_pv_power_produced: pd.Series,
+    total_solar_pv_power_produced: Dict[str, pd.Series],
     wind_speed_data: Optional[pd.Series],
     yearly_electric_load_statistics: pd.DataFrame,
 ) -> SystemAppraisal:
     """
     One optimisation step of the continuous lifetime optimisation
 
     Inputs:
@@ -1138,24 +1138,24 @@
 def multiple_optimisation_step(  # pylint: disable=too-many-locals, too-many-statements
     conventional_cw_source_profiles: Optional[Dict[WaterSource, pd.DataFrame]],
     converters: Dict[str, Converter],
     disable_tqdm: bool,
     finance_inputs: Dict[str, Any],
     ghg_inputs: Dict[str, Any],
     grid_profile: Optional[pd.DataFrame],
-    irradiance_data: pd.Series,
+    irradiance_data: Dict[str, pd.Series],
     kerosene_usage: pd.DataFrame,
     location: Location,
     logger: Logger,
     minigrid: energy_system.Minigrid,
     optimisation: Optimisation,
     optimisation_parameters: OptimisationParameters,
-    temperature_data: pd.Series,
+    temperature_data: Dict[str, pd.Series],
     total_loads: Dict[ResourceType, Optional[pd.DataFrame]],
-    total_solar_pv_power_produced: pd.Series,
+    total_solar_pv_power_produced: Dict[str, pd.Series],
     wind_speed_data: Optional[pd.Series],
     yearly_electric_load_statistics: pd.DataFrame,
     *,
     input_converter_sizes: Optional[Dict[Converter, ConverterSize]] = None,
     input_cw_pvt_system_size: Optional[SolarSystemSize] = None,
     input_cw_tanks: Optional[TankSize] = None,
     input_hw_pvt_system_size: Optional[SolarSystemSize] = None,
```

### Comparing `clover-energy-5.0.8/src/clover/optimisation/single_line_simulation.py` & `clover-energy-5.1.0/src/clover/optimisation/single_line_simulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,28 +65,28 @@
     disable_tqdm: bool,
     end_year: int,
     finance_inputs: Dict[str, Any],
     ghg_inputs: Dict[str, Any],
     grid_profile: Optional[pd.DataFrame],
     hw_pvt_size: SolarSystemSize,
     hw_tanks: TankSize,
-    irradiance_data: pd.Series,
+    irradiance_data: Dict[str, pd.Series],
     kerosene_usage: pd.DataFrame,
     location: Location,
     logger: Logger,
     minigrid: energy_system.Minigrid,
     optimisation: Optimisation,
     potential_system: SystemAppraisal,
     previous_system: Optional[SystemAppraisal],
     pv_system_size: SolarSystemSize,
     start_year: int,
     storage_size: StorageSystemSize,
-    temperature_data: pd.Series,
+    temperature_data: Dict[str, pd.Series],
     total_loads: Dict[ResourceType, Optional[pd.DataFrame]],
-    total_solar_pv_power_produced: pd.Series,
+    total_solar_pv_power_produced: Dict[str, pd.Series],
     wind_speed_data: Optional[pd.Series],
     yearly_electric_load_statistics: pd.DataFrame,
 ) -> Tuple[
     Dict[Converter, ConverterSize],
     SolarSystemSize,
     TankSize,
     SolarSystemSize,
@@ -363,15 +363,15 @@
                 kerosene_usage,
                 location,
                 logger,
                 minigrid,
                 potential_num_clean_water_tanks,
                 potential_num_hot_water_tanks,
                 total_solar_pv_power_produced,
-                pv_system_size.max,
+                {minigrid.pv_panel.name: pv_system_size.max},
                 optimisation.scenario,
                 Simulation(end_year, start_year),
                 temperature_data,
                 total_loads,
                 wind_speed_data,
             )
```

### Comparing `clover-energy-5.0.8/src/clover/printer.py` & `clover-energy-5.1.0/src/clover/printer.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 In order to print information to the end user in an easily understandable way, CLOVER
 utilises this module which exposes functionality for easilly computing and outputting
 strings to the end user.
 
 """
 
 import argparse
-from typing import List
+from typing import Dict, List
 
 from .__utils__ import Scenario
 from .optimisation.__utils__ import OptimisationParameters
 from .simulation.__utils__ import Minigrid
 
 __all__ = ("generate_optimisation_string", "generate_simulation_string")
 
@@ -127,49 +127,54 @@
     return optimisation_string
 
 
 def generate_simulation_string(
     minigrid: Minigrid,
     overrided_default_sizes: bool,
     parsed_args: argparse.Namespace,
+    pv_system_sizes: Dict[str, float],
     scenario: Scenario,
 ) -> str:
     """
     Generate and return the simulation string.
 
     Inputs:
         - minigrid:
             The :class:`Minigrid` being considered for this run.
         - overrided_default_sizes:
             Whether the default sizes of various components have been overriden or not.
         - parsed_args:
             The parsed command-line arguments.
+        - pv_system_sizes:
+            The capacities of the PV panels to consider.
         - scenario:
             The :class:`__utils__.Scenario` currently being considered.
 
     Outputs:
         - A single `str` to display to the user when running a CLOVER simulation.
 
     """
 
     simulation_string_list: List[str] = []
 
     # Append the PV panel information if relevant.
     if scenario.pv and parsed_args.pv_system_size is not None:
-        simulation_string_list.append(
-            f"- {parsed_args.pv_system_size * minigrid.pv_panel.pv_unit} kWp of PV"
-            + (
-                (
-                    f" ({parsed_args.pv_system_size}x "
-                    + f"{minigrid.pv_panel.pv_unit} kWp panels)"
+        for pv_panel in minigrid.pv_panels:
+            simulation_string_list.append(
+                f"- {pv_system_sizes[pv_panel.name] * pv_panel.pv_unit} kWp of "
+                + f"'{pv_panel.name}' PV"
+                + (
+                    (
+                        f" ({pv_system_sizes[pv_panel.name]}x "
+                        + f"{pv_panel.pv_unit} kWp panels)"
+                    )
+                    if overrided_default_sizes
+                    else ""
                 )
-                if overrided_default_sizes
-                else ""
             )
-        )
 
     # Append the battery storage information if relevant.
     if scenario.battery and minigrid.battery is not None:
         simulation_string_list.append(
             f"- {parsed_args.storage_size * minigrid.battery.storage_unit} kWh of "
             + "storage"
             + (
@@ -182,39 +187,41 @@
             )
         )
 
     # Append the clean-water information if relevant.
     if scenario.desalination_scenario is not None:
         if (
             parsed_args.clean_water_pvt_system_size is not None
-            and minigrid.pvt_panel is not None
+            and len(minigrid.pvt_panels) >= 1
         ):
-            simulation_string_list.append(
-                f"- {parsed_args.clean_water_pvt_system_size} Clean-water PV-T panel "
-                + f"units ({minigrid.pvt_panel.pv_unit} kWp PV per unit)\n"
-            )
+            for pvt_panel in minigrid.pvt_panels:
+                simulation_string_list.append(
+                    f"- {parsed_args.clean_water_pvt_system_size} Clean-water PV-T panel "
+                    + f"units ({pvt_panel.pv_unit} kWp PV per unit)\n"
+                )
         if minigrid.clean_water_tank is not None:
             simulation_string_list.append(
                 f"- {parsed_args.num_clean_water_tanks}x "
                 + f"{minigrid.clean_water_tank.mass} litres clean-water storage"
                 + "\n"
                 if scenario.hot_water_scenario is not None
                 else ""
             )
 
     # Append the hot-water information if relevant.
     if scenario.hot_water_scenario is not None:
         if (
             parsed_args.hot_water_pvt_system_size is not None
-            and minigrid.pvt_panel is not None
+            and len(minigrid.pvt_panels) >= 1
         ):
-            simulation_string_list.append(
-                f"- {parsed_args.hot_water_pvt_system_size} Hot-water PV-T panel units "
-                + f"({minigrid.pvt_panel.pv_unit} kWp PV per unit)\n"
-            )
+            for pvt_panel in minigrid.pvt_panels:
+                simulation_string_list.append(
+                    f"- {parsed_args.hot_water_pvt_system_size} Hot-water PV-T panel units "
+                    + f"({pvt_panel.pv_unit} kWp PV per unit)\n"
+                )
         simulation_string_list.append(
             f"- {parsed_args.num_hot_water_tanks}x {minigrid.hot_water_tank.mass} "
             + "litres hot-water storage"
             if minigrid.hot_water_tank is not None
             else ""
         )
```

### Comparing `clover-energy-5.0.8/src/clover/scripts/clover.py` & `clover-energy-5.1.0/src/clover/scripts/clover.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.8/src/clover/scripts/clover_hpc_clover.py` & `clover-energy-5.1.0/src/clover/scripts/clover_hpc_clover.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.8/src/clover/scripts/clover_hpc_outbox_assembly.py` & `clover-energy-5.1.0/src/clover/scripts/clover_hpc_outbox_assembly.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.8/src/clover/scripts/clover_new_location.py` & `clover-energy-5.1.0/src/clover/scripts/clover_new_location.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.8/src/clover/scripts/clover_update_api_token.py` & `clover-energy-5.1.0/src/clover/scripts/clover_update_api_token.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.8/src/clover/scripts/hpc.py` & `clover-energy-5.1.0/src/clover/scripts/hpc.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.8/src/clover/scripts/hpc_clover.py` & `clover-energy-5.1.0/src/clover/scripts/hpc_clover.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.8/src/clover/scripts/hpc_outbox_assembly.py` & `clover-energy-5.1.0/src/clover/scripts/hpc_outbox_assembly.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.8/src/clover/scripts/hpc_utils.py` & `clover-energy-5.1.0/src/clover/scripts/hpc_utils.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.8/src/clover/scripts/new_location.py` & `clover-energy-5.1.0/src/clover/scripts/new_location.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.8/src/clover/scripts/update_api_token.py` & `clover-energy-5.1.0/src/clover/scripts/update_api_token.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.8/src/clover/simulation/__init__.py` & `clover-energy-5.1.0/src/clover/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.8/src/clover/simulation/__utils__.py` & `clover-energy-5.1.0/src/clover/simulation/__utils__.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     BColours,
     CleanWaterMode,
     EXCHANGER,
     InputFileError,
     NAME,
     RESOURCE_NAME_TO_RESOURCE_TYPE_MAPPING,
     OperatingMode,
+    ProgrammerJudgementFault,
     ResourceType,
     Scenario,
 )
 
 from ..conversion.conversion import Converter
 from ..generation.solar import HybridPVTPanel, PVPanel
 from .diesel import DieselGenerator, DieselWaterHeater
@@ -124,19 +125,19 @@
 
     .. attribute:: heat_exchanger
         The heat exchanger associated with the minigrid system.
 
     .. attribute:: hot_water_tank
         The hot-water tank being modelled, if applicable.
 
-    .. attribute:: pv_panel
-        The PV panel being considered.
+    .. attribute:: pv_panels
+        The PV panel(s) being considered.
 
-    .. attribute:: pvt_panel
-        The PV-T panel being considered, if applicable.
+    .. attribute:: pvt_panels
+        The PV-T panel(s) being considered, if applicable.
 
     .. attribute:: water_pump
         The water pump associated with the energy system, as a :class:`Transmitter`
         instance.
 
     """
 
@@ -150,27 +151,27 @@
     dc_to_dc_conversion_efficiency: Optional[float]
     dc_transmission_efficiency: Optional[float]
     diesel_generator: Optional[DieselGenerator]
     diesel_water_heater: Optional[DieselWaterHeater]
     electric_water_heater: Optional[Converter]
     heat_exchanger: Optional[Exchanger]
     hot_water_tank: Optional[HotWaterTank]
-    pv_panel: PVPanel
-    pvt_panel: Optional[HybridPVTPanel]
+    pv_panels: List[PVPanel]
+    pvt_panels: List[HybridPVTPanel]
     water_pump: Optional[Transmitter]
 
     @classmethod
     def from_dict(  # pylint: disable=too-many-locals
         cls,
         diesel_generator: DieselGenerator,
         diesel_water_heater: Optional[DieselWaterHeater],
         electric_water_heater: Optional[Converter],
         minigrid_inputs: Dict[str, Any],
-        pv_panel: PVPanel,
-        pvt_panel: Optional[HybridPVTPanel],
+        pv_panels: List[PVPanel],
+        pvt_panels: List[HybridPVTPanel],
         battery_inputs: Optional[List[Dict[str, Any]]] = None,
         exchanger_inputs: Optional[List[Dict[str, Any]]] = None,
         tank_inputs: Optional[List[Dict[str, Any]]] = None,
         water_pump: Optional[Transmitter] = None,
     ) -> Any:
         """
         Returns a :class:`Minigrid` instance based on the inputs provided.
@@ -183,18 +184,19 @@
                 appropriate.
             - electric_water_heater:
                 The electric water heater associated with the minigrid system, if
                 appropriate.
             - minigrid_inputs:
                 The inputs for the minigrid/energy system, extracted from the input
                 file.
-            - pv_panel:
-                The :class:`PVPanel` instance to use for the run.
-            - pvt_panel:
-                The :class:`HybridPVTPanel` instance to use for the run, if appropriate.
+            - pv_panels:
+                The `list` of :class:`PVPanel` instances to use for the run.
+            - pvt_panels:
+                The `list` of :class:`HybridPVTPanel` instances to use for the run,
+                if appropriate.
             - battery_inputs:
                 The battery input information.
             - exchanger_inputs:
                 The heat-exchanger input information.
             - tank_inputs:
                 The tank input information.
             - water_pump:
@@ -322,19 +324,69 @@
             diesel_generator,
             diesel_water_heater,
             electric_water_heater,
             exchangers[minigrid_inputs[EXCHANGER]]
             if EXCHANGER in minigrid_inputs
             else None,
             hot_water_tank,
-            pv_panel,
-            pvt_panel,
+            pv_panels,
+            pvt_panels,
             water_pump,
         )
 
+    @property
+    def pv_panel(self) -> PVPanel:
+        """
+        Returns a PV panel if there is only one panel being modelled, otherwise errors.
+
+        Outputs:
+            - pv_panel:
+                The :class:`PVPanel` being modelled, if only one is present.
+
+        Raises:
+            - ProgrammerJudgementFault
+                Raised if this is called when multiple panels are present.
+
+        """
+
+        if len(self.pv_panels) > 1:
+            raise ProgrammerJudgementFault(
+                "Minigrid.pv_panel",
+                "Cannot use `pv_panel` when multiple panels present.",
+            )
+
+        return self.pv_panels[0]
+
+    @property
+    def pvt_panel(self) -> Optional[HybridPVTPanel]:
+        """
+        Returns a PV-T panel if there is only one panel modelled, otherwise errors.
+
+        Outputs:
+            - pvt_panel:
+                The :class:`PVTPanel` being modelled, if only one is present. If PV-T
+                panels are not present in the system, `None` is returned.
+
+        Raises:
+            - ProgrammerJudgementFault
+                Raised if this is called when multiple panels are present.
+
+        """
+
+        if self.pvt_panels is None or len(self.pvt_panels) == 0:
+            return None
+
+        if len(self.pvt_panels) > 1:
+            raise ProgrammerJudgementFault(
+                "Minigrid.pvt_panel",
+                "Cannot use `pvt_panel` when multiple panels present.",
+            )
+
+        return self.pvt_panels[0]
+
 
 def check_scenario(
     logger: Logger,
     minigrid: Minigrid,
     operating_mode: OperatingMode,
     parsed_args: Namespace,
     scenario: Scenario,
```

### Comparing `clover-energy-5.0.8/src/clover/simulation/diesel.py` & `clover-energy-5.1.0/src/clover/simulation/diesel.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.8/src/clover/simulation/energy_system.py` & `clover-energy-5.1.0/src/clover/simulation/energy_system.py`

 * *Files 2% similar despite different names*

```diff
@@ -240,22 +240,22 @@
     return electric_desalinators, energy_per_desalinated_litre, maximum_water_throughput
 
 
 def _calculate_renewable_cw_profiles(  # pylint: disable=too-many-locals, too-many-statements
     converters: List[Converter],
     disable_tqdm: bool,
     end_hour: int,
-    irradiance_data: pd.Series,
+    irradiance_data: Dict[str, pd.Series],
     logger: Logger,
     minigrid: Minigrid,
     number_of_cw_tanks: int,
     pvt_size: int,
     scenario: Scenario,
     start_hour: int,
-    temperature_data: pd.Series,
+    temperature_data: Dict[str, pd.Series],
     wind_speed_data: Optional[pd.Series],
 ) -> Tuple[
     Optional[pd.DataFrame],
     pd.DataFrame,
     List[Converter],
     Optional[pd.DataFrame],
     pd.DataFrame,
@@ -478,24 +478,24 @@
             clean_water_pvt_electric_power_per_unit,
             clean_water_pvt_pump_times,
             buffer_tank_temperature,
             buffer_tank_volume_supplied,
         ) = calculate_pvt_output(
             disable_tqdm,
             end_hour,
-            irradiance_data[start_hour:end_hour],
+            irradiance_data[minigrid.pvt_panel.name][start_hour:end_hour],  # type: ignore
             logger,
             minigrid,
             number_of_cw_tanks,
             None,
             pvt_size,
             ResourceType.CLEAN_WATER,
             scenario,
             start_hour,
-            temperature_data[start_hour:end_hour],
+            temperature_data[minigrid.pvt_panel.name][start_hour:end_hour],  # type: ignore
             thermal_desalination_plant,
             wind_speed_data[start_hour:end_hour],
         )
         logger.info("PV-T performance successfully computed.")
 
         # Compute the clean water supplied by the desalination unit.
         renewable_cw_produced: pd.DataFrame = (
@@ -561,23 +561,23 @@
     )
 
 
 def _calculate_renewable_hw_profiles(  # pylint: disable=too-many-locals, too-many-statements
     converters: List[Converter],
     disable_tqdm: bool,
     end_hour: int,
-    irradiance_data: pd.Series,
+    irradiance_data: Dict[str, pd.Series],
     logger: Logger,
     minigrid: Minigrid,
     number_of_hw_tanks: int,
     processed_total_hw_load: pd.DataFrame,
     pvt_size: int,
     scenario: Scenario,
     start_hour: int,
-    temperature_data: pd.Series,
+    temperature_data: Dict[str, pd.Series],
     wind_speed_data: Optional[pd.Series],
 ) -> Tuple[
     Optional[Union[Converter, DieselWaterHeater]],
     pd.DataFrame,
     Optional[pd.DataFrame],
     pd.DataFrame,
     Optional[pd.DataFrame],
@@ -754,24 +754,24 @@
             hot_water_pvt_electric_power_per_unit,
             hot_water_pvt_pump_times,
             hot_water_tank_temperature,
             hot_water_tank_volume_supplied,
         ) = calculate_pvt_output(
             disable_tqdm,
             end_hour,
-            irradiance_data[start_hour:end_hour],
+            irradiance_data[minigrid.pvt_panel.name][start_hour:end_hour],  # type: ignore
             logger,
             minigrid,
             number_of_hw_tanks,
             processed_total_hw_load.iloc[:, 0],
             pvt_size,
             ResourceType.HOT_CLEAN_WATER,
             scenario,
             start_hour,
-            temperature_data[start_hour:end_hour],
+            temperature_data[minigrid.pvt_panel.name][start_hour:end_hour],  # type: ignore
             None,
             wind_speed_data[start_hour:end_hour],
         )
         logger.info("Hot-water PV-T performance successfully computed.")
 
         # Compute the heat consumed by the auxiliary heater.
         # auxiliary_heater_heat_consumption: pd.DataFrame = pd.DataFrame(
@@ -1059,26 +1059,26 @@
     clean_water_pvt_size: int,
     conventional_cw_source_profiles: Optional[Dict[WaterSource, pd.DataFrame]],
     converters: Union[Dict[str, Converter], List[Converter]],
     disable_tqdm: bool,
     electric_storage_size: float,
     grid_profile: Optional[pd.DataFrame],
     hot_water_pvt_size: int,
-    irradiance_data: pd.Series,
+    irradiance_data: Dict[str, pd.Series],
     kerosene_usage: pd.DataFrame,
     location: Location,
     logger: Logger,
     minigrid: Minigrid,
     number_of_cw_tanks: int,
     number_of_hw_tanks: int,
-    pv_power_produced: pd.Series,
-    pv_size: float,
+    pv_power_produced: Dict[str, pd.Series],
+    pv_sizes: Optional[Dict[str, float]],
     scenario: Scenario,
     simulation: Simulation,
-    temperature_data: pd.Series,
+    temperature_data: Dict[str, pd.Series],
     total_loads: Dict[ResourceType, Optional[pd.DataFrame]],
     wind_speed_data: Optional[pd.Series],
 ) -> Tuple[datetime.timedelta, pd.DataFrame, SystemDetails]:
     """
     Simulates a minigrid system
 
     This function simulates the energy system of a given capacity and to the parameters
@@ -1097,39 +1097,40 @@
         - electric_storage_size:
             Amount of storage in terms of the number of batteries included.
         - grid_profile:
             The grid-availability profile.
         - hot_water_pvt_size:
             Amount of PV-T in PV-T units associated with the hot-water system.
         - irradiance_data:
-            The total solar irradiance data.
+            The total solar irradiance data incident on each panel.
         - kerosene_usage:
             The kerosene-usage profile.
         - location:
             The location being considered.
         - logger:
             The :class:`logging.Logger` to use for the run.
         - minigrid:
             The energy system being considered.
         - number_of_cw_tanks:
             The number of clean-water tanks installed in the system.
         - number_of_hw_tanks:
             The number of hot-water tanks installed in the system.
-        - pv_size:
-            Amount of PV in PV units.
+        - pv_sizes:
+            Amount of PV in PV units for each of the pv panels being considered.
         - pv_power_produced:
-            The total energy outputted by the solar system per PV unit.
+            The total energy outputted by the solar system per PV unit for each of the
+            pv panels being considered
         - renewable_cw_produced:
             The amount of clean-water produced renewably, mesaured in litres.
         - scenario:
             The scenario being considered.
         - simulation:
             The simulation to run.
         - temperature_data:
-            The temperature data series.
+            The temperature data series for each of the pv panels being considered
         - total_loads:
             A mapping between :class:`ResourceType`s and their associated total loads
             placed on the system.
         - wind_speed_data:
             The wind-speed data series.
 
     Outputs:
@@ -1413,43 +1414,46 @@
 
     # Compute the electric input profiles.
     battery_storage_profile: pd.DataFrame
     grid_energy: pd.DataFrame
     kerosene_profile: pd.Series
     load_energy: pd.DataFrame
     renewables_energy: pd.DataFrame
-    renewables_energy_map: Dict[RenewableEnergySource, pd.DataFrame] = {
-        RenewableEnergySource.PV: pv_power_produced,  # type: ignore
+    renewables_energy_by_source: Dict[RenewableEnergySource, pd.DataFrame]
+    renewables_energy_map: Dict[
+        RenewableEnergySource, Union[pd.DataFrame, Dict[str, pd.Series]]
+    ] = {
+        RenewableEnergySource.PV: pv_power_produced,
         RenewableEnergySource.CLEAN_WATER_PVT: (
             clean_water_pvt_electric_power_per_unit
         ),
         RenewableEnergySource.HOT_WATER_PVT: hot_water_pvt_electric_power_per_unit,
     }
     renewables_energy_used_directly: pd.DataFrame
     (
         battery_storage_profile,
         grid_energy,
         kerosene_profile,
         load_energy,
         renewables_energy,
-        renewables_energy_map,
+        renewables_energy_by_source,
         renewables_energy_used_directly,
     ) = get_electric_battery_storage_profile(
         clean_water_pvt_size=clean_water_pvt_size,
         grid_profile=grid_profile.iloc[start_hour:end_hour, 0],  # type: ignore
         hot_water_pvt_size=hot_water_pvt_size,
         kerosene_usage=kerosene_usage.iloc[start_hour:end_hour, 0],
         location=location,
         logger=logger,
         minigrid=minigrid,
         processed_total_electric_load=processed_total_electric_load,
         renewables_power_produced=renewables_energy_map,
         scenario=scenario,
         end_hour=end_hour,
-        pv_size=pv_size,
+        pv_sizes=pv_sizes,
         start_hour=start_hour,
     )
 
     if all(renewables_energy.values == 0):
         logger.warning(
             "%sNo renewable electricity was generated. Continuing with grid and diesel "
             "only.%s",
@@ -2014,20 +2018,23 @@
             ]
         )
         if minigrid.pvt_panel is not None and scenario.hot_water_scenario is not None
         else None,
         number_of_buffer_tanks if scenario.desalination_scenario is not None else None,
         number_of_cw_tanks if scenario.desalination_scenario is not None else None,
         number_of_hw_tanks if scenario.hot_water_scenario is not None else None,
-        pv_size
-        * float(
-            solar_degradation(minigrid.pv_panel.lifetime, location.max_years).iloc[
-                HOURS_PER_YEAR * (simulation.end_year - simulation.start_year), 0
-            ]
-        ),
+        {
+            pv_panel.name: (pv_sizes[pv_panel.name] if pv_sizes is not None else 0)
+            * float(
+                solar_degradation(pv_panel.lifetime, location.max_years).iloc[
+                    HOURS_PER_YEAR * (simulation.end_year - simulation.start_year), 0
+                ]
+            )
+            for pv_panel in minigrid.pv_panels
+        },
         float(
             electric_storage_size
             * minigrid.battery.storage_unit
             * np.min(battery_health_frame[ColumnHeader.BATTERY_HEALTH.value])
         ),
         {
             converter.name: available_converters.count(converter)
@@ -2038,28 +2045,32 @@
         else None,
         hot_water_pvt_size
         if minigrid.pvt_panel is not None and scenario.hot_water_scenario is not None
         else None,
         number_of_buffer_tanks if scenario.desalination_scenario is not None else None,
         number_of_cw_tanks if scenario.desalination_scenario is not None else None,
         number_of_hw_tanks if scenario.hot_water_scenario is not None else None,
-        pv_size,
+        pv_sizes
+        if pv_sizes is not None
+        else {pv_panel.name: 0 for pv_panel in minigrid.pv_panels},
         float(electric_storage_size * minigrid.battery.storage_unit),
         [source.name for source in required_cw_feedwater_sources]
         if len(required_cw_feedwater_sources) > 0
         else None,
         simulation.start_year,
     )
 
     # Separate out the various renewable inputs.
-    pv_energy = renewables_energy_map[RenewableEnergySource.PV]
-    clean_water_pvt_energy = renewables_energy_map[
+    pv_energy = renewables_energy_by_source[RenewableEnergySource.PV]
+    clean_water_pvt_energy = renewables_energy_by_source[
         RenewableEnergySource.CLEAN_WATER_PVT
     ]
-    hot_water_pvt_energy = renewables_energy_map[RenewableEnergySource.HOT_WATER_PVT]
+    hot_water_pvt_energy = renewables_energy_by_source[
+        RenewableEnergySource.HOT_WATER_PVT
+    ]
     total_pvt_energy = pd.DataFrame(
         clean_water_pvt_energy.values + hot_water_pvt_energy.values
     )
     total_pvt_energy.columns = pd.Index(
         [ColumnHeader.TOTAL_PVT_ELECTRICITY_SUPPLIED.value]
     )
 
@@ -2218,15 +2229,15 @@
 #         lifetime_output = pd.DataFrame([])
 #         simulation_periods = np.size(optimisation_report, 0)
 #         # Iterate over all simulation periods
 #         for sim in range(simulation_periods):
 #             system_performance_outputs = self.simulation(
 #                 start_year=int(optimisation_report["Start year"][sim]),
 #                 end_year=int(optimisation_report["End year"][sim]),
-#                 pv_size=float(optimisation_report["Initial PV size"][sim]),
+#                 pv_sizes=float(optimisation_report["Initial PV size"][sim]),
 #                 electric_storage_size=float(
 #                     optimisation_report["Initial storage size"][sim]
 #                 ),
 #             )
 #             lifetime_output = pd.concat(
 #                 [lifetime_output, system_performance_outputs[0]], axis=0
 #             )
```

### Comparing `clover-energy-5.0.8/src/clover/simulation/exchanger.py` & `clover-energy-5.1.0/src/clover/simulation/exchanger.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.8/src/clover/simulation/solar.py` & `clover-energy-5.1.0/src/clover/simulation/solar.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.8/src/clover/simulation/storage.py` & `clover-energy-5.1.0/src/clover/simulation/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 CLOVER considers several storage media for various forms of energy. The various
 calculations associated with these storage media are carried out in this module.
 
 """
 
 from logging import Logger
-from typing import Dict, Optional, Tuple
+from typing import Dict, Optional, Tuple, Union
 
 import pandas as pd
 import numpy as np
 
 from ..__utils__ import (
     BColours,
     CleanWaterMode,
@@ -367,20 +367,22 @@
     *,
     grid_profile: pd.Series,
     kerosene_usage: pd.Series,
     location: Location,
     logger: Logger,
     minigrid: Minigrid,
     processed_total_electric_load: pd.DataFrame,
-    renewables_power_produced: Dict[RenewableEnergySource, pd.DataFrame],
+    pv_sizes: Optional[Dict[str, float]] = None,
+    renewables_power_produced: Dict[
+        RenewableEnergySource, Union[pd.DataFrame, Dict[str, pd.Series]]
+    ],
     scenario: Scenario,
     clean_water_pvt_size: int = 0,
     end_hour: int = 4,
     hot_water_pvt_size: int = 0,
-    pv_size: float = 10,
     start_hour: int = 0,
 ) -> Tuple[
     pd.DataFrame,
     pd.DataFrame,
     pd.Series,
     pd.DataFrame,
     pd.DataFrame,
@@ -409,15 +411,15 @@
             The scenatio being considered.
         - clean_water_pvt_size:
             Amount of PV-T in units of PV-T associated with the clean-water system.
         - end_year:
             End year of this simulation period.
         - hot_water_pvt_size:
             Amount of PV-T in units of PV-T associated with the hot-water system.
-        - pv_size:
+        - pv_sizes:
             Amount of PV in units of PV.
         - start_year:
             Start year of this simulation period.
 
     Outputs:
         - battery_storage_profile:
             Amount of energy (kWh) into (+ve) and out of (-ve) the battery.
@@ -437,34 +439,49 @@
             A mapping between :class:`RenewableEnergySource` and the associated
             electrical energy produced.
         - renewables_energy_used_directly:
             Amount of energy (kWh) from renewables used directly to satisfy load (kWh).
 
     """
 
-    # Initialise power generation, including degradation of PV
-    try:
-        pv_power_produced = renewables_power_produced[RenewableEnergySource.PV]
-    except KeyError:
-        logger.critical(
-            "%sCould not determine PV power produced from renewables production.%s",
-            BColours.fail,
-            BColours.endc,
-        )
-        raise InternalError(
-            "No PV power in renewables_power_produced mapping, fatal."
-        ) from None
-    pv_generation_array = pv_power_produced * pv_size
-    solar_degradation_array = solar_degradation(
-        minigrid.pv_panel.lifetime, location.max_years
-    ).iloc[start_hour:end_hour, 0]
-    pv_generation = pd.DataFrame(
-        np.asarray(pv_generation_array.iloc[start_hour:end_hour])
-        * np.asarray(solar_degradation_array)
-    )
+    # Determine the PV power from the panels installed.
+    pv_generation: pd.DataFrame = pd.DataFrame([0] * (end_hour - start_hour))
+
+    if pv_sizes is not None:
+        # Attempt to determine the power produced by PV panels installed.
+        try:
+            pv_power_produced = renewables_power_produced[RenewableEnergySource.PV]
+        except KeyError:
+            logger.critical(
+                "%sCould not determine PV power produced from renewables production.%s",
+                BColours.fail,
+                BColours.endc,
+            )
+            raise InternalError(
+                "No PV power in renewables_power_produced mapping, fatal."
+            ) from None
+
+        # Cycle through the panels and append their performances.
+        for pv_panel in minigrid.pv_panels:
+            # Initialise power generation, including degradation of PV, for each PV panel being
+            # considered.
+            pv_generation_array = (
+                pv_power_produced[pv_panel.name] * pv_sizes[pv_panel.name]
+            )
+            solar_degradation_array = solar_degradation(
+                pv_panel.lifetime, location.max_years
+            ).iloc[start_hour:end_hour, 0]
+            pv_generation_frame = pd.DataFrame(
+                np.asarray(pv_generation_array.iloc[start_hour:end_hour])
+                * np.asarray(solar_degradation_array)
+            )
+            if pv_generation is None:
+                pv_generation = pv_generation_frame
+            else:
+                pv_generation += pv_generation_frame
 
     # Initialise PV-T power generation, including degradation of PV
     if minigrid.pvt_panel is not None:
         # Determine the PV-T degredation.
         pvt_degradation_array = solar_degradation(  # type: ignore
             minigrid.pvt_panel.lifetime, location.max_years
         )[0 : (end_hour - start_hour)]
@@ -483,17 +500,17 @@
                 "No PV-T electric power produced despite a PV-T panel being defined "
                 "for the system.."
             )
 
         # Compute the clean-water PV-T electricity generated.
         if RenewableEnergySource.CLEAN_WATER_PVT in renewables_power_produced:
             try:
-                clean_water_pvt_electric_power_produced = renewables_power_produced[
-                    RenewableEnergySource.CLEAN_WATER_PVT
-                ]
+                clean_water_pvt_electric_power_produced: pd.DataFrame = pd.DataFrame(
+                    renewables_power_produced[RenewableEnergySource.CLEAN_WATER_PVT]
+                )
             except KeyError:
                 logger.error(
                     "%sCould not determine clean-water PV-T power produced from "
                     "renewables production despite a PV-T panel being defined on the "
                     "system.%s",
                     BColours.fail,
                     BColours.endc,
@@ -513,17 +530,17 @@
             clean_water_pvt_electric_generation = pd.DataFrame(
                 [0] * (end_hour - start_hour)
             )
 
         # Compute the clean-water source.
         if RenewableEnergySource.HOT_WATER_PVT in renewables_power_produced:
             try:
-                hot_water_pvt_electric_power_produced = renewables_power_produced[
-                    RenewableEnergySource.HOT_WATER_PVT
-                ]
+                hot_water_pvt_electric_power_produced: pd.DataFrame = pd.DataFrame(
+                    renewables_power_produced[RenewableEnergySource.HOT_WATER_PVT]
+                )
             except KeyError:
                 logger.error(
                     "%sCould not determine PV-T power produced from renewables "
                     "production despite a PV-T panel being defined on the system.%s",
                     BColours.fail,
                     BColours.endc,
                 )
@@ -547,27 +564,31 @@
         clean_water_pvt_electric_generation = pd.DataFrame(
             [0] * (end_hour - start_hour)
         )
         hot_water_pvt_electric_generation = pd.DataFrame([0] * (end_hour - start_hour))
 
     # Consider power distribution network
     if scenario.distribution_network == DistributionNetwork.DC:
-        pv_generation = pv_generation.mul(  # type: ignore
-            minigrid.dc_to_dc_conversion_efficiency
-        )
+        generation_efficiency = minigrid.dc_to_dc_conversion_efficiency
         transmission_efficiency = minigrid.dc_transmission_efficiency
         # grid_conversion_eff = minigrid.ac_to_dc_conversion
 
     else:
-        pv_generation = pv_generation.mul(  # type: ignore
-            minigrid.dc_to_ac_conversion_efficiency
-        )
+        generation_efficiency = minigrid.dc_to_ac_conversion_efficiency
         transmission_efficiency = minigrid.ac_transmission_efficiency
         # grid_conversion_efficiency = minigrid.ac_to_ac_conversion
 
+    pv_generation = pv_generation.mul(generation_efficiency)  # type: ignore
+    clean_water_pvt_electric_generation = clean_water_pvt_electric_generation.mul(  # type: ignore
+        generation_efficiency
+    )
+    hot_water_pvt_electric_generation = clean_water_pvt_electric_generation.mul(  # type: ignore
+        generation_efficiency
+    )
+
     if transmission_efficiency is None:
         logger.error(
             "%sNo valid transmission efficiency was determined based on the energy "
             "system inputs. Check this before continuing.%s",
             BColours.fail,
             BColours.endc,
         )
```

### Comparing `clover-energy-5.0.8/src/clover/simulation/storage_utils.py` & `clover-energy-5.1.0/src/clover/simulation/storage_utils.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.8/src/clover/simulation/transmission.py` & `clover-energy-5.1.0/src/clover/simulation/transmission.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.8/src/clover/src/new_location.yaml` & `clover-energy-5.1.0/src/clover/src/new_location.yaml`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.8/src/clover_energy.egg-info/PKG-INFO` & `clover-energy-5.1.0/src/clover_energy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clover-energy
-Version: 5.0.8
+Version: 5.1.0
 Summary: Continuous Lifetime Optimisation of Variable Electricity Resources
 Home-page: https://github.com/CLOVER-energy/CLOVER
 Author: Phil Sandwell, Ben Winchester and Hamish Beath
 Author-email: philip.sandwell@gmail.com,benedict.winchester@gmail.com,hamishbeath@outlook.com
 Project-URL: Bug Tracker, https://github.com/CLOVER-energy/CLOVER/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `clover-energy-5.0.8/src/clover_energy.egg-info/SOURCES.txt` & `clover-energy-5.1.0/src/clover_energy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

