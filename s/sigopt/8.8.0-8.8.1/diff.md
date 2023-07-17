# Comparing `tmp/sigopt-8.8.0.tar.gz` & `tmp/sigopt-8.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigopt-8.8.0.tar", last modified: Thu Mar 30 19:44:55 2023, max compression
+gzip compressed data, was "sigopt-8.8.1.tar", last modified: Mon Jul 17 18:17:28 2023, max compression
```

## Comparing `sigopt-8.8.0.tar` & `sigopt-8.8.1.tar`

### file list

```diff
@@ -1,360 +1,361 @@
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.340712 sigopt-8.8.0/
--rw-r--r--   0 sahowey    (502) staff       (20)     1083 2023-03-14 23:54:42.000000 sigopt-8.8.0/LICENSE
--rw-r--r--   0 sahowey    (502) staff       (20)      109 2023-03-14 23:54:42.000000 sigopt-8.8.0/MANIFEST.in
--rw-r--r--   0 sahowey    (502) staff       (20)      617 2023-03-30 19:44:55.340307 sigopt-8.8.0/PKG-INFO
--rw-r--r--   0 sahowey    (502) staff       (20)     4180 2023-03-14 23:54:42.000000 sigopt-8.8.0/README.md
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.138145 sigopt-8.8.0/integration_test/
--rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-03-14 23:54:42.000000 sigopt-8.8.0/integration_test/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)     1499 2023-03-14 23:54:42.000000 sigopt-8.8.0/integration_test/test_experiment.py
--rw-r--r--   0 sahowey    (502) staff       (20)     4553 2023-03-14 23:54:42.000000 sigopt-8.8.0/integration_test/test_hyperopt.py
--rw-r--r--   0 sahowey    (502) staff       (20)      724 2023-03-14 23:54:42.000000 sigopt-8.8.0/integration_test/test_sigopt.py
--rw-r--r--   0 sahowey    (502) staff       (20)     6665 2023-03-14 23:54:42.000000 sigopt-8.8.0/integration_test/test_xgboost_experiment.py
--rw-r--r--   0 sahowey    (502) staff       (20)    15003 2023-03-14 23:54:42.000000 sigopt-8.8.0/integration_test/test_xgboost_run.py
--rw-r--r--   0 sahowey    (502) staff       (20)       38 2023-03-30 19:44:55.340830 sigopt-8.8.0/setup.cfg
--rw-r--r--   0 sahowey    (502) staff       (20)     2643 2023-03-30 19:07:11.000000 sigopt-8.8.0/setup.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.158111 sigopt-8.8.0/sigopt/
--rw-r--r--   0 sahowey    (502) staff       (20)     2101 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)     2739 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/aiexperiment_context.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.163361 sigopt-8.8.0/sigopt/cli/
--rw-r--r--   0 sahowey    (502) staff       (20)      121 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)      148 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/__main__.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.175138 sigopt-8.8.0/sigopt/cli/arguments/
--rw-r--r--   0 sahowey    (502) staff       (20)      686 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/arguments/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)      396 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/arguments/cluster_filename.py
--rw-r--r--   0 sahowey    (502) staff       (20)      188 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/arguments/cluster_name.py
--rw-r--r--   0 sahowey    (502) staff       (20)      167 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/arguments/commands.py
--rw-r--r--   0 sahowey    (502) staff       (20)      206 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/arguments/dockerfile.py
--rw-r--r--   0 sahowey    (502) staff       (20)      432 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/arguments/experiment_file.py
--rw-r--r--   0 sahowey    (502) staff       (20)      198 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/arguments/experiment_id.py
--rw-r--r--   0 sahowey    (502) staff       (20)      569 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/arguments/identifiers.py
--rw-r--r--   0 sahowey    (502) staff       (20)     1119 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/arguments/load_yaml.py
--rw-r--r--   0 sahowey    (502) staff       (20)     1155 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/arguments/project.py
--rw-r--r--   0 sahowey    (502) staff       (20)      344 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/arguments/provider.py
--rw-r--r--   0 sahowey    (502) staff       (20)      443 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/arguments/run_file.py
--rw-r--r--   0 sahowey    (502) staff       (20)      477 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/arguments/source_file.py
--rw-r--r--   0 sahowey    (502) staff       (20)      317 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/arguments/validate.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.181352 sigopt-8.8.0/sigopt/cli/commands/
--rw-r--r--   0 sahowey    (502) staff       (20)      383 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/commands/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)      508 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/commands/base.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.194923 sigopt-8.8.0/sigopt/cli/commands/cluster/
--rw-r--r--   0 sahowey    (502) staff       (20)      862 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/commands/cluster/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)      530 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/commands/cluster/base.py
--rw-r--r--   0 sahowey    (502) staff       (20)      263 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/commands/cluster/clean.py
--rw-r--r--   0 sahowey    (502) staff       (20)     1053 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/commands/cluster/connect.py
--rw-r--r--   0 sahowey    (502) staff       (20)      569 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/commands/cluster/create.py
--rw-r--r--   0 sahowey    (502) staff       (20)      285 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/commands/cluster/destroy.py
--rw-r--r--   0 sahowey    (502) staff       (20)      304 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/commands/cluster/disconnect.py
--rw-r--r--   0 sahowey    (502) staff       (20)      302 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/commands/cluster/install_plugins.py
--rw-r--r--   0 sahowey    (502) staff       (20)      521 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/commands/cluster/kubectl.py
--rw-r--r--   0 sahowey    (502) staff       (20)      472 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/commands/cluster/not_installed.py
--rw-r--r--   0 sahowey    (502) staff       (20)      767 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/commands/cluster/optimize.py
--rw-r--r--   0 sahowey    (502) staff       (20)      680 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/commands/cluster/run.py
--rw-r--r--   0 sahowey    (502) staff       (20)      622 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/commands/cluster/status.py
--rw-r--r--   0 sahowey    (502) staff       (20)      511 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/commands/cluster/stop.py
--rw-r--r--   0 sahowey    (502) staff       (20)      295 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/commands/cluster/test.py
--rw-r--r--   0 sahowey    (502) staff       (20)      693 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/commands/cluster/test_run.py
--rw-r--r--   0 sahowey    (502) staff       (20)      369 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/commands/cluster/update.py
--rw-r--r--   0 sahowey    (502) staff       (20)     1264 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/commands/config.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.197871 sigopt-8.8.0/sigopt/cli/commands/experiment/
--rw-r--r--   0 sahowey    (502) staff       (20)      210 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/commands/experiment/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)      686 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/commands/experiment/archive.py
--rw-r--r--   0 sahowey    (502) staff       (20)      951 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/commands/experiment/create.py
--rw-r--r--   0 sahowey    (502) staff       (20)      685 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/commands/experiment/unarchive.py
--rw-r--r--   0 sahowey    (502) staff       (20)      985 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/commands/init.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.200991 sigopt-8.8.0/sigopt/cli/commands/local/
--rw-r--r--   0 sahowey    (502) staff       (20)      196 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/commands/local/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)      800 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/commands/local/optimize.py
--rw-r--r--   0 sahowey    (502) staff       (20)      746 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/commands/local/run.py
--rw-r--r--   0 sahowey    (502) staff       (20)      902 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/commands/local/start_worker.py
--rw-r--r--   0 sahowey    (502) staff       (20)      245 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/commands/optimize_base.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.202929 sigopt-8.8.0/sigopt/cli/commands/project/
--rw-r--r--   0 sahowey    (502) staff       (20)      113 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/commands/project/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)      849 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/commands/project/create.py
--rw-r--r--   0 sahowey    (502) staff       (20)      739 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/commands/run_base.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.205585 sigopt-8.8.0/sigopt/cli/commands/training_run/
--rw-r--r--   0 sahowey    (502) staff       (20)      169 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/commands/training_run/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)      603 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/commands/training_run/archive.py
--rw-r--r--   0 sahowey    (502) staff       (20)      612 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/commands/training_run/unarchive.py
--rw-r--r--   0 sahowey    (502) staff       (20)      235 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/commands/version.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.209021 sigopt-8.8.0/sigopt/cli/resources/
--rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/resources/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)      668 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/resources/init_dockerfile.txt
--rw-r--r--   0 sahowey    (502) staff       (20)       34 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/resources/init_dockerignore.txt
--rw-r--r--   0 sahowey    (502) staff       (20)      208 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/resources/init_experiment.txt
--rw-r--r--   0 sahowey    (502) staff       (20)       83 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/resources/init_run.txt
--rw-r--r--   0 sahowey    (502) staff       (20)     4867 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/cli/utils.py
--rw-r--r--   0 sahowey    (502) staff       (20)      364 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/compat.py
--rw-r--r--   0 sahowey    (502) staff       (20)     3211 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/config.py
--rw-r--r--   0 sahowey    (502) staff       (20)     1852 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/defaults.py
--rw-r--r--   0 sahowey    (502) staff       (20)     1136 2023-03-29 21:49:12.000000 sigopt-8.8.0/sigopt/endpoint.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.210325 sigopt-8.8.0/sigopt/examples/
--rw-r--r--   0 sahowey    (502) staff       (20)       93 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/examples/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)      860 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/examples/franke.py
--rw-r--r--   0 sahowey    (502) staff       (20)     2120 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/exception.py
--rw-r--r--   0 sahowey    (502) staff       (20)     5706 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/factory.py
--rw-r--r--   0 sahowey    (502) staff       (20)     3919 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/file_utils.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.212129 sigopt-8.8.0/sigopt/hyperopt/
--rw-r--r--   0 sahowey    (502) staff       (20)      117 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/hyperopt/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)     3415 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/hyperopt/base.py
--rw-r--r--   0 sahowey    (502) staff       (20)      714 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/hyperopt/compat.py
--rw-r--r--   0 sahowey    (502) staff       (20)    10860 2023-03-29 21:49:12.000000 sigopt-8.8.0/sigopt/interface.py
--rw-r--r--   0 sahowey    (502) staff       (20)     2106 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/lib.py
--rw-r--r--   0 sahowey    (502) staff       (20)     1315 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/local_run_context.py
--rw-r--r--   0 sahowey    (502) staff       (20)     2857 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/log_capture.py
--rw-r--r--   0 sahowey    (502) staff       (20)     4275 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/magics.py
--rw-r--r--   0 sahowey    (502) staff       (20)      244 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/model_aware_run.py
--rw-r--r--   0 sahowey    (502) staff       (20)    15135 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/objects.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.220282 sigopt-8.8.0/sigopt/orchestrate/
--rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/__init__.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.222206 sigopt-8.8.0/sigopt/orchestrate/aws/
--rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/aws/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)    14083 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/aws/service.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.227594 sigopt-8.8.0/sigopt/orchestrate/cloudformation/
--rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/cloudformation/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)     3115 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/cloudformation/cluster-autoscaler-role.yaml
--rw-r--r--   0 sahowey    (502) staff       (20)    11164 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/cloudformation/eks-cluster.yaml
--rw-r--r--   0 sahowey    (502) staff       (20)     5054 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/cloudformation/eks-node-security.yaml
--rw-r--r--   0 sahowey    (502) staff       (20)    12952 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/cloudformation/eks-nodegroup.yaml
--rw-r--r--   0 sahowey    (502) staff       (20)     6702 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/cloudformation/eks-vpc.yaml
--rw-r--r--   0 sahowey    (502) staff       (20)    17544 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/cloudformation/service.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.232202 sigopt-8.8.0/sigopt/orchestrate/cluster/
--rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/cluster/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)      550 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/cluster/context.py
--rw-r--r--   0 sahowey    (502) staff       (20)     1397 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/cluster/errors.py
--rw-r--r--   0 sahowey    (502) staff       (20)     2438 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/cluster/object.py
--rw-r--r--   0 sahowey    (502) staff       (20)     5659 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/cluster/service.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.238481 sigopt-8.8.0/sigopt/orchestrate/cluster_metadata/
--rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/cluster_metadata/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)      841 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/cluster_metadata/errors.py
--rw-r--r--   0 sahowey    (502) staff       (20)     2016 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/cluster_metadata/service.py
--rw-r--r--   0 sahowey    (502) staff       (20)     1194 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/common.py
--rw-r--r--   0 sahowey    (502) staff       (20)    18498 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/controller.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.241356 sigopt-8.8.0/sigopt/orchestrate/custom_cluster/
--rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/custom_cluster/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)     2238 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/custom_cluster/service.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.242328 sigopt-8.8.0/sigopt/orchestrate/docker/
--rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/docker/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)     6360 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/docker/service.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.243220 sigopt-8.8.0/sigopt/orchestrate/ec2/
--rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/ec2/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)     2580 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/ec2/service.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.248883 sigopt-8.8.0/sigopt/orchestrate/ecr/
--rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/ecr/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)     1044 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/ecr/service.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.251658 sigopt-8.8.0/sigopt/orchestrate/eks/
--rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/eks/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)      215 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/eks/kubeconfig.yml
--rw-r--r--   0 sahowey    (502) staff       (20)      577 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/eks/service.py
--rw-r--r--   0 sahowey    (502) staff       (20)     1790 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/exceptions.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.253999 sigopt-8.8.0/sigopt/orchestrate/gpu_options_validator/
--rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/gpu_options_validator/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)      503 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/gpu_options_validator/service.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.256823 sigopt-8.8.0/sigopt/orchestrate/iam/
--rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/iam/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)     3230 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/iam/service.py
--rw-r--r--   0 sahowey    (502) staff       (20)     2773 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/identifier.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.258989 sigopt-8.8.0/sigopt/orchestrate/job_runner/
--rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/job_runner/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)     7593 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/job_runner/service.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.260025 sigopt-8.8.0/sigopt/orchestrate/job_status/
--rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/job_status/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)     2255 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/job_status/service.py
--rw-r--r--   0 sahowey    (502) staff       (20)      831 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/json_stream.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.263357 sigopt-8.8.0/sigopt/orchestrate/kubectl/
--rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/kubectl/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)      779 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/kubectl/service.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.264848 sigopt-8.8.0/sigopt/orchestrate/kubernetes/
--rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/kubernetes/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)     1022 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/kubernetes/http_proxy.py
--rw-r--r--   0 sahowey    (502) staff       (20)    22742 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/kubernetes/service.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.268308 sigopt-8.8.0/sigopt/orchestrate/lib/
--rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/lib/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)     1382 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/lib/lists.py
--rw-r--r--   0 sahowey    (502) staff       (20)     1134 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/lib/types.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.269736 sigopt-8.8.0/sigopt/orchestrate/logging/
--rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/logging/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)      682 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/logging/service.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.270669 sigopt-8.8.0/sigopt/orchestrate/model_packer/
--rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/model_packer/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)     3397 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/model_packer/service.py
--rw-r--r--   0 sahowey    (502) staff       (20)      261 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/node_groups.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.271981 sigopt-8.8.0/sigopt/orchestrate/options_validator/
--rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/options_validator/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)     4696 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/options_validator/service.py
--rw-r--r--   0 sahowey    (502) staff       (20)     3763 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/paths.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.274942 sigopt-8.8.0/sigopt/orchestrate/plugins/
--rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/plugins/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)     4965 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/plugins/autoscaler-plugin-template.yml
--rw-r--r--   0 sahowey    (502) staff       (20)      200 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/plugins/docker-service.yml
--rw-r--r--   0 sahowey    (502) staff       (20)     1699 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/plugins/docker-statefulset.yml
--rw-r--r--   0 sahowey    (502) staff       (20)      800 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/plugins/orchestrate-controller-roles.yml
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.277188 sigopt-8.8.0/sigopt/orchestrate/provider/
--rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/provider/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)      610 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/provider/broker.py
--rw-r--r--   0 sahowey    (502) staff       (20)     1131 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/provider/constants.py
--rw-r--r--   0 sahowey    (502) staff       (20)      604 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/provider/interface.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.278116 sigopt-8.8.0/sigopt/orchestrate/resource/
--rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/resource/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)      887 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/resource/service.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.279073 sigopt-8.8.0/sigopt/orchestrate/s3/
--rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/s3/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)     2380 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/s3/service.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.282474 sigopt-8.8.0/sigopt/orchestrate/services/
--rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/services/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)      297 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/services/aws_base.py
--rw-r--r--   0 sahowey    (502) staff       (20)     1144 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/services/aws_provider_bag.py
--rw-r--r--   0 sahowey    (502) staff       (20)      536 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/services/bag.py
--rw-r--r--   0 sahowey    (502) staff       (20)      198 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/services/base.py
--rw-r--r--   0 sahowey    (502) staff       (20)     1685 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/services/orchestrate_bag.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.283435 sigopt-8.8.0/sigopt/orchestrate/sigopt/
--rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/sigopt/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)     3040 2023-03-29 21:49:12.000000 sigopt-8.8.0/sigopt/orchestrate/sigopt/service.py
--rw-r--r--   0 sahowey    (502) staff       (20)     4569 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/status.py
--rw-r--r--   0 sahowey    (502) staff       (20)     1077 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/stop.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.284397 sigopt-8.8.0/sigopt/orchestrate/sts/
--rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/sts/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)      595 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/sts/service.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.285341 sigopt-8.8.0/sigopt/orchestrate/test/
--rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/test/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)       54 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/test/test_file.txt
--rw-r--r--   0 sahowey    (502) staff       (20)      263 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/version.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.285970 sigopt-8.8.0/sigopt/orchestrate/zigopt/
--rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/orchestrate/zigopt/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)      566 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/paths.py
--rw-r--r--   0 sahowey    (502) staff       (20)      667 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/ratelimit.py
--rw-r--r--   0 sahowey    (502) staff       (20)     5434 2023-03-29 21:49:12.000000 sigopt-8.8.0/sigopt/request_driver.py
--rw-r--r--   0 sahowey    (502) staff       (20)     2185 2023-03-29 21:49:12.000000 sigopt-8.8.0/sigopt/resource.py
--rw-r--r--   0 sahowey    (502) staff       (20)    15336 2023-03-29 21:49:12.000000 sigopt-8.8.0/sigopt/run_context.py
--rw-r--r--   0 sahowey    (502) staff       (20)      738 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/run_factory.py
--rw-r--r--   0 sahowey    (502) staff       (20)     4513 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/run_params.py
--rw-r--r--   0 sahowey    (502) staff       (20)      408 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/sigopt_logging.py
--rw-r--r--   0 sahowey    (502) staff       (20)     1700 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/urllib3_patch.py
--rw-r--r--   0 sahowey    (502) staff       (20)      572 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/utils.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.289344 sigopt-8.8.0/sigopt/validate/
--rw-r--r--   0 sahowey    (502) staff       (20)      257 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/validate/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)     6963 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/validate/aiexperiment_input.py
--rw-r--r--   0 sahowey    (502) staff       (20)      333 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/validate/common.py
--rw-r--r--   0 sahowey    (502) staff       (20)      112 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/validate/exceptions.py
--rw-r--r--   0 sahowey    (502) staff       (20)       95 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/validate/keys.py
--rw-r--r--   0 sahowey    (502) staff       (20)     1721 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/validate/run_input.py
--rw-r--r--   0 sahowey    (502) staff       (20)       89 2023-03-30 19:07:11.000000 sigopt-8.8.0/sigopt/version.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.294176 sigopt-8.8.0/sigopt/xgboost/
--rw-r--r--   0 sahowey    (502) staff       (20)      127 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/xgboost/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)     1084 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/xgboost/checkpoint_callback.py
--rw-r--r--   0 sahowey    (502) staff       (20)      685 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/xgboost/compat.py
--rw-r--r--   0 sahowey    (502) staff       (20)     3040 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/xgboost/compute_metrics.py
--rw-r--r--   0 sahowey    (502) staff       (20)     4053 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/xgboost/constants.py
--rw-r--r--   0 sahowey    (502) staff       (20)    10027 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/xgboost/experiment.py
--rw-r--r--   0 sahowey    (502) staff       (20)    12749 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/xgboost/run.py
--rw-r--r--   0 sahowey    (502) staff       (20)      942 2023-03-14 23:54:42.000000 sigopt-8.8.0/sigopt/xgboost/utils.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.160988 sigopt-8.8.0/sigopt.egg-info/
--rw-r--r--   0 sahowey    (502) staff       (20)      617 2023-03-30 19:44:54.000000 sigopt-8.8.0/sigopt.egg-info/PKG-INFO
--rw-r--r--   0 sahowey    (502) staff       (20)     9880 2023-03-30 19:44:55.000000 sigopt-8.8.0/sigopt.egg-info/SOURCES.txt
--rw-r--r--   0 sahowey    (502) staff       (20)        1 2023-03-30 19:44:54.000000 sigopt-8.8.0/sigopt.egg-info/dependency_links.txt
--rw-r--r--   0 sahowey    (502) staff       (20)       58 2023-03-30 19:44:54.000000 sigopt-8.8.0/sigopt.egg-info/entry_points.txt
--rw-r--r--   0 sahowey    (502) staff       (20)      641 2023-03-30 19:44:54.000000 sigopt-8.8.0/sigopt.egg-info/requires.txt
--rw-r--r--   0 sahowey    (502) staff       (20)       29 2023-03-30 19:44:54.000000 sigopt-8.8.0/sigopt.egg-info/top_level.txt
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.295119 sigopt-8.8.0/test/
--rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/__init__.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.304188 sigopt-8.8.0/test/cli/
--rw-r--r--   0 sahowey    (502) staff       (20)     1236 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/cli/test_cli_config.py
--rw-r--r--   0 sahowey    (502) staff       (20)      517 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/cli/test_cluster_connect.py
--rw-r--r--   0 sahowey    (502) staff       (20)      551 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/cli/test_cluster_create.py
--rw-r--r--   0 sahowey    (502) staff       (20)     1028 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/cli/test_cluster_destroy.py
--rw-r--r--   0 sahowey    (502) staff       (20)      486 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/cli/test_cluster_disconnect.py
--rw-r--r--   0 sahowey    (502) staff       (20)     1393 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/cli/test_cluster_kubectl.py
--rw-r--r--   0 sahowey    (502) staff       (20)      998 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/cli/test_cluster_run.py
--rw-r--r--   0 sahowey    (502) staff       (20)      538 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/cli/test_cluster_test.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.305986 sigopt-8.8.0/test/cli/test_files/
--rw-r--r--   0 sahowey    (502) staff       (20)       90 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/cli/test_files/import_hello.py
--rw-r--r--   0 sahowey    (502) staff       (20)      154 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/cli/test_files/print_args.py
--rw-r--r--   0 sahowey    (502) staff       (20)      125 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/cli/test_files/print_hello.py
--rw-r--r--   0 sahowey    (502) staff       (20)      708 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/cli/test_init.py
--rw-r--r--   0 sahowey    (502) staff       (20)     3185 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/cli/test_optimize.py
--rw-r--r--   0 sahowey    (502) staff       (20)     2437 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/cli/test_run.py
--rw-r--r--   0 sahowey    (502) staff       (20)     2505 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/cli/test_start_worker.py
--rw-r--r--   0 sahowey    (502) staff       (20)      578 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/cli/test_truncate.py
--rw-r--r--   0 sahowey    (502) staff       (20)      382 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/cli/test_version.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.312177 sigopt-8.8.0/test/client/
--rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/client/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)    10122 2023-03-29 21:49:12.000000 sigopt-8.8.0/test/client/test_endpoint.py
--rw-r--r--   0 sahowey    (502) staff       (20)     2849 2023-03-29 21:49:12.000000 sigopt-8.8.0/test/client/test_interface.py
--rw-r--r--   0 sahowey    (502) staff       (20)     4688 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/client/test_lib.py
--rw-r--r--   0 sahowey    (502) staff       (20)    18437 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/client/test_object.py
--rw-r--r--   0 sahowey    (502) staff       (20)     8682 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/client/test_pagination.py
--rw-r--r--   0 sahowey    (502) staff       (20)     3702 2023-03-29 21:49:12.000000 sigopt-8.8.0/test/client/test_request_driver.py
--rw-r--r--   0 sahowey    (502) staff       (20)     3151 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/client/test_requestor.py
--rw-r--r--   0 sahowey    (502) staff       (20)     1621 2023-03-29 21:49:12.000000 sigopt-8.8.0/test/client/test_resource.py
--rw-r--r--   0 sahowey    (502) staff       (20)      785 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/client/test_urllib3_patch.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.313245 sigopt-8.8.0/test/orchestrate/
--rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/orchestrate/__init__.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.314165 sigopt-8.8.0/test/orchestrate/aws/
--rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/orchestrate/aws/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)     2776 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/orchestrate/aws/service_test.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.315050 sigopt-8.8.0/test/orchestrate/cluster/
--rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/orchestrate/cluster/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)     8072 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/orchestrate/cluster/service_test.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.316022 sigopt-8.8.0/test/orchestrate/cluster_metadata/
--rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/orchestrate/cluster_metadata/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)     3062 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/orchestrate/cluster_metadata/service_test.py
--rw-r--r--   0 sahowey    (502) staff       (20)      831 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/orchestrate/common_test.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.316998 sigopt-8.8.0/test/orchestrate/docker/
--rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/orchestrate/docker/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)     1767 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/orchestrate/docker/service_test.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.317978 sigopt-8.8.0/test/orchestrate/ecr/
--rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/orchestrate/ecr/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)      510 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/orchestrate/ecr/service_test.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.318940 sigopt-8.8.0/test/orchestrate/gpu_options_validator/
--rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/orchestrate/gpu_options_validator/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)     1115 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/orchestrate/gpu_options_validator/service_test.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.319913 sigopt-8.8.0/test/orchestrate/job_runner/
--rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/orchestrate/job_runner/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)     1890 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/orchestrate/job_runner/service_test.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.320895 sigopt-8.8.0/test/orchestrate/job_status/
--rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/orchestrate/job_status/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)     1860 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/orchestrate/job_status/service_test.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.322070 sigopt-8.8.0/test/orchestrate/kubernetes/
--rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/orchestrate/kubernetes/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)     4812 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/orchestrate/kubernetes/service_test.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.323879 sigopt-8.8.0/test/orchestrate/lib/
--rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/orchestrate/lib/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)     2398 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/orchestrate/lib/lists_test.py
--rw-r--r--   0 sahowey    (502) staff       (20)     4633 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/orchestrate/lib/types_test.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.324710 sigopt-8.8.0/test/orchestrate/model_packer/
--rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/orchestrate/model_packer/__init__.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.325444 sigopt-8.8.0/test/orchestrate/options_validator/
--rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/orchestrate/options_validator/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)     9268 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/orchestrate/options_validator/service_test.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.326617 sigopt-8.8.0/test/orchestrate/provider/
--rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/orchestrate/provider/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)     1382 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/orchestrate/provider/broker_test.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.327587 sigopt-8.8.0/test/orchestrate/resource/
--rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/orchestrate/resource/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)     1141 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/orchestrate/resource/service_test.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.329155 sigopt-8.8.0/test/orchestrate/services/
--rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/orchestrate/services/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)     1131 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/orchestrate/services/aws_provider_bag_test.py
--rw-r--r--   0 sahowey    (502) staff       (20)      309 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/orchestrate/services/base_test.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.329705 sigopt-8.8.0/test/orchestrate/sigopt/
--rw-r--r--   0 sahowey    (502) staff       (20)      652 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/orchestrate/sigopt/service_test.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.330597 sigopt-8.8.0/test/orchestrate/sts/
--rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/orchestrate/sts/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)      510 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/orchestrate/sts/service_test.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.335701 sigopt-8.8.0/test/runs/
--rw-r--r--   0 sahowey    (502) staff       (20)      595 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/runs/test_config.py
--rw-r--r--   0 sahowey    (502) staff       (20)     7011 2023-03-29 21:49:12.000000 sigopt-8.8.0/test/runs/test_context.py
--rw-r--r--   0 sahowey    (502) staff       (20)      554 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/runs/test_defaults.py
--rw-r--r--   0 sahowey    (502) staff       (20)     2514 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/runs/test_factory.py
--rw-r--r--   0 sahowey    (502) staff       (20)     2035 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/runs/test_local_run_context.py
--rw-r--r--   0 sahowey    (502) staff       (20)      622 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/runs/test_set_project.py
--rw-r--r--   0 sahowey    (502) staff       (20)     5209 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/runs/test_utils.py
--rw-r--r--   0 sahowey    (502) staff       (20)      298 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/runs/utils.py
--rw-r--r--   0 sahowey    (502) staff       (20)      298 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/utils.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.336959 sigopt-8.8.0/test/validate/
--rw-r--r--   0 sahowey    (502) staff       (20)     4673 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/validate/test_validate_experiment.py
--rw-r--r--   0 sahowey    (502) staff       (20)     1924 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/validate/test_validate_run.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-30 19:44:55.339454 sigopt-8.8.0/test/xgboost/
--rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/xgboost/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)     5028 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/xgboost/test_compute_metric.py
--rw-r--r--   0 sahowey    (502) staff       (20)     9164 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/xgboost/test_experiment_config.py
--rw-r--r--   0 sahowey    (502) staff       (20)     3318 2023-03-14 23:54:42.000000 sigopt-8.8.0/test/xgboost/test_run_options_parsing.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.979595 sigopt-8.8.1/
+-rw-r--r--   0 tjackles   (503) staff       (20)     1083 2022-02-18 18:21:31.000000 sigopt-8.8.1/LICENSE
+-rw-r--r--   0 tjackles   (503) staff       (20)      109 2021-10-21 13:30:45.000000 sigopt-8.8.1/MANIFEST.in
+-rw-r--r--   0 tjackles   (503) staff       (20)      617 2023-07-17 18:17:28.979870 sigopt-8.8.1/PKG-INFO
+-rw-r--r--   0 tjackles   (503) staff       (20)     4491 2023-07-17 17:31:25.000000 sigopt-8.8.1/README.md
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.840422 sigopt-8.8.1/integration_test/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/integration_test/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1405 2023-04-03 19:26:20.000000 sigopt-8.8.1/integration_test/test_experiment.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     4110 2023-06-27 22:27:24.000000 sigopt-8.8.1/integration_test/test_hyperopt.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      723 2023-04-03 19:26:20.000000 sigopt-8.8.1/integration_test/test_sigopt.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     6745 2023-04-03 19:26:20.000000 sigopt-8.8.1/integration_test/test_xgboost_experiment.py
+-rw-r--r--   0 tjackles   (503) staff       (20)    15097 2023-04-03 19:26:20.000000 sigopt-8.8.1/integration_test/test_xgboost_run.py
+-rw-r--r--   0 tjackles   (503) staff       (20)       56 2023-04-03 19:26:20.000000 sigopt-8.8.1/pyproject.toml
+-rw-r--r--   0 tjackles   (503) staff       (20)      391 2023-07-17 18:17:28.980538 sigopt-8.8.1/setup.cfg
+-rw-r--r--   0 tjackles   (503) staff       (20)     2728 2023-04-27 20:20:23.000000 sigopt-8.8.1/setup.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.853043 sigopt-8.8.1/sigopt/
+-rw-r--r--   0 tjackles   (503) staff       (20)     2135 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     2907 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/aiexperiment_context.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.858605 sigopt-8.8.1/sigopt/cli/
+-rw-r--r--   0 tjackles   (503) staff       (20)      121 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/cli/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      148 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/cli/__main__.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.868368 sigopt-8.8.1/sigopt/cli/arguments/
+-rw-r--r--   0 tjackles   (503) staff       (20)      686 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/arguments/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      396 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/arguments/cluster_filename.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      188 2023-04-03 17:57:25.000000 sigopt-8.8.1/sigopt/cli/arguments/cluster_name.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      167 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/arguments/commands.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      206 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/cli/arguments/dockerfile.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      432 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/arguments/experiment_file.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      200 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/arguments/experiment_id.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      570 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/arguments/identifiers.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1121 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/arguments/load_yaml.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1157 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/arguments/project.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      344 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/cli/arguments/provider.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      443 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/arguments/run_file.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      478 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/arguments/source_file.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      319 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/arguments/validate.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.871141 sigopt-8.8.1/sigopt/cli/commands/
+-rw-r--r--   0 tjackles   (503) staff       (20)      383 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      510 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/base.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.878359 sigopt-8.8.1/sigopt/cli/commands/cluster/
+-rw-r--r--   0 tjackles   (503) staff       (20)      862 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/cli/commands/cluster/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      531 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/cluster/base.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      263 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/cluster/clean.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1053 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/cluster/connect.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      569 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/cluster/create.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      285 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/cluster/destroy.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      304 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/cluster/disconnect.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      302 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/cluster/install_plugins.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      521 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/cluster/kubectl.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      485 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/cluster/not_installed.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      777 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/cluster/optimize.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      690 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/cluster/run.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      622 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/cluster/status.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      511 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/cluster/stop.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      295 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/cluster/test.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      706 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/cluster/test_run.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      369 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/cluster/update.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1282 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/config.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.879859 sigopt-8.8.1/sigopt/cli/commands/experiment/
+-rw-r--r--   0 tjackles   (503) staff       (20)      210 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/experiment/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      688 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/experiment/archive.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      952 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/experiment/create.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      687 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/experiment/unarchive.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      986 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/init.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.881480 sigopt-8.8.1/sigopt/cli/commands/local/
+-rw-r--r--   0 tjackles   (503) staff       (20)      196 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/cli/commands/local/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      810 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/local/optimize.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      756 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/local/run.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      912 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/local/start_worker.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      244 2023-04-03 19:57:41.000000 sigopt-8.8.1/sigopt/cli/commands/optimize_base.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.882262 sigopt-8.8.1/sigopt/cli/commands/project/
+-rw-r--r--   0 tjackles   (503) staff       (20)      113 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/cli/commands/project/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      850 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/project/create.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      738 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/run_base.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.883428 sigopt-8.8.1/sigopt/cli/commands/training_run/
+-rw-r--r--   0 tjackles   (503) staff       (20)      169 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/cli/commands/training_run/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      605 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/training_run/archive.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      615 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/training_run/unarchive.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      235 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/commands/version.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.885448 sigopt-8.8.1/sigopt/cli/resources/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/cli/resources/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      668 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/cli/resources/init_dockerfile.txt
+-rw-r--r--   0 tjackles   (503) staff       (20)       34 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/cli/resources/init_dockerignore.txt
+-rw-r--r--   0 tjackles   (503) staff       (20)      208 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/cli/resources/init_experiment.txt
+-rw-r--r--   0 tjackles   (503) staff       (20)       83 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/cli/resources/init_run.txt
+-rw-r--r--   0 tjackles   (503) staff       (20)     4897 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/cli/utils.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      355 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/compat.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     3231 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/config.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1867 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/defaults.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1137 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/endpoint.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.886235 sigopt-8.8.1/sigopt/examples/
+-rw-r--r--   0 tjackles   (503) staff       (20)       93 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/examples/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      874 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/examples/franke.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     2117 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/exception.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     5792 2023-04-10 20:37:54.000000 sigopt-8.8.1/sigopt/factory.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     3982 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/file_utils.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.887366 sigopt-8.8.1/sigopt/hyperopt/
+-rw-r--r--   0 tjackles   (503) staff       (20)      117 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/hyperopt/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     3401 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/hyperopt/base.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      715 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/hyperopt/compat.py
+-rw-r--r--   0 tjackles   (503) staff       (20)    10837 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/interface.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     2141 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/lib.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1317 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/local_run_context.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     2824 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/log_capture.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     4298 2023-04-27 20:20:23.000000 sigopt-8.8.1/sigopt/magics.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      245 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/model_aware_run.py
+-rw-r--r--   0 tjackles   (503) staff       (20)    15123 2023-04-27 20:20:23.000000 sigopt-8.8.1/sigopt/objects.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.891562 sigopt-8.8.1/sigopt/orchestrate/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/__init__.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.892285 sigopt-8.8.1/sigopt/orchestrate/aws/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/aws/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)    14083 2023-04-27 20:20:23.000000 sigopt-8.8.1/sigopt/orchestrate/aws/service.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.895158 sigopt-8.8.1/sigopt/orchestrate/cloudformation/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/cloudformation/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     3115 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/cloudformation/cluster-autoscaler-role.yaml
+-rw-r--r--   0 tjackles   (503) staff       (20)    11164 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/cloudformation/eks-cluster.yaml
+-rw-r--r--   0 tjackles   (503) staff       (20)     5054 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/cloudformation/eks-node-security.yaml
+-rw-r--r--   0 tjackles   (503) staff       (20)    12952 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/cloudformation/eks-nodegroup.yaml
+-rw-r--r--   0 tjackles   (503) staff       (20)     6702 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/cloudformation/eks-vpc.yaml
+-rw-r--r--   0 tjackles   (503) staff       (20)    17520 2023-04-27 20:20:23.000000 sigopt-8.8.1/sigopt/orchestrate/cloudformation/service.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.897238 sigopt-8.8.1/sigopt/orchestrate/cluster/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/cluster/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      550 2023-04-03 17:57:26.000000 sigopt-8.8.1/sigopt/orchestrate/cluster/context.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1407 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/orchestrate/cluster/errors.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     2440 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/orchestrate/cluster/object.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     5623 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/orchestrate/cluster/service.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.898294 sigopt-8.8.1/sigopt/orchestrate/cluster_metadata/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/cluster_metadata/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      841 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/orchestrate/cluster_metadata/errors.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     2017 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/orchestrate/cluster_metadata/service.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1196 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/orchestrate/common.py
+-rw-r--r--   0 tjackles   (503) staff       (20)    18441 2023-04-27 20:20:23.000000 sigopt-8.8.1/sigopt/orchestrate/controller.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.899322 sigopt-8.8.1/sigopt/orchestrate/custom_cluster/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/custom_cluster/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     2267 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/orchestrate/custom_cluster/service.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.900523 sigopt-8.8.1/sigopt/orchestrate/docker/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/docker/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     6402 2023-04-27 20:20:23.000000 sigopt-8.8.1/sigopt/orchestrate/docker/service.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.901709 sigopt-8.8.1/sigopt/orchestrate/ec2/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/ec2/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     2570 2023-04-27 20:20:23.000000 sigopt-8.8.1/sigopt/orchestrate/ec2/service.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.903026 sigopt-8.8.1/sigopt/orchestrate/ecr/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/ecr/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1044 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/orchestrate/ecr/service.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.904922 sigopt-8.8.1/sigopt/orchestrate/eks/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/eks/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      215 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/eks/kubeconfig.yml
+-rw-r--r--   0 tjackles   (503) staff       (20)      577 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/orchestrate/eks/service.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1818 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/orchestrate/exceptions.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.906260 sigopt-8.8.1/sigopt/orchestrate/gpu_options_validator/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/gpu_options_validator/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      504 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/orchestrate/gpu_options_validator/service.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.907534 sigopt-8.8.1/sigopt/orchestrate/iam/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/iam/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     3230 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/orchestrate/iam/service.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     2792 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/orchestrate/identifier.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.908759 sigopt-8.8.1/sigopt/orchestrate/job_runner/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/job_runner/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     7853 2023-04-27 20:20:23.000000 sigopt-8.8.1/sigopt/orchestrate/job_runner/service.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.910102 sigopt-8.8.1/sigopt/orchestrate/job_status/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/job_status/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     2214 2023-04-27 20:20:23.000000 sigopt-8.8.1/sigopt/orchestrate/job_status/service.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      800 2023-04-27 20:20:23.000000 sigopt-8.8.1/sigopt/orchestrate/json_stream.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.911519 sigopt-8.8.1/sigopt/orchestrate/kubectl/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/kubectl/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      797 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/orchestrate/kubectl/service.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.913492 sigopt-8.8.1/sigopt/orchestrate/kubernetes/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/kubernetes/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1014 2023-04-27 20:20:23.000000 sigopt-8.8.1/sigopt/orchestrate/kubernetes/http_proxy.py
+-rw-r--r--   0 tjackles   (503) staff       (20)    22925 2023-04-27 20:20:23.000000 sigopt-8.8.1/sigopt/orchestrate/kubernetes/service.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.915384 sigopt-8.8.1/sigopt/orchestrate/lib/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/lib/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1402 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/orchestrate/lib/lists.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1168 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/orchestrate/lib/types.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.916539 sigopt-8.8.1/sigopt/orchestrate/logging/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/logging/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      682 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/orchestrate/logging/service.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.918174 sigopt-8.8.1/sigopt/orchestrate/model_packer/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/model_packer/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     3393 2023-04-27 20:20:23.000000 sigopt-8.8.1/sigopt/orchestrate/model_packer/service.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      261 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/node_groups.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.919525 sigopt-8.8.1/sigopt/orchestrate/options_validator/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/options_validator/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     4606 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/orchestrate/options_validator/service.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     3710 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/orchestrate/paths.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.921961 sigopt-8.8.1/sigopt/orchestrate/plugins/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/plugins/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     4965 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/plugins/autoscaler-plugin-template.yml
+-rw-r--r--   0 tjackles   (503) staff       (20)      200 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/plugins/docker-service.yml
+-rw-r--r--   0 tjackles   (503) staff       (20)     1699 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/plugins/docker-statefulset.yml
+-rw-r--r--   0 tjackles   (503) staff       (20)      800 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/plugins/orchestrate-controller-roles.yml
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.923981 sigopt-8.8.1/sigopt/orchestrate/provider/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/provider/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      610 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/provider/broker.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1120 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/orchestrate/provider/constants.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      604 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/provider/interface.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.924839 sigopt-8.8.1/sigopt/orchestrate/resource/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/resource/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      887 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/orchestrate/resource/service.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.925688 sigopt-8.8.1/sigopt/orchestrate/s3/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/s3/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     2373 2023-04-27 20:20:23.000000 sigopt-8.8.1/sigopt/orchestrate/s3/service.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.928528 sigopt-8.8.1/sigopt/orchestrate/services/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/services/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      302 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/orchestrate/services/aws_base.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1144 2023-04-03 17:57:26.000000 sigopt-8.8.1/sigopt/orchestrate/services/aws_provider_bag.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      547 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/orchestrate/services/bag.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      203 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/orchestrate/services/base.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1685 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/services/orchestrate_bag.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.929324 sigopt-8.8.1/sigopt/orchestrate/sigopt/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/sigopt/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     2995 2023-04-27 20:20:23.000000 sigopt-8.8.1/sigopt/orchestrate/sigopt/service.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     4504 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/orchestrate/status.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1078 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/orchestrate/stop.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.930077 sigopt-8.8.1/sigopt/orchestrate/sts/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/sts/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      595 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/orchestrate/sts/service.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.930775 sigopt-8.8.1/sigopt/orchestrate/test/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/test/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)       54 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/test/test_file.txt
+-rw-r--r--   0 tjackles   (503) staff       (20)      263 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/orchestrate/version.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.931143 sigopt-8.8.1/sigopt/orchestrate/zigopt/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/orchestrate/zigopt/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      570 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/paths.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      666 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/ratelimit.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     5429 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/request_driver.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     2148 2023-04-27 20:20:23.000000 sigopt-8.8.1/sigopt/resource.py
+-rw-r--r--   0 tjackles   (503) staff       (20)    15648 2023-04-27 20:20:23.000000 sigopt-8.8.1/sigopt/run_context.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      757 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/run_factory.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     4514 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/run_params.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      410 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/sigopt_logging.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1713 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/urllib3_patch.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      577 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/utils.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.933846 sigopt-8.8.1/sigopt/validate/
+-rw-r--r--   0 tjackles   (503) staff       (20)      257 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/validate/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     6950 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/validate/aiexperiment_input.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      333 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/validate/common.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      112 2023-03-14 22:13:41.000000 sigopt-8.8.1/sigopt/validate/exceptions.py
+-rw-r--r--   0 tjackles   (503) staff       (20)       95 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/validate/keys.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1721 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/validate/run_input.py
+-rw-r--r--   0 tjackles   (503) staff       (20)       89 2023-07-17 18:13:21.000000 sigopt-8.8.1/sigopt/version.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.937656 sigopt-8.8.1/sigopt/xgboost/
+-rw-r--r--   0 tjackles   (503) staff       (20)      127 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/xgboost/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1085 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/xgboost/checkpoint_callback.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      693 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/xgboost/compat.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     3037 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/xgboost/compute_metrics.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     3913 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/xgboost/constants.py
+-rw-r--r--   0 tjackles   (503) staff       (20)    10142 2023-04-03 19:57:41.000000 sigopt-8.8.1/sigopt/xgboost/experiment.py
+-rw-r--r--   0 tjackles   (503) staff       (20)    12660 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/xgboost/run.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      942 2023-04-03 19:26:20.000000 sigopt-8.8.1/sigopt/xgboost/utils.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.856768 sigopt-8.8.1/sigopt.egg-info/
+-rw-r--r--   0 tjackles   (503) staff       (20)      617 2023-07-17 18:17:28.000000 sigopt-8.8.1/sigopt.egg-info/PKG-INFO
+-rw-r--r--   0 tjackles   (503) staff       (20)     9905 2023-07-17 18:17:28.000000 sigopt-8.8.1/sigopt.egg-info/SOURCES.txt
+-rw-r--r--   0 tjackles   (503) staff       (20)        1 2023-07-17 18:17:28.000000 sigopt-8.8.1/sigopt.egg-info/dependency_links.txt
+-rw-r--r--   0 tjackles   (503) staff       (20)       58 2023-07-17 18:17:28.000000 sigopt-8.8.1/sigopt.egg-info/entry_points.txt
+-rw-r--r--   0 tjackles   (503) staff       (20)      784 2023-07-17 18:17:28.000000 sigopt-8.8.1/sigopt.egg-info/requires.txt
+-rw-r--r--   0 tjackles   (503) staff       (20)       29 2023-07-17 18:17:28.000000 sigopt-8.8.1/sigopt.egg-info/top_level.txt
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.938460 sigopt-8.8.1/test/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/test/__init__.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.945296 sigopt-8.8.1/test/cli/
+-rw-r--r--   0 tjackles   (503) staff       (20)     1294 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/cli/test_cli_config.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      517 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/cli/test_cluster_connect.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      547 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/cli/test_cluster_create.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1028 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/cli/test_cluster_destroy.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      486 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/cli/test_cluster_disconnect.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1426 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/cli/test_cluster_kubectl.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      939 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/cli/test_cluster_run.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      534 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/cli/test_cluster_test.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.946767 sigopt-8.8.1/test/cli/test_files/
+-rw-r--r--   0 tjackles   (503) staff       (20)      123 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/cli/test_files/import_hello.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      157 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/cli/test_files/print_args.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      126 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/cli/test_files/print_hello.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      708 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/cli/test_init.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     3311 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/cli/test_optimize.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     2566 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/cli/test_run.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     2590 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/cli/test_start_worker.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      578 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/cli/test_truncate.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      382 2023-03-14 22:13:41.000000 sigopt-8.8.1/test/cli/test_version.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.952078 sigopt-8.8.1/test/client/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/test/client/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)    10389 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/client/test_endpoint.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     2851 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/client/test_interface.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     4687 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/client/test_lib.py
+-rw-r--r--   0 tjackles   (503) staff       (20)    18457 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/client/test_object.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     9440 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/client/test_pagination.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     3702 2023-03-17 22:29:13.000000 sigopt-8.8.1/test/client/test_request_driver.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     3154 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/client/test_requestor.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1641 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/client/test_resource.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      787 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/client/test_urllib3_patch.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.953359 sigopt-8.8.1/test/orchestrate/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/test/orchestrate/__init__.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.954578 sigopt-8.8.1/test/orchestrate/aws/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/test/orchestrate/aws/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     2862 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/orchestrate/aws/service_test.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.955895 sigopt-8.8.1/test/orchestrate/cluster/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/test/orchestrate/cluster/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     8090 2023-04-27 20:20:23.000000 sigopt-8.8.1/test/orchestrate/cluster/service_test.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.957450 sigopt-8.8.1/test/orchestrate/cluster_metadata/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/test/orchestrate/cluster_metadata/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     3062 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/orchestrate/cluster_metadata/service_test.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      831 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/orchestrate/common_test.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.958739 sigopt-8.8.1/test/orchestrate/docker/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/test/orchestrate/docker/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1767 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/orchestrate/docker/service_test.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.960033 sigopt-8.8.1/test/orchestrate/ecr/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/test/orchestrate/ecr/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      510 2023-03-14 22:13:41.000000 sigopt-8.8.1/test/orchestrate/ecr/service_test.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.961416 sigopt-8.8.1/test/orchestrate/gpu_options_validator/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/test/orchestrate/gpu_options_validator/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1115 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/orchestrate/gpu_options_validator/service_test.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.962990 sigopt-8.8.1/test/orchestrate/job_runner/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/test/orchestrate/job_runner/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     2084 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/orchestrate/job_runner/service_test.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.963872 sigopt-8.8.1/test/orchestrate/job_status/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/test/orchestrate/job_status/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1914 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/orchestrate/job_status/service_test.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.964857 sigopt-8.8.1/test/orchestrate/kubernetes/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/test/orchestrate/kubernetes/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     4812 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/orchestrate/kubernetes/service_test.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.967130 sigopt-8.8.1/test/orchestrate/lib/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/test/orchestrate/lib/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     2347 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/orchestrate/lib/lists_test.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     4633 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/orchestrate/lib/types_test.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.967800 sigopt-8.8.1/test/orchestrate/model_packer/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/test/orchestrate/model_packer/__init__.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.968942 sigopt-8.8.1/test/orchestrate/options_validator/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/test/orchestrate/options_validator/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     9367 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/orchestrate/options_validator/service_test.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.970039 sigopt-8.8.1/test/orchestrate/provider/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/test/orchestrate/provider/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1401 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/orchestrate/provider/broker_test.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.970801 sigopt-8.8.1/test/orchestrate/resource/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/test/orchestrate/resource/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1142 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/orchestrate/resource/service_test.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.972241 sigopt-8.8.1/test/orchestrate/services/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/test/orchestrate/services/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     1131 2023-03-14 22:13:41.000000 sigopt-8.8.1/test/orchestrate/services/aws_provider_bag_test.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      309 2023-03-14 22:13:41.000000 sigopt-8.8.1/test/orchestrate/services/base_test.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.972646 sigopt-8.8.1/test/orchestrate/sigopt/
+-rw-r--r--   0 tjackles   (503) staff       (20)      671 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/orchestrate/sigopt/service_test.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.973386 sigopt-8.8.1/test/orchestrate/sts/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/test/orchestrate/sts/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      510 2023-03-14 22:13:41.000000 sigopt-8.8.1/test/orchestrate/sts/service_test.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.976743 sigopt-8.8.1/test/runs/
+-rw-r--r--   0 tjackles   (503) staff       (20)      599 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/runs/test_config.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     6965 2023-04-27 20:20:23.000000 sigopt-8.8.1/test/runs/test_context.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      577 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/runs/test_defaults.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     2414 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/runs/test_factory.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     2123 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/runs/test_local_run_context.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      624 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/runs/test_set_project.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     5199 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/runs/test_utils.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      299 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/runs/utils.py
+-rw-r--r--   0 tjackles   (503) staff       (20)      299 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/utils.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.977506 sigopt-8.8.1/test/validate/
+-rw-r--r--   0 tjackles   (503) staff       (20)     5235 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/validate/test_validate_experiment.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     2009 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/validate/test_validate_run.py
+drwxr-xr-x   0 tjackles   (503) staff       (20)        0 2023-07-17 18:17:28.979246 sigopt-8.8.1/test/xgboost/
+-rw-r--r--   0 tjackles   (503) staff       (20)        0 2023-03-14 22:13:41.000000 sigopt-8.8.1/test/xgboost/__init__.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     5133 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/xgboost/test_compute_metric.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     8974 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/xgboost/test_experiment_config.py
+-rw-r--r--   0 tjackles   (503) staff       (20)     3345 2023-04-03 19:26:20.000000 sigopt-8.8.1/test/xgboost/test_run_options_parsing.py
```

### Comparing `sigopt-8.8.0/LICENSE` & `sigopt-8.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.0/PKG-INFO` & `sigopt-8.8.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigopt
-Version: 8.8.0
+Version: 8.8.1
 Summary: SigOpt Python API Client
 Home-page: https://sigopt.com/
 Author: SigOpt
 Author-email: support@sigopt.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sigopt-8.8.0/README.md` & `sigopt-8.8.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,16 @@
-[![Build Status](https://circleci.com/gh/sigopt/sigopt-python.svg?style=svg)](https://circleci.com/gh/sigopt/sigopt-python)
+<!--
+Copyright © 2023 Intel Corporation
+
+SPDX-License-Identifier: MIT
+-->
+
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sigopt/sigopt-python/main.svg)](https://results.pre-commit.ci/latest/github/sigopt/sigopt-python/main)
+![integration](https://github.com/sigopt/sigopt-python/actions/workflows/integration.yml/badge.svg)
+![tests](https://github.com/sigopt/sigopt-python/actions/workflows/tests.yml/badge.svg)
 
 # SigOpt Python API
 
 This is the [SigOpt](https://sigopt.com) Python API client.
 Use this to natively call SigOpt API endpoints to create experiments and report data.
 
 For more help getting started with SigOpt and Python, check out the [docs](https://docs.sigopt.com/core-module-api-references/get_started).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sigopt-8.8.0/integration_test/test_experiment.py` & `sigopt-8.8.1/integration_test/test_experiment.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,49 +3,37 @@
 # SPDX-License-Identifier: MIT
 import sigopt
 
 
 class TestExperiment(object):
   def test_update(self):
     parameters = [
-      {
-        'name': 'max_depth',
-        'type': 'int',
-        'bounds': {'min': 2, 'max': 5}
-      },
-      {
-        'name': 'num_boost_round',
-        'type': 'int',
-        'bounds': {'min': 2, 'max': 5}
-      },
+      {"name": "max_depth", "type": "int", "bounds": {"min": 2, "max": 5}},
+      {"name": "num_boost_round", "type": "int", "bounds": {"min": 2, "max": 5}},
     ]
     config = {
-      'name': 'experiment-integration-test',
-      'type': 'offline',
-      'parameters': parameters,
-      'metrics': [{
-        'name': 'f1',
-        'strategy': 'optimize',
-        'objective': 'maximize'
-      }],
-      'parallel_bandwidth': 1,
-      'budget': 3
+      "name": "experiment-integration-test",
+      "type": "offline",
+      "parameters": parameters,
+      "metrics": [{"name": "f1", "strategy": "optimize", "objective": "maximize"}],
+      "parallel_bandwidth": 1,
+      "budget": 3,
     }
     experiment = sigopt.create_aiexperiment(**config)
     parameters = experiment.parameters
     parameters[0].bounds.max = 100
     parameters[1].bounds.min = 1
     new_config = {
-      'name': 'experiment-integration-test-1',
-      'parameters': parameters,
-      'parallel_bandwidth': 2,
-      'budget': 4
+      "name": "experiment-integration-test-1",
+      "parameters": parameters,
+      "parallel_bandwidth": 2,
+      "budget": 4,
     }
     experiment.update(**new_config)
     updated_experiment = sigopt.get_aiexperiment(experiment.id)
-    assert updated_experiment.name == 'experiment-integration-test-1'
+    assert updated_experiment.name == "experiment-integration-test-1"
     assert updated_experiment.budget == 4
     assert updated_experiment.parallel_bandwidth == 2
     assert updated_experiment.parameters[0].bounds.min == 2
     assert updated_experiment.parameters[0].bounds.max == 100
     assert updated_experiment.parameters[1].bounds.min == 1
     assert updated_experiment.parameters[1].bounds.max == 5
```

### Comparing `sigopt-8.8.0/integration_test/test_hyperopt.py` & `sigopt-8.8.1/integration_test/test_hyperopt.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,134 +1,131 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
-from hyperopt import fmin, tpe, hp, STATUS_OK, STATUS_FAIL, SparkTrials
-from hyperopt.mongoexp import MongoTrials
+import time
+import uuid
+
 import hyperopt
-from sigopt.hyperopt import SigOptTrials, upload_trials
-import sigopt
 import numpy as np
 import pytest
-import time
-import uuid
+from hyperopt import STATUS_FAIL, STATUS_OK, SparkTrials, fmin, hp, tpe
+from hyperopt.mongoexp import MongoTrials
+
+import sigopt
+from sigopt.hyperopt import SigOptTrials, upload_trials
+
 
 def objective(p, threshold=1.0, max_sleep_time=0.0):
-  x, y = p['x'], p['y']
+  x, y = p["x"], p["y"]
   if max_sleep_time > 0:
     time.sleep(np.random.rand() * max_sleep_time)
   w = np.random.rand()
   if w <= threshold:
-    return {
-      'loss': x ** 2 + y ** 2,
-      'sum': x + y,
-      'status': STATUS_OK
-    }
+    return {"loss": x**2 + y**2, "sum": x + y, "status": STATUS_OK}
   else:
-    return {
-      'status': STATUS_FAIL
-    }
+    return {"status": STATUS_FAIL}
+
 
 def objective_random(x):
   return objective(x, 0.8)
 
+
 def objective_success(x):
   return objective(x, 1.0)
 
+
 def objective_fail(x):
   return objective(x, -1.0)
 
+
 class TestHyperopt(object):
   def run_fmin(self, online=True, upload=True, objective=objective_success, max_evals=3, wrap=None, **kwargs):
-    project = 'hyperopt-integration-test'
-    if wrap == 'mongo':
-      trials = MongoTrials('mongo://mongodb:27017/foo_db/jobs', exp_key=str(uuid.uuid4()))
-    elif wrap == 'spark':
+    project = "hyperopt-integration-test"
+    if wrap == "mongo":
+      trials = MongoTrials("mongo://localhost:27017/foo_db/jobs", exp_key=str(uuid.uuid4()))
+    elif wrap == "spark":
       trials = SparkTrials()
     else:
       trials = None
     trials = SigOptTrials(project=project, online=(online and upload), trials=trials)
     try:
-      best = fmin(objective,
-                  space={
-                    'x' : hp.uniform('x', -10, 10),
-                    'y': hp.uniform('y', -10, 10)
-                  },
-                  algo=tpe.suggest,
-                  max_evals=max_evals,
-                  trials=trials,
-                  **kwargs
-                  )
+      best = fmin(
+        objective,
+        space={"x": hp.uniform("x", -10, 10), "y": hp.uniform("y", -10, 10)},
+        algo=tpe.suggest,
+        max_evals=max_evals,
+        trials=trials,
+        **kwargs
+      )
     except hyperopt.exceptions.AllTrialsFailed:
       best = None
     if upload and not online:
       trials.upload()
     return trials, best
 
   def test_upload_trials(self):
     trials, _ = self.run_fmin(upload=False)
-    tids = upload_trials('hyperopt-integration-test', trials)
+    tids = upload_trials("hyperopt-integration-test", trials)
     self._verify_uploaded_trials(trials, tids)
 
   def test_trials_delete_all(self):
     trials, _ = self.run_fmin(upload=True)
-    assert(len(trials) > 0 and len(trials) == len(trials.uploaded_tids))
+    assert len(trials) > 0 and len(trials) == len(trials.uploaded_tids)
     trials.delete_all()
-    assert(len(trials) == 0 and len(trials.uploaded_tids) == 0)
+    assert len(trials) == 0 and len(trials.uploaded_tids) == 0
 
-  @pytest.mark.parametrize("online, upload, wrap, max_evals",
-                           [
-                             (False, True, None, 3),
-                             (True, True, None, 3),
-                             (False, False, None, 3),
-                             (True, True, 'mongo', 3),
-                             (True, True, 'spark', 3),
-                            ])
-  @pytest.mark.parametrize("objective",
-                           [objective_random,
-                            objective_success,
-                            objective_fail])
+  @pytest.mark.parametrize(
+    "online, upload, wrap, max_evals",
+    [
+      (False, True, None, 3),
+      (True, True, None, 3),
+      (False, False, None, 3),
+      (True, True, "mongo", 3),
+      (True, True, "spark", 3),
+    ],
+  )
+  @pytest.mark.parametrize("objective", [objective_random, objective_success, objective_fail])
   def test_fmin(self, online, upload, objective, wrap, max_evals):
     trials, best = self.run_fmin(online, upload, objective, max_evals=max_evals, wrap=wrap)
     self._verify_best_trial(best, trials, objective)
     self._verify_runs(trials, upload, max_evals)
 
-
   def _verify_best_trial(self, best, trials, objective):
     if objective is objective_fail:
       assert best is None
     if objective is objective_success:
       assert best is not None
-    losses = [r['loss'] for r in trials.results if r['status'] == STATUS_OK]
+    losses = [r["loss"] for r in trials.results if r["status"] == STATUS_OK]
     assert ((not best) and (not losses)) or (best and losses)
     if best:
-      loss = objective_success(best)['loss']
+      loss = objective_success(best)["loss"]
       assert loss == min(losses)
 
   def _verify_runs(self, trials, upload, max_evals):
     if not upload:
       assert len(trials.uploaded_tids) == 0
       return
     assert len(trials.uploaded_tids) == max_evals
     self._verify_uploaded_trials(trials, trials.uploaded_tids)
 
   def _verify_uploaded_trials(self, trials, uploaded_tids):
-    trial_dict = {tid: (result, parameters)
-                  for tid, result, parameters in zip(trials.tids, trials.results,
-                                                     trials.parameters)}
+    trial_dict = {
+      tid: (result, parameters) for tid, result, parameters in zip(trials.tids, trials.results, trials.parameters)
+    }
 
     def run_result(run):
       result = {}
       if run.state == "completed":
-        result['status'] = STATUS_OK
+        result["status"] = STATUS_OK
         for m in run.values:
           result[m] = run.values[m].value
       elif run.state == "failed":
-        result['status'] = STATUS_FAIL
+        result["status"] = STATUS_FAIL
       else:
-        result['status'] = None
+        result["status"] = None
       return result
 
     def run_parameters(run):
       return dict(run.assignments)
 
     run_dict = {}
     for tid, run_id in uploaded_tids.items():
```

### Comparing `sigopt-8.8.0/integration_test/test_sigopt.py` & `sigopt-8.8.1/integration_test/test_sigopt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 import pytest
+
 import sigopt
 
 
 class TestSigOpt(object):
   def create_run(self, n):
     return {
       "name": f"batch-{n}",
       "assignments": {
         "x": n,
         "y": n * n,
       },
       "values": {
         "r0": dict(value=n * n + n),
-        "r1": dict(value=n ** 2),
+        "r1": dict(value=n**2),
       },
       "state": "completed" if (n % 2 == 0) else "failed",
     }
 
   @pytest.mark.parametrize("n", [10, 11])
   @pytest.mark.parametrize("max_batch_size", [2, 3, 10, 20])
   def test_upload_runs(self, n, max_batch_size):
```

### Comparing `sigopt-8.8.0/integration_test/test_xgboost_experiment.py` & `sigopt-8.8.1/integration_test/test_xgboost_experiment.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,174 +1,174 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 import copy
 import os
-import pytest
 import random
 
-os.environ['SIGOPT_PROJECT'] = "dev-sigopt-xgb-integration-test"
+import pytest
+
+
+os.environ["SIGOPT_PROJECT"] = "dev-sigopt-xgb-integration-test"
 
 import sigopt.xgboost
 from sigopt.xgboost.constants import CLASSIFICATION_METRIC_CHOICES, REGRESSION_METRIC_CHOICES
+
 from .test_xgboost_run import _form_random_run_params
 
+
 SEARCH_SPACES = [
   {
-    'name': 'eta',
-  },
-  {
-    'name': 'min_child_weight',
-  },
-  {
-    'name': 'max_depth',
-    'type': 'int',
-    'bounds': {'min': 2, 'max': 5}
+    "name": "eta",
   },
   {
-    'name': 'num_boost_round',
-    'type': 'int',
-    'bounds': {'min': 2, 'max': 5}
+    "name": "min_child_weight",
   },
+  {"name": "max_depth", "type": "int", "bounds": {"min": 2, "max": 5}},
+  {"name": "num_boost_round", "type": "int", "bounds": {"min": 2, "max": 5}},
 ]
 
 
 class TestXGBoostExperiment:
   experiment_params = None
 
   def _generate_randomized_search_space(self):
     search_space = copy.deepcopy(SEARCH_SPACES)
     if random.randint(0, 1) == 1:  # add bounds and type to eta randomly
-      search_space[0]['type'] = 'double'
-      search_space[0]['bounds'] = {'min': 0.1, 'max': 0.5}
-    if random.randint(0, 1) == 1:   # add bounds and type to min_child_weight randomly
-      search_space[1]['type'] = 'double'
-      search_space[1]['bounds'] = {'min': 0.0, 'max': 0.3}
+      search_space[0]["type"] = "double"
+      search_space[0]["bounds"] = {"min": 0.1, "max": 0.5}
+    if random.randint(0, 1) == 1:  # add bounds and type to min_child_weight randomly
+      search_space[1]["type"] = "double"
+      search_space[1]["bounds"] = {"min": 0.0, "max": 0.3}
     random_subset_size = random.randint(1, len(search_space))
     search_space = random.sample(search_space, random_subset_size)
-    if not any(p['name'] in ['eta', 'min_child_weight'] for p in search_space):
+    if not any(p["name"] in ["eta", "min_child_weight"] for p in search_space):
       search_space.append(SEARCH_SPACES[0])
     return search_space
 
   def _form_random_experiment_config(self, task):
     experiment_params = _form_random_run_params(task)
-    is_classification = bool(task in ('binary', 'multiclass'))
+    is_classification = bool(task in ("binary", "multiclass"))
     if is_classification:
       metric_to_optimize = random.choice(CLASSIFICATION_METRIC_CHOICES)
     else:
       metric_to_optimize = random.choice(REGRESSION_METRIC_CHOICES)
     search_space = self._generate_randomized_search_space()
 
     for param in search_space:
-      experiment_params['params'].pop(param['name'], None)
-      if param['name'] == 'num_boost_round':
-        experiment_params.pop('num_boost_round', None)
+      experiment_params["params"].pop(param["name"], None)
+      if param["name"] == "num_boost_round":
+        experiment_params.pop("num_boost_round", None)
 
     experiment_config = {
-      'name': f"xgboost-experiment-integration-test-{task}",
-      'type': 'offline',
-      'parameters': search_space,
-      'metrics': [{
-        'name': metric_to_optimize,
-        'strategy': 'optimize',
-        'objective': 'maximize'
-      }],
-      'parallel_bandwidth': 1,
-      'budget': random.randint(1, 3)
+      "name": f"xgboost-experiment-integration-test-{task}",
+      "type": "offline",
+      "parameters": search_space,
+      "metrics": [{"name": metric_to_optimize, "strategy": "optimize", "objective": "maximize"}],
+      "parallel_bandwidth": 1,
+      "budget": random.randint(1, 3),
     }
     if random.randint(0, 1) == 0:
-      del experiment_config['metrics']
+      del experiment_config["metrics"]
 
-    experiment_params['experiment_config'] = experiment_config
-    experiment_params['run_options'].pop('name', None)
-    experiment_params.pop('verbose_eval', None)
+    experiment_params["experiment_config"] = experiment_config
+    experiment_params["run_options"].pop("name", None)
+    experiment_params.pop("verbose_eval", None)
     self.experiment_params = experiment_params
 
   def _verify_parameter_assignments_for_all_runs(self, all_runs, parameters_list):
     for ssr in all_runs:
       for param in parameters_list:
-        if param.type in ('double', 'int'):
+        if param.type in ("double", "int"):
           assert param.bounds.min <= ssr.assignments[param.name] <= param.bounds.max
         else:
           categories = [c.name for c in param.categorical_values]
           assert ssr.assignments[param.name] in categories
 
   def _verify_metrics_for_all_runs(self, all_runs, metrics_list):
     for ssr in all_runs:
-      if ssr.state != 'failed':
+      if ssr.state != "failed":
         for metric in metrics_list:
           assert ssr.values[metric.name]
 
-  @pytest.mark.parametrize('task', ['binary', 'multiclass', 'regression'])
+  @pytest.mark.parametrize("task", ["binary", "multiclass", "regression"])
   def test_experiment(self, task):
     self._form_random_experiment_config(task)
-    experiment = sigopt.xgboost.experiment(**self.experiment_params) #pylint: disable=unexpected-keyword-arg
+    # pylint: disable=unexpected-keyword-arg
+    experiment = sigopt.xgboost.experiment(**self.experiment_params)
+    # pylint: enable=unexpected-keyword-arg
     assert experiment.is_finished()
     sigopt_suggested_runs = list(experiment.get_runs())
-    assert len(sigopt_suggested_runs) == self.experiment_params['experiment_config']['budget']
+    assert len(sigopt_suggested_runs) == self.experiment_params["experiment_config"]["budget"]
     self._verify_parameter_assignments_for_all_runs(sigopt_suggested_runs, experiment.parameters)
     self._verify_metrics_for_all_runs(sigopt_suggested_runs, experiment.metrics)
     experiment.archive()
 
   def test_early_stopping(self):
-    self._form_random_experiment_config('binary')
-    self.experiment_params['early_stopping_rounds'] = 1
-    experiment = sigopt.xgboost.experiment(**self.experiment_params) #pylint: disable=unexpected-keyword-arg
+    self._form_random_experiment_config("binary")
+    self.experiment_params["early_stopping_rounds"] = 1
+    # pylint: disable=unexpected-keyword-arg
+    experiment = sigopt.xgboost.experiment(**self.experiment_params)
+    # pylint: enable=unexpected-keyword-arg
     assert experiment.is_finished()
     sigopt_suggested_runs = list(experiment.get_runs())
     for ssr in sigopt_suggested_runs:
-      assert ssr.assignments['early_stopping_rounds'] == self.experiment_params['early_stopping_rounds']
-      assert ssr.values['num_boost_round_before_stopping'].value >= 0
+      assert ssr.assignments["early_stopping_rounds"] == self.experiment_params["early_stopping_rounds"]
+      assert ssr.values["num_boost_round_before_stopping"].value >= 0
     experiment.archive()
 
   def test_experiment_with_custom_loop(self):
-    run_params = _form_random_run_params('binary')
-    if len(run_params['evals']) > 1:
-      run_params['evals'] = run_params['evals'][:1]
+    run_params = _form_random_run_params("binary")
+    if len(run_params["evals"]) > 1:
+      run_params["evals"] = run_params["evals"][:1]
 
     fixed_params = {
-      'alpha': 0.2,
-      'objective': 'binary:logistic',
-      'eval_metric': ['logloss', 'auc'],
+      "alpha": 0.2,
+      "objective": "binary:logistic",
+      "eval_metric": ["logloss", "auc"],
     }
-    experiment_config=dict(
+    experiment_config = dict(
       name="xgboost a la carte",
       type="offline",
       parameters=[
-        dict(name="eta", type="double", bounds=dict(min=1e-4, max=10), transformation='log'),
+        dict(name="eta", type="double", bounds=dict(min=1e-4, max=10), transformation="log"),
         dict(name="num_boost_round", type="int", bounds=dict(min=10, max=50)),
-        dict(name="booster", type="categorical", categorical_values=(['gbtree', 'gblinear'])),
+        dict(
+          name="booster",
+          type="categorical",
+          categorical_values=(["gbtree", "gblinear"]),
+        ),
       ],
       metrics=[
         dict(name="test0-F1"),
         dict(name="Training time", strategy="optimize", objective="minimize"),
         dict(name="test0-recall", strategy="store", objective="maximize"),
       ],
       budget=5,
     )
     experiment = sigopt.create_aiexperiment(**experiment_config)
     custom_run = experiment.create_run()
 
     ctx = sigopt.xgboost.run(
       params=fixed_params,
-      dtrain=run_params['dtrain'],
-      evals=run_params['evals'],
+      dtrain=run_params["dtrain"],
+      evals=run_params["evals"],
       verbose_eval=False,
-      run_options={'run': custom_run},
+      run_options={"run": custom_run},
     )
 
     run_obj = sigopt.get_run(ctx.run.id)
-    assert run_obj.assignments['alpha'] == fixed_params['alpha']
-    assert run_obj.metadata['objective'] == fixed_params['objective']
-    assert run_obj.metadata['eval_metric'] == str(fixed_params['eval_metric'])
-    assert run_obj.assignments['eta']  == custom_run.params['eta']
-    assert run_obj.assignments['num_boost_round'] == custom_run.params['num_boost_round']
-    assert run_obj.assignments['booster'] in ('gbtree', 'gblinear')
-    assert 0 <= run_obj.values['test0-F1'].value <= 1
-    assert 0 <= run_obj.values['test0-recall'].value <= 1
-    assert run_obj.values['Training time'].value > 0
+    assert run_obj.assignments["alpha"] == fixed_params["alpha"]
+    assert run_obj.metadata["objective"] == fixed_params["objective"]
+    assert run_obj.metadata["eval_metric"] == str(fixed_params["eval_metric"])
+    assert run_obj.assignments["eta"] == custom_run.params["eta"]
+    assert run_obj.assignments["num_boost_round"] == custom_run.params["num_boost_round"]
+    assert run_obj.assignments["booster"] in ("gbtree", "gblinear")
+    assert 0 <= run_obj.values["test0-F1"].value <= 1
+    assert 0 <= run_obj.values["test0-recall"].value <= 1
+    assert run_obj.values["Training time"].value > 0
     self._verify_parameter_assignments_for_all_runs([run_obj], experiment.parameters)
     self._verify_metrics_for_all_runs([run_obj], experiment.metrics)
     ctx.run.end()
     assert not experiment.is_finished()
     assert len(list(experiment.get_runs())) == 1
     experiment.archive()
```

### Comparing `sigopt-8.8.0/integration_test/test_xgboost_run.py` & `sigopt-8.8.1/integration_test/test_xgboost_run.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,64 +1,63 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
-from inspect import signature
 import itertools
 import json
+import math
 import os
 import platform
-import pytest
 import random
-import math
+from inspect import signature
+
+import pytest
 
-os.environ['SIGOPT_PROJECT'] = "dev-sigopt-xgb-integration-test"
+
+os.environ["SIGOPT_PROJECT"] = "dev-sigopt-xgb-integration-test"
 
 import numpy
+import xgboost as xgb
+from sklearn import datasets
+from sklearn.model_selection import train_test_split
+
 import sigopt.xgboost
 from sigopt.xgboost.checkpoint_callback import SigOptCheckpointCallback
-from sigopt.xgboost.constants import (
-  CLASSIFICATION_METRIC_CHOICES,
-  DEFAULT_EVALS_NAME,
-  REGRESSION_METRIC_CHOICES,
-)
+from sigopt.xgboost.constants import CLASSIFICATION_METRIC_CHOICES, DEFAULT_EVALS_NAME, REGRESSION_METRIC_CHOICES
 from sigopt.xgboost.run import (
   DEFAULT_CHECKPOINT_PERIOD,
   MAX_NUM_CHECKPOINTS,
   PARAMS_LOGGED_AS_METADATA,
   XGB_INTEGRATION_KEYWORD,
   XGBRunHandler,
 )
-from sklearn import datasets
-from sklearn.model_selection import train_test_split
-import xgboost as xgb
 
 
 POSSIBLE_PARAMETERS = {
-  'eta': 10 ** random.uniform(-4, 1),
-  'gamma': random.uniform(0, 4),
-  'max_depth': random.randint(1, 5),
-  'min_child_weight': random.uniform(0, 3),
-  'lambda': random.uniform(1, 3),
-  'alpha': 10 ** random.uniform(-4, 0),
-  'tree_method': random.choice(['hist', 'exact', 'approx', 'auto']),
+  "eta": 10 ** random.uniform(-4, 1),
+  "gamma": random.uniform(0, 4),
+  "max_depth": random.randint(1, 5),
+  "min_child_weight": random.uniform(0, 3),
+  "lambda": random.uniform(1, 3),
+  "alpha": 10 ** random.uniform(-4, 0),
+  "tree_method": random.choice(["hist", "exact", "approx", "auto"]),
 }
 
 
-def _create_random_dataset(task='binary'):
-  if task == 'binary':
+def _create_random_dataset(task="binary"):
+  if task == "binary":
     n_samples = random.randint(180, 300)
     n_features = random.randint(5, 25)
     n_classes = 2
 
     return datasets.make_classification(
       n_samples=n_samples,
       n_features=n_features,
       n_classes=n_classes,
     )
-  elif task == 'multiclass':
+  elif task == "multiclass":
     n_samples = random.randint(180, 300)
     n_classes = random.randint(3, 8)
     n_informative = random.randint(2 * n_classes, 20)
     n_features = random.randint(n_informative + 2, 40)
 
     return datasets.make_classification(
       n_samples=n_samples,
@@ -74,229 +73,239 @@
     return datasets.make_regression(
       n_samples=n_samples,
       n_features=n_features,
       n_informative=n_informative,
       noise=0.2,
     )
 
-def _create_random_metric_objective(task='binary'):
-  if task == 'binary':
+
+def _create_random_metric_objective(task="binary"):
+  if task == "binary":
     return {
-      'objective': random.choice(['binary:logistic', 'binary:hinge', 'binary:logitraw']),
-      'eval_metric': ['logloss', 'aucpr', 'error'],
+      "objective": random.choice(["binary:logistic", "binary:hinge", "binary:logitraw"]),
+      "eval_metric": ["logloss", "aucpr", "error"],
     }
-  elif task == 'multiclass':
+  elif task == "multiclass":
     return {
-      'objective': random.choice(['multi:softmax', 'multi:softprob']),
-      'eval_metric': ['mlogloss', 'merror'],
+      "objective": random.choice(["multi:softmax", "multi:softprob"]),
+      "eval_metric": ["mlogloss", "merror"],
     }
   else:
     return {
-      'objective': random.choice(['reg:squarederror', 'reg:pseudohubererror']),
-      'eval_metric': ['rmse', 'mae', 'mape'],
+      "objective": random.choice(["reg:squarederror", "reg:pseudohubererror"]),
+      "eval_metric": ["rmse", "mae", "mape"],
     }
 
 
 def _form_random_run_params(task):
   X, y = _create_random_dataset(task)
   X_train, X_test, Y_train, Y_test = train_test_split(X, y, test_size=0.2)
   D_train = xgb.DMatrix(X_train, label=Y_train)
   D_test = xgb.DMatrix(X_test, label=Y_test)
 
   possible_params = POSSIBLE_PARAMETERS
   random_subset_size = random.randint(1, len(possible_params))
   subset_keys = random.sample(possible_params.keys(), random_subset_size)
   subset_params = {k: possible_params[k] for k in subset_keys}
   subset_params.update(_create_random_metric_objective(task))
-  if task == 'multiclass':
-    subset_params.update({'num_class': len(numpy.unique(y))})
+  if task == "multiclass":
+    subset_params.update({"num_class": len(numpy.unique(y))})
 
-  run_options = {'name': f'dev-integration-test-{task}'}
+  run_options = {"name": f"dev-integration-test-{task}"}
 
   return dict(
     params=subset_params,
     dtrain=D_train,
-    evals=[(D_test, f'test{n}') for n in range(random.randint(1, 3))],
+    evals=[(D_test, f"test{n}") for n in range(random.randint(1, 3))],
     num_boost_round=random.randint(3, 15),
     verbose_eval=random.choice([True, False]),
     run_options=run_options,
   )
 
 
 class TestXGBoostRun(object):
   is_classification = None
   run_params = None
 
   def _verify_parameter_logging(self, run):
-    params = self.run_params['params']
+    params = self.run_params["params"]
     for p in params.keys():
       if p not in PARAMS_LOGGED_AS_METADATA:
         assert params[p] == run.assignments[p]
       else:
         if not isinstance(params[p], list):
           assert params[p] == run.metadata[p]
         else:
           assert str(params[p]) == run.metadata[p]
-    assert run.assignments['num_boost_round'] == self.run_params['num_boost_round']
+    assert run.assignments["num_boost_round"] == self.run_params["num_boost_round"]
 
   def _verify_metric_logging(self, run):
     data_names = []
-    if self.run_params['evals']:
-      data_names.extend([e[-1] for e in self.run_params['evals']])
+    if self.run_params["evals"]:
+      data_names.extend([e[-1] for e in self.run_params["evals"]])
     if self.is_classification:
       for d_name, m_name in itertools.product(data_names, CLASSIFICATION_METRIC_CHOICES):
-        assert 0 <= run.values['-'.join((d_name, m_name))].value <= 1
+        assert 0 <= run.values["-".join((d_name, m_name))].value <= 1
     else:
       for d_name, m_name in itertools.product(data_names, REGRESSION_METRIC_CHOICES):
-        assert run.values['-'.join((d_name, m_name))].value >= 0
+        assert run.values["-".join((d_name, m_name))].value >= 0
 
-    if self.run_params['params']['eval_metric']:
-      for d_name, m_name in itertools.product(data_names[1:], self.run_params['params']['eval_metric']):
-        assert run.values['-'.join((d_name, m_name))]
+    if self.run_params["params"]["eval_metric"]:
+      for d_name, m_name in itertools.product(data_names[1:], self.run_params["params"]["eval_metric"]):
+        assert run.values["-".join((d_name, m_name))]
 
-    assert run.values['Training time'].value > 0
-    assert run.values['best_iteration'].value >= 0
+    assert run.values["Training time"].value > 0
+    assert run.values["best_iteration"].value >= 0
 
   def _verify_metadata_logging(self, run):
-    assert run.metadata['Dataset columns'] == self.run_params['dtrain'].num_col()
-    assert run.metadata['Dataset rows'] == self.run_params['dtrain'].num_row()
-    if 'evals' in self.run_params and self.run_params['evals'] is not None:
-      if isinstance(self.run_params['evals'], list):
-        assert run.metadata['Number of Test Sets'] == len(self.run_params['evals'])
+    assert run.metadata["Dataset columns"] == self.run_params["dtrain"].num_col()
+    assert run.metadata["Dataset rows"] == self.run_params["dtrain"].num_row()
+    if "evals" in self.run_params and self.run_params["evals"] is not None:
+      if isinstance(self.run_params["evals"], list):
+        assert run.metadata["Number of Test Sets"] == len(self.run_params["evals"])
       else:
-        assert run.metadata['Number of Test Sets'] == 1
-    assert run.metadata['Python Version'] == platform.python_version()
-    assert run.metadata['XGBoost Version'] == xgb.__version__
+        assert run.metadata["Number of Test Sets"] == 1
+    assert run.metadata["Python Version"] == platform.python_version()
+    assert run.metadata["XGBoost Version"] == xgb.__version__
 
   def _verify_feature_importances_logging(self, run, model):
-    real_scores = sorted(model.get_score(importance_type='weight').items(), key=lambda x: (x[1], x[0]), reverse=True)
+    real_scores = sorted(
+      model.get_score(importance_type="weight").items(),
+      key=lambda x: (x[1], x[0]),
+      reverse=True,
+    )
     if real_scores:
-      feature_importances = run.sys_metadata['feature_importances']
-      saved_scores = sorted(feature_importances['scores'].items(), key=lambda x: (x[1], x[0]), reverse=True)
-      assert feature_importances['type'] == 'weight'
+      feature_importances = run.sys_metadata["feature_importances"]
+      saved_scores = sorted(feature_importances["scores"].items(), key=lambda x: (x[1], x[0]), reverse=True)
+      assert feature_importances["type"] == "weight"
       assert saved_scores and len(saved_scores) <= len(real_scores)
-      real_scores = real_scores[:len(saved_scores)]
+      real_scores = real_scores[: len(saved_scores)]
       assert [feature_name for feature_name, _ in real_scores] == [feature_name for feature_name, _ in saved_scores]
       assert numpy.allclose(
         numpy.array([feature_importance for _, feature_importance in real_scores]),
         numpy.array([feature_importance for _, feature_importance in saved_scores]),
       )
 
   def _verify_miscs_data_logging(self, run):
-    if 'name' in self.run_params['run_options']:
-      assert run.name == self.run_params['run_options']['name']
+    if "name" in self.run_params["run_options"]:
+      assert run.name == self.run_params["run_options"]["name"]
 
-    if 'evals' in self.run_params:
-      if isinstance(self.run_params['evals'], list):
-        assert set(run.datasets) == {e[1] for e in self.run_params['evals']}
+    if "evals" in self.run_params:
+      if isinstance(self.run_params["evals"], list):
+        assert set(run.datasets) == {e[1] for e in self.run_params["evals"]}
       else:
         assert len(run.datasets) == 1
         assert run.datasets[0] == DEFAULT_EVALS_NAME
 
     assert XGB_INTEGRATION_KEYWORD in run.dev_metadata
     assert run.dev_metadata[XGB_INTEGRATION_KEYWORD]
 
   def _verify_checkpoint_logging(self, run):
-    period = self.run_params.get('verbose_eval')
+    period = self.run_params.get("verbose_eval")
     if not period:
       period = DEFAULT_CHECKPOINT_PERIOD
     elif period is True:
       period = 1
-    num_boost_round = self.run_params['num_boost_round']
+    num_boost_round = self.run_params["num_boost_round"]
     period = max(period, math.ceil((num_boost_round + 1) / MAX_NUM_CHECKPOINTS))
     assert run.checkpoint_count == 1 + math.ceil((num_boost_round - 1) / period)
 
-  @pytest.mark.parametrize("task", ['binary', 'multiclass', 'regression'])
+  @pytest.mark.parametrize("task", ["binary", "multiclass", "regression"])
   def test_run(self, task):
-    self.is_classification = bool(task in ('binary', 'multiclass'))
+    self.is_classification = bool(task in ("binary", "multiclass"))
     self.run_params = _form_random_run_params(task)
     ctx = sigopt.xgboost.run(**self.run_params)
     run = sigopt.get_run(ctx.run.id)
 
     self._verify_metadata_logging(run)
     self._verify_parameter_logging(run)
     self._verify_metric_logging(run)
     self._verify_feature_importances_logging(run, ctx.model)
     self._verify_miscs_data_logging(run)
     self._verify_checkpoint_logging(run)
     ctx.run.end()
 
   def test_run_options_no_logging(self):
-    self.run_params = _form_random_run_params(task='binary')
-    self.run_params['run_options'].update({
-      'autolog_checkpoints': False,
-      'autolog_feature_importances': False,
-      'autolog_metrics': False,
-      'autolog_stderr': False,
-      'autolog_stdout': False,
-      'autolog_xgboost_defaults': False,
-    })
+    self.run_params = _form_random_run_params(task="binary")
+    self.run_params["run_options"].update(
+      {
+        "autolog_checkpoints": False,
+        "autolog_feature_importances": False,
+        "autolog_metrics": False,
+        "autolog_stderr": False,
+        "autolog_stdout": False,
+        "autolog_xgboost_defaults": False,
+      }
+    )
     ctx = sigopt.xgboost.run(**self.run_params)
     run = sigopt.get_run(ctx.run.id)
 
     assert run.checkpoint_count == 0
-    assert 'feature_importances' not in run.sys_metadata
-    if self.run_params['evals']:
+    assert "feature_importances" not in run.sys_metadata
+    if self.run_params["evals"]:
       assert set(run.values.keys()) == {
-        '-'.join((data_name[1], metric_name)) for data_name, metric_name in itertools.product(
-          self.run_params['evals'], self.run_params['params']['eval_metric']
+        "-".join((data_name[1], metric_name))
+        for data_name, metric_name in itertools.product(
+          self.run_params["evals"], self.run_params["params"]["eval_metric"]
         )
       }
-    assert len(run.assignments) <= len(self.run_params['params']) + 1
+    assert len(run.assignments) <= len(self.run_params["params"]) + 1
     self._verify_miscs_data_logging(run)
     assert not run.logs
     ctx.run.end()
 
   def test_wrong_dtrain_type(self):
-    self.run_params = _form_random_run_params(task='regression')
-    self.run_params['evals'] = numpy.random.random((5, 3))
+    self.run_params = _form_random_run_params(task="regression")
+    self.run_params["evals"] = numpy.random.random((5, 3))
     with pytest.raises(TypeError):
       sigopt.xgboost.run(**self.run_params)
 
   def test_log_default_params(self):
     self.run_params = _form_random_run_params(task="multiclass")
-    self.run_params['params'] = POSSIBLE_PARAMETERS.copy()
-    del self.run_params['params']['eta']
-    del self.run_params['params']['gamma']
-    del self.run_params['params']['lambda']
-    del self.run_params['num_boost_round']
+    self.run_params["params"] = POSSIBLE_PARAMETERS.copy()
+    del self.run_params["params"]["eta"]
+    del self.run_params["params"]["gamma"]
+    del self.run_params["params"]["lambda"]
+    del self.run_params["num_boost_round"]
     ctx = sigopt.xgboost.run(**self.run_params)
     run = sigopt.get_run(ctx.run.id)
-    assert numpy.isclose(run.assignments['eta'], 0.3)
-    assert run.assignments['gamma'] == 0
-    assert run.assignments['lambda'] == 1
-    assert run.assignments['num_boost_round'] == 10
+    assert numpy.isclose(run.assignments["eta"], 0.3)
+    assert run.assignments["gamma"] == 0
+    assert run.assignments["lambda"] == 1
+    assert run.assignments["num_boost_round"] == 10
 
   def test_provided_run(self):
     self.run_params = _form_random_run_params(task="binary")
     run = sigopt.create_run(name="placeholder-run-with-max-depth-already-logged")
-    run.params.update({'max_depth': 3})
-    run.params.update({'num_boost_round': 7})
+    run.params.update({"max_depth": 3})
+    run.params.update({"num_boost_round": 7})
 
-    self.run_params['run_options'].update({
-      'autolog_checkpoints': False,
-      'autolog_feature_importances': False,
-      'autolog_metrics': False,
-      'autolog_stderr': False,
-      'autolog_stdout': False,
-      'run': run,
-      'name': None,
-    })
-    self.run_params['params'] = {'max_depth': 9}
-    del self.run_params['num_boost_round']
+    self.run_params["run_options"].update(
+      {
+        "autolog_checkpoints": False,
+        "autolog_feature_importances": False,
+        "autolog_metrics": False,
+        "autolog_stderr": False,
+        "autolog_stdout": False,
+        "run": run,
+        "name": None,
+      }
+    )
+    self.run_params["params"] = {"max_depth": 9}
+    del self.run_params["num_boost_round"]
     ctx = sigopt.xgboost.run(**self.run_params)
     booster = ctx.model
     params = json.loads(booster.save_config())
-    trained_max_depth = params['learner']['gradient_booster']['updater']['grow_colmaker']['train_param']['max_depth']
+    trained_max_depth = params["learner"]["gradient_booster"]["updater"]["grow_colmaker"]["train_param"]["max_depth"]
     assert int(trained_max_depth) == 3
-    bst_jsons = booster.get_dump(dump_format='json')
+    bst_jsons = booster.get_dump(dump_format="json")
     assert len(bst_jsons) == 7
     run = sigopt.get_run(ctx.run.id)
-    assert run.assignments['max_depth'] == 3
-    assert run.assignments['num_boost_round'] == 7
+    assert run.assignments["max_depth"] == 3
+    assert run.assignments["num_boost_round"] == 7
     ctx.run.end()
 
 
 class TestFormCallbacks(object):
   run_params = None
 
   def _append_xgbrun_param_none_values(self):
@@ -305,93 +314,93 @@
     for p_name in all_xgbrun_params.keys():
       if p_name not in self.run_params:
         self.run_params[p_name] = None
 
   @pytest.mark.parametrize("verbose_eval", [True, False, 1, 3, 23])
   def test_xgbrun_form_callbacks(self, verbose_eval):
     self.run_params = _form_random_run_params(task="multiclass")
-    self.run_params['verbose_eval'] = verbose_eval
-    self.run_params['num_boost_round'] = 35
-    self.run_params['callbacks'] = None
+    self.run_params["verbose_eval"] = verbose_eval
+    self.run_params["num_boost_round"] = 35
+    self.run_params["callbacks"] = None
     self._append_xgbrun_param_none_values()
     xgbrun = XGBRunHandler(**self.run_params)
     xgbrun.form_callbacks()
     assert len(xgbrun.callbacks) == 1
     callback = xgbrun.callbacks[0]
     assert isinstance(callback, SigOptCheckpointCallback)
     if verbose_eval is False:
       assert callback.period == DEFAULT_CHECKPOINT_PERIOD
     else:
       assert callback.period == int(verbose_eval)
 
   def test_xgbrun_checkpoint_period_high_num_boost_round(self):
     self.run_params = _form_random_run_params(task="multiclass")
-    self.run_params['verbose_eval'] = False
-    self.run_params['num_boost_round'] = 200
-    self.run_params['callbacks'] = None
+    self.run_params["verbose_eval"] = False
+    self.run_params["num_boost_round"] = 200
+    self.run_params["callbacks"] = None
     self._append_xgbrun_param_none_values()
     xgbrun = XGBRunHandler(**self.run_params)
     xgbrun.form_callbacks()
     assert len(xgbrun.callbacks) == 1
     callback = xgbrun.callbacks[0]
     assert callback.period == DEFAULT_CHECKPOINT_PERIOD
 
-    self.run_params['verbose_eval'] = True
-    self.run_params['num_boost_round'] = 999
+    self.run_params["verbose_eval"] = True
+    self.run_params["num_boost_round"] = 999
     xgbrun = XGBRunHandler(**self.run_params)
     xgbrun.form_callbacks()
     callback = xgbrun.callbacks[0]
     assert callback.period == DEFAULT_CHECKPOINT_PERIOD
 
-    self.run_params['num_boost_round'] = 1000
+    self.run_params["num_boost_round"] = 1000
     xgbrun = XGBRunHandler(**self.run_params)
     xgbrun.form_callbacks()
     callback = xgbrun.callbacks[0]
     assert callback.period == 6
 
-    self.run_params['num_boost_round'] = 3000
+    self.run_params["num_boost_round"] = 3000
     xgbrun = XGBRunHandler(**self.run_params)
     xgbrun.form_callbacks()
     callback = xgbrun.callbacks[0]
     assert callback.period == 16
 
   def test_xgbrun_callbacks_appending(self):
     self.run_params = _form_random_run_params(task="multiclass")
-    self.run_params['verbose_eval'] = False
-    self.run_params['callbacks'] = [xgb.callback.EvaluationMonitor(period=3)]
+    self.run_params["verbose_eval"] = False
+    self.run_params["callbacks"] = [xgb.callback.EvaluationMonitor(period=3)]
     self._append_xgbrun_param_none_values()
     xgbrun = XGBRunHandler(**self.run_params)
     xgbrun.form_callbacks()
     assert len(xgbrun.callbacks) == 2
     assert xgbrun.callbacks[0].period == xgbrun.callbacks[1].period
 
   def test_xgbrun_callbacks_no_appending(self):
     self.run_params = _form_random_run_params(task="multiclass")
-    self.run_params['callbacks'] = [xgb.callback.EarlyStopping(rounds=3)]
-    self.run_params['evals'] = None
+    self.run_params["callbacks"] = [xgb.callback.EarlyStopping(rounds=3)]
+    self.run_params["evals"] = None
     self._append_xgbrun_param_none_values()
     xgbrun = XGBRunHandler(**self.run_params)
     xgbrun.form_callbacks()
     assert len(xgbrun.callbacks) == 1
     assert isinstance(xgbrun.callbacks[0], xgb.callback.EarlyStopping)
 
   def test_xgbrun_early_stopping(self):
     """
-    This test is slightly more involved, and uses a dataset and params for which we know XGB will early stop, and
-    then verifies that early stopping occurs
-    """
+        This test is slightly more involved, and uses a dataset and params for which we know XGB will early stop, and
+        then verifies that early stopping occurs
+        """
     n = 100
     X = numpy.linspace(0, 1, n)[:, None]
     y = numpy.zeros(n)
     y[50:] = 1
     X_train, X_test, Y_train, Y_test = train_test_split(X, y, test_size=0.2, random_state=1234)
     D_train = xgb.DMatrix(X_train, label=Y_train)
     D_test = xgb.DMatrix(X_test, label=Y_test)
-    self.run_params =_form_random_run_params(task="binary")
-    self.run_params['dtrain'] = D_train
-    self.run_params['evals'] = D_test
-    self.run_params['num_boost_round'] = 100
-    self.run_params['early_stopping_rounds'] = 2
+    self.run_params = _form_random_run_params(task="binary")
+    self.run_params["dtrain"] = D_train
+    self.run_params["evals"] = D_test
+    self.run_params["num_boost_round"] = 100
+    self.run_params["early_stopping_rounds"] = 2
     ctx = sigopt.xgboost.run(**self.run_params)
     run = sigopt.get_run(ctx.run.id)
-    assert run.assignments['early_stopping_rounds'] == self.run_params['early_stopping_rounds']
-    assert run.values['num_boost_round_before_stopping'].value < self.run_params['num_boost_round']
+    assert run.assignments["early_stopping_rounds"] == self.run_params["early_stopping_rounds"]
+    assert run.values["num_boost_round_before_stopping"].value < self.run_params["num_boost_round"]
```

### Comparing `sigopt-8.8.0/setup.py` & `sigopt-8.8.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,73 +1,79 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
-from codecs import open
 import os
 import sys
 import warnings
 
 from setuptools import find_packages, setup
 
+
 if sys.version_info < (3, 6):
   warnings.warn(
-    'Python versions lower than 3.6 are no longer supported.'
-    ' Please upgrade to Python 3.6 or newer or use an older version of the sigopt-python client.',
-    DeprecationWarning
+    (
+      "Python versions lower than 3.6 are no longer supported. Please upgrade to"
+      " Python 3.6 or newer or use an older version of the sigopt-python client."
+    ),
+    DeprecationWarning,
   )
 
-# NOTE(patrick): We can't `import sigopt.version` directly, because that
+# NOTE: We can't `import sigopt.version` directly, because that
 # will cause us to execute `sigopt/__init__.py`, which may transitively import
 # packages that may not have been installed yet. So jump straight to sigopt/version.py
 # and execute that directly, which should be simple enough that it doesn't import anything
 # Learned from https://github.com/stripe/stripe-python (MIT licensed)
 version_contents = {}
 here = os.path.abspath(os.path.dirname(__file__))
-with open(os.path.join(here, 'sigopt', 'version.py'), encoding='utf-8') as f:
-  exec(f.read(), version_contents)
-VERSION = version_contents['VERSION']
-
-with open(os.path.join(here, 'requirements.txt')) as requirements_fp:
-  install_requires = requirements_fp.read().split('\n')
-with open(os.path.join(here, 'requirements-dev.txt')) as requirements_dev_fp:
-  dev_install_requires = requirements_dev_fp.read().split('\n')
+with open(os.path.join(here, "sigopt", "version.py"), encoding="utf-8") as f:
+  exec(f.read(), version_contents)  # pylint: disable=exec-used
+VERSION = version_contents["VERSION"]
+
+with open(os.path.join(here, "requirements.txt")) as requirements_fp:
+  install_requires = requirements_fp.read().split("\n")
+with open(os.path.join(here, "requirements-dev.txt")) as requirements_dev_fp:
+  dev_install_requires = requirements_dev_fp.read().split("\n")
 
 orchestrate_install_requires = [
   "Pint>=0.16.0,<0.17.0",
   "boto3>=1.16.34,<2.0.0",
   "docker>=4.4.0,<5.0.0",
   "kubernetes>=12.0.1,<13.0.0",
   "pyOpenSSL>=20.0.0",
 ]
-xgboost_install_requires = ['xgboost>=1.3.1', 'numpy>=1.15.0']
-hyperopt_install_requires = ['hyperopt>=0.2.7']
-lite_install_requires = ['sigoptlite>=0.1.1']
+xgboost_install_requires = ["xgboost>=1.3.1", "numpy>=1.15.0"]
+hyperopt_install_requires = ["hyperopt>=0.2.7"]
+lite_install_requires = ["sigoptlite>=0.1.1"]
 
 setup(
-  name='sigopt',
+  name="sigopt",
   version=VERSION,
-  description='SigOpt Python API Client',
-  author='SigOpt',
-  author_email='support@sigopt.com',
-  url='https://sigopt.com/',
-  packages=find_packages(exclude=['tests*']),
+  description="SigOpt Python API Client",
+  author="SigOpt",
+  author_email="support@sigopt.com",
+  url="https://sigopt.com/",
+  packages=find_packages(exclude=["tests*"]),
   package_data={
-    '': ['*.ms', '*.txt', '*.yml', '*.yaml'],
+    "": ["*.ms", "*.txt", "*.yml", "*.yaml"],
   },
   install_requires=install_requires,
   extras_require={
-    'dev': dev_install_requires + xgboost_install_requires + hyperopt_install_requires,
-    'hyperopt': hyperopt_install_requires,
-    'orchestrate': orchestrate_install_requires,
-    'xgboost': xgboost_install_requires,
-    'lite': lite_install_requires,
+    "dev": dev_install_requires
+    + orchestrate_install_requires
+    + xgboost_install_requires
+    + hyperopt_install_requires
+    + lite_install_requires,
+    "hyperopt": hyperopt_install_requires,
+    "orchestrate": orchestrate_install_requires,
+    "xgboost": xgboost_install_requires,
+    "lite": lite_install_requires,
   },
   entry_points={
-    'console_scripts': [
-      'sigopt=sigopt.cli.__main__:sigopt_cli',
+    "console_scripts": [
+      "sigopt=sigopt.cli.__main__:sigopt_cli",
     ],
   },
   classifiers=[
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `sigopt-8.8.0/sigopt/__init__.py` & `sigopt-8.8.1/sigopt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 import warnings
 
 from .config import config
 from .defaults import get_default_project
+from .factory import SigOptFactory
 from .interface import Connection
-from .sigopt_logging import enable_print_logging
 from .run_context import global_run_context as _global_run_context
-from .factory import SigOptFactory
+from .sigopt_logging import enable_print_logging
 from .version import VERSION
 
 
 params = _global_run_context.params
 log_checkpoint = _global_run_context.log_checkpoint
 log_dataset = _global_run_context.log_dataset
 log_failure = _global_run_context.log_failure
@@ -38,21 +38,27 @@
 unarchive_run = _global_factory.unarchive_run
 get_run = _global_factory.get_run
 upload_runs = _global_factory.upload_runs
 
 
 def load_ipython_extension(ipython):
   from .magics import SigOptMagics as _Magics
+
   ipython.register_magics(_Magics)
   enable_print_logging()
 
+
 def get_run_id():
   return _global_run_context.id
 
+
 def set_project(project):
   if get_run_id() is not None:
     warnings.warn(
-      "set_project does nothing when your code is executed with the SigOpt CLI."
-      " Set the SIGOPT_PROJECT environment variable or use the --project CLI option instead.",
+      (
+        "set_project does nothing when your code is executed with the SigOpt"
+        " CLI. Set the SIGOPT_PROJECT environment variable or use the --project"
+        " CLI option instead."
+      ),
       UserWarning,
     )
   return _global_factory.set_project(project)
```

### Comparing `sigopt-8.8.0/sigopt/aiexperiment_context.py` & `sigopt-8.8.1/sigopt/aiexperiment_context.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 import json
 import threading
 
-from .run_factory import BaseRunFactory
-from .run_context import global_run_context
 from .objects import Parameter
+from .run_context import global_run_context
+from .run_factory import BaseRunFactory
 from .validate.aiexperiment_input import validate_aiexperiment_update_input
 
 
 class AIExperimentContext(BaseRunFactory):
-  '''Wraps the AIExperiment object and provides extra utility methods.'''
+  """Wraps the AIExperiment object and provides extra utility methods."""
 
   def __init__(self, aiexperiment, connection):
     self._aiexperiment = aiexperiment
     self._refresh_lock = threading.Lock()
     self._connection = connection
 
   def refresh(self):
-    '''Refresh the state of the AIExperiment from the SigOpt API.'''
+    """Refresh the state of the AIExperiment from the SigOpt API."""
     connection = self._connection
     with self._refresh_lock:
       self._aiexperiment = connection.aiexperiments(self.id).fetch()
 
   def is_finished(self):
-    '''Check if the AIExperiment has consumed its entire budget.'''
+    """Check if the AIExperiment has consumed its entire budget."""
     self.refresh()
     return self.progress.remaining_budget is not None and self.progress.remaining_budget <= 0
 
   def loop(self, name=None):
-    '''Create runs until the AIExperiment has finished.'''
+    """Create runs until the AIExperiment has finished."""
     while not self.is_finished():
       yield self.create_run(name=name)
 
   def archive(self):
     connection = self._connection
     connection.aiexperiments(self.id).delete()
     self.refresh()
@@ -46,38 +46,54 @@
 
   def __getattr__(self, attr):
     return getattr(self._aiexperiment, attr)
 
   def _create_run(self, name, metadata):
     aiexperiment = self._aiexperiment
     connection = self._connection
-    run = connection.aiexperiments(aiexperiment.id).training_runs().create(
-      name=name,
-      metadata=metadata,
+    run = (
+      connection.aiexperiments(aiexperiment.id)
+      .training_runs()
+      .create(
+        name=name,
+        metadata=metadata,
+      )
     )
     run_context = self.run_context_class(connection, run, global_run_context.params)
     return run_context
 
   def get_runs(self):
-    return self._connection.clients(self.client).projects(self.project).training_runs().fetch(filters=json.dumps([{
-      "field": "experiment",
-      "operator": "==",
-      "value": self.id,
-    }])).iterate_pages()
+    return (
+      self._connection.clients(self.client)
+      .projects(self.project)
+      .training_runs()
+      .fetch(
+        filters=json.dumps(
+          [
+            {
+              "field": "experiment",
+              "operator": "==",
+              "value": self.id,
+            }
+          ]
+        )
+      )
+      .iterate_pages()
+    )
 
   def get_best_runs(self):
     return self._connection.aiexperiments(self.id).best_training_runs().fetch().iterate_pages()
 
   def _parse_parameter(self, parameter):
     if isinstance(parameter, Parameter):
       parameter = parameter.as_json(parameter)
-      for attr in ['constraints', 'conditions']:
+      for attr in ["constraints", "conditions"]:
         if not parameter.get(attr):
           parameter.pop(attr, None)
     return parameter
 
   def update(self, **kwargs):
-    if 'parameters' in kwargs:
-      parameters = [self._parse_parameter(p) for p in kwargs['parameters']]
-      kwargs['parameters'] = parameters
+    if "parameters" in kwargs:
+      parameters = [self._parse_parameter(p) for p in kwargs["parameters"]]
+      kwargs["parameters"] = parameters
     kwargs = validate_aiexperiment_update_input(kwargs)
     return self._connection.aiexperiments(self.id).update(**kwargs)
```

### Comparing `sigopt-8.8.0/sigopt/cli/arguments/__init__.py` & `sigopt-8.8.1/sigopt/cli/arguments/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,12 +5,12 @@
 from .cluster_name import cluster_name_option
 from .commands import commands_argument
 from .dockerfile import dockerfile_option
 from .experiment_file import experiment_file_option
 from .experiment_id import experiment_id_argument
 from .identifiers import identifiers_argument, identifiers_help
 from .load_yaml import load_yaml_callback
-from .project import project_option, project_name_option
+from .project import project_name_option, project_option
 from .provider import provider_option
 from .run_file import run_file_option
 from .source_file import source_file_option
 from .validate import validate_id, validate_ids
```

### Comparing `sigopt-8.8.0/sigopt/cli/arguments/identifiers.py` & `sigopt-8.8.1/sigopt/cli/arguments/identifiers.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 def identifiers_callback(ctx, p, value):  # pylint: disable=unused-argument
   try:
     return [parse_identifier(raw) for raw in value]
   except ValueError as ve:
     raise click.BadParameter(str(ve)) from ve
 
+
 identifiers_argument = click.argument(
-  'identifiers',
+  "identifiers",
   nargs=-1,
   callback=identifiers_callback,
 )
 
-identifiers_help = 'IDENTIFIERS can be the name of a run, or one of the following: experiment/[id], run/[id]'
+identifiers_help = "IDENTIFIERS can be the name of a run, or one of the following: experiment/[id], run/[id]"
```

### Comparing `sigopt-8.8.0/sigopt/cli/arguments/load_yaml.py` & `sigopt-8.8.1/sigopt/cli/arguments/load_yaml.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,29 +10,31 @@
 
 
 class ValidatedData:
   def __init__(self, filename, validated_data):
     self.filename = filename
     self.data = validated_data
 
+
 def load_yaml(filename, validator, ignore_no_file):
   if filename is None:
     return None
   try:
     with open(filename) as yaml_fp:
       data = yaml.safe_load(yaml_fp)
   except OSError as ose:
     if ose.errno == errno.ENOENT and ignore_no_file:
       return None
-    raise click.BadParameter(f'Could not open {filename}: {ose}') from ose
+    raise click.BadParameter(f"Could not open {filename}: {ose}") from ose
   except (yaml.parser.ParserError, yaml.scanner.ScannerError) as pe:
-    raise click.BadParameter(f'Could not parse {filename}: {pe}') from pe
+    raise click.BadParameter(f"Could not parse {filename}: {pe}") from pe
 
   try:
     validated_data = validator(data)
   except ValidationError as ve:
-    raise click.BadParameter(f'Bad format in {filename}: {ve}') from ve
+    raise click.BadParameter(f"Bad format in {filename}: {ve}") from ve
 
   return ValidatedData(filename, validated_data)
 
+
 def load_yaml_callback(validator, ignore_no_file=False):
   return lambda ctx, p, value: load_yaml(value, validator, ignore_no_file=ignore_no_file)
```

### Comparing `sigopt-8.8.0/sigopt/cli/arguments/project.py` & `sigopt-8.8.1/sigopt/cli/arguments/project.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,17 +24,19 @@
   Provide the project ID.
   Projects can be created at https://app.sigopt.com/projects or with the command `sigopt create project`.
   If a project ID is not provided then the project ID is determined in the following order:
   first from the SIGOPT_PROJECT environment variable, then by the name of the current directory.
   """,
 )
 
+
 def validate_project_name_callback(ctx, p, value):  # pylint: disable=unused-argument
   if value is None:
     return get_default_project()
   return value
 
+
 project_name_option = click.option(
-  '--project-name',
+  "--project-name",
   callback=validate_project_name_callback,
   help="The name of the project.",
 )
```

### Comparing `sigopt-8.8.0/sigopt/cli/commands/cluster/__init__.py` & `sigopt-8.8.1/sigopt/cli/commands/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.0/sigopt/cli/commands/cluster/base.py` & `sigopt-8.8.1/sigopt/cli/commands/cluster/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,12 +13,13 @@
 
   @property
   def controller(self):
     if self._controller is None:
       self._controller = OrchestrateController.create()
     return self._controller
 
+
 @sigopt_cli.group("cluster")
 @click.pass_context
 def cluster_command(ctx):
-  '''Commands for running SigOpt on Kubernetes clusters.'''
+  """Commands for running SigOpt on Kubernetes clusters."""
   ctx.obj = Context()
```

### Comparing `sigopt-8.8.0/sigopt/cli/commands/cluster/connect.py` & `sigopt-8.8.1/sigopt/cli/commands/cluster/connect.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 from .base import cluster_command
 
 
 @cluster_command.command()
 @cluster_name_option
 @provider_option
 @click.option(
-  '--kubeconfig',
+  "--kubeconfig",
   type=click.Path(exists=True),
   callback=load_yaml_callback(validate_top_level_dict),
-  help='A kubeconfig used to connect to this cluster',
+  help="A kubeconfig used to connect to this cluster",
 )
-@click.option('--registry', help='A custom image registry (host[:port][/path])')
+@click.option("--registry", help="A custom image registry (host[:port][/path])")
 @click.pass_context
 def connect(ctx, cluster_name, provider, kubeconfig, registry):
-  '''Connect to an existing Kubernetes cluster.'''
+  """Connect to an existing Kubernetes cluster."""
   if kubeconfig and provider != provider_to_string(Provider.CUSTOM):
     raise click.BadParameter("Only --provider=custom is allowed with --kubeconfig")
   ctx.obj.controller.connect_to_cluster(cluster_name, provider, registry, kubeconfig and kubeconfig.data)
```

### Comparing `sigopt-8.8.0/sigopt/cli/commands/cluster/create.py` & `sigopt-8.8.1/sigopt/cli/commands/cluster/create.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 
 from ...arguments import load_yaml_callback
 from .base import cluster_command
 
 
 @cluster_command.command()
 @click.option(
-  '-f',
-  '--filename',
+  "-f",
+  "--filename",
   type=click.Path(exists=True),
   callback=load_yaml_callback(validate_top_level_dict),
-  help='cluster config yaml file',
-  default='cluster.yml',
+  help="cluster config yaml file",
+  default="cluster.yml",
 )
 @click.pass_context
 def create(ctx, filename):
-  '''Create a Kubernetes cluster.'''
+  """Create a Kubernetes cluster."""
   ctx.obj.controller.create_cluster(filename.data)
```

### Comparing `sigopt-8.8.0/sigopt/cli/commands/cluster/kubectl.py` & `sigopt-8.8.1/sigopt/cli/commands/cluster/kubectl.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,9 +16,9 @@
 @click.pass_context
 @click.argument(
   "kubectl_arguments",
   nargs=-1,
   type=click.UNPROCESSED,
 )
 def kubectl(ctx, kubectl_arguments):
-  '''Run kubectl with the connected Kubernetes cluster.'''
+  """Run kubectl with the connected Kubernetes cluster."""
   ctx.obj.controller.exec_kubectl(kubectl_arguments)
```

### Comparing `sigopt-8.8.0/sigopt/cli/commands/cluster/optimize.py` & `sigopt-8.8.1/sigopt/cli/commands/cluster/optimize.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,24 +4,26 @@
 import click
 
 from ...arguments import dockerfile_option, project_option
 from ..optimize_base import optimize_command
 from .base import cluster_command
 
 
-@cluster_command.command(context_settings=dict(
-  allow_interspersed_args=False,
-  ignore_unknown_options=True,
-))
+@cluster_command.command(
+  context_settings=dict(
+    allow_interspersed_args=False,
+    ignore_unknown_options=True,
+  )
+)
 @click.pass_context
 @dockerfile_option
 @optimize_command
 @project_option
 def optimize(ctx, command, run_options, experiment_file, dockerfile, project):
-  '''Run an Experiment on the connected Kubernetes cluster.'''
+  """Run an Experiment on the connected Kubernetes cluster."""
   ctx.obj.controller.optimize_on_cluster(
     command=command,
     run_options=run_options,
     optimization_options=experiment_file.data,
     silent=False,
     dockerfile=dockerfile,
     project_id=project,
```

### Comparing `sigopt-8.8.0/sigopt/cli/commands/cluster/status.py` & `sigopt-8.8.1/sigopt/cli/commands/cluster/status.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from ...arguments import identifiers_argument, identifiers_help
 from .base import cluster_command
 
 
 @cluster_command.command(
   context_settings=dict(ignore_unknown_options=True),
-  help=f'''Get the status of the connected Kubernetes cluster. {identifiers_help}''',
+  help=f"""Get the status of the connected Kubernetes cluster. {identifiers_help}""",
 )
 @click.pass_context
 @identifiers_argument
 def status(ctx, identifiers):
   if identifiers:
     for i, identifier in enumerate(identifiers):
       if i > 0:
```

### Comparing `sigopt-8.8.0/sigopt/cli/commands/cluster/test_run.py` & `sigopt-8.8.1/sigopt/cli/commands/cluster/test_run.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,23 +4,26 @@
 import click
 
 from ...arguments import dockerfile_option, project_option
 from ..run_base import run_command
 from .base import cluster_command
 
 
-@cluster_command.command("test-run", context_settings=dict(
-  allow_interspersed_args=False,
-  ignore_unknown_options=True,
-))
+@cluster_command.command(
+  "test-run",
+  context_settings=dict(
+    allow_interspersed_args=False,
+    ignore_unknown_options=True,
+  ),
+)
 @click.pass_context
 @dockerfile_option
 @run_command
 @project_option
 def test_run(ctx, command, run_options, dockerfile, project):
-  '''Start and debug a SigOpt Run on the connected Kubernetes cluster.'''
+  """Start and debug a SigOpt Run on the connected Kubernetes cluster."""
   ctx.obj.controller.test_run_on_cluster(
     command=command,
     run_options=run_options,
     dockerfile=dockerfile,
     project_id=project,
   )
```

### Comparing `sigopt-8.8.0/sigopt/cli/commands/config.py` & `sigopt-8.8.1/sigopt/cli/commands/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,36 +2,40 @@
 #
 # SPDX-License-Identifier: MIT
 import click
 
 from ...config import config as _config
 from .base import sigopt_cli
 
-API_TOKEN_PROMPT = 'SigOpt API token (find at https://app.sigopt.com/tokens/info)'
 
-LOG_COLLECTION_PROMPT = '''Log Collection
+API_TOKEN_PROMPT = "SigOpt API token (find at https://app.sigopt.com/tokens/info)"
+
+LOG_COLLECTION_PROMPT = """Log Collection
 \tThis will capture and upload the standard output and standard error of your
 \tRuns from the CLI and notebook cells so that you can view them on the SigOpt dashboard.
-Enable log collection'''
+Enable log collection"""
 
-CELL_TRACKING_PROMPT = '''Notebook Cell Tracking
+CELL_TRACKING_PROMPT = """Notebook Cell Tracking
 \tThis will record and upload the content of your notebook cells so that you can view them
 \ton the SigOpt dashboard.
-Enable cell tracking'''
+Enable cell tracking"""
+
 
 @sigopt_cli.command()
-@click.option('--api-token', prompt=API_TOKEN_PROMPT)
+@click.option("--api-token", prompt=API_TOKEN_PROMPT)
 @click.option(
-  '--enable-log-collection/--no-enable-log-collection',
+  "--enable-log-collection/--no-enable-log-collection",
   prompt=LOG_COLLECTION_PROMPT,
 )
 @click.option(
-  '--enable-cell-tracking/--no-enable-cell-tracking',
+  "--enable-cell-tracking/--no-enable-cell-tracking",
   prompt=CELL_TRACKING_PROMPT,
 )
 def config(api_token, enable_log_collection, enable_cell_tracking):
-  '''Configure the SigOpt client.'''
-  _config.persist_configuration_options({
-    _config.API_TOKEN_KEY: api_token,
-    _config.CELL_TRACKING_ENABLED_KEY: enable_cell_tracking,
-    _config.LOG_COLLECTION_ENABLED_KEY: enable_log_collection,
-  })
+  """Configure the SigOpt client."""
+  _config.persist_configuration_options(
+    {
+      _config.API_TOKEN_KEY: api_token,
+      _config.CELL_TRACKING_ENABLED_KEY: enable_cell_tracking,
+      _config.LOG_COLLECTION_ENABLED_KEY: enable_log_collection,
+    }
+  )
```

### Comparing `sigopt-8.8.0/sigopt/cli/commands/experiment/archive.py` & `sigopt-8.8.1/sigopt/cli/commands/experiment/archive.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 import click
+
 from sigopt.factory import SigOptFactory
+
 from ...arguments import project_option, validate_ids
 from ..base import archive_command
 
 
 @archive_command.command("experiment")
 @project_option
 @click.argument("EXPERIMENT_IDS", nargs=-1, callback=validate_ids)
 def archive(project, experiment_ids):
-  '''Archive SigOpt Experiments.'''
+  """Archive SigOpt Experiments."""
   factory = SigOptFactory(project)
   factory.set_up_cli()
   for experiment_id in experiment_ids:
     try:
       factory.connection.experiments(experiment_id).delete()
     except Exception as e:
       raise click.ClickException(f"experiment_id: {experiment_id}, {e}") from e
```

### Comparing `sigopt-8.8.0/sigopt/cli/commands/experiment/create.py` & `sigopt-8.8.1/sigopt/cli/commands/experiment/create.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,30 @@
 
 from ...arguments import experiment_file_option, project_option
 from ...utils import create_aiexperiment_from_validated_data
 from ..base import create_command
 
 
 def print_start_worker_help(aiexperiment):
-  msg = f'''
+  msg = f"""
 You can now start workers for this experiment with the following CLI command:
 > sigopt start-worker {aiexperiment.id}
 
 Or use the python client library:
 
   #/usr/bin/env python3
   import sigopt
   experiment = sigopt.get_experiment({aiexperiment.id!r})
   for run in experiment.loop():
     with run:
       ...
-'''
+"""
   print_logger.info(msg)
 
-@create_command.command('experiment')
+
+@create_command.command("experiment")
 @experiment_file_option
 @project_option
 def create(experiment_file, project):
-  '''Create a SigOpt AIExperiment.'''
+  """Create a SigOpt AIExperiment."""
   aiexperiment = create_aiexperiment_from_validated_data(experiment_file, project)
   print_start_worker_help(aiexperiment)
```

### Comparing `sigopt-8.8.0/sigopt/cli/commands/experiment/unarchive.py` & `sigopt-8.8.1/sigopt/cli/commands/experiment/unarchive.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 import click
+
 from sigopt.factory import SigOptFactory
+
 from ...arguments import project_option, validate_ids
 from ..base import unarchive_command
 
 
 @unarchive_command.command("experiment")
 @project_option
 @click.argument("EXPERIMENT_IDS", nargs=-1, callback=validate_ids)
 def unarchive(project, experiment_ids):
-  '''Unarchive SigOpt Experiments.'''
+  """Unarchive SigOpt Experiments."""
   factory = SigOptFactory(project)
   factory.set_up_cli()
   for experiment_id in experiment_ids:
     try:
       factory.unarchive_aiexperiment(experiment_id)
     except Exception as e:
-      raise click.ClickException(f'experiment_id: {experiment_id}, {e}') from e
+      raise click.ClickException(f"experiment_id: {experiment_id}, {e}") from e
```

### Comparing `sigopt-8.8.0/sigopt/cli/commands/init.py` & `sigopt-8.8.1/sigopt/cli/commands/init.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     contents = pkg_resources.resource_string("sigopt.cli.resources", resource)
     with open(path, "wb") as fp:
       fp.write(contents)
       print(f"Wrote file contents for {path}")
   else:
     print(f"Skipping {path}")
 
+
 @sigopt_cli.command()
 def init():
-  '''Initialize a directory for a SigOpt project.'''
+  """Initialize a directory for a SigOpt project."""
   write_file("run.yml", "init_run.txt")
   write_file("experiment.yml", "init_experiment.txt")
   write_file("Dockerfile", "init_dockerfile.txt")
   write_file(".dockerignore", "init_dockerignore.txt")
```

### Comparing `sigopt-8.8.0/sigopt/cli/commands/local/optimize.py` & `sigopt-8.8.1/sigopt/cli/commands/local/optimize.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 from sigopt.config import config
 
 from ...arguments import project_option, source_file_option
-from ...utils import create_aiexperiment_from_validated_data, cli_experiment_loop
+from ...utils import cli_experiment_loop, create_aiexperiment_from_validated_data
 from ..base import sigopt_cli
 from ..optimize_base import optimize_command
 
 
-@sigopt_cli.command(context_settings=dict(
-  allow_interspersed_args=False,
-  ignore_unknown_options=True,
-))
+@sigopt_cli.command(
+  context_settings=dict(
+    allow_interspersed_args=False,
+    ignore_unknown_options=True,
+  )
+)
 @optimize_command
 @source_file_option
 @project_option
 def optimize(command, run_options, experiment_file, source_file, project):
-  '''Run a SigOpt AIExperiment. Requires a path to an experiment YAML file.'''
+  """Run a SigOpt AIExperiment. Requires a path to an experiment YAML file."""
   experiment = create_aiexperiment_from_validated_data(experiment_file, project)
   cli_experiment_loop(config, experiment, command, run_options, source_file)
```

### Comparing `sigopt-8.8.0/sigopt/cli/commands/local/run.py` & `sigopt-8.8.1/sigopt/cli/commands/local/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 from sigopt.config import config
 from sigopt.factory import SigOptFactory
 
-from ...utils import run_user_program
 from ...arguments import project_option, source_file_option
+from ...utils import run_user_program
 from ..base import sigopt_cli
 from ..run_base import run_command
 
 
-@sigopt_cli.command(context_settings=dict(
-  allow_interspersed_args=False,
-  ignore_unknown_options=True,
-))
+@sigopt_cli.command(
+  context_settings=dict(
+    allow_interspersed_args=False,
+    ignore_unknown_options=True,
+  )
+)
 @run_command
 @source_file_option
 @project_option
 def run(command, run_options, source_file, project):
-  '''Create a SigOpt Run.'''
+  """Create a SigOpt Run."""
   factory = SigOptFactory(project)
   factory.set_up_cli()
   with factory.create_run(name=run_options.get("name")) as run_context:
     run_user_program(config, run_context, command, source_file)
```

### Comparing `sigopt-8.8.0/sigopt/cli/commands/local/start_worker.py` & `sigopt-8.8.1/sigopt/cli/commands/local/start_worker.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,29 +2,31 @@
 #
 # SPDX-License-Identifier: MIT
 import click
 
 from sigopt.config import config
 from sigopt.factory import SigOptFactory
 
-from ...utils import cli_experiment_loop
 from ...arguments import experiment_id_argument, source_file_option
+from ...utils import cli_experiment_loop
 from ..base import sigopt_cli
 from ..run_base import run_command
 
 
-@sigopt_cli.command(context_settings=dict(
-  allow_interspersed_args=False,
-  ignore_unknown_options=True,
-))
+@sigopt_cli.command(
+  context_settings=dict(
+    allow_interspersed_args=False,
+    ignore_unknown_options=True,
+  )
+)
 @experiment_id_argument
 @run_command
 @source_file_option
 def start_worker(experiment_id, command, run_options, source_file):
-  '''Start a worker for the given AIExperiment.'''
+  """Start a worker for the given AIExperiment."""
   factory = SigOptFactory.from_default_project()
   factory.set_up_cli()
   try:
     experiment = factory.get_aiexperiment(experiment_id)
   except ValueError as ve:
     raise click.ClickException(str(ve))
   cli_experiment_loop(config, experiment, command, run_options, source_file)
```

### Comparing `sigopt-8.8.0/sigopt/cli/commands/project/create.py` & `sigopt-8.8.1/sigopt/cli/commands/project/create.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,22 +3,23 @@
 # SPDX-License-Identifier: MIT
 import click
 
 from sigopt.exception import ConflictingProjectException
 from sigopt.factory import SigOptFactory
 from sigopt.sigopt_logging import print_logger
 
-from ...arguments import project_option, project_name_option
+from ...arguments import project_name_option, project_option
 from ..base import create_command
 
-@create_command.command('project')
+
+@create_command.command("project")
 @project_option
 @project_name_option
 def create(project, project_name):
-  '''Create a SigOpt Project.'''
+  """Create a SigOpt Project."""
   factory = SigOptFactory(project)
   try:
     factory.create_project(name=project_name)
   except ConflictingProjectException as cpe:
     raise click.ClickException(cpe) from cpe
   print_logger.info("Project '%s' created.", project)
   print_logger.info("To use this project, set the SIGOPT_PROJECT environment variable:")
```

### Comparing `sigopt-8.8.0/sigopt/cli/commands/run_base.py` & `sigopt-8.8.1/sigopt/cli/commands/run_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 import click
 
 from ..arguments import commands_argument, run_file_option
 
 
 def run_command(f):
-
   @commands_argument
   @run_file_option
   @functools.wraps(f)
   def wrapper(*args, commands, run_file, **kwargs):
     if run_file:
       run_options = run_file.data
     else:
```

### Comparing `sigopt-8.8.0/sigopt/cli/commands/training_run/archive.py` & `sigopt-8.8.1/sigopt/cli/commands/training_run/archive.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 import click
+
 from sigopt.factory import SigOptFactory
+
 from ...arguments import project_option, validate_ids
 from ..base import archive_command
 
 
 @archive_command.command("run")
 @project_option
 @click.argument("RUN_IDS", nargs=-1, callback=validate_ids)
 def archive(project, run_ids):
-  '''Archive SigOpt Runs.'''
+  """Archive SigOpt Runs."""
   factory = SigOptFactory(project)
   factory.set_up_cli()
   for run_id in run_ids:
     try:
       factory.archive_run(run_id)
     except Exception as e:
-      raise click.ClickException(f'run_id: {run_id}, {e}') from e
+      raise click.ClickException(f"run_id: {run_id}, {e}") from e
```

### Comparing `sigopt-8.8.0/sigopt/cli/commands/training_run/unarchive.py` & `sigopt-8.8.1/sigopt/cli/commands/training_run/unarchive.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 import click
+
 from sigopt.factory import SigOptFactory
+
 from ...arguments import project_option, validate_ids
 from ..base import unarchive_command
 
+
 @unarchive_command.command("run")
 @project_option
 @click.argument("RUN_IDS", nargs=-1, callback=validate_ids)
 def unarchive(project, run_ids):
-  '''Unarchive SigOpt Runs.'''
+  """Unarchive SigOpt Runs."""
   factory = SigOptFactory(project)
   factory.set_up_cli()
   for run_id in run_ids:
     try:
       factory.unarchive_run(run_id)
     except Exception as e:
-      raise click.ClickException(f'run_id: {run_id}, {e}') from e
+      raise click.ClickException(f"run_id: {run_id}, {e}") from e
```

### Comparing `sigopt-8.8.0/sigopt/cli/resources/init_dockerfile.txt` & `sigopt-8.8.1/sigopt/cli/resources/init_dockerfile.txt`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.0/sigopt/cli/utils.py` & `sigopt-8.8.1/sigopt/cli/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 import subprocess  # nosec
 import sys
 import threading
 
 import click
 
 from sigopt.factory import SigOptFactory
-from sigopt.sigopt_logging import enable_print_logging, print_logger
 from sigopt.run_context import GlobalRunContext
+from sigopt.sigopt_logging import enable_print_logging, print_logger
 
 from .arguments.load_yaml import ValidatedData
 
 
 class StreamThread(threading.Thread):
   def __init__(self, input_stream, output_stream):
     super().__init__()
@@ -31,51 +31,55 @@
     try:
       with self.lock:
         return self.input_stream.readline()
     except ValueError as ve:
       raise StopIteration() from ve
 
   def run(self):
-    for line in iter(self.read_input_line, ''.encode()):
+    for line in iter(self.read_input_line, "".encode()):
       try:
-        data = line.decode('utf-8', 'strict')
+        data = line.decode("utf-8", "strict")
       except UnicodeDecodeError:
-        data = 'Failed to decode binary data to utf-8'
+        data = "Failed to decode binary data to utf-8"
       finally:
         self.buffer.write(data)
         self.output_stream.write(data)
 
   def stop(self):
     with self.lock:
       self.input_stream.close()
     self.join()
     return self.buffer.getvalue()
 
+
 def get_git_hexsha():
   try:
     import git
     from git.exc import InvalidGitRepositoryError
   except ImportError:
     return None
   try:
     repo = git.Repo(search_parent_directories=True)
     return repo.head.object.hexsha
   except InvalidGitRepositoryError:
     return None
 
+
 def get_subprocess_environment(config, run_context, env=None):
   config.set_context_entry(GlobalRunContext(run_context))
   ret = os.environ.copy()
   ret.update(config.get_environment_context())
   ret.update(env or {})
   return ret
 
+
 def run_subprocess(config, run_context, commands, env=None):
   return run_subprocess_command(config, run_context, cmd=commands, env=env)
 
+
 def run_subprocess_command(config, run_context, cmd, env=None):
   env = get_subprocess_environment(config, run_context, env)
   proc_stdout, proc_stderr = subprocess.PIPE, subprocess.PIPE
   try:
     proc = subprocess.Popen(
       cmd,
       env=env,
@@ -112,39 +116,45 @@
     except ProcessLookupError:
       pass
     proc.wait()
     raise
   finally:
     stdout_content, stderr_content = stdout.stop(), stderr.stop()
     if config.log_collection_enabled:
-      run_context.set_logs({
-        'stdout': stdout_content,
-        'stderr': stderr_content,
-      })
+      run_context.set_logs(
+        {
+          "stdout": stdout_content,
+          "stderr": stderr_content,
+        }
+      )
   return return_code
 
+
 def run_user_program(config, run_context, commands, source_code_content):
   source_code = {}
   git_hash = get_git_hexsha()
   if git_hash:
-    source_code['hash'] = git_hash
+    source_code["hash"] = git_hash
   if source_code_content is not None:
-    source_code['content'] = source_code_content
+    source_code["content"] = source_code_content
   run_context.log_source_code(**source_code)
   exit_code = run_subprocess(config, run_context, commands)
   if exit_code != 0:
     print_logger.error("command exited with non-zero status: %s", exit_code)
   return exit_code
 
+
 def setup_cli(config):
-  config.set_user_agent_info(['CLI'])
+  config.set_user_agent_info(["CLI"])
   enable_print_logging()
 
+
 def create_aiexperiment_from_validated_data(experiment_file, project):
   assert isinstance(experiment_file, ValidatedData)
   factory = SigOptFactory(project)
   return factory.create_prevalidated_aiexperiment(experiment_file.data)
 
+
 def cli_experiment_loop(config, experiment, command, run_options, source_code_content):
   for run_context in experiment.loop(name=run_options.get("name")):
     with run_context:
       run_user_program(config, run_context, command, source_code_content)
```

### Comparing `sigopt-8.8.0/sigopt/config.py` & `sigopt-8.8.1/sigopt/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,45 +8,48 @@
 import json
 import os
 
 from .paths import get_root_subdir
 
 
 class UserAgentInfoContext(object):
-  CONFIG_CONTEXT_KEY = 'user_agent_info'
+  CONFIG_CONTEXT_KEY = "user_agent_info"
 
   @classmethod
   def from_config(cls, _config):
     return cls(_config.get_context_data(cls))
 
   def __init__(self, info):
     self.info = info
 
   def to_json(self):
     return self.info
 
+
 class Config(object):
-  API_TOKEN_KEY = 'api_token'
-  CELL_TRACKING_ENABLED_KEY = 'code_tracking_enabled'
-  LOG_COLLECTION_ENABLED_KEY = 'log_collection_enabled'
-  CONTEXT_ENVIRONMENT_KEY = 'SIGOPT_CONTEXT'
+  API_TOKEN_KEY = "api_token"
+  CELL_TRACKING_ENABLED_KEY = "code_tracking_enabled"
+  LOG_COLLECTION_ENABLED_KEY = "log_collection_enabled"
+  CONTEXT_ENVIRONMENT_KEY = "SIGOPT_CONTEXT"
 
   def __init__(self):
-    self._config_json_path = os.path.abspath(os.path.join(
-      get_root_subdir('client'),
-      'config.json',
-    ))
+    self._config_json_path = os.path.abspath(
+      os.path.join(
+        get_root_subdir("client"),
+        "config.json",
+      )
+    )
     self._configuration = self._read_config_json()
     self._json_context = {}
     try:
       encoded_context = os.environ[self.CONTEXT_ENVIRONMENT_KEY]
     except KeyError:
       pass
     else:
-      decoded = base64.b64decode(encoded_context).decode('utf-8')
+      decoded = base64.b64decode(encoded_context).decode("utf-8")
       self._json_context = json.loads(decoded)
     self._object_context = {}
 
   @property
   def config_json_path(self):
     return self._config_json_path
 
@@ -94,22 +97,23 @@
     except (IOError, OSError) as e:
       if e.errno == errno.ENOENT:
         return {}
       raise
 
   def _write_config_json(self, configuration):
     config_path = self._ensure_config_json_path()
-    with open(config_path, 'w') as config_json_fp:
+    with open(config_path, "w") as config_json_fp:
       json.dump(configuration, config_json_fp, indent=2, sort_keys=True)
-      print('', file=config_json_fp)
+      print("", file=config_json_fp)
 
   def persist_configuration_options(self, options):
     self._configuration.update(options)
     self._write_config_json(self._configuration)
 
   def set_user_agent_info(self, info):
     self.set_context_entry(UserAgentInfoContext(info))
 
   def get_user_agent_info(self):
     return UserAgentInfoContext.from_config(self).info
 
+
 config = Config()
```

### Comparing `sigopt-8.8.0/sigopt/defaults.py` & `sigopt-8.8.1/sigopt/defaults.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,54 +1,61 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 import datetime
 import http
-import re
 import os
+import re
 
 from .exception import ApiException, ProjectNotFoundException
 
-INVALID_PROJECT_ID_STRING_CHARACTERS = re.compile(r'[^a-z0-9\-_\.]')
-VALID_PROJECT_ID = re.compile(r'[a-z0-9\-_\.]+\Z')
+
+INVALID_PROJECT_ID_STRING_CHARACTERS = re.compile(r"[^a-z0-9\-_\.]")
+VALID_PROJECT_ID = re.compile(r"[a-z0-9\-_\.]+\Z")
+
 
 def normalize_project_id(project_id):
   project_id = project_id.lower()
-  return re.sub(INVALID_PROJECT_ID_STRING_CHARACTERS, '', project_id)
+  return re.sub(INVALID_PROJECT_ID_STRING_CHARACTERS, "", project_id)
+
 
 def check_valid_project_id(project_id):
   if not VALID_PROJECT_ID.match(project_id):
     raise ValueError(
-      f"Project ID is invalid: '{project_id}'\n"
-      "Project IDs can only consist of lowercase letters, digits, hyphens (-), underscores (_) and periods (.)."
+      f"Project ID is invalid: '{project_id}'\nProject IDs can only consist of"
+      " lowercase letters, digits, hyphens (-), underscores (_) and periods (.)."
     )
 
+
 def get_default_project():
-  project_id = os.environ.get('SIGOPT_PROJECT')
+  project_id = os.environ.get("SIGOPT_PROJECT")
   if project_id:
     check_valid_project_id(project_id)
     return project_id
   cwd_project_id = os.path.basename(os.getcwd())
   project_id = normalize_project_id(cwd_project_id)
   try:
     check_valid_project_id(project_id)
   except ValueError as ve:
     raise ValueError(
-      f"The current directory '{cwd_project_id}' could not be converted into a valid project id."
-
-      " Please rename the directory or use the SIGOPT_PROJECT environment variable instead."
+      f"The current directory '{cwd_project_id}' could not be converted into a"
+      " valid project id. Please rename the directory or use the SIGOPT_PROJECT"
+      " environment variable instead."
     ) from ve
   return project_id
 
+
 def get_default_name(project):
-  datetime_string = datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
-  return f'{project} {datetime_string}'
+  datetime_string = datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
+  return f"{project} {datetime_string}"
+
 
 def get_client_id(connection):
-  return connection.tokens('self').fetch().client
+  return connection.tokens("self").fetch().client
+
 
 def ensure_project_exists(connection, project_id):
   client_id = get_client_id(connection)
   try:
     connection.clients(client_id).projects(project_id).fetch()
   except ApiException as e:
     if e.status_code == http.HTTPStatus.NOT_FOUND:
```

### Comparing `sigopt-8.8.0/sigopt/endpoint.py` & `sigopt-8.8.1/sigopt/endpoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 from .compat import json as simplejson
 
+
 class BoundApiEndpoint(object):
   def __init__(self, bound_resource, endpoint):
     self._bound_resource = bound_resource
     self._endpoint = endpoint
 
   def call_with_json(self, json):
     return self.call_with_params(simplejson.loads(json))
```

### Comparing `sigopt-8.8.0/sigopt/exception.py` & `sigopt-8.8.1/sigopt/exception.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,64 +6,68 @@
 
 class SigOptException(Exception):
   pass
 
 
 class ConnectionException(SigOptException):
   """
-  An exception that occurs when the SigOpt API was unavailable.
-  """
+    An exception that occurs when the SigOpt API was unavailable.
+    """
+
   def __init__(self, message):
     super().__init__(message)
     self.message = message
 
   def __str__(self):
-    return '{0}: {1}'.format(
-      'ConnectionException',
-      self.message if self.message is not None else '',
+    return "{0}: {1}".format(
+      "ConnectionException",
+      self.message if self.message is not None else "",
     )
 
+
 class ApiException(SigOptException):
   """
-  An exception that occurs when the SigOpt API was contacted successfully, but
-  it responded with an error.
-  """
+    An exception that occurs when the SigOpt API was contacted successfully, but
+    it responded with an error.
+    """
+
   def __init__(self, body, status_code):
-    self.message = body.get('message', None) if body is not None else None
+    self.message = body.get("message", None) if body is not None else None
     self._body = body
     if self.message is not None:
       super().__init__(self.message)
     else:
       super().__init__()
     self.status_code = status_code
 
   def __str__(self):
-    return '{0} ({1}): {2}'.format(
-      'ApiException',
+    return "{0} ({1}): {2}".format(
+      "ApiException",
       self.status_code,
-      self.message if self.message is not None else '',
+      self.message if self.message is not None else "",
     )
 
   def to_json(self):
     return copy.deepcopy(self._body)
 
+
 class RunException(SigOptException):
   pass
 
+
 class ConflictingProjectException(SigOptException):
   def __init__(self, project_id):
     super().__init__(f"The project with id '{project_id}' already exists.")
 
+
 class ProjectNotFoundException(SigOptException):
   def __init__(self, project_id):
     super().__init__(
-      f"The project '{project_id}' does not exist.\n"
-      "Try any of the following steps to resolve this:\n"
-      f"  * create a project with the ID '{project_id}' with the command\n"
-      f"    `sigopt create project --project '{project_id}'` or by visiting\n"
-      "    https://app.sigopt.com/projects\n"
-      "  * change the project ID by setting the SIGOPT_PROJECT environment variable or\n"
-      "    by renaming the current directory\n"
-      f"  * (advanced) if the project you want to use is in a different team,\n"
-      "    change your API token by switching to that team and then going to\n"
-      "    https://app.sigopt.com/tokens/info"
+      f"The project '{project_id}' does not exist.\nTry any of the following"
+      f" steps to resolve this:\n  * create a project with the ID '{project_id}'"
+      f" with the command\n    `sigopt create project --project '{project_id}'`"
+      " or by visiting\n    https://app.sigopt.com/projects\n  * change the"
+      " project ID by setting the SIGOPT_PROJECT environment variable or\n    by"
+      " renaming the current directory\n  * (advanced) if the project you want"
+      " to use is in a different team,\n    change your API token by switching"
+      " to that team and then going to\n    https://app.sigopt.com/tokens/info"
     )
```

### Comparing `sigopt-8.8.0/sigopt/factory.py` & `sigopt-8.8.1/sigopt/factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,27 +3,28 @@
 # SPDX-License-Identifier: MIT
 import http
 
 import click
 
 from sigopt.validate import validate_aiexperiment_input
 
-from .defaults import check_valid_project_id, ensure_project_exists, get_default_project, get_client_id
-from .interface import get_connection
-from .sigopt_logging import print_logger
-from .run_factory import BaseRunFactory
-from .exception import ProjectNotFoundException
 from .aiexperiment_context import AIExperimentContext
+from .defaults import check_valid_project_id
+from .defaults import ensure_project_exists as _ensure_project_exists
+from .defaults import get_client_id, get_default_project
+from .exception import ApiException, ConflictingProjectException, ProjectNotFoundException
+from .interface import get_connection
 from .run_context import global_run_context
+from .run_factory import BaseRunFactory
+from .sigopt_logging import print_logger
 from .utils import batcher
-from .exception import ApiException, ConflictingProjectException
 
 
 class SigOptFactory(BaseRunFactory):
-  '''A SigOptFactory creates Runs and AIExperiments that belong to a specified Project.'''
+  """A SigOptFactory creates Runs and AIExperiments that belong to a specified Project."""
 
   _project_id = None
   _assume_project_exists = False
   _client_id = None
 
   @classmethod
   def from_default_project(cls):
@@ -77,15 +78,15 @@
       self.ensure_project_exists()
     except ProjectNotFoundException as pnfe:
       raise click.ClickException(pnfe) from pnfe
 
   def ensure_project_exists(self):
     # if we have already ensured that the project exists then we can skip this step in the future
     if not self._assume_project_exists:
-      self._client_id = ensure_project_exists(self.connection, self.project)
+      self._client_id = _ensure_project_exists(self.connection, self.project)
       self._assume_project_exists = True
     return self._client_id, self.project
 
   def _create_run(self, name, metadata):
     connection = self.connection
     client_id, project_id = self.ensure_project_exists()
     run = connection.clients(client_id).projects(project_id).training_runs().create(name=name, metadata=metadata)
@@ -94,23 +95,28 @@
 
   def upload_runs(self, runs, max_batch_size=10000):
     connection = self.connection
     client_id, project_id = self.ensure_project_exists()
     result = []
     for batch in batcher(runs, max_batch_size):
       result.extend(
-        connection.clients(client_id).projects(project_id).training_runs().create_batch(runs=batch, fields='id').data
+        connection.clients(client_id).projects(project_id).training_runs().create_batch(runs=batch, fields="id").data
       )
     return result
 
   def create_prevalidated_aiexperiment(self, validated_body):
     connection = self.connection
     client_id, project_id = self.ensure_project_exists()
-    aiexperiment = connection.clients(client_id).projects(project_id).aiexperiments().create(
-      **validated_body,
+    aiexperiment = (
+      connection.clients(client_id)
+      .projects(project_id)
+      .aiexperiments()
+      .create(
+        **validated_body,
+      )
     )
     self._on_aiexperiment_created(aiexperiment)
     return AIExperimentContext(aiexperiment, connection=connection)
 
   def create_experiment(self, *args, **kwargs):
     return self.create_aiexperiment(*args, **kwargs)
```

### Comparing `sigopt-8.8.0/sigopt/file_utils.py` & `sigopt-8.8.1/sigopt/file_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,29 +18,32 @@
   if isinstance(image, PILImage):
     image_data = io.BytesIO()
     image.save(image_data, "PNG")
     image_data.seek(0)
     return getattr(image, "filename", None), image_data, "image/png"
   return None
 
+
 def try_load_matplotlib_image(image):
   try:
     from matplotlib.figure import Figure as MatplotlibFigure
   except ImportError:
     return None
   if isinstance(image, MatplotlibFigure):
     image_data = io.BytesIO()
     image.savefig(image_data, format="svg")
     image_data.seek(0)
     return None, image_data, "image/svg+xml"
   return None
 
+
 def try_load_numpy_image(image):
   try:
-    from numpy import ndarray, uint8 as numpy_uint8
+    from numpy import ndarray
+    from numpy import uint8 as numpy_uint8
   except ImportError:
     return None
   if isinstance(image, ndarray):
     channels = 0
     if len(image.shape) == 2:
       channels = 1
     elif len(image.shape) == 3:
@@ -81,54 +84,60 @@
   "image/jpeg",
   "image/png",
   "image/svg+xml",
   "image/webp",
   "image/x-icon",
 }
 
+
 def create_api_image_payload(image):
   if isinstance(image, str):
     content_type = mimetypes.guess_type(image)
     if content_type is None:
       warnings.warn(
         f"Could not guess image type from provided filename, skipping upload: {image}",
         RuntimeWarning,
       )
       return None
     content_type, _ = content_type
     content_type = MIME_TYPE_REMAP.get(content_type, content_type)
     if content_type not in SUPPORTED_IMAGE_MIME_TYPES:
       friendly_supported_types = ", ".join(sorted(SUPPORTED_IMAGE_MIME_TYPES))
       warnings.warn(
-        f"File type `{content_type}` is not supported, please use one of the supported types:"
-        f" {friendly_supported_types}",
+        (
+          f"File type `{content_type}` is not supported, please use one of"
+          f" the supported types: {friendly_supported_types}"
+        ),
         RuntimeWarning,
       )
       return None
     return image, open(image, "rb"), content_type
   payload = try_load_pil_image(image)
   if payload is not None:
     return payload
   payload = try_load_matplotlib_image(image)
   if payload is not None:
     return payload
   payload = try_load_numpy_image(image)
   if payload is not None:
     return payload
   warnings.warn(
-    f"Image type not supported: {type(image)}."
-    " Supported types: str, PIL.Image.Image, matplotlib.figure.Figure, numpy.ndarray",
+    (
+      f"Image type not supported: {type(image)}. Supported types: str,"
+      " PIL.Image.Image, matplotlib.figure.Figure, numpy.ndarray"
+    ),
     RuntimeWarning,
   )
   return None
 
+
 def get_blob_properties(image_data):
   md5 = hashlib.md5()  # nosec
   image_data.seek(0)
   while True:
-    chunk = image_data.read(2 ** 20)
+    chunk = image_data.read(2**20)
     if not chunk:
       break
     md5.update(chunk)
   length = image_data.tell()
   b64_md5 = base64.b64encode(md5.digest()).decode()
   return length, b64_md5
```

### Comparing `sigopt-8.8.0/sigopt/hyperopt/base.py` & `sigopt-8.8.1/sigopt/hyperopt/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,88 +1,88 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
-from .compat import Trials, STATUS_OK, STATUS_FAIL
-from ..local_run_context import LocalRunContext
 from .. import SigOptFactory
 from ..defaults import get_default_name
+from ..local_run_context import LocalRunContext
+from .compat import STATUS_FAIL, STATUS_OK, Trials
 
 
-HYPEROPT_SOURCE_NAME = 'Hyperopt'
+HYPEROPT_SOURCE_NAME = "Hyperopt"
 HYPEROPT_SOURCE_PRIORITY = 1
 
 
 class SigOptTrials(object):
   def __init__(self, project, trials=None, online=True):
     self.factory = SigOptFactory(project)
     self.online = online
     self._trials = trials if trials is not None else Trials()
     self.uploaded_tids = {}
 
     if online:
-      self.saved_refresh = getattr(self._trials, 'refresh')
+      self.saved_refresh = getattr(self._trials, "refresh")
+
       def new_refresh():
         r = self.saved_refresh()
         self.do_refresh()
         return r
-      setattr(self._trials, 'refresh', new_refresh)
+
+      setattr(self._trials, "refresh", new_refresh)
 
   @property
   def parameters(self):
     return [self.trial_parameters(trial) for trial in self.trials]
 
   def upload(self, trials=None, validate=False):
     new_trials = []
     trials = trials if trials is not None else self.trials
     if validate:
       for trial in trials:
         self._trials.assert_valid_trial(trial)
     for trial in trials:
-      result = trial['result']
-      status = result.get('status')
+      result = trial["result"]
+      status = result.get("status")
       if status in [STATUS_OK, STATUS_FAIL]:
-        tid = trial['tid']
+        tid = trial["tid"]
         if tid not in self.uploaded_tids:
           new_trials.append(trial)
     ids = self._upload(new_trials)
     self.uploaded_tids.update(ids)
     return ids
 
   def trial_to_run(self, trial):
-    metadata = {'optimizer': 'hyperopt'}
-    result = trial['result']
-    metrics = {k:v for k, v in result.items() if isinstance(v, (int, float))}
+    metadata = {"optimizer": "hyperopt"}
+    result = trial["result"]
+    metrics = {k: v for k, v in result.items() if isinstance(v, (int, float))}
     parameters = self.trial_parameters(trial)
-    status = result.get('status')
+    status = result.get("status")
     run = LocalRunContext(name=get_default_name(self.factory.project), metadata=metadata)
     run.log_parameters(
       parameters,
       source=HYPEROPT_SOURCE_NAME,
-      source_meta={
-        'sort': HYPEROPT_SOURCE_PRIORITY,
-        'default_show': True
-      })
+      source_meta={"sort": HYPEROPT_SOURCE_PRIORITY, "default_show": True},
+    )
     if status == STATUS_OK:
       if not metrics:
-        raise ValueError('No metrics found in trial result')
+        raise ValueError("No metrics found in trial result")
       run.log_metrics(metrics)
-      run.log_state('completed')
+      run.log_state("completed")
     elif status == STATUS_FAIL:
       run.log_failure()
     else:
-      raise ValueError(f'status must be {STATUS_OK} or {STATUS_FAIL}, actually {status}')
+      raise ValueError(f"status must be {STATUS_OK} or {STATUS_FAIL}, actually {status}")
     return run.get()
 
   def _upload(self, trials):
     runs = [self.trial_to_run(trial) for trial in trials]
     runs = self.factory.upload_runs(runs)
-    return {trial['tid']:run.id for trial, run in zip(trials, runs)}
+    return {trial["tid"]: run.id for trial, run in zip(trials, runs)}
 
   def trial_parameters(self, trial):
-    vals = trial.get('misc', {}).get('vals', {})
+    vals = trial.get("misc", {}).get("vals", {})
     rval = {}
     for k, v in vals.items():
       if v:
         rval[k] = v[0]
     return rval
 
   def do_refresh(self):
```

### Comparing `sigopt-8.8.0/sigopt/interface.py` & `sigopt-8.8.1/sigopt/interface.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,136 +21,137 @@
   Suggestion,
   Token,
   TrainingRun,
 )
 from .request_driver import RequestDriver
 from .resource import ApiResource
 
+
 class ConnectionImpl(object):
   def __init__(self, driver):
     self.driver = driver
 
     suggestions = ApiResource(
       self,
-      'suggestions',
+      "suggestions",
       endpoints=[
-        ApiEndpoint(None, Suggestion, 'POST', 'create'),
-        ApiEndpoint(None, object_or_paginated_objects(Suggestion), 'GET', 'fetch'),
-        ApiEndpoint(None, Suggestion, 'PUT', 'update'),
-        ApiEndpoint(None, None, 'DELETE', 'delete'),
+        ApiEndpoint(None, Suggestion, "POST", "create"),
+        ApiEndpoint(None, object_or_paginated_objects(Suggestion), "GET", "fetch"),
+        ApiEndpoint(None, Suggestion, "PUT", "update"),
+        ApiEndpoint(None, None, "DELETE", "delete"),
       ],
     )
 
     queued_suggestions = ApiResource(
       self,
-      'queued_suggestions',
+      "queued_suggestions",
       endpoints=[
-        ApiEndpoint(None, QueuedSuggestion, 'POST', 'create'),
-        ApiEndpoint(None, object_or_paginated_objects(QueuedSuggestion), 'GET', 'fetch'),
-        ApiEndpoint(None, None, 'DELETE', 'delete'),
-      ]
+        ApiEndpoint(None, QueuedSuggestion, "POST", "create"),
+        ApiEndpoint(None, object_or_paginated_objects(QueuedSuggestion), "GET", "fetch"),
+        ApiEndpoint(None, None, "DELETE", "delete"),
+      ],
     )
 
     observations = ApiResource(
       self,
-      'observations',
+      "observations",
       endpoints=[
-        ApiEndpoint('batch', paginated_objects(Observation), 'POST', 'create_batch'),
-        ApiEndpoint(None, Observation, 'POST', 'create'),
-        ApiEndpoint(None, object_or_paginated_objects(Observation), 'GET', 'fetch'),
-        ApiEndpoint(None, Observation, 'PUT', 'update'),
-        ApiEndpoint(None, None, 'DELETE', 'delete'),
+        ApiEndpoint("batch", paginated_objects(Observation), "POST", "create_batch"),
+        ApiEndpoint(None, Observation, "POST", "create"),
+        ApiEndpoint(None, object_or_paginated_objects(Observation), "GET", "fetch"),
+        ApiEndpoint(None, Observation, "PUT", "update"),
+        ApiEndpoint(None, None, "DELETE", "delete"),
       ],
     )
 
     best_assignments = ApiResource(
       self,
-      'best_assignments',
+      "best_assignments",
       endpoints=[
-        ApiEndpoint(None, object_or_paginated_objects(BestAssignments), 'GET', 'fetch'),
+        ApiEndpoint(None, object_or_paginated_objects(BestAssignments), "GET", "fetch"),
       ],
     )
 
     best_training_runs = ApiResource(
       self,
-      'best_training_runs',
+      "best_training_runs",
       endpoints=[
-        ApiEndpoint(None, paginated_objects(TrainingRun), 'GET', 'fetch'),
+        ApiEndpoint(None, paginated_objects(TrainingRun), "GET", "fetch"),
       ],
     )
 
     importances = ApiResource(
       self,
-      'importances',
+      "importances",
       endpoints=[
-        ApiEndpoint(None, Importances, 'GET', 'fetch'),
+        ApiEndpoint(None, Importances, "GET", "fetch"),
       ],
     )
 
     metric_importances = ApiResource(
       self,
-      'metric_importances',
+      "metric_importances",
       endpoints=[
-        ApiEndpoint(None, paginated_objects(MetricImportances), 'GET', 'fetch'),
+        ApiEndpoint(None, paginated_objects(MetricImportances), "GET", "fetch"),
       ],
     )
 
     stopping_criteria = ApiResource(
       self,
-      'stopping_criteria',
+      "stopping_criteria",
       endpoints=[
-        ApiEndpoint(None, StoppingCriteria, 'GET', 'fetch'),
+        ApiEndpoint(None, StoppingCriteria, "GET", "fetch"),
       ],
     )
 
     checkpoints = ApiResource(
       self,
-      'checkpoints',
+      "checkpoints",
       endpoints=[
-        ApiEndpoint(None, Checkpoint, 'POST', 'create'),
-        ApiEndpoint(None, object_or_paginated_objects(Checkpoint), 'GET', 'fetch')
-      ]
+        ApiEndpoint(None, Checkpoint, "POST", "create"),
+        ApiEndpoint(None, object_or_paginated_objects(Checkpoint), "GET", "fetch"),
+      ],
     )
 
     experiment_training_runs = ApiResource(
       self,
-      'training_runs',
+      "training_runs",
       endpoints=[
-        ApiEndpoint(None, TrainingRun, 'POST', 'create'),
-        ApiEndpoint(None, object_or_paginated_objects(TrainingRun), 'GET', 'fetch'),
-        ApiEndpoint(None, TrainingRun, 'PUT', 'update'),
-        ApiEndpoint(None, None, 'DELETE', 'delete'),
+        ApiEndpoint(None, TrainingRun, "POST", "create"),
+        ApiEndpoint(None, object_or_paginated_objects(TrainingRun), "GET", "fetch"),
+        ApiEndpoint(None, TrainingRun, "PUT", "update"),
+        ApiEndpoint(None, None, "DELETE", "delete"),
       ],
       resources=[checkpoints],
     )
 
     experiment_tokens = ApiResource(
       self,
-      'tokens',
+      "tokens",
       endpoints=[
-        ApiEndpoint(None, Token, 'POST', 'create'),
+        ApiEndpoint(None, Token, "POST", "create"),
       ],
     )
 
     self.tokens = ApiResource(
       self,
-      'tokens',
+      "tokens",
       endpoints=[
-        ApiEndpoint(None, Token, 'GET', 'fetch'),
+        ApiEndpoint(None, Token, "GET", "fetch"),
       ],
     )
 
     self.experiments = ApiResource(
       self,
-      'experiments',
+      "experiments",
       endpoints=[
-        ApiEndpoint(None, Experiment, 'POST', 'create'),
-        ApiEndpoint(None, object_or_paginated_objects(Experiment), 'GET', 'fetch'),
-        ApiEndpoint(None, Experiment, 'PUT', 'update'),
-        ApiEndpoint(None, None, 'DELETE', 'delete'),
+        ApiEndpoint(None, Experiment, "POST", "create"),
+        ApiEndpoint(None, object_or_paginated_objects(Experiment), "GET", "fetch"),
+        ApiEndpoint(None, Experiment, "PUT", "update"),
+        ApiEndpoint(None, None, "DELETE", "delete"),
       ],
       resources=[
         best_assignments,
         best_training_runs,
         experiment_tokens,
         experiment_training_runs,
         importances,
@@ -160,123 +161,123 @@
         stopping_criteria,
         suggestions,
       ],
     )
 
     aiexperiment_training_runs = ApiResource(
       self,
-      'training_runs',
+      "training_runs",
       endpoints=[
-        ApiEndpoint(None, TrainingRun, 'POST', 'create'),
+        ApiEndpoint(None, TrainingRun, "POST", "create"),
       ],
     )
 
     self.aiexperiments = ApiResource(
       self,
-      'aiexperiments',
+      "aiexperiments",
       endpoints=[
-        ApiEndpoint(None, AIExperiment, 'POST', 'create'),
-        ApiEndpoint(None, object_or_paginated_objects(AIExperiment), 'GET', 'fetch'),
-        ApiEndpoint(None, AIExperiment, 'PUT', 'update'),
-        ApiEndpoint(None, None, 'DELETE', 'delete'),
+        ApiEndpoint(None, AIExperiment, "POST", "create"),
+        ApiEndpoint(None, object_or_paginated_objects(AIExperiment), "GET", "fetch"),
+        ApiEndpoint(None, AIExperiment, "PUT", "update"),
+        ApiEndpoint(None, None, "DELETE", "delete"),
       ],
       resources=[
         aiexperiment_training_runs,
         best_training_runs,
       ],
     )
 
     client_experiments = ApiResource(
       self,
-      'experiments',
+      "experiments",
       endpoints=[
-        ApiEndpoint(None, Experiment, 'POST', 'create'),
-        ApiEndpoint(None, paginated_objects(Experiment), 'GET', 'fetch'),
+        ApiEndpoint(None, Experiment, "POST", "create"),
+        ApiEndpoint(None, paginated_objects(Experiment), "GET", "fetch"),
       ],
     )
 
     client_project_aiexperiments = ApiResource(
       self,
-      'aiexperiments',
+      "aiexperiments",
       endpoints=[
-        ApiEndpoint(None, AIExperiment, 'POST', 'create'),
-        ApiEndpoint(None, paginated_objects(AIExperiment), 'GET', 'fetch'),
+        ApiEndpoint(None, AIExperiment, "POST", "create"),
+        ApiEndpoint(None, paginated_objects(AIExperiment), "GET", "fetch"),
       ],
     )
 
     client_project_experiments = ApiResource(
       self,
-      'experiments',
+      "experiments",
       endpoints=[
-        ApiEndpoint(None, paginated_objects(Experiment), 'GET', 'fetch'),
+        ApiEndpoint(None, paginated_objects(Experiment), "GET", "fetch"),
       ],
     )
 
     client_project_training_runs = ApiResource(
       self,
-      'training_runs',
+      "training_runs",
       endpoints=[
-        ApiEndpoint(None, paginated_objects(TrainingRun), 'GET', 'fetch'),
-        ApiEndpoint(None, TrainingRun, 'POST', 'create'),
-        ApiEndpoint('batch', paginated_objects(TrainingRun), 'POST', 'create_batch'),
+        ApiEndpoint(None, paginated_objects(TrainingRun), "GET", "fetch"),
+        ApiEndpoint(None, TrainingRun, "POST", "create"),
+        ApiEndpoint("batch", paginated_objects(TrainingRun), "POST", "create_batch"),
       ],
       resources=[checkpoints],
     )
 
     client_projects = ApiResource(
       self,
-      'projects',
+      "projects",
       endpoints=[
-        ApiEndpoint(None, Project, 'POST', 'create'),
-        ApiEndpoint(None, object_or_paginated_objects(Project), 'GET', 'fetch'),
-        ApiEndpoint(None, Project, 'PUT', 'update'),
+        ApiEndpoint(None, Project, "POST", "create"),
+        ApiEndpoint(None, object_or_paginated_objects(Project), "GET", "fetch"),
+        ApiEndpoint(None, Project, "PUT", "update"),
       ],
       resources=[
         client_project_aiexperiments,
         client_project_experiments,
         client_project_training_runs,
       ],
     )
 
     self.training_runs = ApiResource(
       self,
-      'training_runs',
+      "training_runs",
       endpoints=[
-        ApiEndpoint(None, object_or_paginated_objects(TrainingRun), 'GET', 'fetch'),
-        ApiEndpoint(None, TrainingRun, 'PUT', 'update'),
-        ApiEndpoint(None, None, 'DELETE', 'delete'),
+        ApiEndpoint(None, object_or_paginated_objects(TrainingRun), "GET", "fetch"),
+        ApiEndpoint(None, TrainingRun, "PUT", "update"),
+        ApiEndpoint(None, None, "DELETE", "delete"),
       ],
-      resources=[checkpoints]
+      resources=[checkpoints],
     )
 
     self.clients = ApiResource(
       self,
-      'clients',
+      "clients",
       endpoints=[
-        ApiEndpoint(None, Client, 'GET', 'fetch'),
+        ApiEndpoint(None, Client, "GET", "fetch"),
       ],
       resources=[
         client_experiments,
         client_projects,
       ],
     )
 
     self.organizations = ApiResource(
       self,
-      'organizations',
+      "organizations",
       endpoints=[
-        ApiEndpoint(None, object_or_paginated_objects(Organization), 'GET', 'fetch'),
+        ApiEndpoint(None, object_or_paginated_objects(Organization), "GET", "fetch"),
       ],
     )
 
     self.pki_sessions = ApiResource(
       self,
-      'pki_sessions',
+      "pki_sessions",
       endpoints=[
-        ApiEndpoint(None, Session, 'POST', 'create'),
+        ApiEndpoint(None, Session, "POST", "create"),
       ],
     )
 
   def request(self, method, path, data, headers):
     try:
       return self.driver.request(
         method,
@@ -303,47 +304,50 @@
 
   def set_client_ssl_certs(self, client_ssl_certs):
     self.driver.client_ssl_certs = client_ssl_certs
 
   def set_client_token(self, client_token):
     self.driver.set_client_token(client_token)
 
+
 def instantiate_lite_driver(*args, **kwargs):
   try:
-    from sigoptlite import LocalDriver  # pylint: disable=import-error
+    from sigoptlite import LocalDriver
   except ModuleNotFoundError as mnfe:
     raise ModuleNotFoundError(
       "SigOpt Lite is not installed. It can be installed with the following command: `pip install 'sigopt[lite]'`"
     ) from mnfe
   return LocalDriver(*args, **kwargs)
 
+
 DRIVER_KEY_HTTP = "http"
 DRIVER_KEY_LITE = "lite"
 driver_map = {
   DRIVER_KEY_HTTP: RequestDriver,
   DRIVER_KEY_LITE: instantiate_lite_driver,
 }
 
+
 def create_driver_instance(driver, args, kwargs):
   if isinstance(driver, str):
     try:
       driver = driver_map[driver]
     except KeyError as ke:
       raise ValueError(
-        f"The driver {driver!r} is unknown."
-        f" Only the following options are available: {list(driver_map.keys())}"
+        f"The driver {driver!r} is unknown. Only the following options are available: {list(driver_map.keys())}"
       ) from ke
   return driver(*args, **kwargs)
 
 
 class Connection(object):
   """
-  Client-facing interface for creating Connections.
-  Shouldn't be changed without a major version change.
-  """
+    Client-facing interface for creating Connections.
+    Shouldn't be changed without a major version change.
+    """
+
   def __init__(self, *args, driver="http", **kwargs):
     driver_instance = create_driver_instance(
       driver,
       args,
       kwargs,
     )
     self.impl = ConnectionImpl(driver=driver_instance)
@@ -389,28 +393,34 @@
   @property
   def training_runs(self):
     return self.impl.training_runs
 
   def pki_sessions(self):
     return self.impl.pki_sessions
 
+
 def paginated_objects(api_object):
   def decorator(body, *args, **kwargs):
     return Pagination(api_object, body, *args, **kwargs)
+
   return decorator
 
 
 # Allows response to be a single object of class some_class or a paginated
 # response of objects that come from class some_class
 def object_or_paginated_objects(api_object):
   def decorator(body, *args, **kwargs):
-    if body.get('object') == 'pagination':
+    if body.get("object") == "pagination":
       return Pagination(api_object, body, *args, **kwargs)
     return api_object(body, *args, **kwargs)
+
   return decorator
 
+
 _global_connection = None
+
+
 def get_connection():
   global _global_connection
   if _global_connection is None:
     _global_connection = Connection()
   return _global_connection
```

### Comparing `sigopt-8.8.0/sigopt/lib.py` & `sigopt-8.8.1/sigopt/lib.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,76 +1,83 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 import math as _math
 import numbers as _numbers
-from collections.abc import Mapping as _Mapping, Sequence as _Sequence
+from collections.abc import Mapping as _Mapping
+from collections.abc import Sequence as _Sequence
 
 
 def is_numpy_array(val):
-  return val.__class__.__name__ == 'ndarray'
+  return val.__class__.__name__ == "ndarray"
+
 
 def is_sequence(val):
   """
-  Returns True iff this is a "list-like" type.
-  Avoids the common error that strings are iterable
-  """
+    Returns True iff this is a "list-like" type.
+    Avoids the common error that strings are iterable
+    """
   if is_numpy_array(val):
     return True
-  return (
-    isinstance(val, _Sequence) and
-      not isinstance(val, str) and
-      not isinstance(val, bytes)
-  )
+  return isinstance(val, _Sequence) and not isinstance(val, str) and not isinstance(val, bytes)
+
 
 def is_mapping(val):
   """
-  Returns True iff this is a "dict-like" type
-  """
+    Returns True iff this is a "dict-like" type
+    """
   return isinstance(val, _Mapping)
 
+
 def is_integer(num):
   """
-  Returns True iff this is an integer type. Avoids the common error that bools
-  are instances of int, and handles numpy correctly
-  """
+    Returns True iff this is an integer type. Avoids the common error that bools
+    are instances of int, and handles numpy correctly
+    """
   if isinstance(num, bool):
     return False
   if isinstance(num, _numbers.Integral):
     return True
   return False
 
+
 def is_number(x):
   if isinstance(x, bool):
     return False
   if isinstance(x, float) and _math.isnan(x):
     return False
   return isinstance(x, _numbers.Number) or is_integer(x)
 
+
 def is_string(s):
   return isinstance(s, str)
 
+
 def find(lis, predicate):
   """
-  Finds the first element in lis satisfying predicate, or else None
-  """
+    Finds the first element in lis satisfying predicate, or else None
+    """
   return next((item for item in lis if predicate(item)), None)
 
+
 def remove_nones(mapping):
   return {key: value for key, value in mapping.items() if value is not None}
 
+
 def safe_format(string, *args, **kwargs):
   return string.format(*args, **kwargs)
 
+
 def validate_name(warn, name):
   if not is_string(name):
     raise ValueError(f"The {warn} must be a string, not {type(name).__name__}")
   if not name:
     raise ValueError(f"The {warn} cannot be an empty string")
 
+
 def sanitize_number(warn, name, value):
   if is_integer(value):
     return value
   try:
     value = float(value)
     if _math.isinf(value) or _math.isnan(value):
       raise ValueError
```

### Comparing `sigopt-8.8.0/sigopt/local_run_context.py` & `sigopt-8.8.1/sigopt/local_run_context.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
-from .run_context import BaseRunContext
 import copy
 
+from .run_context import BaseRunContext
+
+
 class LocalRunContext(BaseRunContext):
   def __init__(self, **kwargs):
     self.run = copy.deepcopy(kwargs) if kwargs else {}
 
   def get(self, name=None, default_type=dict):
     if name is None:
       return self.run
-    if not name in self.run:
+    if name not in self.run:
       self.run.setdefault(name, default_type())
     return self.run[name]
 
   def log_state(self, state):
-    self.run['state'] = state
+    self.run["state"] = state
 
   def _set_parameters(self, parameters):
-    self.get('assignments').update(parameters)
+    self.get("assignments").update(parameters)
 
   def _log_failure(self):
-    self.run['state'] = 'failed'
+    self.run["state"] = "failed"
 
   def _log_metadata(self, metadata):
-    self.get('metadata').update(metadata)
+    self.get("metadata").update(metadata)
 
   def _log_metrics(self, metrics):
-    self.get('values').update(metrics)
+    self.get("values").update(metrics)
 
   def _set_parameters_meta(self, parameters_meta):
-    self.get('assignments_meta').update(parameters_meta)
+    self.get("assignments_meta").update(parameters_meta)
 
   def _set_parameters_sources(self, assignments_sources):
-    self.get('assignments_sources').update(assignments_sources)
+    self.get("assignments_sources").update(assignments_sources)
 
   def log_parameters(self, params, source=None, source_meta=None):
     self.set_parameters(params)
     if source is not None:
       self.set_parameters_source(params, source)
       if source_meta is not None:
         self.set_parameters_sources_meta(source, **source_meta)
```

### Comparing `sigopt-8.8.0/sigopt/log_capture.py` & `sigopt-8.8.1/sigopt/log_capture.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,22 +14,22 @@
     self.buffer_stream = None
     self._replace_buffer_stream()
 
   def _replace_buffer_stream(self):
     self.buffer_stream = io.StringIO()
 
   def close(self):
-    raise IOError('MonitorStream cannot be closed')
+    raise IOError("MonitorStream cannot be closed")
 
   @property
   def closed(self):
     return self.original_stream.closed
 
   def fileno(self):
-    raise IOError('MonitorStream has no fileno')
+    raise IOError("MonitorStream has no fileno")
 
   def flush(self):
     return self.original_stream.flush()
 
   def isatty(self):
     return False
 
@@ -39,21 +39,21 @@
   def readline(self, *args, **kwargs):
     return self.original_stream.readline(*args, **kwargs)
 
   def readlines(self, *args, **kwargs):
     return self.original_stream.readlines(*args, **kwargs)
 
   def seek(self, *args, **kwargs):
-    raise IOError('MonitorStream is not seekable')
+    raise IOError("MonitorStream is not seekable")
 
   def seekable(self):
     return False
 
   def tell(self, *args, **kwargs):
-    raise IOError('MonitorStream is not seekable')
+    raise IOError("MonitorStream is not seekable")
 
   def writable(self):
     return True
 
   def write(self, content):
     rval = self.original_stream.write(content)
     with self.buffer_lock:
@@ -66,53 +66,50 @@
 
   def get_buffer_contents(self):
     with self.buffer_lock:
       content = self.buffer_stream.getvalue()
       self._replace_buffer_stream()
     return content
 
+
 class BaseStreamMonitor(object):
   def get_stream_data(self):
     raise NotImplementedError()
 
   def __enter__(self):
     raise NotImplementedError()
 
   def __exit__(self, typ, value, trace):
     raise NotImplementedError()
 
+
 class NullStreamMonitor(BaseStreamMonitor):
   def get_stream_data(self):
     return None
 
   def __enter__(self):
     return self
 
   def __exit__(self, typ, value, trace):
     return None
 
+
 class SystemOutputStreamMonitor(BaseStreamMonitor):
   def __init__(self):
     super().__init__()
     self.monitor_streams = None
 
   def get_stream_data(self):
     if self.monitor_streams is None:
       return None
-    stdout_content, stderr_content = (
-      monitor_stream.get_buffer_contents()
-      for monitor_stream in self.monitor_streams
-    )
+    stdout_content, stderr_content = (monitor_stream.get_buffer_contents() for monitor_stream in self.monitor_streams)
     return stdout_content, stderr_content
 
   def __enter__(self):
     if self.monitor_streams is not None:
-      raise Exception('Already monitoring')
+      raise Exception("Already monitoring")
     self.monitor_streams = MonitorStream(sys.stdout), MonitorStream(sys.stderr)
     sys.stdout, sys.stderr = self.monitor_streams
     return self
 
   def __exit__(self, typ, value, trace):
-    sys.stdout, sys.stderr = (
-      monitor_stream.original_stream
-      for monitor_stream in self.monitor_streams
-    )
+    sys.stdout, sys.stderr = (monitor_stream.original_stream for monitor_stream in self.monitor_streams)
```

### Comparing `sigopt-8.8.0/sigopt/magics.py` & `sigopt-8.8.1/sigopt/magics.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,61 +1,60 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
-import click
 import http
 import io
 import sys
-import yaml
+
+import click
 import IPython
-from IPython.core.magic import (
-  Magics,
-  cell_magic,
-  line_magic,
-  magics_class,
-)
+import yaml
+from IPython.core.magic import Magics, cell_magic, line_magic, magics_class
 
+from .cli.commands.config import API_TOKEN_PROMPT, CELL_TRACKING_PROMPT, LOG_COLLECTION_PROMPT
 from .config import config
-from .cli.commands.config import API_TOKEN_PROMPT, LOG_COLLECTION_PROMPT, CELL_TRACKING_PROMPT
+from .defaults import get_default_project
+from .exception import ApiException
+from .factory import SigOptFactory
 from .log_capture import NullStreamMonitor, SystemOutputStreamMonitor
 from .run_context import global_run_context
-from .factory import SigOptFactory
-from .defaults import get_default_project
-from .validate import validate_aiexperiment_input, ValidationError
 from .sigopt_logging import print_logger
-from .exception import ApiException
+from .validate import ValidationError, validate_aiexperiment_input
 
 
 def get_ns():
-  # NOTE(taylor): inspired by
+  # NOTE: inspired by
   # https://github.com/ipython/ipython/blob/5577a476295146641fbd6f8c992d374b905dc1bc/IPython/core/interactiveshell.py
   # Walk up the stack trace until we find the 'exit' command
   stack_depth = 1
   while True:
     frame = sys._getframe(stack_depth)
     f_locals = frame.f_locals
     try:
-      if isinstance(f_locals['exit'], IPython.core.autocall.ExitAutocall):
+      if isinstance(f_locals["exit"], IPython.core.autocall.ExitAutocall):
         return f_locals
     except KeyError:
       pass
     stack_depth += 1
 
+
 @magics_class
 class SigOptMagics(Magics):
   def __init__(self, shell):
     super().__init__(shell)
     self._experiment = None
     self._factory = SigOptFactory(get_default_project())
 
   def setup(self):
-    config.set_user_agent_info([
-      'Notebook',
-      '/'.join(['IPython', IPython.__version__]),
-    ])
+    config.set_user_agent_info(
+      [
+        "Notebook",
+        "/".join(["IPython", IPython.__version__]),
+      ]
+    )
 
   @cell_magic
   def experiment(self, _, cell):
     ns = get_ns()
 
     # pylint: disable=eval-used
     cell_value = eval(cell, ns)
@@ -85,15 +84,15 @@
       with stream_monitor:
         # pylint: disable=exec-used
         exec(cell, ns)
         # pylint: enable=exec-used
       stream_data = stream_monitor.get_stream_data()
       if stream_data:
         stdout, stderr = stream_data
-        run_context.set_logs({'stdout': stdout, 'stderr': stderr})
+        run_context.set_logs({"stdout": stdout, "stderr": stderr})
     finally:
       global_run_context.clear_run_context()
 
   @cell_magic
   def run(self, line, cell):
     ns = get_ns()
 
@@ -107,15 +106,15 @@
       self.exec_cell(run_context, cell, ns)
 
   @cell_magic
   def optimize(self, line, cell):
     ns = get_ns()
 
     if self._experiment is None:
-      raise Exception('Please create an experiment first with the %%experiment magic command')
+      raise Exception("Please create an experiment first with the %%experiment magic command")
 
     name = None
     if line:
       name = line
 
     self.setup()
 
@@ -126,15 +125,17 @@
   @line_magic
   def sigopt(self, line):
     command = line.strip()
     if command == "config":
       api_token = click.prompt(API_TOKEN_PROMPT, hide_input=True)
       enable_log_collection = click.confirm(LOG_COLLECTION_PROMPT, default=False)
       enable_code_tracking = click.confirm(CELL_TRACKING_PROMPT, default=False)
-      config.persist_configuration_options({
-        config.API_TOKEN_KEY: api_token,
-        config.CELL_TRACKING_ENABLED_KEY: enable_code_tracking,
-        config.LOG_COLLECTION_ENABLED_KEY: enable_log_collection,
-      })
+      config.persist_configuration_options(
+        {
+          config.API_TOKEN_KEY: api_token,
+          config.CELL_TRACKING_ENABLED_KEY: enable_code_tracking,
+          config.LOG_COLLECTION_ENABLED_KEY: enable_log_collection,
+        }
+      )
       self._factory.connection.set_client_token(api_token)
     else:
       raise ValueError(f"Unknown sigopt command: {command}")
```

### Comparing `sigopt-8.8.0/sigopt/objects.py` & `sigopt-8.8.1/sigopt/objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 import copy
 import warnings
 
 from .compat import json
-from .lib import is_sequence, is_mapping, is_integer, is_number, is_numpy_array, is_string
+from .lib import is_integer, is_mapping, is_number, is_numpy_array, is_sequence, is_string
 
 
 class ListOf(object):
   def __init__(self, typ):
     self.type = typ
 
   def __call__(self, value):
@@ -18,20 +18,20 @@
 
 class MapOf(object):
   def __init__(self, value_type, key_type=str):
     self.value_type = value_type
     self.key_type = key_type
 
   def __call__(self, value):
-    d = {self.key_type(k):self.value_type(v) for k, v in value.items()}
+    d = {self.key_type(k): self.value_type(v) for k, v in value.items()}
     return d
 
 
-def DictField(name, type=str):
-  return lambda value: type(value[name])
+def DictField(name, type_=str):
+  return lambda value: type_(value[name])
 
 
 Any = lambda x: x
 
 
 class Field(object):
   def __init__(self, typ):
@@ -42,19 +42,19 @@
       return None
     return self.type(value)
 
 
 class DeprecatedField(Field):
   def __init__(self, typ, recommendation=None):
     super().__init__(typ)
-    self.recommendation = (' ' + recommendation) if recommendation else ''
+    self.recommendation = (" " + recommendation) if recommendation else ""
 
   def __call__(self, value):
     warnings.warn(
-      'This field has been deprecated and may be removed in a future version.{0}'.format(self.recommendation),
+      "This field has been deprecated and may be removed in a future version.{0}".format(self.recommendation),
       DeprecationWarning,
     )
     return super().__call__(value)
 
 
 class BaseApiObject(object):
   def __getattribute__(self, name):
@@ -84,54 +84,52 @@
     except AttributeError:
       return None
     else:
       return subvalue if isinstance(subvalue, Field) else None
 
   def _repr_keys(self):
     attributes = dir(self)
-    attributes = [a for a in attributes if not a.startswith('_')]
+    attributes = [a for a in attributes if not a.startswith("_")]
     attributes = [a for a in attributes if not isinstance(getattr(self.__class__, a), DeprecatedField)]
     attributes = [a for a in attributes if not callable(getattr(self, a))]
     keys_in_json = set(ApiObject.as_json(self._body).keys())
     return keys_in_json.intersection(set(attributes))
 
   @staticmethod
   def _emit_repr(object_name, values_mapping):
     if values_mapping:
-      return '{0}(\n{1}\n)'.format(
+      return "{0}(\n{1}\n)".format(
         object_name,
-        '\n'.join([
-          '  {}={},'.format(key, ApiObject.dumps(value, indent_level=2).lstrip())
-          for key, value
-          in values_mapping.items()
-        ]),
+        "\n".join(
+          [
+            "  {}={},".format(key, ApiObject.dumps(value, indent_level=2).lstrip())
+            for key, value in values_mapping.items()
+          ]
+        ),
       )
-    return '{0}()'.format(object_name)
+    return "{0}()".format(object_name)
 
   def __repr__(self):
     keys = self._repr_keys()
     values = {key: getattr(self, key) for key in keys}
     return BaseApiObject._emit_repr(self.__class__.__name__, values)
 
   def to_json(self):
     return copy.deepcopy(self._body)
 
 
 class ApiObject(BaseApiObject):
   def __init__(self, body, bound_endpoint=None, retrieve_params=None):
     super().__init__()
-    object.__setattr__(self, '_body', body)
-    object.__setattr__(self, '_bound_endpoint', bound_endpoint)
-    object.__setattr__(self, '_retrieve_params', retrieve_params)
+    object.__setattr__(self, "_body", body)
+    object.__setattr__(self, "_bound_endpoint", bound_endpoint)
+    object.__setattr__(self, "_retrieve_params", retrieve_params)
 
   def __eq__(self, other):
-    return (
-      isinstance(other, self.__class__) and
-      self._body == other._body
-    )
+    return isinstance(other, self.__class__) and self._body == other._body
 
   @staticmethod
   def as_json(obj):
     if isinstance(obj, BaseApiObject):
       return obj.to_json()
     if is_mapping(obj):
       c = {}
@@ -146,53 +144,51 @@
       return int(obj)
     if is_number(obj):
       return float(obj)
     return obj
 
   @staticmethod
   def dumps(obj, indent_level=0):
-    indent = ' ' * indent_level
+    indent = " " * indent_level
 
     if isinstance(obj, BaseApiObject):
-      return '{0}{1}'.format(indent, str(obj).replace('\n', '\n{0}'.format(indent)))
+      return "{0}{1}".format(indent, str(obj).replace("\n", "\n{0}".format(indent)))
     if is_mapping(obj):
       if obj:
-        return '{0}{{\n{1},\n{0}}}'.format(
+        return "{0}{{\n{1},\n{0}}}".format(
           indent,
-          ',\n'.join([
-            '  {0}"{1}"={2}'.format(
-              indent,
-              key,
-              ApiObject.dumps(obj[key], indent_level=indent_level + 2).lstrip()
-            )
-            for key
-            in obj
-          ])
+          ",\n".join(
+            [
+              '  {0}"{1}"={2}'.format(
+                indent,
+                key,
+                ApiObject.dumps(obj[key], indent_level=indent_level + 2).lstrip(),
+              )
+              for key in obj
+            ]
+          ),
         )
-      return '{0}{1}'.format(indent, str(obj))
+      return "{0}{1}".format(indent, str(obj))
     if is_numpy_array(obj):
       return ApiObject.dumps(obj.tolist(), indent_level=indent_level)
     if is_sequence(obj):
       if obj:
-        return '{0}[\n{1},\n{0}]'.format(
+        return "{0}[\n{1},\n{0}]".format(
           indent,
-          ',\n'.join([
-            ApiObject.dumps(c, indent_level=indent_level + 2)
-            for c
-            in obj
-          ])
+          ",\n".join([ApiObject.dumps(c, indent_level=indent_level + 2) for c in obj]),
         )
-      return '{0}{1}'.format(indent, str(obj))
+      return "{0}{1}".format(indent, str(obj))
     if is_integer(obj):
-      return '{0}{1}'.format(indent, str(int(obj)))
+      return "{0}{1}".format(indent, str(int(obj)))
     if is_number(obj):
-      return '{0}{1}'.format(indent, str(float(obj)))
+      return "{0}{1}".format(indent, str(float(obj)))
     if is_string(obj):
       return '{0}"{1}"'.format(indent, obj)
-    return '{0}{1}'.format(indent, obj)
+    return "{0}{1}".format(indent, obj)
+
 
 class _DictWrapper(BaseApiObject, dict):
   def __init__(self, body, bound_endpoint=None, retrieve_params=None):
     super().__init__()
     dict.__init__(self, body)
     self._bound_endpoint = bound_endpoint
     self._retrieve_params = retrieve_params
@@ -204,30 +200,28 @@
   def to_json(self):
     return dict(copy.deepcopy(self))
 
   def copy(self):
     return self.__class__(dict.copy(self))
 
   def __eq__(self, other):
-    return (
-      isinstance(other, self.__class__) and
-      dict.__eq__(self, other)
-    )
+    return isinstance(other, self.__class__) and dict.__eq__(self, other)
 
   def __repr__(self):
-    return '{0}({1})'.format(
+    return "{0}({1})".format(
       self.__class__.__name__,
       json.dumps(
         ApiObject.as_json(self._body),
         indent=2,
         sort_keys=True,
-        separators=(',', ': '),
+        separators=(",", ": "),
       ),
     )
 
+
 class Assignments(_DictWrapper):
   pass
 
 
 class Task(ApiObject):
   cost = Field(float)
   name = Field(str)
@@ -271,17 +265,19 @@
   importances = Field(ImportancesMap)
   metric = Field(str)
 
 
 class Metadata(_DictWrapper):
   pass
 
+
 class SysMetadata(_DictWrapper):
   pass
 
+
 class MetricEvaluation(ApiObject):
   name = Field(str)
   value = Field(float)
   value_stddev = Field(float)
 
 
 class Metric(ApiObject):
@@ -322,57 +318,60 @@
   paging = Field(Paging)
 
   def __init__(self, data_cls, body, bound_endpoint=None, retrieve_params=None):
     super().__init__(body, bound_endpoint, retrieve_params)
     self.data_cls = data_cls
 
   def _repr_keys(self):
-    return ['data', 'count', 'paging']
+    return ["data", "count", "paging"]
 
   def __repr__(self):
     values = {
-      'data': self._unsafe_data,
-      'count': self.count,
-      'paging': self.paging,
+      "data": self._unsafe_data,
+      "count": self.count,
+      "paging": self.paging,
     }
     values = {k: v for k, v in values.items() if v is not None}
-    return BaseApiObject._emit_repr('Pagination<{0}>'.format(self.data_cls.__name__), values)
+    return BaseApiObject._emit_repr("Pagination<{0}>".format(self.data_cls.__name__), values)
 
   @property
   def data(self):
     warnings.warn(
-      'The .data field only contains a single page of results, which may be incomplete for large responses.'
-      ' Prefer to use the `.iterate_pages() to ensure that you iterate through all elements in the response.',
+      (
+        "The .data field only contains a single page of results, which may be"
+        " incomplete for large responses. Prefer to use the `.iterate_pages()"
+        " to ensure that you iterate through all elements in the response."
+      ),
       RuntimeWarning,
     )
     return self._unsafe_data
 
   @property
   def _unsafe_data(self):
-    return Field(ListOf(self.data_cls))(self._body.get('data'))
+    return Field(ListOf(self.data_cls))(self._body.get("data"))
 
   def iterate_pages(self):
     # pylint: disable=no-member
     data = self._unsafe_data
     paging = self.paging or Paging({})
 
-    use_before = 'before' in self._retrieve_params or 'after' not in self._retrieve_params
+    use_before = "before" in self._retrieve_params or "after" not in self._retrieve_params
 
     while data:
       for d in data:
         yield d
       next_paging = dict(before=paging.before) if use_before else dict(after=paging.after)
-      if next_paging.get('before') is not None or next_paging.get('after') is not None:
+      if next_paging.get("before") is not None or next_paging.get("after") is not None:
         params = self._retrieve_params.copy()
         if use_before:
-          params['before'] = paging.before
-          params.pop('after', None)
+          params["before"] = paging.before
+          params.pop("after", None)
         else:
-          params.pop('before', None)
-          params['after'] = paging.after
+          params.pop("before", None)
+          params["after"] = paging.after
         response = self._bound_endpoint(**params)
         data = response._unsafe_data
         paging = response.paging
       else:
         data = []
         paging = None
     # pylint: enable=no-member
@@ -398,15 +397,15 @@
   transformation = Field(str)
   tunable = DeprecatedField(bool)
   type = Field(str)
 
 
 class Progress(ApiObject):
   # observation progress fields
-  best_observation = DeprecatedField(Observation, recommendation='Prefer the `best_assignments` endpoint')
+  best_observation = DeprecatedField(Observation, recommendation="Prefer the `best_assignments` endpoint")
   first_observation = Field(Observation)
   last_observation = Field(Observation)
   observation_count = Field(int)
   observation_budget_consumed = Field(float)
   # run progress fields
   active_run_count = Field(int)
   finished_run_count = Field(int)
@@ -458,30 +457,30 @@
   type = Field(str)
 
 
 class TrainingMonitor(ApiObject):
   max_checkpoints = Field(int)
   early_stopping_criteria = Field(ListOf(TrainingEarlyStoppingCriteria))
 
+
 class Experiment(ApiObject):
   budget = Field(float)
   can_be_deleted = DeprecatedField(bool)
   client = Field(str)
   conditionals = Field(ListOf(Conditional))
   created = Field(int)
   development = Field(bool)
   id = Field(str)
   linear_constraints = Field(ListOf(LinearConstraint))
   metadata = Field(Metadata)
   metric = DeprecatedField(
     Metric,
     recommendation=(
-      'Prefer the `metrics` field'
-      '(see https://docs.sigopt.com/core-module-api-references/api-objects/object_experiment)'
-    )
+      "Prefer the `metrics` field(see https://docs.sigopt.com/core-module-api-references/api-objects/object_experiment)"
+    ),
   )
   metrics = Field(ListOf(Metric))
   name = Field(str)
   num_solutions = Field(int)
   observation_budget = Field(int)
   parameters = Field(ListOf(Parameter))
   parallel_bandwidth = Field(int)
@@ -568,15 +567,15 @@
   created = Field(int)
   datasets = Field(ListOf(str))
   deleted = Field(bool)
   experiment = Field(str)
   files = Field(ListOf(str))
   finished = Field(bool)
   id = Field(str)
-  logs = Field(MapOf(DictField('content')))
+  logs = Field(MapOf(DictField("content")))
   metadata = Field(Metadata)
   model = Field(Model)
   name = Field(str)
   object = Field(str)
   observation = Field(str)
   project = Field(str)
   source_code = Field(SourceCode)
```

### Comparing `sigopt-8.8.0/sigopt/orchestrate/aws/service.py` & `sigopt-8.8.1/sigopt/orchestrate/aws/service.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,30 +16,35 @@
 from ..node_groups import ALL_NODE_GROUP_TYPES, NODE_GROUP_TYPE_CPU, NODE_GROUP_TYPE_GPU, NODE_GROUP_TYPE_SYSTEM
 from ..paths import get_executable_path
 from ..provider.constants import Provider
 from ..provider.interface import ProviderInterface
 
 
 def is_cuda_gpu_instance_type(instance_type):
-  prefix, _ = instance_type.split('.', 1)
-  return prefix in ('p4d', 'p3', 'p3dn', 'p2', 'g4dn', 'g3')
+  prefix, _ = instance_type.split(".", 1)
+  return prefix in ("p4d", "p3", "p3dn", "p2", "g4dn", "g3")
 
 
 def catch_aws_permissions_errors(func):
   def wrapper(*args, **kwargs):
     try:
       return func(*args, **kwargs)
     except ClientError as e:
-      code = e.response['Error']['Code']
-      http_status_code = e.response['ResponseMetadata']['HTTPStatusCode']
-      if http_status_code == 403 or code in ('AccessDeniedException', 'UnauthorizedOperation'):
+      code = e.response["Error"]["Code"]
+      http_status_code = e.response["ResponseMetadata"]["HTTPStatusCode"]
+      if http_status_code == 403 or code in (
+        "AccessDeniedException",
+        "UnauthorizedOperation",
+      ):
         raise AwsPermissionsError(e) from e
       raise
+
   return wrapper
 
+
 def make_role_config_map(node_instance_role_arn, cluster_access_role_arn, cluster_access_role_name):
   map_roles = [
     {
       "rolearn": node_instance_role_arn,
       "username": "system:node:{{EC2PrivateDNSName}}",
       "groups": ["system:bootstrappers", "system:nodes"],
     },
@@ -57,80 +62,82 @@
       "namespace": "kube-system",
     },
     "data": {
       "mapRoles": yaml.dump(map_roles),
     },
   }
 
+
 class AwsService(ProviderInterface):
   def __init__(self, services, aws_services):
     super().__init__(services)
     self.aws_services = aws_services
 
   def __getattribute__(self, name):
     attr = super().__getattribute__(name)
     if isinstance(attr, types.MethodType):
       attr = catch_aws_permissions_errors(attr)
     return attr
 
   def describe_kubernetes_cluster(self, cluster_name):
     try:
-      return self.aws_services.eks_service.describe_cluster(cluster_name=cluster_name)['cluster']
+      return self.aws_services.eks_service.describe_cluster(cluster_name=cluster_name)["cluster"]
     except self.aws_services.eks_service.client.exceptions.ResourceNotFoundException as e:
       raise OrchestrateException(
-        f"We cannot find an EKS cluster named '{cluster_name}' using your current AWS credentials."
-        " Did someone delete this cluster?"
+        f"We cannot find an EKS cluster named '{cluster_name}' using your"
+        " current AWS credentials. Did someone delete this cluster?"
       ) from e
 
   def validate_cluster_options(self, cluster_name, node_groups_config, kubernetes_version):
     if kubernetes_version == "latest":
       kubernetes_version = DEFAULT_KUBERNETES_VERSION
     if kubernetes_version:
       assert kubernetes_version in SUPPORTED_KUBERNETES_VERSIONS, (
-        'Unsupported kubernetes version for EKS:'
-        f' {kubernetes_version}. Must be one of: {SUPPORTED_KUBERNETES_VERSIONS}'
+        f"Unsupported kubernetes version for EKS: {kubernetes_version}. Must be one of: {SUPPORTED_KUBERNETES_VERSIONS}"
       )
 
     cpu_nodes_config = node_groups_config.get(NODE_GROUP_TYPE_CPU)
     gpu_nodes_config = node_groups_config.get(NODE_GROUP_TYPE_GPU)
 
-    assert cpu_nodes_config or gpu_nodes_config, "Looks like your cluster config file is not" \
-      " asking us to spin up any CPU or GPU machines."
-    name_regex = '^[a-zA-Z][-a-zA-Z0-9]*$'
-    assert cluster_name and re.match(name_regex, cluster_name), \
-      'Cluster names for AWS must match the regex: /' + name_regex + '/'
+    assert (
+      cpu_nodes_config or gpu_nodes_config
+    ), "Looks like your cluster config file is not asking us to spin up any CPU or GPU machines."
+    name_regex = "^[a-zA-Z][-a-zA-Z0-9]*$"
+    assert cluster_name and re.match(name_regex, cluster_name), (
+      "Cluster names for AWS must match the regex: /" + name_regex + "/"
+    )
 
     if gpu_nodes_config:
-      gpu_instance_type = gpu_nodes_config['instance_type']
-      assert is_cuda_gpu_instance_type(gpu_instance_type), (
-        f"GPUs are not supported on the instance type ({gpu_instance_type})"
-      )
+      gpu_instance_type = gpu_nodes_config["instance_type"]
+      assert is_cuda_gpu_instance_type(
+        gpu_instance_type
+      ), f"GPUs are not supported on the instance type ({gpu_instance_type})"
 
   def _handle_stack_event(self, _, event):
     resource_status = event["ResourceStatus"]
     logical_id = event["LogicalResourceId"]
     print(f"{resource_status} {event['ResourceType']} {logical_id} {event['PhysicalResourceId']}")
     if resource_status.endswith("_FAILED"):
-      print(f"Error {resource_status}: {logical_id}: {event['ResourceStatusReason']}", file=sys.stderr)
+      print(
+        f"Error {resource_status}: {logical_id}: {event['ResourceStatusReason']}",
+        file=sys.stderr,
+      )
 
   def get_node_groups(self, options):
-    return {
-      node_group_type: options.get(node_group_type) or {}
-      for node_group_type in ALL_NODE_GROUP_TYPES
-    }
+    return {node_group_type: options.get(node_group_type) or {} for node_group_type in ALL_NODE_GROUP_TYPES}
 
   def _create_or_update_kubernetes_cluster(self, options, update):
     start_time = datetime.datetime.utcnow().replace(tzinfo=datetime.timezone.utc)
-    cluster_name = options['cluster_name']
-    kubernetes_version = options.get('kubernetes_version') or DEFAULT_KUBERNETES_VERSION
+    cluster_name = options["cluster_name"]
+    kubernetes_version = options.get("kubernetes_version") or DEFAULT_KUBERNETES_VERSION
     node_groups = self.get_node_groups(options)
     self.validate_cluster_options(cluster_name, node_groups, kubernetes_version)
 
-    aws_options = options.get('aws') or {}
-    additional_policies = aws_options.get('additional_policies') or []
+    aws_options = options.get("aws") or {}
+    additional_policies = aws_options.get("additional_policies") or []
 
     common_kwargs = dict(
       cluster_name=cluster_name,
       system_node_config=node_groups[NODE_GROUP_TYPE_SYSTEM],
       cpu_node_config=node_groups[NODE_GROUP_TYPE_CPU],
       gpu_node_config=node_groups[NODE_GROUP_TYPE_GPU],
       key_name=self.aws_services.ec2_service.ensure_key_pair_for_cluster(cluster_name).name,
@@ -141,43 +148,40 @@
       eks_cluster_stack = self.aws_services.cloudformation_service.update_eks_cluster_stack(
         event_handler=self._handle_stack_event,
         **common_kwargs,
       )
     else:
       try:
         eks_cluster_stack = self.aws_services.cloudformation_service.ensure_eks_cluster_stack(
-            **common_kwargs,
+          **common_kwargs,
         )
         self.aws_services.cloudformation_service.wait_for_stack_create_complete(
           eks_cluster_stack.name,
           event_handler=self._handle_stack_event,
           after=start_time,
         )
       except Exception as e:
         print("*" * 50)
         print("ERROR: encountered an error creating EKS cluster; tearing down resources")
         print("*" * 50)
-        # TODO(dan): can we catch something more fine-grained here?
-        # NOTE(dan): since we're just raising here anyway, we don't need to try-except?
+        # TODO: can we catch something more fine-grained here?
+        # NOTE: since we're just raising here anyway, we don't need to try-except?
         self.aws_services.cloudformation_service.ensure_eks_cluster_stack_deleted(
           cluster_name,
           self._handle_stack_event,
         )
         raise e
     eks_cluster_stack.reload()
-    eks_cluster_stack_outputs = {
-      o['OutputKey']: o['OutputValue']
-      for o in eks_cluster_stack.outputs
-    }
+    eks_cluster_stack_outputs = {o["OutputKey"]: o["OutputValue"] for o in eks_cluster_stack.outputs}
     node_instance_role_arn = eks_cluster_stack_outputs["NodeInstanceRoleArn"]
 
     for policy_arn in additional_policies:
       self.aws_services.iam_service.attach_policy(node_instance_role_arn, policy_arn)
 
-    # NOTE(taylor): no reason to update the autoscaler role stack yet, just create it if it doesn't already exist
+    # NOTE: no reason to update the autoscaler role stack yet, just create it if it doesn't already exist
     eks_cluster = self.aws_services.eks_service.describe_cluster(cluster_name)
     self.aws_services.iam_service.ensure_eks_oidc_provider(eks_cluster)
     eks_cluster_autoscaler_role_stack = (
       self.aws_services.cloudformation_service.ensure_eks_cluster_autoscaler_role_stack(
         cluster_name=cluster_name,
         cluster_oidc_provider_url=eks_cluster["cluster"]["identity"]["oidc"]["issuer"],
       )
@@ -188,31 +192,31 @@
       after=start_time,
     )
 
     if not update:
       self._connect_kubernetes_cluster(cluster_name=cluster_name, ignore_role=True)
       self.test_kubernetes_cluster(cluster_name=cluster_name, ignore_role=True)
 
-      # NOTE(taylor): no reason to update the aws-auth config map yet
+      # NOTE: no reason to update the aws-auth config map yet
       role_arn = eks_cluster_stack_outputs["ClusterAccessRoleArn"]
       role_name = eks_cluster_stack_outputs["ClusterAccessRoleName"]
       role_config_map = make_role_config_map(
         node_instance_role_arn=node_instance_role_arn,
         cluster_access_role_arn=role_arn,
         cluster_access_role_name=role_name,
       )
       self.services.kubernetes_service.ensure_config_map(role_config_map)
 
     self._disconnect_kubernetes_cluster(cluster_name=cluster_name)
 
-    print('Testing your kubernetes configuration, you may see an error below but we should be able to resolve it...')
+    print("Testing your kubernetes configuration, you may see an error below but we should be able to resolve it...")
     self._connect_kubernetes_cluster(cluster_name=cluster_name)
-    print('Successfully tested your kubernetes configuration, if you saw any errors above you may ignore them...')
+    print("Successfully tested your kubernetes configuration, if you saw any errors above you may ignore them...")
     self._test_cluster_access_role(cluster_name=cluster_name, retries=3)
-    # Note(Nakul): We disconnect and reconnect to solve an intermittent issue where the kubernetes python client
+    # Note: We disconnect and reconnect to solve an intermittent issue where the kubernetes python client
     # ends up with an empty api key. This is a temporary fix while we resolve the bug. This solves the issue by
     # reloading the key from the config file a second time which I found out works simply by some trial and error.
     self._disconnect_kubernetes_cluster(cluster_name=cluster_name)
     self._connect_kubernetes_cluster(cluster_name=cluster_name)
 
     self.test_kubernetes_cluster(cluster_name=cluster_name)
 
@@ -236,15 +240,16 @@
     cluster_access_role_arn = self.aws_services.iam_service.get_cluster_access_role_arn(cluster_name)
     for try_number in range(retries + 1):
       try:
         self.aws_services.sts_service.assume_role(role_arn=cluster_access_role_arn)
       except ClientError as ce:
         if try_number >= retries:
           raise AwsClusterSharePermissionError(
-            f"You do not have permission to use the role '{cluster_access_role_arn}' for accessing this cluster.\n"
+            "You do not have permission to use the role"
+            f" '{cluster_access_role_arn}' for accessing this cluster.\n"
             "Please read the SigOpt documentation for sharing clusters: "
             "https://docs.sigopt.com/ai-module-api-references/orchestrate/aws_cluster#share-your-kubernetes-cluster"
           ) from ce
         time.sleep(wait_time)
 
   def _connect_kubernetes_cluster(self, cluster_name, ignore_role=False):
     kubeconfig = self.create_kubeconfig(cluster_name, ignore_role)
@@ -265,15 +270,15 @@
     cluster = self.describe_kubernetes_cluster(cluster_name)
 
     if ignore_role:
       cluster_access_role_arn = None
     else:
       cluster_access_role_arn = self.aws_services.iam_service.get_cluster_access_role_arn(cluster_name)
 
-    # TODO(alexandra): optional role_arn is NOT the role ARN used to create the cluster
+    # TODO: optional role_arn is NOT the role ARN used to create the cluster
     # See Step 2 of https://docs.aws.amazon.com/eks/latest/userguide/getting-started.html
 
     kubeconfig = self.services.resource_service.load_yaml("eks", "kubeconfig.yml")
     kubeconfig["clusters"][0]["cluster"] = {
       "server": cluster["endpoint"],
       "certificate-authority-data": cluster["certificateAuthority"]["data"],
     }
@@ -320,21 +325,23 @@
       )
     except Exception as e:
       raise ClusterDestroyError from e
 
   def _node_access_instructions(self, cluster_name):
     filename = self.aws_services.ec2_service.key_pair_location(cluster_name)
     return (
-      '*Optional:'
-      '\n\tTo ssh into any ec2 node in your cluster, use the username `ec2-user` with the key pair located at:'
-      f'\n\t\t{filename}'
-      '\n\tExample:'
-      f'\n\t\tssh -i {filename} ec2-user@<node_dns_name>'
-      '\n\tYou may be required to change security groups on your ec2 instances'
-      '\n\tInstructions: https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/AccessingInstancesLinux.html'
+      "*Optional:"
+      "\n\tTo ssh into any ec2 node in your cluster, use the username `ec2-user`"
+      " with the key pair located at:"
+      f"\n\t\t{filename}"
+      "\n\tExample:"
+      f"\n\t\tssh -i {filename} ec2-user@<node_dns_name>"
+      "\n\tYou may be required to change security groups on your ec2 instances"
+      "\n\tInstructions:"
+      " https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/AccessingInstancesLinux.html"
     )
 
   def create_cluster_object(self, services, name, registry):
     return AWSCluster(
       services=services,
       name=name,
       registry=registry,
```

### Comparing `sigopt-8.8.0/sigopt/orchestrate/cloudformation/cluster-autoscaler-role.yaml` & `sigopt-8.8.1/sigopt/orchestrate/cloudformation/cluster-autoscaler-role.yaml`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.0/sigopt/orchestrate/cloudformation/eks-cluster.yaml` & `sigopt-8.8.1/sigopt/orchestrate/cloudformation/eks-cluster.yaml`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.0/sigopt/orchestrate/cloudformation/eks-node-security.yaml` & `sigopt-8.8.1/sigopt/orchestrate/cloudformation/eks-node-security.yaml`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.0/sigopt/orchestrate/cloudformation/eks-nodegroup.yaml` & `sigopt-8.8.1/sigopt/orchestrate/cloudformation/eks-nodegroup.yaml`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.0/sigopt/orchestrate/cloudformation/eks-vpc.yaml` & `sigopt-8.8.1/sigopt/orchestrate/cloudformation/eks-vpc.yaml`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.0/sigopt/orchestrate/cloudformation/service.py` & `sigopt-8.8.1/sigopt/orchestrate/cloudformation/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,26 +21,27 @@
 
 _call_boto_with_backoff = backoff.on_exception(
   backoff.expo,
   botocore.exceptions.ClientError,
   giveup=lambda ce: ce.response["Error"]["Code"] != "Throttling",
 )
 
+
 class FailedEksStackCreationError(OrchestrateException):
   def __init__(self, stack_name, stack_events):
-    super().__init__(f'Failed to create EKS stack: {stack_name}')
+    super().__init__(f"Failed to create EKS stack: {stack_name}")
     self.stack_name = stack_name
     self.stack_events = stack_events
 
 
 class StackDeletedException(OrchestrateException):
   pass
 
 
-# NOTE(taylor): Anatomy of VPC addresses
+# NOTE: Anatomy of VPC addresses
 # AWS doesn't support masks smaller than /16
 # ipv4: 192     .168     .0       .0
 # bits: 11000000.10101000.00000000.000000000
 # desc: aaaaaaaa.aaaaaaaa.bbcdddee.eeeeeeeee
 #   a: mask
 #   b: future use
 #   c: public/private
@@ -50,19 +51,20 @@
 IP_AZ_ALLOCATED_BITS = 3
 IP_PRIVATE_PUBLIC_BITS = 1
 IP_REMAINING_BITS = 10
 IP_MASK_BITS = 16
 VPC_HOST_IP = "192.168.0.0"
 VPC_BLOCK = f"{VPC_HOST_IP}/{IP_MASK_BITS}"
 
+
 class AwsCloudFormationService(AwsService):
   def __init__(self, services, aws_services, **kwargs):
     super().__init__(services, aws_services)
-    self._client = boto3.client('cloudformation', **kwargs)
-    self._cloudformation = boto3.resource('cloudformation', **kwargs)
+    self._client = boto3.client("cloudformation", **kwargs)
+    self._cloudformation = boto3.resource("cloudformation", **kwargs)
     self.ec2 = boto3.client("ec2", **kwargs)
 
   @property
   def client(self):
     return self._client
 
   @property
@@ -82,22 +84,21 @@
       StackName=self.eks_cluster_autoscaler_role_stack_name(cluster_name),
       TemplateBody=sg_template,
       Parameters=[
         dict(
           ParameterKey=k,
           ParameterValue=v,
         )
-        for (k, v)
-        in [
+        for (k, v) in [
           ("ClusterName", cluster_name),
           ("ClusterOIDCProviderURL", cluster_oidc_provider_url),
         ]
       ],
       Capabilities=[
-        'CAPABILITY_IAM',
+        "CAPABILITY_IAM",
       ],
     )
 
   def delete_eks_cluster_autoscaler_role_stack(self, cluster_name):
     self.describe_eks_cluster_autoscaler_role_stack(cluster_name).delete()
 
   def describe_eks_cluster_autoscaler_role_stack(self, cluster_name):
@@ -108,15 +109,18 @@
       self.create_eks_cluster_autoscaler_role_stack(cluster_name, *args, **kwargs)
     except self.client.exceptions.AlreadyExistsException:
       pass
 
     return self.describe_eks_cluster_autoscaler_role_stack(cluster_name)
 
   def ensure_eks_cluster_autoscaler_role_stack_deleted(self, cluster_name, event_handler=None):
-    self._ensure_stack_deleted(self.eks_cluster_autoscaler_role_stack_name(cluster_name), event_handler=event_handler)
+    self._ensure_stack_deleted(
+      self.eks_cluster_autoscaler_role_stack_name(cluster_name),
+      event_handler=event_handler,
+    )
 
   def eks_cluster_stack_name(self, cluster_name):
     return f"{cluster_name}-stack"
 
   def upload_stack_template(self, template_name):
     return self.aws_services.s3_service.upload_resource_by_hash(
       path_prefix="stack_templates",
@@ -133,41 +137,45 @@
       result = _call_boto_with_backoff(func)(**params)
       yield from result[results_key]
       next_token = result.get("NextToken")
       if not next_token:
         return
 
   def get_compatible_availability_zones_for_instance_types(self, instance_types, az_count, prev_azs=None):
-    supported_azs = set.intersection(*(
-      set(
-        r["Location"] for r in self._page_boto(
-          self.ec2.describe_instance_type_offerings,
-          {
-            "LocationType": "availability-zone",
-            "Filters": [
-              {"Name": "instance-type", "Values": [it]},
-            ],
-          },
-          "InstanceTypeOfferings",
+    supported_azs = set.intersection(
+      *(
+        set(
+          r["Location"]
+          for r in self._page_boto(
+            self.ec2.describe_instance_type_offerings,
+            {
+              "LocationType": "availability-zone",
+              "Filters": [
+                {"Name": "instance-type", "Values": [it]},
+              ],
+            },
+            "InstanceTypeOfferings",
+          )
         )
+        for it in instance_types
       )
-      for it in instance_types
-    ))
+    )
     assert len(supported_azs) >= az_count, (
-      "Not able to find enough supported availability zones for all of the provided instance types:"
-      f" instance types: {instance_types}, required zone count: {az_count}, supported zones: {supported_azs}"
+      "Not able to find enough supported availability zones for all of the"
+      f" provided instance types: instance types: {instance_types}, required zone"
+      f" count: {az_count}, supported zones: {supported_azs}"
     )
     if prev_azs:
       if not all(az in supported_azs for az in prev_azs):
         raise ValueError("The supported availability zones are not compatible with the previous availability zones")
       return prev_azs
     return sorted(supported_azs)[:az_count]
 
   def get_cidr_block(self, public, az):
-    # NOTE(taylor): ">" = big endian (most significant bit first), "I" = unsigned integer
+    # NOTE: ">" = big endian (most significant bit first), "I" = unsigned integer
     network_i = struct.unpack(">I", socket.inet_aton(VPC_HOST_IP))[0]
     if not public:
       network_i |= 1 << (IP_REMAINING_BITS + IP_AZ_ALLOCATED_BITS)
     zone_number = ord(az[-1]) - ord("a")
     assert 0 <= zone_number <= (1 << IP_AZ_ALLOCATED_BITS)
     network_i |= zone_number << IP_REMAINING_BITS
     network = socket.inet_ntoa(struct.pack(">I", network_i))
@@ -223,28 +231,25 @@
         (cpu_max_nodes, cpu_instance_type),
         (gpu_max_nodes, gpu_instance_type),
       ]
       if max_nodes > 0
     ]
     prev_azs = None
     if stack:
-      prev_parameters = {
-        p["ParameterKey"]: p["ParameterValue"]
-        for p in stack.parameters
-      }
-      # NOTE(taylor): Changing availability zones is extremely complicated, maybe even impossible without creating a new
+      prev_parameters = {p["ParameterKey"]: p["ParameterValue"] for p in stack.parameters}
+      # NOTE: Changing availability zones is extremely complicated, maybe even impossible without creating a new
       # cluster. This is because the EKS cluster is created with specific subnets that can't be modified.
       prev_azs = (prev_parameters["AZ01"], prev_parameters["AZ02"])
 
     try:
       az1, az2 = self.get_compatible_availability_zones_for_instance_types(instance_types, 2, prev_azs)
     except ValueError as ve:
       raise Exception(
-        "The requested update cannot be done in-place."
-        " Please destroy your existing cluster and make a new one if you would like to proceed."
+        "The requested update cannot be done in-place. Please destroy your"
+        " existing cluster and make a new one if you would like to proceed."
       ) from ve
 
     for param, public, az in [
       ("PublicSubnet01Block", True, az1),
       ("PublicSubnet02Block", True, az2),
       ("PrivateSubnet01Block", False, az1),
       ("PrivateSubnet02Block", False, az2),
@@ -268,16 +273,15 @@
       StackName=self.eks_cluster_stack_name(cluster_name),
       TemplateURL=eks_cluster_stack_template_url,
       Parameters=[
         dict(
           ParameterKey=k,
           ParameterValue=v,
         )
-        for (k, v)
-        in parameters.items()
+        for (k, v) in parameters.items()
       ],
       Capabilities=[
         "CAPABILITY_IAM",
         "CAPABILITY_NAMED_IAM",
       ],
     )
 
@@ -360,15 +364,15 @@
     stack.reload()
     return stack
 
   def get_stack_status(self, stack_name_or_id):
     stack = self.cloudformation.Stack(stack_name_or_id)
     return _call_boto_with_backoff(lambda: stack.stack_status)()
 
-  # NOTE(taylor): if the stack was deleted then describe_stack_events raises a Throttling error.
+  # NOTE: if the stack was deleted then describe_stack_events raises a Throttling error.
   # We need to make sure a new error gets raised to indicate that the resource does not exist anymore.
   def _describe_stack_events_page(self, StackName, **kwargs):
     try:
       return self.client.describe_stack_events(StackName=StackName, **kwargs)
     except botocore.exceptions.ClientError as ce:
       try:
         stack_status = self.get_stack_status(StackName)
@@ -425,15 +429,14 @@
             pass
       if all_stacks:
         time.sleep(sleep_time)
         sleep_time *= backoff_base
     return failures
 
   def _wait_for_stack_change_complete(self, stack_name, expected_status, event_handler=None, after=None):
-
     def maybe_raise_failures(failures, initial_exc):
       if failures:
         failures_str = "\n".join(
           f"{e['ResourceStatus']} {e['ResourceType']} {e['LogicalResourceId']}: {e['ResourceStatusReason']}"
           for e in failures
         )
         exc = Exception(f"Encountered failures while watching stack: {stack_name}\n{failures_str}")
@@ -443,15 +446,15 @@
       if initial_exc:
         raise initial_exc
 
     failures = []
     try:
       self.watch_stack_events(stack_name, event_handler, after=after, failures=failures)
     except KeyboardInterrupt as ke:
-      # NOTE(taylor): surface any creation errors with a keyboard interrupt,
+      # NOTE: surface any creation errors with a keyboard interrupt,
       # since the user might have interrupted the command after observing resources being deleted
       maybe_raise_failures(failures, ke)
     maybe_raise_failures(failures, None)
 
     stack = self.cloudformation.Stack(stack_name)
     assert stack.stack_status == expected_status, f"Expected {expected_status}, got {stack.stack_status}"
 
@@ -472,22 +475,18 @@
       if ce.response["Error"]["Code"] == "ValidationError":
         return
       raise
 
     after = datetime.datetime.utcnow().replace(tzinfo=datetime.timezone.utc)
     stack.delete()
     self.watch_stack_events(stack.stack_id, event_handler, after=after)
-    self.client.get_waiter('stack_delete_complete').wait(StackName=stack.stack_id)
+    self.client.get_waiter("stack_delete_complete").wait(StackName=stack.stack_id)
 
   def get_stack_output(self, stack, output_key):
     outputs = stack.outputs
     if outputs is None:
       return None
-    return next(
-      o["OutputValue"]
-      for o in outputs
-      if o["OutputKey"] == output_key
-    )
+    return next(o["OutputValue"] for o in outputs if o["OutputKey"] == output_key)
 
   def get_node_instance_role_arn(self, cluster_name):
     cluster_stack = self.describe_eks_cluster_stack(cluster_name)
     return self.get_stack_output(cluster_stack, "NodeInstanceRoleArn")
```

### Comparing `sigopt-8.8.0/sigopt/orchestrate/cluster/context.py` & `sigopt-8.8.1/sigopt/orchestrate/cluster/context.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.0/sigopt/orchestrate/cluster/errors.py` & `sigopt-8.8.1/sigopt/orchestrate/cluster/errors.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,35 +9,35 @@
   pass
 
 
 class MultipleClustersConnectionError(ClusterError):
   def __init__(self, connected_clusters):
     safe_str = "\n\t".join(connected_clusters)
     super().__init__(
-      "You are currently connected to more than one cluster, all of which are listed below."
-      "\nPlease disconnect from some of these clusters before re-running your command."
-      "\nConnected clusters:"
-      f":\n\t{safe_str}"
+      "You are currently connected to more than one cluster, all of which are"
+      " listed below.\nPlease disconnect from some of these clusters before"
+      f" re-running your command.\nConnected clusters::\n\t{safe_str}"
     )
     self.connected_clusters = connected_clusters
 
 
 class PleaseDisconnectError(ClusterError):
   def __init__(self, current_cluster_name):
-    super().__init__(
-      f"Please disconnect from this cluster before re-running your command: {current_cluster_name}"
-    )
+    super().__init__(f"Please disconnect from this cluster before re-running your command: {current_cluster_name}")
     self.current_cluster_name = current_cluster_name
 
 
 class NotConnectedError(ClusterError):
   def __init__(self):
     super().__init__("You are not currently connected to any cluster")
 
 
 class AlreadyConnectedException(ClusterError):
   def __init__(self, current_cluster_name):
     super().__init__(
-      f"You are already connected this cluster: {current_cluster_name}."
-      f" Please run `{CLI_NAME} cluster test` to verify the details of your connection.",
+      (
+        f"You are already connected this cluster: {current_cluster_name}."
+        f" Please run `{CLI_NAME} cluster test` to verify the details of your"
+        " connection."
+      ),
     )
     self.current_cluster_name = current_cluster_name
```

### Comparing `sigopt-8.8.0/sigopt/orchestrate/cluster/object.py` & `sigopt-8.8.1/sigopt/orchestrate/cluster/object.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,40 +38,42 @@
 
   def get_registry_login_credentials(self, repository):
     raise NotImplementedError()
 
   def generate_image_tag(self, repository):
     raise NotImplementedError()
 
+
 class AWSCluster(Cluster):
   @property
   def provider(self):
     return Provider.AWS
 
   def get_registry_login_credentials(self, repository):
     ecr_service = self.provider_service.aws_services.ecr_service
-    registry_id = ecr_service.ensure_repositories([repository])['repositories'][0]['registryId']
-    authorization_data = ecr_service.get_authorization_token([registry_id])['authorizationData'][0]
-    authorization_token = authorization_data['authorizationToken']
+    registry_id = ecr_service.ensure_repositories([repository])["repositories"][0]["registryId"]
+    authorization_data = ecr_service.get_authorization_token([registry_id])["authorizationData"][0]
+    authorization_token = authorization_data["authorizationToken"]
     decoded_bytes = base64.b64decode(authorization_token)
-    (username, password) = decoded_bytes.decode('utf-8').split(':')
-    proxy_endpoint = authorization_data['proxyEndpoint']
+    (username, password) = decoded_bytes.decode("utf-8").split(":")
+    proxy_endpoint = authorization_data["proxyEndpoint"]
     return DockerLoginCredentials(
       registry=proxy_endpoint,
       username=username,
       password=password,
     )
 
   def generate_image_tag(self, repository):
     if self.registry is not None:
       return f"{self.registry}/{repository}"
 
     ecr_service = self.provider_service.aws_services.ecr_service
     descriptions = ecr_service.ensure_repositories([repository])
-    return descriptions['repositories'][0]['repositoryUri']
+    return descriptions["repositories"][0]["repositoryUri"]
+
 
 class CustomCluster(Cluster):
   @property
   def provider(self):
     return Provider.CUSTOM
 
   def get_registry_login_credentials(self, repository):
```

### Comparing `sigopt-8.8.0/sigopt/orchestrate/cluster/service.py` & `sigopt-8.8.1/sigopt/orchestrate/cluster/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,37 +59,37 @@
       self.services.cluster_metadata_service.write_metadata(cluster)
       return self.test()
 
   def create(self, options):
     try:
       self.assert_is_disconnected()
     except PleaseDisconnectError as e:
-      if e.current_cluster_name == options.get('cluster_name', ''):
+      if e.current_cluster_name == options.get("cluster_name", ""):
         raise AlreadyConnectedException(e.current_cluster_name) from e
       raise
 
     self.services.options_validator_service.validate_cluster_options(**options)
-    cluster_name = options.get('cluster_name', '')
+    cluster_name = options.get("cluster_name", "")
 
-    provider_string = options.get('provider', '')
+    provider_string = options.get("provider", "")
     provider = string_to_provider(provider_string)
     provider_service = self.services.provider_broker.get_provider_service(provider)
 
     with DisconnectOnException(cluster_name, self.services):
       cluster = provider_service.create_kubernetes_cluster(options)
       self.services.kubernetes_service.ensure_orchestrate_namespace()
       self.services.cluster_metadata_service.write_metadata(cluster)
       self.services.kubernetes_service.wait_until_nodes_are_ready()
       return cluster.name
 
   def update(self, options):
     self.services.options_validator_service.validate_cluster_options(**options)
-    cluster_name = options.get('cluster_name', '')
+    cluster_name = options.get("cluster_name", "")
 
-    provider_string = options.get('provider', '')
+    provider_string = options.get("provider", "")
     provider = string_to_provider(provider_string)
     provider_service = self.services.provider_broker.get_provider_service(provider)
 
     with DisconnectOnException(cluster_name, self.services):
       cluster = provider_service.update_kubernetes_cluster(options)
       self.services.kubernetes_service.ensure_orchestrate_namespace()
       self.services.kubernetes_service.wait_until_nodes_are_ready()
@@ -99,43 +99,39 @@
     provider = string_to_provider(provider_string)
     provider_service = self.services.provider_broker.get_provider_service(provider)
     provider_service.destroy_kubernetes_cluster(cluster_name=cluster_name)
     self.services.cluster_metadata_service.ensure_metadata_deleted(cluster_name=cluster_name)
 
   def disconnect(self, cluster_name, disconnect_all):
     if (cluster_name and disconnect_all) or (not cluster_name and not disconnect_all):
-      raise ClusterError('Must provide exactly one of --cluster-name <cluster_name> and --all')
+      raise ClusterError("Must provide exactly one of --cluster-name <cluster_name> and --all")
 
     try:
       current_cluster_name = self.assert_is_connected()
       if cluster_name is not None and current_cluster_name != cluster_name:
         raise PleaseDisconnectError(current_cluster_name)
     except MultipleClustersConnectionError:
       if not disconnect_all:
         raise
 
     for cname in self.connected_clusters():
       try:
         self.services.cluster_metadata_service.ensure_metadata_deleted(cluster_name=cname)
         self.services.kubernetes_service.ensure_config_deleted(cluster_name=cname)
-        self.services.logging_service.warning(f'Successfully disconnected from {cname}')
+        self.services.logging_service.warning(f"Successfully disconnected from {cname}")
       except Exception as e:
-        raise ClusterError(
-          f'Looks like an error occured while attempting to disconnect from cluster "{cname}".'
-        ) from e
+        raise ClusterError(f'Looks like an error occured while attempting to disconnect from cluster "{cname}".') from e
 
   def get_connected_cluster(self):
     cluster_name = self.assert_is_connected()
     return self.services.cluster_metadata_service.read_metadata(cluster_name)
 
   def test(self):
     cluster = self.get_connected_cluster()
     provider_service = self.services.provider_broker.get_provider_service(cluster.provider)
 
     try:
       provider_service.test_kubernetes_cluster(cluster_name=cluster.name)
     except Exception as e:
-      raise ClusterError(
-        f'Looks like an error occured while testing cluster "{cluster.name}".'
-      ) from e
+      raise ClusterError(f'Looks like an error occured while testing cluster "{cluster.name}".') from e
 
     return cluster
```

### Comparing `sigopt-8.8.0/sigopt/orchestrate/cluster_metadata/errors.py` & `sigopt-8.8.1/sigopt/orchestrate/cluster_metadata/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 from ..exceptions import OrchestrateException
 
 
 class MetadataError(OrchestrateException):
   def __init__(self, cluster_name, unformatted_msg):
     formatted_msg = unformatted_msg.format(cluster_name=cluster_name)
     super().__init__(
-      f'{formatted_msg} Disconnecting and then reconnecting should resolve the issue.',
+      f"{formatted_msg} Disconnecting and then reconnecting should resolve the issue.",
     )
     self.cluster_name = cluster_name
 
 
 class MetadataNotFoundError(MetadataError):
   def __init__(self, cluster_name):
     super().__init__(
       cluster_name,
-      f'We could not find metadata for cluster {cluster_name}.',
+      f"We could not find metadata for cluster {cluster_name}.",
     )
 
 
 class MetadataAlreadyExistsError(MetadataError):
   def __init__(self, cluster_name):
     super().__init__(
       cluster_name,
-      f'Looks like metadata for cluster {cluster_name} already exists.',
+      f"Looks like metadata for cluster {cluster_name} already exists.",
     )
```

### Comparing `sigopt-8.8.0/sigopt/orchestrate/cluster_metadata/service.py` & `sigopt-8.8.1/sigopt/orchestrate/cluster_metadata/service.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 import errno
 import os
 
 import yaml
+
 from sigopt.paths import ensure_dir, get_root_subdir
 
 from ..provider.constants import string_to_provider
 from ..services.base import Service
 from .errors import MetadataAlreadyExistsError, MetadataNotFoundError
 
 
 class ClusterMetadataService(Service):
   def __init__(self, services):
     super().__init__(services)
-    self._metadata_dir = get_root_subdir('cluster')
+    self._metadata_dir = get_root_subdir("cluster")
 
   def read_metadata(self, cluster_name):
     metadata_path = self._cluster_metadata_path(cluster_name)
 
     if not os.path.isfile(metadata_path):
       raise MetadataNotFoundError(cluster_name)
 
-    with open(metadata_path, 'r') as f:
+    with open(metadata_path, "r") as f:
       data = yaml.safe_load(stream=f)
 
-    provider = string_to_provider(data['provider'])
+    provider = string_to_provider(data["provider"])
     provider_service = self.services.provider_broker.get_provider_service(provider)
     cluster = provider_service.create_cluster_object(
       services=self.services,
-      name=data['name'],
-      registry=data['registry'],
+      name=data["name"],
+      registry=data["registry"],
     )
     return cluster
 
   def write_metadata(self, cluster):
     data = dict(
       name=cluster.name,
       provider=cluster.provider_string,
@@ -44,15 +45,15 @@
 
     ensure_dir(self._metadata_dir)
     metadata_path = self._cluster_metadata_path(cluster.name)
 
     if os.path.isfile(metadata_path):
       raise MetadataAlreadyExistsError(cluster.name)
 
-    with open(metadata_path, 'w') as f:
+    with open(metadata_path, "w") as f:
       yaml.safe_dump(data, stream=f)
 
   def _delete_metadata(self, cluster_name):
     try:
       os.remove(self._cluster_metadata_path(cluster_name))
     except OSError as e:
       if e.errno == errno.ENOENT:
@@ -62,9 +63,9 @@
   def ensure_metadata_deleted(self, cluster_name):
     try:
       self._delete_metadata(cluster_name)
     except MetadataNotFoundError:
       pass
 
   def _cluster_metadata_path(self, cluster_name):
-    filename = f'metadata-{cluster_name}'
+    filename = f"metadata-{cluster_name}"
     return os.path.join(self._metadata_dir, filename)
```

### Comparing `sigopt-8.8.0/sigopt/orchestrate/common.py` & `sigopt-8.8.1/sigopt/orchestrate/common.py`

 * *Files 25% similar despite different names*

```diff
@@ -15,34 +15,38 @@
 
   def __enter__(self):
     return self.directory
 
   def __exit__(self, *args):
     rmtree(self.directory)
 
+
 class Platform(Enum):
   MAC = 1
   LINUX = 2
 
+
 def current_platform():
-  if sys.platform.startswith('linux'):
+  if sys.platform.startswith("linux"):
     return Platform.LINUX
   if sys.platform == "darwin":
     return Platform.MAC
   raise Exception(
-    f"You are attempting to run SigOpt cluster features on the following platform: {sys.platform}."
-    " Currently, only Mac and Linux are supported."
+    "You are attempting to run SigOpt cluster features on the following platform:"
+    f" {sys.platform}. Currently, only Mac and Linux are supported."
   )
 
+
 def retry_with_backoff(func):
   # pylint: disable=inconsistent-return-statements
   def wrapper(*args, **kwargs):
     NUM_RETRIES = 5
     for i in range(NUM_RETRIES + 1):
       try:
         return func(*args, **kwargs)
       except Exception as e:
-        time.sleep(2 ** i + random.random())  # nosec
+        time.sleep(2**i + random.random())  # nosec
         if i == NUM_RETRIES:
           raise e
+
   # pylint: enable=inconsistent-return-statements
   return wrapper
```

### Comparing `sigopt-8.8.0/sigopt/orchestrate/controller.py` & `sigopt-8.8.1/sigopt/orchestrate/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from collections import defaultdict
 
 import click
 import pint
 import yaml
 from botocore.exceptions import NoRegionError
 
-from sigopt.paths import get_bin_dir, ensure_dir
+from sigopt.paths import ensure_dir, get_bin_dir
 from sigopt.utils import accept_sigopt_not_found
 
 from .cluster.errors import AlreadyConnectedException, ClusterError, MultipleClustersConnectionError, NotConnectedError
 from .docker.service import DockerException, DockerService
 from .exceptions import CheckExecutableError, ModelPackingError, OrchestrateException
 from .identifier import IDENTIFIER_TYPE_EXPERIMENT, IDENTIFIER_TYPE_RUN, parse_identifier
 from .kubernetes.service import ORCHESTRATE_NAMESPACE, CleanupFailedException
@@ -37,14 +37,15 @@
 
 
 def docker_login(cluster, docker_service, repository_name):
   creds = cluster.get_registry_login_credentials(repository_name)
   if creds is not None:
     docker_service.login(creds)
 
+
 class OrchestrateController:
   def __init__(self, services):
     self.services = services
 
   @classmethod
   def create(cls):
     try:
@@ -62,37 +63,37 @@
     self,
     cluster,
     docker_service,
     dockerfile,
     run_options,
     quiet,
   ):
-    image_name = run_options.get('image')
+    image_name = run_options.get("image")
     repository_name, tag = DockerService.get_repository_and_tag(image_name)
     docker_login(cluster, docker_service, repository_name)
 
-    build_image = run_options.get('build_image', True)
+    build_image = run_options.get("build_image", True)
 
     if build_image:
       if not quiet:
-        print('Containerizing and uploading your model, this may take a few minutes...')
+        print("Containerizing and uploading your model, this may take a few minutes...")
       try:
         image_tag = self.services.model_packer_service.build_image(
           docker_service=docker_service,
           repository=repository_name,
           tag=tag,
           quiet=quiet,
           dockerfile=dockerfile,
         )
         image = docker_service.get_image(image_tag)
       except ModelPackingError as mpe:
         msg = str(mpe)
-        match = re.search('manifest for (.*?) not found: manifest unknown: manifest unknown', msg)
+        match = re.search("manifest for (.*?) not found: manifest unknown: manifest unknown", msg)
         if match is not None:
-          msg = f'Unable to find base image {match.groups()[0]} when building your docker container'
+          msg = f"Unable to find base image {match.groups()[0]} when building your docker container"
         raise _ExitException(msg) from mpe
 
     repository_name = cluster.generate_image_tag(repository_name)
     repository_image_tag = DockerService.format_image_name(repository_name, tag)
     if build_image:
       image.tag(repository=repository_name, tag=tag)
       if not quiet:
@@ -111,32 +112,32 @@
     project_id,
     quiet=False,
     optimize=True,
     optimization_options=None,
   ):
     if optimize:
       if not optimization_options:
-        raise OrchestrateException('optimize jobs require an experiment yaml file')
+        raise OrchestrateException("optimize jobs require an experiment yaml file")
 
     repository_name, tag = self.build_and_push_image(
       cluster=cluster,
       docker_service=docker_service,
       dockerfile=dockerfile,
       run_options=run_options,
       quiet=quiet,
     )
 
     resource_options = self.services.gpu_options_validator_service.get_resource_options(run_options)
 
     run_command = command
 
-    job_type_str = 'experiment' if optimize else 'run'
+    job_type_str = "experiment" if optimize else "run"
 
     if not quiet:
-      print('Starting your {}'.format(job_type_str))
+      print("Starting your {}".format(job_type_str))
 
     if optimize:
       return self.services.job_runner_service.start_cluster_experiment(
         repository=repository_name,
         tag=tag,
         resource_options=resource_options,
         optimization_options=optimization_options,
@@ -197,22 +198,24 @@
       pod = event["object"]
       for condition in pod.status.conditions or []:
         if condition.type in ("Ready", "PodScheduled") and condition.status == "False":
           print(f"Pod '{pod.metadata.name}' in bad condition: {condition.reason}: {condition.message}")
         if condition.reason == "Unschedulable":
           print(
             "Hint: If you configured your nodes with sufficient resources"
-            " then you probably just need to wait for the cluster to scale up"
+            " then you probably just need to wait for the cluster to"
+            " scale up"
           )
       for container_status in pod.status.container_statuses or []:
         waiting_state = container_status.state.waiting
         if waiting_state:
           print(
-            f"Container '{container_status.name}' in pod '{pod.metadata.name}' is waiting:"
-            f" {waiting_state.reason}: {waiting_state.message}"
+            f"Container '{container_status.name}' in pod"
+            f" '{pod.metadata.name}' is waiting: {waiting_state.reason}:"
+            f" {waiting_state.message}"
           )
 
     self.services.kubernetes_service.wait_for_pod_to_start(
       label_selector=run_identifier["controller_label_selector"],
       event_handler=check_pod_condition,
     )
     print("controller started, waiting for run to be created...")
@@ -266,111 +269,110 @@
     )
     if quiet:
       print(identifier)
     else:
       print(f'Started "{identifier}"')
 
   def create_cluster(self, options):
-    print('Creating your cluster, this process may take 20-30 minutes or longer...')
+    print("Creating your cluster, this process may take 20-30 minutes or longer...")
 
-    # NOTE(dan): checks again now that we know provider, in case aws iam authenticator is needed
-    check_authenticator_binary(provider=options.get('provider'))
+    # NOTE: checks again now that we know provider, in case aws iam authenticator is needed
+    check_authenticator_binary(provider=options.get("provider"))
     try:
       cluster_name = self.services.cluster_service.create(options=options)
     except ClusterError as pde:
       raise _ExitException(str(pde)) from pde
 
-    print(f'Successfully created kubernetes cluster: {cluster_name}')
+    print(f"Successfully created kubernetes cluster: {cluster_name}")
 
   def update_cluster(self, options):
-    print('Updating your cluster, this process may take 5-10 minutes or longer...')
+    print("Updating your cluster, this process may take 5-10 minutes or longer...")
 
-    # NOTE(dan): checks again now that we know provider, in case aws iam authenticator is needed
-    check_authenticator_binary(provider=options.get('provider'))
+    # NOTE: checks again now that we know provider, in case aws iam authenticator is needed
+    check_authenticator_binary(provider=options.get("provider"))
     cluster_name = self.services.cluster_service.update(options=options)
 
-    print(f'Successfully updated kubernetes cluster: {cluster_name}')
+    print(f"Successfully updated kubernetes cluster: {cluster_name}")
 
   def destroy_connected_cluster(self):
     cluster = self.services.cluster_service.get_connected_cluster()
-    print(f'Destroying cluster {cluster.name}, this process may take 20-30 minutes or longer...')
+    print(f"Destroying cluster {cluster.name}, this process may take 20-30 minutes or longer...")
 
     try:
       self.services.kubernetes_service.cleanup_for_destroy()
     except CleanupFailedException as cfe:
       raise _ExitException(str(cfe)) from cfe
     self.services.cluster_service.destroy(
       cluster_name=cluster.name,
       provider_string=cluster.provider_string,
     )
-    print(f'Successfully destroyed kubernetes cluster: {cluster.name}')
+    print(f"Successfully destroyed kubernetes cluster: {cluster.name}")
 
   def connect_to_cluster(self, cluster_name, provider_string, registry, kubeconfig):
     check_authenticator_binary(provider=provider_string)
 
-    print(f'Connecting to cluster {cluster_name}...')
+    print(f"Connecting to cluster {cluster_name}...")
     try:
       self.services.cluster_service.connect(
         cluster_name=cluster_name,
         provider_string=provider_string,
         kubeconfig=kubeconfig,
         registry=registry,
       )
-      print(f'Successfully connected to kubernetes cluster: {cluster_name}')
+      print(f"Successfully connected to kubernetes cluster: {cluster_name}")
     except AlreadyConnectedException as ace:
       raise _ExitException(
-        f'Already connected to cluster: {ace.current_cluster_name}',
+        f"Already connected to cluster: {ace.current_cluster_name}",
       ) from ace
 
   def disconnect_from_connected_cluster(self):
     cluster = self.services.cluster_service.get_connected_cluster()
-    print(f'Disconnecting from cluster {cluster.name}...')
+    print(f"Disconnecting from cluster {cluster.name}...")
 
     try:
       self.services.cluster_service.disconnect(cluster.name, disconnect_all=False)
     except NotConnectedError:
-      self.services.logging_service.warning('Not connected to any clusters')
+      self.services.logging_service.warning("Not connected to any clusters")
     except MultipleClustersConnectionError as mcce:
       cluster_names = ", ".join(mcce.connected_clusters)
       self.services.logging_service.warning(
-        f'Connected to multiple clusters: {cluster_names}. '
-        'Rerun with `disconnect --all`.'
+        f"Connected to multiple clusters: {cluster_names}. Rerun with `disconnect --all`."
       )
     except ClusterError as ce:
       raise _ExitException(str(ce)) from ce
 
   def test_cluster_connection(self):
-    print('Testing if you are connected to a cluster, this may take a moment...')
+    print("Testing if you are connected to a cluster, this may take a moment...")
     try:
       cluster = self.services.cluster_service.test()
     except NotConnectedError as nce:
       raise _ExitException(
-        'You are not currently connected to a cluster.',
+        "You are not currently connected to a cluster.",
       ) from nce
 
-    registry_str = cluster.registry if cluster.registry is not None else 'default'
+    registry_str = cluster.registry if cluster.registry is not None else "default"
     print(
-      '\nYou are connected to a cluster! Here is the info:'
-      f'\n\tcluster name: {cluster.name}'
-      f'\n\tprovider: {cluster.provider_string}'
-      f'\n\tregistry: {registry_str}'
+      "\nYou are connected to a cluster! Here is the info:"
+      f"\n\tcluster name: {cluster.name}"
+      f"\n\tprovider: {cluster.provider_string}"
+      f"\n\tregistry: {registry_str}"
     )
 
     try:
       docker_service = DockerService.create(self.services)
       docker_service.check_connection()
     except DockerException as e:
       raise _ExitException(str(e)) from e
 
   def cluster_status(self):
     try:
       cluster = self.services.cluster_service.test()
     except NotConnectedError as nce:
       raise _ExitException(
-        'You are not currently connected to a cluster',
+        "You are not currently connected to a cluster",
       ) from nce
 
     print(f"You are currently connected to the cluster: {cluster.name}")
     all_pods = self.services.kubernetes_service.get_pods()
     nodes = self.services.kubernetes_service.get_nodes()
     individual_pods = []
     experiment_pods = defaultdict(list)
@@ -413,53 +415,48 @@
       if pod.status.phase == "Running":
         running_pods_by_node[pod.spec.node_name].append(pod)
     CPU = "cpu"
     MEMORY = "memory"
     GPU = "nvidia.com/gpu"
     RESOURCE_META = ((CPU, "CPU"), (MEMORY, "B"), (GPU, "GPU"))
     unit_registry = pint.UnitRegistry()
-    # NOTE(taylor): creates a new unit "CPU". "mCPU = milli CPU = 0.001 * CPU"
+    # NOTE: creates a new unit "CPU". "mCPU = milli CPU = 0.001 * CPU"
     unit_registry.define("CPU = [cpu]")
     unit_registry.define("GPU = [gpu]")
     for node in nodes.items:
       print(f"\t{node.metadata.name}:")
       node_resources = [
         (c.resources.requests, c.resources.limits)
         for p in running_pods_by_node[node.metadata.name]
         for c in p.spec.containers
       ]
-      # NOTE(taylor): create an inital value for each resource type for requests and limits
+      # NOTE: create an inital value for each resource type for requests and limits
       all_totals = tuple(
-        {
-          resource_type: 0 * unit_registry(ext)
-          for resource_type, ext in RESOURCE_META
-        }
-        for _ in range(2)
+        {resource_type: 0 * unit_registry(ext) for resource_type, ext in RESOURCE_META} for _ in range(2)
       )
       for resources in node_resources:
         for resource_allocation, totals in zip(resources, all_totals):
           if not resource_allocation:
             continue
           for resource_type, ext in RESOURCE_META:
-            # NOTE(taylor): this parses the resource quantity with a magnitude and unit.
+            # NOTE: this parses the resource quantity with a magnitude and unit.
             # ex. "12Mi" + "B" == "12*2^20 bytes", "100m" + "CPU" == "0.1 CPU"
             totals[resource_type] += unit_registry.Quantity(resource_allocation.get(resource_type, "0") + ext)
       requests_totals, limits_totals = all_totals
       for resource_type, ext in RESOURCE_META:
         allocatable = unit_registry.Quantity(node.status.allocatable.get(resource_type, "0") + ext)
         if not allocatable:
           continue
         print(f"\t\t{resource_type}:")
         total_request = requests_totals[resource_type]
         percent_request = (100 * total_request / allocatable).to_reduced_units()
         total_limit = limits_totals[resource_type]
         percent_limit = (100 * total_limit / allocatable).to_reduced_units()
         allocatable, total_request, total_limit = (
-          value.to_compact()
-          for value in (allocatable, total_request, total_limit)
+          value.to_compact() for value in (allocatable, total_request, total_limit)
         )
         print(f"\t\t\tAllocatable: {allocatable:~.2f}")
         print(f"\t\t\tRequests: {total_request:~.2f}, {percent_request:~.2f} %")
         print(f"\t\t\tLimits: {total_limit:~.2f}, {percent_limit:~.2f} %")
 
   def print_status(self, identifier):
     print(f"{identifier['raw']}:")
@@ -476,39 +473,43 @@
     print("Uploading required images to your registry...")
     print("Finished installing plugins")
 
   def exec_kubectl(self, arguments):
     self.services.cluster_service.assert_is_connected()
     check_binary(kubectl_check)
     cmd = self.services.kubectl_service.get_kubectl_command()
-    args = [cmd, '--namespace', ORCHESTRATE_NAMESPACE, *arguments]
+    args = [cmd, "--namespace", ORCHESTRATE_NAMESPACE, *arguments]
     os.execvpe(
       cmd,
       args,
       env=self.services.kubectl_service.get_kubectl_env(),
     )
 
-kubectl_check = (check_kubectl_executable, download_kubectl_executable, 'kubernetes')
+
+kubectl_check = (check_kubectl_executable, download_kubectl_executable, "kubernetes")
 aws_iam_authenticator_check = (
   check_iam_authenticator_executable,
   download_iam_authenticator_executable,
-  'aws iam-authentication',
+  "aws iam-authentication",
 )
 
+
 def check_authenticator_binary(provider):
   if provider == PROVIDER_TO_STRING[Provider.AWS]:
     check_binary(aws_iam_authenticator_check)
 
+
 def check_binary(options):
   ensure_dir(get_bin_dir())
   check, download, name = options
   try:
     check()
   except CheckExecutableError:
     print(f"Downloading {name} executable, this could take some time...")
     download()
     check(full_check=True)
 
+
 def load_user_options(filename):
   with open(filename) as f:
     options = yaml.safe_load(f) or {}
   return options
```

### Comparing `sigopt-8.8.0/sigopt/orchestrate/custom_cluster/service.py` & `sigopt-8.8.1/sigopt/orchestrate/custom_cluster/service.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,37 +8,40 @@
 from ..version import CLI_NAME
 
 
 class CustomClusterService(ProviderInterface):
   def create_kubernetes_cluster(self, options):
     cluster_name = options.get("cluster_name", "my-cluster")
     raise OrchestrateException(
-      f'When you use provider = "{provider_to_string(Provider.CUSTOM)}",'
-      ' we assume that you have created your own kubernetes cluster.'
-      ' If you are attempting to connect to a custom cluster that you have already created, please use:'
-      f'\n{CLI_NAME} cluster connect --provider custom --kubeconfig <kubeconfig> --cluster-name {cluster_name}'
+      f'When you use provider = "{provider_to_string(Provider.CUSTOM)}", we'
+      " assume that you have created your own kubernetes cluster. If you are"
+      " attempting to connect to a custom cluster that you have already created,"
+      f" please use:\n{CLI_NAME} cluster connect --provider custom --kubeconfig"
+      f" <kubeconfig> --cluster-name {cluster_name}"
     )
 
   def destroy_kubernetes_cluster(self, cluster_name):
     raise OrchestrateException(
-      f'When you use provider = "{provider_to_string(Provider.CUSTOM)}",'
-      ' we assume that you have created your own kubernetes cluster.'
-      ' If you are attempting to disconnect from a custom cluster that you have already created, please use:'
-      f'\n{CLI_NAME} cluster disconnect --cluster-name {cluster_name}'
+      f'When you use provider = "{provider_to_string(Provider.CUSTOM)}", we'
+      " assume that you have created your own kubernetes cluster. If you are"
+      " attempting to disconnect from a custom cluster that you have already"
+      f" created, please use:\n{CLI_NAME} cluster disconnect --cluster-name"
+      f" {cluster_name}"
     )
 
   def create_kubeconfig(self, cluster_name, ignore_role=False):
     raise OrchestrateException(
-      f'When you use provider = "{provider_to_string(Provider.CUSTOM)}",'
-      ' we assume that you have created your own kubernetes cluster.'
-      ' Additionally we assume that you have a copy of the kubeconfig file that is used to access the cluster.'
-      ' Please provide the path to the kubeconfig as an argument.'
-      ' You will also need to provide the URL for your container registry, if using a private one.'
-      f'\n{CLI_NAME} cluster connect --provider custom --kubeconfig <kubeconfig>'
-      f' --cluster-name {cluster_name} [--registry <registry-url>]'
+      f'When you use provider = "{provider_to_string(Provider.CUSTOM)}", we'
+      " assume that you have created your own kubernetes cluster. Additionally"
+      " we assume that you have a copy of the kubeconfig file that is used to"
+      " access the cluster. Please provide the path to the kubeconfig as an"
+      " argument. You will also need to provide the URL for your container"
+      f" registry, if using a private one.\n{CLI_NAME} cluster connect --provider"
+      " custom --kubeconfig <kubeconfig> --cluster-name"
+      f" {cluster_name} [--registry <registry-url>]"
     )
 
   def test_kubernetes_cluster(self, cluster_name, ignore_role=False):
     self.services.kubernetes_service.test_config()
 
   def create_cluster_object(self, services, name, registry):
     return CustomCluster(
```

### Comparing `sigopt-8.8.0/sigopt/orchestrate/docker/service.py` & `sigopt-8.8.1/sigopt/orchestrate/docker/service.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,48 +16,60 @@
 from ..json_stream import json_stream
 from ..services.base import Service
 
 
 DOCKER_TARGET_VERSION = "1.41"
 
 
-DockerLoginCredentials = namedtuple('DockerLoginCredentials', [
-  'username',
-  'password',
-  'registry',
-])
+DockerLoginCredentials = namedtuple(
+  "DockerLoginCredentials",
+  [
+    "username",
+    "password",
+    "registry",
+  ],
+)
+
 
 class DockerException(OrchestrateException):
   pass
 
+
 class DockerInstallationError(DockerException):
   pass
 
+
 class DockerPodTimeoutError(DockerException):
   pass
 
+
 class DockerConnectionError(DockerException):
   pass
 
+
 class DockerService(Service):
   @classmethod
   def create(cls, services):
     if not services.kubernetes_service.is_docker_installed():
-      raise DockerInstallationError("\n".join([
-        "Docker not found in your cluster.",
-        "SigOpt no longer uses your local Docker installation to build images.",
-        "Please install the SigOpt plugins to get Docker running on your cluster:",
-        "\tsigopt cluster install-plugins",
-      ]))
+      raise DockerInstallationError(
+        "\n".join(
+          [
+            "Docker not found in your cluster.",
+            "SigOpt no longer uses your local Docker installation to build images.",
+            "Please install the SigOpt plugins to get Docker running on your cluster:",
+            "\tsigopt cluster install-plugins",
+          ]
+        )
+      )
     try:
       services.kubernetes_service.wait_for_docker_pod()
     except TimeoutError as e:
       raise DockerPodTimeoutError(str(e)) from e
     client = docker.DockerClient(
-      # HACK(taylor): DockerClient can't accept the kubernetes proxy url if it doesn't have a port specified, so give it
+      # HACK: DockerClient can't accept the kubernetes proxy url if it doesn't have a port specified, so give it
       # a fake url to initialize
       base_url="tcp://a:1",
       version=DOCKER_TARGET_VERSION,
     )
     services.kubernetes_service.mount_http_proxy_adapter(client.api)
     client.api.base_url = services.kubernetes_service.get_docker_connection_url()
     return cls(services, client)
@@ -66,53 +78,50 @@
     super().__init__(services)
     self.client = client
 
   def check_connection(self):
     try:
       self.client.images.list()
     except (docker.errors.DockerException, requests.exceptions.ConnectionError) as e:
-      raise DockerConnectionError(
-        f'An error occurred while checking your docker connection: {e}'
-      ) from e
+      raise DockerConnectionError(f"An error occurred while checking your docker connection: {e}") from e
 
   def print_logs(self, logs):
     for log in logs:
       sys.stdout.write(log)
       sys.stdout.flush()
 
   def stream_build_log(self, logs, dockerfile, show_all_logs):
     downloading = False
     for parsed_log in json_stream(logs):
-      if 'error' in parsed_log:
+      if "error" in parsed_log:
         if show_all_logs:
-          print(parsed_log['error'], file=sys.stderr)
-        raise ModelPackingError(parsed_log['error'], dockerfile)
-      if 'status' in parsed_log:
-        if not downloading and parsed_log['status'] == 'Downloading':
-          yield 'Downloading the base image...\n'
+          print(parsed_log["error"], file=sys.stderr)
+        raise ModelPackingError(parsed_log["error"], dockerfile)
+      if "status" in parsed_log:
+        if not downloading and parsed_log["status"] == "Downloading":
+          yield "Downloading the base image...\n"
           downloading = True
-      elif 'stream' in parsed_log:
+      elif "stream" in parsed_log:
         if show_all_logs:
-          yield parsed_log['stream']
+          yield parsed_log["stream"]
         downloading = False
 
   def build(
     self,
     tag=None,
     dockerfile_name=None,
     dockerfile_contents=None,
     directory=None,
     quiet=True,
     build_args=None,
     show_all_logs=False,
   ):
     if dockerfile_contents:
-      assert not dockerfile_name, \
-        "only one of dockerfile_name, dockerfile_contents can be provided"
-      with NamedTemporaryFile(mode='w', delete=False) as dockerfile_fp:
+      assert not dockerfile_name, "only one of dockerfile_name, dockerfile_contents can be provided"
+      with NamedTemporaryFile(mode="w", delete=False) as dockerfile_fp:
         dockerfile_fp.write(dockerfile_contents)
         dockerfile = dockerfile_fp.name
     else:
       dockerfile = dockerfile_name
     try:
       tag = tag or (
         "sigopt-temp:" + "".join(random.choice(string.ascii_lowercase + string.digits) for _ in range(8))  # nosec
@@ -140,48 +149,48 @@
     except docker.errors.BuildError as e:
       raise ModelPackingError(str(e), dockerfile) from e
 
   def push(self, repository, tag=None, retries=1, quiet=True):
     for try_number in range(retries + 1):
       try:
         for obj in json_stream(self.client.images.push(repository=repository, tag=tag, stream=True)):
-          if 'error' in obj:
-            raise Exception(obj['error'])
+          if "error" in obj:
+            raise Exception(obj["error"])
       except urllib3.exceptions.ReadTimeoutError:
         if try_number >= retries:
           raise
         if not quiet:
           print("Docker push failed, retrying...")
 
-  def pull(self, repository, tag='latest'):
+  def pull(self, repository, tag="latest"):
     self.client.images.pull(repository=repository, tag=tag)
 
   def login(self, docker_login_credentials):
     creds = docker_login_credentials
     response = self.client.login(
       username=creds.username,
       password=creds.password,
       registry=creds.registry,
       dockercfg_path="/dev/null",
     )
     response_status = response.get("Status")
     if response_status:
-      assert response_status == 'Login Succeeded', (
-        f'Docker failed logging into registry {creds.registry} with username {creds.username}',
+      assert response_status == "Login Succeeded", (
+        f"Docker failed logging into registry {creds.registry} with username {creds.username}",
       )
 
   @staticmethod
   def format_image_name(repository, tag):
-    return f'{repository}:{tag}' if tag is not None else repository
+    return f"{repository}:{tag}" if tag is not None else repository
 
   @staticmethod
   def get_repository_and_tag(image):
-    image_regex = r'^([a-z0-9\_\-]+(?::[0-9]+)?\/?[a-z0-9\_\-]+)(:[a-zA-Z0-9\_\-\.]+)?$'
+    image_regex = r"^([a-z0-9\_\-]+(?::[0-9]+)?\/?[a-z0-9\_\-]+)(:[a-zA-Z0-9\_\-\.]+)?$"
     match = re.match(image_regex, image)
-    assert match, 'image must match the regex: /' + image_regex + '/'
+    assert match, "image must match the regex: /" + image_regex + "/"
     groups = match.groups()
     repository = groups[0]
     tag = groups[1][1:] if groups[1] else None
     return repository, tag
 
   def get_image(self, tag):
     return self.client.images.get(tag)
@@ -190,15 +199,15 @@
     self.client.images.remove(tag)
 
   def untag(self, image):
     for tag in image.tags:
       self.client.images.remove(tag)
 
   def untag_all(self, label):
-    for image in self.client.images.list(filters={'label': label}):
+    for image in self.client.images.list(filters={"label": label}):
       self.untag(image)
 
   def image_exists_in_registry(self, repo, tag):
     try:
       for _ in self.client.api.pull(repo + ":" + tag, stream=True):
         return True
     except docker.errors.NotFound:
```

### Comparing `sigopt-8.8.0/sigopt/orchestrate/ec2/service.py` & `sigopt-8.8.1/sigopt/orchestrate/ec2/service.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,61 +2,62 @@
 #
 # SPDX-License-Identifier: MIT
 import errno
 import os
 
 import boto3
 from botocore.exceptions import ClientError
+
 from sigopt.paths import ensure_dir, get_root_subdir
 
 from ..services.aws_base import AwsService
 
 
 class AwsEc2Service(AwsService):
   def __init__(self, services, aws_services, **kwargs):
     super().__init__(services, aws_services)
-    self._ec2 = boto3.resource('ec2', **kwargs)
+    self._ec2 = boto3.resource("ec2", **kwargs)
 
   @property
   def ec2(self):
     return self._ec2
 
   def get_subnets(self, subnet_ids):
     subnets = self.ec2.subnets.all()
     return list(subnet for subnet in subnets if subnet.id in subnet_ids)
 
   def key_pair_for_cluster_name(self, cluster_name):
-    return f'key-pair-for-cluster-{cluster_name}'
+    return f"key-pair-for-cluster-{cluster_name}"
 
   def describe_key_pair_for_cluster(self, cluster_name):
     return self.ec2.KeyPair(self.key_pair_for_cluster_name(cluster_name))
 
   def create_key_pair_for_cluster(self, cluster_name):
     key_pair = self.ec2.create_key_pair(KeyName=self.key_pair_for_cluster_name(cluster_name))
 
     self.ensure_key_pair_directory()
 
     try:
       with os.fdopen(
         os.open(self.key_pair_location(cluster_name), os.O_CREAT | os.O_WRONLY, 0o600),
-        'w',
+        "w",
       ) as f:
         f.write(key_pair.key_material)
     except Exception:
       # We only get one chance to read the key, so if we mess up then delete the key so we can try again next time
       key_pair.delete()
       raise
 
     return key_pair
 
   def ensure_key_pair_for_cluster(self, cluster_name):
     try:
       self.create_key_pair_for_cluster(cluster_name)
     except ClientError as e:
-      if not e.response['Error']['Code'] == 'InvalidKeyPair.Duplicate':
+      if not e.response["Error"]["Code"] == "InvalidKeyPair.Duplicate":
         raise e
 
     return self.describe_key_pair_for_cluster(cluster_name)
 
   def delete_key_pair_for_cluster(self, cluster_name):
     try:
       os.remove(self.key_pair_location(cluster_name))
@@ -64,21 +65,21 @@
       if e.errno != errno.ENOENT:
         raise
 
     self.describe_key_pair_for_cluster(cluster_name).delete()
 
   @property
   def key_pair_directory(self):
-    return get_root_subdir('ssh')
+    return get_root_subdir("ssh")
 
   def ensure_key_pair_directory(self):
     ensure_dir(self.key_pair_directory)
 
   def key_pair_location(self, cluster_name):
     key_name = self.key_pair_for_cluster_name(cluster_name)
-    filename = f'{key_name}.pem'
+    filename = f"{key_name}.pem"
     return os.path.join(self.key_pair_directory, filename)
 
   def ensure_key_pair_for_cluster_deleted(self, cluster_name):
-    # Note(alexandra): under our current structure, no error occurs if we attempt to
+    # Note: under our current structure, no error occurs if we attempt to
     # delete a non-existent keypair
     self.delete_key_pair_for_cluster(cluster_name)
```

### Comparing `sigopt-8.8.0/sigopt/orchestrate/ecr/service.py` & `sigopt-8.8.1/sigopt/orchestrate/ecr/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from ..services.aws_base import AwsService
 
 
 class AwsEcrService(AwsService):
   def __init__(self, services, aws_services, **kwargs):
     super().__init__(services, aws_services)
-    self._client = boto3.client('ecr', **kwargs)
+    self._client = boto3.client("ecr", **kwargs)
 
   @property
   def client(self):
     return self._client
 
   def _create_repository(self, repository_name):
     return self.client.create_repository(repositoryName=repository_name)
```

### Comparing `sigopt-8.8.0/sigopt/orchestrate/eks/service.py` & `sigopt-8.8.1/sigopt/orchestrate/eks/service.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 DEFAULT_KUBERNETES_VERSION = "1.23"
 SUPPORTED_KUBERNETES_VERSIONS = ("1.20", "1.21", "1.22", "1.23")
 
 
 class AwsEksService(AwsService):
   def __init__(self, services, aws_services, **kwargs):
     super().__init__(services, aws_services)
-    self._client = boto3.client('eks', **kwargs)
+    self._client = boto3.client("eks", **kwargs)
 
   @property
   def client(self):
     return self._client
 
   def describe_cluster(self, cluster_name):
     return self.client.describe_cluster(name=cluster_name)
```

### Comparing `sigopt-8.8.0/sigopt/orchestrate/exceptions.py` & `sigopt-8.8.1/sigopt/orchestrate/exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,53 +8,64 @@
 
 class OrchestrateException(click.ClickException):
   def __init__(self, msg=None):
     if msg is None:
       msg = f"Uncaught exception: {type(self).__name__}"
     super().__init__(msg)
 
+
 class CheckExecutableError(OrchestrateException):
   pass
 
+
 class CheckConnectionError(OrchestrateException):
   pass
 
+
 class AwsClusterSharePermissionError(OrchestrateException):
   pass
 
+
 class AwsPermissionsError(OrchestrateException):
   def __init__(self, error):
     super().__init__(
       "Looks like you have encountered the below AWS permissions error."
-      " Please check out our documentation and ensure you have granted yourself the correct AWS permissions"
+      " Please check out our documentation and ensure you have granted yourself"
+      " the correct AWS permissions"
       " to use SigOpt cluster features:"
       " https://docs.sigopt.com/ai-module-api-references/orchestrate/aws_cluster#aws-configuration"
       f"\n\n{error}"
     )
 
+
 class MissingGpuNodesException(OrchestrateException):
   pass
 
+
 class ModelPackingError(OrchestrateException):
   def __init__(self, error_str, dockerfile):
     super().__init__(
-      f'{error_str}\n'
-      f'Dockerfile: {dockerfile}\n'
-      f'If you suspect that you are out of space, run `{CLI_NAME} clean` and try again.',
+      (
+        f"{error_str}\nDockerfile: {dockerfile}\nIf you suspect that you are"
+        f" out of space, run `{CLI_NAME} clean` and try again."
+      ),
     )
 
+
 class ClusterDestroyError(OrchestrateException):
   def __init__(self):
-    print('The following exceptions occurred during cluster destroy:\n')
+    print("The following exceptions occurred during cluster destroy:\n")
     super().__init__()
 
+
 class NodesNotReadyError(OrchestrateException):
   pass
 
+
 class FileAlreadyExistsError(OrchestrateException):
   def __init__(self, filename):
     self.filename = filename
 
     super().__init__(
-      f'We are attempting to write a file, but it already exists on your system: {filename}.'
-      ' Please delete the file and try your request again.'
+      "We are attempting to write a file, but it already exists on your system:"
+      f" {filename}. Please delete the file and try your request again."
     )
```

### Comparing `sigopt-8.8.0/sigopt/orchestrate/iam/service.py` & `sigopt-8.8.1/sigopt/orchestrate/iam/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,30 +11,30 @@
 
 from ..services.aws_base import AwsService
 
 
 class AwsIamService(AwsService):
   def __init__(self, services, aws_services, **kwargs):
     super().__init__(services, aws_services)
-    self._client = boto3.client('iam', **kwargs)
-    self._iam = boto3.resource('iam', **kwargs)
-    self._sts = boto3.client('sts', **kwargs)
+    self._client = boto3.client("iam", **kwargs)
+    self._iam = boto3.resource("iam", **kwargs)
+    self._sts = boto3.client("sts", **kwargs)
 
   @property
   def client(self):
     return self._client
 
   @property
   def iam(self):
     return self._iam
 
   def get_user_arn(self):
     response = self.client.get_user()
-    user = response['User']
-    return user['Arn']
+    user = response["User"]
+    return user["Arn"]
 
   def describe_eks_role(self, role_name):
     return self.iam.Role(role_name)
 
   def get_thumbprint_from_oidc_issuer(self, oidc_url):
     response = requests.get(f"{oidc_url}/.well-known/openid-configuration")
     response.raise_for_status()
@@ -77,15 +77,15 @@
     arn = self.get_oidc_arn(url)
     try:
       self.client.delete_open_id_connect_provider(OpenIDConnectProviderArn=arn)
     except self.client.exceptions.NoSuchEntityException:
       pass
 
   def _role_name_from_role_arn(self, role_arn):
-    return role_arn.split(':role/')[1]
+    return role_arn.split(":role/")[1]
 
   def attach_policy(self, role_arn, policy_arn):
     role_name = self._role_name_from_role_arn(role_arn)
     self.iam.Role(role_name).attach_policy(PolicyArn=policy_arn)
 
   def get_cluster_access_role_arn(self, cluster_name):
     role_name = f"{cluster_name}-k8s-access-role"
```

### Comparing `sigopt-8.8.0/sigopt/orchestrate/identifier.py` & `sigopt-8.8.1/sigopt/orchestrate/identifier.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
   IDENTIFIER_TYPE_RUN,
   IDENTIFIER_TYPE_SUGGESTION,
 }
 IDENTIFIER_QUERY_ID = "id"
 IDENTIFIER_QUERY_NAME = "name"
 IDENTIFIER_QUERY_SUGGESTION = "suggestion"
 
+
 def parse_identifier(id_str):
   if "/" not in id_str:
     return {
       "raw": id_str,
       "type": IDENTIFIER_TYPE_RUN,
       "query": IDENTIFIER_QUERY_NAME,
       "value": id_str,
@@ -33,40 +34,44 @@
     "type": _type,
     "query": IDENTIFIER_QUERY_ID,
     "value": _id,
     "pod_label_selector": f"type=run,{_type}={_id}",
     "controller_label_selector": f"type=controller,{_type}={_id}",
   }
 
+
 def maybe_convert_to_run_identifier(identifier):
   if identifier["type"] == IDENTIFIER_TYPE_SUGGESTION:
     return {
       "raw": identifier["raw"],
       "type": IDENTIFIER_TYPE_RUN,
       "query": IDENTIFIER_QUERY_SUGGESTION,
       "value": identifier["value"],
       "pod_label_selector": identifier["pod_label_selector"],
       "controller_label_selector": identifier["controller_label_selector"],
     }
   return identifier
 
+
 def get_run_and_pod_from_identifier(identifier, services):
   identifier = maybe_convert_to_run_identifier(identifier)
   assert identifier["type"] == IDENTIFIER_TYPE_RUN, f"Can't get a single run or pod from {identifier['raw']}"
   run = None
   run_id = None
   pod = None
 
   # find the run from the identifier
   if identifier["query"] in (IDENTIFIER_QUERY_NAME, IDENTIFIER_QUERY_SUGGESTION):
     filter_field = identifier["query"]
     filter_value = identifier["value"]
-    runs = list(services.sigopt_service.iterate_runs_by_filters(
-      [{"operator": "==", "field": filter_field, "value": filter_value}],
-    ))
+    runs = list(
+      services.sigopt_service.iterate_runs_by_filters(
+        [{"operator": "==", "field": filter_field, "value": filter_value}],
+      )
+    )
     if len(runs) > 1:
       raise Exception(f"Multiple runs found with {filter_field}: {filter_value}")
     if len(runs) == 1:
       run = runs[0]
   elif identifier["query"] == IDENTIFIER_QUERY_ID:
     run_id = identifier["value"]
     run = services.sigopt_service.conn.training_runs(run_id).fetch()
```

### Comparing `sigopt-8.8.0/sigopt/orchestrate/job_runner/service.py` & `sigopt-8.8.1/sigopt/orchestrate/job_runner/service.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,60 +9,61 @@
 from ..docker.service import DockerService
 from ..exceptions import OrchestrateException
 from ..services.base import Service
 from ..version import DEFAULT_CONTROLLER_IMAGE
 
 
 def format_k8s_env_vars(env_vars):
-  return [
-    dict(name=key, value=value)
-    for key, value in env_vars.items()
-  ]
+  return [dict(name=key, value=value) for key, value in env_vars.items()]
+
 
 class JobRunnerService(Service):
   DEFAULT_EPHEMERAL_STORAGE_REQUEST = "128Mi"
   EXPERIMENT_ENV_KEY = "ORCHESTRATE_EXPERIMENT_ID"
 
   @property
   def controller_image(self):
     return os.environ.get("SIGOPT_CONTROLLER_IMAGE", DEFAULT_CONTROLLER_IMAGE)
 
   def sigopt_env_vars(self, project_id):
     client, project = self.services.sigopt_service.ensure_project_exists(project_id)
-    return format_k8s_env_vars({
-      'SIGOPT_API_TOKEN': self.services.sigopt_service.api_token,
-      'SIGOPT_API_URL': self.services.sigopt_service.api_url,
-      'SIGOPT_PROJECT': project,
-      'SIGOPT_CLIENT': client,
-    })
+    return format_k8s_env_vars(
+      {
+        "SIGOPT_API_TOKEN": self.services.sigopt_service.api_token,
+        "SIGOPT_API_URL": self.services.sigopt_service.api_url,
+        "SIGOPT_PROJECT": project,
+        "SIGOPT_CLIENT": client,
+      }
+    )
 
   def format_resources(self, resource_options):
     resource_options = resource_options or {}
     requests = resource_options.setdefault("requests", {})
     requests.setdefault("ephemeral-storage", self.DEFAULT_EPHEMERAL_STORAGE_REQUEST)
     limits = resource_options.setdefault("limits", {})
 
-    if resource_options.get('gpus'):
-      if 'nvidia.com/gpu' in limits:
+    if resource_options.get("gpus"):
+      if "nvidia.com/gpu" in limits:
         raise OrchestrateException(
-          'The value in resources.gpus will override the value in resources.limits.nvidia.com/gpu,'
-          'please remove one of these fields.'
+          "The value in resources.gpus will override the value in"
+          " resources.limits.nvidia.com/gpu,please remove one of these"
+          " fields."
         )
-      limits['nvidia.com/gpu'] = resource_options.pop('gpus')
+      limits["nvidia.com/gpu"] = resource_options.pop("gpus")
 
   def random_id_string(self):
     return "".join(random.choice(string.ascii_lowercase) for _ in range(8))  # nosec
 
   def create_sigopt_experiment(self, optimization_options, project_id):
     data = optimization_options.copy()
 
-    metadata = data.pop('metadata', None) or {}
+    metadata = data.pop("metadata", None) or {}
 
     cluster = self.services.cluster_service.get_connected_cluster()
-    metadata['cluster_name'] = cluster.name
+    metadata["cluster_name"] = cluster.name
 
     data["metadata"] = metadata
 
     experiment = self.services.sigopt_service.create_aiexperiment(data, project_id)
     return experiment.id
 
   def create_controller(
@@ -80,128 +81,134 @@
     image_name = DockerService.format_image_name(repository, tag)
     cluster = self.services.cluster_service.get_connected_cluster()
     self.format_resources(resource_options)
     job_info_path = "/etc/job-info"
     job_info_volume_name = "job-info"
     env_vars = [
       {
-        'name': 'KUBE_CONFIG',
-        'value': "incluster",
+        "name": "KUBE_CONFIG",
+        "value": "incluster",
       },
       {
-        'name': 'USER_IMAGE',
-        'value': image_name,
+        "name": "USER_IMAGE",
+        "value": image_name,
       },
       {
-        'name': 'USER_RESOURCES',
-        'value': json.dumps(resource_options),
+        "name": "USER_RESOURCES",
+        "value": json.dumps(resource_options),
       },
       {
-        'name': 'NAMESPACE',
-        'valueFrom': {
-          'fieldRef': {
-            'fieldPath': 'metadata.namespace',
+        "name": "NAMESPACE",
+        "valueFrom": {
+          "fieldRef": {
+            "fieldPath": "metadata.namespace",
           },
         },
       },
       {
-        'name': "CLUSTER_NAME",
-        'value': cluster.name,
+        "name": "CLUSTER_NAME",
+        "value": cluster.name,
       },
       {
-        'name': 'JOB_INFO_PATH',
-        'value': job_info_path,
+        "name": "JOB_INFO_PATH",
+        "value": job_info_path,
       },
       {
         "name": "CONTROLLER_MODE",
         "value": controller_mode,
       },
       *(self.sigopt_env_vars(project_id)),
       *extra_env_vars,
     ]
     if self.services.sigopt_service.log_collection_enabled:
-      env_vars.append({
-        "name": "SIGOPT_LOG_COLLECTION_ENABLED",
-        "value": "1",
-      })
+      env_vars.append(
+        {
+          "name": "SIGOPT_LOG_COLLECTION_ENABLED",
+          "value": "1",
+        }
+      )
 
     labels = {
       "mode": controller_mode,
       "type": "controller",
       **extra_labels,
     }
 
     if not run_command:
       run_command = []
 
-    self.services.kubernetes_service.start_job({
-      'apiVersion': 'batch/v1',
-      'kind': 'Job',
-      'metadata': {
-        'name': controller_name,
-        'labels': labels,
-      },
-      'spec': {
-        'template': {
-          'metadata': {
-            'labels': labels,
-          },
-          'spec': {
-            'serviceAccount': 'controller',
-            'securityContext': {
-              'allowPrivilegeEscalation': False,
-              'readOnlyRootFilesystem': True,
+    self.services.kubernetes_service.start_job(
+      {
+        "apiVersion": "batch/v1",
+        "kind": "Job",
+        "metadata": {
+          "name": controller_name,
+          "labels": labels,
+        },
+        "spec": {
+          "template": {
+            "metadata": {
+              "labels": labels,
             },
-            'restartPolicy': 'Never',
-            'containers': [
-              {
-                'image': self.controller_image,
-                'imagePullPolicy': 'Always',
-                'name': 'controller',
-                'env': env_vars,
-                'args': run_command,
-                'resources': {
-                  'limits': {
-                    'cpu': '100m',
-                    'memory': '128Mi',
+            "spec": {
+              "serviceAccount": "controller",
+              "securityContext": {
+                "allowPrivilegeEscalation": False,
+                "readOnlyRootFilesystem": True,
+              },
+              "restartPolicy": "Never",
+              "containers": [
+                {
+                  "image": self.controller_image,
+                  "imagePullPolicy": "Always",
+                  "name": "controller",
+                  "env": env_vars,
+                  "args": run_command,
+                  "resources": {
+                    "limits": {
+                      "cpu": "100m",
+                      "memory": "128Mi",
+                    },
                   },
-                },
-                'volumeMounts': [
-                  {
-                    'name': job_info_volume_name,
-                    'mountPath': job_info_path,
+                  "volumeMounts": [
+                    {
+                      "name": job_info_volume_name,
+                      "mountPath": job_info_path,
+                    },
+                  ],
+                  "securityContext": {
+                    "allowPrivilegeEscalation": False,
+                    "readOnlyRootFilesystem": True,
                   },
-                ],
-                'securityContext': {
-                  'allowPrivilegeEscalation': False,
-                  'readOnlyRootFilesystem': True,
                 },
-              },
-            ],
-            'volumes': [{
-              # NOTE(taylor): the job-info downwardAPI volume allows the controller to link newly created pods
-              # to the controller job so that the garbage collector will clean up dangling pods
-              'name': job_info_volume_name,
-              'downwardAPI': {
-                'items': [
-                  {
-                    'path': 'name',
-                    'fieldRef': {'fieldPath': "metadata.labels['job-name']"},
-                  },
-                  {
-                    'path': 'uid',
-                    'fieldRef': {'fieldPath': "metadata.labels['controller-uid']"},
+              ],
+              "volumes": [
+                {
+                  # NOTE: the job-info downwardAPI volume allows the controller to link newly created pods
+                  # to the controller job so that the garbage collector will clean up dangling pods
+                  "name": job_info_volume_name,
+                  "downwardAPI": {
+                    "items": [
+                      {
+                        "path": "name",
+                        "fieldRef": {"fieldPath": "metadata.labels['job-name']"},
+                      },
+                      {
+                        "path": "uid",
+                        "fieldRef": {"fieldPath": "metadata.labels['controller-uid']"},
+                      },
+                    ],
                   },
-                ],
-              },
-            }],
+                }
+              ],
+            },
           },
         },
-      },
-    })
+      }
+    )
 
   def start_cluster_run(
     self,
     repository,
     tag,
     resource_options,
     project_id,
@@ -257,18 +264,20 @@
     self.services.kubernetes_service.check_nodes_are_ready()
 
     experiment_id = experiment_id or self.create_sigopt_experiment(optimization_options, project_id)
 
     controller_name = f"experiment-controller-{experiment_id}"
     labels = {"experiment": str(experiment_id)}
     controller_mode = "experiment"
-    env_vars = [{
-      "name": self.EXPERIMENT_ENV_KEY,
-      "value": str(experiment_id),
-    }]
+    env_vars = [
+      {
+        "name": self.EXPERIMENT_ENV_KEY,
+        "value": str(experiment_id),
+      }
+    ]
 
     self.create_controller(
       repository,
       tag,
       resource_options,
       run_command,
       controller_mode,
```

### Comparing `sigopt-8.8.0/sigopt/orchestrate/job_status/service.py` & `sigopt-8.8.1/sigopt/orchestrate/job_status/service.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,66 +7,62 @@
 class JobStatusService(Service):
   def parse_job(self, job):
     job_name = job.metadata.name
 
     conditions = []
     if job.status.conditions:
       for c in job.status.conditions:
-        if c.status == 'True':
+        if c.status == "True":
           conditions.append(c.type)
-        elif c.status == 'False':
+        elif c.status == "False":
           conditions.append(f"Not {c.type}")
         else:
           conditions.append(f"Maybe {c.type}")
 
-    job_status = ', '.join(conditions) if conditions else 'Not Complete'
+    job_status = ", ".join(conditions) if conditions else "Not Complete"
 
     experiment_id = self.services.job_runner_service.experiment_id(job_name)
     experiment = self.services.sigopt_service.safe_fetch_experiment(experiment_id)
 
     return dict(
       experiment=experiment,
       name=job_name,
       status=job_status,
-      experiment_id=experiment_id or '??',
-      experiment_name=(experiment.name if experiment else 'unknown'),
-      budget=(
-        str(float(experiment.budget))
-        if experiment and experiment.budget is not None
-        else 'n/a'
-      ),
-      total_run_count=str(experiment.progress.total_run_count) if experiment else 'n/a',
+      experiment_id=experiment_id or "??",
+      experiment_name=(experiment.name if experiment else "unknown"),
+      budget=(str(float(experiment.budget)) if experiment and experiment.budget is not None else "n/a"),
+      total_run_count=str(experiment.progress.total_run_count) if experiment else "n/a",
     )
 
   def get_runs_by_pod(self, experiment):
     runs_by_pod = dict()
     for run in self.services.sigopt_service.iterate_runs(experiment):
-      pod_name = run.metadata.get('pod_name') if run.metadata else 'UNKNOWN'
+      pod_name = run.metadata.get("pod_name") if run.metadata else "UNKNOWN"
 
       if pod_name not in runs_by_pod:
         runs_by_pod[pod_name] = dict(success=0, failed=0)
 
-      # TODO(patrick): Include active state in output as well
-      if run.state == 'failed':
-        runs_by_pod[pod_name]['failed'] += 1
-      elif run.state != 'active':
-        runs_by_pod[pod_name]['success'] += 1
+      # TODO: Include active state in output as well
+      if run.state == "failed":
+        runs_by_pod[pod_name]["failed"] += 1
+      elif run.state != "active":
+        runs_by_pod[pod_name]["success"] += 1
 
     return runs_by_pod
 
   def parse_pod(self, pod, runs_by_pod):
     pod_name = pod.metadata.name
     runs = runs_by_pod.get(pod_name, dict(success=0, failed=0))
 
     phase = pod.status.phase
     status = phase
-    if phase in ['Pending', 'Failed', 'Unknown']:
+    if phase in ["Pending", "Failed", "Unknown"]:
       reasons = [condition.reason for condition in pod.status.conditions if condition.reason]
       if reasons:
         status = f'{status} - {", ".join(reasons)}'
 
     return dict(
       name=pod_name,
-      success=runs['success'],
-      failed=runs['failed'],
+      success=runs["success"],
+      failed=runs["failed"],
       status=status,
     )
```

### Comparing `sigopt-8.8.0/sigopt/orchestrate/json_stream.py` & `sigopt-8.8.1/sigopt/orchestrate/json_stream.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,26 +11,23 @@
   def consume(self, chunk):
     if isinstance(chunk, bytes):
       chunk = chunk.decode("utf-8")
     self.buffer.append(chunk)
     return self.emit_data()
 
   def emit_data(self):
-    parts = ''.join(self.buffer).splitlines(True)
+    parts = "".join(self.buffer).splitlines(True)
     if not parts:
       return []
     if parts[-1] and parts[-1][-1] != "\n":
-      # NOTE(taylor): the last line is not a whole line and should be buffered
+      # NOTE: the last line is not a whole line and should be buffered
       self.buffer = [parts[-1]]
       parts = parts[:-1]
     else:
       self.buffer = []
-    return [
-      json.loads(part)
-      for part in parts
-      if part.strip()
-    ]
+    return [json.loads(part) for part in parts if part.strip()]
+
 
 def json_stream(stream):
   json_buffer = JsonBuffer()
   for chunk in stream:
     yield from json_buffer.consume(chunk)
```

### Comparing `sigopt-8.8.0/sigopt/orchestrate/kubectl/service.py` & `sigopt-8.8.1/sigopt/orchestrate/kubectl/service.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,24 +7,26 @@
 
 from ..paths import get_executable_path
 from ..services.base import Service
 
 
 class KubectlService(Service):
   def get_kubectl_command(self):
-    return get_executable_path('kubectl')
+    return get_executable_path("kubectl")
 
   def get_kubectl_env(self):
     kube_config = self.get_kube_config()
     assert kube_config, "The kubectl service has no kubernetes config"
     orchestrate_bin = get_bin_dir()
     env = os.environ.copy()
-    previous_path = env.get('PATH', '')
-    env.update(dict(
-      KUBECONFIG=kube_config,
-      PATH=f'{orchestrate_bin}:{previous_path}'.encode(),
-    ))
+    previous_path = env.get("PATH", "")
+    env.update(
+      dict(
+        KUBECONFIG=kube_config,
+        PATH=f"{orchestrate_bin}:{previous_path}".encode(),
+      )
+    )
     return env
 
   @property
   def get_kube_config(self):
     return self.services.kubernetes_service.kube_config
```

### Comparing `sigopt-8.8.0/sigopt/orchestrate/kubernetes/http_proxy.py` & `sigopt-8.8.1/sigopt/orchestrate/kubernetes/http_proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,10 +18,10 @@
     assert not query, "query string based auth not yet supported"
 
   def init_poolmanager(self, connections, maxsize, block=None, **_):
     rest_client = RESTClientObject(self.k8s_api_client.configuration, pools_size=connections, maxsize=maxsize)
     self.poolmanager = rest_client.pool_manager
 
   def cert_verify(self, conn, url, verify, cert):
-    # NOTE(taylor): Session.request tries to reset the certificate (why???) so just make sure certs are required and
+    # NOTE: Session.request tries to reset the certificate (why???) so just make sure certs are required and
     # carry on
     assert conn.cert_reqs == ssl.CERT_REQUIRED
```

### Comparing `sigopt-8.8.0/sigopt/orchestrate/kubernetes/service.py` & `sigopt-8.8.1/sigopt/orchestrate/kubernetes/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,107 +14,120 @@
 
 import backoff
 import requests
 import yaml
 from kubernetes import client, config, utils, watch
 from kubernetes.client.models.v1_container_image import V1ContainerImage
 from OpenSSL import crypto
+
 from sigopt.paths import ensure_dir, get_root_subdir
 
 from ..exceptions import FileAlreadyExistsError, NodesNotReadyError, OrchestrateException
 from ..provider.constants import Provider
 from ..services.base import Service
 from ..version import CLI_NAME
 from .http_proxy import KubeProxyHTTPAdapter
 
 
-DEFAULT_NAMESPACE = 'default'
-ORCHESTRATE_NAMESPACE = 'orchestrate'
-KUBESYSTEM_NAMESPACE = 'kube-system'
+DEFAULT_NAMESPACE = "default"
+ORCHESTRATE_NAMESPACE = "orchestrate"
+KUBESYSTEM_NAMESPACE = "kube-system"
 NVIDIA_DEVICE_PLUGIN_URL = "https://raw.githubusercontent.com/NVIDIA/k8s-device-plugin/v0.9.0/nvidia-device-plugin.yml"
 
-# NOTE(dan): monkeypatch for containerd not naming all images (?)
+
+# NOTE: monkeypatch for containerd not naming all images (?)
 # https://github.com/kubernetes-client/python/issues/895#issuecomment-515025300
 # pylint: disable=all
 def names(self, names):
   self._names = names
+
+
 V1ContainerImage.names = V1ContainerImage.names.setter(names)
 # pylint: enable=all
 
+
 class NoNodesInClusterError(NodesNotReadyError):
   def __init__(self):
     super().__init__(
-      'Looks like your cluster does not have any nodes.'
-      ' Please check that your cluster configuration file has defined either `cpu` or `gpu` nodes.'
-      ' For AWS clusters, check that you see nodes on the EC2 console.'
+      "Looks like your cluster does not have any nodes. Please check that your"
+      " cluster configuration file has defined either `cpu` or `gpu` nodes. For"
+      " AWS clusters, check that you see nodes on the EC2 console."
     )
 
+
 class NodeStatusNotReadyError(NodesNotReadyError):
   def __init__(self):
     super().__init__(
-      'None of your nodes are ready to go.'
-      f' Run `{CLI_NAME} kubectl get nodes` to see the status of your nodes.'
+      f"None of your nodes are ready to go. Run `{CLI_NAME} kubectl get nodes` to see the status of your nodes."
     )
 
+
 class KubernetesException(OrchestrateException):
   pass
 
+
 class JobNotFoundException(KubernetesException):
   pass
 
+
 class PodNotFoundException(KubernetesException):
   pass
 
+
 class StartJobException(KubernetesException):
   pass
 
+
 class CleanupFailedException(KubernetesException):
   pass
 
+
 class KubernetesService(Service):
   def __init__(self, services):
     super().__init__(services)
     self._kube_config = None
-    self._kube_dir = get_root_subdir('cluster')
+    self._kube_dir = get_root_subdir("cluster")
     self._set_all_clients()
 
   def warmup(self):
     kube_configs = self._get_config_files()
     if kube_configs:
       self._kube_config = os.path.join(self._kube_dir, kube_configs[0])
     try:
       configuration = client.Configuration()
       config.load_kube_config(self._kube_config, client_configuration=configuration)
-      if os.environ.get('HTTPS_PROXY'):
-        configuration.proxy = os.environ['HTTPS_PROXY']
+      if os.environ.get("HTTPS_PROXY"):
+        configuration.proxy = os.environ["HTTPS_PROXY"]
       api_client = client.ApiClient(configuration)
       self._set_all_clients(api_client)
     except Exception as e:
-      if 'Invalid kube-config file. No configuration found.' not in str(e):
+      if "Invalid kube-config file. No configuration found." not in str(e):
         self.services.logging_service.warning(
-          'Experienced the following error while attempting to create kubernetes client from cluster configuration:'
-          '\n%s'
-          '\nDisconnecting and reconnecting may resolve the issue.'
-          '\nPlease try running:'
-          f'\n\t{CLI_NAME} cluster disconnect -a',
+          (
+            "Experienced the following error while attempting to create"
+            " kubernetes client from cluster"
+            " configuration:\n%s\nDisconnecting and reconnecting may"
+            " resolve the issue.\nPlease try"
+            f" running:\n\t{CLI_NAME} cluster disconnect -a"
+          ),
           str(e),
         )
       self._set_all_clients(None)
 
   @property
   def kube_config(self):
     return self._kube_config
 
   def get_jobs(self, job_name=None):
     if job_name:
       try:
         return self._v1_batch.read_namespaced_job(job_name, ORCHESTRATE_NAMESPACE)
       except client.rest.ApiException as e:
         if e.status == http_client.NOT_FOUND:
-          raise JobNotFoundException(f'Job with name {job_name} not found') from e
+          raise JobNotFoundException(f"Job with name {job_name} not found") from e
         else:
           raise
     else:
       return self._v1_batch.list_namespaced_job(ORCHESTRATE_NAMESPACE, watch=False)
 
   def get_jobs_by_label_selector(self, label_selector):
     return self._v1_batch.list_namespaced_job(
@@ -124,38 +137,38 @@
     )
 
   def delete_job(self, job_name, propogation_policy=None):
     try:
       self._v1_batch.delete_namespaced_job(
         job_name,
         ORCHESTRATE_NAMESPACE,
-        body=client.V1DeleteOptions(propagation_policy=propogation_policy)
+        body=client.V1DeleteOptions(propagation_policy=propogation_policy),
       )
     except client.rest.ApiException as e:
       if e.status == http_client.NOT_FOUND:
-        raise JobNotFoundException(f'Job with name {job_name} not found') from e
+        raise JobNotFoundException(f"Job with name {job_name} not found") from e
       else:
         raise
 
   def start_job(self, job_spec_dict):
     try:
       return self._v1_batch.create_namespaced_job(ORCHESTRATE_NAMESPACE, job_spec_dict)
     except client.rest.ApiException as e:
       if e.status == http_client.BAD_REQUEST:
         k8s_error_message = json.loads(e.body).get("message")
         error_message = (
-          "\n[ERROR]\t\tKubernetes reported a bad request"
-          " this is most likely from an error in the experiment configuration file."
-          f"\n\t\tFormated Kubernetes Error:\n{k8s_error_message}\n"
+          "\n[ERROR]\t\tKubernetes reported a bad request this is most"
+          " likely from an error in the experiment configuration"
+          f" file.\n\t\tFormated Kubernetes Error:\n{k8s_error_message}\n"
         )
         raise StartJobException(error_message) from e
       else:
         raise
 
-  # TODO(alexandra): control how logs are displayed, should this be sent to stdout by subprocess or by the CLI?
+  # TODO: control how logs are displayed, should this be sent to stdout by subprocess or by the CLI?
   def logs(self, pod_name, follow=False):
     if follow:
       watcher = watch.Watch()
       return watcher.stream(
         self._v1_core.read_namespaced_pod_log,
         pod_name,
         ORCHESTRATE_NAMESPACE,
@@ -171,15 +184,15 @@
       ORCHESTRATE_NAMESPACE,
       watch=False,
       label_selector=label_selector,
     )
 
   def get_pods(self, job_name=None):
     if job_name:
-      return self.get_pods_by_label_selector(label_selector=f'job-name={job_name}')
+      return self.get_pods_by_label_selector(label_selector=f"job-name={job_name}")
     else:
       return self._v1_core.list_namespaced_pod(ORCHESTRATE_NAMESPACE, watch=False)
 
   def get_pod(self, pod_name):
     return self._v1_core.read_namespaced_pod(pod_name, ORCHESTRATE_NAMESPACE)
 
   def delete_pod(self, pod_name):
@@ -220,19 +233,15 @@
           time.sleep(random.uniform(20, 40))  # nosec
 
   def check_nodes_are_ready(self):
     nodes = self.get_nodes().items
     if not nodes:
       raise NoNodesInClusterError()
 
-    any_node_ready = any(
-      c.type == 'Ready' and c.status == 'True'
-      for node in nodes
-      for c in node.status.conditions
-    )
+    any_node_ready = any(c.type == "Ready" and c.status == "True" for node in nodes for c in node.status.conditions)
     if not any_node_ready:
       raise NodeStatusNotReadyError()
 
   def ensure_config_map(self, config_map):
     try:
       self._v1_core.create_namespaced_config_map(KUBESYSTEM_NAMESPACE, config_map)
     except client.rest.ApiException as e:
@@ -241,26 +250,26 @@
 
   def write_config(self, cluster_name, data):
     ensure_dir(self._kube_dir)
     new_file_path = self._kube_config_path(cluster_name)
     if os.path.isfile(new_file_path):
       raise FileAlreadyExistsError(new_file_path)
 
-    with open(new_file_path, 'w') as f:
+    with open(new_file_path, "w") as f:
       yaml.dump(data, f)
 
     self.warmup()
 
   def test_config(self, retries=0, wait_time=5):
     if self._v1_core is None:
       raise OrchestrateException(
-        'We ran into an issue connecting to your cluster.'
-        '\nDisconnecting and then reconnecting may resolve the issue.'
-        '\nDisconnect by running:'
-        f'\n\t{CLI_NAME} cluster disconnect -a'
+        "We ran into an issue connecting to your cluster."
+        "\nDisconnecting and then reconnecting may resolve the issue."
+        "\nDisconnect by running:"
+        f"\n\t{CLI_NAME} cluster disconnect -a"
       )
 
     for try_number in range(retries + 1):
       try:
         return self._v1_core.list_namespaced_service(DEFAULT_NAMESPACE)
       except Exception:
         if try_number >= retries:
@@ -278,16 +287,16 @@
   def get_cluster_names(self):
     return [self._cluster_name_from_config(c) for c in self._get_config_files()]
 
   def ensure_plugins(self, cluster_name, provider):
     with urllib.request.urlopen(NVIDIA_DEVICE_PLUGIN_URL) as nvidia_plugin_fp:
       self._ensure_plugin_fp(nvidia_plugin_fp, namespace=KUBESYSTEM_NAMESPACE)
     self.ensure_orchestrate_namespace()
-    self._ensure_plugin('orchestrate-controller-roles.yml', namespace=ORCHESTRATE_NAMESPACE)
-    # NOTE(taylor): disabled until remote image builds are working (consistently)
+    self._ensure_plugin("orchestrate-controller-roles.yml", namespace=ORCHESTRATE_NAMESPACE)
+    # NOTE: disabled until remote image builds are working (consistently)
     self.ensure_docker_plugin(
       resources=dict(
         requests=dict(
           cpu="0.5",
           memory="2Gi",
         ),
       ),
@@ -304,19 +313,21 @@
     ca_cert = crypto.X509()
     ca_cert.get_subject().CN = "sigopt:docker ca"
     ca_cert.set_serial_number(random.getrandbits(64))
     ca_cert.set_issuer(ca_cert.get_subject())
     ca_cert.set_pubkey(ca_key)
     ca_cert.gmtime_adj_notBefore(0)
     ca_cert.gmtime_adj_notAfter(ten_years)
-    ca_cert.add_extensions([
-      crypto.X509Extension(b"basicConstraints", True, b"CA:TRUE, pathlen:0"),
-      crypto.X509Extension(b"keyUsage", True, b"keyCertSign, cRLSign"),
-      crypto.X509Extension(b"subjectKeyIdentifier", False, b"hash", subject=ca_cert),
-    ])
+    ca_cert.add_extensions(
+      [
+        crypto.X509Extension(b"basicConstraints", True, b"CA:TRUE, pathlen:0"),
+        crypto.X509Extension(b"keyUsage", True, b"keyCertSign, cRLSign"),
+        crypto.X509Extension(b"subjectKeyIdentifier", False, b"hash", subject=ca_cert),
+      ]
+    )
     ca_cert.sign(ca_key, "sha256")
     outputs["ca.pem"] = crypto.dump_certificate(crypto.FILETYPE_PEM, ca_cert).decode("ascii")
     server_key = crypto.PKey()
     server_key.generate_key(crypto.TYPE_RSA, 4096)
     outputs["key.pem"] = crypto.dump_privatekey(crypto.FILETYPE_PEM, server_key).decode("ascii")
     server_req = crypto.X509Req()
     server_req.get_subject().CN = "sigopt:docker server"
@@ -325,22 +336,24 @@
     server_cert = crypto.X509()
     server_cert.set_serial_number(random.getrandbits(64))
     server_cert.gmtime_adj_notBefore(0)
     server_cert.gmtime_adj_notAfter(ten_years)
     server_cert.set_issuer(ca_cert.get_subject())
     server_cert.set_subject(server_req.get_subject())
     server_cert.set_pubkey(server_req.get_pubkey())
-    server_cert.add_extensions([
-      crypto.X509Extension(
-        b"subjectAltName",
-        False,
-        f"DNS:localhost, DNS:docker.{KUBESYSTEM_NAMESPACE}.svc.cluster.local, IP:127.0.0.1".encode(),
-      ),
-      crypto.X509Extension(b"extendedKeyUsage", False, b"serverAuth"),
-    ])
+    server_cert.add_extensions(
+      [
+        crypto.X509Extension(
+          b"subjectAltName",
+          False,
+          f"DNS:localhost, DNS:docker.{KUBESYSTEM_NAMESPACE}.svc.cluster.local, IP:127.0.0.1".encode(),
+        ),
+        crypto.X509Extension(b"extendedKeyUsage", False, b"serverAuth"),
+      ]
+    )
     server_cert.sign(ca_key, "sha256")
     outputs["cert.pem"] = crypto.dump_certificate(crypto.FILETYPE_PEM, server_cert).decode("ascii")
     return outputs
 
   def is_docker_installed(self):
     try:
       self._v1_apps.read_namespaced_stateful_set("docker", KUBESYSTEM_NAMESPACE)
@@ -356,43 +369,50 @@
         docker_pod = self._v1_core.read_namespaced_pod("docker-0", KUBESYSTEM_NAMESPACE)
         if docker_pod.status.phase == "Running":
           return
       except client.rest.ApiException as e:
         if e.status != http_client.NOT_FOUND:
           raise
       time.sleep(sleep_time)
-    raise TimeoutError("\n".join([
-      "Timed out waiting for Docker to start.",
-      "You can find more information by running the following:",
-      "\tsigopt cluster kubectl -nkube-system describe pod/docker-0",
-    ]))
+    raise TimeoutError(
+      "\n".join(
+        [
+          "Timed out waiting for Docker to start.",
+          "You can find more information by running the following:",
+          "\tsigopt cluster kubectl -nkube-system describe pod/docker-0",
+        ]
+      )
+    )
 
   def ensure_docker_plugin(self, resources, storage_capacity):
     docker_certs_secret_name = "docker-certs"
     try:
       self._v1_core.read_namespaced_secret(docker_certs_secret_name, KUBESYSTEM_NAMESPACE)
     except client.rest.ApiException as e:
       if e.status != http_client.NOT_FOUND:
         raise
       docker_certs = self.create_docker_tls_certs()
-      self._v1_core.create_namespaced_secret(KUBESYSTEM_NAMESPACE, {
-        "metadata": {
-          "name": docker_certs_secret_name,
-          "labels": {"app": "docker"},
+      self._v1_core.create_namespaced_secret(
+        KUBESYSTEM_NAMESPACE,
+        {
+          "metadata": {
+            "name": docker_certs_secret_name,
+            "labels": {"app": "docker"},
+          },
+          "data": {key: base64.b64encode(value.encode()).decode("ascii") for key, value in docker_certs.items()},
+          "type": "Opaque",
         },
-        "data": {key: base64.b64encode(value.encode()).decode("ascii") for key, value in docker_certs.items()},
-        "type": "Opaque",
-      })
+      )
 
     with self.services.resource_service.open("plugins", "docker-statefulset.yml") as resource_fp:
       docker_stateful_set_template = yaml.safe_load(resource_fp)
     docker_stateful_set_template["spec"]["template"]["spec"]["containers"][0]["resources"] = resources
-    docker_stateful_set_template["spec"]["volumeClaimTemplates"][0]["spec"]["resources"]["requests"]["storage"] = (
-      storage_capacity
-    )
+    docker_stateful_set_template["spec"]["volumeClaimTemplates"][0]["spec"]["resources"]["requests"][
+      "storage"
+    ] = storage_capacity
     self._apply_object(
       self._v1_apps.create_namespaced_stateful_set,
       self._v1_apps.patch_namespaced_stateful_set,
       docker_stateful_set_template,
       KUBESYSTEM_NAMESPACE,
     )
     with self.services.resource_service.open("plugins", "docker-service.yml") as resource_fp:
@@ -401,15 +421,18 @@
       self._v1_core.create_namespaced_service,
       self._v1_core.patch_namespaced_service,
       docker_service_template,
       KUBESYSTEM_NAMESPACE,
     )
 
   def mount_http_proxy_adapter(self, session):
-    session.mount(self._api_client.configuration.host, KubeProxyHTTPAdapter(k8s_api_client=self._api_client))
+    session.mount(
+      self._api_client.configuration.host,
+      KubeProxyHTTPAdapter(k8s_api_client=self._api_client),
+    )
 
   def get_docker_connection_url(self):
     return (
       f"{self._api_client.configuration.host}"
       f"/api/v1/namespaces/{KUBESYSTEM_NAMESPACE}/services/https:docker:https/proxy"
     )
 
@@ -420,15 +443,17 @@
       if e.status != http_client.NOT_FOUND:
         raise
     selector = "orchestrate/cleanup-before-destroy"
     for pvc in self._v1_core.list_persistent_volume_claim_for_all_namespaces(
       label_selector=selector,
     ).items:
       self._v1_core.delete_namespaced_persistent_volume_claim(pvc.metadata.name, pvc.metadata.namespace)
-    remaining_pvs = backoff.on_predicate(backoff.expo, lambda pvs: len(pvs.items) > 0, max_time=120)(self._v1_core.list_persistent_volume)()
+    remaining_pvs = backoff.on_predicate(backoff.expo, lambda pvs: len(pvs.items) > 0, max_time=120)(
+      self._v1_core.list_persistent_volume
+    )()
     if remaining_pvs.items:
       raise CleanupFailedException(
         "Some volumes could not be cleaned up, please remove them before destroying the cluster"
       )
 
   def ensure_orchestrate_namespace(self):
     try:
@@ -444,44 +469,39 @@
       try:
         utils.create_from_yaml(self._api_client, temp_fp.name)
       except utils.FailToCreateError as fce:
         if not all(exc.status == http_client.CONFLICT for exc in fce.api_exceptions):
           raise
 
   def _ensure_plugin(self, file_name, namespace):
-    with self.services.resource_service.open('plugins', file_name) as file_content:
+    with self.services.resource_service.open("plugins", file_name) as file_content:
       self._ensure_plugin_fp(file_content, namespace)
 
   def _cluster_name_from_config(self, config_name):
     basename = os.path.basename(config_name)
-    if basename.startswith('config-'):
-      return basename[len('config-'):]
+    if basename.startswith("config-"):
+      return basename[len("config-") :]
     else:
       return None
 
   def get_nodes(self):
     return self._v1_core.list_node()
 
   def _delete_config(self, cluster_name):
     self._kube_config = None
     self._set_all_clients()
     os.remove(self._kube_config_path(cluster_name))
 
   def _kube_config_path(self, cluster_name):
-    filename = f'config-{cluster_name}'
+    filename = f"config-{cluster_name}"
     return os.path.join(self._kube_dir, filename)
 
   def _get_config_files(self):
     if os.path.exists(self._kube_dir):
-      return [
-        config
-        for config
-        in os.listdir(self._kube_dir)
-        if config.startswith('config-')
-      ]
+      return [config for config in os.listdir(self._kube_dir) if config.startswith("config-")]
     return []
 
   def _set_all_clients(self, api_client=None):
     self._api_client = api_client
     if api_client:
       self._v1_apps = client.AppsV1Api(api_client)
       self._v1_batch = client.BatchV1Api(api_client)
@@ -494,20 +514,18 @@
       self._v1_rbac = None
 
   def _get_autoscaler_args(self, cluster_name):
     aws_provider = self.services.provider_broker.get_provider_service(Provider.AWS)
     aws_services = aws_provider.aws_services
     autoscaler_stack = aws_services.cloudformation_service.describe_eks_cluster_autoscaler_role_stack(cluster_name)
     autoscaler_role_arn = [
-      out["OutputValue"]
-      for out in autoscaler_stack.outputs
-      if out["OutputKey"] == 'ClusterAutoscalerRoleArn'
+      out["OutputValue"] for out in autoscaler_stack.outputs if out["OutputKey"] == "ClusterAutoscalerRoleArn"
     ][0]
 
-    kubernetes_version = aws_services.eks_service.describe_cluster(cluster_name)['cluster']['version']
+    kubernetes_version = aws_services.eks_service.describe_cluster(cluster_name)["cluster"]["version"]
     return (autoscaler_role_arn, kubernetes_version)
 
   def _get_autoscaler_image_version(self, kubernetes_version):
     k8s_version_to_autoscaler_release = {
       "1.20": "1.20.3",
       "1.21": "1.21.2",
     }
@@ -521,25 +539,25 @@
       cluster_role_dict,
       role_dict,
       cluster_role_binding_dict,
       role_binding_dict,
       deployment_dict,
     ) = objs
 
-    service_account_dict['metadata']['annotations'] = {
-      'eks.amazonaws.com/role-arn': autoscaler_role_arn,
+    service_account_dict["metadata"]["annotations"] = {
+      "eks.amazonaws.com/role-arn": autoscaler_role_arn,
     }
 
     autoscaler_version = self._get_autoscaler_image_version(kubernetes_version)
     autoscaler_image = f"k8s.gcr.io/autoscaling/cluster-autoscaler:v{autoscaler_version}"
-    deployment_dict['spec']['template']['spec']['containers'][0]['image'] = autoscaler_image
+    deployment_dict["spec"]["template"]["spec"]["containers"][0]["image"] = autoscaler_image
 
-    auto_discovery_tag = f'tag=k8s.io/cluster-autoscaler/enabled,k8s.io/cluster-autoscaler/{cluster_name}'
-    auto_discovery_arg = f'--node-group-auto-discovery=asg:{auto_discovery_tag}'
-    deployment_dict['spec']['template']['spec']['containers'][0]['command'].append(auto_discovery_arg)
+    auto_discovery_tag = f"tag=k8s.io/cluster-autoscaler/enabled,k8s.io/cluster-autoscaler/{cluster_name}"
+    auto_discovery_arg = f"--node-group-auto-discovery=asg:{auto_discovery_tag}"
+    deployment_dict["spec"]["template"]["spec"]["containers"][0]["command"].append(auto_discovery_arg)
     return (
       service_account_dict,
       cluster_role_dict,
       role_dict,
       cluster_role_binding_dict,
       role_binding_dict,
       deployment_dict,
@@ -549,23 +567,30 @@
     kwargs = {"body": body}
     if namespace is not None:
       kwargs["namespace"] = namespace
     try:
       create_func(**kwargs)
     except client.rest.ApiException as e:
       if e.status == http_client.CONFLICT:
-        kwargs['name'] = body['metadata']['name']
+        kwargs["name"] = body["metadata"]["name"]
         patch_func(**kwargs)
       else:
         raise
 
   def create_autoscaler(self, cluster_name):
     (autoscaler_role_arn, kubernetes_version) = self._get_autoscaler_args(cluster_name)
     autoscaler_dicts = self._parameterize_autoscaler_dicts(cluster_name, autoscaler_role_arn, kubernetes_version)
-    (sa_dict, cluster_role_dict, role_dict, crb_dict, rb_dict, deployment_dict) = autoscaler_dicts
+    (
+      sa_dict,
+      cluster_role_dict,
+      role_dict,
+      crb_dict,
+      rb_dict,
+      deployment_dict,
+    ) = autoscaler_dicts
     self._apply_object(
       self._v1_core.create_namespaced_service_account,
       self._v1_core.patch_namespaced_service_account,
       sa_dict,
       KUBESYSTEM_NAMESPACE,
     )
     self._apply_object(
@@ -594,27 +619,34 @@
       self._v1_apps.create_namespaced_deployment,
       self._v1_apps.patch_namespaced_deployment,
       deployment_dict,
       KUBESYSTEM_NAMESPACE,
     )
 
   def _delete_autoscaler_object(self, delete_func, body, namespace=None):
-    kwargs = {'name': body['metadata']['name']}
+    kwargs = {"name": body["metadata"]["name"]}
     if namespace is not None:
-      kwargs['namespace'] = namespace
+      kwargs["namespace"] = namespace
     try:
       delete_func(**kwargs)
     except client.rest.ApiException as e:
       if e.status != http_client.NOT_FOUND:
         raise
 
   def delete_autoscaler(self, cluster_name):
     (autoscaler_role_arn, kubernetes_version) = self._get_autoscaler_args(cluster_name)
     autoscaler_dicts = self._parameterize_autoscaler_dicts(cluster_name, autoscaler_role_arn, kubernetes_version)
-    (sa_dict, cluster_role_dict, role_dict, crb_dict, rb_dict, deployment_dict) = autoscaler_dicts
+    (
+      sa_dict,
+      cluster_role_dict,
+      role_dict,
+      crb_dict,
+      rb_dict,
+      deployment_dict,
+    ) = autoscaler_dicts
 
     self._delete_autoscaler_object(
       self._v1_core.delete_namespaced_service_account,
       sa_dict,
       KUBESYSTEM_NAMESPACE,
     )
     self._delete_autoscaler_object(
```

### Comparing `sigopt-8.8.0/sigopt/orchestrate/lib/lists.py` & `sigopt-8.8.1/sigopt/orchestrate/lib/lists.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,48 +5,48 @@
 Common utility functions for working with lists
 """
 from .types import is_mapping, is_sequence, is_set
 
 
 def list_get(lis, index):
   """
-  Gets the list item at the provided index, or None if that index is invalid
-  """
+    Gets the list item at the provided index, or None if that index is invalid
+    """
   try:
     return lis[index]
   except IndexError:
     return None
 
 
 def remove_nones(lis):
   """
-  Returns a copy of this object with all `None` values removed.
-  """
+    Returns a copy of this object with all `None` values removed.
+    """
   if is_mapping(lis):
     return {k: v for k, v in lis.items() if v is not None}
   if is_set(lis):
     return lis - {None}
   if is_sequence(lis):
     return [l for l in lis if l is not None]
   raise Exception(f"Unsupported type: {type(lis)}")
 
 
 def coalesce(*args):
   """
-  Returns the first non-None value, or None if no such value exists
-  """
+    Returns the first non-None value, or None if no such value exists
+    """
   return list_get(remove_nones(args), 0)
 
 
 def partition(lis, predicate):
   """
-  Splits a list into two lists based on a predicate. The first list will contain
-  all elements of the provided list where predicate is true, and the second list
-  will contain the rest
-  """
+    Splits a list into two lists based on a predicate. The first list will contain
+    all elements of the provided list where predicate is true, and the second list
+    will contain the rest
+    """
   as_list = list(lis)
   true_list = []
   false_list = []
   for l in as_list:
     pred_value = predicate(l)
     if pred_value is True:
       true_list.append(l)
```

### Comparing `sigopt-8.8.0/sigopt/orchestrate/lib/types.py` & `sigopt-8.8.1/sigopt/orchestrate/lib/types.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,47 +2,53 @@
 #
 # SPDX-License-Identifier: MIT
 from collections import abc as _abc
 
 
 def is_sequence(val):
   """
-  Returns True iff this is a "list-like" type. Avoids the common error that strings
-  are iterable, and handles numpy and protobufs correctly
-  """
-  return (isinstance(val, _abc.Sequence) and not isinstance(val, str))
+    Returns True iff this is a "list-like" type. Avoids the common error that strings
+    are iterable, and handles numpy and protobufs correctly
+    """
+  return isinstance(val, _abc.Sequence) and not isinstance(val, str)
+
 
 def is_string_sequence(val):
   """
-  Returns True iff this is a "list-like" type and all list elements are strings.
-  """
+    Returns True iff this is a "list-like" type and all list elements are strings.
+    """
   return is_sequence(val) and all(is_string(element) for element in val)
 
+
 def is_mapping(val):
   """
-  Returns True iff this is a "dict-like" type
-  """
+    Returns True iff this is a "dict-like" type
+    """
   return isinstance(val, _abc.Mapping)
 
+
 def is_set(val):
   """
-  Returns True iff this is a "set-like" type
-  """
+    Returns True iff this is a "set-like" type
+    """
   return isinstance(val, (frozenset, set))
 
+
 def is_string(val):
   """
-  Return True iff this is a string
-  """
+    Return True iff this is a string
+    """
   return isinstance(val, str)
 
+
 def is_integer(val):
   """
-  Return True iff this is an integer
-  """
+    Return True iff this is an integer
+    """
   return (val is not True) and (val is not False) and isinstance(val, int)
 
+
 def is_boolean(val):
   """
-  Return True iff this is a boolean
-  """
+    Return True iff this is a boolean
+    """
   return isinstance(val, bool)
```

### Comparing `sigopt-8.8.0/sigopt/orchestrate/logging/service.py` & `sigopt-8.8.1/sigopt/orchestrate/logging/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # SPDX-License-Identifier: MIT
 import logging
 
 from ..services.base import Service
 
 
 class LoggingService(Service):
-  def __init__(self, services, logger_name='sigopt'):
+  def __init__(self, services, logger_name="sigopt"):
     super().__init__(services)
     self._logger = logging.getLogger(logger_name)
 
   @property
   def logger(self):
     return self._logger
```

### Comparing `sigopt-8.8.0/sigopt/orchestrate/model_packer/service.py` & `sigopt-8.8.1/sigopt/orchestrate/model_packer/service.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 import os
-import shutil
 import shlex
+import shutil
 
 from sigopt.config import config as sigopt_config
 
 from ..common import TemporaryDirectory
 from ..services.base import Service
 
 
@@ -25,62 +25,63 @@
     lines.append(f"ENV SIGOPT_API_VERIFY_SSL_CERTS {shlex.quote(verify_ssl_certs)}")
   if no_verify_ssl_certs:
     lines.append(f"ENV SIGOPT_API_NO_VERIFY_SSL_CERTS {shlex.quote(no_verify_ssl_certs)}")
   if sigopt_home:
     lines.append(f"ENV SIGOPT_HOME {shlex.quote(sigopt_home)}")
   return "".join(f"{l}\n" for l in lines)
 
+
 class ModelPackerService(Service):
   def build_image(
     self,
     docker_service,
     repository,
     tag,
     quiet=False,
     dockerfile=None,
   ):
     if not os.path.isfile(dockerfile):
-      raise Exception('Please specify a path to a Dockerfile')
+      raise Exception("Please specify a path to a Dockerfile")
 
     with open(dockerfile) as dockerfile_fp:
       dockerfile_contents = dockerfile_fp.read()
       cwd = os.getcwd()
 
       user_image_tag = docker_service.build(
         directory=cwd,
         dockerfile_contents=dockerfile_contents,
         quiet=quiet,
         show_all_logs=True,
       )
 
     try:
       with TemporaryDirectory() as root_dirname:
-        ssl_dirname = os.path.join(root_dirname, 'etc', 'ssl')
-        sigopt_config_dirname = os.path.join(root_dirname, 'etc', 'sigopt', 'client')
+        ssl_dirname = os.path.join(root_dirname, "etc", "ssl")
+        sigopt_config_dirname = os.path.join(root_dirname, "etc", "sigopt", "client")
         for dirname in (ssl_dirname, sigopt_config_dirname):
           os.makedirs(dirname)
 
         verify_ssl_certs = None
         no_verify_ssl_certs = None
         local_verify_ssl_certs = self.services.sigopt_service.verify_ssl_certs
-        # NOTE(dan): we intentionally leave verify_ssl_certs as None in the bool/True case because
+        # NOTE: we intentionally leave verify_ssl_certs as None in the bool/True case because
         # verify_ssl_certs must refer to a file when being passed as an environment variable
         if isinstance(local_verify_ssl_certs, bool):
           no_verify_ssl_certs = not local_verify_ssl_certs
         elif local_verify_ssl_certs is not None:
-          build_context_verify_ssl_certs = os.path.join(ssl_dirname, 'sigopt-ca.crt')
+          build_context_verify_ssl_certs = os.path.join(ssl_dirname, "sigopt-ca.crt")
           shutil.copyfile(local_verify_ssl_certs, build_context_verify_ssl_certs)
-          verify_ssl_certs = build_context_verify_ssl_certs.replace(root_dirname, '/')
+          verify_ssl_certs = build_context_verify_ssl_certs.replace(root_dirname, "/")
 
         sigopt_home = None
         local_config_path = sigopt_config.config_json_path
         if local_config_path is not None and os.path.exists(local_config_path):
-          build_context_config_path = os.path.join(sigopt_config_dirname, 'config.json')
+          build_context_config_path = os.path.join(sigopt_config_dirname, "config.json")
           shutil.copyfile(local_config_path, build_context_config_path)
-          sigopt_home = os.path.dirname(os.path.dirname(build_context_config_path.replace(root_dirname, '/')))
+          sigopt_home = os.path.dirname(os.path.dirname(build_context_config_path.replace(root_dirname, "/")))
 
         return docker_service.build(
           tag=docker_service.format_image_name(repository, tag),
           directory=root_dirname,
           dockerfile_contents=create_model_packer_dockerfile(
             base_image=user_image_tag,
             verify_ssl_certs=verify_ssl_certs,
```

### Comparing `sigopt-8.8.0/sigopt/orchestrate/options_validator/service.py` & `sigopt-8.8.1/sigopt/orchestrate/options_validator/service.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,94 +5,82 @@
 from ..node_groups import ALL_NODE_GROUP_TYPES, NODE_GROUP_TYPE_CPU, NODE_GROUP_TYPE_GPU, NODE_GROUP_TYPE_SYSTEM
 from ..services.base import Service
 
 
 class OptionsValidatorService(Service):
   def validate_resources(self, gpus=None, requests=None, limits=None):
     if gpus is not None:
-      assert is_integer(gpus) and gpus >= 0, f'resources.gpus is not a non-negative integer: {gpus}'
+      assert is_integer(gpus) and gpus >= 0, f"resources.gpus is not a non-negative integer: {gpus}"
     if requests is not None:
-      assert is_mapping(requests), f'resources.requests is not a mapping: {requests}'
+      assert is_mapping(requests), f"resources.requests is not a mapping: {requests}"
     if limits is not None:
-      assert is_mapping(limits), f'resources.limits is not a mapping: {limits}'
+      assert is_mapping(limits), f"resources.limits is not a mapping: {limits}"
 
   def validate_aws_for_orchestrate(
     self,
     aws_access_key_id=None,
     aws_secret_access_key=None,
   ):
-    self.validate_aws_keys(
-      aws_access_key_id=aws_access_key_id,
-      aws_secret_access_key=aws_secret_access_key
-    )
+    self.validate_aws_keys(aws_access_key_id=aws_access_key_id, aws_secret_access_key=aws_secret_access_key)
 
   def validate_aws_for_cluster(
     self,
     aws_access_key_id=None,
     aws_secret_access_key=None,
     additional_policies=None,
   ):
-    self.validate_aws_keys(
-      aws_access_key_id=aws_access_key_id,
-      aws_secret_access_key=aws_secret_access_key
-    )
+    self.validate_aws_keys(aws_access_key_id=aws_access_key_id, aws_secret_access_key=aws_secret_access_key)
 
     if additional_policies:
-      assert is_sequence(additional_policies), f'aws.additional_policies is not a list: {additional_policies}'
+      assert is_sequence(additional_policies), f"aws.additional_policies is not a list: {additional_policies}"
 
   def validate_aws_keys(
     self,
     aws_access_key_id=None,
     aws_secret_access_key=None,
   ):
     if aws_secret_access_key is not None:
-      assert is_string(aws_secret_access_key) and aws_secret_access_key, (
-        f'Please provide a string aws.aws_secret_access_key: {aws_secret_access_key}'
-      )
+      assert (
+        is_string(aws_secret_access_key) and aws_secret_access_key
+      ), f"Please provide a string aws.aws_secret_access_key: {aws_secret_access_key}"
     if aws_access_key_id is not None:
-      assert is_string(aws_access_key_id) and aws_access_key_id, (
-        f'Please provide a string aws.aws_access_key_id: {aws_access_key_id}'
-      )
+      assert (
+        is_string(aws_access_key_id) and aws_access_key_id
+      ), f"Please provide a string aws.aws_access_key_id: {aws_access_key_id}"
 
   def validate_sigopt(self, api_token=None, verify_ssl_certs=None):
     if api_token is not None:
-      assert is_string(api_token) and api_token, (
-        f'Please provide a string sigopt.api_token: {api_token}'
-      )
+      assert is_string(api_token) and api_token, f"Please provide a string sigopt.api_token: {api_token}"
     if verify_ssl_certs is not None:
-      assert (
-        is_boolean(verify_ssl_certs) or (is_string(verify_ssl_certs) and verify_ssl_certs)
-      ), (
-        f'Please provide a boolean or string sigopt.verify_ssl_certs: {verify_ssl_certs}'
-      )
+      assert is_boolean(verify_ssl_certs) or (
+        is_string(verify_ssl_certs) and verify_ssl_certs
+      ), f"Please provide a boolean or string sigopt.verify_ssl_certs: {verify_ssl_certs}"
 
   def validate_cluster_options(
     self,
     provider=None,
     cluster_name=None,
     aws=None,
     kubernetes_version=None,
     **kwargs,
   ):
     unknown_options = set(kwargs) - ALL_NODE_GROUP_TYPES
     assert not unknown_options, f"Unknown options provided: {', '.join(unknown_options)}"
-    assert provider and is_string(provider), (
-      f'We need a string `provider` to create your cluster: {provider}'
-    )
+    assert provider and is_string(provider), f"We need a string `provider` to create your cluster: {provider}"
 
     if aws is not None:
       self.validate_aws_for_cluster(**aws)
 
     if kubernetes_version is not None:
       assert is_string(kubernetes_version), "kubernetes_version should have a string value"
 
-    assert is_string(cluster_name) and cluster_name, 'We need a string `cluster_name` to create your cluster'
-    assert kwargs.get(NODE_GROUP_TYPE_CPU) or kwargs.get(NODE_GROUP_TYPE_GPU), (
-      'Please specify some cpu or gpu (or both) nodes for your cluster'
-    )
+    assert is_string(cluster_name) and cluster_name, "We need a string `cluster_name` to create your cluster"
+    assert kwargs.get(NODE_GROUP_TYPE_CPU) or kwargs.get(
+      NODE_GROUP_TYPE_GPU
+    ), "Please specify some cpu or gpu (or both) nodes for your cluster"
     for node_group_type in ALL_NODE_GROUP_TYPES:
       node_group_options = kwargs.get(node_group_type)
       if not node_group_options:
         continue
       assert is_mapping(node_group_options), f"{node_group_type} is not a mapping: {node_group_options}"
       self.validate_worker_stack(name=node_group_type, **node_group_options)
 
@@ -101,24 +89,24 @@
     name,
     instance_type=None,
     max_nodes=None,
     min_nodes=None,
     node_volume_size=None,
   ):
     if name != NODE_GROUP_TYPE_SYSTEM:
-      assert instance_type is not None, f'Missing: {name}.instance_type'
-      assert max_nodes is not None, f'Missing: {name}.max_nodes (can be the same as {name}.min_nodes)'
-      assert min_nodes is not None, f'Missing: {name}.min_nodes (can be the same as {name}.max_nodes)'
+      assert instance_type is not None, f"Missing: {name}.instance_type"
+      assert max_nodes is not None, f"Missing: {name}.max_nodes (can be the same as {name}.min_nodes)"
+      assert min_nodes is not None, f"Missing: {name}.min_nodes (can be the same as {name}.max_nodes)"
 
     if instance_type is not None:
-      assert is_string(instance_type), f'{name}.instance_type is not a string: {instance_type}'
+      assert is_string(instance_type), f"{name}.instance_type is not a string: {instance_type}"
 
     if max_nodes is not None:
-      assert is_integer(max_nodes) and max_nodes > 0, f'{name}.max_nodes is not a positive integer: {max_nodes}'
+      assert is_integer(max_nodes) and max_nodes > 0, f"{name}.max_nodes is not a positive integer: {max_nodes}"
 
     if min_nodes is not None:
-      assert is_integer(min_nodes) and min_nodes >= 0, f'{name}.min_nodes is not a non-negative integer: {min_nodes}'
+      assert is_integer(min_nodes) and min_nodes >= 0, f"{name}.min_nodes is not a non-negative integer: {min_nodes}"
 
     if node_volume_size is not None:
-      assert is_integer(node_volume_size) and node_volume_size > 0, (
-        f'{name}.node_volume_size is not a positive integer: {node_volume_size}'
-      )
+      assert (
+        is_integer(node_volume_size) and node_volume_size > 0
+      ), f"{name}.node_volume_size is not a positive integer: {node_volume_size}"
```

### Comparing `sigopt-8.8.0/sigopt/orchestrate/paths.py` & `sigopt-8.8.1/sigopt/orchestrate/paths.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,104 +13,99 @@
 from .exceptions import CheckExecutableError
 
 
 def check_executable(command, sha256, full_check):
   exec_path = get_executable_path(command)
   try:
     if full_check:
-      with open(exec_path, 'rb') as exec_fp:
+      with open(exec_path, "rb") as exec_fp:
         contents = exec_fp.read()
       file_sha256 = hashlib.sha256(contents).hexdigest()
     else:
-      with open(f'{exec_path}.sha256', 'r') as exec_sha256_fp:
+      with open(f"{exec_path}.sha256", "r") as exec_sha256_fp:
         file_sha256 = exec_sha256_fp.read()
   except IOError as e:
     if e.errno == errno.ENOENT:
-      raise CheckExecutableError(f'Error opening the hash files for: {command}') from e
+      raise CheckExecutableError(f"Error opening the hash files for: {command}") from e
     raise
 
   if not sha256 == file_sha256:
-    filetype = 'executable' if full_check else 'hash file'
-    raise CheckExecutableError(
-      f"the {filetype} for '{command}' does not have the expected hash"
-    )
+    filetype = "executable" if full_check else "hash file"
+    raise CheckExecutableError(f"the {filetype} for '{command}' does not have the expected hash")
 
   if not os.access(exec_path, os.X_OK):
     raise CheckExecutableError(f"the file for '{command}' is not executable")
 
   if full_check:
-    with open(os.devnull, 'w') as devnull:
+    with open(os.devnull, "w") as devnull:
       try:
         subprocess.check_call([exec_path], stdout=devnull, stderr=devnull)
         subprocess.check_call(
           [command],
-          env={'PATH': get_bin_dir()},
+          env={"PATH": get_bin_dir()},
           stdout=devnull,
           stderr=devnull,
         )
       except subprocess.CalledProcessError as e:
-        raise CheckExecutableError(f'Exception checking the excecutable for {command}: {e}') from e
+        raise CheckExecutableError(f"Exception checking the excecutable for {command}: {e}") from e
       except OSError as e:
         if e.errno == errno.ENOENT:
-          raise CheckExecutableError(f'System cannot find executable for {command}') from e
+          raise CheckExecutableError(f"System cannot find executable for {command}") from e
         raise
 
 
-KUBECTL_VERSION = 'v1.25.2'
-KUBECTL_URL_FORMAT = 'https://dl.k8s.io/release/{}/bin/{}/amd64/kubectl'
-KUBECTL_SHA256_LINUX = '8639f2b9c33d38910d706171ce3d25be9b19fc139d0e3d4627f38ce84f9040eb'
-KUBECTL_SHA256_MAC = 'b859766d7b47267af5cc1ee01a2d0c3c137dbfc53cd5be066181beed11ec7d34'
+KUBECTL_VERSION = "v1.25.2"
+KUBECTL_URL_FORMAT = "https://dl.k8s.io/release/{}/bin/{}/amd64/kubectl"
+KUBECTL_SHA256_LINUX = "8639f2b9c33d38910d706171ce3d25be9b19fc139d0e3d4627f38ce84f9040eb"
+KUBECTL_SHA256_MAC = "b859766d7b47267af5cc1ee01a2d0c3c137dbfc53cd5be066181beed11ec7d34"
 
 AWS_IAM_AUTHENTICATOR_URL_FORMAT = (
-  'https://github.com/kubernetes-sigs/aws-iam-authenticator/releases/download/v0.5.9/aws-iam-'
-  'authenticator_0.5.9_{}_amd64'
+  "https://github.com/kubernetes-sigs/aws-iam-authenticator/releases/download/v0.5.9/aws-iam-"
+  "authenticator_0.5.9_{}_amd64"
 )
-AWS_IAM_AUTHENTICATOR_SHA256_LINUX = 'b192431c22d720c38adbf53b016c33ab17105944ee73b25f485aa52c9e9297a7'
-AWS_IAM_AUTHENTICATOR_SHA256_MAC = '7656bd290a7e9cb588df1d9ccec43fab7f2447b88ed4f41d3f5092fd114b0939'
+AWS_IAM_AUTHENTICATOR_SHA256_LINUX = "b192431c22d720c38adbf53b016c33ab17105944ee73b25f485aa52c9e9297a7"
+AWS_IAM_AUTHENTICATOR_SHA256_MAC = "7656bd290a7e9cb588df1d9ccec43fab7f2447b88ed4f41d3f5092fd114b0939"
+
 
 def check_kubectl_executable(full_check=False):
   check_executable(
-    command='kubectl',
-    sha256=(
-      KUBECTL_SHA256_MAC
-      if current_platform() == Platform.MAC
-      else KUBECTL_SHA256_LINUX
-    ),
+    command="kubectl",
+    sha256=(KUBECTL_SHA256_MAC if current_platform() == Platform.MAC else KUBECTL_SHA256_LINUX),
     full_check=full_check,
   )
 
+
 def check_iam_authenticator_executable(full_check=False):
   check_executable(
-    command='aws-iam-authenticator',
+    command="aws-iam-authenticator",
     sha256=(
-      AWS_IAM_AUTHENTICATOR_SHA256_MAC
-      if current_platform() == Platform.MAC
-      else AWS_IAM_AUTHENTICATOR_SHA256_LINUX
+      AWS_IAM_AUTHENTICATOR_SHA256_MAC if current_platform() == Platform.MAC else AWS_IAM_AUTHENTICATOR_SHA256_LINUX
     ),
     full_check=full_check,
   )
 
+
 def download_executable(command, url):
   executable_path = get_executable_path(command)
   urlretrieve(url, executable_path)  # nosec
   os.chmod(executable_path, 0o700)
-  with \
-    open(executable_path, 'rb') as exec_fp, \
-    open(f'{executable_path}.sha256', 'w') as sha256_fp:
+  with open(executable_path, "rb") as exec_fp, open(f"{executable_path}.sha256", "w") as sha256_fp:
     sha256_fp.write(hashlib.sha256(exec_fp.read()).hexdigest())
 
+
 def download_kubectl_executable():
   download_executable(
-    'kubectl',
+    "kubectl",
     KUBECTL_URL_FORMAT.format(
       KUBECTL_VERSION,
-      ('darwin' if current_platform() == Platform.MAC else 'linux'),
-    )
+      ("darwin" if current_platform() == Platform.MAC else "linux"),
+    ),
   )
 
+
 def download_iam_authenticator_executable():
   download_executable(
-    'aws-iam-authenticator',
+    "aws-iam-authenticator",
     AWS_IAM_AUTHENTICATOR_URL_FORMAT.format(
-      ('darwin' if current_platform() == Platform.MAC else 'linux'),
-    )
+      ("darwin" if current_platform() == Platform.MAC else "linux"),
+    ),
   )
```

### Comparing `sigopt-8.8.0/sigopt/orchestrate/plugins/autoscaler-plugin-template.yml` & `sigopt-8.8.1/sigopt/orchestrate/plugins/autoscaler-plugin-template.yml`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.0/sigopt/orchestrate/plugins/docker-statefulset.yml` & `sigopt-8.8.1/sigopt/orchestrate/plugins/docker-statefulset.yml`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.0/sigopt/orchestrate/plugins/orchestrate-controller-roles.yml` & `sigopt-8.8.1/sigopt/orchestrate/plugins/orchestrate-controller-roles.yml`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.0/sigopt/orchestrate/provider/broker.py` & `sigopt-8.8.1/sigopt/orchestrate/provider/broker.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.0/sigopt/orchestrate/provider/constants.py` & `sigopt-8.8.1/sigopt/orchestrate/provider/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,19 +21,18 @@
 class UnknownProviderStringError(OrchestrateException):
   def __init__(self, provider_string):
     if provider_string is None:
       provider_error = "Please include a provider with your request."
     else:
       provider_error = f"{provider_string!r} is not a supported provider."
 
-    super().__init__(
-      f"{provider_error} Supported providers are: {', '.join(STRING_TO_PROVIDER)}"
-    )
+    super().__init__(f"{provider_error} Supported providers are: {', '.join(STRING_TO_PROVIDER)}")
     self.provider_string = provider_string
 
+
 def string_to_provider(provider_string):
   try:
     return STRING_TO_PROVIDER[provider_string.lower()]
   except (KeyError, AttributeError) as e:
     raise UnknownProviderStringError(provider_string) from e
```

### Comparing `sigopt-8.8.0/sigopt/orchestrate/provider/interface.py` & `sigopt-8.8.1/sigopt/orchestrate/provider/interface.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.0/sigopt/orchestrate/resource/service.py` & `sigopt-8.8.1/sigopt/orchestrate/resource/service.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 import shutil
 import tempfile
-import yaml
 
 import pkg_resources
+import yaml
 
 from ..services.base import Service
 
 
 class ResourceService(Service):
   def get_package_name(self, package):
-    return f'sigopt.orchestrate.{package}'
+    return f"sigopt.orchestrate.{package}"
 
   def stream(self, package, resource):
     return pkg_resources.resource_stream(self.get_package_name(package), resource)
 
   def open(self, package, resource):
     contents_fp = tempfile.NamedTemporaryFile("wb+")
     with self.stream(package, resource) as source:
```

### Comparing `sigopt-8.8.0/sigopt/orchestrate/s3/service.py` & `sigopt-8.8.1/sigopt/orchestrate/s3/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from ..services.aws_base import AwsService
 
 
 class AwsS3Service(AwsService):
   def __init__(self, services, aws_services, **kwargs):
     super().__init__(services, aws_services)
-    self._client = boto3.client('s3', **kwargs)
+    self._client = boto3.client("s3", **kwargs)
     self.region = boto3.session.Session().region_name
     self._init_kwargs = kwargs
 
   @property
   def client(self):
     return self._client
 
@@ -29,15 +29,15 @@
     return f"sigopt.{self.account_id}"
 
   def ensure_orchestrate_bucket(self):
     create_bucket_params = dict(
       ACL="private",
       Bucket=self.orchestrate_bucket_name,
     )
-    # NOTE(taylor): LocationConstraint is required for all regions but us-east-1.
+    # NOTE: LocationConstraint is required for all regions but us-east-1.
     # In us-east-1 create_bucket will fail when LocationConstraint is provided.
     # https://github.com/boto/boto3/issues/125
     if self.region != "us-east-1":
       create_bucket_params["CreateBucketConfiguration"] = {"LocationConstraint": self.region}
     try:
       self.client.create_bucket(**create_bucket_params)
       self.client.put_bucket_encryption(
@@ -47,15 +47,15 @@
             {
               "ApplyServerSideEncryptionByDefault": {
                 "SSEAlgorithm": "AES256",
               },
               "BucketKeyEnabled": True,
             },
           ]
-        }
+        },
       )
     except self.client.exceptions.BucketAlreadyOwnedByYou:
       pass
     return self.orchestrate_bucket_name
 
   def upload_resource_by_hash(self, path_prefix, package, resource_name):
     resource_content = self.services.resource_service.read(package, resource_name)
```

### Comparing `sigopt-8.8.0/sigopt/orchestrate/services/aws_provider_bag.py` & `sigopt-8.8.1/sigopt/orchestrate/services/aws_provider_bag.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.0/sigopt/orchestrate/services/bag.py` & `sigopt-8.8.1/sigopt/orchestrate/services/bag.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 class ServiceBag(object):
   """
-  A top-level container for all of our services. A service bag should be passed
-  around where needed to grant access to these services. This gives us
-  dependency injection, and lets us reuse services when they have a startup
-  cost (such as creating DB connections).
-  """
+    A top-level container for all of our services. A service bag should be passed
+    around where needed to grant access to these services. This gives us
+    dependency injection, and lets us reuse services when they have a startup
+    cost (such as creating DB connections).
+    """
+
   def __init__(self):
     self._create_services()
     self._warmup_services()
 
   def _create_services(self):
     pass
```

### Comparing `sigopt-8.8.0/sigopt/orchestrate/services/orchestrate_bag.py` & `sigopt-8.8.1/sigopt/orchestrate/services/orchestrate_bag.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.0/sigopt/orchestrate/sigopt/service.py` & `sigopt-8.8.1/sigopt/orchestrate/sigopt/service.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,57 +39,53 @@
   def log_collection_enabled(self):
     return config.log_collection_enabled
 
   def check_connection(self):
     try:
       self.conn.experiments().fetch(limit=1)
     except ApiException as e:
-      raise CheckConnectionError(f'An error occured while checking your SigOpt connection: {e}') from e
+      raise CheckConnectionError(f"An error occured while checking your SigOpt connection: {e}") from e
 
   def create_aiexperiment(self, experiment_body, project_id):
     factory = SigOptFactory(project_id)
     return factory.create_prevalidated_aiexperiment(experiment_body)
 
   def fetch_experiment(self, experiment_id):
     factory = SigOptFactory.from_default_project()
     return factory.get_aiexperiment(experiment_id)
 
   def create_run(self, run_name, cluster, project_id):
     factory = SigOptFactory(project_id)
     return factory.create_run(
       name=run_name,
-      metadata={'cluster_name': cluster.name},
+      metadata={"cluster_name": cluster.name},
     )
 
   def fetch_run(self, run_id):
     return self.conn.training_runs(run_id).fetch()
 
   def ensure_project_exists(self, project_id):
     factory = SigOptFactory(project_id)
     return factory.ensure_project_exists()
 
   def iterate_runs_by_filters(self, filters, project=None, client=None):
     if project is None:
       client, project = SigOptFactory.from_default_project().ensure_project_exists()
     return (
-      self.conn.clients(client)
-        .projects(project)
-        .training_runs()
-        .fetch(filters=json.dumps(filters))
-        .iterate_pages()
+      self.conn.clients(client).projects(project).training_runs().fetch(filters=json.dumps(filters)).iterate_pages()
     )
 
   def iterate_runs(self, experiment):
     if experiment.project:
       return self.iterate_runs_by_filters(
-        [{'operator': '==', 'field': 'experiment', 'value': experiment.id}],
+        [{"operator": "==", "field": "experiment", "value": experiment.id}],
         project=experiment.project,
         client=experiment.client,
       )
-    # TODO(patrick): api.sigopt.com returns extended JSON for the new endpoint fetch, which we need for the state
+    # TODO: api.sigopt.com returns extended JSON for the new endpoint fetch, which we need for the state
     # field. But we can only do that for experiments in projects.
     # So we fall back safely here, but this can be removed in the future
     return self.conn.experiments(experiment.id).training_runs().fetch().iterate_pages()
 
   def safe_fetch_experiment(self, experiment_id):
     try:
       return self.fetch_experiment(experiment_id)
```

### Comparing `sigopt-8.8.0/sigopt/orchestrate/status.py` & `sigopt-8.8.1/sigopt/orchestrate/status.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,33 +18,25 @@
   assert experiment_identifier["query"] == IDENTIFIER_QUERY_ID
   experiment_id = experiment_identifier["value"]
   experiment = services.sigopt_service.fetch_experiment(experiment_id)
 
   parsed_job = {}
   parsed_job["experiment_id"] = experiment_id
   parsed_job["experiment_name"] = experiment.name
-  parsed_job["budget"] = (
-    str(float(experiment.budget))
-    if experiment and experiment.budget is not None
-    else 'n/a'
-  )
-  parsed_job["total_run_count"] = (
-    str(experiment.progress.total_run_count) if experiment else 'n/a'
-  )
+  parsed_job["budget"] = str(float(experiment.budget)) if experiment and experiment.budget is not None else "n/a"
+  parsed_job["total_run_count"] = str(experiment.progress.total_run_count) if experiment else "n/a"
 
   runs = list(services.sigopt_service.iterate_runs(experiment))
-  total_failures = sum(v.state == 'failed' for v in runs)
+  total_failures = sum(v.state == "failed" for v in runs)
 
-  yield 'Experiment Name: {experiment_name}'.format(**parsed_job)
-  yield '{total_run_count} / {budget} budget'.format(
-    **parsed_job
-  )
-  yield f'{total_failures} Run(s) failed'
+  yield "Experiment Name: {experiment_name}".format(**parsed_job)
+  yield "{total_run_count} / {budget} budget".format(**parsed_job)
+  yield f"{total_failures} Run(s) failed"
 
-  yield '{:20}\t{:15}\t{:15}\t{:35}'.format(
+  yield "{:20}\t{:15}\t{:15}\t{:35}".format(
     "Run Name",
     "Pod phase",
     "Status",
     "Link",
   )
 
   pods_by_name = {
@@ -53,24 +45,22 @@
       experiment_identifier["pod_label_selector"],
     ).items
   }
   runs_by_name = {run.to_json()["name"]: run for run in runs}
   for run_name in sorted(set(pods_by_name) | set(runs_by_name)):
     run = runs_by_name.get(run_name)
     pod = pods_by_name.get(run_name)
-    state = run.state if run else 'creating'
-    phase = pod.status.phase if pod else 'Deleted'
+    state = run.state if run else "creating"
+    phase = pod.status.phase if pod else "Deleted"
     url = f"https://app.sigopt.com/run/{run.id}" if run else ""
-    yield f'{run_name:20}\t{phase:15}\t{state:15}\t{url:35}'
+    yield f"{run_name:20}\t{phase:15}\t{state:15}\t{url:35}"
+
+  yield (f"Follow logs: sigopt cluster kubectl logs -ltype=run,experiment={experiment.id} --max-log-requests=1000 -f")
+  yield f"View more at: https://app.sigopt.com/aiexperiment/{experiment_id}"
 
-  yield (
-    "Follow logs: "
-    f"sigopt cluster kubectl logs -ltype=run,experiment={experiment.id} --max-log-requests=1000 -f"
-  )
-  yield f'View more at: https://app.sigopt.com/aiexperiment/{experiment_id}'
 
 def print_run_status(run_identifier, services):
   run_identifier = maybe_convert_to_run_identifier(run_identifier)
   run, pod = get_run_and_pod_from_identifier(run_identifier, services)
   if not run and not pod:
     yield f"Could not find a run for {run_identifier['raw']}"
     return
@@ -103,40 +93,39 @@
   # scrape info from the pod
   if pod:
     run_name = run_name or pod.metadata.name
     node_name = node_name or pod.spec.node_name
     pod_phase = pod_phase or pod.status.phase
 
   # set values if still None
-  run_state = run_state or 'creating'
-  pod_phase = pod_phase or 'Deleted'
-  node_name = node_name or 'unknown'
+  run_state = run_state or "creating"
+  pod_phase = pod_phase or "Deleted"
+  node_name = node_name or "unknown"
 
   yield f"Run Name: {run_name}"
   if run_id is not None:
     yield f"Link: https://app.sigopt.com/run/{run_id}"
   yield f"State: {run_state}"
   if experiment_id is not None:
     yield f"Experiment link: https://app.sigopt.com/experiment/{experiment_id}"
   if suggestion_id is not None:
     yield f"Suggestion id: {suggestion_id}"
   if observation_id is not None:
     yield f"Observation id: {observation_id}"
   yield f"Pod phase: {pod_phase}"
   yield f"Node name: {node_name}"
-  yield (
-    "Follow logs: "
-    f"sigopt cluster kubectl logs \"pod/{run_name}\" -f"
-  )
+  yield (f'Follow logs: sigopt cluster kubectl logs "pod/{run_name}" -f')
+
 
 IDENTIFIER_TYPE_TO_PRINTER = {
   IDENTIFIER_TYPE_EXPERIMENT: print_experiment_status,
   IDENTIFIER_TYPE_RUN: print_run_status,
   IDENTIFIER_TYPE_SUGGESTION: print_run_status,
 }
 
+
 def print_status(identifier, services):
   try:
     printer = IDENTIFIER_TYPE_TO_PRINTER[identifier["type"]]
   except KeyError as ke:
     raise NotImplementedError() from ke
   return printer(identifier, services)
```

### Comparing `sigopt-8.8.0/sigopt/orchestrate/stop.py` & `sigopt-8.8.1/sigopt/orchestrate/stop.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,22 +7,23 @@
 def stop_experiment(experiment_identifier, services):
   assert experiment_identifier["type"] == IDENTIFIER_TYPE_EXPERIMENT
   experiment_jobs = services.kubernetes_service.get_jobs_by_label_selector(
     experiment_identifier["controller_label_selector"],
   ).items
 
   for job in experiment_jobs:
-    services.kubernetes_service.delete_job(job.metadata.name, propogation_policy='Background')
+    services.kubernetes_service.delete_job(job.metadata.name, propogation_policy="Background")
+
 
 def stop_run(run_identifier, services):
   assert run_identifier["type"] == IDENTIFIER_TYPE_RUN
 
   _, pod = get_run_and_pod_from_identifier(run_identifier, services)
 
   if pod:
     services.kubernetes_service.delete_pod(pod.metadata.name)
 
   run_controller_jobs = services.kubernetes_service.get_jobs_by_label_selector(
     run_identifier["controller_label_selector"],
   ).items
   for job in run_controller_jobs:
-    services.kubernetes_service.delete_job(job.metadata.name, propogation_policy='Background')
+    services.kubernetes_service.delete_job(job.metadata.name, propogation_policy="Background")
```

### Comparing `sigopt-8.8.0/sigopt/orchestrate/sts/service.py` & `sigopt-8.8.1/sigopt/orchestrate/sts/service.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 
 from ..services.aws_base import AwsService
 
 
 class AwsStsService(AwsService):
   def __init__(self, services, aws_services, **kwargs):
     super().__init__(services, aws_services)
-    self._client = boto3.client('sts', **kwargs)
+    self._client = boto3.client("sts", **kwargs)
 
   @property
   def client(self):
     return self._client
 
   def assume_role(self, role_arn, duration_seconds=900):
     return self.client.assume_role(
       RoleArn=role_arn,
-      RoleSessionName=f'sigopt-{uuid.uuid4()}',
+      RoleSessionName=f"sigopt-{uuid.uuid4()}",
       DurationSeconds=duration_seconds,
     )
```

### Comparing `sigopt-8.8.0/sigopt/paths.py` & `sigopt-8.8.1/sigopt/paths.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,25 +2,29 @@
 #
 # SPDX-License-Identifier: MIT
 import errno
 import os
 
 
 def get_root_dir():
-  root_dir = os.environ.get('SIGOPT_HOME', os.path.join('~', '.sigopt'))
+  root_dir = os.environ.get("SIGOPT_HOME", os.path.join("~", ".sigopt"))
   return os.path.expanduser(root_dir)
 
+
 def get_root_subdir(dirname):
   return os.path.join(get_root_dir(), dirname)
 
+
 def get_bin_dir():
-  return get_root_subdir('bin')
+  return get_root_subdir("bin")
+
 
 def ensure_dir(path):
   try:
     os.makedirs(path)
   except os.error as oserr:
     if oserr.errno != errno.EEXIST:
       raise
 
+
 def get_executable_path(command):
   return os.path.join(get_bin_dir(), command)
```

### Comparing `sigopt-8.8.0/sigopt/ratelimit.py` & `sigopt-8.8.1/sigopt/ratelimit.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,17 @@
     self.count = 0
 
   def increment_and_check(self):
     with self.thread_lock:
       self.count += 1
       multiples_over = self.count // self.limit
     if multiples_over:
-      quadratic_backoff = multiples_over ** 2
+      quadratic_backoff = multiples_over**2
       jitter = random.random() * 2
       time.sleep(quadratic_backoff + jitter)
 
   def clear(self):
     with self.thread_lock:
       self.count = 0
 
+
 failed_status_rate_limit = _FailedStatusRateLimit(5)
```

### Comparing `sigopt-8.8.0/sigopt/request_driver.py` & `sigopt-8.8.1/sigopt/request_driver.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
-import backoff
 import os
-import requests
 from http import HTTPStatus
+
+import backoff
+import requests
 from requests.adapters import HTTPAdapter
 
 from .compat import json as simplejson
 from .config import config
 from .exception import ApiException, ConnectionException
 from .objects import ApiObject
 from .ratelimit import failed_status_rate_limit
 from .urllib3_patch import ExpiringHTTPConnectionPool, ExpiringHTTPSConnectionPool
 from .version import VERSION
 
-DEFAULT_API_URL = 'https://api.sigopt.com'
+
+DEFAULT_API_URL = "https://api.sigopt.com"
 DEFAULT_HTTP_TIMEOUT = 150
 
 
 def get_expiring_session():
   adapter = HTTPAdapter()
   adapter.poolmanager.pool_classes_by_scheme = {
     "http": ExpiringHTTPConnectionPool,
     "https": ExpiringHTTPSConnectionPool,
   }
   session = requests.Session()
   session.mount("http://", adapter)
   session.mount("https://", adapter)
   return session
 
+
 class RequestDriver(object):
   api_version = "v1"
 
   def __init__(
     self,
     client_token=None,
     headers=None,
@@ -57,16 +60,16 @@
       self.verify_ssl_certs = os.environ.get("SIGOPT_API_VERIFY_SSL_CERTS")
     self.proxies = proxies
     self.timeout = timeout
     self.client_ssl_certs = client_ssl_certs
     self.session = session or get_expiring_session()
     self.api_url = api_url or os.environ.get("SIGOPT_API_URL") or DEFAULT_API_URL
     self.default_headers = {
-      'Content-Type': 'application/json',
-      'X-SigOpt-Python-Version': VERSION,
+      "Content-Type": "application/json",
+      "X-SigOpt-Python-Version": VERSION,
     }
     if headers:
       self.default_headers.update(headers)
 
   def _set_auth(self, username, password):
     if username is not None:
       self.auth = requests.auth.HTTPBasicAuth(username, password)
@@ -77,81 +80,78 @@
     req_params = params or {}
 
     def serialize(value):
       if isinstance(value, (dict, list)):
         return simplejson.dumps(value, indent=None, separators=(",", ":"))
       return str(value)
 
-    return dict((
-      (key, serialize(ApiObject.as_json(value)))
-      for key, value
-      in req_params.items()
-      if value is not None
-    ))
+    return dict(((key, serialize(ApiObject.as_json(value))) for key, value in req_params.items() if value is not None))
 
   def set_client_token(self, client_token):
-    self._set_auth(client_token, '')
+    self._set_auth(client_token, "")
 
   def set_api_url(self, api_url):
     self.api_url = api_url
 
   def _request(self, method, url, params, json, headers):
     headers = self._with_default_headers(headers)
     try:
-      caller = (self.session or requests)
+      caller = self.session or requests
       response = caller.request(
         method=method,
         url=url,
         params=params,
         json=json,
         auth=self.auth,
         headers=headers,
         verify=self.verify_ssl_certs,
         proxies=self.proxies,
         timeout=self.timeout,
         cert=self.client_ssl_certs,
       )
     except requests.exceptions.RequestException as rqe:
-      message = ['An error occurred connecting to SigOpt.']
+      message = ["An error occurred connecting to SigOpt."]
       if not url or not url.startswith(DEFAULT_API_URL):
-        message.append('The host may be misconfigured or unavailable.')
-      message.append('Contact support@sigopt.com for assistance.')
-      message.append('')
+        message.append("The host may be misconfigured or unavailable.")
+      message.append("Contact support@sigopt.com for assistance.")
+      message.append("")
       message.append(str(rqe))
-      raise ConnectionException('\n'.join(message)) from rqe
+      raise ConnectionException("\n".join(message)) from rqe
     return response
 
   def request(self, method, path, data, headers):
     method = method.upper()
     url = "/".join(str(v) for v in (self.api_url, self.api_version, *path))
-    if method in ('GET', 'DELETE'):
+    if method in ("GET", "DELETE"):
       json, params = None, self._request_params(data)
     else:
       json, params = ApiObject.as_json(data), None
     retry = backoff.on_predicate(
       backoff.expo,
       lambda response: response.status_code == HTTPStatus.TOO_MANY_REQUESTS,
       max_time=self.timeout,
       jitter=backoff.full_jitter,
     )
     response = retry(self._request)(method, url, params, json, headers)
     return self._handle_response(response)
 
   def _with_default_headers(self, headers):
-    user_agent_str = f'sigopt-python/{VERSION}'
+    user_agent_str = f"sigopt-python/{VERSION}"
     user_agent_info = config.get_user_agent_info()
     if user_agent_info:
-      user_agent_info_str = ''.join([
-        '(',
-        '; '.join(user_agent_info),
-        ')',
-      ])
-      user_agent_str = ' '.join([user_agent_str, user_agent_info_str])
+      user_agent_info_str = "".join(
+        [
+          "(",
+          "; ".join(user_agent_info),
+          ")",
+        ]
+      )
+      user_agent_str = " ".join([user_agent_str, user_agent_info_str])
 
-    request_headers = {'User-Agent': user_agent_str}
+    request_headers = {"User-Agent": user_agent_str}
 
     if headers:
       request_headers.update(headers)
 
     request_headers.update(self.default_headers)
     return request_headers
 
@@ -161,15 +161,15 @@
 
     if status_code == 204:
       response_json = None
     else:
       try:
         response_json = simplejson.loads(response.text)
       except ValueError:
-        response_json = {'message': response.text}
+        response_json = {"message": response.text}
         status_code = 500 if is_success else status_code
 
     if is_success:
       failed_status_rate_limit.clear()
       return response_json
     failed_status_rate_limit.increment_and_check()
     raise ApiException(response_json, status_code)
```

### Comparing `sigopt-8.8.0/sigopt/resource.py` & `sigopt-8.8.1/sigopt/resource.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 from .endpoint import BoundApiEndpoint
 
+
 _NO_ARG = object()
 
+
 class BoundApiResource(object):
-  def __init__(self, resource, id, path):
+  def __init__(self, resource, id_, path):
     self._resource = resource
-    self._id = id
+    self._id = id_
 
     self._base_path = list(path)
-    if id is not _NO_ARG:
-      self._base_path.append(id)
+    if id_ is not _NO_ARG:
+      self._base_path.append(id_)
 
   def get_bound_entity(self, name):
     endpoint = self._resource._endpoints.get(name)
     if endpoint:
       return BoundApiEndpoint(self, endpoint)
     sub_resource = self._resource._sub_resources.get(name)
     if sub_resource:
@@ -24,51 +26,46 @@
     return None
 
   def __getattr__(self, attr):
     bound_entity = self.get_bound_entity(attr)
     if bound_entity:
       return bound_entity
     raise AttributeError(
-        'Cannot find attribute `{attribute}` on resource `{resource}`, likely no endpoint exists for: '
-        '{path}/{attribute}, or `{resource}` does not support `{attribute}`.'
-      .format(
+      "Cannot find attribute `{attribute}` on resource `{resource}`, likely no"
+      " endpoint exists for: {path}/{attribute}, or `{resource}` does not support"
+      " `{attribute}`.".format(
         attribute=attr,
         resource=self._resource._name,
         path="/".join(self._base_path),
       )
     )
 
+
 class PartiallyBoundApiResource(object):
   def __init__(self, resource, bound_parent_resource):
     self._resource = resource
     self._bound_parent_resource = bound_parent_resource
 
-  def __call__(self, id=_NO_ARG):
+  def __call__(self, id_=_NO_ARG):
     path = self._bound_parent_resource._base_path + [self._resource._name]
-    return BoundApiResource(self._resource, id, path)
+    return BoundApiResource(self._resource, id_, path)
+
 
 class BaseApiResource(object):
   def __init__(self, conn, name, endpoints=None, resources=None):
     self._conn = conn
     self._name = name
 
-    self._endpoints = dict((
-      (endpoint._attribute_name, endpoint)
-      for endpoint
-      in endpoints
-    )) if endpoints else {}
-
-    self._sub_resources = dict((
-      (resource._name, resource)
-      for resource
-      in resources
-    )) if resources else {}
+    self._endpoints = dict(((endpoint._attribute_name, endpoint) for endpoint in endpoints)) if endpoints else {}
+
+    self._sub_resources = dict(((resource._name, resource) for resource in resources)) if resources else {}
+
+  def __call__(self, id_=_NO_ARG):
+    return BoundApiResource(self, id_, [self._name])
 
-  def __call__(self, id=_NO_ARG):
-    return BoundApiResource(self, id, [self._name])
 
 class ApiResource(BaseApiResource):
   def __init__(self, conn, name, endpoints=None, resources=None):
     super().__init__(
       conn=conn,
       name=name,
       endpoints=endpoints,
```

### Comparing `sigopt-8.8.0/sigopt/run_context.py` & `sigopt-8.8.1/sigopt/run_context.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,43 +5,48 @@
 
 import requests
 
 from .config import config
 from .exception import RunException
 from .file_utils import create_api_image_payload, get_blob_properties
 from .interface import get_connection
-from .lib import remove_nones, sanitize_number, validate_name, is_mapping, is_string
-from .sigopt_logging import print_logger
+from .lib import is_mapping, is_string, remove_nones, sanitize_number, validate_name
 from .objects import TrainingRun
-from .run_params import RunParameters, GlobalRunParameters
+from .run_params import GlobalRunParameters, RunParameters
+from .sigopt_logging import print_logger
 
 
 _UNSET = object()
 
+
 def maybe_truncate_log(log_content):
   # If log content is extremely long, preserve some useful content instead of failing.
-  # TODO(patrick): Support streaming logs to avoid this
+  # TODO: Support streaming logs to avoid this
   max_size = 1024
   if len(log_content) >= max_size:
-    truncated_disclaimer = '[ WARNING ] The max size has been reached so these logs have been truncated'
+    truncated_disclaimer = "[ WARNING ] The max size has been reached so these logs have been truncated"
     half = max_size // 2
     head = log_content[:half]
     tail = log_content[-half:]
-    log_content = '\n\n'.join([
-      truncated_disclaimer,
-      head,
-      '... truncated ...',
-      tail,
-    ])
+    log_content = "\n\n".join(
+      [
+        truncated_disclaimer,
+        head,
+        "... truncated ...",
+        tail,
+      ]
+    )
   return log_content
 
+
 class NoDefaultParameterError(RunException):
   def __init__(self, parameter_name):
     super().__init__(f'No default provided for parameter "{parameter_name}"')
 
+
 class BaseRunContext(object):
   @property
   def id(self):
     raise NotImplementedError
 
   @property
   def experiment(self):
@@ -68,15 +73,15 @@
 
   def _log_dev_metadata(self, metadata):
     raise NotImplementedError
 
   def _log_metrics(self, metrics):
     raise NotImplementedError
 
-  def _log_model(self, type):
+  def _log_model(self, type_):
     raise NotImplementedError
 
   def _log_source_code(self, source_code):
     raise NotImplementedError
 
   def _set_logs(self, logs):
     raise NotImplementedError
@@ -87,21 +92,21 @@
   def _log_image(self, name, payload):
     raise NotImplementedError
 
   def _end(self, exception):
     raise NotImplementedError
 
   def set_parameter(self, name, value):
-    '''
-    sigopt.set_parameter(name, value)
-    name: string, required
-      The name of the parameter.
-    value: number/string, required
-      The value of the parameter.
-    '''
+    """
+        sigopt.set_parameter(name, value)
+        name: string, required
+          The name of the parameter.
+        value: number/string, required
+          The value of the parameter.
+        """
     return self._set_parameters({name: value})
 
   def set_parameter_meta(self, name, value):
     return self._set_parameters_meta({name: value})
 
   def set_parameters_meta(self, parameters_meta):
     return self._set_parameters_meta(parameters_meta)
@@ -112,228 +117,222 @@
   def set_parameters_source(self, parameters, source):
     return self._set_parameters_meta({key: {"source": source} for key in parameters.keys()})
 
   def set_parameters_sources_meta(self, source_name, sort, default_show):
     return self._set_parameters_sources({source_name: {"sort": sort, "default_show": default_show}})
 
   def set_parameters(self, parameters):
-    '''
-    sigopt.set_parameter(parameters)
-    name: dict, required
-      A mapping of parameter names to values.
-    '''
+    """
+        sigopt.set_parameter(parameters)
+        name: dict, required
+          A mapping of parameter names to values.
+        """
     return self._set_parameters(parameters)
 
   def log_dataset(self, name):
-    '''
-    sigopt.log_dataset(name)
-      Logs a dataset that will be used for your Run.
-    name: string, required
-      The name of the dataset you would like to track.
-    '''
-    validate_name('dataset name', name)
+    """
+        sigopt.log_dataset(name)
+          Logs a dataset that will be used for your Run.
+        name: string, required
+          The name of the dataset you would like to track.
+        """
+    validate_name("dataset name", name)
     self._log_dataset(name)
 
   def log_failure(self):
-    '''
-    sigopt.log_failure()
-      Indicates that the Run has failed for any reason.
-    '''
+    """
+        sigopt.log_failure()
+          Indicates that the Run has failed for any reason.
+        """
     self._log_failure()
 
   def log_metadata(self, key, value):
-    '''
-    sigopt.log_metadata(key, value)
-      Stores some extra information about your Run.
-    key: string, required
-      The metadata key that your would like to store.
-    value: number/object, required
-      The value of the metadata that you would like to track.
-      If value is not a number then it will be logged as a string.
-    '''
-    validate_name('metadata key', key)
+    """
+        sigopt.log_metadata(key, value)
+          Stores some extra information about your Run.
+        key: string, required
+          The metadata key that your would like to store.
+        value: number/object, required
+          The value of the metadata that you would like to track.
+          If value is not a number then it will be logged as a string.
+        """
+    validate_name("metadata key", key)
     if value is not None and not isinstance(value, str):
       try:
-        value = sanitize_number('metadata', key, value)
+        value = sanitize_number("metadata", key, value)
       except ValueError:
         value = str(value)
     return self._log_metadata({key: value})
 
-
   def log_dev_metadata(self, key, value):
-    validate_name('metadata key', key)
+    validate_name("metadata key", key)
     if value is not None and not isinstance(value, str):
       try:
-        value = sanitize_number('metadata', key, value)
+        value = sanitize_number("metadata", key, value)
       except ValueError:
         value = str(value)
     return self._log_dev_metadata({key: value})
 
-
   def log_sys_metadata(self, key, value, mode=None):
-    validate_name('metadata key', key)
-    if mode == 'metadata':
+    validate_name("metadata key", key)
+    if mode == "metadata":
       return self.log_metadata(key, value)
-    elif mode == 'dev':
+    elif mode == "dev":
       return self.log_dev_metadata(key, value)
     return self._log_sys_metadata({key: value})
 
   def log_metric(self, name, value, stddev=None):
-    '''
-    sigopt.log_metric(name, value, stddev=None)
-      Logs a metric value from your model's evaluation.
-    name: string, required
-      The name of the metric that you would like to track.
-    value: number, required
-      The value of the metric to track.
-    stddev: number
-      The standard deviation of the metric to track.
-    '''
-    validate_name('metric name', name)
+    """
+        sigopt.log_metric(name, value, stddev=None)
+          Logs a metric value from your model's evaluation.
+        name: string, required
+          The name of the metric that you would like to track.
+        value: number, required
+          The value of the metric to track.
+        stddev: number
+          The standard deviation of the metric to track.
+        """
+    validate_name("metric name", name)
     metric_log = {}
-    metric_log['value'] = sanitize_number('metric', name, value)
+    metric_log["value"] = sanitize_number("metric", name, value)
     if stddev is not None:
-      metric_log['value_stddev'] = sanitize_number('metric stddev', name, stddev)
+      metric_log["value_stddev"] = sanitize_number("metric stddev", name, stddev)
     self._log_metrics({name: metric_log})
 
   def log_metrics(self, *args, **metric_kwargs):
-    '''
-    sigopt.log_metrics(metrics_dict)
-    sigopt.log_metrics(**metric_kwargs)
-      Logs multiple metric values for your run. Metrics can be provided as a dictionary or as keyword arguments.
-    metrics_dict: dict
-      A dictionary mapping metric names to their values.
-    '''
+    """
+        sigopt.log_metrics(metrics_dict)
+        sigopt.log_metrics(**metric_kwargs)
+          Logs multiple metric values for your run. Metrics can be provided as a dictionary or as keyword arguments.
+        metrics_dict: dict
+          A dictionary mapping metric names to their values.
+        """
     all_metrics = dict()
     all_metrics.update(*args, **metric_kwargs)
     metric_logs = {}
     for name, value in all_metrics.items():
-      validate_name('metric name', name)
+      validate_name("metric name", name)
       metric_logs[name] = {"value": sanitize_number("metric", name, value)}
     self._log_metrics(metric_logs)
 
-  def log_model(self, type=None):
-    '''
-    sigopt.log_model(type=None)
-      Logs information about your model.
-      This will be converted to a string before it is tracked.
-    type: object
-      The model object being tracked, or a string representing the type of model.
-      The str builtin will be used to convert your model to a string.
-    '''
-    if type is not None:
-      type = str(type)
-    self._log_model(type)
+  def log_model(self, type_=None):
+    """
+        sigopt.log_model(type_=None)
+          Logs information about your model.
+          This will be converted to a string before it is tracked.
+        type_: object
+          The model object being tracked, or a string representing the type_ of model.
+          The str builtin will be used to convert your model to a string.
+        """
+    if type_ is not None:
+      type_ = str(type_)
+    self._log_model(type_)
 
   def log_source_code(self, **source_code):
     self._log_source_code(source_code)
 
   def set_logs(self, logs):
     if not is_mapping(logs):
       raise TypeError(f"logs must be a mapping, got {type(logs).__name__}")
     for stream_name, stream_content in logs.items():
       validate_name("log stream", stream_name)
       if not is_string(stream_content):
         raise TypeError(f"log content must be a string, got {type(logs).__name__}")
     self._set_logs(logs)
 
   def log_checkpoint(self, values):
-    '''
-    sigopt.log_checkpoint(values)
-      Logs a checkpoint from your model's evaluation.
-    values: dict
-      A mapping of the metric names to the values they take for the current checkpoint.
-    '''
+    """
+        sigopt.log_checkpoint(values)
+          Logs a checkpoint from your model's evaluation.
+        values: dict
+          A mapping of the metric names to the values they take for the current checkpoint.
+        """
     if not isinstance(values, dict):
-      raise ValueError('values must be a dict')
+      raise ValueError("values must be a dict")
     checkpoint_values = []
     for name, value in values.items():
-      validate_name('metric name', name)
+      validate_name("metric name", name)
       if value is not None:
-        checkpoint_values.append({
-          'name': name,
-          'value': sanitize_number('metric_stddev', name, value),
-        })
+        checkpoint_values.append(
+          {
+            "name": name,
+            "value": sanitize_number("metric_stddev", name, value),
+          }
+        )
     self._log_checkpoint(checkpoint_values)
 
   def log_image(self, image, name=None):
-    '''
-    sigopt.log_image(image, name=None)
-      Logs an image artifact from your model's evaluation. See the documentation for more details:
-      https://docs.sigopt.com/ai-module-api-references/api_reference/python_tracking#sigopt.log_image-image-name-none
-    image: string, PIL.Image.Image, matplotlib.figure.Figure or numpy.ndarray, required
-      The image artifact to upload. This will be converted to an appropriate format and then uploaded.
-    name: string
-      An optional name to give your uploaded image.
-    '''
+    """
+        sigopt.log_image(image, name=None)
+          Logs an image artifact from your model's evaluation. See the documentation for more details:
+          https://docs.sigopt.com/ai-module-api-references/api_reference/python_tracking#sigopt.log_image-image-name-none
+        image: string, PIL.Image.Image, matplotlib.figure.Figure or numpy.ndarray, required
+          The image artifact to upload. This will be converted to an appropriate format and then uploaded.
+        name: string
+          An optional name to give your uploaded image.
+        """
     if name is not None:
-      validate_name('image name', name)
+      validate_name("image name", name)
     payload = create_api_image_payload(image)
     if payload is None:
       return
     image_data = payload[1]
     with image_data:
       self._log_image(name, payload)
 
   def end(self, exception=None):
-    '''
-    run.end(exception=None)
-      Stops the run. In most cases it should be easier to use your run in a context manager instead, ex.
-      with run:
-        ...
-    exception: instanceof(Exception)
-      The exception that occurred that caused the termination of the run. Not needed if the run ended gracefully.
-    '''
+    """
+        run.end(exception=None)
+          Stops the run. In most cases it should be easier to use your run in a context manager instead, ex.
+          with run:
+            ...
+        exception: instanceof(Exception)
+          The exception that occurred that caused the termination of the run. Not needed if the run ended gracefully.
+        """
     self._end(exception=exception)
 
 
 def updates(update_key):
-
   def function_wrapper(wrapped_function):
-
     def function_impl(self, *args, **kwargs):
       update_value = wrapped_function(self, *args, **kwargs)
       self._update_run({update_key: update_value})
 
     function_impl.__doc__ = wrapped_function.__doc__
     return function_impl
 
   return function_wrapper
 
-def creates_checkpoint():
 
+def creates_checkpoint():
   def function_wrapper(wrapped_function):
-
     @functools.wraps(wrapped_function)
     def function_impl(self, *args, **kwargs):
       checkpoint_values = wrapped_function(self, *args, **kwargs)
-      self._create_checkpoint({'values': checkpoint_values})
+      self._create_checkpoint({"values": checkpoint_values})
 
     return function_impl
 
   return function_wrapper
 
+
 def allow_state_update(new_state, old_state):
   if new_state == old_state:
     return False
   precedence = {
-    'failed': 2,
-    'completed': 1,
+    "failed": 2,
+    "completed": 1,
   }
   new_state_precedence = precedence.get(new_state, 0)
   old_state_precedence = precedence.get(old_state, 0)
   return new_state_precedence >= old_state_precedence
 
+
 class RunContext(BaseRunContext):
-  def __init__(
-    self,
-    connection,
-    run,
-    default_params=None
-  ):
+  def __init__(self, connection, run, default_params=None):
     super().__init__()
     self.connection = connection
     self.run = run
     fixed_values = dict(run.assignments)
     self._params = RunParameters(self, fixed_values, default_params)
 
   def to_json(self):
@@ -356,109 +355,109 @@
   @property
   def params(self):
     return self._params
 
   def __enter__(self):
     return self
 
-  def __exit__(self, type, value, tb):
+  def __exit__(self, type_, value, tb):
     self._end(exception=value)
 
   def _end(self, exception):
     old_run_state = self.connection.training_runs(self.run.id).fetch().state
-    new_run_state = 'failed' if exception else 'completed'
+    new_run_state = "failed" if exception else "completed"
     if allow_state_update(new_run_state, old_run_state):
-      self._update_run({'state': new_run_state})
-    print_logger.info("Run finished, view it on the SigOpt dashboard at https://app.sigopt.com/run/%s", self.id)
+      self._update_run({"state": new_run_state})
+    print_logger.info(
+      "Run finished, view it on the SigOpt dashboard at https://app.sigopt.com/run/%s",
+      self.id,
+    )
 
   def _request(self, method, path, params, headers=None):
     run_id = self.run.id
     return self.connection.impl.request(
       method,
       ["training_runs", run_id, *path],
       params,
       headers,
     )
 
   def _update_run(self, body):
     self._request(
-      method='MERGE',
+      method="MERGE",
       path=[],
       params=body,
-      headers={'X-Response-Content': 'skip'},
+      headers={"X-Response-Content": "skip"},
     )
 
   def _create_checkpoint(self, body):
     self._request(
-      method='POST',
+      method="POST",
       path=["checkpoints"],
       params=body,
-      headers={'X-Response-Content': 'skip'},
+      headers={"X-Response-Content": "skip"},
     )
 
-  @updates('assignments')
+  @updates("assignments")
   def _set_parameters(self, parameters):
     return parameters
 
-  @updates('assignments_meta')
+  @updates("assignments_meta")
   def _set_parameters_meta(self, parameters_meta):
     return parameters_meta
 
-  @updates('assignments_sources')
+  @updates("assignments_sources")
   def _set_parameters_sources(self, assignments_sources):
     return assignments_sources
 
-  @updates('datasets')
+  @updates("datasets")
   def _log_dataset(self, name):
     return {name: {}}
 
-  @updates('state')
+  @updates("state")
   def _log_failure(self):
-    return 'failed'
+    return "failed"
 
-  @updates('metadata')
+  @updates("metadata")
   def _log_metadata(self, metadata):
     return metadata
 
-  @updates('sys_metadata')
+  @updates("sys_metadata")
   def _log_sys_metadata(self, metadata):
     return metadata
 
-  @updates('dev_metadata')
+  @updates("dev_metadata")
   def _log_dev_metadata(self, metadata):
     return metadata
 
-  @updates('values')
+  @updates("values")
   def _log_metrics(self, metrics):
     return metrics
 
-  @updates('model')
-  def _log_model(self, type):
-    return remove_nones({'type': type})
+  @updates("model")
+  def _log_model(self, type_):
+    return remove_nones({"type": type_})
 
-  @updates('source_code')
+  @updates("source_code")
   def _log_source_code(self, source_code):
     return source_code
 
-  @updates('logs')
+  @updates("logs")
   def _set_logs(self, logs):
-    return {
-      name: {"content": maybe_truncate_log(content)}
-      for name, content in logs.items()
-    }
+    return {name: {"content": maybe_truncate_log(content)} for name, content in logs.items()}
 
   @creates_checkpoint()
   def _log_checkpoint(self, values):
     return values
 
   def _log_image(self, name, payload):
     filename, image_data, content_type = payload
     content_length, content_md5_base64 = get_blob_properties(image_data)
     file_info = self._request(
-      method='POST',
+      method="POST",
       path=["files"],
       params={
         "content_length": content_length,
         "content_md5": content_md5_base64,
         "content_type": content_type,
         "name": name,
         "filename": filename,
@@ -470,19 +469,21 @@
       upload_info["method"],
       upload_info["url"],
       headers=upload_info["headers"],
       data=image_data,
     )
     response.raise_for_status()
 
+
 class GlobalRunContext(BaseRunContext):
-  '''
-  If a RunContext is available then methods will call the RunContext.
-  Fallback to noop.
-  '''
+  """
+    If a RunContext is available then methods will call the RunContext.
+    Fallback to noop.
+    """
+
   CONFIG_CONTEXT_KEY = "global_run_context"
 
   def __init__(self, run_context):
     self._run_context = run_context
     self._params = GlobalRunParameters(self)
 
   @property
@@ -514,16 +515,16 @@
   def from_config(cls, config_):
     data = config_.get_context_data(cls)
     run_context = None
     if data is not None:
       run_context = RunContext.from_json(data)
     return cls(run_context)
 
-def delegate_to_run_context(method_name):
 
+def delegate_to_run_context(method_name):
   def func(self, *args, **kwargs):
     run_context = self.run_context
     if run_context is not None:
       getattr(run_context, method_name)(*args, **kwargs)
 
   setattr(GlobalRunContext, method_name, func)
```

### Comparing `sigopt-8.8.0/sigopt/run_factory.py` & `sigopt-8.8.1/sigopt/run_factory.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 from .defaults import get_default_name
-from .sigopt_logging import print_logger
 from .run_context import RunContext
+from .sigopt_logging import print_logger
 
 
 class BaseRunFactory(object):
   run_context_class = RunContext
 
   def _on_run_created(self, run):
-    print_logger.info("Run started, view it on the SigOpt dashboard at https://app.sigopt.com/run/%s", run.id)
+    print_logger.info(
+      "Run started, view it on the SigOpt dashboard at https://app.sigopt.com/run/%s",
+      run.id,
+    )
 
   @property
   def project(self):
     raise NotImplementedError
 
   def _create_run(self, name, metadata):
     raise NotImplementedError
```

### Comparing `sigopt-8.8.0/sigopt/run_params.py` & `sigopt-8.8.1/sigopt/run_params.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from .lib import is_string
 
 
 _get = object.__getattribute__
 _set = object.__setattr__
 
+
 class RunParameters(MutableMapping):
   def __init__(self, run_context, fixed_items, default_items=None):
     if default_items:
       items = dict(default_items)
       items.update(fixed_items)
     else:
       items = dict(fixed_items)
```

### Comparing `sigopt-8.8.0/sigopt/urllib3_patch.py` & `sigopt-8.8.1/sigopt/urllib3_patch.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,20 +3,22 @@
 # SPDX-License-Identifier: MIT
 import logging
 import time
 
 from urllib3.connection import HTTPConnection, HTTPSConnection
 from urllib3.connectionpool import HTTPConnectionPool, HTTPSConnectionPool
 
+
 logger = logging.getLogger("sigopt.urllib3_patch")
 
+
 class SigOptHTTPConnection(HTTPConnection):
   """
-  Tracks the time since the last activity of the connection.
-  """
+    Tracks the time since the last activity of the connection.
+    """
 
   def __init__(self, *args, **kwargs):
     super().__init__(*args, **kwargs)
     self.reset_activity()
 
   def reset_activity(self):
     self.last_activity = time.time()
@@ -29,30 +31,33 @@
     super().request_chunked(*args, **kwargs)
     self.reset_activity()
 
   def close(self, *args, **kwargs):
     super().close()
     self.reset_activity()
 
+
 class SigOptHTTPSConnection(SigOptHTTPConnection, HTTPSConnection):
   pass
 
+
 class ExpiringHTTPConnectionPool(HTTPConnectionPool):
   """
-  Returns a new connection when the time since the connection was last used is greater than the expiration time.
-  """
+    Returns a new connection when the time since the connection was last used is greater than the expiration time.
+    """
 
   ConnectionCls = SigOptHTTPConnection
 
   def __init__(self, *args, expiration_seconds=30, **kwargs):
     super().__init__(*args, **kwargs)
     self.expiration_seconds = expiration_seconds
 
   def _get_conn(self, timeout=None):
     conn = super()._get_conn(timeout=timeout)
     if time.time() - conn.last_activity > self.expiration_seconds:
       logger.debug("Abandoning expired connection")
       return self._new_conn()
     return conn
 
+
 class ExpiringHTTPSConnectionPool(ExpiringHTTPConnectionPool, HTTPSConnectionPool):
   ConnectionCls = SigOptHTTPSConnection
```

### Comparing `sigopt-8.8.0/sigopt/utils.py` & `sigopt-8.8.1/sigopt/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,25 +2,28 @@
 #
 # SPDX-License-Identifier: MIT
 import contextlib
 from http import HTTPStatus
 
 from sigopt.exception import ApiException
 
+
 class HandledException:
   def __init__(self):
     self.exception = None
 
+
 @contextlib.contextmanager
 def accept_sigopt_not_found():
   handled = HandledException()
   try:
     yield handled
   except ApiException as ae:
     if ae.status_code != HTTPStatus.NOT_FOUND:
       raise
     handled.exception = ae
 
+
 def batcher(alist, n=1):
   l = len(alist)
   for ndx in range(0, l, n):
-    yield alist[ndx:min(ndx + n, l)]
+    yield alist[ndx : min(ndx + n, l)]
```

### Comparing `sigopt-8.8.0/sigopt/validate/aiexperiment_input.py` & `sigopt-8.8.1/sigopt/validate/aiexperiment_input.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
-from sigopt.lib import validate_name, is_string, is_sequence, is_mapping, is_number, is_integer
+from sigopt.lib import is_integer, is_mapping, is_number, is_sequence, is_string, validate_name
 
 from .common import validate_top_level_dict
 from .exceptions import ValidationError
 from .keys import PROJECT_KEY
 
 
 def get_validated_name(aiexperiment_input):
@@ -15,23 +15,22 @@
     raise ValidationError("name is required") from ke
   try:
     validate_name("AIExperiment name", name)
   except ValueError as ve:
     raise ValidationError(str(ve)) from ve
   return name
 
+
 def get_validated_metric(metric_input):
   validated_metric = {}
 
   if is_mapping(metric_input):
     metric = dict(metric_input)
   else:
-    raise ValidationError(
-      "all metrics must be a mapping of keys to values"
-    )
+    raise ValidationError("all metrics must be a mapping of keys to values")
 
   try:
     metric_name = metric["name"]
   except KeyError as ke:
     raise ValidationError("all metrics require a name") from ke
 
   try:
@@ -62,29 +61,29 @@
   for key, value in metric.items():
     if key not in validated_metric:
       if not is_string(key):
         raise ValidationError("all metric keys must be strings")
       validated_metric[key] = value
   return validated_metric
 
+
 def get_validated_metrics(aiexperiment_input):
   try:
     metrics = aiexperiment_input.pop("metrics")
   except KeyError as ke:
     raise ValidationError("a list of metrics is required") from ke
   if not is_sequence(metrics):
     raise ValidationError("metrics must be a non-empty list")
   metrics = list(metrics)
   if not metrics:
     raise ValidationError("metrics must be a non-empty list")
-  validated_metrics = [
-    get_validated_metric(metric) for metric in metrics
-  ]
+  validated_metrics = [get_validated_metric(metric) for metric in metrics]
   return validated_metrics
 
+
 def get_validated_parameters(aiexperiment_input):
   try:
     parameters = aiexperiment_input.pop("parameters")
   except KeyError as ke:
     raise ValidationError("a list of parameters is required") from ke
   if not is_sequence(parameters):
     raise ValidationError("parameters must be a non-empty list")
@@ -118,34 +117,37 @@
       if key not in validated_param:
         if not is_string(key):
           raise ValidationError("all parameter keys must be strings")
         validated_param[key] = value
     validated_parameters.append(validated_param)
   return validated_parameters
 
+
 def get_validated_budget(aiexperiment_input):
   budget = aiexperiment_input["budget"]
   if not (budget is None or is_number(budget) and budget >= 0):
     raise ValidationError("budget must be a non-negative number")
   if budget == float("inf"):
     raise ValidationError("budget cannot be infinity")
   return budget
 
+
 def get_validated_parallel_bandwidth(aiexperiment_input):
   parallel_bandwidth = aiexperiment_input.pop("parallel_bandwidth")
   if parallel_bandwidth is None or is_integer(parallel_bandwidth) and parallel_bandwidth > 0:
     return parallel_bandwidth
   raise ValidationError("parallel_bandwidth must be a positive integer")
 
+
 def validate_aiexperiment_input(aiexperiment_input):
   aiexperiment_input = validate_top_level_dict(aiexperiment_input)
   if PROJECT_KEY in aiexperiment_input:
     raise ValidationError(
-      'The project field is not permitted in the AIExperiment.'
-      ' Please set the SIGOPT_PROJECT environment variable instead.'
+      "The project field is not permitted in the AIExperiment."
+      " Please set the SIGOPT_PROJECT environment variable instead."
     )
   aiexperiment_input = dict(aiexperiment_input)
   validated = {}
   validated["name"] = get_validated_name(aiexperiment_input)
   validated["parameters"] = get_validated_parameters(aiexperiment_input)
   validated["metrics"] = get_validated_metrics(aiexperiment_input)
   try:
@@ -158,20 +160,21 @@
     pass
   for key, value in aiexperiment_input.items():
     if not is_string(key):
       raise ValidationError("all AIExperiment keys must be strings")
     validated[key] = value
   return validated
 
+
 def validate_aiexperiment_update_input(aiexperiment_input):
   aiexperiment_input = validate_top_level_dict(aiexperiment_input)
   if PROJECT_KEY in aiexperiment_input:
     raise ValidationError(
-      'The project field is not permitted in the AIExperiment.'
-      ' Please set the SIGOPT_PROJECT environment variable instead.'
+      "The project field is not permitted in the AIExperiment."
+      " Please set the SIGOPT_PROJECT environment variable instead."
     )
   aiexperiment_input = dict(aiexperiment_input)
   validated = {}
   try:
     validated["name"] = get_validated_name(aiexperiment_input)
   except KeyError:
     pass
```

### Comparing `sigopt-8.8.0/sigopt/validate/run_input.py` & `sigopt-8.8.1/sigopt/validate/run_input.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
-from sigopt.lib import validate_name, is_string, is_mapping, is_sequence
+from sigopt.lib import is_mapping, is_sequence, is_string, validate_name
 
 from .common import validate_top_level_dict
 from .exceptions import ValidationError
 
 
 def validate_run_input(run_input):
   run_input = validate_top_level_dict(run_input)
```

### Comparing `sigopt-8.8.0/sigopt/xgboost/checkpoint_callback.py` & `sigopt-8.8.1/sigopt/xgboost/checkpoint_callback.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 from .compat import xgboost
 
+
 class SigOptCheckpointCallback(xgboost.callback.TrainingCallback):
   def __init__(self, run, period=1):
     self.run = run
     self.period = period
     self._latest = None
     super().__init__()
 
@@ -17,15 +18,15 @@
     checkpoint_logs = {}
     for dataset, metric_dict in evals_log.items():
       for metric_label, metric_record in metric_dict.items():
         if isinstance(metric_record[-1], tuple):
           chkpt_value = metric_record[-1][0]
         else:
           chkpt_value = metric_record[-1]
-        checkpoint_logs.update({'-'.join((dataset, metric_label)): chkpt_value})
+        checkpoint_logs.update({"-".join((dataset, metric_label)): chkpt_value})
     if (epoch % self.period) == 0 or self.period == 1:
       self.run.log_checkpoint(checkpoint_logs)
       self._latest = None
     else:
       self._latest = checkpoint_logs
 
     return False
```

### Comparing `sigopt-8.8.0/sigopt/xgboost/compat.py` & `sigopt-8.8.1/sigopt/xgboost/compat.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 # pylint: disable=unused-import
 from packaging.version import parse
 
+
 MIN_REQUIRED_XGBOOST_VERSION = "1.3.0"
 
 try:
   import xgboost
   from xgboost import Booster, DMatrix
 except ImportError as ie_xgb:
   raise ImportError(
-    "xgboost needs to be installed in order to use sigopt.xgboost.run functionality. "
-    "Try running `pip install 'sigopt[xgboost]'`."
+    "xgboost needs to be installed in order to use sigopt.xgboost.run"
+    " functionality. Try running `pip install 'sigopt[xgboost]'`."
   ) from ie_xgb
 
 if parse(xgboost.__version__) < parse(MIN_REQUIRED_XGBOOST_VERSION):
   raise ImportError(
-    f"sigopt.xgboost.run is compatible with xgboost>={MIN_REQUIRED_XGBOOST_VERSION}. "
-    f"You have version {xgboost.__version__} installed."
+    "sigopt.xgboost.run is compatible with"
+    f" xgboost>={MIN_REQUIRED_XGBOOST_VERSION}. You have version"
+    f" {xgboost.__version__} installed."
   )
```

### Comparing `sigopt-8.8.0/sigopt/xgboost/compute_metrics.py` & `sigopt-8.8.1/sigopt/xgboost/compute_metrics.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 import numpy
 
 from .compat import Booster
 
+
 def compute_positives_and_negatives(y_true, y_pred, class_label):
   y_true_equals = y_true == class_label
   y_true_notequals = y_true != class_label
   y_pred_equals = y_pred == class_label
   y_pred_notequals = y_pred != class_label
   tp = numpy.count_nonzero(numpy.logical_and(y_true_equals, y_pred_equals))
   tn = numpy.count_nonzero(numpy.logical_and(y_true_notequals, y_pred_notequals))
@@ -21,65 +22,65 @@
   accuracy = numpy.count_nonzero(y_true == y_pred) / len(y_true)
   return accuracy
 
 
 def compute_classification_report(y_true, y_pred):
   classes = numpy.unique(y_true)
   classification_report = {}
-  classification_report['weighted avg'] = {
-    'f1-score': 0,
-    'recall': 0,
-    'precision': 0,
+  classification_report["weighted avg"] = {
+    "f1-score": 0,
+    "recall": 0,
+    "precision": 0,
   }
   for class_label in classes:
     tp, _, fp, fn = compute_positives_and_negatives(y_true, y_pred, class_label)
     precision = tp / (tp + fp) if (tp + fp) != 0 else 0
     recall = tp / (tp + fn) if (tp + fn) != 0 else 0
     f1 = tp / (tp + 0.5 * (fp + fn)) if (tp + 0.5 * (fp + fn)) != 0 else 0
     support = numpy.count_nonzero(y_true == class_label)
     classification_report[str(class_label)] = {
-      'precision': precision,
-      'recall': recall,
-      'f1-score': f1,
-      'support': support,
+      "precision": precision,
+      "recall": recall,
+      "f1-score": f1,
+      "support": support,
     }
-    classification_report['weighted avg']['precision'] += (support / len(y_pred)) * precision
-    classification_report['weighted avg']['recall'] += (support / len(y_pred)) * recall
-    classification_report['weighted avg']['f1-score'] += (support / len(y_pred)) * f1
+    classification_report["weighted avg"]["precision"] += (support / len(y_pred)) * precision
+    classification_report["weighted avg"]["recall"] += (support / len(y_pred)) * recall
+    classification_report["weighted avg"]["f1-score"] += (support / len(y_pred)) * f1
   return classification_report
 
 
 def compute_mae(y_true, y_pred):
   d = y_true - y_pred
   return numpy.mean(abs(d))
 
 
 def compute_mse(y_true, y_pred):
   d = y_true - y_pred
-  return numpy.mean(d ** 2)
+  return numpy.mean(d**2)
 
 
 def compute_classification_metrics(model, D_matrix_pair):
   assert isinstance(model, Booster)
   D_matrix, D_name = D_matrix_pair
   preds = model.predict(D_matrix)
   # Check shape of preds
   if len(preds.shape) == 2:
     preds = numpy.argmax(preds, axis=1)
   else:
     preds = numpy.round(preds)
   y_test = D_matrix.get_label()
   accuracy = compute_accuracy(y_test, preds)
   rep = compute_classification_report(y_test, preds)
-  other_metrics = rep['weighted avg']
+  other_metrics = rep["weighted avg"]
   return {
-    f"{D_name}-accuracy" : accuracy,
-    f"{D_name}-F1" : other_metrics['f1-score'],
-    f"{D_name}-recall": other_metrics['recall'],
-    f"{D_name}-precision": other_metrics['precision'],
+    f"{D_name}-accuracy": accuracy,
+    f"{D_name}-F1": other_metrics["f1-score"],
+    f"{D_name}-recall": other_metrics["recall"],
+    f"{D_name}-precision": other_metrics["precision"],
   }
 
 
 def compute_regression_metrics(model, D_matrix_pair):
   assert isinstance(model, Booster)
   D_matrix, D_name = D_matrix_pair
   preds = model.predict(D_matrix)
```

### Comparing `sigopt-8.8.0/sigopt/xgboost/experiment.py` & `sigopt-8.8.1/sigopt/xgboost/experiment.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,26 +19,37 @@
   SIGOPT_DEFAULTS_SOURCE_PRIORITY,
   SUPPORTED_AUTOBOUND_PARAMS,
   SUPPORTED_METRICS_TO_OPTIMIZE,
 )
 from .run import parse_run_options
 from .run import run as XGBRunWrapper
 
-XGB_EXPERIMENT_KEYWORD = '_IS_XGB_EXPERIMENT'
+
+XGB_EXPERIMENT_KEYWORD = "_IS_XGB_EXPERIMENT"
+
 
 # Sentinel value to distinguish between default early_stopping_rounds and input early_stopping_rounds w/ default value
 class DefaultEarlyStoppingRounds:
   pass
 
 
 _default_early_stopping_rounds = DefaultEarlyStoppingRounds()
 
 
 class XGBExperiment:
-  def __init__(self, experiment_config, dtrain, evals, params, num_boost_round, early_stopping_rounds, run_options):
+  def __init__(
+    self,
+    experiment_config,
+    dtrain,
+    evals,
+    params,
+    num_boost_round,
+    early_stopping_rounds,
+    run_options,
+  ):
     self.experiment_config_parsed = copy.deepcopy(experiment_config)
     self.dtrain = dtrain
     self.evals = evals
     self.params = params
     self.num_boost_round = num_boost_round
     self.run_options = run_options
     if early_stopping_rounds == _default_early_stopping_rounds:
@@ -46,159 +57,164 @@
       self.early_stopping_round_used_sigopt_default = True
     else:
       self.early_stopping_rounds = early_stopping_rounds  # if None, deactivate early stopping
       self.early_stopping_round_used_sigopt_default = False
     self.sigopt_experiment = None
 
   def parse_and_create_metrics(self):
-    if 'metrics' in self.experiment_config_parsed and isinstance(self.experiment_config_parsed['metrics'], list):
-      for metric in self.experiment_config_parsed['metrics']:
-        if metric['strategy'] == 'optimize' and metric['name'] not in SUPPORTED_METRICS_TO_OPTIMIZE:
-          raise ValueError(
-            f"The chosen metric to optimize, {metric['name']}, is not supported."
-          )
+    if "metrics" in self.experiment_config_parsed and isinstance(self.experiment_config_parsed["metrics"], list):
+      for metric in self.experiment_config_parsed["metrics"]:
+        if metric["strategy"] == "optimize" and metric["name"] not in SUPPORTED_METRICS_TO_OPTIMIZE:
+          raise ValueError(f"The chosen metric to optimize, {metric['name']}, is not supported.")
 
     else:
-      if 'metrics' not in self.experiment_config_parsed:  # pick a default metric
-        if 'objective' in self.params:
-          objective = self.params['objective']
-          if objective.split(':')[0] in ['binary', 'multi']:
+      if "metrics" not in self.experiment_config_parsed:  # pick a default metric
+        if "objective" in self.params:
+          objective = self.params["objective"]
+          if objective.split(":")[0] in ["binary", "multi"]:
             metric_to_optimize = DEFAULT_CLASSIFICATION_METRIC
           else:
             metric_to_optimize = DEFAULT_REGRESSION_METRIC  # do regression if anything else (including ranking)
         else:
           metric_to_optimize = DEFAULT_REGRESSION_METRIC
       else:
-        if self.experiment_config_parsed['metrics'] not in SUPPORTED_METRICS_TO_OPTIMIZE:
+        if self.experiment_config_parsed["metrics"] not in SUPPORTED_METRICS_TO_OPTIMIZE:
           raise ValueError(
             f"The chosen metric to optimize, {self.experiment_config_parsed['metrics']}, is not supported."
           )
-        metric_to_optimize = self.experiment_config_parsed['metrics']
+        metric_to_optimize = self.experiment_config_parsed["metrics"]
 
       optimization_strategy = METRICS_OPTIMIZATION_STRATEGY[metric_to_optimize]
-      self.experiment_config_parsed['metrics'] = [{
-        'name': metric_to_optimize,
-        'strategy': 'optimize',
-        'objective': optimization_strategy
-      }]
+      self.experiment_config_parsed["metrics"] = [
+        {
+          "name": metric_to_optimize,
+          "strategy": "optimize",
+          "objective": optimization_strategy,
+        }
+      ]
 
     # change optimized metric to reflect updated name
-    for metric in self.experiment_config_parsed['metrics']:
-      if metric['strategy'] == 'optimize':
+    for metric in self.experiment_config_parsed["metrics"]:
+      if metric["strategy"] == "optimize":
         if isinstance(self.evals, list):
-          metric['name'] = self.evals[0][1] + '-' + metric['name']  # optimize metric on first eval set by default
+          metric["name"] = self.evals[0][1] + "-" + metric["name"]  # optimize metric on first eval set by default
         else:
-          metric['name'] = DEFAULT_EVALS_NAME + '-' + metric['name']
+          metric["name"] = DEFAULT_EVALS_NAME + "-" + metric["name"]
 
   def check_and_fill_parameter_types(self):
-    params_to_check = [p for p in self.experiment_config_parsed['parameters'] if p['name'] in PARAMETER_INFORMATION]
+    params_to_check = [p for p in self.experiment_config_parsed["parameters"] if p["name"] in PARAMETER_INFORMATION]
     for parameter in params_to_check:
-      parameter_name = parameter['name']
-      proper_parameter_type = PARAMETER_INFORMATION[parameter_name]['type']
-      if 'type' in parameter:
-        experiment_config_parameter_type = parameter['type']
+      parameter_name = parameter["name"]
+      proper_parameter_type = PARAMETER_INFORMATION[parameter_name]["type"]
+      if "type" in parameter:
+        experiment_config_parameter_type = parameter["type"]
         if experiment_config_parameter_type != proper_parameter_type:
           raise ValueError(
-            f'Parameter {parameter_name} type listed incorrectly as {experiment_config_parameter_type} '
-            f'in experiment config, and should be listed as having type {proper_parameter_type}.'
+            f"Parameter {parameter_name} type listed incorrectly as"
+            f" {experiment_config_parameter_type} in experiment config, and"
+            f" should be listed as having type {proper_parameter_type}."
           )
       else:
-        parameter['type'] = proper_parameter_type
+        parameter["type"] = proper_parameter_type
 
   def check_and_fill_parameter_bounds(self):
-    params_to_check = [p for p in self.experiment_config_parsed['parameters'] if p['name'] in PARAMETER_INFORMATION]
+    params_to_check = [p for p in self.experiment_config_parsed["parameters"] if p["name"] in PARAMETER_INFORMATION]
     for parameter in params_to_check:
-      parameter_name = parameter['name']
-      if 'bounds' not in parameter and PARAMETER_INFORMATION[parameter_name]['type'] in ['double', 'int']:
+      parameter_name = parameter["name"]
+      if "bounds" not in parameter and PARAMETER_INFORMATION[parameter_name]["type"] in ["double", "int"]:
         if parameter_name not in SUPPORTED_AUTOBOUND_PARAMS:
-          raise ValueError(f'We do not support autoselection of bounds for {parameter_name}.')
+          raise ValueError(f"We do not support autoselection of bounds for {parameter_name}.")
         param_info = PARAMETER_INFORMATION[parameter_name]
-        transformation = param_info['transformation'] if 'transformation' in param_info else None
+        transformation = param_info["transformation"] if "transformation" in param_info else None
         parameter.update(
           dict(
             name=parameter_name,
-            type=param_info['type'],
-            bounds=param_info['bounds'],
-            transformation=transformation
+            type=param_info["type"],
+            bounds=param_info["bounds"],
+            transformation=transformation,
           )
         )
       else:
-        if parameter['type'] == 'categorical':
-          if 'categorical_values' not in parameter:
-            raise ValueError(f'We do not support autoselection of categorical_values for {parameter_name}.')
+        if parameter["type"] == "categorical":
+          if "categorical_values" not in parameter:
+            raise ValueError(f"We do not support autoselection of categorical_values for {parameter_name}.")
 
-          proper_parameter_values = PARAMETER_INFORMATION[parameter_name]['values']
-          config_parameter_values = parameter['categorical_values']
+          proper_parameter_values = PARAMETER_INFORMATION[parameter_name]["values"]
+          config_parameter_values = parameter["categorical_values"]
           if not set(proper_parameter_values) > set(config_parameter_values):
             raise ValueError(
-              f'The set of possible categorical values {config_parameter_values} is not a subset of '
-              f'the permissible categorical values {proper_parameter_values}.'
+              "The set of possible categorical values"
+              f" {config_parameter_values} is not a subset of the"
+              " permissible categorical values"
+              f" {proper_parameter_values}."
             )
 
         else:
           pass  # TODO: check bounds for double, int, and grid parameters in later PR
 
   def parse_and_create_parameters(self):
-    if 'parameters' not in self.experiment_config_parsed:
+    if "parameters" not in self.experiment_config_parsed:
       default_search_space = []
       for parameter_name in DEFAULT_SEARCH_PARAMS:
         param_info = PARAMETER_INFORMATION[parameter_name]
-        transformation = param_info['transformation'] if 'transformation' in param_info else None
+        transformation = param_info["transformation"] if "transformation" in param_info else None
         default_search_space.append(
           dict(
             name=parameter_name,
-            type=param_info['type'],
-            bounds=param_info['bounds'],
-            transformation=transformation
+            type=param_info["type"],
+            bounds=param_info["bounds"],
+            transformation=transformation,
           )
         )
-      self.experiment_config_parsed['parameters'] = default_search_space
+      self.experiment_config_parsed["parameters"] = default_search_space
     else:
       self.check_and_fill_parameter_types()
       self.check_and_fill_parameter_bounds()
 
     # Check key overlap between parameters to be optimized and parameters that are set
-    params_optimized = [param['name'] for param in self.experiment_config_parsed['parameters']]
+    params_optimized = [param["name"] for param in self.experiment_config_parsed["parameters"]]
     params_overlap = set(params_optimized) & set(self.params.keys())
     if len(params_overlap) != 0:
       raise ValueError(
-        f'There is overlap between tuned parameters and user-set parameters: {params_overlap}.'
-        'Parameter names cannot be defined in both locations'
+        "There is overlap between tuned parameters and user-set parameters:"
+        f" {params_overlap}.Parameter names cannot be defined in both locations"
       )
 
     # Check that num_boost_round is not set by both sigopt experiment and user
-    if self.num_boost_round and 'num_boost_round' in params_optimized:
+    if self.num_boost_round and "num_boost_round" in params_optimized:
       raise ValueError(
-        'num_boost_round has been denoted as an optimization parameter, but also has been fixed in the input arguments'
-        f'to have value {self.num_boost_round}. Please remove it from either the search space or the input arguments.'
+        "num_boost_round has been denoted as an optimization parameter, but"
+        " also has been fixed in the input argumentsto have value"
+        f" {self.num_boost_round}. Please remove it from either the search"
+        " space or the input arguments."
       )
 
   def parse_and_create_aiexperiment(self):
     self.parse_and_create_metrics()
     self.parse_and_create_parameters()
-    if 'budget' not in self.experiment_config_parsed:
-      chosen_budget = DEFAULT_ITERS_PER_DIM * len(self.experiment_config_parsed['parameters'])
-      self.experiment_config_parsed['budget'] = min(chosen_budget, MAX_BO_ITERATIONS)
-    if 'parallel_bandwidth' not in self.experiment_config_parsed:
-      self.experiment_config_parsed['parallel_bandwidth'] = 1
-    if 'type' not in self.experiment_config_parsed:
-      self.experiment_config_parsed['type'] = 'offline'
-    self.experiment_config_parsed['metadata'] = {XGB_EXPERIMENT_KEYWORD: 'True'}
+    if "budget" not in self.experiment_config_parsed:
+      chosen_budget = DEFAULT_ITERS_PER_DIM * len(self.experiment_config_parsed["parameters"])
+      self.experiment_config_parsed["budget"] = min(chosen_budget, MAX_BO_ITERATIONS)
+    if "parallel_bandwidth" not in self.experiment_config_parsed:
+      self.experiment_config_parsed["parallel_bandwidth"] = 1
+    if "type" not in self.experiment_config_parsed:
+      self.experiment_config_parsed["type"] = "offline"
+    self.experiment_config_parsed["metadata"] = {XGB_EXPERIMENT_KEYWORD: "True"}
     self.sigopt_experiment = create_aiexperiment(**self.experiment_config_parsed)
 
   def run_experiment(self):
     for run in self.sigopt_experiment.loop():
       with run:
         if self.num_boost_round:
           num_boost_round_run = self.num_boost_round
-        elif 'num_boost_round' in run.params:
-          num_boost_round_run = run.params['num_boost_round']
+        elif "num_boost_round" in run.params:
+          num_boost_round_run = run.params["num_boost_round"]
         else:
           num_boost_round_run = DEFAULT_NUM_BOOST_ROUND
-        self.run_options['run'] = run
+        self.run_options["run"] = run
 
         XGBRunWrapper(
           self.params,
           self.dtrain,
           num_boost_round=num_boost_round_run,
           evals=self.evals,
           early_stopping_rounds=self.early_stopping_rounds,
@@ -210,18 +226,19 @@
         if self.early_stopping_round_used_sigopt_default:
           run.set_parameters_sources_meta(
             SIGOPT_DEFAULTS_SOURCE_NAME,
             sort=SIGOPT_DEFAULTS_SOURCE_PRIORITY,
             default_show=True,
           )
           run.set_parameters_source(
-            {'early_stopping_rounds': DEFAULT_EARLY_STOPPING_ROUNDS},
+            {"early_stopping_rounds": DEFAULT_EARLY_STOPPING_ROUNDS},
             SIGOPT_DEFAULTS_SOURCE_NAME,
           )
 
+
 def experiment(
   experiment_config,
   dtrain,
   evals,
   params,
   num_boost_round=None,
   early_stopping_rounds=_default_early_stopping_rounds,
```

### Comparing `sigopt-8.8.0/sigopt/xgboost/run.py` & `sigopt-8.8.1/sigopt/xgboost/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 import copy
-from inspect import signature
-import math
 import json
+import math
 import platform
 import time
 import warnings
+from inspect import signature
 
 from .. import create_run
 from ..log_capture import SystemOutputStreamMonitor
 from ..model_aware_run import ModelAwareRun
 from ..run_context import RunContext
 from .checkpoint_callback import SigOptCheckpointCallback
 from .compat import Booster, DMatrix, xgboost
@@ -23,77 +23,67 @@
   XGBOOST_DEFAULTS_SOURCE_NAME,
   XGBOOST_DEFAULTS_SOURCE_PRIORITY,
 )
 from .utils import get_booster_params
 
 
 DEFAULT_RUN_OPTIONS = {
-  'autolog_checkpoints': True,
-  'autolog_feature_importances': True,
-  'autolog_metrics': True,
-  'autolog_stdout': True,
-  'autolog_stderr': True,
-  'autolog_sys_info': True,
-  'autolog_xgboost_defaults': True,
-  'name': None,
-  'run': None,
+  "autolog_checkpoints": True,
+  "autolog_feature_importances": True,
+  "autolog_metrics": True,
+  "autolog_stdout": True,
+  "autolog_stderr": True,
+  "autolog_sys_info": True,
+  "autolog_xgboost_defaults": True,
+  "name": None,
+  "run": None,
 }
 DEFAULT_CHECKPOINT_PERIOD = 5
 MAX_NUM_CHECKPOINTS = 200
 FEATURE_IMPORTANCES_MAX_NUM_FEATURE = 50
 FEATURE_IMPORTANCES_MAX_KEY_CHARS = 100
-XGB_INTEGRATION_KEYWORD = '_IS_XGB_RUN'
+XGB_INTEGRATION_KEYWORD = "_IS_XGB_RUN"
 
 PARAMS_LOGGED_AS_METADATA = [
-  'eval_metric',
-  'interaction_constraints',
-  'monotone_constraints',
-  'num_class',
-  'objective',
-  'updater',
+  "eval_metric",
+  "interaction_constraints",
+  "monotone_constraints",
+  "num_class",
+  "objective",
+  "updater",
 ]
 SUPPORTED_OBJECTIVE_PREFIXES = [
-  'binary',
-  'multi',
-  'reg',
+  "binary",
+  "multi",
+  "reg",
 ]
 DOC_URL = "https://docs.sigopt.com/ai-module-api-references/xgboost/xgboost_run"
 
 
 def parse_run_options(run_options):
   if run_options is None:
     return copy.deepcopy(DEFAULT_RUN_OPTIONS)
 
   if not isinstance(run_options, dict):
-    raise TypeError(
-      f"run_options should be a dictionary. Refer to the sigopt.xgboost.run documentation {DOC_URL}"
-    )
+    raise TypeError(f"run_options should be a dictionary. Refer to the sigopt.xgboost.run documentation {DOC_URL}")
 
   if run_options.keys() - DEFAULT_RUN_OPTIONS.keys():
-    raise ValueError(
-      f"Unsupported keys {run_options.keys() - DEFAULT_RUN_OPTIONS.keys()} in run_options."
-    )
+    raise ValueError(f"Unsupported keys {run_options.keys() - DEFAULT_RUN_OPTIONS.keys()} in run_options.")
 
   for key, value in run_options.items():
     if key.startswith("autolog") and not isinstance(value, bool):
-      raise TypeError(
-        f"run_options key `{key}` expects a Boolean value, not {type(value)}."
-      )
+      raise TypeError(f"run_options key `{key}` expects a Boolean value, not {type(value)}.")
 
-  if {'run', 'name'}.issubset(run_options.keys()):
-    if run_options['run'] and run_options['name']:
-      raise ValueError(
-        "Cannot specify both `run` and `name` keys inside run_options."
-      )
-
-  if 'run' in run_options.keys() and run_options['run'] is not None:
-    if not isinstance(run_options['run'], RunContext):
-      raise TypeError(
-        f"`run` must be an instance of RunContext object, not {type(run_options['run']).__name__}."
-      )
+  if {"run", "name"}.issubset(run_options.keys()):
+    if run_options["run"] and run_options["name"]:
+      raise ValueError("Cannot specify both `run` and `name` keys inside run_options.")
+
+  if "run" in run_options.keys() and run_options["run"] is not None:
+    if not isinstance(run_options["run"], RunContext):
+      raise TypeError(f"`run` must be an instance of RunContext object, not {type(run_options['run']).__name__}.")
 
   return {**DEFAULT_RUN_OPTIONS, **run_options}
 
 
 def validate_xgboost_kwargs(xgb_kwargs):
   if not xgb_kwargs:
     return
@@ -108,16 +98,16 @@
 
 
 class XGBRun(ModelAwareRun):
   def __init__(self, run, model):
     assert isinstance(model, Booster)
     super().__init__(run, model)
 
-class XGBRunHandler:
 
+class XGBRunHandler:
   def __init__(
     self,
     params,
     dtrain,
     num_boost_round,
     evals,
     early_stopping_rounds,
@@ -141,15 +131,15 @@
     self.model = xgb_model
     self.is_regression = None
     self.kwargs = kwargs
     validate_xgboost_kwargs(self.kwargs)
 
   def form_callbacks(self):
     # if no validation set, checkpointing not possible
-    if not (self.run_options_parsed['autolog_checkpoints'] and self.validation_sets):
+    if not (self.run_options_parsed["autolog_checkpoints"] and self.validation_sets):
       return
 
     if self.callbacks is None:
       self.callbacks = []
     period = DEFAULT_CHECKPOINT_PERIOD
     if self.callbacks:
       for cb in self.callbacks:
@@ -158,25 +148,25 @@
     if self.verbose_eval:
       period = 1 if self.verbose_eval is True else self.verbose_eval
     period = max(period, math.ceil((self.num_boost_round + 1) / MAX_NUM_CHECKPOINTS))
     sigopt_checkpoint_callback = SigOptCheckpointCallback(self.run, period=period)
     self.callbacks.append(sigopt_checkpoint_callback)
 
   def make_run(self):
-    if self.run_options_parsed['run'] is not None:
-      self.run = self.run_options_parsed['run']
-    elif self.run_options_parsed['name'] is not None:
-      self.run = create_run(name=self.run_options_parsed['name'])
+    if self.run_options_parsed["run"] is not None:
+      self.run = self.run_options_parsed["run"]
+    elif self.run_options_parsed["name"] is not None:
+      self.run = create_run(name=self.run_options_parsed["name"])
     else:
       self.run = create_run()
 
   def log_metadata(self):
     self.run.log_dev_metadata(XGB_INTEGRATION_KEYWORD, True)
 
-    if self.run_options_parsed['autolog_sys_info']:
+    if self.run_options_parsed["autolog_sys_info"]:
       python_version = platform.python_version()
       self.run.log_metadata("Python Version", python_version)
       self.run.log_metadata("XGBoost Version", xgboost.__version__)
     self.run.log_model("XGBoost")
     self.run.log_metadata("Dataset columns", self.dtrain.num_col())
     self.run.log_metadata("Dataset rows", self.dtrain.num_row())
     for name in PARAMS_LOGGED_AS_METADATA:
@@ -193,140 +183,139 @@
 
   def log_params(self):
     self.run.set_parameters_sources_meta(USER_SOURCE_NAME, sort=USER_SOURCE_PRIORITY, default_show=True)
     for p_name, p_value in self.params.items():
       if p_name not in self.run.params and p_name not in PARAMS_LOGGED_AS_METADATA:
         self._log_param_by_source(p_name, p_value, USER_SOURCE_NAME)
 
-    if 'num_boost_round' not in self.run.params.keys():
-      self._log_param_by_source('num_boost_round', self.num_boost_round, USER_SOURCE_NAME)
+    if "num_boost_round" not in self.run.params.keys():
+      self._log_param_by_source("num_boost_round", self.num_boost_round, USER_SOURCE_NAME)
 
-    if self.early_stopping_rounds is not None and 'early_stopping_rounds' not in self.run.params.keys():
-      self._log_param_by_source('early_stopping_rounds', self.early_stopping_rounds, USER_SOURCE_NAME)
+    if self.early_stopping_rounds is not None and "early_stopping_rounds" not in self.run.params.keys():
+      self._log_param_by_source("early_stopping_rounds", self.early_stopping_rounds, USER_SOURCE_NAME)
 
-    if self.run_options_parsed['autolog_xgboost_defaults']:
+    if self.run_options_parsed["autolog_xgboost_defaults"]:
       self.log_default_params()
 
   def log_default_params(self):
     all_xgb_params = get_booster_params(self.model)
     reported_params = self.run.params.keys()
 
     xgb_default_params = {}
     self.run.set_parameters_sources_meta(
       XGBOOST_DEFAULTS_SOURCE_NAME,
       sort=XGBOOST_DEFAULTS_SOURCE_PRIORITY,
-      default_show=False
+      default_show=False,
     )
     for p_name, p_value in all_xgb_params.items():
       if p_name not in reported_params and p_name not in PARAMS_LOGGED_AS_METADATA:
         if p_value is not None:
           xgb_default_params.update({p_name: p_value})
     self.run.set_parameters(xgb_default_params)
     self.run.set_parameters_source(xgb_default_params, XGBOOST_DEFAULTS_SOURCE_NAME)
 
   def check_learning_task(self):
     config = self.model.save_config()
     config_dict = json.loads(config)
-    objective = config_dict['learner']['objective']['name']
+    objective = config_dict["learner"]["objective"]["name"]
     # NOTE: do not log metrics if learning task isn't regression or classification
-    if not any(s in config_dict['learner']['objective']['name'] for s in SUPPORTED_OBJECTIVE_PREFIXES):
-      self.run_options_parsed['autolog_metrics'] = False
-    if objective.split(':')[0] == 'reg':
+    if not any(s in config_dict["learner"]["objective"]["name"] for s in SUPPORTED_OBJECTIVE_PREFIXES):
+      self.run_options_parsed["autolog_metrics"] = False
+    if objective.split(":")[0] == "reg":
       self.is_regression = True
     else:
       self.is_regression = False
 
-  def log_feature_importances(self, importance_type='weight', fmap=''):
+  def log_feature_importances(self, importance_type="weight", fmap=""):
     scores = self.model.get_score(importance_type=importance_type, fmap=fmap)
     # NOTE: do not log importances if there is no split at all.
     if not scores:
       return
     scores = dict(
-      sorted(scores.items(), key=lambda x:(x[1], x[0]), reverse=True)[:FEATURE_IMPORTANCES_MAX_NUM_FEATURE]
+      sorted(scores.items(), key=lambda x: (x[1], x[0]), reverse=True)[:FEATURE_IMPORTANCES_MAX_NUM_FEATURE]
     )
 
     if any(len(k) > FEATURE_IMPORTANCES_MAX_KEY_CHARS for k in scores.keys()):
       warnings.warn(
-        f"Some of the feature names have more than {FEATURE_IMPORTANCES_MAX_KEY_CHARS} characters,"
-        " skipping logging feature importances.",
+        (
+          "Some of the feature names have more than"
+          f" {FEATURE_IMPORTANCES_MAX_KEY_CHARS} characters, skipping logging"
+          " feature importances."
+        ),
         RuntimeWarning,
       )
       return
 
     fp = {
-      'type': importance_type,
-      'scores': scores,
+      "type": importance_type,
+      "scores": scores,
     }
-    self.run.log_sys_metadata('feature_importances', fp)
+    self.run.log_sys_metadata("feature_importances", fp)
 
   def train_xgb(self):
     stream_monitor = SystemOutputStreamMonitor()
     with stream_monitor:
       params = copy.deepcopy(self.params)
       if self.run.params:
         params.update(self.run.params)
-        if 'num_boost_round' in params:
-          self.num_boost_round = params.pop('num_boost_round')
-        if 'early_stopping_rounds' in params:
-          self.early_stopping_rounds = params.pop('early_stopping_rounds')
+        if "num_boost_round" in params:
+          self.num_boost_round = params.pop("num_boost_round")
+        if "early_stopping_rounds" in params:
+          self.early_stopping_rounds = params.pop("early_stopping_rounds")
       xgb_args = {
-        'params': params,
-        'dtrain': self.dtrain,
-        'num_boost_round': self.num_boost_round,
-        'early_stopping_rounds': self.early_stopping_rounds,
-        'verbose_eval': self.verbose_eval,
-        'xgb_model': self.model,
-        'callbacks': self.callbacks,
+        "params": params,
+        "dtrain": self.dtrain,
+        "num_boost_round": self.num_boost_round,
+        "early_stopping_rounds": self.early_stopping_rounds,
+        "verbose_eval": self.verbose_eval,
+        "xgb_model": self.model,
+        "callbacks": self.callbacks,
       }
       if self.kwargs:
         xgb_args.update(self.kwargs)
       if self.validation_sets is not None:
         self.evals_result = {} if self.evals_result is None else self.evals_result
-        xgb_args['evals'] = self.validation_sets
-        xgb_args['evals_result'] = self.evals_result
+        xgb_args["evals"] = self.validation_sets
+        xgb_args["evals_result"] = self.evals_result
       t_start = time.time()
       bst = xgboost.train(**xgb_args)
       t_train = time.time() - t_start
-      if self.run_options_parsed['autolog_metrics']:
+      if self.run_options_parsed["autolog_metrics"]:
         self.run.log_metric("Training time", t_train)
-        self.run.log_metric('best_iteration', bst.best_iteration)
+        self.run.log_metric("best_iteration", bst.best_iteration)
 
     stream_data = stream_monitor.get_stream_data()
     if stream_data:
       stdout, stderr = stream_data
       log_dict = {}
-      if self.run_options_parsed['autolog_stdout']:
+      if self.run_options_parsed["autolog_stdout"]:
         log_dict["stdout"] = stdout
-      if self.run_options_parsed['autolog_stderr']:
+      if self.run_options_parsed["autolog_stderr"]:
         log_dict["stderr"] = stderr
       self.run.set_logs(log_dict)
     self.model = bst
 
   def log_validation_metrics(self):
     # Always log xgb-default eval_metric
     n_eval_rounds = 0
     if self.evals_result is not None:
       for dataset, metric_dict in self.evals_result.items():
         for metric_label, metric_record in metric_dict.items():
           self.run.log_metric(f"{dataset}-{metric_label}", metric_record[-1])
           n_eval_rounds = len(metric_record)
 
       if self.early_stopping_rounds:
-        self.run.log_metric('num_boost_round_before_stopping', n_eval_rounds)
+        self.run.log_metric("num_boost_round_before_stopping", n_eval_rounds)
 
     if self.run_options_parsed["autolog_metrics"] and self.validation_sets:
       for validation_set in self.validation_sets:
         if self.is_regression:
-          self.run.log_metrics(
-            compute_regression_metrics(self.model, (validation_set))
-          )
+          self.run.log_metrics(compute_regression_metrics(self.model, (validation_set)))
         else:
-          self.run.log_metrics(
-            compute_classification_metrics(self.model, (validation_set))
-          )
+          self.run.log_metrics(compute_classification_metrics(self.model, (validation_set)))
 
 
 def run(
   params,
   dtrain,
   num_boost_round=10,
   evals=None,
@@ -335,24 +324,22 @@
   verbose_eval=True,
   callbacks=None,
   xgb_model=None,
   run_options=None,
   **kwargs,
 ):
   """
-  Sigopt integration for XGBoost mirrors the standard xgboost.train interface for the most part, with the option
-  for additional arguments. Unlike the usual train interface, sigopt.xgboost.run() returns a XGBRun object,
-  where XGBRun.run and XGBRun.model are the resulting RunContext and XGBoost model, respectively.
-  """
+    Sigopt integration for XGBoost mirrors the standard xgboost.train interface for the most part, with the option
+    for additional arguments. Unlike the usual train interface, sigopt.xgboost.run() returns a XGBRun object,
+    where XGBRun.run and XGBRun.model are the resulting RunContext and XGBoost model, respectively.
+    """
   if evals is not None:
     if not isinstance(evals, (DMatrix, list)):
-      dmatrix_module_name = '.'.join((DMatrix.__module__, DMatrix.__name__))
-      raise TypeError(
-        f"`evals` must be a {dmatrix_module_name} object or list of ({dmatrix_module_name}, str) tuples."
-      )
+      dmatrix_module_name = ".".join((DMatrix.__module__, DMatrix.__name__))
+      raise TypeError(f"`evals` must be a {dmatrix_module_name} object or list of ({dmatrix_module_name}, str) tuples.")
 
   _run = XGBRunHandler(
     params=params,
     dtrain=dtrain,
     num_boost_round=num_boost_round,
     evals=evals,
     early_stopping_rounds=early_stopping_rounds,
@@ -367,10 +354,10 @@
   _run.make_run()
   _run.form_callbacks()
   _run.train_xgb()
   _run.log_metadata()
   _run.log_params()
   _run.check_learning_task()
   _run.log_validation_metrics()
-  if _run.run_options_parsed['autolog_feature_importances']:
+  if _run.run_options_parsed["autolog_feature_importances"]:
     _run.log_feature_importances()
   return XGBRun(_run.run, _run.model)
```

### Comparing `sigopt-8.8.0/sigopt/xgboost/utils.py` & `sigopt-8.8.1/sigopt/xgboost/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,15 +22,15 @@
   assert isinstance(booster, Booster)
   config = json.loads(booster.save_config())
   stack = [config]
   all_xgboost_params = {}
   while stack:
     obj = stack.pop()
     for k, v in obj.items():
-      if k.endswith('_param'):
+      if k.endswith("_param"):
         for p_k, p_v in v.items():
           all_xgboost_params[p_k] = p_v
       elif isinstance(v, dict):
         stack.append(v)
 
   params = {}
   for k, v in all_xgboost_params.items():
```

### Comparing `sigopt-8.8.0/sigopt.egg-info/PKG-INFO` & `sigopt-8.8.1/sigopt.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigopt
-Version: 8.8.0
+Version: 8.8.1
 Summary: SigOpt Python API Client
 Home-page: https://sigopt.com/
 Author: SigOpt
 Author-email: support@sigopt.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sigopt-8.8.0/sigopt.egg-info/SOURCES.txt` & `sigopt-8.8.1/sigopt.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
+setup.cfg
 setup.py
 integration_test/__init__.py
 integration_test/test_experiment.py
 integration_test/test_hyperopt.py
 integration_test/test_sigopt.py
 integration_test/test_xgboost_experiment.py
 integration_test/test_xgboost_run.py
```

### Comparing `sigopt-8.8.0/sigopt.egg-info/requires.txt` & `sigopt-8.8.1/sigopt.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,42 @@
-GitPython>=2.0.0
-PyYAML<6.0.0,>=5.4.1
 backoff<2.0.0,>=1.10.0
+certifi==2022.12.7
 click>=8.0.0
+GitPython>=2.0.0
 packaging>=21.3
 pypng>=0.0.20
+PyYAML<7,>=5
 requests<3.0.0,>=2.25.0
 urllib3<2.0.0,>=1.26.5
 
 [dev]
-Pillow
-flake8==3.8.4
 matplotlib>=3.3.4
 mock>=3.0.5
 nose==1.3.7
 notebook
 numpy<2.0.0,>=1.15.0
+Pillow
+pre-commit<3,>=2.5.2
 pylint==2.9.6
 pymongo==3.12.3
 pyspark
 pytest==7.2.1
+scikit-learn>=0.23.2
 setuptools>=47.3.1
 twine<4.0.0,>=3.2.0
-scikit-learn>=0.23.2
-vulture==2.3.0
+vulture==2.7
+Pint<0.17.0,>=0.16.0
+boto3<2.0.0,>=1.16.34
+docker<5.0.0,>=4.4.0
+kubernetes<13.0.0,>=12.0.1
+pyOpenSSL>=20.0.0
 xgboost>=1.3.1
 numpy>=1.15.0
 hyperopt>=0.2.7
+sigoptlite>=0.1.1
 
 [hyperopt]
 hyperopt>=0.2.7
 
 [lite]
 sigoptlite>=0.1.1
```

### Comparing `sigopt-8.8.0/test/cli/test_cli_config.py` & `sigopt-8.8.1/test/cli/test_cli_config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
-import click
 import mock
 import pytest
 from click.testing import CliRunner
 
 from sigopt.cli import cli
 
 
 class TestRunCli(object):
-  @pytest.mark.parametrize('opt_into_log_collection', [False, True])
-  @pytest.mark.parametrize('opt_into_cell_tracking', [False, True])
+  @pytest.mark.parametrize("opt_into_log_collection", [False, True])
+  @pytest.mark.parametrize("opt_into_cell_tracking", [False, True])
   def test_config_command(self, opt_into_log_collection, opt_into_cell_tracking):
     runner = CliRunner()
-    log_collection_arg = '--enable-log-collection' if opt_into_log_collection else '--no-enable-log-collection'
-    cell_tracking_arg = '--enable-cell-tracking' if opt_into_cell_tracking else '--no-enable-cell-tracking'
-    with mock.patch('sigopt.cli.commands.config._config.persist_configuration_options') as persist_configuration_options:
-      result = runner.invoke(cli, [
-        'config',
-        '--api-token=some_test_token',
-        log_collection_arg,
-        cell_tracking_arg,
-      ])
-      persist_configuration_options.assert_called_once_with({
-        'api_token': 'some_test_token',
-        'code_tracking_enabled': opt_into_cell_tracking,
-        'log_collection_enabled': opt_into_log_collection,
-      })
+    log_collection_arg = "--enable-log-collection" if opt_into_log_collection else "--no-enable-log-collection"
+    cell_tracking_arg = "--enable-cell-tracking" if opt_into_cell_tracking else "--no-enable-cell-tracking"
+    with mock.patch(
+      "sigopt.cli.commands.config._config.persist_configuration_options"
+    ) as persist_configuration_options:
+      result = runner.invoke(
+        cli,
+        [
+          "config",
+          "--api-token=some_test_token",
+          log_collection_arg,
+          cell_tracking_arg,
+        ],
+      )
+      persist_configuration_options.assert_called_once_with(
+        {
+          "api_token": "some_test_token",
+          "code_tracking_enabled": opt_into_cell_tracking,
+          "log_collection_enabled": opt_into_log_collection,
+        }
+      )
     assert result.exit_code == 0
-    assert result.output == ''
+    assert result.output == ""
```

### Comparing `sigopt-8.8.0/test/cli/test_cluster_connect.py` & `sigopt-8.8.1/test/cli/test_cluster_connect.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,10 +7,10 @@
 from sigopt.cli import cli
 
 
 class TestClusterConnectCli(object):
   def test_cluster_connect_command(self):
     services = Mock()
     runner = CliRunner()
-    with patch('sigopt.orchestrate.controller.OrchestrateServiceBag', return_value=services):
+    with patch("sigopt.orchestrate.controller.OrchestrateServiceBag", return_value=services):
       result = runner.invoke(cli, ["cluster", "connect", "-n", "foobar", "--provider", "custom"])
     assert result.exit_code == 0
```

### Comparing `sigopt-8.8.0/test/cli/test_cluster_create.py` & `sigopt-8.8.1/test/cli/test_cluster_create.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,13 +7,13 @@
 from sigopt.cli import cli
 
 
 class TestClusterCreateCli(object):
   def test_cluster_create(self):
     services = Mock()
     runner = CliRunner()
-    with \
-      runner.isolated_filesystem(), \
-      patch('sigopt.orchestrate.controller.OrchestrateServiceBag', return_value=services):
+    with runner.isolated_filesystem(), patch(
+      "sigopt.orchestrate.controller.OrchestrateServiceBag", return_value=services
+    ):
       open("cluster.yml", "w").close()
       result = runner.invoke(cli, ["cluster", "create"])
     assert result.exit_code == 0
```

### Comparing `sigopt-8.8.0/test/cli/test_cluster_destroy.py` & `sigopt-8.8.1/test/cli/test_cluster_destroy.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
   def test_cluster_destroy_command(self):
     services = Mock()
     cluster = Mock()
     cluster.name = "foobar"
     cluster.provider_string = "aws"
     services.cluster_service.get_connected_cluster.return_value = cluster
     runner = CliRunner()
-    with patch('sigopt.orchestrate.controller.OrchestrateServiceBag', return_value=services):
+    with patch("sigopt.orchestrate.controller.OrchestrateServiceBag", return_value=services):
       result = runner.invoke(cli, ["cluster", "destroy"])
     services.kubernetes_service.cleanup_for_destroy.assert_called_once()
     services.cluster_service.destroy.assert_called_once_with(
       cluster_name="foobar",
       provider_string="aws",
     )
     assert result.output.splitlines() == [
```

### Comparing `sigopt-8.8.0/test/cli/test_cluster_kubectl.py` & `sigopt-8.8.1/test/cli/test_cluster_kubectl.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,39 +2,44 @@
 #
 # SPDX-License-Identifier: MIT
 import pytest
 from click.testing import CliRunner
 from mock import patch
 
 from sigopt.cli import cli
-from sigopt.orchestrate.paths import get_executable_path
 from sigopt.orchestrate.kubernetes.service import ORCHESTRATE_NAMESPACE
+from sigopt.orchestrate.paths import get_executable_path
 
 
 class TestClusterKubectlCli(object):
-  @pytest.mark.parametrize("arguments", [
-    (),
-    ("-h",),
-    ("--help",),
-    ("--help",),
-    ("get", "--help"),
-    ("exec", "-ti", "po/helloworld", "--", "/bin/sh"),
-  ])
+  @pytest.mark.parametrize(
+    "arguments",
+    [
+      (),
+      ("-h",),
+      ("--help",),
+      ("--help",),
+      ("get", "--help"),
+      ("exec", "-ti", "po/helloworld", "--", "/bin/sh"),
+    ],
+  )
   def test_cluster_kubectl_command(self, arguments):
     kubectl_env_dict = {
-      'KUBECONFIG': 'dummy_kubeconfig',
-      'PATH': '/dummy/bin',
+      "KUBECONFIG": "dummy_kubeconfig",
+      "PATH": "/dummy/bin",
     }
     runner = CliRunner()
-    with \
-      patch('os.execvpe') as mock_execvpe, \
-      patch("sigopt.orchestrate.sigopt.service.get_connection"), \
-      patch('sigopt.orchestrate.kubectl.service.KubectlService.get_kubectl_env', side_effect=[kubectl_env_dict]), \
-      patch('sigopt.orchestrate.cluster.service.ClusterService.assert_is_connected', return_value='foobar'):
+    with patch("os.execvpe") as mock_execvpe, patch("sigopt.orchestrate.sigopt.service.get_connection"), patch(
+      "sigopt.orchestrate.kubectl.service.KubectlService.get_kubectl_env",
+      side_effect=[kubectl_env_dict],
+    ), patch(
+      "sigopt.orchestrate.cluster.service.ClusterService.assert_is_connected",
+      return_value="foobar",
+    ):
       result = runner.invoke(cli, ["cluster", "kubectl", *arguments], catch_exceptions=False)
-      exec_path = get_executable_path('kubectl')
+      exec_path = get_executable_path("kubectl")
       mock_execvpe.assert_called_once_with(
         exec_path,
-        [exec_path, '--namespace', ORCHESTRATE_NAMESPACE, *arguments],
+        [exec_path, "--namespace", ORCHESTRATE_NAMESPACE, *arguments],
         env=kubectl_env_dict,
       )
     assert result.exit_code == 0
```

### Comparing `sigopt-8.8.0/test/cli/test_cluster_run.py` & `sigopt-8.8.1/test/cli/test_cluster_run.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
-import click
-import mock
-import pytest
 from click.testing import CliRunner
 from mock import Mock, patch
 
 from sigopt.cli import cli
 
 
 class TestRunCli(object):
   def test_orchestrate_run(self):
     services = Mock()
     runner = CliRunner()
     with runner.isolated_filesystem():
-      with \
-        patch('sigopt.orchestrate.controller.OrchestrateServiceBag', return_value=services), \
-        patch('sigopt.orchestrate.docker.service.DockerService.create'), \
-        patch(
-          'sigopt.orchestrate.docker.service.DockerService.get_repository_and_tag',
-          return_value=("docker.io/test", "123"),
-        ):
+      with patch("sigopt.orchestrate.controller.OrchestrateServiceBag", return_value=services), patch(
+        "sigopt.orchestrate.docker.service.DockerService.create"
+      ), patch(
+        "sigopt.orchestrate.docker.service.DockerService.get_repository_and_tag",
+        return_value=("docker.io/test", "123"),
+      ):
         services.cluster_service.assert_is_connected = Mock()
         services.gpu_options_validator_service.get_resource_options = Mock(return_value=None)
         open("Dockerfile", "w").close()
         result = runner.invoke(cli, ["cluster", "run", "echo", "hello"])
       assert result.exit_code == 0
```

### Comparing `sigopt-8.8.0/test/cli/test_cluster_test.py` & `sigopt-8.8.1/test/cli/test_cluster_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,12 +7,12 @@
 from sigopt.cli import cli
 
 
 class TestClusterTestCli(object):
   def test_cluster_test_command(self):
     services = Mock()
     runner = CliRunner()
-    with \
-      patch('sigopt.orchestrate.controller.OrchestrateServiceBag', return_value=services), \
-      patch('sigopt.orchestrate.controller.DockerService'):
+    with patch("sigopt.orchestrate.controller.OrchestrateServiceBag", return_value=services), patch(
+      "sigopt.orchestrate.controller.DockerService"
+    ):
       result = runner.invoke(cli, ["cluster", "test"])
     assert result.exit_code == 0
```

### Comparing `sigopt-8.8.0/test/cli/test_init.py` & `sigopt-8.8.1/test/cli/test_init.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
       "run.yml",
       "experiment.yml",
       "Dockerfile",
       ".dockerignore",
     ]
     runner = CliRunner()
     with runner.isolated_filesystem():
-      result = runner.invoke(cli, ['init'])
+      result = runner.invoke(cli, ["init"])
       for filename in files:
         assert os.path.exists(filename)
     assert result.exit_code == 0
     lines = result.output.splitlines()
     assert len(lines) == len(files)
     for line, filename in zip(lines, files):
       assert line == f"Wrote file contents for {filename}"
```

### Comparing `sigopt-8.8.0/test/cli/test_optimize.py` & `sigopt-8.8.1/test/cli/test_optimize.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
-import click
-import mock
 import os
-import pytest
 import shutil
+
+import mock
+import pytest
 from click.testing import CliRunner
 
-from sigopt.cli import cli
 from sigopt.aiexperiment_context import AIExperimentContext
+from sigopt.cli import cli
 from sigopt.run_context import RunContext
 
 
 class TestRunCli(object):
   @pytest.fixture
   def run_context(self):
     run = RunContext(mock.Mock(), mock.Mock(assignments={"fixed1": 0, "fixed2": "test"}))
     run.to_json = mock.Mock(return_value={"run": {}})
     run._end = mock.Mock()
     run._log_source_code = mock.Mock()
     return run
 
   @pytest.fixture(autouse=True)
   def patch_experiment(self, run_context):
-    with mock.patch('sigopt.cli.commands.local.optimize.create_aiexperiment_from_validated_data') as create_aiexperiment:
+    with mock.patch(
+      "sigopt.cli.commands.local.optimize.create_aiexperiment_from_validated_data"
+    ) as create_aiexperiment:
       experiment = AIExperimentContext(mock.Mock(project="test-project"), mock.Mock())
       experiment.create_run = mock.Mock(return_value=run_context)
       experiment.refresh = mock.Mock()
       experiment.is_finished = mock.Mock(side_effect=[False, True])
       create_aiexperiment.return_value = experiment
       yield
 
@@ -44,58 +46,70 @@
         "valid_sigopt.yml",
         "invalid_sigopt.yml",
       ]:
         shutil.copy(os.path.join(root, file), ".")
       yield runner
 
   def test_optimize_command(self, runner):
-    result = runner.invoke(cli, [
-      "optimize",
-      "--experiment-file=valid_sigopt.yml",
-      "python",
-      "print_hello.py",
-    ])
+    result = runner.invoke(
+      cli,
+      [
+        "optimize",
+        "--experiment-file=valid_sigopt.yml",
+        "python",
+        "print_hello.py",
+      ],
+    )
     assert result.output == "hello\n"
     assert result.exit_code == 0
 
   def test_optimize_command_with_args(self, runner):
-    result = runner.invoke(cli, [
-      "optimize",
-      "--experiment-file=valid_sigopt.yml",
-      "python",
-      "print_args.py",
-      "--kwarg=value",
-      "positional_arg",
-      "--",
-      "after -- arg",
-    ])
+    result = runner.invoke(
+      cli,
+      [
+        "optimize",
+        "--experiment-file=valid_sigopt.yml",
+        "python",
+        "print_args.py",
+        "--kwarg=value",
+        "positional_arg",
+        "--",
+        "after -- arg",
+      ],
+    )
     assert result.output == "print_args.py\n--kwarg=value\npositional_arg\n--\nafter -- arg\n"
     assert result.exit_code == 0
 
   def test_optimize_command_track_source_code(self, runner, run_context):
-    runner.invoke(cli, [
-      "optimize",
-      "--experiment-file=valid_sigopt.yml",
-      "--source-file=print_args.py",
-      "python",
-      "print_args.py",
-    ])
+    runner.invoke(
+      cli,
+      [
+        "optimize",
+        "--experiment-file=valid_sigopt.yml",
+        "--source-file=print_args.py",
+        "python",
+        "print_args.py",
+      ],
+    )
     with open("print_args.py") as fp:
       content = fp.read()
     run_context._log_source_code.assert_called_once_with({"content": content})
 
   def test_optimize_command_needs_existing_sigopt_yaml(self, runner):
     runner = CliRunner()
     result = runner.invoke(cli, ["optimize", "python", "print_hello.py"])
     assert "Path 'experiment.yml' does not exist" in result.output
     assert result.exit_code == 2
 
   def test_optimize_command_needs_valid_sigopt_yaml(self, runner):
     runner = CliRunner()
-    result = runner.invoke(cli, [
-      "optimize",
-      "--experiment-file=invalid_sigopt.yml",
-      "python",
-      "print_hello.py",
-    ])
+    result = runner.invoke(
+      cli,
+      [
+        "optimize",
+        "--experiment-file=invalid_sigopt.yml",
+        "python",
+        "print_hello.py",
+      ],
+    )
     assert "The top level should be a mapping of keys to values" in str(result.output)
     assert result.exit_code == 2
```

### Comparing `sigopt-8.8.0/test/cli/test_run.py` & `sigopt-8.8.1/test/cli/test_run.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
+import os
 import shutil
-import click
+
 import mock
-import os
 import pytest
 from click.testing import CliRunner
 
 from sigopt.cli import cli
 from sigopt.run_context import RunContext
 
 
@@ -19,15 +19,15 @@
     run.to_json = mock.Mock(return_value={"run": {}})
     run._end = mock.Mock()
     run._log_source_code = mock.Mock()
     return run
 
   @pytest.fixture(autouse=True)
   def patch_run_factory(self, run_context):
-    with mock.patch('sigopt.cli.commands.local.run.SigOptFactory') as factory:
+    with mock.patch("sigopt.cli.commands.local.run.SigOptFactory") as factory:
       instance = mock.Mock()
       instance.create_run.return_value = run_context
       factory.return_value = instance
       yield
 
   @pytest.fixture
   def runner(self):
@@ -39,55 +39,70 @@
         "print_args.py",
         "import_hello.py",
       ]:
         shutil.copy(os.path.join(root, file), ".")
       yield runner
 
   def test_run_command_echo(self, runner):
-    result = runner.invoke(cli, [
-      "run",
-      "echo",
-      "hello",
-    ])
+    result = runner.invoke(
+      cli,
+      [
+        "run",
+        "echo",
+        "hello",
+      ],
+    )
     assert result.exit_code == 0
     assert result.output == "hello\n"
 
   def test_run_command(self, runner):
     runner = CliRunner()
-    result = runner.invoke(cli, [
-      "run",
-      "python",
-      "print_hello.py",
-    ])
+    result = runner.invoke(
+      cli,
+      [
+        "run",
+        "python",
+        "print_hello.py",
+      ],
+    )
     assert result.exit_code == 0
     assert result.output == "hello\n"
 
   def test_run_command_with_args(self, runner):
-    result = runner.invoke(cli, [
-      "run",
-      "python",
-      "print_args.py",
-      "--kwarg=value",
-      "positional_arg",
-    ])
+    result = runner.invoke(
+      cli,
+      [
+        "run",
+        "python",
+        "print_args.py",
+        "--kwarg=value",
+        "positional_arg",
+      ],
+    )
     assert result.output == "print_args.py\n--kwarg=value\npositional_arg\n"
     assert result.exit_code == 0
 
   def test_run_command_import_sibling(self, runner):
-    result = runner.invoke(cli, [
-      "run",
-      "python",
-      "import_hello.py",
-    ])
+    result = runner.invoke(
+      cli,
+      [
+        "run",
+        "python",
+        "import_hello.py",
+      ],
+    )
     assert result.output == "hello\n"
     assert result.exit_code == 0
 
   def test_run_command_track_source_code(self, runner, run_context):
-    runner.invoke(cli, [
-      "run",
-      "--source-file=print_hello.py",
-      "python",
-      "print_hello.py",
-    ])
+    runner.invoke(
+      cli,
+      [
+        "run",
+        "--source-file=print_hello.py",
+        "python",
+        "print_hello.py",
+      ],
+    )
     with open("print_hello.py") as fp:
       content = fp.read()
     run_context._log_source_code.assert_called_once_with({"content": content})
```

### Comparing `sigopt-8.8.0/test/cli/test_start_worker.py` & `sigopt-8.8.1/test/cli/test_start_worker.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
-import click
-import mock
 import os
-import pytest
 import shutil
+
+import mock
+import pytest
 from click.testing import CliRunner
 
-from sigopt.cli import cli
 from sigopt.aiexperiment_context import AIExperimentContext
+from sigopt.cli import cli
 from sigopt.run_context import RunContext
 
 
 class TestRunCli(object):
   @pytest.fixture
   def run_context(self):
     run = RunContext(mock.Mock(), mock.Mock(assignments={"fixed1": 0, "fixed2": "test"}))
     run.to_json = mock.Mock(return_value={"run": {}})
     run._end = mock.Mock()
     run._log_source_code = mock.Mock()
     return run
 
   @pytest.fixture(autouse=True)
   def patch_run_factory(self, run_context):
-    with mock.patch('sigopt.cli.commands.local.start_worker.SigOptFactory') as factory:
+    with mock.patch("sigopt.cli.commands.local.start_worker.SigOptFactory") as factory:
       experiment = AIExperimentContext(mock.Mock(project="test-project"), mock.Mock())
       experiment.create_run = mock.Mock(return_value=run_context)
       experiment.refresh = mock.Mock()
       experiment.is_finished = mock.Mock(side_effect=[False, True])
       instance = mock.Mock()
       instance.get_aiexperiment.return_value = experiment
       factory.from_default_project = mock.Mock(return_value=instance)
@@ -44,41 +44,50 @@
         "print_args.py",
         "import_hello.py",
       ]:
         shutil.copy(os.path.join(root, file), ".")
       yield runner
 
   def test_start_worker_command(self, runner):
-    result = runner.invoke(cli, [
-      "start-worker",
-      "1234",
-      "python",
-      "print_hello.py",
-    ])
+    result = runner.invoke(
+      cli,
+      [
+        "start-worker",
+        "1234",
+        "python",
+        "print_hello.py",
+      ],
+    )
     assert result.output == "hello\n"
     assert result.exit_code == 0
 
   def test_start_worker_command_with_args(self, runner):
-    result = runner.invoke(cli, [
-      "start-worker",
-      "1234",
-      "python",
-      "print_args.py",
-      "--kwarg=value",
-      "positional_arg",
-      "--",
-      "after -- arg",
-    ])
+    result = runner.invoke(
+      cli,
+      [
+        "start-worker",
+        "1234",
+        "python",
+        "print_args.py",
+        "--kwarg=value",
+        "positional_arg",
+        "--",
+        "after -- arg",
+      ],
+    )
     assert result.output == "print_args.py\n--kwarg=value\npositional_arg\n--\nafter -- arg\n"
     assert result.exit_code == 0
 
   def test_start_worker_command_track_source_code(self, runner, run_context):
-    runner.invoke(cli, [
-      "start-worker",
-      "--source-file=print_args.py",
-      "1234",
-      "python",
-      "print_args.py",
-    ])
+    runner.invoke(
+      cli,
+      [
+        "start-worker",
+        "--source-file=print_args.py",
+        "1234",
+        "python",
+        "print_args.py",
+      ],
+    )
     with open("print_args.py") as fp:
       content = fp.read()
     run_context._log_source_code.assert_called_once_with({"content": content})
```

### Comparing `sigopt-8.8.0/test/cli/test_truncate.py` & `sigopt-8.8.1/test/cli/test_truncate.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 from sigopt.run_context import maybe_truncate_log
 
 
 def test_short_logs_dont_get_truncated():
-  short_logs = 'hello there\n'
+  short_logs = "hello there\n"
   content = maybe_truncate_log(short_logs)
   assert content == short_logs
 
+
 def test_long_logs_get_truncated():
   max_size = 1024
-  long_logs = 'a' * (max_size * 2) + '\n'
+  long_logs = "a" * (max_size * 2) + "\n"
   content = maybe_truncate_log(long_logs)
   assert max_size < len(content) < max_size * 2
-  assert content.startswith('[ WARNING ] ')
-  assert '... truncated ...'  in content
-  assert content.endswith('aaaa\n')
+  assert content.startswith("[ WARNING ] ")
+  assert "... truncated ..." in content
+  assert content.endswith("aaaa\n")
```

### Comparing `sigopt-8.8.0/test/client/test_endpoint.py` & `sigopt-8.8.1/test/client/test_endpoint.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # SPDX-License-Identifier: MIT
 import mock
 import pytest
 
 from sigopt.interface import ConnectionImpl
 from sigopt.request_driver import RequestDriver
 
+
 class TestEndpoint(object):
   @pytest.fixture
   def requestor(self):
     requestor = mock.Mock(RequestDriver)
     response = mock.Mock()
     response.status_code = 200
     response.json = mock.Mock(return_value={})
@@ -18,191 +19,234 @@
     return requestor
 
   @pytest.fixture
   def connection(self, requestor):
     return ConnectionImpl(requestor)
 
   def assert_called(self, requestor, connection, method, path, params=None, headers=None):
-    requestor.request.assert_called_once_with(
-      method.upper(),
-      path,
-      params or {},
-      headers
-    )
+    requestor.request.assert_called_once_with(method.upper(), path, params or {}, headers)
 
   def test_client_detail(self, requestor, connection):
     connection.clients(1).fetch()
-    self.assert_called(requestor, connection, 'get', ["clients", 1])
+    self.assert_called(requestor, connection, "get", ["clients", 1])
 
   def test_client_experiments(self, requestor, connection):
     connection.clients(1).experiments().fetch()
-    self.assert_called(requestor, connection, 'get', ["clients", 1, "experiments"])
+    self.assert_called(requestor, connection, "get", ["clients", 1, "experiments"])
 
   def test_experiment_list(self, requestor, connection):
     connection.experiments().fetch()
-    self.assert_called(requestor, connection, 'get', ["experiments"])
+    self.assert_called(requestor, connection, "get", ["experiments"])
 
   def test_experiment_list_params(self, requestor, connection):
-    connection.experiments().fetch(limit=10, before='1')
-    self.assert_called(requestor, connection, 'get', ["experiments"], params={'limit': 10, 'before': '1'})
+    connection.experiments().fetch(limit=10, before="1")
+    self.assert_called(requestor, connection, "get", ["experiments"], params={"limit": 10, "before": "1"})
 
   def test_experiment_detail(self, requestor, connection):
     connection.experiments(1).fetch()
-    self.assert_called(requestor, connection, 'get', ["experiments", 1])
+    self.assert_called(requestor, connection, "get", ["experiments", 1])
 
   def test_experiment_best_assignments(self, requestor, connection):
     connection.experiments(1).best_assignments().fetch()
-    self.assert_called(requestor, connection, 'get', ["experiments", 1, "best_assignments"])
+    self.assert_called(requestor, connection, "get", ["experiments", 1, "best_assignments"])
 
   def test_experiment_best_training_runs(self, requestor, connection):
     connection.experiments(1).best_training_runs().fetch()
-    self.assert_called(requestor, connection, 'get', ["experiments", 1, "best_training_runs"])
+    self.assert_called(requestor, connection, "get", ["experiments", 1, "best_training_runs"])
 
   def test_experiment_importances(self, requestor, connection):
     connection.experiments(1).importances().fetch()
-    self.assert_called(requestor, connection, 'get', ["experiments", 1, "importances"])
+    self.assert_called(requestor, connection, "get", ["experiments", 1, "importances"])
 
   def test_experiment_metric_importances(self, requestor, connection):
     connection.experiments(1).metric_importances().fetch()
-    self.assert_called(requestor, connection, 'get', ["experiments", 1, "metric_importances"])
+    self.assert_called(requestor, connection, "get", ["experiments", 1, "metric_importances"])
 
   def test_experiment_create(self, requestor, connection):
     connection.experiments().create()
-    self.assert_called(requestor, connection, 'post', ["experiments"])
+    self.assert_called(requestor, connection, "post", ["experiments"])
 
   def test_experiment_create_params(self, requestor, connection):
-    connection.experiments().create(name='Experiment', parameters=[])
-    self.assert_called(requestor, connection, 'post', ["experiments"], params={'name': 'Experiment', 'parameters': []})
+    connection.experiments().create(name="Experiment", parameters=[])
+    self.assert_called(
+      requestor,
+      connection,
+      "post",
+      ["experiments"],
+      params={"name": "Experiment", "parameters": []},
+    )
 
   def test_experiment_update(self, requestor, connection):
     connection.experiments(1).update()
-    self.assert_called(requestor, connection, 'put', ["experiments", 1])
+    self.assert_called(requestor, connection, "put", ["experiments", 1])
 
   def test_experiment_delete(self, requestor, connection):
     connection.experiments(1).delete()
-    self.assert_called(requestor, connection, 'delete', ["experiments", 1])
+    self.assert_called(requestor, connection, "delete", ["experiments", 1])
 
   def test_suggestion_list(self, requestor, connection):
     connection.experiments(1).suggestions().fetch()
-    self.assert_called(requestor, connection, 'get', ["experiments", 1, "suggestions"])
+    self.assert_called(requestor, connection, "get", ["experiments", 1, "suggestions"])
 
   def test_suggestion_list_params(self, requestor, connection):
-    connection.experiments(1).suggestions().fetch(limit=10, before='1')
-    self.assert_called(requestor, connection, 'get', ["experiments", 1, "suggestions"], params={'limit': 10, 'before': '1'})
+    connection.experiments(1).suggestions().fetch(limit=10, before="1")
+    self.assert_called(
+      requestor,
+      connection,
+      "get",
+      ["experiments", 1, "suggestions"],
+      params={"limit": 10, "before": "1"},
+    )
 
   def test_suggestion_detail(self, requestor, connection):
     connection.experiments(1).suggestions(2).fetch()
-    self.assert_called(requestor, connection, 'get', ["experiments", 1, "suggestions", 2])
+    self.assert_called(requestor, connection, "get", ["experiments", 1, "suggestions", 2])
 
   def test_suggestion_create(self, requestor, connection):
     connection.experiments(1).suggestions().create()
-    self.assert_called(requestor, connection, 'post', ["experiments", 1, "suggestions"])
+    self.assert_called(requestor, connection, "post", ["experiments", 1, "suggestions"])
 
   def test_suggestion_create_params(self, requestor, connection):
-    connection.experiments(1).suggestions().create(assignments={'a': 1})
-    self.assert_called(requestor, connection, 'post', ["experiments", 1, "suggestions"], params={'assignments': {'a': 1}})
+    connection.experiments(1).suggestions().create(assignments={"a": 1})
+    self.assert_called(
+      requestor,
+      connection,
+      "post",
+      ["experiments", 1, "suggestions"],
+      params={"assignments": {"a": 1}},
+    )
 
   def test_suggestion_delete(self, requestor, connection):
     connection.experiments(1).suggestions(2).delete()
-    self.assert_called(requestor, connection, 'delete', ["experiments", 1, "suggestions", 2])
+    self.assert_called(requestor, connection, "delete", ["experiments", 1, "suggestions", 2])
 
   def test_suggestion_delete_all(self, requestor, connection):
     connection.experiments(1).suggestions().delete()
-    self.assert_called(requestor, connection, 'delete', ["experiments", 1, "suggestions"])
+    self.assert_called(requestor, connection, "delete", ["experiments", 1, "suggestions"])
 
   def test_suggestion_delete_all_params(self, requestor, connection):
-    connection.experiments(1).suggestions().delete(state='open')
-    self.assert_called(requestor, connection, 'delete', ["experiments", 1, "suggestions"], params={'state': 'open'})
+    connection.experiments(1).suggestions().delete(state="open")
+    self.assert_called(
+      requestor,
+      connection,
+      "delete",
+      ["experiments", 1, "suggestions"],
+      params={"state": "open"},
+    )
 
   def test_queued_suggestion_list(self, requestor, connection):
     connection.experiments(1).queued_suggestions().fetch()
-    self.assert_called(requestor, connection, 'get', ["experiments", 1, "queued_suggestions"])
+    self.assert_called(requestor, connection, "get", ["experiments", 1, "queued_suggestions"])
 
   def test_queued_suggestion_list_params(self, requestor, connection):
-    connection.experiments(1).queued_suggestions().fetch(limit=10, before='1')
+    connection.experiments(1).queued_suggestions().fetch(limit=10, before="1")
     self.assert_called(
       requestor,
       connection,
-      'get',
+      "get",
       ["experiments", 1, "queued_suggestions"],
-      params={'limit': 10, 'before': '1'},
+      params={"limit": 10, "before": "1"},
     )
 
   def test_queued_suggestion_detail(self, requestor, connection):
     connection.experiments(1).queued_suggestions(2).fetch()
-    self.assert_called(requestor, connection, 'get', ["experiments", 1, "queued_suggestions", 2])
+    self.assert_called(requestor, connection, "get", ["experiments", 1, "queued_suggestions", 2])
 
   def test_queued_suggestion_create_params(self, requestor, connection):
-    connection.experiments(1).queued_suggestions().create(assignments={'a': 1})
-    self.assert_called(requestor, connection, 'post', ["experiments", 1, "queued_suggestions"], params={'assignments': {'a': 1}})
+    connection.experiments(1).queued_suggestions().create(assignments={"a": 1})
+    self.assert_called(
+      requestor,
+      connection,
+      "post",
+      ["experiments", 1, "queued_suggestions"],
+      params={"assignments": {"a": 1}},
+    )
 
   def test_queued_suggestion_delete(self, requestor, connection):
     connection.experiments(1).queued_suggestions(2).delete()
-    self.assert_called(requestor, connection, 'delete', ["experiments", 1, "queued_suggestions", 2])
+    self.assert_called(requestor, connection, "delete", ["experiments", 1, "queued_suggestions", 2])
 
   def test_observation_list(self, requestor, connection):
     connection.experiments(1).observations().fetch()
-    self.assert_called(requestor, connection, 'get', ["experiments", 1, "observations"])
+    self.assert_called(requestor, connection, "get", ["experiments", 1, "observations"])
 
   def test_observation_list_params(self, requestor, connection):
-    connection.experiments(1).observations().fetch(limit=10, before='1')
-    self.assert_called(requestor, connection, 'get', ["experiments", 1, "observations"], params={'limit': 10, 'before': '1'})
+    connection.experiments(1).observations().fetch(limit=10, before="1")
+    self.assert_called(
+      requestor,
+      connection,
+      "get",
+      ["experiments", 1, "observations"],
+      params={"limit": 10, "before": "1"},
+    )
 
   def test_observation_detail(self, requestor, connection):
     connection.experiments(1).observations(2).fetch()
-    self.assert_called(requestor, connection, 'get', ["experiments", 1, "observations", 2])
+    self.assert_called(requestor, connection, "get", ["experiments", 1, "observations", 2])
 
   def test_observation_create(self, requestor, connection):
     connection.experiments(1).observations().create()
-    self.assert_called(requestor, connection, 'post', ["experiments", 1, "observations"])
+    self.assert_called(requestor, connection, "post", ["experiments", 1, "observations"])
 
   def test_observation_create_params(self, requestor, connection):
-    connection.experiments(1).observations().create(assignments={'a': 1})
-    self.assert_called(requestor, connection, 'post', ["experiments", 1, "observations"], params={'assignments': {'a': 1}})
+    connection.experiments(1).observations().create(assignments={"a": 1})
+    self.assert_called(
+      requestor,
+      connection,
+      "post",
+      ["experiments", 1, "observations"],
+      params={"assignments": {"a": 1}},
+    )
 
   def test_observation_create_batch(self, requestor, connection):
     connection.experiments(1).observations().create_batch()
-    self.assert_called(requestor, connection, 'post', ["experiments", 1, "observations", "batch"])
+    self.assert_called(requestor, connection, "post", ["experiments", 1, "observations", "batch"])
 
   def test_observation_update(self, requestor, connection):
     connection.experiments(1).observations(2).update()
-    self.assert_called(requestor, connection, 'put', ["experiments", 1, "observations", 2])
+    self.assert_called(requestor, connection, "put", ["experiments", 1, "observations", 2])
 
   def test_observation_update_params(self, requestor, connection):
     connection.experiments(1).observations(2).update(value=5)
-    self.assert_called(requestor, connection, 'put', ["experiments", 1, "observations", 2], params={'value': 5})
+    self.assert_called(
+      requestor,
+      connection,
+      "put",
+      ["experiments", 1, "observations", 2],
+      params={"value": 5},
+    )
 
   def test_observation_delete(self, requestor, connection):
     connection.experiments(1).observations(2).delete()
-    self.assert_called(requestor, connection, 'delete', ["experiments", 1, "observations", 2])
+    self.assert_called(requestor, connection, "delete", ["experiments", 1, "observations", 2])
 
   def test_observation_delete_all(self, requestor, connection):
     connection.experiments(1).observations().delete()
-    self.assert_called(requestor, connection, 'delete', ["experiments", 1, "observations"])
+    self.assert_called(requestor, connection, "delete", ["experiments", 1, "observations"])
 
   def test_token_create(self, requestor, connection):
     connection.experiments(1).tokens().create()
-    self.assert_called(requestor, connection, 'post', ["experiments", 1, "tokens"])
+    self.assert_called(requestor, connection, "post", ["experiments", 1, "tokens"])
 
   def test_call_with_json(self, requestor, connection):
-    connection.experiments(1).tokens().create.call_with_json('{}')
-    self.assert_called(requestor, connection, 'post', ["experiments", 1, "tokens"])
+    connection.experiments(1).tokens().create.call_with_json("{}")
+    self.assert_called(requestor, connection, "post", ["experiments", 1, "tokens"])
 
   def test_call_with_json_params(self, requestor, connection):
     connection.experiments(1).tokens().create.call_with_json('{"value": 5}')
-    self.assert_called(requestor, connection, 'post', ["experiments", 1, "tokens"], params={'value': 5})
+    self.assert_called(requestor, connection, "post", ["experiments", 1, "tokens"], params={"value": 5})
 
   def test_call_with_params(self, requestor, connection):
     connection.experiments(1).tokens().create.call_with_params({})
-    self.assert_called(requestor, connection, 'post', ["experiments", 1, "tokens"])
+    self.assert_called(requestor, connection, "post", ["experiments", 1, "tokens"])
 
   def test_call_with_params_params(self, requestor, connection):
-    connection.experiments(1).tokens().create.call_with_params({'value': 5})
-    self.assert_called(requestor, connection, 'post', ["experiments", 1, "tokens"], params={'value': 5})
+    connection.experiments(1).tokens().create.call_with_params({"value": 5})
+    self.assert_called(requestor, connection, "post", ["experiments", 1, "tokens"], params={"value": 5})
 
   def test_organizations_list(self, requestor, connection):
     connection.organizations().fetch()
-    self.assert_called(requestor, connection, 'get', ["organizations"])
+    self.assert_called(requestor, connection, "get", ["organizations"])
 
   def test_organization_details(self, requestor, connection):
     connection.organizations(1).fetch()
-    self.assert_called(requestor, connection, 'get', ["organizations", 1])
+    self.assert_called(requestor, connection, "get", ["organizations", 1])
```

### Comparing `sigopt-8.8.0/test/client/test_interface.py` & `sigopt-8.8.1/test/client/test_interface.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,80 +1,82 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 import os
+
 import mock
 import pytest
 
 from sigopt.config import config
 from sigopt.interface import Connection
 from sigopt.request_driver import DEFAULT_HTTP_TIMEOUT
 from sigopt.resource import ApiResource
 
+
 class TestInterface(object):
   @pytest.yield_fixture
   def config_dict(self, autouse=True):
     with mock.patch.dict(config._configuration, {}):
       yield config._configuration
 
   def test_create(self):
-    conn = Connection(client_token='client_token')
-    assert conn.impl.driver.api_url == 'https://api.sigopt.com'
+    conn = Connection(client_token="client_token")
+    assert conn.impl.driver.api_url == "https://api.sigopt.com"
     assert conn.impl.driver.verify_ssl_certs is None
     assert conn.impl.driver.proxies is None
     assert conn.impl.driver.timeout == DEFAULT_HTTP_TIMEOUT
-    assert conn.impl.driver.auth.username == 'client_token'
+    assert conn.impl.driver.auth.username == "client_token"
     assert isinstance(conn.clients, ApiResource)
     assert isinstance(conn.experiments, ApiResource)
 
   def test_create_uses_session_if_provided(self):
     session = mock.Mock()
-    conn = Connection(client_token='client_token', session=session)
+    conn = Connection(client_token="client_token", session=session)
     assert conn.impl.driver.session is session
 
     response = mock.Mock()
     session.request.return_value = response
     response.status_code = 200
-    response.text = '{}'
+    response.text = "{}"
     session.request.assert_not_called()
     conn.experiments().fetch()
     session.request.assert_called_once()
 
   def test_environment_variable(self):
-    with mock.patch.dict(os.environ, {'SIGOPT_API_TOKEN': 'client_token'}):
+    with mock.patch.dict(os.environ, {"SIGOPT_API_TOKEN": "client_token"}):
       conn = Connection()
-      assert conn.impl.driver.auth.username == 'client_token'
+      assert conn.impl.driver.auth.username == "client_token"
 
   def test_token_in_config(self, config_dict):
-    with mock.patch.dict(config_dict, {'api_token': 'test_token_in_config'}), mock.patch.dict(os.environ, {}):
+    with mock.patch.dict(config_dict, {"api_token": "test_token_in_config"}), mock.patch.dict(os.environ, {}):
       conn = Connection()
-      assert conn.impl.driver.auth.username == 'test_token_in_config'
+      assert conn.impl.driver.auth.username == "test_token_in_config"
 
   def test_api_url(self):
-    conn = Connection('client_token')
-    conn.set_api_url('https://api-test.sigopt.com')
-    assert conn.impl.driver.api_url == 'https://api-test.sigopt.com'
+    conn = Connection("client_token")
+    conn.set_api_url("https://api-test.sigopt.com")
+    assert conn.impl.driver.api_url == "https://api-test.sigopt.com"
 
   def test_api_url_env(self):
-    with mock.patch.dict(os.environ, {'SIGOPT_API_URL': 'https://api-env.sigopt.com'}):
-      conn = Connection('client_token')
-      assert conn.impl.driver.api_url == 'https://api-env.sigopt.com'
+    with mock.patch.dict(os.environ, {"SIGOPT_API_URL": "https://api-env.sigopt.com"}):
+      conn = Connection("client_token")
+      assert conn.impl.driver.api_url == "https://api-env.sigopt.com"
 
   def test_verify(self):
-    conn = Connection('client_token')
+    conn = Connection("client_token")
     conn.set_verify_ssl_certs(False)
     assert conn.impl.driver.verify_ssl_certs is False
 
   def test_proxies(self):
-    conn = Connection('client_token')
-    conn.set_proxies({'http': 'http://127.0.0.1:6543'})
-    assert conn.impl.driver.proxies['http'] == 'http://127.0.0.1:6543'
+    conn = Connection("client_token")
+    conn.set_proxies({"http": "http://127.0.0.1:6543"})
+    assert conn.impl.driver.proxies["http"] == "http://127.0.0.1:6543"
 
   def test_error(self):
-    with mock.patch.dict(os.environ, {'SIGOPT_API_TOKEN': ''}):
+    with mock.patch.dict(os.environ, {"SIGOPT_API_TOKEN": ""}):
       with pytest.raises(ValueError):
         Connection()
 
   def test_timeout(self):
-    conn = Connection('client_token')
+    conn = Connection("client_token")
     conn.set_timeout(30)
     assert conn.impl.driver.timeout == 30
```

### Comparing `sigopt-8.8.0/test/client/test_lib.py` & `sigopt-8.8.1/test/client/test_lib.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,45 +1,48 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
+import warnings
+
 import numpy
 import pytest
-import warnings
 
 from sigopt.lib import *
 
+
 LONG_NUMBER = 100000000000000000000000
 
+
 class TestBase(object):
   @pytest.fixture(autouse=True)
   def set_warnings(self):
     warnings.simplefilter("error")
 
   def test_is_integer(self):
-    assert is_integer(int('3')) is True
+    assert is_integer(int("3")) is True
     assert is_integer(0) is True
     assert is_integer(LONG_NUMBER) is True
     assert is_integer(numpy.int32()) is True
     assert is_integer(numpy.int64()) is True
 
     assert is_integer([]) is False
     assert is_integer([2]) is False
     assert is_integer({1: 2}) is False
     assert is_integer(None) is False
     assert is_integer(True) is False
     assert is_integer(False) is False
     assert is_integer(4.0) is False
-    assert is_integer('3') is False
+    assert is_integer("3") is False
     assert is_integer(3.14) is False
     assert is_integer(numpy.float32()) is False
     assert is_integer(numpy.float64()) is False
     assert is_integer(numpy.nan) is False
 
   def test_is_number(self):
-    assert is_number(int('3')) is True
+    assert is_number(int("3")) is True
     assert is_number(0) is True
     assert is_number(LONG_NUMBER) is True
     assert is_number(4.0) is True
     assert is_number(3.14) is True
     assert is_number(numpy.int32()) is True
     assert is_number(numpy.int64()) is True
     assert is_number(numpy.float32()) is True
@@ -47,15 +50,15 @@
 
     assert is_number([]) is False
     assert is_number([2]) is False
     assert is_number({1: 2}) is False
     assert is_number(None) is False
     assert is_number(True) is False
     assert is_number(False) is False
-    assert is_number('3') is False
+    assert is_number("3") is False
     assert is_number(numpy.nan) is False
 
   def test_is_numpy_array(self):
     assert is_numpy_array(numpy.array([]))
     assert is_numpy_array(numpy.array([1, 2, 3]))
 
     assert not is_numpy_array([])
@@ -63,85 +66,85 @@
     assert not is_numpy_array(())
     assert not is_numpy_array((1, 2, 3))
     assert not is_numpy_array(None)
     assert not is_numpy_array(False)
     assert not is_numpy_array(True)
     assert not is_numpy_array(0)
     assert not is_numpy_array(1.0)
-    assert not is_numpy_array('abc')
-    assert not is_numpy_array(u'abc')
-    assert not is_numpy_array(b'abc')
+    assert not is_numpy_array("abc")
+    assert not is_numpy_array("abc")
+    assert not is_numpy_array(b"abc")
     assert not is_numpy_array({})
-    assert not is_numpy_array({'a': 123})
+    assert not is_numpy_array({"a": 123})
     assert not is_numpy_array(set())
-    assert not is_numpy_array(set((1, 'a')))
-    assert not is_numpy_array({1, 'a'})
-    assert not is_numpy_array(frozenset((1, 'a')))
+    assert not is_numpy_array(set((1, "a")))
+    assert not is_numpy_array({1, "a"})
+    assert not is_numpy_array(frozenset((1, "a")))
 
   def test_is_sequence(self):
     assert is_sequence([])
     assert is_sequence([1, 2, 3])
     assert is_sequence(())
     assert is_sequence((1, 2, 3))
     assert is_sequence(numpy.array([]))
     assert is_sequence(numpy.array([1, 2, 3]))
 
     assert not is_sequence(None)
     assert not is_sequence(False)
     assert not is_sequence(True)
     assert not is_sequence(0)
     assert not is_sequence(1.0)
-    assert not is_sequence('abc')
-    assert not is_sequence(u'abc')
-    assert not is_sequence(b'abc')
+    assert not is_sequence("abc")
+    assert not is_sequence("abc")
+    assert not is_sequence(b"abc")
     assert not is_sequence({})
-    assert not is_sequence({'a': 123})
+    assert not is_sequence({"a": 123})
     assert not is_sequence(set())
-    assert not is_sequence(set((1, 'a')))
-    assert not is_sequence({1, 'a'})
-    assert not is_sequence(frozenset((1, 'a')))
+    assert not is_sequence(set((1, "a")))
+    assert not is_sequence({1, "a"})
+    assert not is_sequence(frozenset((1, "a")))
 
   def test_is_mapping(self):
     assert is_mapping({})
-    assert is_mapping({'a': 123})
+    assert is_mapping({"a": 123})
 
     assert not is_mapping([])
     assert not is_mapping([1, 2, 3])
     assert not is_mapping(())
     assert not is_mapping((1, 2, 3))
     assert not is_mapping(numpy.array([]))
     assert not is_mapping(numpy.array([1, 2, 3]))
     assert not is_mapping(None)
     assert not is_mapping(False)
     assert not is_mapping(True)
     assert not is_mapping(0)
     assert not is_mapping(1.0)
-    assert not is_mapping('abc')
-    assert not is_mapping(u'abc')
-    assert not is_mapping(b'abc')
+    assert not is_mapping("abc")
+    assert not is_mapping("abc")
+    assert not is_mapping(b"abc")
     assert not is_mapping(set())
-    assert not is_mapping(set((1, 'a')))
-    assert not is_mapping({1, 'a'})
-    assert not is_mapping(frozenset((1, 'a')))
+    assert not is_mapping(set((1, "a")))
+    assert not is_mapping({1, "a"})
+    assert not is_mapping(frozenset((1, "a")))
 
   def test_is_string(self):
-    assert is_string('abc')
-    assert is_string(u'abc')
+    assert is_string("abc")
+    assert is_string("abc")
 
-    assert not is_string(b'abc')
+    assert not is_string(b"abc")
     assert not is_string({})
-    assert not is_string({'a': 123})
+    assert not is_string({"a": 123})
     assert not is_string([])
     assert not is_string([1, 2, 3])
     assert not is_string(())
     assert not is_string((1, 2, 3))
     assert not is_string(numpy.array([]))
     assert not is_string(numpy.array([1, 2, 3]))
     assert not is_string(None)
     assert not is_string(False)
     assert not is_string(True)
     assert not is_string(0)
     assert not is_string(1.0)
     assert not is_string(set())
-    assert not is_string(set((1, 'a')))
-    assert not is_string({1, 'a'})
-    assert not is_string(frozenset((1, 'a')))
+    assert not is_string(set((1, "a")))
+    assert not is_string({1, "a"})
+    assert not is_string(frozenset((1, "a")))
```

### Comparing `sigopt-8.8.0/test/client/test_object.py` & `sigopt-8.8.1/test/client/test_object.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 import json
-import numpy
 import os
-import pytest
 import warnings
 
+import numpy
+import pytest
+
 from sigopt.objects import *
+
 from ..utils import ObserveWarnings
 
+
 def load(filename):
-  with open(os.path.join(os.path.dirname(__file__), 'json_data', filename), "r") as f:
+  with open(os.path.join(os.path.dirname(__file__), "json_data", filename), "r") as f:
     return json.load(f)
 
+
 def load_and_parse(Cls, filename):
   data = load(filename)
   obj = Cls(data)
   assert obj.to_json() == data
   assert ApiObject.as_json(obj) == data
   return obj
 
+
 class TestBase(object):
   @pytest.fixture(autouse=True)
   def set_warnings(self):
     warnings.simplefilter("error")
 
   def test_as_json(self):
     assert ApiObject.as_json(None) is None
@@ -34,15 +39,15 @@
     assert ApiObject.as_json(1.1) == 1.1
     assert ApiObject.as_json(numpy.int8(4)) == 4
     assert ApiObject.as_json(numpy.int32(4)) == 4
     assert ApiObject.as_json(numpy.int64(4)) == 4
     assert ApiObject.as_json(numpy.float16(5.5)) == 5.5
     assert ApiObject.as_json(numpy.float32(5.5)) == 5.5
     assert ApiObject.as_json(numpy.float64(5.5)) == 5.5
-    assert ApiObject.as_json('abc') == 'abc'
+    assert ApiObject.as_json("abc") == "abc"
 
     assert ApiObject.as_json({}) == {}
     assert ApiObject.as_json({"a": "b"}) == {"a": "b"}
     assert ApiObject.as_json(Assignments({"a": "b"})) == {"a": "b"}
     assert ApiObject.as_json(Experiment({"name": "test"})) == {"name": "test"}
     assert ApiObject.as_json(Experiment({"bounds": {"min": 0}})) == {"bounds": {"min": 0}}
 
@@ -58,368 +63,371 @@
 
   def test_equality(self):
     assert Experiment({}) == Experiment({})
     assert Experiment({}) != {}
     assert {} != Experiment({})
     assert Bounds({}) != Experiment({})
 
-    assert Experiment({'a': 'b'}) == Experiment({'a': 'b'})
-    assert Experiment({'a': 'b'}) != Experiment({})
-    assert Experiment({'a': 'b'}) != Experiment({'a': 'c'})
-    assert Experiment({'a': 'b'}) != Experiment({'a': 'b', 'c': 'd'})
-
-    assert Assignments({'a': 'b'}) == Assignments({'a': 'b'})
-    assert Assignments({'a': 'b'}) != Assignments({})
-    assert Assignments({'a': 'b'}) != Assignments({'a': 'c'})
-    assert Assignments({'a': 'b'}) != Assignments({'a': 'b', 'c': 'd'})
+    assert Experiment({"a": "b"}) == Experiment({"a": "b"})
+    assert Experiment({"a": "b"}) != Experiment({})
+    assert Experiment({"a": "b"}) != Experiment({"a": "c"})
+    assert Experiment({"a": "b"}) != Experiment({"a": "b", "c": "d"})
+
+    assert Assignments({"a": "b"}) == Assignments({"a": "b"})
+    assert Assignments({"a": "b"}) != Assignments({})
+    assert Assignments({"a": "b"}) != Assignments({"a": "c"})
+    assert Assignments({"a": "b"}) != Assignments({"a": "b", "c": "d"})
 
   def test_repr(self):
-    assert repr(Experiment({})) == 'Experiment()'
-    assert repr(Experiment({'user': 'b'})) == 'Experiment(\n  user="b",\n)'
-    assert repr(Assignments({})) == 'Assignments({})'
-    assert repr(Assignments({'a': 'b'})) == 'Assignments({\n  "a": "b"\n})'
-    assert repr(Assignments({'a': 'b', 'c': 'd'})) == 'Assignments({\n  "a": "b",\n  "c": "d"\n})'
+    assert repr(Experiment({})) == "Experiment()"
+    assert repr(Experiment({"user": "b"})) == 'Experiment(\n  user="b",\n)'
+    assert repr(Assignments({})) == "Assignments({})"
+    assert repr(Assignments({"a": "b"})) == 'Assignments({\n  "a": "b"\n})'
+    assert repr(Assignments({"a": "b", "c": "d"})) == 'Assignments({\n  "a": "b",\n  "c": "d"\n})'
     assert (
-        repr(Bounds({'max': 0.1, 'min': -0.2})) == 'Bounds(\n  max=0.1,\n  min=-0.2,\n)'
-        or repr(Bounds({'max': 0.1, 'min': -0.2})) == 'Bounds(\n  min=-0.2,\n  max=0.1,\n)'
+      repr(Bounds({"max": 0.1, "min": -0.2})) == "Bounds(\n  max=0.1,\n  min=-0.2,\n)"
+      or repr(Bounds({"max": 0.1, "min": -0.2})) == "Bounds(\n  min=-0.2,\n  max=0.1,\n)"
     )
-    assert repr(Pagination(Experiment, {'data': [{}]})) == (
-      'Pagination<Experiment>(\n  data=[\n    Experiment(),\n  ],\n)'
+    assert (
+      repr(Pagination(Experiment, {"data": [{}]})) == "Pagination<Experiment>(\n  data=[\n    Experiment(),\n  ],\n)"
     )
 
   def test_json(self):
     assert Experiment({}).to_json() == {}
-    assert Experiment({'bounds': {'min': 1, 'max': 2}}).to_json() == {'bounds': {'min': 1, 'max': 2}}
+    assert Experiment({"bounds": {"min": 1, "max": 2}}).to_json() == {"bounds": {"min": 1, "max": 2}}
     assert Assignments({}).to_json() == {}
-    assert Assignments({'abc': 'def', 'ghi': 123}).to_json() == {'abc': 'def', 'ghi': 123}
+    assert Assignments({"abc": "def", "ghi": 123}).to_json() == {
+      "abc": "def",
+      "ghi": 123,
+    }
 
   def test_dict_like(self):
-    a = Assignments({'abc': 'def', 'ghi': 123})
-    assert a['abc'] == 'def'
-    assert a.get('abc') == 'def'
-    assert a.get('abc', 'fake') == 'def'
-    assert a['ghi'] == 123
-    assert a.get('ghi') == 123
-    assert a.get('ghi', 'fake') == 123
+    a = Assignments({"abc": "def", "ghi": 123})
+    assert a["abc"] == "def"
+    assert a.get("abc") == "def"
+    assert a.get("abc", "fake") == "def"
+    assert a["ghi"] == 123
+    assert a.get("ghi") == 123
+    assert a.get("ghi", "fake") == 123
 
     with pytest.raises(AttributeError):
       a.method_that_doesnt_exist_on_dict()
 
     with pytest.raises(KeyError):
-      a['xyz']  # pylint: disable=pointless-statement
-    assert a.get('xyz') is None
-    assert a.get('xyz', 'fake') == 'fake'
+      a["xyz"]  # pylint: disable=pointless-statement
+    assert a.get("xyz") is None
+    assert a.get("xyz", "fake") == "fake"
 
     assert len(a) == 2
-    assert set(a.keys()) == set(('abc', 'ghi'))
-    assert 'abc' in a
-    assert 'xyz' not in a
-
-    a['abc'] = 123
-    a['lmn'] = 'pqr'
-    assert a['abc'] == 123
-    assert a['lmn'] == 'pqr'
-    assert a.to_json()['abc'] == 123
-    assert a.to_json()['lmn'] == 'pqr'
+    assert set(a.keys()) == set(("abc", "ghi"))
+    assert "abc" in a
+    assert "xyz" not in a
+
+    a["abc"] = 123
+    a["lmn"] = "pqr"
+    assert a["abc"] == 123
+    assert a["lmn"] == "pqr"
+    assert a.to_json()["abc"] == 123
+    assert a.to_json()["lmn"] == "pqr"
 
     assert a.copy() == a
 
 
 class TestObjects(object):
   @pytest.fixture
   def experiment(self):
-    return load_and_parse(Experiment, 'experiment.json')
+    return load_and_parse(Experiment, "experiment.json")
 
   def test_experiment(self, experiment):
-    assert experiment.id == '123'
-    assert experiment.name == 'Test Experiment'
+    assert experiment.id == "123"
+    assert experiment.name == "Test Experiment"
     assert experiment.created == 321
     assert isinstance(experiment.metrics[0], Metric)
-    assert experiment.metrics[0].name == 'Revenue'
-    assert experiment.metrics[0].objective == 'maximize'
-    assert experiment.metrics[0].strategy == 'optimize'
+    assert experiment.metrics[0].name == "Revenue"
+    assert experiment.metrics[0].objective == "maximize"
+    assert experiment.metrics[0].strategy == "optimize"
     assert experiment.metrics[0].threshold is None
     assert isinstance(experiment.metrics[1], Metric)
-    assert experiment.metrics[1].name == 'Sales'
-    assert experiment.metrics[1].strategy == 'optimize'
+    assert experiment.metrics[1].name == "Sales"
+    assert experiment.metrics[1].strategy == "optimize"
     assert experiment.metrics[1].threshold == -3.0
-    assert experiment.client == '678'
+    assert experiment.client == "678"
     assert experiment.linear_constraints
     assert experiment.linear_constraints[0]
-    assert experiment.linear_constraints[0].type == 'greater_than'
+    assert experiment.linear_constraints[0].type == "greater_than"
     assert experiment.linear_constraints[0].threshold == 5
     assert experiment.linear_constraints[0].terms
-    assert experiment.linear_constraints[0].terms[0].name == 'a'
+    assert experiment.linear_constraints[0].terms[0].name == "a"
     assert experiment.linear_constraints[0].terms[0].weight == 2
     assert experiment.conditionals
     assert experiment.conditionals[0]
-    assert experiment.conditionals[0].name == 'num_hidden_layers'
-    assert experiment.conditionals[0].values == ['1', '3']
+    assert experiment.conditionals[0].name == "num_hidden_layers"
+    assert experiment.conditionals[0].values == ["1", "3"]
     assert isinstance(experiment.progress, Progress)
     assert experiment.progress.observation_count == 3
     assert experiment.progress.observation_budget_consumed == 3.0
     assert isinstance(experiment.progress.first_observation, Observation)
-    assert experiment.progress.first_observation.id == '1'
+    assert experiment.progress.first_observation.id == "1"
     assert isinstance(experiment.progress.first_observation.assignments, Assignments)
-    assert experiment.progress.first_observation.assignments.get('a') == 1
-    assert experiment.progress.first_observation.assignments.get('b') == 'c'
-    assert experiment.progress.first_observation.values[0].name == 'Revenue'
+    assert experiment.progress.first_observation.assignments.get("a") == 1
+    assert experiment.progress.first_observation.assignments.get("b") == "c"
+    assert experiment.progress.first_observation.values[0].name == "Revenue"
     assert experiment.progress.first_observation.values[0].value == 3.1
     assert experiment.progress.first_observation.values[0].value_stddev is None
-    assert experiment.progress.first_observation.values[1].name == 'Sales'
+    assert experiment.progress.first_observation.values[1].name == "Sales"
     assert experiment.progress.first_observation.values[1].value == 2.5
     assert experiment.progress.first_observation.values[1].value_stddev is None
     assert experiment.progress.first_observation.failed is False
     assert experiment.progress.first_observation.created == 451
-    assert experiment.progress.first_observation.suggestion == '11'
-    assert experiment.progress.first_observation.experiment == '123'
+    assert experiment.progress.first_observation.suggestion == "11"
+    assert experiment.progress.first_observation.experiment == "123"
     assert isinstance(experiment.progress.last_observation, Observation)
-    assert experiment.progress.last_observation.id == '2'
+    assert experiment.progress.last_observation.id == "2"
     assert isinstance(experiment.progress.last_observation.assignments, Assignments)
-    assert experiment.progress.last_observation.assignments.get('a') == 2
-    assert experiment.progress.last_observation.assignments.get('b') == 'd'
-    assert experiment.progress.last_observation.values[0].name == 'Revenue'
+    assert experiment.progress.last_observation.assignments.get("a") == 2
+    assert experiment.progress.last_observation.assignments.get("b") == "d"
+    assert experiment.progress.last_observation.values[0].name == "Revenue"
     assert experiment.progress.last_observation.values[0].value == 3.1
     assert experiment.progress.last_observation.values[0].value_stddev == 0.5
-    assert experiment.progress.last_observation.values[1].name == 'Sales'
+    assert experiment.progress.last_observation.values[1].name == "Sales"
     assert experiment.progress.last_observation.values[1].value == 2.5
     assert experiment.progress.last_observation.values[1].value_stddev == 0.8
     assert experiment.progress.last_observation.failed is False
     assert experiment.progress.last_observation.created == 452
-    assert experiment.progress.last_observation.suggestion == '12'
-    assert experiment.progress.last_observation.experiment == '123'
+    assert experiment.progress.last_observation.suggestion == "12"
+    assert experiment.progress.last_observation.experiment == "123"
     assert len(experiment.parameters) == 2
     assert isinstance(experiment.parameters[0], Parameter)
-    assert experiment.parameters[0].name == 'a'
-    assert experiment.parameters[0].type == 'double'
+    assert experiment.parameters[0].name == "a"
+    assert experiment.parameters[0].type == "double"
     assert isinstance(experiment.parameters[0].bounds, Bounds)
     assert experiment.parameters[0].bounds.min == 1
     assert experiment.parameters[0].bounds.max == 2
     assert experiment.parameters[0].categorical_values is None
     assert experiment.parameters[0].precision == 3
     assert experiment.parameters[0].default_value == 2
     assert isinstance(experiment.parameters[0].conditions, Conditions)
-    assert experiment.parameters[0].conditions['num_hidden_layers'] == []
+    assert experiment.parameters[0].conditions["num_hidden_layers"] == []
     assert isinstance(experiment.parameters[1], Parameter)
-    assert experiment.parameters[1].name == 'b'
-    assert experiment.parameters[1].type == 'categorical'
+    assert experiment.parameters[1].name == "b"
+    assert experiment.parameters[1].type == "categorical"
     assert experiment.parameters[1].bounds is None
     assert len(experiment.parameters[1].categorical_values) == 2
     assert isinstance(experiment.parameters[1].categorical_values[0], CategoricalValue)
-    assert experiment.parameters[1].categorical_values[0].name == 'c'
+    assert experiment.parameters[1].categorical_values[0].name == "c"
     assert experiment.parameters[1].categorical_values[0].enum_index == 1
-    assert experiment.parameters[1].categorical_values[1].name == 'd'
+    assert experiment.parameters[1].categorical_values[1].name == "d"
     assert experiment.parameters[1].categorical_values[1].enum_index == 2
     assert experiment.parameters[1].precision is None
     assert experiment.parameters[1].default_value is None
     assert isinstance(experiment.parameters[1].conditions, Conditions)
-    assert experiment.parameters[1].conditions['num_hidden_layers'] == ['1', '3']
+    assert experiment.parameters[1].conditions["num_hidden_layers"] == ["1", "3"]
     assert isinstance(experiment.metadata, Metadata)
-    assert experiment.metadata['abc'] == 'def'
-    assert experiment.metadata['ghi'] == 123
+    assert experiment.metadata["abc"] == "def"
+    assert experiment.metadata["ghi"] == 123
     assert experiment.parallel_bandwidth == 2
     assert experiment.updated == 453
-    assert experiment.user == '789'
+    assert experiment.user == "789"
 
     with ObserveWarnings() as w:
       assert experiment.can_be_deleted is None
       assert len(w) == 1
       assert issubclass(w[-1].category, DeprecationWarning)
 
     with ObserveWarnings() as w:
       assert experiment.parameters[0].tunable is None
       assert len(w) == 1
       assert issubclass(w[-1].category, DeprecationWarning)
 
     with ObserveWarnings() as w:
       best_observation = experiment.progress.best_observation
       assert isinstance(best_observation, Observation)
-      assert best_observation.id == '3'
+      assert best_observation.id == "3"
       assert isinstance(best_observation.assignments, Assignments)
-      assert best_observation.assignments.get('a') == 3
-      assert best_observation.assignments.get('b') == 'd'
-      assert best_observation.values[0].name == 'Revenue'
+      assert best_observation.assignments.get("a") == 3
+      assert best_observation.assignments.get("b") == "d"
+      assert best_observation.values[0].name == "Revenue"
       assert best_observation.values[0].value is None
       assert best_observation.values[0].value_stddev is None
-      assert best_observation.values[1].name == 'Sales'
+      assert best_observation.values[1].name == "Sales"
       assert best_observation.values[1].value is None
       assert best_observation.values[1].value_stddev is None
       assert best_observation.failed is True
       assert best_observation.created == 453
-      assert best_observation.suggestion == '13'
-      assert best_observation.experiment == '123'
+      assert best_observation.suggestion == "13"
+      assert best_observation.experiment == "123"
       assert isinstance(best_observation.metadata, Metadata)
-      assert best_observation.metadata['abc'] == 'def'
-      assert best_observation.metadata['ghi'] == 123
+      assert best_observation.metadata["abc"] == "def"
+      assert best_observation.metadata["ghi"] == 123
       assert len(w) == 1
       assert issubclass(w[0].category, DeprecationWarning)
-      assert 'best_assignments' in str(w[0].message)
+      assert "best_assignments" in str(w[0].message)
 
     tasks_dict = {et.name: et.cost for et in experiment.tasks}
-    assert tasks_dict == {'task 1': 0.567, 'task 2': 1.0}
+    assert tasks_dict == {"task 1": 0.567, "task 2": 1.0}
 
   def test_mutable_experiment(self, experiment):
-    experiment.name = 'other name'
-    assert experiment.name == 'other name'
-    assert experiment.to_json()['name'] == 'other name'
+    experiment.name = "other name"
+    assert experiment.name == "other name"
+    assert experiment.to_json()["name"] == "other name"
 
     experiment.parameters = [Parameter({})]
     assert len(experiment.parameters) == 1
     assert isinstance(experiment.parameters[0], Parameter)
     assert experiment.parameters[0].to_json() == {}
-    assert experiment.to_json()['parameters'] == [{}]
+    assert experiment.to_json()["parameters"] == [{}]
 
-    experiment.metadata = {'rst': 'zzz'}
+    experiment.metadata = {"rst": "zzz"}
     assert isinstance(experiment.metadata, Metadata)
-    assert experiment.metadata['rst'] == 'zzz'
-    assert experiment.metadata.get('abc') is None
+    assert experiment.metadata["rst"] == "zzz"
+    assert experiment.metadata.get("abc") is None
 
   def test_del_experiment(self, experiment):
     assert experiment.name is not None
     assert experiment.parameters is not None
     assert experiment.metadata is not None
     del experiment.name
     del experiment.parameters
     del experiment.metadata
     assert experiment.name is None
     assert experiment.parameters is None
     assert experiment.metadata is None
 
   def test_client(self):
-    client = load_and_parse(Client, 'client.json')
+    client = load_and_parse(Client, "client.json")
     assert isinstance(client, Client)
-    assert client.id == '1'
-    assert client.name == 'Client'
+    assert client.id == "1"
+    assert client.name == "Client"
     assert client.created == 123
-    assert client.organization == '2'
+    assert client.organization == "2"
 
   def test_suggestion(self):
-    suggestion = load_and_parse(Suggestion, 'suggestion.json')
+    suggestion = load_and_parse(Suggestion, "suggestion.json")
     assert isinstance(suggestion, Suggestion)
-    assert suggestion.id == '1'
+    assert suggestion.id == "1"
     assert isinstance(suggestion.assignments, Assignments)
-    assert suggestion.assignments.get('a') == 1
-    assert suggestion.assignments.get('b') == 'c'
-    assert suggestion.state == 'open'
-    assert suggestion.experiment == '1'
+    assert suggestion.assignments.get("a") == 1
+    assert suggestion.assignments.get("b") == "c"
+    assert suggestion.state == "open"
+    assert suggestion.experiment == "1"
     assert suggestion.created == 123
     assert isinstance(suggestion.metadata, Metadata)
-    assert suggestion.metadata['abc'] == 'def'
-    assert suggestion.metadata['ghi'] == 123
+    assert suggestion.metadata["abc"] == "def"
+    assert suggestion.metadata["ghi"] == 123
     assert isinstance(suggestion.task, Task)
-    assert suggestion.task.name == 'task 1'
+    assert suggestion.task.name == "task 1"
     assert suggestion.task.cost == 0.567
 
   def test_queued_suggestion(self):
-    queued_suggestion = load_and_parse(QueuedSuggestion, 'queued_suggestion.json')
+    queued_suggestion = load_and_parse(QueuedSuggestion, "queued_suggestion.json")
     assert isinstance(queued_suggestion, QueuedSuggestion)
-    assert queued_suggestion.id == '1'
+    assert queued_suggestion.id == "1"
     assert isinstance(queued_suggestion.assignments, Assignments)
-    assert queued_suggestion.assignments.get('a') == 1
-    assert queued_suggestion.assignments.get('b') == 'c'
-    assert queued_suggestion.experiment == '1'
+    assert queued_suggestion.assignments.get("a") == 1
+    assert queued_suggestion.assignments.get("b") == "c"
+    assert queued_suggestion.experiment == "1"
     assert queued_suggestion.created == 123
     assert isinstance(queued_suggestion.task, Task)
-    assert queued_suggestion.task.name == 'task 1'
+    assert queued_suggestion.task.name == "task 1"
     assert queued_suggestion.task.cost == 0.567
 
   def test_pagination(self):
-    pagination = Pagination(Experiment, load('pagination.json'))
+    pagination = Pagination(Experiment, load("pagination.json"))
     assert isinstance(pagination, Pagination)
     assert pagination.count == 2
     assert isinstance(pagination.paging, Paging)
-    assert pagination.paging.before == '1'
-    assert pagination.paging.after == '2'
+    assert pagination.paging.before == "1"
+    assert pagination.paging.after == "2"
     with ObserveWarnings() as w:
       data = pagination.data
       assert len(data) == 1
       assert isinstance(data[0], Experiment)
       assert len(w) == 1
       assert issubclass(w[-1].category, RuntimeWarning)
 
   def test_token(self):
-    token = load_and_parse(Token, 'token.json')
+    token = load_and_parse(Token, "token.json")
     assert isinstance(token, Token)
     assert token.all_experiments is False
-    assert token.client == '456'
+    assert token.client == "456"
     assert token.development is True
-    assert token.experiment == '1'
+    assert token.experiment == "1"
     assert token.expires == 1547139000
-    assert token.token == '123'
-    assert token.token_type == 'client-dev'
-    assert token.user == '789'
+    assert token.token == "123"
+    assert token.token_type == "client-dev"
+    assert token.user == "789"
 
     with ObserveWarnings() as w:
-      assert token.permissions == 'read'
+      assert token.permissions == "read"
       assert len(w) == 1
       assert issubclass(w[-1].category, DeprecationWarning)
 
   def test_metric(self):
-    metric = load_and_parse(Metric, 'metric.json')
+    metric = load_and_parse(Metric, "metric.json")
     assert isinstance(metric, Metric)
-    assert metric.name == 'Test'
-    assert metric.objective == 'maximize'
+    assert metric.name == "Test"
+    assert metric.objective == "maximize"
     assert metric.threshold is None
 
   def test_importances(self):
-    importances = load_and_parse(Importances, 'importances.json')
+    importances = load_and_parse(Importances, "importances.json")
     assert isinstance(importances, Importances)
     assert isinstance(importances.importances, ImportancesMap)
-    assert importances.importances['a'] == 0.92
-    assert importances.importances['b'] == 0.03
+    assert importances.importances["a"] == 0.92
+    assert importances.importances["b"] == 0.03
 
   def test_metric_importances(self):
-    metric_importances = load_and_parse(MetricImportances, 'metric_importances.json')
+    metric_importances = load_and_parse(MetricImportances, "metric_importances.json")
     assert isinstance(metric_importances, MetricImportances)
     assert isinstance(metric_importances.importances, ImportancesMap)
-    assert metric_importances.importances['parameter_1'] == 0.92
-    assert metric_importances.importances['parameter_2'] == 0.65
-    assert metric_importances.importances['parameter_3'] == 0.03
+    assert metric_importances.importances["parameter_1"] == 0.92
+    assert metric_importances.importances["parameter_2"] == 0.65
+    assert metric_importances.importances["parameter_3"] == 0.03
 
   def test_organization(self):
-    organization = load_and_parse(Organization, 'organization.json')
+    organization = load_and_parse(Organization, "organization.json")
     assert isinstance(organization, Organization)
     assert organization.created == 123456
     assert organization.id == "7890"
     assert organization.name == "SigOpt"
 
   def test_task(self):
-    task = load_and_parse(Task, 'task.json')
+    task = load_and_parse(Task, "task.json")
     assert isinstance(task, Task)
-    assert task.name == 'task 1'
+    assert task.name == "task 1"
     assert task.cost == 0.567
 
   def test_training_run(self):
-    run = load_and_parse(TrainingRun, 'training_run.json')
-    assert run.assignments['m'] == 1
-    assert run.assignments['n'] == 2
-    assert run.best_checkpoint == 'cp0'
-    assert run.client == '11674'
+    run = load_and_parse(TrainingRun, "training_run.json")
+    assert run.assignments["m"] == 1
+    assert run.assignments["n"] == 2
+    assert run.best_checkpoint == "cp0"
+    assert run.client == "11674"
     assert run.checkpoint_count == 2
     assert run.completed == 1631654369
     assert run.created == 1631654365
-    assert run.datasets == ['dataset1', 'dataset2']
+    assert run.datasets == ["dataset1", "dataset2"]
     assert run.deleted is False
-    assert run.experiment == '432979'
-    assert run.files == ['f0', 'f1']
+    assert run.experiment == "432979"
+    assert run.files == ["f0", "f1"]
     assert run.finished is True
-    assert run.id == '95658'
-    assert run.logs['stderr'] == 'message stderr\n'
-    assert run.logs['stdout'] == 'message stdout\n'
-    assert run.metadata['m0'] == 'v0'
-    assert run.metadata['m1'] == 'v1'
-    assert run.model.type == 'type0'
-    assert run.name == 'run-examples 2021-09-14 14:19:26'
-    assert run.object == 'training_run'
-    assert run.observation == '31818393'
-    assert run.project == 'run-examples'
-    assert run.source_code.content == 'c0'
-    assert run.source_code.hash == 'h0'
-    assert run.state == 'completed'
-    assert run.suggestion == '46227605'
-    assert run.tags == ['t0', 't1']
+    assert run.id == "95658"
+    assert run.logs["stderr"] == "message stderr\n"
+    assert run.logs["stdout"] == "message stdout\n"
+    assert run.metadata["m0"] == "v0"
+    assert run.metadata["m1"] == "v1"
+    assert run.model.type == "type0"
+    assert run.name == "run-examples 2021-09-14 14:19:26"
+    assert run.object == "training_run"
+    assert run.observation == "31818393"
+    assert run.project == "run-examples"
+    assert run.source_code.content == "c0"
+    assert run.source_code.hash == "h0"
+    assert run.state == "completed"
+    assert run.suggestion == "46227605"
+    assert run.tags == ["t0", "t1"]
     assert run.updated == 1631654369
-    assert run.user == '53628'
-    assert run.values['accuracy'].value == 1
-    assert run.values['accuracy'].value_stddev == 0.1
-    assert run.values['f1'].value == 2
-    assert run.values['f1'].value_stddev == 0.2
+    assert run.user == "53628"
+    assert run.values["accuracy"].value == 1
+    assert run.values["accuracy"].value_stddev == 0.1
+    assert run.values["f1"].value == 2
+    assert run.values["f1"].value_stddev == 0.2
```

### Comparing `sigopt-8.8.0/test/client/test_pagination.py` & `sigopt-8.8.1/test/client/test_pagination.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,245 +1,323 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
+import warnings
+
 import mock
 import pytest
-import warnings
 
 from sigopt.endpoint import BoundApiEndpoint
 from sigopt.objects import *
 
+
 warnings.simplefilter("error")
 
+
 class TestPagination(object):
   @pytest.fixture(autouse=True)
   def set_warnings(self):
     warnings.simplefilter("error")
 
   @pytest.fixture
   def experiment1(self):
-    return Experiment({'object': 'experiment'})
+    return Experiment({"object": "experiment"})
 
   @pytest.fixture
   def experiment2(self):
-    return Experiment({'object': 'experiment', 'type': 'offline'})
+    return Experiment({"object": "experiment", "type": "offline"})
 
   @pytest.fixture
   def bound_endpoint(self, experiment2, no_paging):
-    second_page = Pagination(Experiment, {
-      'object': 'pagination',
-      'count': 2,
-      'data': [experiment2.to_json()],
-      'paging': no_paging,
-    })
+    second_page = Pagination(
+      Experiment,
+      {
+        "object": "pagination",
+        "count": 2,
+        "data": [experiment2.to_json()],
+        "paging": no_paging,
+      },
+    )
     return mock.Mock(BoundApiEndpoint, side_effect=lambda *args, **kwargs: second_page)
 
   def test_empty(self, bound_endpoint):
     assert list(Pagination(Experiment, {}, bound_endpoint, {}).iterate_pages()) == []
     assert bound_endpoint.mock_calls == []
 
   @pytest.fixture
   def no_paging(self):
     return dict(before=None, after=None)
 
-  @pytest.fixture(params=[
-    dict(before='1', after='2'),
-    dict(after='2'),
-  ])
+  @pytest.fixture(
+    params=[
+      dict(before="1", after="2"),
+      dict(after="2"),
+    ]
+  )
   def backward_paging(self, request):
     return request.param
 
-  @pytest.fixture(params=[
-    dict(before='1', after=None),
-    dict(before='1', after='2'),
-  ])
+  @pytest.fixture(
+    params=[
+      dict(before="1", after=None),
+      dict(before="1", after="2"),
+    ]
+  )
   def forward_paging(self, request):
     return request.param
 
   def test_single_page(self, experiment1, bound_endpoint, no_paging):
-    assert list(Pagination(Experiment, {
-      'object': 'pagination',
-      'count': 1,
-      'data': [experiment1.to_json()],
-      'paging': no_paging,
-    }, bound_endpoint, {}).iterate_pages()) == [experiment1]
+    assert list(
+      Pagination(
+        Experiment,
+        {
+          "object": "pagination",
+          "count": 1,
+          "data": [experiment1.to_json()],
+          "paging": no_paging,
+        },
+        bound_endpoint,
+        {},
+      ).iterate_pages()
+    ) == [experiment1]
     assert bound_endpoint.mock_calls == []
 
   def make_call(self, paging, bound_endpoint, retrieve_params):
-    list(Pagination(Experiment, {
-      'object': 'pagination',
-      'count': 1,
-      'data': [{'object': 'experiment'}],
-      'paging': paging,
-    }, bound_endpoint, retrieve_params).iterate_pages())
+    list(
+      Pagination(
+        Experiment,
+        {
+          "object": "pagination",
+          "count": 1,
+          "data": [{"object": "experiment"}],
+          "paging": paging,
+        },
+        bound_endpoint,
+        retrieve_params,
+      ).iterate_pages()
+    )
 
   def test_next_page(self, experiment1, experiment2, bound_endpoint, forward_paging):
-    assert list(Pagination(Experiment, {
-      'object': 'pagination',
-      'count': 1,
-      'data': [experiment1.to_json()],
-      'paging': forward_paging,
-    }, bound_endpoint, {}).iterate_pages()) == [experiment1, experiment2]
+    assert list(
+      Pagination(
+        Experiment,
+        {
+          "object": "pagination",
+          "count": 1,
+          "data": [experiment1.to_json()],
+          "paging": forward_paging,
+        },
+        bound_endpoint,
+        {},
+      ).iterate_pages()
+    ) == [experiment1, experiment2]
     assert len(bound_endpoint.mock_calls) == 1
 
   def test_receive_after_doesnt_page(self, experiment1, experiment2, bound_endpoint, backward_paging):
-    assert list(Pagination(Experiment, {
-      'object': 'pagination',
-      'count': 1,
-      'data': [experiment1.to_json()],
-      'paging': {'after': '2'},
-    }, bound_endpoint, {}).iterate_pages()) == [experiment1]
+    assert list(
+      Pagination(
+        Experiment,
+        {
+          "object": "pagination",
+          "count": 1,
+          "data": [experiment1.to_json()],
+          "paging": {"after": "2"},
+        },
+        bound_endpoint,
+        {},
+      ).iterate_pages()
+    ) == [experiment1]
     assert len(bound_endpoint.mock_calls) == 0
 
   def test_retrieve_params(self, bound_endpoint, forward_paging):
     self.make_call(
-      retrieve_params={'state': 'all'},
+      retrieve_params={"state": "all"},
       paging=forward_paging,
       bound_endpoint=bound_endpoint,
     )
     assert len(bound_endpoint.mock_calls) == 1
-    assert bound_endpoint.call_args[1]['state'] == 'all'
+    assert bound_endpoint.call_args[1]["state"] == "all"
 
   def test_iterate_pages_before_returns_before(self, bound_endpoint):
     self.make_call(
-      retrieve_params={'before': '888'},
-      paging={'before': '1', 'after': None},
+      retrieve_params={"before": "888"},
+      paging={"before": "1", "after": None},
       bound_endpoint=bound_endpoint,
     )
     assert len(bound_endpoint.mock_calls) == 1
-    assert bound_endpoint.call_args[1].get('before') == '1'
-    assert bound_endpoint.call_args[1].get('after') is None
+    assert bound_endpoint.call_args[1].get("before") == "1"
+    assert bound_endpoint.call_args[1].get("after") is None
 
   def test_iterate_pages_before_returns_after(self, bound_endpoint):
     self.make_call(
-      retrieve_params={'before': '888'},
-      paging={'before': None, 'after': '2'},
+      retrieve_params={"before": "888"},
+      paging={"before": None, "after": "2"},
       bound_endpoint=bound_endpoint,
     )
     assert len(bound_endpoint.mock_calls) == 0
 
   def test_iterate_pages_before_returns_both(self, bound_endpoint):
     self.make_call(
-      retrieve_params={'before': '888'},
-      paging={'before': '1', 'after': '2'},
+      retrieve_params={"before": "888"},
+      paging={"before": "1", "after": "2"},
       bound_endpoint=bound_endpoint,
     )
-    assert bound_endpoint.call_args[1].get('before') == '1'
-    assert bound_endpoint.call_args[1].get('after') is None
+    assert bound_endpoint.call_args[1].get("before") == "1"
+    assert bound_endpoint.call_args[1].get("after") is None
 
   def test_iterate_pages_after_returns_before(self, bound_endpoint):
     self.make_call(
-      retrieve_params={'after': '999'},
-      paging={'before': '1', 'after': None},
+      retrieve_params={"after": "999"},
+      paging={"before": "1", "after": None},
       bound_endpoint=bound_endpoint,
     )
     assert len(bound_endpoint.mock_calls) == 0
 
   def test_iterate_pages_after_returns_after(self, bound_endpoint):
     self.make_call(
-      retrieve_params={'after': '999'},
-      paging={'before': None, 'after': '2'},
+      retrieve_params={"after": "999"},
+      paging={"before": None, "after": "2"},
       bound_endpoint=bound_endpoint,
     )
     assert len(bound_endpoint.mock_calls) == 1
-    assert bound_endpoint.call_args[1].get('before') is None
-    assert bound_endpoint.call_args[1].get('after') == '2'
+    assert bound_endpoint.call_args[1].get("before") is None
+    assert bound_endpoint.call_args[1].get("after") == "2"
 
   def test_iterate_pages_after_returns_both(self, bound_endpoint):
     self.make_call(
-      retrieve_params={'after': '999'},
-      paging={'before': '1', 'after': '2'},
+      retrieve_params={"after": "999"},
+      paging={"before": "1", "after": "2"},
       bound_endpoint=bound_endpoint,
     )
     assert len(bound_endpoint.mock_calls) == 1
-    assert bound_endpoint.call_args[1].get('before') is None
-    assert bound_endpoint.call_args[1].get('after') == '2'
+    assert bound_endpoint.call_args[1].get("before") is None
+    assert bound_endpoint.call_args[1].get("after") == "2"
 
   def test_iterate_pages_before_after_returns_before(self, bound_endpoint):
     self.make_call(
-      retrieve_params={'before': '999', 'after': '888'},
-      paging={'before': '1', 'after': None},
+      retrieve_params={"before": "999", "after": "888"},
+      paging={"before": "1", "after": None},
       bound_endpoint=bound_endpoint,
     )
     assert len(bound_endpoint.mock_calls) == 1
-    assert bound_endpoint.call_args[1].get('before') == '1'
-    assert bound_endpoint.call_args[1].get('after') is None
+    assert bound_endpoint.call_args[1].get("before") == "1"
+    assert bound_endpoint.call_args[1].get("after") is None
 
   def test_iterate_pages_before_after_returns_after(self, bound_endpoint):
     self.make_call(
-      retrieve_params={'before': '999', 'after': '888'},
-      paging={'before': None, 'after': '2'},
+      retrieve_params={"before": "999", "after": "888"},
+      paging={"before": None, "after": "2"},
       bound_endpoint=bound_endpoint,
     )
     assert len(bound_endpoint.mock_calls) == 0
 
   def test_iterate_pages_before_after_returns_both(self, bound_endpoint):
     self.make_call(
-      retrieve_params={'before': '999', 'after': '888'},
-      paging={'before': '1', 'after': '2'},
+      retrieve_params={"before": "999", "after": "888"},
+      paging={"before": "1", "after": "2"},
       bound_endpoint=bound_endpoint,
     )
     assert len(bound_endpoint.mock_calls) == 1
-    assert bound_endpoint.call_args[1].get('before') == '1'
-    assert bound_endpoint.call_args[1].get('after') is None
+    assert bound_endpoint.call_args[1].get("before") == "1"
+    assert bound_endpoint.call_args[1].get("after") is None
 
   def test_lazy_iterator(self, experiment1, bound_endpoint, forward_paging):
-    iterator = Pagination(Experiment, {
-      'object': 'pagination',
-      'count': 1,
-      'data': [experiment1.to_json()],
-      'paging': forward_paging,
-    }, bound_endpoint, {}).iterate_pages()
+    iterator = Pagination(
+      Experiment,
+      {
+        "object": "pagination",
+        "count": 1,
+        "data": [experiment1.to_json()],
+        "paging": forward_paging,
+      },
+      bound_endpoint,
+      {},
+    ).iterate_pages()
     assert len(bound_endpoint.mock_calls) == 0
     list(iterator)
     assert len(bound_endpoint.mock_calls) == 1
 
   def test_paging_before_precedence_rules_forward(self, experiment1, bound_endpoint, forward_paging):
-    list(Pagination(Experiment, {
-      'object': 'pagination',
-      'count': 1,
-      'data': [experiment1.to_json()],
-      'paging': forward_paging,
-    }, bound_endpoint, {'before': '1'}).iterate_pages())
+    list(
+      Pagination(
+        Experiment,
+        {
+          "object": "pagination",
+          "count": 1,
+          "data": [experiment1.to_json()],
+          "paging": forward_paging,
+        },
+        bound_endpoint,
+        {"before": "1"},
+      ).iterate_pages()
+    )
     assert len(bound_endpoint.mock_calls) == 1
-    assert bound_endpoint.call_args[1]['before'] == '1'
-    assert 'after' not in bound_endpoint.call_args[1]
+    assert bound_endpoint.call_args[1]["before"] == "1"
+    assert "after" not in bound_endpoint.call_args[1]
 
   def test_paging_before_precedence_rules_backward(self, experiment1, bound_endpoint):
-    list(Pagination(Experiment, {
-      'object': 'pagination',
-      'count': 1,
-      'data': [experiment1.to_json()],
-      'paging': {'after': '2'},
-    }, bound_endpoint, {'before': '1'}).iterate_pages())
+    list(
+      Pagination(
+        Experiment,
+        {
+          "object": "pagination",
+          "count": 1,
+          "data": [experiment1.to_json()],
+          "paging": {"after": "2"},
+        },
+        bound_endpoint,
+        {"before": "1"},
+      ).iterate_pages()
+    )
     assert len(bound_endpoint.mock_calls) == 0
 
   def test_paging_after_precedence_rules_forward(self, experiment1, bound_endpoint):
-    list(Pagination(Experiment, {
-      'object': 'pagination',
-      'count': 1,
-      'data': [experiment1.to_json()],
-      'paging': {'before': '1'},
-    }, bound_endpoint, {'after': '2'}).iterate_pages())
+    list(
+      Pagination(
+        Experiment,
+        {
+          "object": "pagination",
+          "count": 1,
+          "data": [experiment1.to_json()],
+          "paging": {"before": "1"},
+        },
+        bound_endpoint,
+        {"after": "2"},
+      ).iterate_pages()
+    )
     assert len(bound_endpoint.mock_calls) == 0
 
   def test_paging_after_precedence_rules_backward(self, experiment1, bound_endpoint, backward_paging):
-    list(Pagination(Experiment, {
-      'object': 'pagination',
-      'count': 1,
-      'data': [experiment1.to_json()],
-      'paging': backward_paging,
-    }, bound_endpoint, {'after': '2'}).iterate_pages())
+    list(
+      Pagination(
+        Experiment,
+        {
+          "object": "pagination",
+          "count": 1,
+          "data": [experiment1.to_json()],
+          "paging": backward_paging,
+        },
+        bound_endpoint,
+        {"after": "2"},
+      ).iterate_pages()
+    )
     assert len(bound_endpoint.mock_calls) == 1
-    assert 'before' not in bound_endpoint.call_args[1]
-    assert bound_endpoint.call_args[1]['after'] == '2'
+    assert "before" not in bound_endpoint.call_args[1]
+    assert bound_endpoint.call_args[1]["after"] == "2"
 
   def test_paging_before_and_after_precedence_rules(self, experiment1, bound_endpoint):
-    list(Pagination(Experiment, {
-      'object': 'pagination',
-      'count': 1,
-      'data': [experiment1.to_json()],
-      'paging': {'before': '1', 'after': '2'},
-    }, bound_endpoint, {}).iterate_pages())
+    list(
+      Pagination(
+        Experiment,
+        {
+          "object": "pagination",
+          "count": 1,
+          "data": [experiment1.to_json()],
+          "paging": {"before": "1", "after": "2"},
+        },
+        bound_endpoint,
+        {},
+      ).iterate_pages()
+    )
     assert len(bound_endpoint.mock_calls) == 1
-    assert bound_endpoint.call_args[1]['before'] == '1'
-    assert 'after' not in bound_endpoint.call_args[1]
+    assert bound_endpoint.call_args[1]["before"] == "1"
+    assert "after" not in bound_endpoint.call_args[1]
```

### Comparing `sigopt-8.8.0/test/client/test_request_driver.py` & `sigopt-8.8.1/test/client/test_request_driver.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.0/test/client/test_requestor.py` & `sigopt-8.8.1/test/client/test_requestor.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,33 +13,35 @@
     self.response = response
 
   def __getattr__(self, name):
     def func(*args, **kwargs):
       if isinstance(self.response, Exception):
         raise self.response
       return self.response
+
     func.__name__ = name
     return func
 
 
-MESSAGE = 'This is an exception message.'
+MESSAGE = "This is an exception message."
 
 SAMPLE_EXCEPTION = {
-  'message': MESSAGE,
+  "message": MESSAGE,
 }
 
 SAMPLE_RESPONSE = {
-  'number': 1.2,
-  'string': 'abc',
-  'list': [1, 2, 3],
-  'object': {
-    'key': 'value',
-  }
+  "number": 1.2,
+  "string": "abc",
+  "list": [1, 2, 3],
+  "object": {
+    "key": "value",
+  },
 }
 
+
 class TestRequestor(object):
   def returns(self, response):
     return MockRequestor(response)
 
   def test_ok(self):
     connection = ConnectionImpl(self.returns(SAMPLE_RESPONSE))
     assert connection.experiments(1).fetch() == Experiment(SAMPLE_RESPONSE)
@@ -61,35 +63,35 @@
     assert connection.experiments(1).fetch() is None
 
   def test_client_error(self):
     connection = ConnectionImpl(self.returns(ApiException(SAMPLE_RESPONSE, 400)))
     with pytest.raises(ApiException) as e:
       connection.experiments(1).fetch()
     e = e.value
-    assert str(e) == 'ApiException (400): '
+    assert str(e) == "ApiException (400): "
     assert e.status_code == 400
     assert e.to_json() == SAMPLE_RESPONSE
 
   def test_client_error_message(self):
     connection = ConnectionImpl(self.returns(ApiException(SAMPLE_EXCEPTION, 400)))
     with pytest.raises(ApiException) as e:
       connection.experiments(1).fetch()
     e = e.value
-    assert str(e) == 'ApiException (400): ' + MESSAGE
+    assert str(e) == "ApiException (400): " + MESSAGE
     assert e.status_code == 400
     assert e.to_json() == SAMPLE_EXCEPTION
 
   def test_server_error(self):
     connection = ConnectionImpl(self.returns(ApiException(SAMPLE_EXCEPTION, status_code=500)))
     with pytest.raises(ApiException) as e:
       connection.experiments(1).fetch()
     e = e.value
-    assert str(e) == 'ApiException (500): ' + MESSAGE
+    assert str(e) == "ApiException (500): " + MESSAGE
     assert e.status_code == 500
     assert e.to_json() == SAMPLE_EXCEPTION
 
   def test_connection_error(self):
-    connection = ConnectionImpl(self.returns(ConnectionException('fake connection exception')))
+    connection = ConnectionImpl(self.returns(ConnectionException("fake connection exception")))
     with pytest.raises(ConnectionException) as e:
       connection.experiments(1).fetch()
     e = e.value
-    assert str(e) == 'ConnectionException: fake connection exception'
+    assert str(e) == "ConnectionException: fake connection exception"
```

### Comparing `sigopt-8.8.0/test/client/test_resource.py` & `sigopt-8.8.1/test/client/test_resource.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 import pytest
+
 from sigopt.endpoint import BoundApiEndpoint
 from sigopt.interface import ConnectionImpl
 from sigopt.resource import BoundApiResource, PartiallyBoundApiResource
 
 
 class TestResource(object):
   @pytest.fixture
@@ -28,9 +29,12 @@
     assert isinstance(partially_bound_api_resource(1), BoundApiResource)
 
   def test_bind_endpoint(self, connection):
     assert isinstance(connection.experiments().fetch, BoundApiEndpoint)
     assert isinstance(connection.experiments(1).fetch, BoundApiEndpoint)
 
   def test_get_bound_entity(self, connection):
-    assert isinstance(connection.experiments().get_bound_entity('fetch'), BoundApiEndpoint)
-    assert isinstance(connection.experiments().get_bound_entity('observations'), PartiallyBoundApiResource)
+    assert isinstance(connection.experiments().get_bound_entity("fetch"), BoundApiEndpoint)
+    assert isinstance(
+      connection.experiments().get_bound_entity("observations"),
+      PartiallyBoundApiResource,
+    )
```

### Comparing `sigopt-8.8.0/test/client/test_urllib3_patch.py` & `sigopt-8.8.1/test/client/test_urllib3_patch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 import pytest
 
 from sigopt.urllib3_patch import ExpiringHTTPConnectionPool, ExpiringHTTPSConnectionPool
 
+
 @pytest.mark.parametrize("pool_cls", [ExpiringHTTPConnectionPool, ExpiringHTTPSConnectionPool])
 def test_pool_reuses_connections(pool_cls):
   pool = pool_cls(host="sigopt.com", expiration_seconds=30)
   conn1 = pool._get_conn()
   pool._put_conn(conn1)
   conn2 = pool._get_conn()
   assert conn1 is conn2
 
+
 @pytest.mark.parametrize("pool_cls", [ExpiringHTTPConnectionPool, ExpiringHTTPSConnectionPool])
 def test_pool_expires_connections(pool_cls):
   pool = pool_cls(host="sigopt.com", expiration_seconds=0)
   conn1 = pool._get_conn()
   pool._put_conn(conn1)
   conn2 = pool._get_conn()
   assert conn1 is not conn2
```

### Comparing `sigopt-8.8.0/test/orchestrate/aws/service_test.py` & `sigopt-8.8.1/test/orchestrate/aws/service_test.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,66 +11,78 @@
   @pytest.fixture()
   def aws_service(self):
     services = Mock()
     aws_services = Mock()
     return AwsService(services, aws_services)
 
   def test_gpu_instance_type(self):
-    assert is_cuda_gpu_instance_type('p4d.24xlarge')
-    assert is_cuda_gpu_instance_type('p3.2xlarge')
-    assert is_cuda_gpu_instance_type('p3dn.24xlarge')
-    assert is_cuda_gpu_instance_type('p2.16xlarge')
-    assert is_cuda_gpu_instance_type('g4dn.xlarge')
-    assert is_cuda_gpu_instance_type('g4dn.metal')
-    assert is_cuda_gpu_instance_type('g3.16xlarge')
-
-    assert not is_cuda_gpu_instance_type('g4ad.16xlarge')
-    assert not is_cuda_gpu_instance_type('f1.16xlarge')
-    assert not is_cuda_gpu_instance_type('c5.24xlarge')
-    assert not is_cuda_gpu_instance_type('t2.small')
+    assert is_cuda_gpu_instance_type("p4d.24xlarge")
+    assert is_cuda_gpu_instance_type("p3.2xlarge")
+    assert is_cuda_gpu_instance_type("p3dn.24xlarge")
+    assert is_cuda_gpu_instance_type("p2.16xlarge")
+    assert is_cuda_gpu_instance_type("g4dn.xlarge")
+    assert is_cuda_gpu_instance_type("g4dn.metal")
+    assert is_cuda_gpu_instance_type("g3.16xlarge")
+
+    assert not is_cuda_gpu_instance_type("g4ad.16xlarge")
+    assert not is_cuda_gpu_instance_type("f1.16xlarge")
+    assert not is_cuda_gpu_instance_type("c5.24xlarge")
+    assert not is_cuda_gpu_instance_type("t2.small")
 
   @pytest.fixture
   def cpu_config(self):
     return {"min_size": 1, "max_size": 2, "instance_type": "m5.large"}
 
   @pytest.fixture
   def gpu_config(self):
     return {"min_size": 1, "max_size": 2, "instance_type": "p3.2xlarge"}
 
-  @pytest.mark.parametrize('cluster_name', [
-    '',
-    'inval_id1-123',
-    'also-invalid_cluster-name',
-    '123',
-  ])
+  @pytest.mark.parametrize(
+    "cluster_name",
+    [
+      "",
+      "inval_id1-123",
+      "also-invalid_cluster-name",
+      "123",
+    ],
+  )
   def test_invalid_cluster_name(self, aws_service, cluster_name, cpu_config, gpu_config):
     with pytest.raises(AssertionError):
       aws_service.validate_cluster_options(cluster_name, {"cpu": cpu_config, "gpu": gpu_config}, None)
 
-  @pytest.mark.parametrize('cluster_name', [
-    'valid-123',
-    'also-valid-cluster-name',
-  ])
+  @pytest.mark.parametrize(
+    "cluster_name",
+    [
+      "valid-123",
+      "also-valid-cluster-name",
+    ],
+  )
   def test_valid_cluster_names(self, aws_service, cluster_name, cpu_config, gpu_config):
     aws_service.validate_cluster_options(cluster_name, {"cpu": cpu_config, "gpu": gpu_config}, None)
 
-  @pytest.mark.parametrize('kubernetes_version', [
-    '1.9',
-    '1.15',
-    'not-a-version',
-  ])
+  @pytest.mark.parametrize(
+    "kubernetes_version",
+    [
+      "1.9",
+      "1.15",
+      "not-a-version",
+    ],
+  )
   def test_invalid_kubernetes_version(self, aws_service, kubernetes_version, cpu_config, gpu_config):
     with pytest.raises(AssertionError):
-      aws_service.validate_cluster_options('cluster-name', {"cpu": cpu_config, "gpu": gpu_config}, kubernetes_version)
+      aws_service.validate_cluster_options("cluster-name", {"cpu": cpu_config, "gpu": gpu_config}, kubernetes_version)
 
-  @pytest.mark.parametrize('kubernetes_version', [
-    None,
-    '1.20',
-    '1.23',
-    'latest',
-  ])
+  @pytest.mark.parametrize(
+    "kubernetes_version",
+    [
+      None,
+      "1.20",
+      "1.23",
+      "latest",
+    ],
+  )
   def test_valid_kubernetes_versions(self, aws_service, kubernetes_version, cpu_config, gpu_config):
-    aws_service.validate_cluster_options('valid-name', {"cpu": cpu_config, "gpu": gpu_config}, kubernetes_version)
+    aws_service.validate_cluster_options("valid-name", {"cpu": cpu_config, "gpu": gpu_config}, kubernetes_version)
 
   def test_create_kubernetes_cluster_fail(self, aws_service, cpu_config, gpu_config):
     with pytest.raises(AssertionError):
       aws_service.create_kubernetes_cluster(dict(cluster_name="44_44", cpu=cpu_config, gpu=gpu_config))
```

### Comparing `sigopt-8.8.0/test/orchestrate/cluster/service_test.py` & `sigopt-8.8.1/test/orchestrate/cluster/service_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,24 +17,26 @@
 from sigopt.orchestrate.provider.constants import Provider
 
 
 class TestClusterService(object):
   @pytest.fixture
   def services(self):
     mock_services = Mock()
-    mock_services.get_option = Mock(return_value='bar')
+    mock_services.get_option = Mock(return_value="bar")
 
     def fake_get_provider_service(provider):
       if provider == Provider.AWS:
         return Mock(
-          create_kubernetes_cluster=Mock(return_value=AWSCluster(
-            services=mock_services,
-            name='foobar',
-            registry=None,
-          ))
+          create_kubernetes_cluster=Mock(
+            return_value=AWSCluster(
+              services=mock_services,
+              name="foobar",
+              registry=None,
+            )
+          )
         )
       elif provider == Provider.CUSTOM:
         return CustomClusterService(mock_services)
       else:
         raise NotImplementedError()
 
     mock_services.provider_broker.get_provider_service = fake_get_provider_service
@@ -45,189 +47,192 @@
     cluster_service = ClusterService(services)
     services.cluster_service = cluster_service
     return cluster_service
 
   def test_connected_clusters(self, cluster_service):
     cluster_service.services.kubernetes_service.get_cluster_names.return_value = []
     assert cluster_service.connected_clusters() == []
-    cluster_service.services.kubernetes_service.get_cluster_names.return_value = ['foo']
-    assert cluster_service.connected_clusters() == ['foo']
-    cluster_service.services.kubernetes_service.get_cluster_names.return_value = ['foo', 'bar']
-    assert sorted(cluster_service.connected_clusters()) == ['bar', 'foo']
+    cluster_service.services.kubernetes_service.get_cluster_names.return_value = ["foo"]
+    assert cluster_service.connected_clusters() == ["foo"]
+    cluster_service.services.kubernetes_service.get_cluster_names.return_value = [
+      "foo",
+      "bar",
+    ]
+    assert sorted(cluster_service.connected_clusters()) == ["bar", "foo"]
 
   def test_multiple_clusters(self, cluster_service):
-    cluster_service.connected_clusters = Mock(return_value=['bar', 'foo'])
+    cluster_service.connected_clusters = Mock(return_value=["bar", "foo"])
 
     with pytest.raises(MultipleClustersConnectionError):
       cluster_service.assert_is_connected()
     with pytest.raises(MultipleClustersConnectionError):
       cluster_service.assert_is_disconnected()
     with pytest.raises(MultipleClustersConnectionError):
       cluster_service.connect(
         cluster_name=None,
-        provider_string='aws',
+        provider_string="aws",
         kubeconfig=None,
         registry=None,
       )
     with pytest.raises(MultipleClustersConnectionError):
       cluster_service.create(None)
     with pytest.raises(MultipleClustersConnectionError):
-      cluster_service.disconnect('bar', None)
+      cluster_service.disconnect("bar", None)
     with pytest.raises(MultipleClustersConnectionError):
       cluster_service.test()
 
     cluster_service.disconnect(cluster_name=None, disconnect_all=True)
 
-    # TODO(alexandra): decide which permissions to validate for cluster destroy
-    cluster_service.destroy(None, 'aws')
+    # TODO: decide which permissions to validate for cluster destroy
+    cluster_service.destroy(None, "aws")
 
   def test_no_clusters(self, cluster_service):
     cluster_service.connected_clusters = Mock(return_value=[])
 
     with pytest.raises(NotConnectedError):
       cluster_service.assert_is_connected()
     with pytest.raises(NotConnectedError):
-      cluster_service.disconnect('bar', None)
+      cluster_service.disconnect("bar", None)
     with pytest.raises(NotConnectedError):
       cluster_service.disconnect(cluster_name=None, disconnect_all=True)
     with pytest.raises(NotConnectedError):
       cluster_service.test()
 
     cluster_service.assert_is_disconnected()
     cluster_service.test = Mock()
     cluster_service.connect(
-      cluster_name='cluster_name',
-      provider_string='aws',
+      cluster_name="cluster_name",
+      provider_string="aws",
       kubeconfig=None,
       registry=None,
     )
     assert cluster_service.test.call_count == 1
-    cluster_service.create(dict(provider='aws'))
+    cluster_service.create(dict(provider="aws"))
 
-    # TODO(alexandra): decide which permissions to validate for cluster destroy
-    cluster_service.destroy(None, 'aws')
+    # TODO: decide which permissions to validate for cluster destroy
+    cluster_service.destroy(None, "aws")
 
   def test_one_clusters(self, cluster_service):
-    cluster_service.connected_clusters = Mock(return_value=['foo'])
+    cluster_service.connected_clusters = Mock(return_value=["foo"])
     cluster_service.services.cluster_metadata_service.read_metadata = Mock(
       return_value=CustomCluster(
         services=cluster_service.services,
-        name='foo',
+        name="foo",
         registry=None,
       )
     )
 
     with pytest.raises(PleaseDisconnectError):
       cluster_service.assert_is_disconnected()
     with pytest.raises(PleaseDisconnectError):
       cluster_service.connect(
-        cluster_name='bar',
-        provider_string='aws',
+        cluster_name="bar",
+        provider_string="aws",
         kubeconfig=None,
         registry=None,
       )
     with pytest.raises(PleaseDisconnectError):
-      cluster_service.create(dict(cluster_name='bar'))
+      cluster_service.create(dict(cluster_name="bar"))
     with pytest.raises(PleaseDisconnectError):
-      cluster_service.disconnect('bar', None)
+      cluster_service.disconnect("bar", None)
 
     cluster_service.assert_is_connected()
 
     with pytest.raises(AlreadyConnectedException):
       cluster_service.connect(
-        cluster_name='foo',
-        provider_string='aws',
+        cluster_name="foo",
+        provider_string="aws",
         kubeconfig=None,
         registry=None,
       )
     with pytest.raises(AlreadyConnectedException):
-      cluster_service.create(dict(cluster_name='foo'))
+      cluster_service.create(dict(cluster_name="foo"))
 
-    cluster_service.disconnect('foo', None)
+    cluster_service.disconnect("foo", None)
     cluster_service.disconnect(cluster_name=None, disconnect_all=True)
-    cluster_service.destroy('foo', 'aws')
+    cluster_service.destroy("foo", "aws")
     cluster_service.test()
 
-    # TODO(alexandra): decide which permissions to validate for cluster destroy
-    cluster_service.destroy('bar', 'aws')
+    # TODO: decide which permissions to validate for cluster destroy
+    cluster_service.destroy("bar", "aws")
 
   def test_create_cluster(self, cluster_service):
     cluster_service.connected_clusters = Mock(return_value=[])
-    cluster_name = cluster_service.create(dict(provider='aws'))
-    assert cluster_name == 'foobar'
+    cluster_name = cluster_service.create(dict(provider="aws"))
+    assert cluster_name == "foobar"
 
   def test_create_cluster_fails(self, cluster_service):
     # Mock this function so that cluster create things that we are not connected, and will try to creat a cluster
     cluster_service.assert_is_disconnected = Mock()
     # Mock this function so that cluster disconnect will think that we are connected to foobar
-    cluster_service.connected_clusters = Mock(return_value=['foobar'])
+    cluster_service.connected_clusters = Mock(return_value=["foobar"])
 
     exc = Exception()
     cluster_service.services.provider_broker.get_provider_service = Mock(
       return_value=Mock(
         create_kubernetes_cluster=Mock(side_effect=exc),
       ),
     )
     with pytest.raises(Exception) as e:
-      cluster_service.create(dict(cluster_name='foobar', provider='aws'))
+      cluster_service.create(dict(cluster_name="foobar", provider="aws"))
     assert e.value is exc
-    cluster_service.services.kubernetes_service.ensure_config_deleted.assert_called_with(cluster_name='foobar')
+    cluster_service.services.kubernetes_service.ensure_config_deleted.assert_called_with(cluster_name="foobar")
 
   def test_cluster_test(self, cluster_service):
-    cluster_service.connected_clusters = Mock(return_value=['foobar'])
+    cluster_service.connected_clusters = Mock(return_value=["foobar"])
     cluster_service.services.cluster_metadata_service.read_metadata = Mock(
       return_value=CustomCluster(
         services=cluster_service.services,
-        name='foobar',
+        name="foobar",
         registry=None,
       )
     )
 
     cluster = cluster_service.test()
-    assert cluster.name == 'foobar'
-    assert cluster.provider_string == 'custom'
+    assert cluster.name == "foobar"
+    assert cluster.provider_string == "custom"
 
-    cluster_service.connected_clusters = Mock(return_value=['bar'])
+    cluster_service.connected_clusters = Mock(return_value=["bar"])
     cluster_service.services.cluster_metadata_service.read_metadata = Mock(
       return_value=AWSCluster(
         services=cluster_service.services,
-        name='bar',
+        name="bar",
         registry=None,
       )
     )
 
     cluster = cluster_service.test()
-    assert cluster.name == 'bar'
-    assert cluster.provider_string == 'aws'
+    assert cluster.name == "bar"
+    assert cluster.provider_string == "aws"
 
   def test_cluster_connect(self, cluster_service):
     cluster_service.connected_clusters = Mock(return_value=[])
     cluster_service.test = Mock()
     cluster_service.connect(
-      cluster_name='bar',
-      provider_string='custom',
-      kubeconfig='foo',
+      cluster_name="bar",
+      provider_string="custom",
+      kubeconfig="foo",
       registry=None,
     )
 
     cluster_service.connect(
-      cluster_name='bar',
-      provider_string='aws',
+      cluster_name="bar",
+      provider_string="aws",
       kubeconfig=None,
       registry=None,
     )
 
     with pytest.raises(AssertionError):
       cluster_service.connect(
-        cluster_name='bar',
-        provider_string='aws',
-        kubeconfig='foo',
+        cluster_name="bar",
+        provider_string="aws",
+        kubeconfig="foo",
         registry=None,
       )
 
     with pytest.raises(OrchestrateException):
       cluster_service.connect(
-        cluster_name='bar',
-        provider_string='custom',
+        cluster_name="bar",
+        provider_string="custom",
         kubeconfig=None,
         registry=None,
       )
```

### Comparing `sigopt-8.8.0/test/orchestrate/cluster_metadata/service_test.py` & `sigopt-8.8.1/test/orchestrate/cluster_metadata/service_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,88 +1,90 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 import pytest
 from mock import Mock
 
-from sigopt.orchestrate.common import TemporaryDirectory
 from sigopt.orchestrate.cluster.object import AWSCluster
 from sigopt.orchestrate.cluster_metadata.errors import *
 from sigopt.orchestrate.cluster_metadata.service import ClusterMetadataService
+from sigopt.orchestrate.common import TemporaryDirectory
 from sigopt.orchestrate.custom_cluster.service import CustomClusterService
 from sigopt.orchestrate.provider.constants import Provider
 
 
 # pylint: disable=protected-access
 
+
 class TestClusterService(object):
   @pytest.fixture
   def services(self):
     mock_services = Mock()
 
     def fake_create_cluster_object(services, name, registry):
       return AWSCluster(
         services=services,
         name=name,
         registry=registry,
       )
 
     def fake_get_provider_service(provider):
       if provider == Provider.AWS:
-        return Mock(
-          create_cluster_object=fake_create_cluster_object
-        )
+        return Mock(create_cluster_object=fake_create_cluster_object)
       elif provider == Provider.CUSTOM:
         return CustomClusterService(mock_services)
       else:
         raise NotImplementedError()
 
     mock_services.provider_broker.get_provider_service = fake_get_provider_service
     return mock_services
 
   @pytest.fixture
   def cluster_metadata_service(self, services):
     cluster_metadata_service = ClusterMetadataService(services)
     services.cluster_metadata_service = cluster_metadata_service
     return cluster_metadata_service
 
-  @pytest.mark.parametrize('provider', [
-    Provider.AWS,
-    Provider.CUSTOM,
-  ])
+  @pytest.mark.parametrize(
+    "provider",
+    [
+      Provider.AWS,
+      Provider.CUSTOM,
+    ],
+  )
   def test_custom_cluster(self, cluster_metadata_service, provider):
     with TemporaryDirectory() as root_dirname:
       cluster_metadata_service._metadata_dir = root_dirname
 
       provider_service = cluster_metadata_service.services.provider_broker.get_provider_service(provider)
       cluster = provider_service.create_cluster_object(
         services=cluster_metadata_service.services,
-        name='foobar',
+        name="foobar",
         registry=None,
       )
       cluster_metadata_service.write_metadata(cluster)
 
-      cluster = cluster_metadata_service.read_metadata('foobar')
-      assert cluster.name == 'foobar'
+      cluster = cluster_metadata_service.read_metadata("foobar")
+      assert cluster.name == "foobar"
       assert cluster.provider == provider
 
   def test_double_write(self, cluster_metadata_service):
     with TemporaryDirectory() as root_dirname:
       cluster_metadata_service._metadata_dir = root_dirname
 
       custom_cluster_service = cluster_metadata_service.services.provider_broker.get_provider_service(Provider.CUSTOM)
       cluster = custom_cluster_service.create_cluster_object(
         services=cluster_metadata_service.services,
-        name='foobar',
+        name="foobar",
         registry=None,
       )
       cluster_metadata_service.write_metadata(cluster)
 
       with pytest.raises(MetadataAlreadyExistsError):
         cluster_metadata_service.write_metadata(cluster)
 
   def test_no_metadata(self, cluster_metadata_service):
     with TemporaryDirectory() as root_dirname:
       cluster_metadata_service._metadata_dir = root_dirname
 
       with pytest.raises(Exception):
-        cluster_metadata_service.read_metadata('foobar')
+        cluster_metadata_service.read_metadata("foobar")
```

### Comparing `sigopt-8.8.0/test/orchestrate/common_test.py` & `sigopt-8.8.1/test/orchestrate/common_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 import pytest
 from mock import patch
 
 from sigopt.orchestrate.common import Platform, current_platform
 
 
 class TestCurrentPlatform(object):
-  @pytest.mark.parametrize('platform', ['foobar.linux', 'foobar', ''])
+  @pytest.mark.parametrize("platform", ["foobar.linux", "foobar", ""])
   def test_bad_platform(self, platform):
-    with patch('sigopt.orchestrate.common.sys.platform', platform):
+    with patch("sigopt.orchestrate.common.sys.platform", platform):
       with pytest.raises(Exception):
         current_platform()
 
   def test_mac_platform(self):
-    with patch('sigopt.orchestrate.common.sys.platform', 'darwin'):
+    with patch("sigopt.orchestrate.common.sys.platform", "darwin"):
       assert current_platform() == Platform.MAC
 
-  @pytest.mark.parametrize('platform', ['linux', 'linux.foobar'])
+  @pytest.mark.parametrize("platform", ["linux", "linux.foobar"])
   def test_linux_platform(self, platform):
-    with patch('sigopt.orchestrate.common.sys.platform', platform):
+    with patch("sigopt.orchestrate.common.sys.platform", platform):
       assert current_platform() == Platform.LINUX
```

### Comparing `sigopt-8.8.0/test/orchestrate/gpu_options_validator/service_test.py` & `sigopt-8.8.1/test/orchestrate/gpu_options_validator/service_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,29 +10,29 @@
 class TestOptionsValidatorService(object):
   @pytest.fixture()
   def gpu_options_validator_service(self):
     services = Mock()
     return GpuOptionsValidatorService(services)
 
   @pytest.mark.parametrize(
-    'input_gpus,expected_resources',
+    "input_gpus,expected_resources",
     [
       (None, {}),
-      (0, {'gpus': 0}),
+      (0, {"gpus": 0}),
     ],
   )
   def test_get_resources_without_confirmation(
     self,
     gpu_options_validator_service,
     input_gpus,
     expected_resources,
   ):
     options = {}
     if input_gpus is not None:
-      options[RESOURCES_OPTION] = {'gpus': input_gpus}
+      options[RESOURCES_OPTION] = {"gpus": input_gpus}
     resource_options = gpu_options_validator_service.get_resource_options(options)
     assert resource_options == expected_resources
 
   def test_get_local_without_gpus(self, gpu_options_validator_service):
     options = {}
     resource_options = gpu_options_validator_service.get_resource_options(options)
     assert RESOURCES_OPTION not in resource_options
```

### Comparing `sigopt-8.8.0/test/orchestrate/kubernetes/service_test.py` & `sigopt-8.8.1/test/orchestrate/kubernetes/service_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,95 +14,92 @@
   @pytest.fixture()
   def kubernetes_service(self):
     services = Mock()
     return KubernetesService(services)
 
   def test_delete_job(self, kubernetes_service):
     kubernetes_service._v1_batch = Mock()
-    kubernetes_service.delete_job('test_job_name')
+    kubernetes_service.delete_job("test_job_name")
 
     kubernetes_service._v1_batch.delete_namespaced_job.assert_called_with(
-      'test_job_name',
+      "test_job_name",
       ORCHESTRATE_NAMESPACE,
       body=client.V1DeleteOptions(),
     )
 
   def test_start_job(self, kubernetes_service):
     kubernetes_service._v1_batch = Mock()
-    kubernetes_service.start_job('test_job_spec')
+    kubernetes_service.start_job("test_job_spec")
 
-    kubernetes_service._v1_batch.create_namespaced_job.assert_called_with(
-      ORCHESTRATE_NAMESPACE,
-      'test_job_spec'
-    )
+    kubernetes_service._v1_batch.create_namespaced_job.assert_called_with(ORCHESTRATE_NAMESPACE, "test_job_spec")
 
   def test_logs(self, kubernetes_service):
     kubernetes_service._v1_core = Mock()
-    kubernetes_service.logs('foobar')
+    kubernetes_service.logs("foobar")
 
-    kubernetes_service._v1_core.read_namespaced_pod_log.assert_called_with('foobar', ORCHESTRATE_NAMESPACE)
+    kubernetes_service._v1_core.read_namespaced_pod_log.assert_called_with("foobar", ORCHESTRATE_NAMESPACE)
 
   def test_pod_names(self, kubernetes_service):
     foo_mock = Mock()
-    foo_mock.metadata.name = 'foo'
+    foo_mock.metadata.name = "foo"
     bar_mock = Mock()
-    bar_mock.metadata.name = 'bar'
+    bar_mock.metadata.name = "bar"
 
     get_pods_result = MagicMock()
     get_pods_result.items = [foo_mock, bar_mock]
     kubernetes_service.get_pods = Mock(return_value=get_pods_result)
 
-    assert kubernetes_service.pod_names('baz') == ['foo', 'bar']
-    kubernetes_service.get_pods.assert_called_with(job_name='baz')
+    assert kubernetes_service.pod_names("baz") == ["foo", "bar"]
+    kubernetes_service.get_pods.assert_called_with(job_name="baz")
 
   def test_get_pods(self, kubernetes_service):
     kubernetes_service._v1_core = Mock()
     kubernetes_service.get_pods()
 
     kubernetes_service._v1_core.list_namespaced_pod.assert_called_with(ORCHESTRATE_NAMESPACE, watch=False)
 
   def test_get_pods_with_job_name(self, kubernetes_service):
     kubernetes_service._v1_core = Mock()
-    kubernetes_service.get_pods('test_job_name')
+    kubernetes_service.get_pods("test_job_name")
 
     kubernetes_service._v1_core.list_namespaced_pod.assert_called_with(
-      ORCHESTRATE_NAMESPACE,
-      watch=False,
-      label_selector='job-name=test_job_name'
+      ORCHESTRATE_NAMESPACE, watch=False, label_selector="job-name=test_job_name"
     )
 
   def test_wait_until_nodes_are_ready(self, kubernetes_service):
-    with patch('sigopt.orchestrate.kubernetes.service.time') as mock_time:
-      kubernetes_service.check_nodes_are_ready = Mock(side_effect=[
-        NodesNotReadyError("not ready"),
-        NodesNotReadyError("not ready"),
-        NodesNotReadyError("not ready"),
-        None,
-        None,
-      ])
+    with patch("sigopt.orchestrate.kubernetes.service.time") as mock_time:
+      kubernetes_service.check_nodes_are_ready = Mock(
+        side_effect=[
+          NodesNotReadyError("not ready"),
+          NodesNotReadyError("not ready"),
+          NodesNotReadyError("not ready"),
+          None,
+          None,
+        ]
+      )
       kubernetes_service.wait_until_nodes_are_ready()
       assert kubernetes_service.check_nodes_are_ready.call_count == 4
       assert mock_time.sleep.called
 
   def test_check_nodes_are_ready(self, kubernetes_service):
-    ready_true_cond = Mock(status='True', type='Ready')
-    foobar_true_cond = Mock(status='True', type='foobar')
-    foobar_false_cond = Mock(status='False', type='foobar')
+    ready_true_cond = Mock(status="True", type="Ready")
+    foobar_true_cond = Mock(status="True", type="foobar")
+    foobar_false_cond = Mock(status="False", type="foobar")
 
     node_mock1 = Mock(status=Mock(conditions=[ready_true_cond, foobar_true_cond]))
     node_mock2 = Mock(status=Mock(conditions=[ready_true_cond, foobar_false_cond]))
 
     kubernetes_service.get_nodes = MagicMock()
     kubernetes_service.get_nodes().items = [node_mock1, node_mock2]
 
     kubernetes_service.check_nodes_are_ready()
 
   def test_check_nodes_are_not_ready_status(self, kubernetes_service):
-    ready_false_cond = Mock(status='False', type='Ready')
-    foobar_true_cond = Mock(status='True', type='foobar')
+    ready_false_cond = Mock(status="False", type="Ready")
+    foobar_true_cond = Mock(status="True", type="foobar")
 
     node_mock1 = Mock(status=Mock(conditions=[ready_false_cond, foobar_true_cond]))
     node_mock2 = Mock(status=Mock(conditions=[ready_false_cond, foobar_true_cond]))
 
     kubernetes_service.get_nodes = MagicMock()
     kubernetes_service.get_nodes().items = [node_mock1, node_mock2]
 
@@ -119,13 +116,15 @@
   def test_get_nodes(self, kubernetes_service):
     kubernetes_service._v1_core = Mock()
     kubernetes_service.get_nodes()
 
     kubernetes_service._v1_core.list_node.assert_called_with()
 
   def test_get_cluster_names(self, kubernetes_service):
-    kubernetes_service._get_config_files = MagicMock(return_value=['config-test-cluster'])
-    assert kubernetes_service.get_cluster_names() == ['test-cluster']
+    kubernetes_service._get_config_files = MagicMock(return_value=["config-test-cluster"])
+    assert kubernetes_service.get_cluster_names() == ["test-cluster"]
 
     kubernetes_service._get_config_files = MagicMock(return_value=[])
     assert kubernetes_service.get_cluster_names() == []
+
+
 # pylint: enable=protected-access
```

### Comparing `sigopt-8.8.0/test/orchestrate/lib/lists_test.py` & `sigopt-8.8.1/test/orchestrate/lib/lists_test.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,55 +4,47 @@
 from sigopt.orchestrate.lib.lists import *
 
 
 class TestLists(object):
   def test_remove_nones(self):
     assert remove_nones([]) == []
     assert remove_nones([False, None, [], 0, {}]) == [False, [], 0, {}]
-    assert remove_nones([False, None, [], 0, {}, 1, 2, 3, True, [1]]) == [False, [], 0, {}, 1, 2, 3, True, [1]]
+    assert remove_nones([False, None, [], 0, {}, 1, 2, 3, True, [1]]) == [
+      False,
+      [],
+      0,
+      {},
+      1,
+      2,
+      3,
+      True,
+      [1],
+    ]
     assert remove_nones({}) == {}
-    assert remove_nones({
-      'a': False,
-      'b': None,
-      'c': [],
-      'd': 0,
-      'e': {},
-    }) == {
-      'a': False,
-      'c': [],
-      'd': 0,
-      'e': {},
+    assert remove_nones({"a": False, "b": None, "c": [], "d": 0, "e": {},}) == {
+      "a": False,
+      "c": [],
+      "d": 0,
+      "e": {},
     }
-    assert remove_nones({
-      'a': False,
-      'b': None,
-      'c': [],
-      'd': 0,
-      'e': {},
-      'f': 1,
-      'g': True,
-    }) == {
-      'a': False,
-      'c': [],
-      'd': 0,
-      'e': {},
-      'f': 1,
-      'g': True,
+    assert remove_nones({"a": False, "b": None, "c": [], "d": 0, "e": {}, "f": 1, "g": True,}) == {
+      "a": False,
+      "c": [],
+      "d": 0,
+      "e": {},
+      "f": 1,
+      "g": True,
     }
-    assert remove_nones({
-      'a': {
-        'b': None,
-      },
-    }) == {
-      'a': {
-        'b': None,
+    assert remove_nones({"a": {"b": None,},}) == {
+      "a": {
+        "b": None,
       },
     }
-    assert remove_nones(set((1, 'a', None))) == set((1, 'a'))
-    assert remove_nones(set((1, 'a'))) == set((1, 'a'))
+    assert remove_nones(set((1, "a", None))) == set((1, "a"))
+    assert remove_nones(set((1, "a"))) == set((1, "a"))
     assert remove_nones(set()) == set()
 
   def test_coalesce(self):
     assert coalesce() is None
     assert coalesce(None) is None
     assert coalesce(None, None) is None
     assert coalesce(None, None, None) is None
```

### Comparing `sigopt-8.8.0/test/orchestrate/lib/types_test.py` & `sigopt-8.8.1/test/orchestrate/lib/types_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,89 +12,89 @@
     assert is_sequence((1, 2, 3))
 
     assert not is_sequence(None)
     assert not is_sequence(False)
     assert not is_sequence(True)
     assert not is_sequence(0)
     assert not is_sequence(1.0)
-    assert not is_sequence('abc')
+    assert not is_sequence("abc")
     assert not is_sequence({})
-    assert not is_sequence({'a': 123})
+    assert not is_sequence({"a": 123})
     assert not is_sequence(set())
-    assert not is_sequence(set((1, 'a')))
-    assert not is_sequence({1, 'a'})
-    assert not is_sequence(frozenset((1, 'a')))
+    assert not is_sequence(set((1, "a")))
+    assert not is_sequence({1, "a"})
+    assert not is_sequence(frozenset((1, "a")))
 
   def test_is_string_sequence(self):
     assert is_string_sequence([])
     assert is_string_sequence(())
-    assert is_string_sequence(('a', 'b', 'c'))
-    assert is_string_sequence([''])
-    assert is_string_sequence(['a'])
-    assert is_string_sequence(['a', '', 'b'])
+    assert is_string_sequence(("a", "b", "c"))
+    assert is_string_sequence([""])
+    assert is_string_sequence(["a"])
+    assert is_string_sequence(["a", "", "b"])
 
     assert not is_string_sequence(None)
     assert not is_string_sequence(True)
     assert not is_string_sequence(False)
-    assert not is_string_sequence((None, 'a', 'b'))
-    assert not is_string_sequence(['a', 1])
-    assert not is_string_sequence(['b', None])
-    assert not is_string_sequence(['a', 'b', True, 'c'])
-    assert not is_string_sequence('string')
-    assert not is_string_sequence(('a', False))
+    assert not is_string_sequence((None, "a", "b"))
+    assert not is_string_sequence(["a", 1])
+    assert not is_string_sequence(["b", None])
+    assert not is_string_sequence(["a", "b", True, "c"])
+    assert not is_string_sequence("string")
+    assert not is_string_sequence(("a", False))
 
   def test_is_mapping(self):
     assert is_mapping({})
-    assert is_mapping({'a': 123})
+    assert is_mapping({"a": 123})
 
     assert not is_mapping([])
     assert not is_mapping([1, 2, 3])
     assert not is_mapping(())
     assert not is_mapping((1, 2, 3))
     assert not is_mapping(None)
     assert not is_mapping(False)
     assert not is_mapping(True)
     assert not is_mapping(0)
     assert not is_mapping(1.0)
-    assert not is_mapping('abc')
+    assert not is_mapping("abc")
     assert not is_mapping(set())
-    assert not is_mapping(set((1, 'a')))
-    assert not is_mapping({1, 'a'})
-    assert not is_mapping(frozenset((1, 'a')))
+    assert not is_mapping(set((1, "a")))
+    assert not is_mapping({1, "a"})
+    assert not is_mapping(frozenset((1, "a")))
 
   def test_is_set(self):
     assert is_set(set())
-    assert is_set(set((1, 'a')))
-    assert is_set({1, 'a'})
-    assert is_set(frozenset((1, 'a')))
+    assert is_set(set((1, "a")))
+    assert is_set({1, "a"})
+    assert is_set(frozenset((1, "a")))
 
     assert not is_set({})
-    assert not is_set({'a': 123})
+    assert not is_set({"a": 123})
     assert not is_set([])
     assert not is_set([1, 2, 3])
     assert not is_set(())
     assert not is_set((1, 2, 3))
     assert not is_set(None)
     assert not is_set(False)
     assert not is_set(True)
     assert not is_set(0)
     assert not is_set(1.0)
-    assert not is_set('abc')
+    assert not is_set("abc")
 
   def test_is_string(self):
-    assert is_string('')
-    assert is_string('abc')
-    assert is_string('123')
+    assert is_string("")
+    assert is_string("abc")
+    assert is_string("123")
 
     assert not is_string(set())
-    assert not is_string(set((1, 'a')))
-    assert not is_string({1, 'a'})
-    assert not is_string(frozenset((1, 'a')))
+    assert not is_string(set((1, "a")))
+    assert not is_string({1, "a"})
+    assert not is_string(frozenset((1, "a")))
     assert not is_string({})
-    assert not is_string({'a': 123})
+    assert not is_string({"a": 123})
     assert not is_string([])
     assert not is_string([1, 2, 3])
     assert not is_string(())
     assert not is_string((1, 2, 3))
     assert not is_string(None)
     assert not is_string(False)
     assert not is_string(True)
@@ -103,50 +103,50 @@
 
   def test_is_integer(self):
     assert is_integer(0)
     assert is_integer(1)
     assert is_integer(-1)
 
     assert not is_integer(set())
-    assert not is_integer(set((1, 'a')))
-    assert not is_integer({1, 'a'})
-    assert not is_integer(frozenset((1, 'a')))
+    assert not is_integer(set((1, "a")))
+    assert not is_integer({1, "a"})
+    assert not is_integer(frozenset((1, "a")))
     assert not is_integer({})
-    assert not is_integer({'a': 123})
+    assert not is_integer({"a": 123})
     assert not is_integer([])
     assert not is_integer([1, 2, 3])
     assert not is_integer(())
     assert not is_integer((1, 2, 3))
     assert not is_integer(None)
     assert not is_integer(False)
     assert not is_integer(True)
     assert not is_integer(1.0)
-    assert not is_integer('')
-    assert not is_integer('abc')
-    assert not is_integer('123')
+    assert not is_integer("")
+    assert not is_integer("abc")
+    assert not is_integer("123")
 
   def test_is_boolean(self):
     assert is_boolean(True)
     assert is_boolean(False)
 
     assert not is_boolean(set())
     assert not is_boolean(set((True, False)))
     assert not is_boolean({True, False})
     assert not is_boolean(frozenset((True, False)))
     assert not is_boolean({})
-    assert not is_boolean({'a': True})
+    assert not is_boolean({"a": True})
     assert not is_boolean([])
     assert not is_boolean([True, False])
     assert not is_boolean(())
     assert not is_boolean((True, False))
-    assert not is_boolean('')
+    assert not is_boolean("")
     assert not is_boolean(None)
-    assert not is_boolean('abc')
-    assert not is_boolean('123')
-    assert not is_boolean('True')
-    assert not is_boolean('False')
-    assert not is_boolean('true')
-    assert not is_boolean('false')
+    assert not is_boolean("abc")
+    assert not is_boolean("123")
+    assert not is_boolean("True")
+    assert not is_boolean("False")
+    assert not is_boolean("true")
+    assert not is_boolean("false")
     assert not is_boolean(0)
     assert not is_boolean(1)
     assert not is_boolean(1.0)
     assert not is_boolean(-1)
```

### Comparing `sigopt-8.8.0/test/orchestrate/options_validator/service_test.py` & `sigopt-8.8.1/test/orchestrate/options_validator/service_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,312 +9,322 @@
 
 class TestOptionsValidatorService(object):
   @pytest.fixture()
   def options_validator_service(self):
     services = Mock()
     return OptionsValidatorService(services)
 
-  @pytest.mark.parametrize('resource', [
-    {'requests': {'cpu': 1, 'memory': '200Gi'}, 'gpus': 1},
-    {'limits': {'cpu': '200m', 'memory': 200}},
-    {'requests': None, 'gpus': 1},
-    {'requests': {'cpu': 1, 'memory': '200Gi'}, 'gpus': None},
-  ])
+  @pytest.mark.parametrize(
+    "resource",
+    [
+      {"requests": {"cpu": 1, "memory": "200Gi"}, "gpus": 1},
+      {"limits": {"cpu": "200m", "memory": 200}},
+      {"requests": None, "gpus": 1},
+      {"requests": {"cpu": 1, "memory": "200Gi"}, "gpus": None},
+    ],
+  )
   def test_validate_resources(self, options_validator_service, resource):
     options_validator_service.validate_resources(**resource)
 
-  @pytest.mark.parametrize('resource', [
-    {'requests': {'cpu': 1, 'memory': '200Gi'}, 'gpus': -1},
-    {'limits': {'cpu': '200m', 'memory': 200}, 'requests': 55},
-  ])
+  @pytest.mark.parametrize(
+    "resource",
+    [
+      {"requests": {"cpu": 1, "memory": "200Gi"}, "gpus": -1},
+      {"limits": {"cpu": "200m", "memory": 200}, "requests": 55},
+    ],
+  )
   def test_orchestrate_resources_bad(self, options_validator_service, resource):
     with pytest.raises(AssertionError):
       options_validator_service.validate_resources(**resource)
 
-  @pytest.mark.parametrize('gpus', [-1, [], dict()])
+  @pytest.mark.parametrize("gpus", [-1, [], dict()])
   def test_validate_resources_wrong_type(self, options_validator_service, gpus):
     with pytest.raises(AssertionError):
       options_validator_service.validate_resources(gpus=gpus)
 
   def test_validate_aws(self, options_validator_service):
     options_validator_service.validate_aws_for_orchestrate(
-      aws_access_key_id='foobar',
-      aws_secret_access_key='barfoo',
+      aws_access_key_id="foobar",
+      aws_secret_access_key="barfoo",
     )
 
     options_validator_service.validate_aws_for_cluster(
-      aws_access_key_id='foobar',
-      aws_secret_access_key='barfoo',
-      additional_policies=['bar']
+      aws_access_key_id="foobar",
+      aws_secret_access_key="barfoo",
+      additional_policies=["bar"],
     )
 
   def test_validate_aws_simple(self, options_validator_service):
     options_validator_service.validate_aws_for_orchestrate()
     options_validator_service.validate_aws_for_cluster()
 
   def test_validate_aws_rejects_ecr(self, options_validator_service):
     with pytest.raises(TypeError):
       options_validator_service.validate_aws_for_cluster(
         ecr=dict(
-          image='orchestrate/test',
+          image="orchestrate/test",
         ),
       )
 
     with pytest.raises(TypeError):
       options_validator_service.validate_aws_for_orchestrate(
         ecr=dict(
-          image='orchestrate/test',
+          image="orchestrate/test",
         ),
       )
 
     with pytest.raises(TypeError):
       options_validator_service.validate_aws_for_orchestrate(
         ecr=dict(),
       )
 
   def test_validate_aws_additional_policies(self, options_validator_service):
     options_validator_service.validate_aws_for_cluster(additional_policies=[])
     options_validator_service.validate_aws_for_cluster(additional_policies=None)
 
     with pytest.raises(AssertionError):
-      options_validator_service.validate_aws_for_cluster(additional_policies='policy')
+      options_validator_service.validate_aws_for_cluster(additional_policies="policy")
 
   def test_validate_sigopt(self, options_validator_service):
     options_validator_service.validate_sigopt(
-      api_token='foobar',
+      api_token="foobar",
     )
 
   def test_validate_sigopt_simple(self, options_validator_service):
     options_validator_service.validate_sigopt()
 
-  @pytest.mark.parametrize('api_token', ['', 0])
+  @pytest.mark.parametrize("api_token", ["", 0])
   def test_validate_sigopt_wrong_value(self, options_validator_service, api_token):
     with pytest.raises(AssertionError):
       options_validator_service.validate_sigopt(
         api_token=api_token,
       )
 
   def test_validate_cluster_options(self, options_validator_service):
     options_validator_service.validate_cluster_options(
-      provider='aws',
-      cluster_name='test-cluster',
+      provider="aws",
+      cluster_name="test-cluster",
       cpu=dict(
-        instance_type='t2.small',
+        instance_type="t2.small",
         min_nodes=1,
         max_nodes=1,
       ),
       gpu=dict(
-        instance_type='p3.2xlarge',
+        instance_type="p3.2xlarge",
         min_nodes=2,
         max_nodes=2,
       ),
       system=dict(
-        instance_type='t3.small',
+        instance_type="t3.small",
         min_nodes=1,
         max_nodes=2,
       ),
     )
 
   def test_validate_cluster_options_ok_missing_values(self, options_validator_service):
     options_validator_service.validate_cluster_options(
-      cluster_name='test-cluster',
-      provider='custom',
+      cluster_name="test-cluster",
+      provider="custom",
       cpu=dict(
-        instance_type='t2.small',
+        instance_type="t2.small",
         min_nodes=1,
         max_nodes=1,
       ),
       gpu=dict(
-        instance_type='p3.2xlarge',
+        instance_type="p3.2xlarge",
         min_nodes=2,
         max_nodes=2,
       ),
       system=dict(
-        instance_type='t3.small',
+        instance_type="t3.small",
         min_nodes=1,
         max_nodes=2,
       ),
     )
 
     options_validator_service.validate_cluster_options(
-      provider='aws',
-      cluster_name='test-cluster',
+      provider="aws",
+      cluster_name="test-cluster",
       gpu=dict(
-        instance_type='p3.2xlarge',
+        instance_type="p3.2xlarge",
         min_nodes=2,
         max_nodes=2,
       ),
       system=dict(
-        instance_type='t3.small',
+        instance_type="t3.small",
         min_nodes=1,
         max_nodes=2,
       ),
     )
 
     options_validator_service.validate_cluster_options(
-      provider='aws',
-      cluster_name='test-cluster',
+      provider="aws",
+      cluster_name="test-cluster",
       cpu=dict(
-        instance_type='t2.small',
+        instance_type="t2.small",
         min_nodes=1,
         max_nodes=1,
       ),
       system=dict(
-        instance_type='t3.small',
+        instance_type="t3.small",
         min_nodes=1,
         max_nodes=2,
       ),
     )
 
-  @pytest.mark.parametrize('cluster_name', ['', None, dict()])
+  @pytest.mark.parametrize("cluster_name", ["", None, dict()])
   def test_validate_cluster_options_cluster_name(self, options_validator_service, cluster_name):
     with pytest.raises(AssertionError):
       options_validator_service.validate_cluster_options(
-        provider='aws',
+        provider="aws",
         cluster_name=cluster_name,
         cpu=dict(
-          instance_type='t2.small',
+          instance_type="t2.small",
           min_nodes=1,
           max_nodes=1,
         ),
         system=dict(
-          instance_type='t3.small',
+          instance_type="t3.small",
           min_nodes=1,
           max_nodes=2,
         ),
       )
 
   def test_validate_cluster_options_extra_options(self, options_validator_service):
     with pytest.raises(AssertionError):
       options_validator_service.validate_cluster_options(
-        provider='aws',
-        cluster_name='test-cluster',
+        provider="aws",
+        cluster_name="test-cluster",
         tpu=dict(
-          instance_type='p3.2xlarge',
+          instance_type="p3.2xlarge",
           min_nodes=2,
           max_nodes=2,
         ),
       )
 
   def test_validate_cluster_options_wrong_type(self, options_validator_service):
     with pytest.raises(AssertionError):
       options_validator_service.validate_cluster_options(
-        provider='aws',
-        cluster_name='test-cluster',
-        gpu=[dict(
-          instance_type='p3.2xlarge',
-          min_nodes=2,
-          max_nodes=2,
-        )],
+        provider="aws",
+        cluster_name="test-cluster",
+        gpu=[
+          dict(
+            instance_type="p3.2xlarge",
+            min_nodes=2,
+            max_nodes=2,
+          )
+        ],
       )
 
     with pytest.raises(AssertionError):
       options_validator_service.validate_cluster_options(
-        provider='aws',
-        cluster_name='test-cluster',
-        cpu=[dict(
-          instance_type='t2.small',
-          min_nodes=1,
-          max_nodes=1,
-        )],
+        provider="aws",
+        cluster_name="test-cluster",
+        cpu=[
+          dict(
+            instance_type="t2.small",
+            min_nodes=1,
+            max_nodes=1,
+          )
+        ],
         system=dict(
-          instance_type='t3.small',
+          instance_type="t3.small",
           min_nodes=1,
           max_nodes=2,
         ),
       )
 
   def test_validate_cluster_options_ignore_values(self, options_validator_service):
     options_validator_service.validate_cluster_options(
-      provider='aws',
-      cluster_name='test-cluster',
+      provider="aws",
+      cluster_name="test-cluster",
       cpu=dict(
-        instance_type='t2.small',
+        instance_type="t2.small",
         min_nodes=1,
         max_nodes=1,
       ),
       system=dict(
-        instance_type='t3.small',
+        instance_type="t3.small",
         min_nodes=1,
         max_nodes=2,
       ),
     )
 
   def test_validate_worker_stack(self, options_validator_service):
     options_validator_service.validate_worker_stack(
-      name='cpu',
-      instance_type='t2.small',
+      name="cpu",
+      instance_type="t2.small",
       min_nodes=1,
       max_nodes=1,
     )
 
   def test_validate_worker_stack_ignores_values(self, options_validator_service):
     options_validator_service.validate_worker_stack(
-      name='foobar',
-      instance_type='bazzle',
+      name="foobar",
+      instance_type="bazzle",
       min_nodes=2,
       max_nodes=19,
     )
 
   def test_validate_worker_stack_missing_options(self, options_validator_service):
     with pytest.raises(AssertionError):
       options_validator_service.validate_worker_stack(
-        name='cpu',
+        name="cpu",
         min_nodes=1,
         max_nodes=1,
       )
 
     with pytest.raises(AssertionError):
       options_validator_service.validate_worker_stack(
-        name='cpu',
-        instance_type='t2.small',
+        name="cpu",
+        instance_type="t2.small",
         max_nodes=1,
       )
 
     with pytest.raises(AssertionError):
       options_validator_service.validate_worker_stack(
-        name='cpu',
-        instance_type='t2.small',
+        name="cpu",
+        instance_type="t2.small",
         min_nodes=1,
       )
 
   def test_validate_worker_stack_wrong_type(self, options_validator_service):
     with pytest.raises(AssertionError):
       options_validator_service.validate_worker_stack(
-        name='cpu',
+        name="cpu",
         instance_type=2,
         min_nodes=1,
         max_nodes=1,
       )
 
     with pytest.raises(AssertionError):
       options_validator_service.validate_worker_stack(
-        name='cpu',
-        instance_type='t2.small',
-        min_nodes='1',
+        name="cpu",
+        instance_type="t2.small",
+        min_nodes="1",
         max_nodes=1,
       )
 
     with pytest.raises(AssertionError):
       options_validator_service.validate_worker_stack(
-        name='cpu',
-        instance_type='t2.small',
+        name="cpu",
+        instance_type="t2.small",
         min_nodes=1,
-        max_nodes='1',
+        max_nodes="1",
       )
 
   def test_validate_worker_stack_negative(self, options_validator_service):
     with pytest.raises(AssertionError):
       options_validator_service.validate_worker_stack(
-        name='cpu',
-        instance_type='t2.small',
+        name="cpu",
+        instance_type="t2.small",
         min_nodes=-1,
         max_nodes=1,
       )
 
     with pytest.raises(AssertionError):
       options_validator_service.validate_worker_stack(
-        name='cpu',
-        instance_type='t2.small',
+        name="cpu",
+        instance_type="t2.small",
         min_nodes=1,
         max_nodes=-1,
       )
```

### Comparing `sigopt-8.8.0/test/orchestrate/provider/broker_test.py` & `sigopt-8.8.1/test/orchestrate/provider/broker_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,26 +10,29 @@
 from sigopt.orchestrate.provider.constants import Provider, string_to_provider
 
 
 class TestProviderBroker(object):
   @pytest.fixture
   def services(self):
     return Mock(
-      get_option=Mock(return_value='foo'),
+      get_option=Mock(return_value="foo"),
     )
 
   @pytest.fixture
   def provider_broker(self, services):
     return ProviderBroker(services)
 
   def test_get_provider_service(self, provider_broker, services):
-    assert isinstance(provider_broker.get_provider_service(string_to_provider('aws')), AwsService)
-    assert isinstance(provider_broker.get_provider_service(string_to_provider('AWS')), AwsService)
+    assert isinstance(provider_broker.get_provider_service(string_to_provider("aws")), AwsService)
+    assert isinstance(provider_broker.get_provider_service(string_to_provider("AWS")), AwsService)
     assert isinstance(provider_broker.get_provider_service(Provider.AWS), AwsService)
 
   def test_custom_provider(self, provider_broker, services):
-    assert isinstance(provider_broker.get_provider_service(string_to_provider('custom')), CustomClusterService)
+    assert isinstance(
+      provider_broker.get_provider_service(string_to_provider("custom")),
+      CustomClusterService,
+    )
     assert isinstance(provider_broker.get_provider_service(Provider.CUSTOM), CustomClusterService)
 
   def test_unknown_provider(self, provider_broker):
     with pytest.raises(NotImplementedError):
       provider_broker.get_provider_service(0)
```

### Comparing `sigopt-8.8.0/test/orchestrate/resource/service_test.py` & `sigopt-8.8.1/test/orchestrate/resource/service_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,31 +4,32 @@
 import os
 
 import pytest
 
 from sigopt.orchestrate.resource.service import ResourceService
 
 
-TEST_MODULE = 'test'
-TEST_FILE = 'test_file.txt'
+TEST_MODULE = "test"
+TEST_FILE = "test_file.txt"
 ACTUAL_TEXT = "This is a test file for testing the resource service.\n".encode()
 
+
 class TestResourceService(object):
   @pytest.fixture
   def resource_service(self):
     return ResourceService(None)
 
   def test_resource_stream(self, resource_service):
     with resource_service.stream(TEST_MODULE, TEST_FILE) as stream:
       assert ACTUAL_TEXT == stream.read()
 
   def test_resource_open(self, resource_service):
     with resource_service.open(TEST_MODULE, TEST_FILE) as test_fp:
       assert ACTUAL_TEXT == test_fp.read()
-      with open(test_fp.name, mode='rb') as second_open:
+      with open(test_fp.name, mode="rb") as second_open:
         assert ACTUAL_TEXT == second_open.read()
 
   def test_tempfile_removed(self, resource_service):
     test_fp = resource_service.open(TEST_MODULE, TEST_FILE)
     test_fp.close()
     assert not os.path.isfile(test_fp.name)
```

### Comparing `sigopt-8.8.0/test/orchestrate/services/aws_provider_bag_test.py` & `sigopt-8.8.1/test/orchestrate/services/aws_provider_bag_test.py`

 * *Files identical despite different names*

### Comparing `sigopt-8.8.0/test/orchestrate/sigopt/service_test.py` & `sigopt-8.8.1/test/orchestrate/sigopt/service_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,12 +11,15 @@
 
 class TestSigOptService(object):
   @pytest.fixture
   def services(self):
     return Mock()
 
   def test_reads_from_environment(self, services):
-    with patch.dict(os.environ, dict(SIGOPT_API_TOKEN='foobar', SIGOPT_API_URL='https://api-env.sigopt.com')):
+    with patch.dict(
+      os.environ,
+      dict(SIGOPT_API_TOKEN="foobar", SIGOPT_API_URL="https://api-env.sigopt.com"),
+    ):
       sigopt_service = SigOptService(services)
       assert sigopt_service.conn is not None
-      assert sigopt_service.api_token == 'foobar'
-      assert sigopt_service.api_url == 'https://api-env.sigopt.com'
+      assert sigopt_service.api_token == "foobar"
+      assert sigopt_service.api_url == "https://api-env.sigopt.com"
```

### Comparing `sigopt-8.8.0/test/runs/test_config.py` & `sigopt-8.8.1/test/runs/test_config.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 import base64
-import mock
 import os
 
+import mock
+
 from sigopt.config import Config
 
-fake_context = base64.b64encode(b'{"a": "b"}').decode('utf-8')
+
+fake_context = base64.b64encode(b'{"a": "b"}').decode("utf-8")
+
 
 class FakeConfigContext(object):
   def __init__(self, key):
     self.CONFIG_CONTEXT_KEY = key
 
+
 class TestConfig(object):
   def test_load_json_config(self):
-    with mock.patch.dict(os.environ, {'SIGOPT_CONTEXT': fake_context}):
+    with mock.patch.dict(os.environ, {"SIGOPT_CONTEXT": fake_context}):
       config = Config()
 
-    assert config.get_context_data(FakeConfigContext('a')) == 'b'
-    assert config.get_context_data(FakeConfigContext('none')) is None
+    assert config.get_context_data(FakeConfigContext("a")) == "b"
+    assert config.get_context_data(FakeConfigContext("none")) is None
```

### Comparing `sigopt-8.8.0/test/runs/test_context.py` & `sigopt-8.8.1/test/runs/test_context.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 from __future__ import print_function
+
 import io
 
 import mock
 import pytest
 
 from sigopt.interface import Connection
-from sigopt.run_context import allow_state_update, RunContext
+from sigopt.run_context import RunContext, allow_state_update
 
 
 @pytest.mark.parametrize(
   "new_state,old_state,expected",
   [
     ("completed", "active", True),
     ("failed", "active", True),
@@ -54,34 +55,30 @@
     ],
   )
   def test_assignment_setitem(self, run_context, test_value):
     test_key = "assignment_test_key"
     run_context.params[test_key] = test_value
     assert run_context.params[test_key] == test_value
     assert getattr(run_context.params, test_key) == test_value
-    self.assert_run_update_request_called(
-      run_context, {"assignments": {test_key: test_value}}
-    )
+    self.assert_run_update_request_called(run_context, {"assignments": {test_key: test_value}})
 
   @pytest.mark.parametrize(
     "test_value",
     [
       12345,
       1.2345,
       "hello",
     ],
   )
   def test_assignment_setattr(self, run_context, test_value):
     test_key = "assignment_test_key"
     setattr(run_context.params, test_key, test_value)
     assert run_context.params[test_key] == test_value
     assert getattr(run_context.params, test_key) == test_value
-    self.assert_run_update_request_called(
-      run_context, {"assignments": {test_key: test_value}}
-    )
+    self.assert_run_update_request_called(run_context, {"assignments": {test_key: test_value}})
 
   def test_log_failure_method(self, run_context):
     return_value = run_context.log_failure()
     assert return_value is None
     self.assert_run_update_request_called(run_context, {"state": "failed"})
 
   @pytest.mark.parametrize(
@@ -91,17 +88,15 @@
       1.2345,
     ],
   )
   def test_log_metadata_method_with_numbers(self, run_context, test_value):
     test_key = "test_metadata_key"
     return_value = run_context.log_metadata(test_key, test_value)
     assert return_value is None
-    self.assert_run_update_request_called(
-      run_context, {"metadata": {test_key: test_value}}
-    )
+    self.assert_run_update_request_called(run_context, {"metadata": {test_key: test_value}})
 
   def test_log_metadata_method_with_null(self, run_context):
     test_key = "test_metadata_key"
     return_value = run_context.log_metadata(test_key, None)
     assert return_value is None
     self.assert_run_update_request_called(run_context, {"metadata": {test_key: None}})
 
@@ -114,17 +109,15 @@
       object(),
     ],
   )
   def test_log_metadata_method_stringifies_objects(self, run_context, test_value):
     test_key = "test_metadata_key"
     return_value = run_context.log_metadata(test_key, test_value)
     assert return_value is None
-    self.assert_run_update_request_called(
-      run_context, {"metadata": {test_key: str(test_value)}}
-    )
+    self.assert_run_update_request_called(run_context, {"metadata": {test_key: str(test_value)}})
 
   @pytest.mark.parametrize(
     "test_value",
     [
       12345,
       1.2345,
     ],
@@ -209,15 +202,15 @@
           dataset_name: {},
         }
       },
     )
 
   def test_log_model(self, run_context):
     model_type = "test type"
-    return_value = run_context.log_model(type=model_type)
+    return_value = run_context.log_model(type_=model_type)
     assert return_value is None
     self.assert_run_update_request_called(run_context, {"model": {"type": model_type}})
 
   def test_log_image(self, run_context):
     run_context.connection.impl.driver.request.return_value = {
       "upload": {
         "method": "TEST",
```

### Comparing `sigopt-8.8.0/test/runs/test_factory.py` & `sigopt-8.8.1/test/runs/test_factory.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,75 +1,77 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
+import warnings
+
 import mock
 import pytest
-from contextlib import contextmanager
-import warnings
 
-import sigopt
-from sigopt.exception import RunException
-from sigopt.run_context import RunContext, GlobalRunContext
 from sigopt.factory import SigOptFactory
 
 
 warnings.simplefilter("always")
 
 
 class TestSigOptFactory(object):
   @pytest.fixture
   def api_connection(self):
     conn = mock.Mock()
-    conn.clients().projects().training_runs().create.return_value = mock.Mock(assignments={"fixed1": 0, "fixed2": "test"})
+    conn.clients().projects().training_runs().create.return_value = mock.Mock(
+      assignments={"fixed1": 0, "fixed2": "test"}
+    )
     return conn
 
   @pytest.fixture(autouse=True)
   def patched_connection(self, api_connection):
-    with mock.patch('sigopt.factory.get_connection') as connection_singleton:
+    with mock.patch("sigopt.factory.get_connection") as connection_singleton:
       connection_singleton.return_value = api_connection
       yield
 
   @pytest.fixture
   def factory(self):
     factory = SigOptFactory("test-project")
     return factory
 
   def test_create_run(self, factory):
     run_context = factory.create_run()
     assert run_context is not None
 
   def test_create_context_with_name(self, factory, api_connection):
-    run_context = factory.create_run(name='test context')
+    run_context = factory.create_run(name="test context")
     assert run_context is not None
     api_connection.clients().projects().training_runs().create.assert_called_once()
-    assert api_connection.clients().projects().training_runs().create.call_args[1]['name'] == 'test context'
+    assert api_connection.clients().projects().training_runs().create.call_args[1]["name"] == "test context"
 
   def test_local_run_context_methods(self, factory):
-    with factory.create_run(name='test-run') as local_run:
+    with factory.create_run(name="test-run") as local_run:
       local_run._update_run = mock.Mock()
       local_run.params.p1 = 1
       local_run.params.setdefault("p2", 2)
       local_run.params.update({"p3": 3, "p4": 4})
       local_run.params.setdefault("p3", 0)
       local_run.params.pop("p2")
-      local_run.log_metric('metric', 1, 0.1)
-    local_run._update_run.assert_has_calls([
-      mock.call({'assignments': {'p1': 1}}),
-      mock.call({'assignments': {'p2': 2}}),
-      mock.call({'assignments': {'p3': 3, 'p4': 4}}),
-      mock.call({'assignments': {'p2': None}}),
-      mock.call({'values': {'metric': {'value': 1, 'value_stddev': 0.1}}}),
-      mock.call({'state': 'completed'}),
-    ])
+      local_run.log_metric("metric", 1, 0.1)
+    local_run._update_run.assert_has_calls(
+      [
+        mock.call({"assignments": {"p1": 1}}),
+        mock.call({"assignments": {"p2": 2}}),
+        mock.call({"assignments": {"p3": 3, "p4": 4}}),
+        mock.call({"assignments": {"p2": None}}),
+        mock.call({"values": {"metric": {"value": 1, "value_stddev": 0.1}}}),
+        mock.call({"state": "completed"}),
+      ]
+    )
 
   def test_local_run_context_exception(self, factory):
-
     class TestException(Exception):
       pass
 
     with pytest.raises(TestException):
-      with factory.create_run(name='test-run') as local_run:
+      with factory.create_run(name="test-run") as local_run:
         local_run._update_run = mock.Mock()
         raise TestException()
-    local_run._update_run.assert_has_calls([
-      mock.call({'state': 'failed'}),
-    ])
+    local_run._update_run.assert_has_calls(
+      [
+        mock.call({"state": "failed"}),
+      ]
+    )
```

### Comparing `sigopt-8.8.0/test/runs/test_local_run_context.py` & `sigopt-8.8.1/test/runs/test_local_run_context.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,73 +1,76 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
-from sigopt.local_run_context import LocalRunContext
 import pytest
 
+from sigopt.local_run_context import LocalRunContext
 
-class TestLocalRunContext(object):
 
+class TestLocalRunContext(object):
   @pytest.fixture
   def context(self):
     return LocalRunContext()
 
   @pytest.fixture
   def params(self):
-    return {
-      'x': 1.0,
-      'y': 2.0
-    }
+    return {"x": 1.0, "y": 2.0}
 
   @pytest.fixture
   def metrics(self):
     return {
-      'v0': 1,
-      'v1': 2.0,
+      "v0": 1,
+      "v1": 2.0,
     }
 
   def test_init(self):
-    name = 'test0'
-    metadata = {'m0': 1, 'm2': 2.0}
+    name = "test0"
+    metadata = {"m0": 1, "m2": 2.0}
     context = LocalRunContext(name=name, metadata=metadata)
     run = context.get()
-    assert run['name'] == name
-    assert run['metadata'] == metadata
+    assert run["name"] == name
+    assert run["metadata"] == metadata
 
-  @pytest.mark.parametrize('state', ['completed', 'failed'])
+  @pytest.mark.parametrize("state", ["completed", "failed"])
   def test_log_state(self, context, state):
     context.log_state(state)
     run = context.get()
-    assert run['state'] == state
+    assert run["state"] == state
 
   def test_log_failure(self, context):
     context.log_failure()
     run = context.get()
-    assert run['state'] == 'failed'
+    assert run["state"] == "failed"
 
   def test_log_metrics(self, context, metrics):
-    context.log_metrics()
+    context.log_metrics(metrics)
     run = context.get()
-    run['values'] == metrics
+    assert run["values"] == {k: {"value": v} for k, v in metrics.items()}
 
-  @pytest.mark.parametrize('source, source_sort, source_default_show', [
-    ('s0', 10, True),
-    ('s0', 20, False),
-    ('s0', None, None),
-    (None, 20, False),
-  ])
+  @pytest.mark.parametrize(
+    "source, source_sort, source_default_show",
+    [
+      ("s0", 10, True),
+      ("s0", 20, False),
+      ("s0", None, None),
+      (None, 20, False),
+    ],
+  )
   def test_log_parameters(self, context, params, source, source_sort, source_default_show):
     if source_sort is not None:
-      source_meta = {'sort': source_sort, 'default_show': source_default_show}
+      source_meta = {"sort": source_sort, "default_show": source_default_show}
     else:
       source_meta = None
     context.log_parameters(params, source, source_meta)
     run = context.get()
-    assert run['assignments'] == params
+    assert run["assignments"] == params
     if source is not None:
-      assert run['assignments_meta'] == {p: {'source': source} for p in params}
+      assert run["assignments_meta"] == {p: {"source": source} for p in params}
       if source_sort is not None:
-        assert run['assignments_sources'][source] == {'sort': source_sort, 'default_show': source_default_show}
+        assert run["assignments_sources"][source] == {
+          "sort": source_sort,
+          "default_show": source_default_show,
+        }
       else:
-        assert 'assignments_sources' not in run
+        assert "assignments_sources" not in run
     else:
-      assert 'assignments_meta' not in run and 'assignments_sources' not in run
+      assert "assignments_meta" not in run and "assignments_sources" not in run
```

### Comparing `sigopt-8.8.0/test/runs/test_set_project.py` & `sigopt-8.8.1/test/runs/test_set_project.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 import mock
 import pytest
 
-from sigopt import set_project, _global_factory
+from sigopt import _global_factory, set_project
+
 
 def test_set_project_with_global_run():
   with mock.patch("sigopt.get_run_id", mock.Mock(return_value="1")):
     with pytest.warns(UserWarning):
       set_project("test-123")
   assert _global_factory.project == "test-123"
 
+
 def test_set_project_without_run():
   with mock.patch("sigopt.get_run_id", mock.Mock(return_value=None)):
     with pytest.warns(None) as warnings:
       set_project("test-123")
   assert len(warnings) == 0
   assert _global_factory.project == "test-123"
```

### Comparing `sigopt-8.8.0/test/runs/test_utils.py` & `sigopt-8.8.1/test/runs/test_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
+import matplotlib
 import pytest
 
-import matplotlib
+
 matplotlib.use("Agg")
 
 import io
-import numpy
 import os
-from PIL import Image
-from matplotlib import pyplot as plt
 import xml.etree.ElementTree as ET
 
+import numpy
+from matplotlib import pyplot as plt
+from PIL import Image
+from utils import ObserveWarnings
+
 from sigopt.file_utils import (
   create_api_image_payload,
   get_blob_properties,
   try_load_matplotlib_image,
   try_load_numpy_image,
   try_load_pil_image,
 )
-from utils import ObserveWarnings
 
 
 @pytest.fixture
 def pil_image():
   return Image.new("RGB", (16, 16), (255, 0, 0))
 
 
@@ -128,19 +130,22 @@
 
   assert numpy.all(loaded_numpy_img[:16] == 0)
   assert numpy.all(loaded_numpy_img[16:] == 255)
 
   assert content_type == "image/png"
 
 
-@pytest.mark.parametrize("image_path,expected_type", [
-  ("test.png", "image/png"),
-  ("test.svg", "image/svg+xml"),
-  ("test.bmp", "image/bmp"),
-])
+@pytest.mark.parametrize(
+  "image_path,expected_type",
+  [
+    ("test.png", "image/png"),
+    ("test.svg", "image/svg+xml"),
+    ("test.bmp", "image/bmp"),
+  ],
+)
 def test_create_api_image_payload_string_path(image_path, expected_type):
   image_path = os.path.join("./test/runs/test_files", image_path)
   data = create_api_image_payload(image_path)
   assert data is not None
   filepath, image_data, content_type = data
   with image_data:
     image_data.seek(0)
@@ -159,32 +164,32 @@
     assert len(w) == 1
     assert issubclass(w[-1].category, RuntimeWarning)
 
 
 def test_create_api_image_payload_pil_image(pil_image):
   data = create_api_image_payload(pil_image)
   assert data is not None
-  filepath, image_data, content_type = data
+  filepath, _, content_type = data
   assert filepath is None
   assert content_type == "image/png"
 
 
 def test_create_api_image_payload_matplotlib_figure(matplotlib_figure):
   data = create_api_image_payload(matplotlib_figure)
   assert data is not None
-  filepath, image_data, content_type = data
+  filepath, _, content_type = data
   assert filepath is None
   assert content_type == "image/svg+xml"
 
 
 def test_create_api_image_payload_numpy_image():
   numpy_image = numpy.random.randint(0, 255, (16, 16))
   data = create_api_image_payload(numpy_image)
   assert data is not None
-  filepath, image_data, content_type = data
+  filepath, _, content_type = data
   assert filepath is None
   assert content_type == "image/png"
 
 
 def test_create_api_image_payload_unsupported_type():
   with ObserveWarnings() as w:
     data = create_api_image_payload({})
```

### Comparing `sigopt-8.8.0/test/validate/test_validate_experiment.py` & `sigopt-8.8.1/test/validate/test_validate_experiment.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 import copy
+
 import pytest
 
 from sigopt.validate.aiexperiment_input import validate_aiexperiment_input
 from sigopt.validate.exceptions import ValidationError
 
 
 VALID_EXPERIMENT_INPUT = {
@@ -21,64 +22,125 @@
     },
   ],
   "metrics": [{"name": "m1"}],
   "budget": 10,
   "parallel_bandwidth": 4,
 }
 
+
 class TestValidateExperiment:
-  @pytest.mark.parametrize("mutator,expected_message", [
-    (lambda e: e.__delitem__("name"), "name is required"),
-    (lambda e: e.__setitem__("name", None), "name must be a string"),
-    (lambda e: e.__setitem__("name", ""), "name cannot be an empty string"),
-    (lambda e: e.__setitem__("name", 1), "name must be a string"),
-    (lambda e: e.__setitem__("name", {}), "name must be a string"),
-    (lambda e: e.__delitem__("parameters"), "parameters is required"),
-    (lambda e: e.__setitem__("parameters", None), "parameters must be a non-empty list"),
-    (lambda e: e.__setitem__("parameters", {}), "parameters must be a non-empty list"),
-    (lambda e: e.__setitem__("parameters", []), "parameters must be a non-empty list"),
-    (lambda e: e["parameters"].__setitem__(0, []), "parameters must be a mapping"),
-    (lambda e: e["parameters"][0].__delitem__("name"), "parameters require a name"),
-    (lambda e: e["parameters"][0].__setitem__("name", None), "parameter name must be a string"),
-    (lambda e: e["parameters"][0].__setitem__("name", ""), "parameter name cannot be an empty string"),
-    (lambda e: e["parameters"][0].__delitem__("type"), "parameters require a type"),
-    (lambda e: e["parameters"][0].__setitem__("type", None), "parameter type must be a string"),
-    (lambda e: e["parameters"][0].__setitem__("type", {}), "parameter type must be a string"),
-    (lambda e: e["parameters"][0].__setitem__("type", ""), "parameter type cannot be an empty string"),
-    (lambda e: e.__delitem__("metrics"), "metrics is required"),
-    (lambda e: e.__setitem__("metrics", None), "metrics must be a non-empty list"),
-    (lambda e: e.__setitem__("metrics", {}), "metrics must be a non-empty list"),
-    (lambda e: e.__setitem__("metrics", []), "metrics must be a non-empty list"),
-    (lambda e: e["metrics"].__setitem__(0, []), "metrics must be a mapping"),
-    (lambda e: e["metrics"][0].__delitem__("name"), "metrics require a name"),
-    (lambda e: e["metrics"][0].__setitem__("name", None), "metric name must be a string"),
-    (lambda e: e["metrics"][0].__setitem__("name", ""), "metric name cannot be an empty string"),
-    (lambda e: e.__setitem__("budget", []), "budget must be a non-negative number"),
-    (lambda e: e.__setitem__("budget", -1), "budget must be a non-negative number"),
-    (lambda e: e.__setitem__("budget", float("inf")), "budget cannot be infinity"),
-    (lambda e: e.__setitem__("parallel_bandwidth", []), "parallel_bandwidth must be a positive integer"),
-    (lambda e: e.__setitem__("parallel_bandwidth", -1), "parallel_bandwidth must be a positive integer"),
-    (lambda e: e.__setitem__("parallel_bandwidth", 0), "parallel_bandwidth must be a positive integer"),
-    (lambda e: e.__setitem__("parallel_bandwidth", 0.5), "parallel_bandwidth must be a positive integer"),
-  ])
+  @pytest.mark.parametrize(
+    "mutator,expected_message",
+    [
+      (lambda e: e.__delitem__("name"), "name is required"),
+      (lambda e: e.__setitem__("name", None), "name must be a string"),
+      (lambda e: e.__setitem__("name", ""), "name cannot be an empty string"),
+      (lambda e: e.__setitem__("name", 1), "name must be a string"),
+      (lambda e: e.__setitem__("name", {}), "name must be a string"),
+      (lambda e: e.__delitem__("parameters"), "parameters is required"),
+      (
+        lambda e: e.__setitem__("parameters", None),
+        "parameters must be a non-empty list",
+      ),
+      (
+        lambda e: e.__setitem__("parameters", {}),
+        "parameters must be a non-empty list",
+      ),
+      (
+        lambda e: e.__setitem__("parameters", []),
+        "parameters must be a non-empty list",
+      ),
+      (lambda e: e["parameters"].__setitem__(0, []), "parameters must be a mapping"),
+      (lambda e: e["parameters"][0].__delitem__("name"), "parameters require a name"),
+      (
+        lambda e: e["parameters"][0].__setitem__("name", None),
+        "parameter name must be a string",
+      ),
+      (
+        lambda e: e["parameters"][0].__setitem__("name", ""),
+        "parameter name cannot be an empty string",
+      ),
+      (lambda e: e["parameters"][0].__delitem__("type"), "parameters require a type"),
+      (
+        lambda e: e["parameters"][0].__setitem__("type", None),
+        "parameter type must be a string",
+      ),
+      (
+        lambda e: e["parameters"][0].__setitem__("type", {}),
+        "parameter type must be a string",
+      ),
+      (
+        lambda e: e["parameters"][0].__setitem__("type", ""),
+        "parameter type cannot be an empty string",
+      ),
+      (lambda e: e.__delitem__("metrics"), "metrics is required"),
+      (lambda e: e.__setitem__("metrics", None), "metrics must be a non-empty list"),
+      (lambda e: e.__setitem__("metrics", {}), "metrics must be a non-empty list"),
+      (lambda e: e.__setitem__("metrics", []), "metrics must be a non-empty list"),
+      (lambda e: e["metrics"].__setitem__(0, []), "metrics must be a mapping"),
+      (lambda e: e["metrics"][0].__delitem__("name"), "metrics require a name"),
+      (
+        lambda e: e["metrics"][0].__setitem__("name", None),
+        "metric name must be a string",
+      ),
+      (
+        lambda e: e["metrics"][0].__setitem__("name", ""),
+        "metric name cannot be an empty string",
+      ),
+      (lambda e: e.__setitem__("budget", []), "budget must be a non-negative number"),
+      (lambda e: e.__setitem__("budget", -1), "budget must be a non-negative number"),
+      (lambda e: e.__setitem__("budget", float("inf")), "budget cannot be infinity"),
+      (
+        lambda e: e.__setitem__("parallel_bandwidth", []),
+        "parallel_bandwidth must be a positive integer",
+      ),
+      (
+        lambda e: e.__setitem__("parallel_bandwidth", -1),
+        "parallel_bandwidth must be a positive integer",
+      ),
+      (
+        lambda e: e.__setitem__("parallel_bandwidth", 0),
+        "parallel_bandwidth must be a positive integer",
+      ),
+      (
+        lambda e: e.__setitem__("parallel_bandwidth", 0.5),
+        "parallel_bandwidth must be a positive integer",
+      ),
+    ],
+  )
   def test_invalid_experiment(self, mutator, expected_message):
     experiment_input = copy.deepcopy(VALID_EXPERIMENT_INPUT)
     mutator(experiment_input)
     with pytest.raises(ValidationError) as validation_error:
       validate_aiexperiment_input(experiment_input)
     assert expected_message in str(validation_error)
 
-  @pytest.mark.parametrize("mutator,check", [
-    (lambda e: e, lambda e: e["name"] == "test experiment"),
-    (lambda e: e, lambda e: e["parameters"] == [{"name": "p1", "type": "int", "bounds": {"min": 0, "max": 1}}]),
-    (lambda e: e, lambda e: e["metrics"] == [{"name": "m1"}]),
-    (lambda e: e, lambda e: e["parallel_bandwidth"] == 4),
-    # support new features without needing to write new validation
-    (lambda e: e.__setitem__("unrecognized_key", []), lambda e: e["unrecognized_key"] == []),
-    (lambda e: e["parameters"][0].__setitem__("unrecognized_key", []), lambda e: e["parameters"][0]["unrecognized_key"] == []),
-    (lambda e: e["metrics"][0].__setitem__("unrecognized_key", []), lambda e: e["metrics"][0]["unrecognized_key"] == []),
-  ])
+  @pytest.mark.parametrize(
+    "mutator,check",
+    [
+      (lambda e: e, lambda e: e["name"] == "test experiment"),
+      (
+        lambda e: e,
+        lambda e: e["parameters"] == [{"name": "p1", "type": "int", "bounds": {"min": 0, "max": 1}}],
+      ),
+      (lambda e: e, lambda e: e["metrics"] == [{"name": "m1"}]),
+      (lambda e: e, lambda e: e["parallel_bandwidth"] == 4),
+      # support new features without needing to write new validation
+      (
+        lambda e: e.__setitem__("unrecognized_key", []),
+        lambda e: e["unrecognized_key"] == [],
+      ),
+      (
+        lambda e: e["parameters"][0].__setitem__("unrecognized_key", []),
+        lambda e: e["parameters"][0]["unrecognized_key"] == [],
+      ),
+      (
+        lambda e: e["metrics"][0].__setitem__("unrecognized_key", []),
+        lambda e: e["metrics"][0]["unrecognized_key"] == [],
+      ),
+    ],
+  )
   def test_valid_experiment(self, mutator, check):
     experiment_input = copy.deepcopy(VALID_EXPERIMENT_INPUT)
     mutator(experiment_input)
     validated = validate_aiexperiment_input(experiment_input)
     assert check(validated)
```

### Comparing `sigopt-8.8.0/test/validate/test_validate_run.py` & `sigopt-8.8.1/test/validate/test_validate_run.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,47 +1,58 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 import copy
+
 import pytest
 
-from sigopt.validate.run_input import validate_run_input
 from sigopt.validate.exceptions import ValidationError
+from sigopt.validate.run_input import validate_run_input
 
 
 VALID_RUN_INPUT = {
   "name": "test run",
   "run": "python test.py",
   "resources": {"gpus": 2},
 }
 
+
 class TestValidateRun:
-  @pytest.mark.parametrize("mutator,expected_message", [
-    (lambda r: r.__setitem__("name", ""), "name cannot be an empty string"),
-    (lambda r: r.__setitem__("name", 1), "name must be a string"),
-    (lambda r: r.__setitem__("name", {}), "name must be a string"),
-    (lambda r: r.__setitem__("run", {}), "must be a command"),
-    (lambda r: r.__setitem__("run", [1, 2, 3]), "has some non-string arguments"),
-    (lambda r: r.__setitem__("resources", []), "must be a mapping"),
-    (lambda r: r.__setitem__("resources", {1: 2}), "can only have string keys"),
-  ])
+  @pytest.mark.parametrize(
+    "mutator,expected_message",
+    [
+      (lambda r: r.__setitem__("name", ""), "name cannot be an empty string"),
+      (lambda r: r.__setitem__("name", 1), "name must be a string"),
+      (lambda r: r.__setitem__("name", {}), "name must be a string"),
+      (lambda r: r.__setitem__("run", {}), "must be a command"),
+      (lambda r: r.__setitem__("run", [1, 2, 3]), "has some non-string arguments"),
+      (lambda r: r.__setitem__("resources", []), "must be a mapping"),
+      (lambda r: r.__setitem__("resources", {1: 2}), "can only have string keys"),
+    ],
+  )
   def test_invalid_run(self, mutator, expected_message):
     run_input = copy.deepcopy(VALID_RUN_INPUT)
     mutator(run_input)
     with pytest.raises(ValidationError) as validation_error:
       validate_run_input(run_input)
     assert expected_message in str(validation_error)
 
-  @pytest.mark.parametrize("mutator,check", [
-    (lambda r: r, lambda r: r["name"] == "test run"),
-    (lambda r: r, lambda r: r["run"] == ["sh", "-c", "python test.py"]),
-    (lambda r: r.__setitem__("run", ["python", "test.py"]), lambda r: r["run"] == ["python", "test.py"]),
-    (lambda r: r.__delitem__("run"), lambda r: r["run"] == []),
-    (lambda r: r.__setitem__("run", None), lambda r: r["run"] == []),
-    (lambda r: r, lambda r: r["resources"] == {"gpus": 2}),
-    (lambda r: r.__delitem__("resources"), lambda r: r["resources"] == {}),
-  ])
+  @pytest.mark.parametrize(
+    "mutator,check",
+    [
+      (lambda r: r, lambda r: r["name"] == "test run"),
+      (lambda r: r, lambda r: r["run"] == ["sh", "-c", "python test.py"]),
+      (
+        lambda r: r.__setitem__("run", ["python", "test.py"]),
+        lambda r: r["run"] == ["python", "test.py"],
+      ),
+      (lambda r: r.__delitem__("run"), lambda r: r["run"] == []),
+      (lambda r: r.__setitem__("run", None), lambda r: r["run"] == []),
+      (lambda r: r, lambda r: r["resources"] == {"gpus": 2}),
+      (lambda r: r.__delitem__("resources"), lambda r: r["resources"] == {}),
+    ],
+  )
   def test_valid_run(self, mutator, check):
     run_input = copy.deepcopy(VALID_RUN_INPUT)
     mutator(run_input)
     validated = validate_run_input(run_input)
     assert check(validated)
```

### Comparing `sigopt-8.8.0/test/xgboost/test_experiment_config.py` & `sigopt-8.8.1/test/xgboost/test_experiment_config.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,80 +1,58 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 import copy
-from mock import Mock
+
 import pytest
+from mock import Mock
 
-from sigopt.xgboost.constants import (
-  DEFAULT_CLASSIFICATION_METRIC,
-  DEFAULT_EVALS_NAME,
-  DEFAULT_REGRESSION_METRIC,
-  PARAMETER_INFORMATION,
-  SUPPORTED_AUTOBOUND_PARAMS,
-)
+from sigopt.xgboost.constants import DEFAULT_CLASSIFICATION_METRIC, DEFAULT_EVALS_NAME, DEFAULT_REGRESSION_METRIC
 from sigopt.xgboost.experiment import XGBExperiment
 
+
 EXPERIMENT_CONFIG_BASE = dict(
-  name='Single metric optimization',
-  type='offline',
+  name="Single metric optimization",
+  type="offline",
   parameters=[
-    dict(
-      name='eta',
-      type='double',
-      bounds={'min': 0.1, 'max': 0.5}
-    ),
-    dict(
-      name='max_depth',
-      type='int',
-      bounds={'min': 2, 'max': 6}
-    ),
-    dict(
-      name='num_boost_round',
-      type='int',
-      bounds={'min': 2, 'max': 6}
-    )
-  ],
-  metrics=[
-    dict(
-      name='accuracy',
-      strategy='optimize',
-      objective='maximize'
-    )
+    dict(name="eta", type="double", bounds={"min": 0.1, "max": 0.5}),
+    dict(name="max_depth", type="int", bounds={"min": 2, "max": 6}),
+    dict(name="num_boost_round", type="int", bounds={"min": 2, "max": 6}),
   ],
+  metrics=[dict(name="accuracy", strategy="optimize", objective="maximize")],
   parallel_bandwidth=1,
-  budget=2
+  budget=2,
 )
 PARAMS_BASE = {
-  'num_class': 3,
-  'lambda': 1,
+  "num_class": 3,
+  "lambda": 1,
 }
 
 
 def verify_experiment_config_integrity(experiment_config):
   assert isinstance(experiment_config, dict)
-  assert 'type' in experiment_config
-  assert 'parameters' in experiment_config
-  assert 'metrics' in experiment_config
-  assert 'budget' in experiment_config
+  assert "type" in experiment_config
+  assert "parameters" in experiment_config
+  assert "metrics" in experiment_config
+  assert "budget" in experiment_config
 
-  parameters = experiment_config['parameters']
+  parameters = experiment_config["parameters"]
   for parameter in parameters:
-    assert 'name' in parameter
-    assert 'type' in parameter
-    if parameter['type'] in ['int', 'double']:
-      assert 'bounds' in parameter
+    assert "name" in parameter
+    assert "type" in parameter
+    if parameter["type"] in ["int", "double"]:
+      assert "bounds" in parameter
     else:
-      assert 'categorical_values' in parameter
+      assert "categorical_values" in parameter
 
-  metrics = experiment_config['metrics']
+  metrics = experiment_config["metrics"]
   for metric in metrics:
-    assert 'name' in metric
-    assert 'strategy' in metric
-    assert 'objective' in metric
+    assert "name" in metric
+    assert "strategy" in metric
+    assert "objective" in metric
 
 
 def parse_and_create_aiexperiment_config(experiment_config, params):
   num_boost_round = None
   run_options = None
   early_stopping_rounds = 10
   d_train = Mock()
@@ -102,169 +80,165 @@
     experiment_config = copy.deepcopy(EXPERIMENT_CONFIG_BASE)
     params = copy.deepcopy(PARAMS_BASE)
     self.verify_integrity(experiment_config, params)
 
   def test_config_no_search_space(self):
     experiment_config = copy.deepcopy(EXPERIMENT_CONFIG_BASE)
     params = copy.deepcopy(PARAMS_BASE)
-    del experiment_config['parameters']
+    del experiment_config["parameters"]
     self.verify_integrity(experiment_config, params)
 
   def test_config_search_space_name_only(self):
     experiment_config = copy.deepcopy(EXPERIMENT_CONFIG_BASE)
     params = copy.deepcopy(PARAMS_BASE)
-    for parameter in experiment_config['parameters']:
-      del parameter['type']
-      del parameter['bounds']
+    for parameter in experiment_config["parameters"]:
+      del parameter["type"]
+      del parameter["bounds"]
     self.verify_integrity(experiment_config, params)
 
   def test_config_detect_log_transformation(self):
     experiment_config = copy.deepcopy(EXPERIMENT_CONFIG_BASE)
     params = copy.deepcopy(PARAMS_BASE)
-    experiment_config['parameters'] = [dict(name='eta')]
+    experiment_config["parameters"] = [dict(name="eta")]
     xgb_experiment = parse_and_create_aiexperiment_config(experiment_config, params)
-    assert xgb_experiment.experiment_config_parsed['parameters'][0]['transformation'] == 'log'
+    assert xgb_experiment.experiment_config_parsed["parameters"][0]["transformation"] == "log"
 
   def test_config_search_space_mixed(self):
     experiment_config = copy.deepcopy(EXPERIMENT_CONFIG_BASE)
     params = copy.deepcopy(PARAMS_BASE)
-    del experiment_config['parameters'][2]['type']
-    del experiment_config['parameters'][2]['bounds']
+    del experiment_config["parameters"][2]["type"]
+    del experiment_config["parameters"][2]["bounds"]
     self.verify_integrity(experiment_config, params)
 
   def test_config_search_space_wrong_type(self):
     experiment_config = copy.deepcopy(EXPERIMENT_CONFIG_BASE)
     params = copy.deepcopy(PARAMS_BASE)
-    experiment_config['parameters'][0]['type'] = 'int'
-    del experiment_config['parameters'][0]['bounds']
+    experiment_config["parameters"][0]["type"] = "int"
+    del experiment_config["parameters"][0]["bounds"]
     with pytest.raises(ValueError):
       self.verify_integrity(experiment_config, params)
 
   def test_config_search_space_no_type(self):
     experiment_config = copy.deepcopy(EXPERIMENT_CONFIG_BASE)
     params = copy.deepcopy(PARAMS_BASE)
-    del experiment_config['parameters'][0]['type']
-    del experiment_config['parameters'][1]['type']
-    del experiment_config['parameters'][2]['type']
+    del experiment_config["parameters"][0]["type"]
+    del experiment_config["parameters"][1]["type"]
+    del experiment_config["parameters"][2]["type"]
     self.verify_integrity(experiment_config, params)
 
   def test_config_search_space_categories_no_type(self):
     experiment_config = copy.deepcopy(EXPERIMENT_CONFIG_BASE)
     params = copy.deepcopy(PARAMS_BASE)
-    experiment_config['parameters'].append(
+    experiment_config["parameters"].append(
       dict(
-        name='tree_method',
-        categorical_values=['auto', 'exact', 'hist', 'gpu_hist'],
+        name="tree_method",
+        categorical_values=["auto", "exact", "hist", "gpu_hist"],
       )
     )
     self.verify_integrity(experiment_config, params)
 
   def test_config_search_space_no_categorical_values(self):
     experiment_config = copy.deepcopy(EXPERIMENT_CONFIG_BASE)
     params = copy.deepcopy(PARAMS_BASE)
-    experiment_config['parameters'].append(
+    experiment_config["parameters"].append(
       dict(
-        name='tree_method',
-        type='categorical',
+        name="tree_method",
+        type="categorical",
       )
     )
     with pytest.raises(ValueError):
       self.verify_integrity(experiment_config, params)
 
   def test_config_search_space_wrong_categories(self):
     experiment_config = copy.deepcopy(EXPERIMENT_CONFIG_BASE)
     params = copy.deepcopy(PARAMS_BASE)
-    experiment_config['parameters'].append(
+    experiment_config["parameters"].append(
       dict(
-        name='tree_method',
-        type='categorical',
-        categorical_values=['auto', 'exact', 'hist', 'gpu_hist', 'WrongCategory'],
+        name="tree_method",
+        type="categorical",
+        categorical_values=["auto", "exact", "hist", "gpu_hist", "WrongCategory"],
       )
     )
     with pytest.raises(ValueError):
       self.verify_integrity(experiment_config, params)
 
   def test_config_search_space_fake_categories(self):
     experiment_config = copy.deepcopy(EXPERIMENT_CONFIG_BASE)
     params = copy.deepcopy(PARAMS_BASE)
-    experiment_config['parameters'].append(
+    experiment_config["parameters"].append(
       dict(
-        name='foo',
-        type='categorical',
-        categorical_values=['auto', 'exact', 'hist', 'gpu_hist', 'WrongCategory'],
+        name="foo",
+        type="categorical",
+        categorical_values=["auto", "exact", "hist", "gpu_hist", "WrongCategory"],
       )
     )
     self.verify_integrity(experiment_config, params)
 
   def test_config_no_supported_bounds(self):
     experiment_config = copy.deepcopy(EXPERIMENT_CONFIG_BASE)
-    experiment_config['parameters'].append(dict(name='max_leaves'))
+    experiment_config["parameters"].append(dict(name="max_leaves"))
     params = copy.deepcopy(PARAMS_BASE)
     with pytest.raises(ValueError):
       self.verify_integrity(experiment_config, params)
 
   def test_autodetect_metric_from_objective(self):
     experiment_config = copy.deepcopy(EXPERIMENT_CONFIG_BASE)
-    del experiment_config['metrics']
+    del experiment_config["metrics"]
     params = copy.deepcopy(PARAMS_BASE)
 
-    params['objective'] = 'binary:logistic'
+    params["objective"] = "binary:logistic"
     xgb_experiment = parse_and_create_aiexperiment_config(experiment_config, params)
-    assert xgb_experiment.experiment_config_parsed['metrics'][0]['name'] == '-'.join(
+    assert xgb_experiment.experiment_config_parsed["metrics"][0]["name"] == "-".join(
       (DEFAULT_EVALS_NAME, DEFAULT_CLASSIFICATION_METRIC)
     )
 
-    params['objective'] = 'multi:softmax'
+    params["objective"] = "multi:softmax"
     xgb_experiment = parse_and_create_aiexperiment_config(experiment_config, params)
-    assert xgb_experiment.experiment_config_parsed['metrics'][0]['name'] == '-'.join(
+    assert xgb_experiment.experiment_config_parsed["metrics"][0]["name"] == "-".join(
       (DEFAULT_EVALS_NAME, DEFAULT_CLASSIFICATION_METRIC)
     )
 
-    params['objective'] = 'reg:squarederror'
+    params["objective"] = "reg:squarederror"
     xgb_experiment = parse_and_create_aiexperiment_config(experiment_config, params)
-    assert xgb_experiment.experiment_config_parsed['metrics'][0]['name'] == '-'.join(
+    assert xgb_experiment.experiment_config_parsed["metrics"][0]["name"] == "-".join(
       (DEFAULT_EVALS_NAME, DEFAULT_REGRESSION_METRIC)
     )
 
   def test_config_metric_string_only(self):
     experiment_config = copy.deepcopy(EXPERIMENT_CONFIG_BASE)
     params = copy.deepcopy(PARAMS_BASE)
-    experiment_config['metrics'] = 'accuracy'
+    experiment_config["metrics"] = "accuracy"
     self.verify_integrity(experiment_config, params)
 
   def test_config_metric_list(self):
     experiment_config = copy.deepcopy(EXPERIMENT_CONFIG_BASE)
-    experiment_config['metrics'].append(dict(
-      name='f1',
-      strategy='store',
-      objective='maximize'
-    ))
+    experiment_config["metrics"].append(dict(name="f1", strategy="store", objective="maximize"))
     params = copy.deepcopy(PARAMS_BASE)
     self.verify_integrity(experiment_config, params)
 
   def test_config_param_defined_twice(self):
     experiment_config = copy.deepcopy(EXPERIMENT_CONFIG_BASE)
     params = copy.deepcopy(PARAMS_BASE)
-    params['eta'] = 0.1
+    params["eta"] = 0.1
     with pytest.raises(ValueError):
       self.verify_integrity(experiment_config, params)
 
   def test_config_num_boost_round_defined_twice(self):
     experiment_config = copy.deepcopy(EXPERIMENT_CONFIG_BASE)
     params = copy.deepcopy(PARAMS_BASE)
-    params['num_boost_round'] = 10
+    params["num_boost_round"] = 10
     with pytest.raises(ValueError):
       self.verify_integrity(experiment_config, params)
 
   def test_config_wrong_metric_string(self):
     experiment_config = copy.deepcopy(EXPERIMENT_CONFIG_BASE)
-    experiment_config['metrics'] = 'NOT_A_METRIC_SUPPORTED'
+    experiment_config["metrics"] = "NOT_A_METRIC_SUPPORTED"
     params = copy.deepcopy(PARAMS_BASE)
     with pytest.raises(ValueError):
       self.verify_integrity(experiment_config, params)
 
   def test_config_wrong_metric_list(self):
     experiment_config = copy.deepcopy(EXPERIMENT_CONFIG_BASE)
-    experiment_config['metrics'][0]['name'] = 'NOT_A_METRIC_SUPPORTED'
+    experiment_config["metrics"][0]["name"] = "NOT_A_METRIC_SUPPORTED"
     params = copy.deepcopy(PARAMS_BASE)
     with pytest.raises(ValueError):
       self.verify_integrity(experiment_config, params)
```

### Comparing `sigopt-8.8.0/test/xgboost/test_run_options_parsing.py` & `sigopt-8.8.1/test/xgboost/test_run_options_parsing.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
-from mock import Mock
-import pytest
 import random
 
+import pytest
+from mock import Mock
+
 from sigopt.objects import TrainingRun
 from sigopt.run_context import RunContext
-from sigopt.xgboost.run import DEFAULT_RUN_OPTIONS, parse_run_options, XGBRunHandler
+from sigopt.xgboost.run import DEFAULT_RUN_OPTIONS, XGBRunHandler, parse_run_options
+
 from ..utils import ObserveWarnings
 
+
 class TestXGBoostKwargs(object):
   def test_xgboost_kwargs_remove_wrong_key(self):
     kwargs = {
       "WRONG_KEY_1": True,
       "WRONG_KEY_2": 3.14,
     }
     with ObserveWarnings() as ws:
@@ -28,15 +31,15 @@
         xgb_model=Mock(),
         callbacks=None,
         run_options=None,
         **kwargs
       )
       assert not xgb_run_handler.kwargs
       assert len(ws) == len(kwargs)
-      for w in ws:
+      for w in ws:  # pylint: disable=not-an-iterable
         assert issubclass(w.category, RuntimeWarning)
 
   def test_xgboost_kwargs_keep_right_key(self):
     xgb_run_handler = XGBRunHandler(
       params={"max_depth": 2},
       dtrain=Mock(),
       num_boost_round=21,
@@ -47,71 +50,70 @@
       xgb_model=None,
       callbacks=None,
       maximize=True,
       run_options={"autolog_metrics": True},
     )
     assert len(xgb_run_handler.kwargs) == 1
     assert "maximize" in xgb_run_handler.kwargs
-    assert xgb_run_handler.kwargs["maximize"] == True
+    assert xgb_run_handler.kwargs["maximize"] is True
+
 
 class TestRunOptionsParsing(object):
   def test_run_options_wrong_type(self):
     run_options = Mock(log_params=True)
     with pytest.raises(TypeError):
       parse_run_options(run_options)
 
   def test_run_options_wrong_keys(self):
     run_options = {
-      'autolog_metric': True,
+      "autolog_metric": True,
     }
     with pytest.raises(ValueError):
       parse_run_options(run_options)
 
   def test_run_options_autolog_not_bool(self):
     run_options = {
-      'autolog_metrics': 12,
+      "autolog_metrics": 12,
     }
     with pytest.raises(TypeError):
       parse_run_options(run_options)
 
   def test_run_options_run_and_name_keys(self):
     run_options = {
-      'name': 'test-run',
-      'run': Mock(),
+      "name": "test-run",
+      "run": Mock(),
     }
     with pytest.raises(ValueError):
       parse_run_options(run_options)
 
     run_options = {
-      'name': None,
-      'run': None,
+      "name": None,
+      "run": None,
     }
     assert parse_run_options(run_options)
 
     run_options = {
-      'name': "",
-      'run': None,
+      "name": "",
+      "run": None,
     }
     assert parse_run_options(run_options)
 
     run_options = {
-      'name': "",
-      'run': RunContext(Mock(), Mock(assignments={'a': 1})),
+      "name": "",
+      "run": RunContext(Mock(), Mock(assignments={"a": 1})),
     }
     assert parse_run_options(run_options)
 
   def test_run_options_run_context_object(self):
-    run_options = {
-      'run': TrainingRun(Mock())
-    }
+    run_options = {"run": TrainingRun(Mock())}
     with pytest.raises(TypeError):
       parse_run_options(run_options)
 
     run_options = {
-      'run': RunContext(Mock(), Mock(assignments={'a': 1})),
+      "run": RunContext(Mock(), Mock(assignments={"a": 1})),
     }
     assert parse_run_options(run_options)
 
   def test_run_options_fully_parsed(self):
     num_of_options = random.randint(1, len(DEFAULT_RUN_OPTIONS))
     run_options_keys = random.sample(DEFAULT_RUN_OPTIONS.keys(), num_of_options)
     run_options = {k: DEFAULT_RUN_OPTIONS[k] for k in run_options_keys}
```

