# Comparing `tmp/sigopt-8.8.1.tar.gz` & `tmp/sigopt-8.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigopt-8.8.1.tar", last modified: Mon Jul 17 18:17:28 2023, max compression
+gzip compressed data, was "sigopt-8.8.2.tar", last modified: Mon Jul 17 20:41:28 2023, max compression
```

## Comparing `sigopt-8.8.1.tar` & `sigopt-8.8.2.tar`

### file list

```diff
@@ -1,361 +1,361 @@
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.979595 sigopt-8.8.1/
--rw-r--r--   0 tjackles   (503) staff       (20)     1083 2022-02-18 18:21:31.000000 sigopt-8.8.1/LICENSE
--rw-r--r--   0 tjackles   (503) staff       (20)      109 2021-10-21 13:30:45.000000 sigopt-8.8.1/MANIFEST.in
--rw-r--r--   0 tjackles   (503) staff       (20)      617 2023-07-17 18:17:28.979870 sigopt-8.8.1/PKG-INFO
--rw-r--r--   0 tjackles   (503) staff       (20)     4491 2023-07-17 17:31:25.000000 sigopt-8.8.1/README.md
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.840422 sigopt-8.8.1/integration_test/
--rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/integration_test/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)     1405 2023-04-03 19:26:20.000000 sigopt-8.8.1/integration_test/test_experiment.py
--rw-r--r--   0 tjackles   (503) staff       (20)     4110 2023-06-27 22:27:24.000000 sigopt-8.8.1/integration_test/test_hyperopt.py
--rw-r--r--   0 tjackles   (503) staff       (20)      723 2023-04-03 19:26:20.000000 sigopt-8.8.1/integration_test/test_sigopt.py
--rw-r--r--   0 tjackles   (503) staff       (20)     6745 2023-04-03 19:26:20.000000 sigopt-8.8.1/integration_test/test_xgboost_experiment.py
--rw-r--r--   0 tjackles   (503) staff       (20)    15097 2023-04-03 19:26:20.000000 sigopt-8.8.1/integration_test/test_xgboost_run.py
--rw-r--r--   0 tjackles   (503) staff       (20)       56 2023-04-03 19:26:20.000000 sigopt-8.8.1/pyproject.toml
--rw-r--r--   0 tjackles   (503) staff       (20)      391 2023-07-17 18:17:28.980538 sigopt-8.8.1/setup.cfg
--rw-r--r--   0 tjackles   (503) staff       (20)     2728 2023-04-27 20:20:23.000000 sigopt-8.8.1/setup.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.853043 sigopt-8.8.1/sigopt/
--rw-r--r--   0 tjackles   (503) staff       (20)     2135 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)     2907 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/aiexperiment_context.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.858605 sigopt-8.8.1/sigopt/cli/
--rw-r--r--   0 tjackles   (503) staff       (20)      121 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/cli/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)      148 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/cli/__main__.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.868368 sigopt-8.8.1/sigopt/cli/arguments/
--rw-r--r--   0 tjackles   (503) staff       (20)      686 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/arguments/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)      396 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/arguments/cluster_filename.py
--rw-r--r--   0 tjackles   (503) staff       (20)      188 2023-04-03 17:57:25.000000 sigopt-8.8.1/sigopt/cli/arguments/cluster_name.py
--rw-r--r--   0 tjackles   (503) staff       (20)      167 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/arguments/commands.py
--rw-r--r--   0 tjackles   (503) staff       (20)      206 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/cli/arguments/dockerfile.py
--rw-r--r--   0 tjackles   (503) staff       (20)      432 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/arguments/experiment_file.py
--rw-r--r--   0 tjackles   (503) staff       (20)      200 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/arguments/experiment_id.py
--rw-r--r--   0 tjackles   (503) staff       (20)      570 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/arguments/identifiers.py
--rw-r--r--   0 tjackles   (503) staff       (20)     1121 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/arguments/load_yaml.py
--rw-r--r--   0 tjackles   (503) staff       (20)     1157 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/arguments/project.py
--rw-r--r--   0 tjackles   (503) staff       (20)      344 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/cli/arguments/provider.py
--rw-r--r--   0 tjackles   (503) staff       (20)      443 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/arguments/run_file.py
--rw-r--r--   0 tjackles   (503) staff       (20)      478 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/arguments/source_file.py
--rw-r--r--   0 tjackles   (503) staff       (20)      319 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/arguments/validate.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.871141 sigopt-8.8.1/sigopt/cli/commands/
--rw-r--r--   0 tjackles   (503) staff       (20)      383 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)      510 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/base.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.878359 sigopt-8.8.1/sigopt/cli/commands/cluster/
--rw-r--r--   0 tjackles   (503) staff       (20)      862 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/cli/commands/cluster/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)      531 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/cluster/base.py
--rw-r--r--   0 tjackles   (503) staff       (20)      263 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/cluster/clean.py
--rw-r--r--   0 tjackles   (503) staff       (20)     1053 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/cluster/connect.py
--rw-r--r--   0 tjackles   (503) staff       (20)      569 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/cluster/create.py
--rw-r--r--   0 tjackles   (503) staff       (20)      285 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/cluster/destroy.py
--rw-r--r--   0 tjackles   (503) staff       (20)      304 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/cluster/disconnect.py
--rw-r--r--   0 tjackles   (503) staff       (20)      302 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/cluster/install_plugins.py
--rw-r--r--   0 tjackles   (503) staff       (20)      521 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/cluster/kubectl.py
--rw-r--r--   0 tjackles   (503) staff       (20)      485 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/cluster/not_installed.py
--rw-r--r--   0 tjackles   (503) staff       (20)      777 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/cluster/optimize.py
--rw-r--r--   0 tjackles   (503) staff       (20)      690 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/cluster/run.py
--rw-r--r--   0 tjackles   (503) staff       (20)      622 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/cluster/status.py
--rw-r--r--   0 tjackles   (503) staff       (20)      511 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/cluster/stop.py
--rw-r--r--   0 tjackles   (503) staff       (20)      295 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/cluster/test.py
--rw-r--r--   0 tjackles   (503) staff       (20)      706 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/cluster/test_run.py
--rw-r--r--   0 tjackles   (503) staff       (20)      369 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/cluster/update.py
--rw-r--r--   0 tjackles   (503) staff       (20)     1282 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/config.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.879859 sigopt-8.8.1/sigopt/cli/commands/experiment/
--rw-r--r--   0 tjackles   (503) staff       (20)      210 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/experiment/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)      688 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/experiment/archive.py
--rw-r--r--   0 tjackles   (503) staff       (20)      952 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/experiment/create.py
--rw-r--r--   0 tjackles   (503) staff       (20)      687 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/experiment/unarchive.py
--rw-r--r--   0 tjackles   (503) staff       (20)      986 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/init.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.881480 sigopt-8.8.1/sigopt/cli/commands/local/
--rw-r--r--   0 tjackles   (503) staff       (20)      196 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/cli/commands/local/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)      810 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/local/optimize.py
--rw-r--r--   0 tjackles   (503) staff       (20)      756 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/local/run.py
--rw-r--r--   0 tjackles   (503) staff       (20)      912 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/local/start_worker.py
--rw-r--r--   0 tjackles   (503) staff       (20)      244 2023-04-03 19:57:41.000000 sigopt-8.8.1/sigopt/cli/commands/optimize_base.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.882262 sigopt-8.8.1/sigopt/cli/commands/project/
--rw-r--r--   0 tjackles   (503) staff       (20)      113 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/cli/commands/project/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)      850 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/project/create.py
--rw-r--r--   0 tjackles   (503) staff       (20)      738 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/run_base.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.883428 sigopt-8.8.1/sigopt/cli/commands/training_run/
--rw-r--r--   0 tjackles   (503) staff       (20)      169 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/cli/commands/training_run/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)      605 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/training_run/archive.py
--rw-r--r--   0 tjackles   (503) staff       (20)      615 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/training_run/unarchive.py
--rw-r--r--   0 tjackles   (503) staff       (20)      235 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/version.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.885448 sigopt-8.8.1/sigopt/cli/resources/
--rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/cli/resources/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)      668 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/cli/resources/init_dockerfile.txt
--rw-r--r--   0 tjackles   (503) staff       (20)       34 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/cli/resources/init_dockerignore.txt
--rw-r--r--   0 tjackles   (503) staff       (20)      208 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/cli/resources/init_experiment.txt
--rw-r--r--   0 tjackles   (503) staff       (20)       83 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/cli/resources/init_run.txt
--rw-r--r--   0 tjackles   (503) staff       (20)     4897 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/utils.py
--rw-r--r--   0 tjackles   (503) staff       (20)      355 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/compat.py
--rw-r--r--   0 tjackles   (503) staff       (20)     3231 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/config.py
--rw-r--r--   0 tjackles   (503) staff       (20)     1867 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/defaults.py
--rw-r--r--   0 tjackles   (503) staff       (20)     1137 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/endpoint.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.886235 sigopt-8.8.1/sigopt/examples/
--rw-r--r--   0 tjackles   (503) staff       (20)       93 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/examples/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)      874 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/examples/franke.py
--rw-r--r--   0 tjackles   (503) staff       (20)     2117 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/exception.py
--rw-r--r--   0 tjackles   (503) staff       (20)     5792 2023-04-10 20:37:54.000000 sigopt-8.8.1/sigopt/factory.py
--rw-r--r--   0 tjackles   (503) staff       (20)     3982 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/file_utils.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.887366 sigopt-8.8.1/sigopt/hyperopt/
--rw-r--r--   0 tjackles   (503) staff       (20)      117 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/hyperopt/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)     3401 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/hyperopt/base.py
--rw-r--r--   0 tjackles   (503) staff       (20)      715 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/hyperopt/compat.py
--rw-r--r--   0 tjackles   (503) staff       (20)    10837 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/interface.py
--rw-r--r--   0 tjackles   (503) staff       (20)     2141 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/lib.py
--rw-r--r--   0 tjackles   (503) staff       (20)     1317 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/local_run_context.py
--rw-r--r--   0 tjackles   (503) staff       (20)     2824 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/log_capture.py
--rw-r--r--   0 tjackles   (503) staff       (20)     4298 2023-04-27 20:20:23.000000 sigopt-8.8.1/sigopt/magics.py
--rw-r--r--   0 tjackles   (503) staff       (20)      245 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/model_aware_run.py
--rw-r--r--   0 tjackles   (503) staff       (20)    15123 2023-04-27 20:20:23.000000 sigopt-8.8.1/sigopt/objects.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.891562 sigopt-8.8.1/sigopt/orchestrate/
--rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/__init__.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.892285 sigopt-8.8.1/sigopt/orchestrate/aws/
--rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/aws/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)    14083 2023-04-27 20:20:23.000000 sigopt-8.8.1/sigopt/orchestrate/aws/service.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.895158 sigopt-8.8.1/sigopt/orchestrate/cloudformation/
--rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/cloudformation/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)     3115 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/cloudformation/cluster-autoscaler-role.yaml
--rw-r--r--   0 tjackles   (503) staff       (20)    11164 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/cloudformation/eks-cluster.yaml
--rw-r--r--   0 tjackles   (503) staff       (20)     5054 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/cloudformation/eks-node-security.yaml
--rw-r--r--   0 tjackles   (503) staff       (20)    12952 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/cloudformation/eks-nodegroup.yaml
--rw-r--r--   0 tjackles   (503) staff       (20)     6702 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/cloudformation/eks-vpc.yaml
--rw-r--r--   0 tjackles   (503) staff       (20)    17520 2023-04-27 20:20:23.000000 sigopt-8.8.1/sigopt/orchestrate/cloudformation/service.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.897238 sigopt-8.8.1/sigopt/orchestrate/cluster/
--rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/cluster/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)      550 2023-04-03 17:57:26.000000 sigopt-8.8.1/sigopt/orchestrate/cluster/context.py
--rw-r--r--   0 tjackles   (503) staff       (20)     1407 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/orchestrate/cluster/errors.py
--rw-r--r--   0 tjackles   (503) staff       (20)     2440 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/orchestrate/cluster/object.py
--rw-r--r--   0 tjackles   (503) staff       (20)     5623 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/orchestrate/cluster/service.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.898294 sigopt-8.8.1/sigopt/orchestrate/cluster_metadata/
--rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/cluster_metadata/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)      841 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/orchestrate/cluster_metadata/errors.py
--rw-r--r--   0 tjackles   (503) staff       (20)     2017 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/orchestrate/cluster_metadata/service.py
--rw-r--r--   0 tjackles   (503) staff       (20)     1196 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/orchestrate/common.py
--rw-r--r--   0 tjackles   (503) staff       (20)    18441 2023-04-27 20:20:23.000000 sigopt-8.8.1/sigopt/orchestrate/controller.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.899322 sigopt-8.8.1/sigopt/orchestrate/custom_cluster/
--rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/custom_cluster/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)     2267 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/orchestrate/custom_cluster/service.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.900523 sigopt-8.8.1/sigopt/orchestrate/docker/
--rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/docker/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)     6402 2023-04-27 20:20:23.000000 sigopt-8.8.1/sigopt/orchestrate/docker/service.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.901709 sigopt-8.8.1/sigopt/orchestrate/ec2/
--rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/ec2/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)     2570 2023-04-27 20:20:23.000000 sigopt-8.8.1/sigopt/orchestrate/ec2/service.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.903026 sigopt-8.8.1/sigopt/orchestrate/ecr/
--rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/ecr/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)     1044 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/orchestrate/ecr/service.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.904922 sigopt-8.8.1/sigopt/orchestrate/eks/
--rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/eks/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)      215 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/eks/kubeconfig.yml
--rw-r--r--   0 tjackles   (503) staff       (20)      577 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/orchestrate/eks/service.py
--rw-r--r--   0 tjackles   (503) staff       (20)     1818 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/orchestrate/exceptions.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.906260 sigopt-8.8.1/sigopt/orchestrate/gpu_options_validator/
--rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/gpu_options_validator/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)      504 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/orchestrate/gpu_options_validator/service.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.907534 sigopt-8.8.1/sigopt/orchestrate/iam/
--rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/iam/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)     3230 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/orchestrate/iam/service.py
--rw-r--r--   0 tjackles   (503) staff       (20)     2792 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/orchestrate/identifier.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.908759 sigopt-8.8.1/sigopt/orchestrate/job_runner/
--rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/job_runner/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)     7853 2023-04-27 20:20:23.000000 sigopt-8.8.1/sigopt/orchestrate/job_runner/service.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.910102 sigopt-8.8.1/sigopt/orchestrate/job_status/
--rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/job_status/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)     2214 2023-04-27 20:20:23.000000 sigopt-8.8.1/sigopt/orchestrate/job_status/service.py
--rw-r--r--   0 tjackles   (503) staff       (20)      800 2023-04-27 20:20:23.000000 sigopt-8.8.1/sigopt/orchestrate/json_stream.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.911519 sigopt-8.8.1/sigopt/orchestrate/kubectl/
--rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/kubectl/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)      797 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/orchestrate/kubectl/service.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.913492 sigopt-8.8.1/sigopt/orchestrate/kubernetes/
--rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/kubernetes/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)     1014 2023-04-27 20:20:23.000000 sigopt-8.8.1/sigopt/orchestrate/kubernetes/http_proxy.py
--rw-r--r--   0 tjackles   (503) staff       (20)    22925 2023-04-27 20:20:23.000000 sigopt-8.8.1/sigopt/orchestrate/kubernetes/service.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.915384 sigopt-8.8.1/sigopt/orchestrate/lib/
--rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/lib/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)     1402 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/orchestrate/lib/lists.py
--rw-r--r--   0 tjackles   (503) staff       (20)     1168 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/orchestrate/lib/types.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.916539 sigopt-8.8.1/sigopt/orchestrate/logging/
--rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/logging/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)      682 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/orchestrate/logging/service.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.918174 sigopt-8.8.1/sigopt/orchestrate/model_packer/
--rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/model_packer/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)     3393 2023-04-27 20:20:23.000000 sigopt-8.8.1/sigopt/orchestrate/model_packer/service.py
--rw-r--r--   0 tjackles   (503) staff       (20)      261 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/node_groups.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.919525 sigopt-8.8.1/sigopt/orchestrate/options_validator/
--rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/options_validator/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)     4606 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/orchestrate/options_validator/service.py
--rw-r--r--   0 tjackles   (503) staff       (20)     3710 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/orchestrate/paths.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.921961 sigopt-8.8.1/sigopt/orchestrate/plugins/
--rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/plugins/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)     4965 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/plugins/autoscaler-plugin-template.yml
--rw-r--r--   0 tjackles   (503) staff       (20)      200 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/plugins/docker-service.yml
--rw-r--r--   0 tjackles   (503) staff       (20)     1699 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/plugins/docker-statefulset.yml
--rw-r--r--   0 tjackles   (503) staff       (20)      800 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/plugins/orchestrate-controller-roles.yml
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.923981 sigopt-8.8.1/sigopt/orchestrate/provider/
--rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/provider/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)      610 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/provider/broker.py
--rw-r--r--   0 tjackles   (503) staff       (20)     1120 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/orchestrate/provider/constants.py
--rw-r--r--   0 tjackles   (503) staff       (20)      604 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/provider/interface.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.924839 sigopt-8.8.1/sigopt/orchestrate/resource/
--rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/resource/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)      887 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/orchestrate/resource/service.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.925688 sigopt-8.8.1/sigopt/orchestrate/s3/
--rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/s3/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)     2373 2023-04-27 20:20:23.000000 sigopt-8.8.1/sigopt/orchestrate/s3/service.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.928528 sigopt-8.8.1/sigopt/orchestrate/services/
--rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/services/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)      302 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/orchestrate/services/aws_base.py
--rw-r--r--   0 tjackles   (503) staff       (20)     1144 2023-04-03 17:57:26.000000 sigopt-8.8.1/sigopt/orchestrate/services/aws_provider_bag.py
--rw-r--r--   0 tjackles   (503) staff       (20)      547 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/orchestrate/services/bag.py
--rw-r--r--   0 tjackles   (503) staff       (20)      203 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/orchestrate/services/base.py
--rw-r--r--   0 tjackles   (503) staff       (20)     1685 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/services/orchestrate_bag.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.929324 sigopt-8.8.1/sigopt/orchestrate/sigopt/
--rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/sigopt/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)     2995 2023-04-27 20:20:23.000000 sigopt-8.8.1/sigopt/orchestrate/sigopt/service.py
--rw-r--r--   0 tjackles   (503) staff       (20)     4504 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/orchestrate/status.py
--rw-r--r--   0 tjackles   (503) staff       (20)     1078 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/orchestrate/stop.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.930077 sigopt-8.8.1/sigopt/orchestrate/sts/
--rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/sts/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)      595 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/orchestrate/sts/service.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.930775 sigopt-8.8.1/sigopt/orchestrate/test/
--rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/test/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)       54 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/test/test_file.txt
--rw-r--r--   0 tjackles   (503) staff       (20)      263 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/orchestrate/version.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.931143 sigopt-8.8.1/sigopt/orchestrate/zigopt/
--rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/zigopt/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)      570 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/paths.py
--rw-r--r--   0 tjackles   (503) staff       (20)      666 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/ratelimit.py
--rw-r--r--   0 tjackles   (503) staff       (20)     5429 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/request_driver.py
--rw-r--r--   0 tjackles   (503) staff       (20)     2148 2023-04-27 20:20:23.000000 sigopt-8.8.1/sigopt/resource.py
--rw-r--r--   0 tjackles   (503) staff       (20)    15648 2023-04-27 20:20:23.000000 sigopt-8.8.1/sigopt/run_context.py
--rw-r--r--   0 tjackles   (503) staff       (20)      757 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/run_factory.py
--rw-r--r--   0 tjackles   (503) staff       (20)     4514 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/run_params.py
--rw-r--r--   0 tjackles   (503) staff       (20)      410 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/sigopt_logging.py
--rw-r--r--   0 tjackles   (503) staff       (20)     1713 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/urllib3_patch.py
--rw-r--r--   0 tjackles   (503) staff       (20)      577 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/utils.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.933846 sigopt-8.8.1/sigopt/validate/
--rw-r--r--   0 tjackles   (503) staff       (20)      257 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/validate/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)     6950 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/validate/aiexperiment_input.py
--rw-r--r--   0 tjackles   (503) staff       (20)      333 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/validate/common.py
--rw-r--r--   0 tjackles   (503) staff       (20)      112 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/validate/exceptions.py
--rw-r--r--   0 tjackles   (503) staff       (20)       95 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/validate/keys.py
--rw-r--r--   0 tjackles   (503) staff       (20)     1721 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/validate/run_input.py
--rw-r--r--   0 tjackles   (503) staff       (20)       89 2023-07-17 18:13:21.000000 sigopt-8.8.1/sigopt/version.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.937656 sigopt-8.8.1/sigopt/xgboost/
--rw-r--r--   0 tjackles   (503) staff       (20)      127 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/xgboost/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)     1085 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/xgboost/checkpoint_callback.py
--rw-r--r--   0 tjackles   (503) staff       (20)      693 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/xgboost/compat.py
--rw-r--r--   0 tjackles   (503) staff       (20)     3037 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/xgboost/compute_metrics.py
--rw-r--r--   0 tjackles   (503) staff       (20)     3913 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/xgboost/constants.py
--rw-r--r--   0 tjackles   (503) staff       (20)    10142 2023-04-03 19:57:41.000000 sigopt-8.8.1/sigopt/xgboost/experiment.py
--rw-r--r--   0 tjackles   (503) staff       (20)    12660 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/xgboost/run.py
--rw-r--r--   0 tjackles   (503) staff       (20)      942 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/xgboost/utils.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.856768 sigopt-8.8.1/sigopt.egg-info/
--rw-r--r--   0 tjackles   (503) staff       (20)      617 2023-07-17 18:17:28.000000 sigopt-8.8.1/sigopt.egg-info/PKG-INFO
--rw-r--r--   0 tjackles   (503) staff       (20)     9905 2023-07-17 18:17:28.000000 sigopt-8.8.1/sigopt.egg-info/SOURCES.txt
--rw-r--r--   0 tjackles   (503) staff       (20)        1 2023-07-17 18:17:28.000000 sigopt-8.8.1/sigopt.egg-info/dependency_links.txt
--rw-r--r--   0 tjackles   (503) staff       (20)       58 2023-07-17 18:17:28.000000 sigopt-8.8.1/sigopt.egg-info/entry_points.txt
--rw-r--r--   0 tjackles   (503) staff       (20)      784 2023-07-17 18:17:28.000000 sigopt-8.8.1/sigopt.egg-info/requires.txt
--rw-r--r--   0 tjackles   (503) staff       (20)       29 2023-07-17 18:17:28.000000 sigopt-8.8.1/sigopt.egg-info/top_level.txt
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.938460 sigopt-8.8.1/test/
--rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/test/__init__.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.945296 sigopt-8.8.1/test/cli/
--rw-r--r--   0 tjackles   (503) staff       (20)     1294 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/cli/test_cli_config.py
--rw-r--r--   0 tjackles   (503) staff       (20)      517 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/cli/test_cluster_connect.py
--rw-r--r--   0 tjackles   (503) staff       (20)      547 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/cli/test_cluster_create.py
--rw-r--r--   0 tjackles   (503) staff       (20)     1028 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/cli/test_cluster_destroy.py
--rw-r--r--   0 tjackles   (503) staff       (20)      486 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/cli/test_cluster_disconnect.py
--rw-r--r--   0 tjackles   (503) staff       (20)     1426 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/cli/test_cluster_kubectl.py
--rw-r--r--   0 tjackles   (503) staff       (20)      939 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/cli/test_cluster_run.py
--rw-r--r--   0 tjackles   (503) staff       (20)      534 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/cli/test_cluster_test.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.946767 sigopt-8.8.1/test/cli/test_files/
--rw-r--r--   0 tjackles   (503) staff       (20)      123 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/cli/test_files/import_hello.py
--rw-r--r--   0 tjackles   (503) staff       (20)      157 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/cli/test_files/print_args.py
--rw-r--r--   0 tjackles   (503) staff       (20)      126 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/cli/test_files/print_hello.py
--rw-r--r--   0 tjackles   (503) staff       (20)      708 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/cli/test_init.py
--rw-r--r--   0 tjackles   (503) staff       (20)     3311 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/cli/test_optimize.py
--rw-r--r--   0 tjackles   (503) staff       (20)     2566 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/cli/test_run.py
--rw-r--r--   0 tjackles   (503) staff       (20)     2590 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/cli/test_start_worker.py
--rw-r--r--   0 tjackles   (503) staff       (20)      578 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/cli/test_truncate.py
--rw-r--r--   0 tjackles   (503) staff       (20)      382 2023-03-14 22:13:41.000000 sigopt-8.8.1/test/cli/test_version.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.952078 sigopt-8.8.1/test/client/
--rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/test/client/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)    10389 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/client/test_endpoint.py
--rw-r--r--   0 tjackles   (503) staff       (20)     2851 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/client/test_interface.py
--rw-r--r--   0 tjackles   (503) staff       (20)     4687 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/client/test_lib.py
--rw-r--r--   0 tjackles   (503) staff       (20)    18457 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/client/test_object.py
--rw-r--r--   0 tjackles   (503) staff       (20)     9440 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/client/test_pagination.py
--rw-r--r--   0 tjackles   (503) staff       (20)     3702 2023-03-17 22:29:13.000000 sigopt-8.8.1/test/client/test_request_driver.py
--rw-r--r--   0 tjackles   (503) staff       (20)     3154 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/client/test_requestor.py
--rw-r--r--   0 tjackles   (503) staff       (20)     1641 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/client/test_resource.py
--rw-r--r--   0 tjackles   (503) staff       (20)      787 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/client/test_urllib3_patch.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.953359 sigopt-8.8.1/test/orchestrate/
--rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/test/orchestrate/__init__.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.954578 sigopt-8.8.1/test/orchestrate/aws/
--rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/test/orchestrate/aws/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)     2862 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/orchestrate/aws/service_test.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.955895 sigopt-8.8.1/test/orchestrate/cluster/
--rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/test/orchestrate/cluster/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)     8090 2023-04-27 20:20:23.000000 sigopt-8.8.1/test/orchestrate/cluster/service_test.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.957450 sigopt-8.8.1/test/orchestrate/cluster_metadata/
--rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/test/orchestrate/cluster_metadata/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)     3062 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/orchestrate/cluster_metadata/service_test.py
--rw-r--r--   0 tjackles   (503) staff       (20)      831 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/orchestrate/common_test.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.958739 sigopt-8.8.1/test/orchestrate/docker/
--rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/test/orchestrate/docker/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)     1767 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/orchestrate/docker/service_test.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.960033 sigopt-8.8.1/test/orchestrate/ecr/
--rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/test/orchestrate/ecr/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)      510 2023-03-14 22:13:41.000000 sigopt-8.8.1/test/orchestrate/ecr/service_test.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.961416 sigopt-8.8.1/test/orchestrate/gpu_options_validator/
--rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/test/orchestrate/gpu_options_validator/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)     1115 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/orchestrate/gpu_options_validator/service_test.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.962990 sigopt-8.8.1/test/orchestrate/job_runner/
--rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/test/orchestrate/job_runner/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)     2084 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/orchestrate/job_runner/service_test.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.963872 sigopt-8.8.1/test/orchestrate/job_status/
--rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/test/orchestrate/job_status/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)     1914 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/orchestrate/job_status/service_test.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.964857 sigopt-8.8.1/test/orchestrate/kubernetes/
--rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/test/orchestrate/kubernetes/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)     4812 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/orchestrate/kubernetes/service_test.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.967130 sigopt-8.8.1/test/orchestrate/lib/
--rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/test/orchestrate/lib/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)     2347 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/orchestrate/lib/lists_test.py
--rw-r--r--   0 tjackles   (503) staff       (20)     4633 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/orchestrate/lib/types_test.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.967800 sigopt-8.8.1/test/orchestrate/model_packer/
--rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/test/orchestrate/model_packer/__init__.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.968942 sigopt-8.8.1/test/orchestrate/options_validator/
--rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/test/orchestrate/options_validator/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)     9367 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/orchestrate/options_validator/service_test.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.970039 sigopt-8.8.1/test/orchestrate/provider/
--rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/test/orchestrate/provider/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)     1401 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/orchestrate/provider/broker_test.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.970801 sigopt-8.8.1/test/orchestrate/resource/
--rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/test/orchestrate/resource/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)     1142 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/orchestrate/resource/service_test.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.972241 sigopt-8.8.1/test/orchestrate/services/
--rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/test/orchestrate/services/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)     1131 2023-03-14 22:13:41.000000 sigopt-8.8.1/test/orchestrate/services/aws_provider_bag_test.py
--rw-r--r--   0 tjackles   (503) staff       (20)      309 2023-03-14 22:13:41.000000 sigopt-8.8.1/test/orchestrate/services/base_test.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.972646 sigopt-8.8.1/test/orchestrate/sigopt/
--rw-r--r--   0 tjackles   (503) staff       (20)      671 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/orchestrate/sigopt/service_test.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.973386 sigopt-8.8.1/test/orchestrate/sts/
--rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/test/orchestrate/sts/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)      510 2023-03-14 22:13:41.000000 sigopt-8.8.1/test/orchestrate/sts/service_test.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.976743 sigopt-8.8.1/test/runs/
--rw-r--r--   0 tjackles   (503) staff       (20)      599 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/runs/test_config.py
--rw-r--r--   0 tjackles   (503) staff       (20)     6965 2023-04-27 20:20:23.000000 sigopt-8.8.1/test/runs/test_context.py
--rw-r--r--   0 tjackles   (503) staff       (20)      577 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/runs/test_defaults.py
--rw-r--r--   0 tjackles   (503) staff       (20)     2414 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/runs/test_factory.py
--rw-r--r--   0 tjackles   (503) staff       (20)     2123 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/runs/test_local_run_context.py
--rw-r--r--   0 tjackles   (503) staff       (20)      624 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/runs/test_set_project.py
--rw-r--r--   0 tjackles   (503) staff       (20)     5199 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/runs/test_utils.py
--rw-r--r--   0 tjackles   (503) staff       (20)      299 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/runs/utils.py
--rw-r--r--   0 tjackles   (503) staff       (20)      299 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/utils.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.977506 sigopt-8.8.1/test/validate/
--rw-r--r--   0 tjackles   (503) staff       (20)     5235 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/validate/test_validate_experiment.py
--rw-r--r--   0 tjackles   (503) staff       (20)     2009 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/validate/test_validate_run.py
-drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.979246 sigopt-8.8.1/test/xgboost/
--rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/test/xgboost/__init__.py
--rw-r--r--   0 tjackles   (503) staff       (20)     5133 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/xgboost/test_compute_metric.py
--rw-r--r--   0 tjackles   (503) staff       (20)     8974 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/xgboost/test_experiment_config.py
--rw-r--r--   0 tjackles   (503) staff       (20)     3345 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/xgboost/test_run_options_parsing.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.375712 sigopt-8.8.2/
+-rw-r--r--   0 tjackles   (503) staff       (20)     1083 2022-02-18 18:21:31.000000 sigopt-8.8.2/LICENSE
+-rw-r--r--   0 tjackles   (503) staff       (20)      109 2021-10-21 13:30:45.000000 sigopt-8.8.2/MANIFEST.in
+-rw-r--r--   0 tjackles   (503) staff       (20)      617 2023-07-17 20:41:28.375920 sigopt-8.8.2/PKG-INFO
+-rw-r--r--   0 tjackles   (503) staff       (20)     4491 2023-07-17 17:31:25.000000 sigopt-8.8.2/README.md
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.186968 sigopt-8.8.2/integration_test/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.2/integration_test/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1405 2023-04-03 19:26:20.000000 sigopt-8.8.2/integration_test/test_experiment.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     4110 2023-06-27 22:27:24.000000 sigopt-8.8.2/integration_test/test_hyperopt.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      723 2023-04-03 19:26:20.000000 sigopt-8.8.2/integration_test/test_sigopt.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     6745 2023-04-03 19:26:20.000000 sigopt-8.8.2/integration_test/test_xgboost_experiment.py
+-rw-r--r--   0 tjackles   (503) staff       (20)    15097 2023-04-03 19:26:20.000000 sigopt-8.8.2/integration_test/test_xgboost_run.py
+-rw-r--r--   0 tjackles   (503) staff       (20)       56 2023-04-03 19:26:20.000000 sigopt-8.8.2/pyproject.toml
+-rw-r--r--   0 tjackles   (503) staff       (20)      391 2023-07-17 20:41:28.376867 sigopt-8.8.2/setup.cfg
+-rw-r--r--   0 tjackles   (503) staff       (20)     2752 2023-07-17 20:40:26.000000 sigopt-8.8.2/setup.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.203750 sigopt-8.8.2/sigopt/
+-rw-r--r--   0 tjackles   (503) staff       (20)     2135 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     2907 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/aiexperiment_context.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.209488 sigopt-8.8.2/sigopt/cli/
+-rw-r--r--   0 tjackles   (503) staff       (20)      121 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/cli/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      148 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/cli/__main__.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.222367 sigopt-8.8.2/sigopt/cli/arguments/
+-rw-r--r--   0 tjackles   (503) staff       (20)      686 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/cli/arguments/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      396 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/cli/arguments/cluster_filename.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      188 2023-04-03 17:57:25.000000 sigopt-8.8.2/sigopt/cli/arguments/cluster_name.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      167 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/cli/arguments/commands.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      206 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/cli/arguments/dockerfile.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      432 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/cli/arguments/experiment_file.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      200 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/cli/arguments/experiment_id.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      570 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/cli/arguments/identifiers.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1121 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/cli/arguments/load_yaml.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1157 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/cli/arguments/project.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      344 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/cli/arguments/provider.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      443 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/cli/arguments/run_file.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      478 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/cli/arguments/source_file.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      319 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/cli/arguments/validate.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.225809 sigopt-8.8.2/sigopt/cli/commands/
+-rw-r--r--   0 tjackles   (503) staff       (20)      383 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/cli/commands/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      510 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/cli/commands/base.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.233358 sigopt-8.8.2/sigopt/cli/commands/cluster/
+-rw-r--r--   0 tjackles   (503) staff       (20)      862 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/cli/commands/cluster/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      531 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/cli/commands/cluster/base.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      263 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/cli/commands/cluster/clean.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1053 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/cli/commands/cluster/connect.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      569 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/cli/commands/cluster/create.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      285 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/cli/commands/cluster/destroy.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      304 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/cli/commands/cluster/disconnect.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      302 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/cli/commands/cluster/install_plugins.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      521 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/cli/commands/cluster/kubectl.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      485 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/cli/commands/cluster/not_installed.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      777 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/cli/commands/cluster/optimize.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      690 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/cli/commands/cluster/run.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      622 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/cli/commands/cluster/status.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      511 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/cli/commands/cluster/stop.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      295 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/cli/commands/cluster/test.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      706 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/cli/commands/cluster/test_run.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      369 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/cli/commands/cluster/update.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1282 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/cli/commands/config.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.235109 sigopt-8.8.2/sigopt/cli/commands/experiment/
+-rw-r--r--   0 tjackles   (503) staff       (20)      210 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/cli/commands/experiment/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      688 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/cli/commands/experiment/archive.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      952 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/cli/commands/experiment/create.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      687 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/cli/commands/experiment/unarchive.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      986 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/cli/commands/init.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.236705 sigopt-8.8.2/sigopt/cli/commands/local/
+-rw-r--r--   0 tjackles   (503) staff       (20)      196 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/cli/commands/local/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      810 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/cli/commands/local/optimize.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      756 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/cli/commands/local/run.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      912 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/cli/commands/local/start_worker.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      244 2023-04-03 19:57:41.000000 sigopt-8.8.2/sigopt/cli/commands/optimize_base.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.237545 sigopt-8.8.2/sigopt/cli/commands/project/
+-rw-r--r--   0 tjackles   (503) staff       (20)      113 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/cli/commands/project/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      850 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/cli/commands/project/create.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      738 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/cli/commands/run_base.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.238673 sigopt-8.8.2/sigopt/cli/commands/training_run/
+-rw-r--r--   0 tjackles   (503) staff       (20)      169 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/cli/commands/training_run/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      605 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/cli/commands/training_run/archive.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      615 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/cli/commands/training_run/unarchive.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      235 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/cli/commands/version.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.241611 sigopt-8.8.2/sigopt/cli/resources/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/cli/resources/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      668 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/cli/resources/init_dockerfile.txt
+-rw-r--r--   0 tjackles   (503) staff       (20)       34 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/cli/resources/init_dockerignore.txt
+-rw-r--r--   0 tjackles   (503) staff       (20)      208 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/cli/resources/init_experiment.txt
+-rw-r--r--   0 tjackles   (503) staff       (20)       83 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/cli/resources/init_run.txt
+-rw-r--r--   0 tjackles   (503) staff       (20)     4897 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/cli/utils.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      355 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/compat.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     3231 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/config.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1867 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/defaults.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1137 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/endpoint.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.243229 sigopt-8.8.2/sigopt/examples/
+-rw-r--r--   0 tjackles   (503) staff       (20)       93 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/examples/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      874 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/examples/franke.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     2117 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/exception.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     5792 2023-04-10 20:37:54.000000 sigopt-8.8.2/sigopt/factory.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     3982 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/file_utils.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.245623 sigopt-8.8.2/sigopt/hyperopt/
+-rw-r--r--   0 tjackles   (503) staff       (20)      117 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/hyperopt/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     3401 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/hyperopt/base.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      715 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/hyperopt/compat.py
+-rw-r--r--   0 tjackles   (503) staff       (20)    10837 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/interface.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     2141 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/lib.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1317 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/local_run_context.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     2824 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/log_capture.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     4298 2023-04-27 20:20:23.000000 sigopt-8.8.2/sigopt/magics.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      245 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/model_aware_run.py
+-rw-r--r--   0 tjackles   (503) staff       (20)    15123 2023-04-27 20:20:23.000000 sigopt-8.8.2/sigopt/objects.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.254458 sigopt-8.8.2/sigopt/orchestrate/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/orchestrate/__init__.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.256102 sigopt-8.8.2/sigopt/orchestrate/aws/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/orchestrate/aws/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)    14083 2023-04-27 20:20:23.000000 sigopt-8.8.2/sigopt/orchestrate/aws/service.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.262280 sigopt-8.8.2/sigopt/orchestrate/cloudformation/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/orchestrate/cloudformation/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     3115 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/orchestrate/cloudformation/cluster-autoscaler-role.yaml
+-rw-r--r--   0 tjackles   (503) staff       (20)    11164 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/orchestrate/cloudformation/eks-cluster.yaml
+-rw-r--r--   0 tjackles   (503) staff       (20)     5054 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/orchestrate/cloudformation/eks-node-security.yaml
+-rw-r--r--   0 tjackles   (503) staff       (20)    12952 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/orchestrate/cloudformation/eks-nodegroup.yaml
+-rw-r--r--   0 tjackles   (503) staff       (20)     6702 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/orchestrate/cloudformation/eks-vpc.yaml
+-rw-r--r--   0 tjackles   (503) staff       (20)    17520 2023-04-27 20:20:23.000000 sigopt-8.8.2/sigopt/orchestrate/cloudformation/service.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.265492 sigopt-8.8.2/sigopt/orchestrate/cluster/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/orchestrate/cluster/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      550 2023-04-03 17:57:26.000000 sigopt-8.8.2/sigopt/orchestrate/cluster/context.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1407 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/orchestrate/cluster/errors.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     2440 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/orchestrate/cluster/object.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     5623 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/orchestrate/cluster/service.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.267716 sigopt-8.8.2/sigopt/orchestrate/cluster_metadata/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/orchestrate/cluster_metadata/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      841 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/orchestrate/cluster_metadata/errors.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     2017 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/orchestrate/cluster_metadata/service.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1196 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/orchestrate/common.py
+-rw-r--r--   0 tjackles   (503) staff       (20)    18441 2023-04-27 20:20:23.000000 sigopt-8.8.2/sigopt/orchestrate/controller.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.268699 sigopt-8.8.2/sigopt/orchestrate/custom_cluster/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/orchestrate/custom_cluster/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     2267 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/orchestrate/custom_cluster/service.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.269748 sigopt-8.8.2/sigopt/orchestrate/docker/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/orchestrate/docker/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     6402 2023-04-27 20:20:23.000000 sigopt-8.8.2/sigopt/orchestrate/docker/service.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.270599 sigopt-8.8.2/sigopt/orchestrate/ec2/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/orchestrate/ec2/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     2570 2023-04-27 20:20:23.000000 sigopt-8.8.2/sigopt/orchestrate/ec2/service.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.271571 sigopt-8.8.2/sigopt/orchestrate/ecr/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/orchestrate/ecr/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1044 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/orchestrate/ecr/service.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.273706 sigopt-8.8.2/sigopt/orchestrate/eks/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/orchestrate/eks/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      215 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/orchestrate/eks/kubeconfig.yml
+-rw-r--r--   0 tjackles   (503) staff       (20)      577 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/orchestrate/eks/service.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1818 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/orchestrate/exceptions.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.274774 sigopt-8.8.2/sigopt/orchestrate/gpu_options_validator/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/orchestrate/gpu_options_validator/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      504 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/orchestrate/gpu_options_validator/service.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.276028 sigopt-8.8.2/sigopt/orchestrate/iam/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/orchestrate/iam/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     3230 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/orchestrate/iam/service.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     2792 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/orchestrate/identifier.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.277434 sigopt-8.8.2/sigopt/orchestrate/job_runner/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/orchestrate/job_runner/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     7853 2023-04-27 20:20:23.000000 sigopt-8.8.2/sigopt/orchestrate/job_runner/service.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.278770 sigopt-8.8.2/sigopt/orchestrate/job_status/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/orchestrate/job_status/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     2214 2023-04-27 20:20:23.000000 sigopt-8.8.2/sigopt/orchestrate/job_status/service.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      800 2023-04-27 20:20:23.000000 sigopt-8.8.2/sigopt/orchestrate/json_stream.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.280479 sigopt-8.8.2/sigopt/orchestrate/kubectl/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/orchestrate/kubectl/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      797 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/orchestrate/kubectl/service.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.282913 sigopt-8.8.2/sigopt/orchestrate/kubernetes/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/orchestrate/kubernetes/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1014 2023-04-27 20:20:23.000000 sigopt-8.8.2/sigopt/orchestrate/kubernetes/http_proxy.py
+-rw-r--r--   0 tjackles   (503) staff       (20)    22925 2023-04-27 20:20:23.000000 sigopt-8.8.2/sigopt/orchestrate/kubernetes/service.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.286349 sigopt-8.8.2/sigopt/orchestrate/lib/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/orchestrate/lib/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1402 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/orchestrate/lib/lists.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1168 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/orchestrate/lib/types.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.287924 sigopt-8.8.2/sigopt/orchestrate/logging/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/orchestrate/logging/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      682 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/orchestrate/logging/service.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.289863 sigopt-8.8.2/sigopt/orchestrate/model_packer/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/orchestrate/model_packer/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     3393 2023-04-27 20:20:23.000000 sigopt-8.8.2/sigopt/orchestrate/model_packer/service.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      261 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/orchestrate/node_groups.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.291361 sigopt-8.8.2/sigopt/orchestrate/options_validator/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/orchestrate/options_validator/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     4606 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/orchestrate/options_validator/service.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     3710 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/orchestrate/paths.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.294878 sigopt-8.8.2/sigopt/orchestrate/plugins/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/orchestrate/plugins/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     4965 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/orchestrate/plugins/autoscaler-plugin-template.yml
+-rw-r--r--   0 tjackles   (503) staff       (20)      200 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/orchestrate/plugins/docker-service.yml
+-rw-r--r--   0 tjackles   (503) staff       (20)     1699 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/orchestrate/plugins/docker-statefulset.yml
+-rw-r--r--   0 tjackles   (503) staff       (20)      800 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/orchestrate/plugins/orchestrate-controller-roles.yml
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.299792 sigopt-8.8.2/sigopt/orchestrate/provider/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/orchestrate/provider/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      610 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/orchestrate/provider/broker.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1120 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/orchestrate/provider/constants.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      604 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/orchestrate/provider/interface.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.301248 sigopt-8.8.2/sigopt/orchestrate/resource/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/orchestrate/resource/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      887 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/orchestrate/resource/service.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.302682 sigopt-8.8.2/sigopt/orchestrate/s3/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/orchestrate/s3/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     2373 2023-04-27 20:20:23.000000 sigopt-8.8.2/sigopt/orchestrate/s3/service.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.307347 sigopt-8.8.2/sigopt/orchestrate/services/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/orchestrate/services/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      302 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/orchestrate/services/aws_base.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1144 2023-04-03 17:57:26.000000 sigopt-8.8.2/sigopt/orchestrate/services/aws_provider_bag.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      547 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/orchestrate/services/bag.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      203 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/orchestrate/services/base.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1685 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/orchestrate/services/orchestrate_bag.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.308080 sigopt-8.8.2/sigopt/orchestrate/sigopt/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/orchestrate/sigopt/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     2995 2023-04-27 20:20:23.000000 sigopt-8.8.2/sigopt/orchestrate/sigopt/service.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     4504 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/orchestrate/status.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1078 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/orchestrate/stop.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.309147 sigopt-8.8.2/sigopt/orchestrate/sts/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/orchestrate/sts/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      595 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/orchestrate/sts/service.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.310635 sigopt-8.8.2/sigopt/orchestrate/test/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/orchestrate/test/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)       54 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/orchestrate/test/test_file.txt
+-rw-r--r--   0 tjackles   (503) staff       (20)      263 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/orchestrate/version.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.311220 sigopt-8.8.2/sigopt/orchestrate/zigopt/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/orchestrate/zigopt/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      570 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/paths.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      666 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/ratelimit.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     5429 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/request_driver.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     2148 2023-04-27 20:20:23.000000 sigopt-8.8.2/sigopt/resource.py
+-rw-r--r--   0 tjackles   (503) staff       (20)    15648 2023-04-27 20:20:23.000000 sigopt-8.8.2/sigopt/run_context.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      757 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/run_factory.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     4514 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/run_params.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      410 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/sigopt_logging.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1713 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/urllib3_patch.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      577 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/utils.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.315260 sigopt-8.8.2/sigopt/validate/
+-rw-r--r--   0 tjackles   (503) staff       (20)      257 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/validate/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     6950 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/validate/aiexperiment_input.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      333 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/validate/common.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      112 2023-03-14 22:13:41.000000 sigopt-8.8.2/sigopt/validate/exceptions.py
+-rw-r--r--   0 tjackles   (503) staff       (20)       95 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/validate/keys.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1721 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/validate/run_input.py
+-rw-r--r--   0 tjackles   (503) staff       (20)       89 2023-07-17 20:40:42.000000 sigopt-8.8.2/sigopt/version.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.321089 sigopt-8.8.2/sigopt/xgboost/
+-rw-r--r--   0 tjackles   (503) staff       (20)      127 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/xgboost/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1085 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/xgboost/checkpoint_callback.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      693 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/xgboost/compat.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     3037 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/xgboost/compute_metrics.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     3913 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/xgboost/constants.py
+-rw-r--r--   0 tjackles   (503) staff       (20)    10142 2023-04-03 19:57:41.000000 sigopt-8.8.2/sigopt/xgboost/experiment.py
+-rw-r--r--   0 tjackles   (503) staff       (20)    12660 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/xgboost/run.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      942 2023-04-03 19:26:20.000000 sigopt-8.8.2/sigopt/xgboost/utils.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.207211 sigopt-8.8.2/sigopt.egg-info/
+-rw-r--r--   0 tjackles   (503) staff       (20)      617 2023-07-17 20:41:27.000000 sigopt-8.8.2/sigopt.egg-info/PKG-INFO
+-rw-r--r--   0 tjackles   (503) staff       (20)     9905 2023-07-17 20:41:28.000000 sigopt-8.8.2/sigopt.egg-info/SOURCES.txt
+-rw-r--r--   0 tjackles   (503) staff       (20)        1 2023-07-17 20:41:27.000000 sigopt-8.8.2/sigopt.egg-info/dependency_links.txt
+-rw-r--r--   0 tjackles   (503) staff       (20)       58 2023-07-17 20:41:27.000000 sigopt-8.8.2/sigopt.egg-info/entry_points.txt
+-rw-r--r--   0 tjackles   (503) staff       (20)      803 2023-07-17 20:41:27.000000 sigopt-8.8.2/sigopt.egg-info/requires.txt
+-rw-r--r--   0 tjackles   (503) staff       (20)       29 2023-07-17 20:41:27.000000 sigopt-8.8.2/sigopt.egg-info/top_level.txt
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.322308 sigopt-8.8.2/test/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.2/test/__init__.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.332646 sigopt-8.8.2/test/cli/
+-rw-r--r--   0 tjackles   (503) staff       (20)     1294 2023-04-03 19:26:20.000000 sigopt-8.8.2/test/cli/test_cli_config.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      517 2023-04-03 19:26:20.000000 sigopt-8.8.2/test/cli/test_cluster_connect.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      547 2023-04-03 19:26:20.000000 sigopt-8.8.2/test/cli/test_cluster_create.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1028 2023-04-03 19:26:20.000000 sigopt-8.8.2/test/cli/test_cluster_destroy.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      486 2023-04-03 19:26:20.000000 sigopt-8.8.2/test/cli/test_cluster_disconnect.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1426 2023-04-03 19:26:20.000000 sigopt-8.8.2/test/cli/test_cluster_kubectl.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      939 2023-04-03 19:26:20.000000 sigopt-8.8.2/test/cli/test_cluster_run.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      534 2023-04-03 19:26:20.000000 sigopt-8.8.2/test/cli/test_cluster_test.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.334548 sigopt-8.8.2/test/cli/test_files/
+-rw-r--r--   0 tjackles   (503) staff       (20)      123 2023-04-03 19:26:20.000000 sigopt-8.8.2/test/cli/test_files/import_hello.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      157 2023-04-03 19:26:20.000000 sigopt-8.8.2/test/cli/test_files/print_args.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      126 2023-04-03 19:26:20.000000 sigopt-8.8.2/test/cli/test_files/print_hello.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      708 2023-04-03 19:26:20.000000 sigopt-8.8.2/test/cli/test_init.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     3311 2023-04-03 19:26:20.000000 sigopt-8.8.2/test/cli/test_optimize.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     2566 2023-04-03 19:26:20.000000 sigopt-8.8.2/test/cli/test_run.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     2590 2023-04-03 19:26:20.000000 sigopt-8.8.2/test/cli/test_start_worker.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      578 2023-04-03 19:26:20.000000 sigopt-8.8.2/test/cli/test_truncate.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      382 2023-03-14 22:13:41.000000 sigopt-8.8.2/test/cli/test_version.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.342035 sigopt-8.8.2/test/client/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.2/test/client/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)    10389 2023-04-03 19:26:20.000000 sigopt-8.8.2/test/client/test_endpoint.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     2851 2023-04-03 19:26:20.000000 sigopt-8.8.2/test/client/test_interface.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     4687 2023-04-03 19:26:20.000000 sigopt-8.8.2/test/client/test_lib.py
+-rw-r--r--   0 tjackles   (503) staff       (20)    18457 2023-04-03 19:26:20.000000 sigopt-8.8.2/test/client/test_object.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     9440 2023-04-03 19:26:20.000000 sigopt-8.8.2/test/client/test_pagination.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     3702 2023-03-17 22:29:13.000000 sigopt-8.8.2/test/client/test_request_driver.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     3154 2023-04-03 19:26:20.000000 sigopt-8.8.2/test/client/test_requestor.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1641 2023-04-03 19:26:20.000000 sigopt-8.8.2/test/client/test_resource.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      787 2023-04-03 19:26:20.000000 sigopt-8.8.2/test/client/test_urllib3_patch.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.343618 sigopt-8.8.2/test/orchestrate/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.2/test/orchestrate/__init__.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.345583 sigopt-8.8.2/test/orchestrate/aws/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.2/test/orchestrate/aws/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     2862 2023-04-03 19:26:20.000000 sigopt-8.8.2/test/orchestrate/aws/service_test.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.347239 sigopt-8.8.2/test/orchestrate/cluster/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.2/test/orchestrate/cluster/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     8090 2023-04-27 20:20:23.000000 sigopt-8.8.2/test/orchestrate/cluster/service_test.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.348864 sigopt-8.8.2/test/orchestrate/cluster_metadata/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.2/test/orchestrate/cluster_metadata/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     3062 2023-04-03 19:26:20.000000 sigopt-8.8.2/test/orchestrate/cluster_metadata/service_test.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      831 2023-04-03 19:26:20.000000 sigopt-8.8.2/test/orchestrate/common_test.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.350144 sigopt-8.8.2/test/orchestrate/docker/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.2/test/orchestrate/docker/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1767 2023-04-03 19:26:20.000000 sigopt-8.8.2/test/orchestrate/docker/service_test.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.351997 sigopt-8.8.2/test/orchestrate/ecr/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.2/test/orchestrate/ecr/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      510 2023-03-14 22:13:41.000000 sigopt-8.8.2/test/orchestrate/ecr/service_test.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.353634 sigopt-8.8.2/test/orchestrate/gpu_options_validator/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.2/test/orchestrate/gpu_options_validator/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1115 2023-04-03 19:26:20.000000 sigopt-8.8.2/test/orchestrate/gpu_options_validator/service_test.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.355308 sigopt-8.8.2/test/orchestrate/job_runner/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.2/test/orchestrate/job_runner/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     2084 2023-04-03 19:26:20.000000 sigopt-8.8.2/test/orchestrate/job_runner/service_test.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.356397 sigopt-8.8.2/test/orchestrate/job_status/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.2/test/orchestrate/job_status/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1914 2023-04-03 19:26:20.000000 sigopt-8.8.2/test/orchestrate/job_status/service_test.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.357420 sigopt-8.8.2/test/orchestrate/kubernetes/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.2/test/orchestrate/kubernetes/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     4812 2023-04-03 19:26:20.000000 sigopt-8.8.2/test/orchestrate/kubernetes/service_test.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.359239 sigopt-8.8.2/test/orchestrate/lib/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.2/test/orchestrate/lib/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     2347 2023-04-03 19:26:20.000000 sigopt-8.8.2/test/orchestrate/lib/lists_test.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     4633 2023-04-03 19:26:20.000000 sigopt-8.8.2/test/orchestrate/lib/types_test.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.359970 sigopt-8.8.2/test/orchestrate/model_packer/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.2/test/orchestrate/model_packer/__init__.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.360621 sigopt-8.8.2/test/orchestrate/options_validator/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.2/test/orchestrate/options_validator/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     9367 2023-04-03 19:26:20.000000 sigopt-8.8.2/test/orchestrate/options_validator/service_test.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.361890 sigopt-8.8.2/test/orchestrate/provider/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.2/test/orchestrate/provider/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1401 2023-04-03 19:26:20.000000 sigopt-8.8.2/test/orchestrate/provider/broker_test.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.362949 sigopt-8.8.2/test/orchestrate/resource/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.2/test/orchestrate/resource/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1142 2023-04-03 19:26:20.000000 sigopt-8.8.2/test/orchestrate/resource/service_test.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.364603 sigopt-8.8.2/test/orchestrate/services/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.2/test/orchestrate/services/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1131 2023-03-14 22:13:41.000000 sigopt-8.8.2/test/orchestrate/services/aws_provider_bag_test.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      309 2023-03-14 22:13:41.000000 sigopt-8.8.2/test/orchestrate/services/base_test.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.365253 sigopt-8.8.2/test/orchestrate/sigopt/
+-rw-r--r--   0 tjackles   (503) staff       (20)      671 2023-04-03 19:26:20.000000 sigopt-8.8.2/test/orchestrate/sigopt/service_test.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.366178 sigopt-8.8.2/test/orchestrate/sts/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.2/test/orchestrate/sts/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      510 2023-03-14 22:13:41.000000 sigopt-8.8.2/test/orchestrate/sts/service_test.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.371111 sigopt-8.8.2/test/runs/
+-rw-r--r--   0 tjackles   (503) staff       (20)      599 2023-04-03 19:26:20.000000 sigopt-8.8.2/test/runs/test_config.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     6965 2023-04-27 20:20:23.000000 sigopt-8.8.2/test/runs/test_context.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      577 2023-04-03 19:26:20.000000 sigopt-8.8.2/test/runs/test_defaults.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     2414 2023-04-03 19:26:20.000000 sigopt-8.8.2/test/runs/test_factory.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     2123 2023-04-03 19:26:20.000000 sigopt-8.8.2/test/runs/test_local_run_context.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      624 2023-04-03 19:26:20.000000 sigopt-8.8.2/test/runs/test_set_project.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     5199 2023-04-03 19:26:20.000000 sigopt-8.8.2/test/runs/test_utils.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      299 2023-04-03 19:26:20.000000 sigopt-8.8.2/test/runs/utils.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      299 2023-04-03 19:26:20.000000 sigopt-8.8.2/test/utils.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.372283 sigopt-8.8.2/test/validate/
+-rw-r--r--   0 tjackles   (503) staff       (20)     5235 2023-04-03 19:26:20.000000 sigopt-8.8.2/test/validate/test_validate_experiment.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     2009 2023-04-03 19:26:20.000000 sigopt-8.8.2/test/validate/test_validate_run.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 20:41:28.375280 sigopt-8.8.2/test/xgboost/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.2/test/xgboost/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     5133 2023-04-03 19:26:20.000000 sigopt-8.8.2/test/xgboost/test_compute_metric.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     8974 2023-04-03 19:26:20.000000 sigopt-8.8.2/test/xgboost/test_experiment_config.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     3345 2023-04-03 19:26:20.000000 sigopt-8.8.2/test/xgboost/test_run_options_parsing.py
```

### Comparing `sigopt-8.8.1/LICENSE` & `sigopt-8.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/PKG-INFO` & `sigopt-8.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigopt
-Version: 8.8.1
+Version: 8.8.2
 Summary: SigOpt Python API Client
 Home-page: https://sigopt.com/
 Author: SigOpt
 Author-email: support@sigopt.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sigopt-8.8.1/README.md` & `sigopt-8.8.2/README.md`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/integration_test/test_experiment.py` & `sigopt-8.8.2/integration_test/test_experiment.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/integration_test/test_hyperopt.py` & `sigopt-8.8.2/integration_test/test_hyperopt.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/integration_test/test_sigopt.py` & `sigopt-8.8.2/integration_test/test_sigopt.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/integration_test/test_xgboost_experiment.py` & `sigopt-8.8.2/integration_test/test_xgboost_experiment.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/integration_test/test_xgboost_run.py` & `sigopt-8.8.2/integration_test/test_xgboost_run.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/setup.py` & `sigopt-8.8.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,14 +32,15 @@
   install_requires = requirements_fp.read().split("\n")
 with open(os.path.join(here, "requirements-dev.txt")) as requirements_dev_fp:
   dev_install_requires = requirements_dev_fp.read().split("\n")
 
 orchestrate_install_requires = [
   "Pint>=0.16.0,<0.17.0",
   "boto3>=1.16.34,<2.0.0",
+  "certifi>=2022.12.7",
   "docker>=4.4.0,<5.0.0",
   "kubernetes>=12.0.1,<13.0.0",
   "pyOpenSSL>=20.0.0",
 ]
 xgboost_install_requires = ["xgboost>=1.3.1", "numpy>=1.15.0"]
 hyperopt_install_requires = ["hyperopt>=0.2.7"]
 lite_install_requires = ["sigoptlite>=0.1.1"]
```

### Comparing `sigopt-8.8.1/sigopt/__init__.py` & `sigopt-8.8.2/sigopt/__init__.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/aiexperiment_context.py` & `sigopt-8.8.2/sigopt/aiexperiment_context.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/cli/arguments/__init__.py` & `sigopt-8.8.2/sigopt/cli/arguments/__init__.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/cli/arguments/identifiers.py` & `sigopt-8.8.2/sigopt/cli/arguments/identifiers.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/cli/arguments/load_yaml.py` & `sigopt-8.8.2/sigopt/cli/arguments/load_yaml.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/cli/arguments/project.py` & `sigopt-8.8.2/sigopt/cli/arguments/project.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/cli/commands/cluster/__init__.py` & `sigopt-8.8.2/sigopt/cli/commands/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/cli/commands/cluster/base.py` & `sigopt-8.8.2/sigopt/cli/commands/cluster/base.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/cli/commands/cluster/connect.py` & `sigopt-8.8.2/sigopt/cli/commands/cluster/connect.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/cli/commands/cluster/create.py` & `sigopt-8.8.2/sigopt/cli/commands/cluster/create.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/cli/commands/cluster/kubectl.py` & `sigopt-8.8.2/sigopt/cli/commands/cluster/kubectl.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/cli/commands/cluster/optimize.py` & `sigopt-8.8.2/sigopt/cli/commands/cluster/optimize.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/cli/commands/cluster/run.py` & `sigopt-8.8.2/sigopt/cli/commands/cluster/run.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/cli/commands/cluster/status.py` & `sigopt-8.8.2/sigopt/cli/commands/cluster/status.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/cli/commands/cluster/test_run.py` & `sigopt-8.8.2/sigopt/cli/commands/cluster/test_run.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/cli/commands/config.py` & `sigopt-8.8.2/sigopt/cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/cli/commands/experiment/archive.py` & `sigopt-8.8.2/sigopt/cli/commands/experiment/archive.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/cli/commands/experiment/create.py` & `sigopt-8.8.2/sigopt/cli/commands/experiment/create.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/cli/commands/experiment/unarchive.py` & `sigopt-8.8.2/sigopt/cli/commands/experiment/unarchive.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/cli/commands/init.py` & `sigopt-8.8.2/sigopt/cli/commands/init.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/cli/commands/local/optimize.py` & `sigopt-8.8.2/sigopt/cli/commands/local/optimize.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/cli/commands/local/run.py` & `sigopt-8.8.2/sigopt/cli/commands/local/run.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/cli/commands/local/start_worker.py` & `sigopt-8.8.2/sigopt/cli/commands/local/start_worker.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/cli/commands/project/create.py` & `sigopt-8.8.2/sigopt/cli/commands/project/create.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/cli/commands/run_base.py` & `sigopt-8.8.2/sigopt/cli/commands/run_base.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/cli/commands/training_run/archive.py` & `sigopt-8.8.2/sigopt/cli/commands/training_run/archive.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/cli/commands/training_run/unarchive.py` & `sigopt-8.8.2/sigopt/cli/commands/training_run/unarchive.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/cli/resources/init_dockerfile.txt` & `sigopt-8.8.2/sigopt/cli/resources/init_dockerfile.txt`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/cli/utils.py` & `sigopt-8.8.2/sigopt/cli/utils.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/config.py` & `sigopt-8.8.2/sigopt/config.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/defaults.py` & `sigopt-8.8.2/sigopt/defaults.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/endpoint.py` & `sigopt-8.8.2/sigopt/endpoint.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/examples/franke.py` & `sigopt-8.8.2/sigopt/examples/franke.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/exception.py` & `sigopt-8.8.2/sigopt/exception.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/factory.py` & `sigopt-8.8.2/sigopt/factory.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/file_utils.py` & `sigopt-8.8.2/sigopt/file_utils.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/hyperopt/base.py` & `sigopt-8.8.2/sigopt/hyperopt/base.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/hyperopt/compat.py` & `sigopt-8.8.2/sigopt/hyperopt/compat.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/interface.py` & `sigopt-8.8.2/sigopt/interface.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/lib.py` & `sigopt-8.8.2/sigopt/lib.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/local_run_context.py` & `sigopt-8.8.2/sigopt/local_run_context.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/log_capture.py` & `sigopt-8.8.2/sigopt/log_capture.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/magics.py` & `sigopt-8.8.2/sigopt/magics.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/objects.py` & `sigopt-8.8.2/sigopt/objects.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/orchestrate/aws/service.py` & `sigopt-8.8.2/sigopt/orchestrate/aws/service.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/orchestrate/cloudformation/cluster-autoscaler-role.yaml` & `sigopt-8.8.2/sigopt/orchestrate/cloudformation/cluster-autoscaler-role.yaml`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/orchestrate/cloudformation/eks-cluster.yaml` & `sigopt-8.8.2/sigopt/orchestrate/cloudformation/eks-cluster.yaml`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/orchestrate/cloudformation/eks-node-security.yaml` & `sigopt-8.8.2/sigopt/orchestrate/cloudformation/eks-node-security.yaml`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/orchestrate/cloudformation/eks-nodegroup.yaml` & `sigopt-8.8.2/sigopt/orchestrate/cloudformation/eks-nodegroup.yaml`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/orchestrate/cloudformation/eks-vpc.yaml` & `sigopt-8.8.2/sigopt/orchestrate/cloudformation/eks-vpc.yaml`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/orchestrate/cloudformation/service.py` & `sigopt-8.8.2/sigopt/orchestrate/cloudformation/service.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/orchestrate/cluster/context.py` & `sigopt-8.8.2/sigopt/orchestrate/cluster/context.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/orchestrate/cluster/errors.py` & `sigopt-8.8.2/sigopt/orchestrate/cluster/errors.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/orchestrate/cluster/object.py` & `sigopt-8.8.2/sigopt/orchestrate/cluster/object.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/orchestrate/cluster/service.py` & `sigopt-8.8.2/sigopt/orchestrate/cluster/service.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/orchestrate/cluster_metadata/errors.py` & `sigopt-8.8.2/sigopt/orchestrate/cluster_metadata/errors.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/orchestrate/cluster_metadata/service.py` & `sigopt-8.8.2/sigopt/orchestrate/cluster_metadata/service.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/orchestrate/common.py` & `sigopt-8.8.2/sigopt/orchestrate/common.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/orchestrate/controller.py` & `sigopt-8.8.2/sigopt/orchestrate/controller.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/orchestrate/custom_cluster/service.py` & `sigopt-8.8.2/sigopt/orchestrate/custom_cluster/service.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/orchestrate/docker/service.py` & `sigopt-8.8.2/sigopt/orchestrate/docker/service.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/orchestrate/ec2/service.py` & `sigopt-8.8.2/sigopt/orchestrate/ec2/service.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/orchestrate/ecr/service.py` & `sigopt-8.8.2/sigopt/orchestrate/ecr/service.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/orchestrate/eks/service.py` & `sigopt-8.8.2/sigopt/orchestrate/eks/service.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/orchestrate/exceptions.py` & `sigopt-8.8.2/sigopt/orchestrate/exceptions.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/orchestrate/iam/service.py` & `sigopt-8.8.2/sigopt/orchestrate/iam/service.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/orchestrate/identifier.py` & `sigopt-8.8.2/sigopt/orchestrate/identifier.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/orchestrate/job_runner/service.py` & `sigopt-8.8.2/sigopt/orchestrate/job_runner/service.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/orchestrate/job_status/service.py` & `sigopt-8.8.2/sigopt/orchestrate/job_status/service.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/orchestrate/json_stream.py` & `sigopt-8.8.2/sigopt/orchestrate/json_stream.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/orchestrate/kubectl/service.py` & `sigopt-8.8.2/sigopt/orchestrate/kubectl/service.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/orchestrate/kubernetes/http_proxy.py` & `sigopt-8.8.2/sigopt/orchestrate/kubernetes/http_proxy.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/orchestrate/kubernetes/service.py` & `sigopt-8.8.2/sigopt/orchestrate/kubernetes/service.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/orchestrate/lib/lists.py` & `sigopt-8.8.2/sigopt/orchestrate/lib/lists.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/orchestrate/lib/types.py` & `sigopt-8.8.2/sigopt/orchestrate/lib/types.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/orchestrate/logging/service.py` & `sigopt-8.8.2/sigopt/orchestrate/logging/service.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/orchestrate/model_packer/service.py` & `sigopt-8.8.2/sigopt/orchestrate/model_packer/service.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/orchestrate/options_validator/service.py` & `sigopt-8.8.2/sigopt/orchestrate/options_validator/service.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/orchestrate/paths.py` & `sigopt-8.8.2/sigopt/orchestrate/paths.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/orchestrate/plugins/autoscaler-plugin-template.yml` & `sigopt-8.8.2/sigopt/orchestrate/plugins/autoscaler-plugin-template.yml`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/orchestrate/plugins/docker-statefulset.yml` & `sigopt-8.8.2/sigopt/orchestrate/plugins/docker-statefulset.yml`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/orchestrate/plugins/orchestrate-controller-roles.yml` & `sigopt-8.8.2/sigopt/orchestrate/plugins/orchestrate-controller-roles.yml`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/orchestrate/provider/broker.py` & `sigopt-8.8.2/sigopt/orchestrate/provider/broker.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/orchestrate/provider/constants.py` & `sigopt-8.8.2/sigopt/orchestrate/provider/constants.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/orchestrate/provider/interface.py` & `sigopt-8.8.2/sigopt/orchestrate/provider/interface.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/orchestrate/resource/service.py` & `sigopt-8.8.2/sigopt/orchestrate/resource/service.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/orchestrate/s3/service.py` & `sigopt-8.8.2/sigopt/orchestrate/s3/service.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/orchestrate/services/aws_provider_bag.py` & `sigopt-8.8.2/sigopt/orchestrate/services/aws_provider_bag.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/orchestrate/services/bag.py` & `sigopt-8.8.2/sigopt/orchestrate/services/bag.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/orchestrate/services/orchestrate_bag.py` & `sigopt-8.8.2/sigopt/orchestrate/services/orchestrate_bag.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/orchestrate/sigopt/service.py` & `sigopt-8.8.2/sigopt/orchestrate/sigopt/service.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/orchestrate/status.py` & `sigopt-8.8.2/sigopt/orchestrate/status.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/orchestrate/stop.py` & `sigopt-8.8.2/sigopt/orchestrate/stop.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/orchestrate/sts/service.py` & `sigopt-8.8.2/sigopt/orchestrate/sts/service.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/paths.py` & `sigopt-8.8.2/sigopt/paths.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/ratelimit.py` & `sigopt-8.8.2/sigopt/ratelimit.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/request_driver.py` & `sigopt-8.8.2/sigopt/request_driver.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/resource.py` & `sigopt-8.8.2/sigopt/resource.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/run_context.py` & `sigopt-8.8.2/sigopt/run_context.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/run_factory.py` & `sigopt-8.8.2/sigopt/run_factory.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/run_params.py` & `sigopt-8.8.2/sigopt/run_params.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/urllib3_patch.py` & `sigopt-8.8.2/sigopt/urllib3_patch.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/utils.py` & `sigopt-8.8.2/sigopt/utils.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/validate/aiexperiment_input.py` & `sigopt-8.8.2/sigopt/validate/aiexperiment_input.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/validate/run_input.py` & `sigopt-8.8.2/sigopt/validate/run_input.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/xgboost/checkpoint_callback.py` & `sigopt-8.8.2/sigopt/xgboost/checkpoint_callback.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/xgboost/compat.py` & `sigopt-8.8.2/sigopt/xgboost/compat.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/xgboost/compute_metrics.py` & `sigopt-8.8.2/sigopt/xgboost/compute_metrics.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/xgboost/constants.py` & `sigopt-8.8.2/sigopt/xgboost/constants.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/xgboost/experiment.py` & `sigopt-8.8.2/sigopt/xgboost/experiment.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/xgboost/run.py` & `sigopt-8.8.2/sigopt/xgboost/run.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt/xgboost/utils.py` & `sigopt-8.8.2/sigopt/xgboost/utils.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt.egg-info/PKG-INFO` & `sigopt-8.8.2/sigopt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigopt
-Version: 8.8.1
+Version: 8.8.2
 Summary: SigOpt Python API Client
 Home-page: https://sigopt.com/
 Author: SigOpt
 Author-email: support@sigopt.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sigopt-8.8.1/sigopt.egg-info/SOURCES.txt` & `sigopt-8.8.2/sigopt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/sigopt.egg-info/requires.txt` & `sigopt-8.8.2/sigopt.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 backoff<2.0.0,>=1.10.0
-certifi==2022.12.7
 click>=8.0.0
 GitPython>=2.0.0
 packaging>=21.3
 pypng>=0.0.20
 PyYAML<7,>=5
 requests<3.0.0,>=2.25.0
 urllib3<2.0.0,>=1.26.5
@@ -22,14 +21,15 @@
 pytest==7.2.1
 scikit-learn>=0.23.2
 setuptools>=47.3.1
 twine<4.0.0,>=3.2.0
 vulture==2.7
 Pint<0.17.0,>=0.16.0
 boto3<2.0.0,>=1.16.34
+certifi>=2022.12.7
 docker<5.0.0,>=4.4.0
 kubernetes<13.0.0,>=12.0.1
 pyOpenSSL>=20.0.0
 xgboost>=1.3.1
 numpy>=1.15.0
 hyperopt>=0.2.7
 sigoptlite>=0.1.1
@@ -39,14 +39,15 @@
 
 [lite]
 sigoptlite>=0.1.1
 
 [orchestrate]
 Pint<0.17.0,>=0.16.0
 boto3<2.0.0,>=1.16.34
+certifi>=2022.12.7
 docker<5.0.0,>=4.4.0
 kubernetes<13.0.0,>=12.0.1
 pyOpenSSL>=20.0.0
 
 [xgboost]
 xgboost>=1.3.1
 numpy>=1.15.0
```

### Comparing `sigopt-8.8.1/test/cli/test_cli_config.py` & `sigopt-8.8.2/test/cli/test_cli_config.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/test/cli/test_cluster_connect.py` & `sigopt-8.8.2/test/cli/test_cluster_connect.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/test/cli/test_cluster_create.py` & `sigopt-8.8.2/test/cli/test_cluster_create.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/test/cli/test_cluster_destroy.py` & `sigopt-8.8.2/test/cli/test_cluster_destroy.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/test/cli/test_cluster_kubectl.py` & `sigopt-8.8.2/test/cli/test_cluster_kubectl.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/test/cli/test_cluster_run.py` & `sigopt-8.8.2/test/cli/test_cluster_run.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/test/cli/test_cluster_test.py` & `sigopt-8.8.2/test/cli/test_cluster_test.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/test/cli/test_init.py` & `sigopt-8.8.2/test/cli/test_init.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/test/cli/test_optimize.py` & `sigopt-8.8.2/test/cli/test_optimize.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/test/cli/test_run.py` & `sigopt-8.8.2/test/cli/test_run.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/test/cli/test_start_worker.py` & `sigopt-8.8.2/test/cli/test_start_worker.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/test/cli/test_truncate.py` & `sigopt-8.8.2/test/cli/test_truncate.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/test/client/test_endpoint.py` & `sigopt-8.8.2/test/client/test_endpoint.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/test/client/test_interface.py` & `sigopt-8.8.2/test/client/test_interface.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/test/client/test_lib.py` & `sigopt-8.8.2/test/client/test_lib.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/test/client/test_object.py` & `sigopt-8.8.2/test/client/test_object.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/test/client/test_pagination.py` & `sigopt-8.8.2/test/client/test_pagination.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/test/client/test_request_driver.py` & `sigopt-8.8.2/test/client/test_request_driver.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/test/client/test_requestor.py` & `sigopt-8.8.2/test/client/test_requestor.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/test/client/test_resource.py` & `sigopt-8.8.2/test/client/test_resource.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/test/client/test_urllib3_patch.py` & `sigopt-8.8.2/test/client/test_urllib3_patch.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/test/orchestrate/aws/service_test.py` & `sigopt-8.8.2/test/orchestrate/aws/service_test.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/test/orchestrate/cluster/service_test.py` & `sigopt-8.8.2/test/orchestrate/cluster/service_test.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/test/orchestrate/cluster_metadata/service_test.py` & `sigopt-8.8.2/test/orchestrate/cluster_metadata/service_test.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/test/orchestrate/common_test.py` & `sigopt-8.8.2/test/orchestrate/common_test.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/test/orchestrate/docker/service_test.py` & `sigopt-8.8.2/test/orchestrate/docker/service_test.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/test/orchestrate/gpu_options_validator/service_test.py` & `sigopt-8.8.2/test/orchestrate/gpu_options_validator/service_test.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/test/orchestrate/job_runner/service_test.py` & `sigopt-8.8.2/test/orchestrate/job_runner/service_test.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/test/orchestrate/job_status/service_test.py` & `sigopt-8.8.2/test/orchestrate/job_status/service_test.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/test/orchestrate/kubernetes/service_test.py` & `sigopt-8.8.2/test/orchestrate/kubernetes/service_test.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/test/orchestrate/lib/lists_test.py` & `sigopt-8.8.2/test/orchestrate/lib/lists_test.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/test/orchestrate/lib/types_test.py` & `sigopt-8.8.2/test/orchestrate/lib/types_test.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/test/orchestrate/options_validator/service_test.py` & `sigopt-8.8.2/test/orchestrate/options_validator/service_test.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/test/orchestrate/provider/broker_test.py` & `sigopt-8.8.2/test/orchestrate/provider/broker_test.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/test/orchestrate/resource/service_test.py` & `sigopt-8.8.2/test/orchestrate/resource/service_test.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/test/orchestrate/services/aws_provider_bag_test.py` & `sigopt-8.8.2/test/orchestrate/services/aws_provider_bag_test.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/test/orchestrate/sigopt/service_test.py` & `sigopt-8.8.2/test/orchestrate/sigopt/service_test.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/test/runs/test_config.py` & `sigopt-8.8.2/test/runs/test_config.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/test/runs/test_context.py` & `sigopt-8.8.2/test/runs/test_context.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/test/runs/test_defaults.py` & `sigopt-8.8.2/test/runs/test_defaults.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/test/runs/test_factory.py` & `sigopt-8.8.2/test/runs/test_factory.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/test/runs/test_local_run_context.py` & `sigopt-8.8.2/test/runs/test_local_run_context.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/test/runs/test_set_project.py` & `sigopt-8.8.2/test/runs/test_set_project.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/test/runs/test_utils.py` & `sigopt-8.8.2/test/runs/test_utils.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/test/validate/test_validate_experiment.py` & `sigopt-8.8.2/test/validate/test_validate_experiment.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/test/validate/test_validate_run.py` & `sigopt-8.8.2/test/validate/test_validate_run.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/test/xgboost/test_compute_metric.py` & `sigopt-8.8.2/test/xgboost/test_compute_metric.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/test/xgboost/test_experiment_config.py` & `sigopt-8.8.2/test/xgboost/test_experiment_config.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.1/test/xgboost/test_run_options_parsing.py` & `sigopt-8.8.2/test/xgboost/test_run_options_parsing.py`

 * *Files identical despite different names*

