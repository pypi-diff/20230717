# Comparing `tmp/hypernets-0.2.5.7.tar.gz` & `tmp/hypernets-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypernets-0.2.5.7.tar", last modified: Thu Nov 24 02:43:05 2022, max compression
+gzip compressed data, was "hypernets-0.3.0.tar", last modified: Mon Jul 17 15:14:38 2023, max compression
```

## Comparing `hypernets-0.2.5.7.tar` & `hypernets-0.3.0.tar`

### file list

```diff
@@ -1,328 +1,342 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 02:43:05.680426 hypernets-0.2.5.7/
--rw-r--r--   0 runner    (1001) docker     (122)    10142 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     5738 2022-11-24 02:43:05.680426 hypernets-0.2.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4498 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 02:43:05.612427 hypernets-0.2.5.7/hypernets/
--rw-r--r--   0 runner    (1001) docker     (122)       71 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 02:43:05.616427 hypernets-0.2.5.7/hypernets/conf/
--rw-r--r--   0 runner    (1001) docker     (122)      199 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2443 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/conf/_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 02:43:05.616427 hypernets-0.2.5.7/hypernets/core/
--rw-r--r--   0 runner    (1001) docker     (122)      749 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15002 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/core/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (122)       55 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/core/config.py
--rw-r--r--   0 runner    (1001) docker     (122)      400 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/core/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     2324 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/core/meta_learner.py
--rw-r--r--   0 runner    (1001) docker     (122)     2156 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/core/mutables.py
--rw-r--r--   0 runner    (1001) docker     (122)    11636 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/core/ops.py
--rw-r--r--   0 runner    (1001) docker     (122)      563 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/core/random_state.py
--rw-r--r--   0 runner    (1001) docker     (122)    35716 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/core/search_space.py
--rw-r--r--   0 runner    (1001) docker     (122)     1812 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/core/searcher.py
--rw-r--r--   0 runner    (1001) docker     (122)      211 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/core/stateful.py
--rw-r--r--   0 runner    (1001) docker     (122)    17641 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/core/trial.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 02:43:05.620427 hypernets-0.2.5.7/hypernets/discriminators/
--rw-r--r--   0 runner    (1001) docker     (122)     1483 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/discriminators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2742 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/discriminators/_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     4714 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/discriminators/percentile.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 02:43:05.620427 hypernets-0.2.5.7/hypernets/dispatchers/
--rw-r--r--   0 runner    (1001) docker     (122)     1320 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/dispatchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1779 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/dispatchers/cfg.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 02:43:05.620427 hypernets-0.2.5.7/hypernets/dispatchers/cluster/
--rw-r--r--   0 runner    (1001) docker     (122)      129 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/dispatchers/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6592 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/dispatchers/cluster/cluster.py
--rw-r--r--   0 runner    (1001) docker     (122)     6589 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/dispatchers/cluster/driver_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     4645 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/dispatchers/cluster/executor_dispatcher.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 02:43:05.620427 hypernets-0.2.5.7/hypernets/dispatchers/cluster/grpc/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/dispatchers/cluster/grpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 02:43:05.624427 hypernets-0.2.5.7/hypernets/dispatchers/cluster/grpc/proto/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/dispatchers/cluster/grpc/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11944 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/dispatchers/cluster/grpc/proto/spec_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)     2812 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/dispatchers/cluster/grpc/proto/spec_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)     5122 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/dispatchers/cluster/grpc/search_driver_client.py
--rw-r--r--   0 runner    (1001) docker     (122)    13398 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/dispatchers/cluster/grpc/search_driver_service.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 02:43:05.624427 hypernets-0.2.5.7/hypernets/dispatchers/dask/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/dispatchers/dask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10766 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/dispatchers/dask/dask_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     5588 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/dispatchers/in_process_dispatcher.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 02:43:05.624427 hypernets-0.2.5.7/hypernets/dispatchers/predict/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/dispatchers/predict/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 02:43:05.624427 hypernets-0.2.5.7/hypernets/dispatchers/predict/grpc/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/dispatchers/predict/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1159 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/dispatchers/predict/grpc/predict_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     1576 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/dispatchers/predict/grpc/predict_service.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 02:43:05.624427 hypernets-0.2.5.7/hypernets/dispatchers/predict/grpc/proto/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/dispatchers/predict/grpc/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6292 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/dispatchers/predict/grpc/proto/predict_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)     1853 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/dispatchers/predict/grpc/proto/predict_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)     6631 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/dispatchers/predict/predict_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 02:43:05.624427 hypernets-0.2.5.7/hypernets/dispatchers/process/
--rw-r--r--   0 runner    (1001) docker     (122)      138 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/dispatchers/process/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 02:43:05.624427 hypernets-0.2.5.7/hypernets/dispatchers/process/grpc/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/dispatchers/process/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4602 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/dispatchers/process/grpc/process_broker_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     6470 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/dispatchers/process/grpc/process_broker_service.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 02:43:05.628427 hypernets-0.2.5.7/hypernets/dispatchers/process/grpc/proto/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/dispatchers/process/grpc/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11144 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/dispatchers/process/grpc/proto/proc_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)     2821 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/dispatchers/process/grpc/proto/proc_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1704 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/dispatchers/process/grpc_process.py
--rw-r--r--   0 runner    (1001) docker     (122)     1835 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/dispatchers/process/local_process.py
--rw-r--r--   0 runner    (1001) docker     (122)     3517 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/dispatchers/process/ssh_process.py
--rw-r--r--   0 runner    (1001) docker     (122)     2534 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/dispatchers/run.py
--rw-r--r--   0 runner    (1001) docker     (122)      968 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/dispatchers/run_broker.py
--rw-r--r--   0 runner    (1001) docker     (122)     1005 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/dispatchers/run_predict.py
--rw-r--r--   0 runner    (1001) docker     (122)      606 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/dispatchers/run_predict_server.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 02:43:05.628427 hypernets-0.2.5.7/hypernets/examples/
--rw-r--r--   0 runner    (1001) docker     (122)       55 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15809 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/examples/plain_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1294 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/examples/smoke_testing.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 02:43:05.628427 hypernets-0.2.5.7/hypernets/experiment/
--rw-r--r--   0 runner    (1001) docker     (122)      682 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/experiment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    21712 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/experiment/_callback.py
--rw-r--r--   0 runner    (1001) docker     (122)     5977 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/experiment/_experiment.py
--rw-r--r--   0 runner    (1001) docker     (122)    24512 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/experiment/_extractor.py
--rw-r--r--   0 runner    (1001) docker     (122)    16045 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/experiment/_maker.py
--rw-r--r--   0 runner    (1001) docker     (122)     2177 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/experiment/cfg.py
--rw-r--r--   0 runner    (1001) docker     (122)    96617 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/experiment/compete.py
--rw-r--r--   0 runner    (1001) docker     (122)     2043 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/experiment/general.py
--rw-r--r--   0 runner    (1001) docker     (122)     3033 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/experiment/job.py
--rw-r--r--   0 runner    (1001) docker     (122)    34851 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/experiment/report.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 02:43:05.632427 hypernets-0.2.5.7/hypernets/hyperctl/
--rw-r--r--   0 runner    (1001) docker     (122)       50 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/hyperctl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1335 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/hyperctl/api.py
--rw-r--r--   0 runner    (1001) docker     (122)     6536 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/hyperctl/appliation.py
--rw-r--r--   0 runner    (1001) docker     (122)     7227 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/hyperctl/batch.py
--rw-r--r--   0 runner    (1001) docker     (122)     9098 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/hyperctl/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (122)    11836 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/hyperctl/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     1364 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/hyperctl/consts.py
--rw-r--r--   0 runner    (1001) docker     (122)    14975 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/hyperctl/executor.py
--rw-r--r--   0 runner    (1001) docker     (122)    11312 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/hyperctl/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (122)     5065 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/hyperctl/server.py
--rw-r--r--   0 runner    (1001) docker     (122)     1495 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/hyperctl/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 02:43:05.632427 hypernets-0.2.5.7/hypernets/model/
--rw-r--r--   0 runner    (1001) docker     (122)      150 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5084 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/model/estimator.py
--rw-r--r--   0 runner    (1001) docker     (122)    10589 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/model/hyper_model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 02:43:05.632427 hypernets-0.2.5.7/hypernets/pipeline/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6947 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/pipeline/base.py
--rw-r--r--   0 runner    (1001) docker     (122)    16376 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/pipeline/transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 02:43:05.636427 hypernets-0.2.5.7/hypernets/searchers/
--rw-r--r--   0 runner    (1001) docker     (122)     1911 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/searchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8298 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/searchers/evolution_searcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     2019 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/searchers/grid_searcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     7263 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/searchers/mcts_core.py
--rw-r--r--   0 runner    (1001) docker     (122)     4836 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/searchers/mcts_searcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     1165 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/searchers/playback_searcher.py
--rw-r--r--   0 runner    (1001) docker     (122)      754 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/searchers/random_searcher.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 02:43:05.636427 hypernets-0.2.5.7/hypernets/server/
--rw-r--r--   0 runner    (1001) docker     (122)       55 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 02:43:05.636427 hypernets-0.2.5.7/hypernets/tabular/
--rw-r--r--   0 runner    (1001) docker     (122)      704 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4223 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/_base.py
--rw-r--r--   0 runner    (1001) docker     (122)    10041 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/cache.py
--rw-r--r--   0 runner    (1001) docker     (122)     2639 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/cfg.py
--rw-r--r--   0 runner    (1001) docker     (122)     2908 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/collinearity.py
--rw-r--r--   0 runner    (1001) docker     (122)    12451 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/column_selector.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 02:43:05.640426 hypernets-0.2.5.7/hypernets/tabular/cuml_ex/
--rw-r--r--   0 runner    (1001) docker     (122)      147 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/cuml_ex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2117 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/cuml_ex/_data_cleaner.py
--rw-r--r--   0 runner    (1001) docker     (122)      978 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/cuml_ex/_data_hasher.py
--rw-r--r--   0 runner    (1001) docker     (122)     2110 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/cuml_ex/_dataframe_mapper.py
--rw-r--r--   0 runner    (1001) docker     (122)      742 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/cuml_ex/_drift_detection.py
--rw-r--r--   0 runner    (1001) docker     (122)     1155 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/cuml_ex/_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (122)     3536 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/cuml_ex/_estimator.py
--rw-r--r--   0 runner    (1001) docker     (122)      564 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/cuml_ex/_estimator_detector.py
--rw-r--r--   0 runner    (1001) docker     (122)     5077 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/cuml_ex/_metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)     2484 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/cuml_ex/_model_selection.py
--rw-r--r--   0 runner    (1001) docker     (122)     1216 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/cuml_ex/_persistence.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      657 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/cuml_ex/_pseudo_labeling.py
--rw-r--r--   0 runner    (1001) docker     (122)    25168 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/cuml_ex/_toolbox.py
--rw-r--r--   0 runner    (1001) docker     (122)    19032 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/cuml_ex/_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 02:43:05.644426 hypernets-0.2.5.7/hypernets/tabular/dask_ex/
--rw-r--r--   0 runner    (1001) docker     (122)      919 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/dask_ex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      523 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/dask_ex/_collinearity.py
--rw-r--r--   0 runner    (1001) docker     (122)     2160 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/dask_ex/_data_cleaner.py
--rw-r--r--   0 runner    (1001) docker     (122)     1200 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/dask_ex/_data_hasher.py
--rw-r--r--   0 runner    (1001) docker     (122)     1677 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/dask_ex/_dataframe_mapper.py
--rw-r--r--   0 runner    (1001) docker     (122)      605 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/dask_ex/_drift_detection.py
--rw-r--r--   0 runner    (1001) docker     (122)     7448 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/dask_ex/_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (122)      443 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/dask_ex/_feature_generators.py
--rw-r--r--   0 runner    (1001) docker     (122)     3020 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/dask_ex/_metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)      747 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/dask_ex/_model_selection.py
--rw-r--r--   0 runner    (1001) docker     (122)     4336 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/dask_ex/_persistence.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3530 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/dask_ex/_pseudo_labeling.py
--rw-r--r--   0 runner    (1001) docker     (122)    31068 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/dask_ex/_toolbox.py
--rw-r--r--   0 runner    (1001) docker     (122)    30795 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/dask_ex/_transformers.py
--rw-r--r--   0 runner    (1001) docker     (122)    14773 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/data_cleaner.py
--rw-r--r--   0 runner    (1001) docker     (122)     2855 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/data_hasher.py
--rw-r--r--   0 runner    (1001) docker     (122)    19548 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/dataframe_mapper.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 02:43:05.648426 hypernets-0.2.5.7/hypernets/tabular/datasets/
--rw-r--r--   0 runner    (1001) docker     (122)   728875 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/datasets/Bike_Sharing.csv
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   440029 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/datasets/adult-uci.csv.gz
--rw-r--r--   0 runner    (1001) docker     (122)    70855 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/datasets/bank-uci.csv.gz
--rw-r--r--   0 runner    (1001) docker     (122)    10521 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/datasets/blood.csv
--rw-r--r--   0 runner    (1001) docker     (122)     1575 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/datasets/dsutils.py
--rw-r--r--   0 runner    (1001) docker     (122)    11903 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/datasets/glass_uci.csv
--rw-r--r--   0 runner    (1001) docker     (122)    11024 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/datasets/heart-disease-uci.csv
--rw-r--r--   0 runner    (1001) docker     (122)    15155 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/datasets/movielens_sample.txt
--rw-r--r--   0 runner    (1001) docker     (122)  1477467 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/datasets/telescope.csv
--rw-r--r--   0 runner    (1001) docker     (122)    19076 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/drift_detection.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 02:43:05.652426 hypernets-0.2.5.7/hypernets/tabular/ensemble/
--rw-r--r--   0 runner    (1001) docker     (122)      190 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7871 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/ensemble/base_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (122)     2096 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/ensemble/stacking.py
--rw-r--r--   0 runner    (1001) docker     (122)     7932 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/ensemble/voting.py
--rw-r--r--   0 runner    (1001) docker     (122)     2821 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/estimator_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 02:43:05.652426 hypernets-0.2.5.7/hypernets/tabular/evaluator/
--rw-r--r--   0 runner    (1001) docker     (122)      101 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/evaluator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2489 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/evaluator/_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1261 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/evaluator/auto_sklearn.py
--rw-r--r--   0 runner    (1001) docker     (122)     1029 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/evaluator/h2o.py
--rw-r--r--   0 runner    (1001) docker     (122)     2256 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/evaluator/hyperdt.py
--rw-r--r--   0 runner    (1001) docker     (122)     5536 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/evaluator/hypergbm.py
--rw-r--r--   0 runner    (1001) docker     (122)     6401 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/evaluator/tests.py
--rw-r--r--   0 runner    (1001) docker     (122)     1195 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/evaluator/tpot.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 02:43:05.652426 hypernets-0.2.5.7/hypernets/tabular/feature_generators/
--rw-r--r--   0 runner    (1001) docker     (122)      211 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/feature_generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      496 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/feature_generators/_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     4588 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/feature_generators/_primitives.py
--rw-r--r--   0 runner    (1001) docker     (122)    14389 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/feature_generators/_transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 02:43:05.652426 hypernets-0.2.5.7/hypernets/tabular/lifelong_learning/
--rw-r--r--   0 runner    (1001) docker     (122)      110 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/lifelong_learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4647 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/lifelong_learning/_split.py
--rw-r--r--   0 runner    (1001) docker     (122)       57 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/lifelong_learning/_validation.py
--rw-r--r--   0 runner    (1001) docker     (122)    11839 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)     3996 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/persistence.py
--rw-r--r--   0 runner    (1001) docker     (122)     3363 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/pseudo_labeling.py
--rw-r--r--   0 runner    (1001) docker     (122)    53861 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/sklearn_ex.py
--rw-r--r--   0 runner    (1001) docker     (122)    28504 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tabular/toolbox.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 02:43:05.656427 hypernets-0.2.5.7/hypernets/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      270 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 02:43:05.656427 hypernets-0.2.5.7/hypernets/tests/board/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/board/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 02:43:05.656427 hypernets-0.2.5.7/hypernets/tests/core/
--rw-r--r--   0 runner    (1001) docker     (122)       55 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1909 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/core/callback_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    14247 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/core/connection_space_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    14749 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/core/hyper_space_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1106 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/core/mutable_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     9927 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/core/parameter_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 02:43:05.656427 hypernets-0.2.5.7/hypernets/tests/discriminators/
--rw-r--r--   0 runner    (1001) docker     (122)     1327 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/discriminators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1173 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/discriminators/base_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2469 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/discriminators/percentile.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 02:43:05.656427 hypernets-0.2.5.7/hypernets/tests/dispatchers/
--rw-r--r--   0 runner    (1001) docker     (122)       55 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/dispatchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1527 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/dispatchers/process_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 02:43:05.660426 hypernets-0.2.5.7/hypernets/tests/experiment/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/experiment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6826 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/experiment/compete_experiment_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     7841 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/experiment/experiment_factory.py
--rw-r--r--   0 runner    (1001) docker     (122)     4224 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/experiment/extractor_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1988 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/experiment/general_experiment_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2996 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/experiment/job_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    11758 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/experiment/make_experiment_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     5406 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/experiment/report_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      924 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/experiment/run_export_experiment_report.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 02:43:05.660426 hypernets-0.2.5.7/hypernets/tests/hyperctl/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/hyperctl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2694 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/hyperctl/batch_factory.py
--rw-r--r--   0 runner    (1001) docker     (122)      160 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/hyperctl/plain_job_script.py
--rw-r--r--   0 runner    (1001) docker     (122)     3653 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/hyperctl/test_application.py
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/hyperctl/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (122)      651 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/hyperctl/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (122)    14332 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/hyperctl/test_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 02:43:05.660426 hypernets-0.2.5.7/hypernets/tests/model/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1371 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/model/plain_model_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 02:43:05.660426 hypernets-0.2.5.7/hypernets/tests/pipeline/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6091 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/pipeline/pipeline_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 02:43:05.664426 hypernets-0.2.5.7/hypernets/tests/searchers/
--rw-r--r--   0 runner    (1001) docker     (122)       55 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/searchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6994 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/searchers/evolution_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2763 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/searchers/grid_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     7332 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/searchers/mcts_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1243 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/searchers/playback_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     3002 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/searchers/random_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 02:43:05.664426 hypernets-0.2.5.7/hypernets/tests/tabular/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/tabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1892 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/tabular/cache_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2976 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/tabular/column_selector_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     6864 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/tabular/data_cleaner_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     5170 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/tabular/drift_detection_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 02:43:05.664426 hypernets-0.2.5.7/hypernets/tests/tabular/ensemble/
--rw-r--r--   0 runner    (1001) docker     (122)       55 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/tabular/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6398 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/tabular/ensemble/ensemble_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     8705 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/tabular/feature_generator_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     3411 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/tabular/feature_importance_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 02:43:05.664426 hypernets-0.2.5.7/hypernets/tests/tabular/lifelong_learning/
--rw-r--r--   0 runner    (1001) docker     (122)       55 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/tabular/lifelong_learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4557 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/tabular/lifelong_learning/split_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2898 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/tabular/persitence_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2172 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/tabular/psudo_labeling_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    14685 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/tabular/sklearn_transformer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 02:43:05.668426 hypernets-0.2.5.7/hypernets/tests/tabular/tb_cuml/
--rw-r--r--   0 runner    (1001) docker     (122)      336 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/tabular/tb_cuml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2138 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/tabular/tb_cuml/cache_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      349 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/tabular/tb_cuml/data_cleaner_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     3460 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/tabular/tb_cuml/data_split_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2954 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/tabular/tb_cuml/drift_detection_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     5789 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/tabular/tb_cuml/estimator_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     5097 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/tabular/tb_cuml/experiment_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      461 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/tabular/tb_cuml/feature_importance_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      420 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/tabular/tb_cuml/psudo_labeling_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     3878 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/tabular/tb_cuml/toolbox_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     9848 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/tabular/tb_cuml/transformer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 02:43:05.672426 hypernets-0.2.5.7/hypernets/tests/tabular/tb_dask/
--rw-r--r--   0 runner    (1001) docker     (122)     1463 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/tabular/tb_dask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2222 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/tabular/tb_dask/cache_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2296 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/tabular/tb_dask/dask_ex_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     5728 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/tabular/tb_dask/dask_transofromer_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      394 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/tabular/tb_dask/data_cleaner_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     3355 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/tabular/tb_dask/drift_detection_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     8709 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/tabular/tb_dask/feature_generator_dask_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      490 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/tabular/tb_dask/feature_importance_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     3941 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/tabular/tb_dask/persitence_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      416 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/tabular/tb_dask/psudo_labeling_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1623 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/tabular/tb_dask/toolbox_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2265 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/tabular/toolbox_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1413 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/tabular/utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 02:43:05.672426 hypernets-0.2.5.7/hypernets/tests/trial/
--rw-r--r--   0 runner    (1001) docker     (122)       55 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/trial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2843 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/trial/trial_history_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1140 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/trial/trial_store_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 02:43:05.672426 hypernets-0.2.5.7/hypernets/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (122)       56 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1717 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/utils/common_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     8907 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/utils/df_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      698 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/utils/estimators_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      266 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/utils/perf_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     6857 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/utils/ssh_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1005 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/utils/tic_toc_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2301 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/tests/utils/tuning_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 02:43:05.680426 hypernets-0.2.5.7/hypernets/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      797 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2709 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/utils/_doc_lens.py
--rw-r--r--   0 runner    (1001) docker     (122)     4115 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/utils/_estimators.py
--rw-r--r--   0 runner    (1001) docker     (122)    13015 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/utils/_fsutils.py
--rw-r--r--   0 runner    (1001) docker     (122)     5390 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/utils/_perf.py
--rw-r--r--   0 runner    (1001) docker     (122)     6797 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/utils/_tic_tok.py
--rw-r--r--   0 runner    (1001) docker     (122)     6701 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (122)      371 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/utils/const.py
--rw-r--r--   0 runner    (1001) docker     (122)     6807 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/utils/df_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     9685 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (122)     5505 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/utils/param_tuning.py
--rw-r--r--   0 runner    (1001) docker     (122)     4069 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/hypernets/utils/ssh_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 02:43:05.616427 hypernets-0.2.5.7/hypernets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     5738 2022-11-24 02:43:05.000000 hypernets-0.2.5.7/hypernets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    11020 2022-11-24 02:43:05.000000 hypernets-0.2.5.7/hypernets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-24 02:43:05.000000 hypernets-0.2.5.7/hypernets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       57 2022-11-24 02:43:05.000000 hypernets-0.2.5.7/hypernets.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-24 02:43:05.000000 hypernets-0.2.5.7/hypernets.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      676 2022-11-24 02:43:05.000000 hypernets-0.2.5.7/hypernets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2022-11-24 02:43:05.000000 hypernets-0.2.5.7/hypernets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-24 02:43:05.680426 hypernets-0.2.5.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2687 2022-11-24 02:42:54.000000 hypernets-0.2.5.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:38.002404 hypernets-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-07-17 15:14:32.000000 hypernets-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7382 2023-07-17 15:14:38.002404 hypernets-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-07-17 15:14:32.000000 hypernets-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:37.962403 hypernets-0.3.0/hypernets/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:37.962403 hypernets-0.3.0/hypernets/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/conf/_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:37.966404 hypernets-0.3.0/hypernets/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15224 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/core/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/core/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/core/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/core/meta_learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/core/mutables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/core/objective.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11636 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/core/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/core/pareto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/core/random_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35716 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/core/search_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/core/searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/core/stateful.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21064 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/core/trial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:37.966404 hypernets-0.3.0/hypernets/discriminators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/discriminators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/discriminators/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/discriminators/percentile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:37.966404 hypernets-0.3.0/hypernets/dispatchers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/dispatchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/dispatchers/cfg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:37.966404 hypernets-0.3.0/hypernets/dispatchers/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/dispatchers/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/dispatchers/cluster/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/dispatchers/cluster/driver_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/dispatchers/cluster/executor_dispatcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:37.966404 hypernets-0.3.0/hypernets/dispatchers/cluster/grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/dispatchers/cluster/grpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:37.966404 hypernets-0.3.0/hypernets/dispatchers/cluster/grpc/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/dispatchers/cluster/grpc/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11944 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/dispatchers/cluster/grpc/proto/spec_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/dispatchers/cluster/grpc/proto/spec_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/dispatchers/cluster/grpc/search_driver_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13398 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/dispatchers/cluster/grpc/search_driver_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:37.966404 hypernets-0.3.0/hypernets/dispatchers/dask/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/dispatchers/dask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10774 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/dispatchers/dask/dask_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/dispatchers/in_process_dispatcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:37.966404 hypernets-0.3.0/hypernets/dispatchers/predict/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/dispatchers/predict/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:37.970404 hypernets-0.3.0/hypernets/dispatchers/predict/grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/dispatchers/predict/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/dispatchers/predict/grpc/predict_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/dispatchers/predict/grpc/predict_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:37.970404 hypernets-0.3.0/hypernets/dispatchers/predict/grpc/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/dispatchers/predict/grpc/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/dispatchers/predict/grpc/proto/predict_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/dispatchers/predict/grpc/proto/predict_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/dispatchers/predict/predict_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:37.970404 hypernets-0.3.0/hypernets/dispatchers/process/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/dispatchers/process/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:37.970404 hypernets-0.3.0/hypernets/dispatchers/process/grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/dispatchers/process/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/dispatchers/process/grpc/process_broker_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/dispatchers/process/grpc/process_broker_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:37.970404 hypernets-0.3.0/hypernets/dispatchers/process/grpc/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/dispatchers/process/grpc/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11144 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/dispatchers/process/grpc/proto/proc_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/dispatchers/process/grpc/proto/proc_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/dispatchers/process/grpc_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/dispatchers/process/local_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/dispatchers/process/ssh_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/dispatchers/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/dispatchers/run_broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/dispatchers/run_predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/dispatchers/run_predict_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:37.970404 hypernets-0.3.0/hypernets/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17458 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/examples/plain_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/examples/smoke_testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:37.974404 hypernets-0.3.0/hypernets/experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/experiment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22290 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/experiment/_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/experiment/_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24697 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/experiment/_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18691 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/experiment/_maker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/experiment/cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98518 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/experiment/compete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/experiment/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/experiment/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35007 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/experiment/report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:37.974404 hypernets-0.3.0/hypernets/hyperctl/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/hyperctl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/hyperctl/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/hyperctl/appliation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/hyperctl/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9098 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/hyperctl/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11837 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/hyperctl/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/hyperctl/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14975 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/hyperctl/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11312 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/hyperctl/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/hyperctl/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/hyperctl/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:37.974404 hypernets-0.3.0/hypernets/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/model/estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12670 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/model/hyper_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15258 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/model/objectives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:37.974404 hypernets-0.3.0/hypernets/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/pipeline/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16743 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/pipeline/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:37.978404 hypernets-0.3.0/hypernets/searchers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/searchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8241 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/searchers/evolution_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/searchers/genetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/searchers/grid_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7263 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/searchers/mcts_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/searchers/mcts_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15683 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/searchers/moead_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/searchers/moo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21619 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/searchers/nsga_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/searchers/playback_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/searchers/random_searcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:37.978404 hypernets-0.3.0/hypernets/server/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:37.978404 hypernets-0.3.0/hypernets/tabular/
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10609 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/collinearity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12448 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/column_selector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:37.982404 hypernets-0.3.0/hypernets/tabular/cuml_ex/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/cuml_ex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/cuml_ex/_data_cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/cuml_ex/_data_hasher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/cuml_ex/_dataframe_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/cuml_ex/_drift_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/cuml_ex/_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/cuml_ex/_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/cuml_ex/_estimator_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/cuml_ex/_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/cuml_ex/_model_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/cuml_ex/_persistence.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      657 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/cuml_ex/_pseudo_labeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25176 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/cuml_ex/_toolbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19278 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/cuml_ex/_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:37.982404 hypernets-0.3.0/hypernets/tabular/dask_ex/
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/dask_ex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/dask_ex/_collinearity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/dask_ex/_data_cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/dask_ex/_data_hasher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/dask_ex/_dataframe_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/dask_ex/_drift_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/dask_ex/_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/dask_ex/_feature_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/dask_ex/_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/dask_ex/_model_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/dask_ex/_persistence.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3530 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/dask_ex/_pseudo_labeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32072 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/dask_ex/_toolbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30804 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/dask_ex/_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14773 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/data_cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/data_hasher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19548 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/dataframe_mapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:37.986404 hypernets-0.3.0/hypernets/tabular/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)   728875 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/datasets/Bike_Sharing.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   440029 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/datasets/adult-uci.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    70855 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/datasets/bank-uci.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    10521 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/datasets/blood.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    12019 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/datasets/boston.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/datasets/dsutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11903 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/datasets/glass_uci.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/datasets/heart-disease-uci.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    15155 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/datasets/movielens_sample.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  1477467 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/datasets/telescope.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    19076 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/drift_detection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:37.986404 hypernets-0.3.0/hypernets/tabular/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/ensemble/base_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/ensemble/stacking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7932 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/ensemble/voting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/estimator_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:37.990404 hypernets-0.3.0/hypernets/tabular/evaluator/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/evaluator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/evaluator/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/evaluator/auto_sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/evaluator/h2o.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/evaluator/hyperdt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/evaluator/hypergbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/evaluator/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/evaluator/tpot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:37.990404 hypernets-0.3.0/hypernets/tabular/feature_generators/
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/feature_generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/feature_generators/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/feature_generators/_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14389 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/feature_generators/_transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:37.990404 hypernets-0.3.0/hypernets/tabular/lifelong_learning/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/lifelong_learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/lifelong_learning/_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/lifelong_learning/_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11839 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/pseudo_labeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55135 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/sklearn_ex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28678 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tabular/toolbox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:37.990404 hypernets-0.3.0/hypernets/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:37.990404 hypernets-0.3.0/hypernets/tests/board/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/board/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:37.990404 hypernets-0.3.0/hypernets/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/core/callback_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14247 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/core/connection_space_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14749 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/core/hyper_space_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/core/mutable_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9927 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/core/parameter_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:37.990404 hypernets-0.3.0/hypernets/tests/discriminators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/discriminators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/discriminators/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/discriminators/percentile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:37.990404 hypernets-0.3.0/hypernets/tests/dispatchers/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/dispatchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/dispatchers/process_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:37.994404 hypernets-0.3.0/hypernets/tests/experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/experiment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10078 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/experiment/compete_experiment_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7852 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/experiment/experiment_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/experiment/extractor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/experiment/general_experiment_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/experiment/job_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18462 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/experiment/make_experiment_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/experiment/report_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/experiment/run_export_experiment_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:37.994404 hypernets-0.3.0/hypernets/tests/hyperctl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/hyperctl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/hyperctl/batch_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/hyperctl/plain_job_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/hyperctl/test_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/hyperctl/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/hyperctl/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14334 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/hyperctl/test_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:37.994404 hypernets-0.3.0/hypernets/tests/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/model/plain_model_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10446 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/model/test_objectives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:37.994404 hypernets-0.3.0/hypernets/tests/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6091 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/pipeline/pipeline_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:37.994404 hypernets-0.3.0/hypernets/tests/searchers/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/searchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6994 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/searchers/evolution_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/searchers/grid_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/searchers/mcts_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/searchers/playback_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/searchers/random_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/searchers/test_genetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/searchers/test_moead_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/searchers/test_moo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10569 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/searchers/test_nsga2_searcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:37.998404 hypernets-0.3.0/hypernets/tests/tabular/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/tabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/tabular/cache_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/tabular/column_selector_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/tabular/data_cleaner_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/tabular/drift_detection_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:37.998404 hypernets-0.3.0/hypernets/tests/tabular/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/tabular/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/tabular/ensemble/ensemble_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8840 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/tabular/feature_generator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/tabular/feature_importance_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:37.998404 hypernets-0.3.0/hypernets/tests/tabular/lifelong_learning/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/tabular/lifelong_learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/tabular/lifelong_learning/split_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/tabular/persitence_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/tabular/psudo_labeling_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14770 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/tabular/sklearn_transformer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:37.998404 hypernets-0.3.0/hypernets/tests/tabular/tb_cuml/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/tabular/tb_cuml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/tabular/tb_cuml/cache_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/tabular/tb_cuml/data_cleaner_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/tabular/tb_cuml/data_split_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/tabular/tb_cuml/drift_detection_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/tabular/tb_cuml/estimator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/tabular/tb_cuml/experiment_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/tabular/tb_cuml/feature_importance_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/tabular/tb_cuml/psudo_labeling_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/tabular/tb_cuml/toolbox_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9848 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/tabular/tb_cuml/transformer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:38.002404 hypernets-0.3.0/hypernets/tests/tabular/tb_dask/
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/tabular/tb_dask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/tabular/tb_dask/cache_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/tabular/tb_dask/dask_ex_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/tabular/tb_dask/dask_transofromer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/tabular/tb_dask/data_cleaner_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/tabular/tb_dask/drift_detection_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8830 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/tabular/tb_dask/feature_generator_dask_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/tabular/tb_dask/feature_importance_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/tabular/tb_dask/persitence_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/tabular/tb_dask/psudo_labeling_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/tabular/tb_dask/toolbox_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/tabular/toolbox_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/tabular/utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:38.002404 hypernets-0.3.0/hypernets/tests/trial/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/trial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/trial/trial_history_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/trial/trial_store_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:38.002404 hypernets-0.3.0/hypernets/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/utils/common_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8860 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/utils/df_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/utils/estimators_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/utils/perf_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6857 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/utils/ssh_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/utils/tic_toc_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/tests/utils/tuning_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:38.002404 hypernets-0.3.0/hypernets/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/utils/_doc_lens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/utils/_estimators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13015 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/utils/_fsutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/utils/_perf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/utils/_tic_tok.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6701 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/utils/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6793 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/utils/df_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9988 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/utils/param_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-07-17 15:14:32.000000 hypernets-0.3.0/hypernets/utils/ssh_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:14:37.962403 hypernets-0.3.0/hypernets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7382 2023-07-17 15:14:37.000000 hypernets-0.3.0/hypernets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11522 2023-07-17 15:14:37.000000 hypernets-0.3.0/hypernets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 15:14:37.000000 hypernets-0.3.0/hypernets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-17 15:14:37.000000 hypernets-0.3.0/hypernets.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 15:14:37.000000 hypernets-0.3.0/hypernets.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-17 15:14:37.000000 hypernets-0.3.0/hypernets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-17 15:14:37.000000 hypernets-0.3.0/hypernets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 15:14:38.006404 hypernets-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-07-17 15:14:32.000000 hypernets-0.3.0/setup.py
```

### Comparing `hypernets-0.2.5.7/LICENSE` & `hypernets-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/PKG-INFO` & `hypernets-0.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: hypernets
-Version: 0.2.5.7
+Version: 0.3.0
 Summary: An General Automated Machine Learning Framework
-Home-page: 
+Home-page: https://github.com/DataCanvasIO/Hypernets
 Author: DataCanvas Community
 Author-email: yangjian@zetyun.com
 License: Apache License 2.0
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
@@ -17,54 +17,62 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6.*
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: dask
-Provides-Extra: notebook
 Provides-Extra: extra
+Provides-Extra: notebook
 Provides-Extra: board
 Provides-Extra: tests
 Provides-Extra: cuml
 Provides-Extra: zhcn
+Provides-Extra: dask
+Provides-Extra: fg
 Provides-Extra: all
 License-File: LICENSE
 
 <p align="center">
-<img src="docs/source/images/Hypernets.png" width="500" >
+<img src="https://raw.githubusercontent.com/DataCanvasIO/Hypernets/master/docs/source/images/Hypernets.png" width="500" >
 
 
 [![Python Versions](https://img.shields.io/pypi/pyversions/hypernets.svg)](https://pypi.org/project/hypernets)
 [![Downloads](https://pepy.tech/badge/hypernets)](https://pepy.tech/project/hypernets)
 [![PyPI Version](https://img.shields.io/pypi/v/hypernets.svg)](https://pypi.org/project/hypernets)
 
 ## We Are Hiring！
 Dear folks, we are offering challenging opportunities located in Beijing for both professionals and students who are keen on AutoML/NAS. Come be a part of DataCanvas! Please send your CV to yangjian@zetyun.com. (Application deadline: TBD.)  
 
 ## Hypernets: A General Automated Machine Learning Framework
 Hypernets is a general AutoML framework, based on which it can implement automatic optimization tools for various machine learning frameworks and libraries, including deep learning frameworks such as tensorflow, keras, pytorch, and machine learning libraries like sklearn, lightgbm, xgboost, etc.
+It also adopted various state-of-the-art optimization algorithms, including but not limited to evolution algorithm, monte carlo tree search for single objective optimization and multi-objective optimization algorithms such as MOEA/D,NSGA-II,R-NSGA-II.
 We introduced an abstract search space representation, taking into account the requirements of hyperparameter optimization and neural architecture search(NAS), making Hypernets a general framework that can adapt to various automated machine learning needs. As an abstraction computing layer, tabular toolbox, has successfully implemented in various tabular data types: pandas, dask, cudf, etc.  
 
 
 
 ## Overview
 ### Conceptual Model
 <p align="center">
-<img src="docs/source/images/hypernets_conceptual_model.png" width="100%"/>
+<img src="https://raw.githubusercontent.com/DataCanvasIO/Hypernets/master/docs/source/images/hypernets_conceptual_model.png" width="100%"/>
 </p>
 
 ### Illustration of the Search Space 
 <p align="center">
-<img src="docs/source/images/hypernets_search_space.png" width="100%"/>
+<img src="https://raw.githubusercontent.com/DataCanvasIO/Hypernets/master/docs/source/images/hypernets_search_space.png" width="100%"/>
 </p>
 
+## What's NEW !
+
+- **New feature:** [Multi-objectives optimization support](https://hypernets.readthedocs.io/en/latest/searchers.html#multi-objective-optimization)
+- **New feature:** [Performance and model complexity measurement metrics](https://github.com/DataCanvasIO/HyperGBM/blob/main/hypergbm/examples/66.Objectives_example.ipynb)
+- **New feature:** [Distributed computing](https://hypergbm.readthedocs.io/en/latest/example_dask.html) and [GPU acceleration](https://hypergbm.readthedocs.io/en/latest/example_cuml.html) base on computational abstraction layer
+
 
 ## Installation
 
 ### Conda
 
 Install Hypernets with `conda` from the channel *conda-forge*:
 
@@ -99,43 +107,62 @@
 
 * Install all above with one command:
 ```bash
 pip install hypernets[all]
 ```
 
 
-***Verify installation***:
+To ***Verify*** your installation:
 ```bash
 python -m hypernets.examples.smoke_testing
 ```
 
 ## Related Links
 
 * [A Brief Tutorial for Developing AutoML Tools with Hypernets](https://github.com/BochenLv/knn_toy_model/blob/main/Introduction.md)
 
-## Hypernets related projects
-* [Hypernets](https://github.com/DataCanvasIO/Hypernets): A general automated machine learning (AutoML) framework.
-* [HyperGBM](https://github.com/DataCanvasIO/HyperGBM): A full pipeline AutoML tool integrated various GBM models.
-* [HyperDT/DeepTables](https://github.com/DataCanvasIO/DeepTables): An AutoDL tool for tabular data.
-* [HyperTS](https://github.com/DataCanvasIO/HyperTS): A full pipeline AutoML&AutoDL tool for time series datasets.
-* [HyperKeras](https://github.com/DataCanvasIO/HyperKeras): An AutoDL tool for Neural Architecture Search and Hyperparameter Optimization on Tensorflow and Keras.
-* [HyperBoard](https://github.com/DataCanvasIO/HyperBoard): A visualization tool for Hypernets.
-* [Cooka](https://github.com/DataCanvasIO/Cooka): Lightweight interactive AutoML system.
-
-
-![DataCanvas AutoML Toolkit](docs/source/images/DAT_logo.png)
-
 ## Documents
 * [Overview](https://hypernets.readthedocs.io/en/latest/overview.html)
 * [QuickStart](https://hypernets.readthedocs.io/en/latest/quick_start.html)
 * [Search Space](https://hypernets.readthedocs.io/en/latest/search_space.html)
 * [Searcher](https://hypernets.readthedocs.io/en/latest/searchers.html)
 * [HyperModel](https://hypernets.readthedocs.io/en/latest/hypermodels.html)
 * [Experiment](https://hypernets.readthedocs.io/en/latest/experiment.html)
 ## Neural Architecture Search
 * [Define A DNN Search Space](https://hypernets.readthedocs.io/en/latest/nas.html#define-a-dnn-search-space)
 * [Define A CNN Search Space](https://hypernets.readthedocs.io/en/latest/nas.html#define-a-cnn-search-space)
 * [Define An ENAS Micro Search Space](https://hypernets.readthedocs.io/en/latest/nas.html#define-an-enas-micro-search-space)
 
 
+## Hypernets related projects
+* [Hypernets](https://github.com/DataCanvasIO/Hypernets): A general automated machine learning (AutoML) framework.
+* [HyperGBM](https://github.com/DataCanvasIO/HyperGBM): A full pipeline AutoML tool integrated various GBM models.
+* [HyperDT/DeepTables](https://github.com/DataCanvasIO/DeepTables): An AutoDL tool for tabular data.
+* [HyperTS](https://github.com/DataCanvasIO/HyperTS): A full pipeline AutoML&AutoDL tool for time series datasets.
+* [HyperKeras](https://github.com/DataCanvasIO/HyperKeras): An AutoDL tool for Neural Architecture Search and Hyperparameter Optimization on Tensorflow and Keras.
+* [HyperBoard](https://github.com/DataCanvasIO/HyperBoard): A visualization tool for Hypernets.
+* [Cooka](https://github.com/DataCanvasIO/Cooka): Lightweight interactive AutoML system.
+
+
+![DataCanvas AutoML Toolkit](https://raw.githubusercontent.com/DataCanvasIO/Hypernets/master/docs/source/images/DAT_latest.png)
+
+## Citation
+
+If you use Hypernets in your research, please cite us as follows:
+
+   Jian Yang, Xuefeng Li, Haifeng Wu. 
+   **Hypernets: A General Automated Machine Learning Framework.** https://github.com/DataCanvasIO/Hypernets. 2020. Version 0.2.x.
+
+BibTex:
+
+```
+@misc{hypernets,
+  author={Jian Yang, Xuefeng Li, Haifeng Wu},
+  title={{Hypernets}: { A General Automated Machine Learning Framework}},
+  howpublished={https://github.com/DataCanvasIO/Hypernets},
+  note={Version 0.2.x},
+  year={2020}
+}
+```
+
 ## DataCanvas
 Hypernets is an open source project created by [DataCanvas](https://www.datacanvas.com/).
```

### Comparing `hypernets-0.2.5.7/README.md` & `hypernets-0.3.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,42 @@
 <p align="center">
-<img src="docs/source/images/Hypernets.png" width="500" >
+<img src="https://raw.githubusercontent.com/DataCanvasIO/Hypernets/master/docs/source/images/Hypernets.png" width="500" >
 
 
 [![Python Versions](https://img.shields.io/pypi/pyversions/hypernets.svg)](https://pypi.org/project/hypernets)
 [![Downloads](https://pepy.tech/badge/hypernets)](https://pepy.tech/project/hypernets)
 [![PyPI Version](https://img.shields.io/pypi/v/hypernets.svg)](https://pypi.org/project/hypernets)
 
 ## We Are Hiring！
 Dear folks, we are offering challenging opportunities located in Beijing for both professionals and students who are keen on AutoML/NAS. Come be a part of DataCanvas! Please send your CV to yangjian@zetyun.com. (Application deadline: TBD.)  
 
 ## Hypernets: A General Automated Machine Learning Framework
 Hypernets is a general AutoML framework, based on which it can implement automatic optimization tools for various machine learning frameworks and libraries, including deep learning frameworks such as tensorflow, keras, pytorch, and machine learning libraries like sklearn, lightgbm, xgboost, etc.
+It also adopted various state-of-the-art optimization algorithms, including but not limited to evolution algorithm, monte carlo tree search for single objective optimization and multi-objective optimization algorithms such as MOEA/D,NSGA-II,R-NSGA-II.
 We introduced an abstract search space representation, taking into account the requirements of hyperparameter optimization and neural architecture search(NAS), making Hypernets a general framework that can adapt to various automated machine learning needs. As an abstraction computing layer, tabular toolbox, has successfully implemented in various tabular data types: pandas, dask, cudf, etc.  
 
 
 
 ## Overview
 ### Conceptual Model
 <p align="center">
-<img src="docs/source/images/hypernets_conceptual_model.png" width="100%"/>
+<img src="https://raw.githubusercontent.com/DataCanvasIO/Hypernets/master/docs/source/images/hypernets_conceptual_model.png" width="100%"/>
 </p>
 
 ### Illustration of the Search Space 
 <p align="center">
-<img src="docs/source/images/hypernets_search_space.png" width="100%"/>
+<img src="https://raw.githubusercontent.com/DataCanvasIO/Hypernets/master/docs/source/images/hypernets_search_space.png" width="100%"/>
 </p>
 
+## What's NEW !
+
+- **New feature:** [Multi-objectives optimization support](https://hypernets.readthedocs.io/en/latest/searchers.html#multi-objective-optimization)
+- **New feature:** [Performance and model complexity measurement metrics](https://github.com/DataCanvasIO/HyperGBM/blob/main/hypergbm/examples/66.Objectives_example.ipynb)
+- **New feature:** [Distributed computing](https://hypergbm.readthedocs.io/en/latest/example_dask.html) and [GPU acceleration](https://hypergbm.readthedocs.io/en/latest/example_cuml.html) base on computational abstraction layer
+
 
 ## Installation
 
 ### Conda
 
 Install Hypernets with `conda` from the channel *conda-forge*:
 
@@ -64,43 +71,62 @@
 
 * Install all above with one command:
 ```bash
 pip install hypernets[all]
 ```
 
 
-***Verify installation***:
+To ***Verify*** your installation:
 ```bash
 python -m hypernets.examples.smoke_testing
 ```
 
 ## Related Links
 
 * [A Brief Tutorial for Developing AutoML Tools with Hypernets](https://github.com/BochenLv/knn_toy_model/blob/main/Introduction.md)
 
-## Hypernets related projects
-* [Hypernets](https://github.com/DataCanvasIO/Hypernets): A general automated machine learning (AutoML) framework.
-* [HyperGBM](https://github.com/DataCanvasIO/HyperGBM): A full pipeline AutoML tool integrated various GBM models.
-* [HyperDT/DeepTables](https://github.com/DataCanvasIO/DeepTables): An AutoDL tool for tabular data.
-* [HyperTS](https://github.com/DataCanvasIO/HyperTS): A full pipeline AutoML&AutoDL tool for time series datasets.
-* [HyperKeras](https://github.com/DataCanvasIO/HyperKeras): An AutoDL tool for Neural Architecture Search and Hyperparameter Optimization on Tensorflow and Keras.
-* [HyperBoard](https://github.com/DataCanvasIO/HyperBoard): A visualization tool for Hypernets.
-* [Cooka](https://github.com/DataCanvasIO/Cooka): Lightweight interactive AutoML system.
-
-
-![DataCanvas AutoML Toolkit](docs/source/images/DAT_logo.png)
-
 ## Documents
 * [Overview](https://hypernets.readthedocs.io/en/latest/overview.html)
 * [QuickStart](https://hypernets.readthedocs.io/en/latest/quick_start.html)
 * [Search Space](https://hypernets.readthedocs.io/en/latest/search_space.html)
 * [Searcher](https://hypernets.readthedocs.io/en/latest/searchers.html)
 * [HyperModel](https://hypernets.readthedocs.io/en/latest/hypermodels.html)
 * [Experiment](https://hypernets.readthedocs.io/en/latest/experiment.html)
 ## Neural Architecture Search
 * [Define A DNN Search Space](https://hypernets.readthedocs.io/en/latest/nas.html#define-a-dnn-search-space)
 * [Define A CNN Search Space](https://hypernets.readthedocs.io/en/latest/nas.html#define-a-cnn-search-space)
 * [Define An ENAS Micro Search Space](https://hypernets.readthedocs.io/en/latest/nas.html#define-an-enas-micro-search-space)
 
 
+## Hypernets related projects
+* [Hypernets](https://github.com/DataCanvasIO/Hypernets): A general automated machine learning (AutoML) framework.
+* [HyperGBM](https://github.com/DataCanvasIO/HyperGBM): A full pipeline AutoML tool integrated various GBM models.
+* [HyperDT/DeepTables](https://github.com/DataCanvasIO/DeepTables): An AutoDL tool for tabular data.
+* [HyperTS](https://github.com/DataCanvasIO/HyperTS): A full pipeline AutoML&AutoDL tool for time series datasets.
+* [HyperKeras](https://github.com/DataCanvasIO/HyperKeras): An AutoDL tool for Neural Architecture Search and Hyperparameter Optimization on Tensorflow and Keras.
+* [HyperBoard](https://github.com/DataCanvasIO/HyperBoard): A visualization tool for Hypernets.
+* [Cooka](https://github.com/DataCanvasIO/Cooka): Lightweight interactive AutoML system.
+
+
+![DataCanvas AutoML Toolkit](https://raw.githubusercontent.com/DataCanvasIO/Hypernets/master/docs/source/images/DAT_latest.png)
+
+## Citation
+
+If you use Hypernets in your research, please cite us as follows:
+
+   Jian Yang, Xuefeng Li, Haifeng Wu. 
+   **Hypernets: A General Automated Machine Learning Framework.** https://github.com/DataCanvasIO/Hypernets. 2020. Version 0.2.x.
+
+BibTex:
+
+```
+@misc{hypernets,
+  author={Jian Yang, Xuefeng Li, Haifeng Wu},
+  title={{Hypernets}: { A General Automated Machine Learning Framework}},
+  howpublished={https://github.com/DataCanvasIO/Hypernets},
+  note={Version 0.2.x},
+  year={2020}
+}
+```
+
 ## DataCanvas
 Hypernets is an open source project created by [DataCanvas](https://www.datacanvas.com/).
```

### Comparing `hypernets-0.2.5.7/hypernets/conf/_configuration.py` & `hypernets-0.3.0/hypernets/conf/_configuration.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/core/__init__.py` & `hypernets-0.3.0/hypernets/core/__init__.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/core/callbacks.py` & `hypernets-0.3.0/hypernets/core/callbacks.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,16 @@
         self.triggered_reason = None
 
     def on_trial_begin(self, hyper_model, space, trial_no):
         if self.start_time is None:
             self.start_time = time.time()
 
     def on_trial_end(self, hyper_model, space, trial_no, reward, improved, elapsed):
+        reward = reward[0]  # NOTE only use first metric
+
         if self.start_time is None:
             self.start_time = time.time()
 
         time_total = time.time() - self.start_time
 
         if self.time_limit is not None and self.time_limit > 0:
             if time_total > self.time_limit:
@@ -165,14 +167,15 @@
 
     def on_trial_begin(self, hyper_model, space, trial_no):
         pass
         # with open(f'{self.output_dir}/trial_{trial_no}.log', 'w') as f:
         #     f.write(space.params_summary())
 
     def on_trial_end(self, hyper_model, space, trial_no, reward, improved, elapsed):
+        reward = reward[0]
         with self.open(f'{self.output_dir}/trial_{improved}_{trial_no:04d}_{reward:010.8f}_{elapsed:06.2f}.log',
                        'w') as f:
             f.write(space.params_summary())
             f.write('\r\n----------------Summary for Searcher----------------\r\n')
             f.write(hyper_model.searcher.summary())
 
         topn = 10
@@ -187,16 +190,17 @@
             configs = hyper_model.export_configuration(trials)
             for trial, conf in zip(trials, configs):
                 f.write(f'Trial No: {trial.trial_no}, Reward: {trial.reward}\r\n')
                 f.write(conf)
                 f.write('\r\n---------------------------------------------------\r\n\r\n')
 
     def on_skip_trial(self, hyper_model, space, trial_no, reason, reward, improved, elapsed):
+        reward_repr = "_".join(list(map(lambda v: f"{v:010.8f}", reward)))
         with self.open(
-                f'{self.output_dir}/trial_{reason}_{improved}_{trial_no:04d}_{reward:010.8f}_{elapsed:06.2f}.log',
+                f'{self.output_dir}/trial_{reason}_{improved}_{trial_no:04d}_{reward_repr}_{elapsed:06.2f}.log',
                 'w') as f:
             f.write(space.params_summary())
 
         topn = 5
         diff = hyper_model.history.diff(hyper_model.history.get_top(topn))
         with self.open(f'{self.output_dir}/top_{topn}_diff.txt', 'w') as f:
             diff_str = json.dumps(diff, indent=5)
@@ -336,19 +340,20 @@
         df_best_trials = pd.DataFrame([
             (t.trial_no, t.reward, t.elapsed, t.space_sample.vectors) for t in hyper_model.get_top_trials(5)],
             columns=['Trial No.', 'Reward', 'Elapsed', 'Space Vector'])
         if self.current_trial_display_id is not None:
             update_display(df_best_trials, display_id=self.current_trial_display_id)
 
     def on_trial_end(self, hyper_model, space, trial_no, reward, improved, elapsed):
+        reward = reward[0]
         self.last_trial_no = trial_no
         self.last_reward = reward
 
         best_trial = hyper_model.get_best_trial()
-        if best_trial is not None and self.best_trial_display_id is not None:
+        if best_trial is not None and not isinstance(best_trial, list) and self.best_trial_display_id is not None:
             update_display(best_trial.space_sample, display_id=self.best_trial_display_id)
 
     def on_trial_error(self, hyper_model, space, trial_no):
         self.last_trial_no = trial_no
         self.last_reward = 'ERR'
```

### Comparing `hypernets-0.2.5.7/hypernets/core/meta_learner.py` & `hypernets-0.3.0/hypernets/core/meta_learner.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         if store_history is None:
             store_history = ([], [])
 
         store_x, store_y = store_history
         x = x + store_x
         y = y + store_y
         if len(x) >= 2:
-            regressor = LGBMRegressor()
+            regressor = LGBMRegressor(min_data=1, min_data_in_bin=1, verbosity=-1)
             regressor.fit(x, y)
             #  if logger.is_info_enabled():
             #      logger.info(regressor.predict(x))
             self.regressors[space_signature] = regressor
 
     def predict(self, space_sample, default_value=np.inf):
         regressor = self.regressors.get(space_sample.signature)
```

### Comparing `hypernets-0.2.5.7/hypernets/core/mutables.py` & `hypernets-0.3.0/hypernets/core/mutables.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/core/ops.py` & `hypernets-0.3.0/hypernets/core/ops.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/core/random_state.py` & `hypernets-0.3.0/hypernets/core/random_state.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/core/search_space.py` & `hypernets-0.3.0/hypernets/core/search_space.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/core/searcher.py` & `hypernets-0.3.0/hypernets/core/searcher.py`

 * *Files 18% similar despite different names*

```diff
@@ -25,26 +25,31 @@
     def set_meta_learner(self, meta_learner):
         self.meta_learner = meta_learner
 
     @property
     def parallelizable(self):
         return False
 
-    def sample(self):
+    def sample(self, space_options=None):
         raise NotImplementedError
 
-    def _random_sample(self):
-        space_sample = self.space_fn()
+    def _random_sample(self, **space_kwargs):
+        if space_kwargs is None:
+            space_kwargs = {}
+        space_sample = self.space_fn(**space_kwargs)
         space_sample.random_sample()
         return space_sample
 
-    def _sample_and_check(self, sample_fn):
+    def _sample_and_check(self, sample_fn, space_options=None):
+        if space_options is None:
+            space_options = {}
+
         counter = 0
         while True:
-            space_sample = sample_fn()
+            space_sample = sample_fn(**space_options)
             counter += 1
             if counter >= 1000:
                 raise ValueError('Unable to take valid sample and exceed the retry limit 1000.')
             if self.space_sample_validation_fn is not None:
                 if self.space_sample_validation_fn(space_sample):
                     break
             else:
@@ -62,9 +67,15 @@
 
     def reset(self):
         raise NotImplementedError
 
     def export(self):
         raise NotImplementedError
 
+    def kind(self):
+        """Type of the Searcher, should be one of soo, moo.
+           This property used to avoid having to import MOOSearcher when detecting Searcher type.
+        """
+        return 'soo'
+
     def __repr__(self):
         return to_repr(self)
```

### Comparing `hypernets-0.2.5.7/hypernets/core/trial.py` & `hypernets-0.3.0/hypernets/core/trial.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,33 +3,48 @@
 
 """
 import datetime
 import os
 import pickle
 import shutil
 from collections import OrderedDict
+from typing import List
 
 import numpy as np
 import pandas as pd
 
 from hypernets.utils.common import isnotebook, to_repr
 from ..core.searcher import OptimizeDirection
+from ..core import pareto
+
+
+def _is_bigdata(v):
+    big_data_types = (pd.Series, pd.DataFrame, np.ndarray)
+    if isinstance(v, big_data_types):
+        return True
+
+    type_name = type(v).__name__.lower()
+    if any(type_name.find(s) for s in ('array', 'dataframe', 'series')):
+        return True
+
+    return False
 
 
 class Trial():
-    def __init__(self, space_sample, trial_no, reward, elapsed, model_file=None, succeeded=True):
+    def __init__(self, space_sample, trial_no, reward=None, elapsed=None, model_file=None, succeeded=True):
         self.space_sample = space_sample
         self.trial_no = trial_no
         self.reward = reward
         self.elapsed = elapsed
         self.model_file = model_file
         self.succeeded = succeeded
 
         self.memo = {}
         self.iteration_scores = {}
+        self.context = None
 
     def __repr__(self):
         return to_repr(self)
 
     def _repr_html_(self):
         html = f'<div><h>Trial:</h>'
         html += '''<table border="1" class="dataframe">
@@ -77,18 +92,17 @@
         try:
             state = super().__getstate__()
         except AttributeError:
             state = self.__dict__
 
         # state = {k: v for k, v in state.items() if k != 'memo'}
         memo = state.get('memo', None)
-        big_data_types = (pd.Series, pd.DataFrame, np.ndarray)
-        big_data_exists = isinstance(memo, dict) and any(isinstance(v, big_data_types) for v in memo.values())
+        big_data_exists = isinstance(memo, dict) and any(_is_bigdata(v) for v in memo.values())
         if big_data_exists:
-            compacted_memo = {k: v for k, v in memo.items() if not isinstance(v, big_data_types)}
+            compacted_memo = {k: v for k, v in memo.items() if not _is_bigdata(v)}
             state = state.copy()
             state['memo'] = compacted_memo
 
         return state
 
     def to_df(self, include_params=False):
         out = OrderedDict(trial_no=self.trial_no, succeeded=self.succeeded, reward=self.reward, elapsed=self.elapsed)
@@ -367,14 +381,93 @@
 
         if destination == 'notebook':
             return chart.render_notebook()
         else:
             return chart.render(output)
 
 
+class DominateBasedTrialHistory(TrialHistory):
+
+    def __init__(self, directions, objective_names):
+        super(DominateBasedTrialHistory, self).__init__(optimize_direction=directions[0])
+
+        self.directions = directions
+        self.objective_names = objective_names
+
+    def get_best(self):
+        succeed_trials = list(filter(lambda t: t.succeeded, self.trials))
+        solutions = np.asarray([t.reward for t in succeed_trials])
+        optimal_inx = pareto.calc_nondominated_set(solutions=solutions, directions=self.directions)
+        return [succeed_trials[i] for i in optimal_inx]
+
+    def append(self, trial):
+        self.trials.append(trial)
+        return trial in self.get_best()
+
+    def to_df(self, include_params=False):
+        if len(self.trials) > 0:
+            df = super(DominateBasedTrialHistory, self).to_df(include_params=include_params)
+            ns = self.get_best()
+
+            df['non_dominated'] = [t in ns for t in self.trials]
+            df['model_index'] = [ns.index(t) if t in ns else None for t in self.trials]
+
+            scores: np.ndarray = np.array(df['reward'].values.tolist())
+            assert scores.shape[1] == len(self.objective_names)
+            for i, name in enumerate(self.objective_names):
+                df[f'reward_{name}'] = scores[:, i]
+        else:
+            df = pd.DataFrame()
+
+        return df
+
+    def plot_best_trials(self, index=True, figsize=(5, 5), loc=None, bbox_to_anchor=None, xlim=None, ylim=None):
+        try:
+            from matplotlib import pyplot as plt
+        except Exception:
+            raise RuntimeError("it requires matplotlib installed.")
+
+        if len(self.objective_names) != 2:
+            raise RuntimeError("plot currently works only in case of 2 objectives. ")
+
+        best_trials = self.get_best()
+        objective_names = self.objective_names
+
+        fig = plt.figure(figsize=figsize)
+        ax = fig.add_subplot()
+
+        comparison = list(filter(lambda v: v not in best_trials, self.trials))
+
+        if len(comparison) > 0:
+            comp_scores = np.array([t.reward for t in comparison])
+            ax.scatter(comp_scores[:, 0], comp_scores[:, 1], c='blue', label='dominated', marker='o')
+
+        if len(best_trials) > 0:
+            best_scores = np.array([t.reward for t in best_trials])
+            ax.scatter(best_scores[:, 0], best_scores[:, 1], c='red', label='non-dominated', marker='o')
+            best_scores_sorted = np.array(sorted(best_scores, key=lambda v: v[1]))
+            # non-dominated does not mean optimal
+            ax.plot(best_scores_sorted[:, 0], best_scores_sorted[:, 1], color='c')
+
+        if index:
+            for i, t in enumerate(best_trials):
+                ax.text(t.reward[0], t.reward[1], f"{i}", ha='center', va='bottom', fontsize=9)
+
+        if xlim:
+            ax.set_xlim(*xlim)
+        if ylim:
+            ax.set_ylim(*ylim)
+
+        ax.legend(loc=loc, bbox_to_anchor=bbox_to_anchor)
+        plt.xlabel(objective_names[0])
+        plt.ylabel(objective_names[1])
+        plt.title(f"Best trials in TrialHistory(total={len(self.trials)})")
+        return fig, ax
+
+
 class TrialStore(object):
     def __init__(self):
         self.reset()
         self.load()
 
     def put(self, dataset_id, trial):
         self.put_to_cache(dataset_id, trial)
```

### Comparing `hypernets-0.2.5.7/hypernets/discriminators/__init__.py` & `hypernets-0.3.0/hypernets/discriminators/__init__.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/discriminators/_base.py` & `hypernets-0.3.0/hypernets/discriminators/_base.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/discriminators/percentile.py` & `hypernets-0.3.0/hypernets/discriminators/percentile.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/dispatchers/__init__.py` & `hypernets-0.3.0/hypernets/dispatchers/__init__.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/dispatchers/cfg.py` & `hypernets-0.3.0/hypernets/dispatchers/cfg.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/dispatchers/cluster/cluster.py` & `hypernets-0.3.0/hypernets/dispatchers/cluster/cluster.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/dispatchers/cluster/driver_dispatcher.py` & `hypernets-0.3.0/hypernets/dispatchers/cluster/driver_dispatcher.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/dispatchers/cluster/executor_dispatcher.py` & `hypernets-0.3.0/hypernets/dispatchers/cluster/executor_dispatcher.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/dispatchers/cluster/grpc/proto/spec_pb2.py` & `hypernets-0.3.0/hypernets/dispatchers/cluster/grpc/proto/spec_pb2.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/dispatchers/cluster/grpc/proto/spec_pb2_grpc.py` & `hypernets-0.3.0/hypernets/dispatchers/cluster/grpc/proto/spec_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/dispatchers/cluster/grpc/search_driver_client.py` & `hypernets-0.3.0/hypernets/dispatchers/cluster/grpc/search_driver_client.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/dispatchers/cluster/grpc/search_driver_service.py` & `hypernets-0.3.0/hypernets/dispatchers/cluster/grpc/search_driver_service.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/dispatchers/dask/dask_dispatcher.py` & `hypernets-0.3.0/hypernets/dispatchers/dask/dask_dispatcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,15 +163,15 @@
         super(DaskDispatcher, self).__init__()
 
         self.work_dir = work_dir
         self.models_dir = f'{work_dir}/models'
 
         fs.makedirs(self.models_dir, exist_ok=True)
 
-    def dispatch(self, hyper_model, X, y, X_val, y_val, cv, num_folds, max_trials, dataset_id, trial_store,
+    def dispatch(self, hyper_model, X, y, X_val, y_val, X_test, cv, num_folds, max_trials, dataset_id, trial_store,
                  **fit_kwargs):
         assert not any(dask.is_dask_collection(i) for i in (X, y, X_val, y_val)), \
             f'{self.__class__.__name__} does not support to run trial with dask collection.'
 
         queue_size = c.dask_search_queue
         worker_count = c.dask_search_executors
         retry_limit = c.trial_retry_limit
```

### Comparing `hypernets-0.2.5.7/hypernets/dispatchers/in_process_dispatcher.py` & `hypernets-0.3.0/hypernets/dispatchers/in_process_dispatcher.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,49 @@
 # -*- coding:utf-8 -*-
 import gc
 
 from .cfg import DispatchCfg as c
 from ..core.callbacks import EarlyStoppingError
 from ..core.dispatcher import Dispatcher
 from ..core.trial import Trial
-from ..utils import logging, fs
+from ..tabular import get_tool_box
+from ..utils import logging, fs, const
 
 logger = logging.get_logger(__name__)
 
 
 class InProcessDispatcher(Dispatcher):
     def __init__(self, models_dir):
         super(InProcessDispatcher, self).__init__()
 
         self.models_dir = models_dir
         fs.makedirs(models_dir, exist_ok=True)
 
-    def dispatch(self, hyper_model, X, y, X_eval, y_eval, cv, num_folds, max_trials, dataset_id, trial_store,
+    def dispatch(self, hyper_model, X, y, X_eval, y_eval, X_test, cv, num_folds, max_trials, dataset_id, trial_store,
                  **fit_kwargs):
         retry_limit = c.trial_retry_limit
 
         trial_no = 1
         retry_counter = 0
 
+        space_options = {}
+        if hyper_model.searcher.kind() == const.SEARCHER_MOO:
+            if 'feature_usage' in [_.name for _ in hyper_model.searcher.objectives]:
+                tb = get_tool_box(X, y)
+                preprocessor = tb.general_preprocessor(X)
+                estimator = tb.general_estimator(X, y, task=hyper_model.task)
+                estimator.fit(preprocessor.fit_transform(X, y), y)
+                importances = list(zip(estimator.feature_name_, estimator.feature_importances_))
+                space_options['importances'] = importances
+
         while trial_no <= max_trials:
             gc.collect()
             try:
-                space_sample = hyper_model.searcher.sample()
+
+                space_sample = hyper_model.searcher.sample(space_options=space_options)
                 if hyper_model.history.is_existed(space_sample):
                     if retry_counter >= retry_limit:
                         logger.info(f'Unable to take valid sample and exceed the retry limit {retry_limit}.')
                         break
                     trial = hyper_model.history.get_trial(space_sample)
                     for callback in hyper_model.callbacks:
                         try:
@@ -76,15 +88,15 @@
                     except EarlyStoppingError:
                         raise
                     except Exception as e:
                         logger.warn(e)
 
                 model_file = '%s/%05d_%s.pkl' % (self.models_dir, trial_no, space_sample.space_id)
 
-                trial = hyper_model._run_trial(space_sample, trial_no, X, y, X_eval, y_eval, cv, num_folds, model_file,
+                trial = hyper_model._run_trial(space_sample, trial_no, X, y, X_eval, y_eval, X_test, cv, num_folds, model_file,
                                                **fit_kwargs)
 
                 if trial.succeeded:
                     improved = hyper_model.history.append(trial)
                     for callback in hyper_model.callbacks:
                         try:
                             callback.on_trial_end(hyper_model, space_sample, trial_no, trial.reward,
```

### Comparing `hypernets-0.2.5.7/hypernets/dispatchers/predict/grpc/predict_client.py` & `hypernets-0.3.0/hypernets/dispatchers/predict/grpc/predict_client.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/dispatchers/predict/grpc/predict_service.py` & `hypernets-0.3.0/hypernets/dispatchers/predict/grpc/predict_service.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/dispatchers/predict/grpc/proto/predict_pb2.py` & `hypernets-0.3.0/hypernets/dispatchers/predict/grpc/proto/predict_pb2.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/dispatchers/predict/grpc/proto/predict_pb2_grpc.py` & `hypernets-0.3.0/hypernets/dispatchers/predict/grpc/proto/predict_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/dispatchers/predict/predict_helper.py` & `hypernets-0.3.0/hypernets/dispatchers/predict/predict_helper.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/dispatchers/process/grpc/process_broker_client.py` & `hypernets-0.3.0/hypernets/dispatchers/process/grpc/process_broker_client.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/dispatchers/process/grpc/process_broker_service.py` & `hypernets-0.3.0/hypernets/dispatchers/process/grpc/process_broker_service.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/dispatchers/process/grpc/proto/proc_pb2.py` & `hypernets-0.3.0/hypernets/dispatchers/process/grpc/proto/proc_pb2.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/dispatchers/process/grpc/proto/proc_pb2_grpc.py` & `hypernets-0.3.0/hypernets/dispatchers/process/grpc/proto/proc_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/dispatchers/process/grpc_process.py` & `hypernets-0.3.0/hypernets/dispatchers/process/grpc_process.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,31 +17,31 @@
         self.cmd = cmd
         self.in_file = in_file
         self.out_file = out_file
         self.err_file = err_file
         self.environment = environment
         self._exit_code = PValue('i', -1)
 
-    def run(self):
-        if logger.is_info_enabled():
+    def run(self, verbose=False):
+        if verbose and logger.is_info_enabled():
             msg = f'[{self.name}] [GRPC {self.grpc_broker}] {self.cmd}, out={self.out_file}, err={self.err_file}'
             logger.info(msg)
 
         try:
             client = ProcessBrokerClient(self.grpc_broker)
             buffer_size = 16
             if self.out_file and self.err_file:
                 with open(self.out_file, 'wb', buffering=0)as o, open(self.err_file, 'wb', buffering=0) as e:
                     code = client.run(self.cmd.split(' '), stdout=o, stderr=e, buffer_size=buffer_size)
             else:
                 code = client.run(self.cmd.split(' '), stdout=sys.stdout, stderr=sys.stderr, buffer_size=buffer_size)
         except KeyboardInterrupt:
             code = 137
 
-        if logger.is_info_enabled():
+        if verbose and logger.is_info_enabled():
             logger.info(f'[{self.name}] [GRPC {self.grpc_broker}] {self.cmd} done with {code}')
         self._exit_code.value = code
 
     @property
     def exitcode(self):
         code = self._exit_code.value
         return code if code >= 0 else None
```

### Comparing `hypernets-0.2.5.7/hypernets/dispatchers/process/local_process.py` & `hypernets-0.3.0/hypernets/dispatchers/process/local_process.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,16 +15,16 @@
         self.cmd = cmd
         self.in_file = in_file
         self.out_file = out_file
         self.err_file = err_file
         self.environment = environment
         self._exit_code = PValue('i', -1)
 
-    def run(self):
-        if logger.is_info_enabled():
+    def run(self, verbose=False):
+        if verbose and logger.is_info_enabled():
             logger.info(f'[{self.name}] [CMD] {self.cmd}, out={self.out_file}, err={self.err_file}')
 
         try:
             if self.out_file and self.err_file:
                 with open(self.out_file, 'wb', buffering=0)as o, open(self.err_file, 'wb', buffering=0) as e:
                     p = subprocess.run(self.cmd.split(' '),
                                        shell=False,
@@ -38,15 +38,15 @@
                                    stdin=subprocess.DEVNULL,
                                    stdout=sys.stdout,
                                    stderr=sys.stderr)
                 code = p.returncode
         except KeyboardInterrupt:
             code = 137
 
-        if logger.is_info_enabled():
+        if verbose and logger.is_info_enabled():
             logger.info(f'[{self.name}] [CMD] {self.cmd} done with {code}')
 
         self._exit_code.value = code
 
     @property
     def exitcode(self):
         code = self._exit_code.value
```

### Comparing `hypernets-0.2.5.7/hypernets/dispatchers/process/ssh_process.py` & `hypernets-0.3.0/hypernets/dispatchers/process/ssh_process.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,28 +41,28 @@
         self.cmd = cmd
         self.in_file = in_file
         self.out_file = out_file
         self.err_file = err_file
         self.environment = environment
         self._exit_code = PValue('i', -1)
 
-    def run(self):
-        if logger.is_info_enabled():
+    def run(self, verbose=False):
+        if verbose and logger.is_info_enabled():
             logger.info(f'[{self.name}] [SSH {self.ssh_host}]: {self.cmd}')
         try:
             code = self.ssh_run(self.ssh_host, self.ssh_port,
                                 self.cmd,
                                 self.in_file,
                                 self.out_file,
                                 self.err_file,
                                 self.environment)
         except KeyboardInterrupt:
             code = 137
 
-        if logger.is_info_enabled():
+        if verbose and logger.is_info_enabled():
             logger.info(f'[{self.name}] [SSH {self.ssh_host}] {self.cmd} done with {code}')
 
         self._exit_code.value = code
 
     @staticmethod
     def ssh_run(ssh_host, ssh_port, cmd, in_file, out_file, err_file, environment):
         with SSHClient() as ssh:
```

### Comparing `hypernets-0.2.5.7/hypernets/dispatchers/run.py` & `hypernets-0.3.0/hypernets/dispatchers/run.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/dispatchers/run_broker.py` & `hypernets-0.3.0/hypernets/dispatchers/run_broker.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/dispatchers/run_predict.py` & `hypernets-0.3.0/hypernets/dispatchers/run_predict.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/dispatchers/run_predict_server.py` & `hypernets-0.3.0/hypernets/dispatchers/run_predict_server.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/examples/plain_model.py` & `hypernets-0.3.0/hypernets/examples/plain_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,16 +9,27 @@
 from sklearn.neural_network import MLPClassifier
 from sklearn.tree import DecisionTreeClassifier, DecisionTreeRegressor
 
 from hypernets.core import set_random_state, randint
 from hypernets.core.ops import ModuleChoice, HyperInput, ModuleSpace
 from hypernets.core.search_space import HyperSpace, Choice, Int, Real, Cascade, Constant, HyperNode
 from hypernets.model import Estimator, HyperModel
-from hypernets.tabular import get_tool_box
-from hypernets.utils import fs, logging, const
+from hypernets.tabular import get_tool_box, column_selector
+from hypernets.utils import fs, const
+
+
+from hypernets.core import randint
+from hypernets.core.ops import ModuleChoice, HyperInput
+from hypernets.core.search_space import HyperSpace, Choice, Int, Real
+from hypernets.pipeline.base import DataFrameMapper
+from hypernets.pipeline.transformers import FeatureImportanceSelection
+
+from hypernets.utils import logging
+
+
 
 logger = logging.get_logger(__name__)
 
 
 class PlainSearchSpace(object):
     def __init__(self, enable_dt=True, enable_lr=True, enable_nn=True, enable_dtr=False):
         assert enable_dt or enable_lr or enable_nn or enable_dtr
@@ -110,14 +121,29 @@
     def _cascade(fn, key, args, space):
         with space.as_default():
             kvalue = args[key]
             if isinstance(kvalue, HyperNode):
                 kvalue = kvalue.value
             return fn(kvalue)
 
+    def create_feature_selection(self, hyper_input, importances, seq_no=0):
+        from hypernets.pipeline.base import Pipeline
+
+        selection = FeatureImportanceSelection(name=f'feature_importance_selection_{seq_no}',
+                                               importances=importances,
+                                               quantile=Real(0, 1, step=0.1))
+        pipeline = Pipeline([selection],
+                            name=f'feature_selection_{seq_no}',
+                            columns=column_selector.column_all)(hyper_input)
+
+        preprocessor = DataFrameMapper(default=False, input_df=True, df_out=True,
+                                       df_out_dtype_transforms=None)([pipeline])
+
+        return preprocessor
+
     # HyperSpace
     def __call__(self, *args, **kwargs):
         space = HyperSpace()
 
         with space.as_default():
             hyper_input = HyperInput(name='input1')
 
@@ -126,17 +152,22 @@
                 estimators.append(self.dt)
             if self.enable_dtr:
                 estimators.append(self.dtr)
             if self.enable_lr:
                 estimators.append(self.lr)
             if self.enable_nn:
                 estimators.append(self.nn)
-
             modules = [ModuleSpace(name=f'{e["cls"].__name__}', **e) for e in estimators]
-            outputs = ModuleChoice(modules)(hyper_input)
+
+            if "importances" in kwargs and kwargs["importances"] is not None:
+                importances = kwargs.pop("importances")
+                ss = self.create_feature_selection(hyper_input, importances)
+                outputs = ModuleChoice(modules)(ss)
+            else:
+                outputs = ModuleChoice(modules)(hyper_input)
             space.set_inputs(hyper_input)
 
         return space
 
 
 class PlainEstimator(Estimator):
     def __init__(self, space_sample, task=const.TASK_BINARY, transformer=None):
@@ -204,14 +235,18 @@
 
         if isinstance(y, (pd.Series, pd.DataFrame)):
             y = y.values
 
         oof_ = None
         oof_scores = []
         cv_models = []
+        x_vals = []
+        y_vals = []
+        X_trains = []
+        y_trains = []
         logger.info('start training')
         for n_fold, (train_idx, valid_idx) in enumerate(iterators.split(X, y)):
             x_train_fold, y_train_fold = X.iloc[train_idx], y[train_idx]
             x_val_fold, y_val_fold = X.iloc[valid_idx], y[valid_idx]
 
             logger.info(f'fit fold {n_fold}')
             fold_model = copy.deepcopy(self.model)
@@ -242,25 +277,30 @@
             fold_scores = tb.metrics.calc_score(y_val_fold, preds, proba, metrics, task=self.task)
 
             # save fold result
             oof_[valid_idx] = proba
             oof_scores.append(fold_scores)
             cv_models.append(fold_model)
 
+            x_vals.append(x_val_fold)
+            y_vals.append(y_val_fold)
+            X_trains.append(x_train_fold)
+            y_trains.append(y_train_fold)
+
         self.classes_ = getattr(cv_models[0], 'classes_', None)
         self.cv_ = True
         self.cv_models_ = cv_models
 
         # calc final score with mean
         scores = pd.concat([pd.Series(s) for s in oof_scores], axis=1).mean(axis=1).to_dict()
         logger.info(f'fit_cross_validation score:{scores}, folds score:{oof_scores}')
 
         # return
         oof_, = tb_original.from_local(oof_)
-        return scores, oof_, oof_scores
+        return scores, oof_, oof_scores, X_trains, y_trains, x_vals, y_vals
 
     def predict(self, X, **kwargs):
         eval_set = kwargs.pop('eval_set', None)  # ignore
 
         if self.transformer is not None:
             logger.info('transform local')
             X = self.transformer.transform(X)
```

### Comparing `hypernets-0.2.5.7/hypernets/examples/smoke_testing.py` & `hypernets-0.3.0/hypernets/examples/smoke_testing.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,12 +33,12 @@
     )
 
     for searcher in searchers:
         for i in range(100):
             space_sample = searcher.sample()
             assert space_sample.all_assigned == True
             print(searcher.__class__.__name__, i, space_sample.params_summary())
-            searcher.update_result(space_sample, np.random.uniform(0.1, 0.9))
+            searcher.update_result(space_sample, [np.random.uniform(0.1, 0.9)])
 
 
 if __name__ == '__main__':
     run_search()
```

### Comparing `hypernets-0.2.5.7/hypernets/experiment/__init__.py` & `hypernets-0.3.0/hypernets/experiment/__init__.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/experiment/_callback.py` & `hypernets-0.3.0/hypernets/experiment/_callback.py`

 * *Files 4% similar despite different names*

```diff
@@ -167,22 +167,28 @@
         super().step_end(exp, step, output, elapsed)
 
         try:
             fitted_params = exp.get_step(step).get_fitted_params()
             proba = fitted_params.get('test_proba')
             proba = proba[:, 1]  # fixme for multi-classes
 
-            import seaborn as sns
+            from scipy.stats import gaussian_kde
             import matplotlib.pyplot as plt
+
+            kde = gaussian_kde(proba)
+            kde.set_bandwidth(0.01 * kde.factor)
+            x = np.linspace(proba.min(), proba.max(), num=100)
+            y = kde(x)
+
             # Draw Plot
             plt.figure(figsize=(8, 4), dpi=80)
-            sns.kdeplot(proba, shade=True, color="g", label="Proba", alpha=.7, bw_adjust=0.01)
+            plt.plot(x, y, 'g-', alpha=0.7)
+            plt.fill_between(x, y, color='g', alpha=0.2)
             # Decoration
             plt.title('Density Plot of Probability', fontsize=22)
-            plt.legend()
             plt.show()
         except:
             pass
 
 
 _default_step_callback = NotebookStepCallback
 
@@ -233,30 +239,37 @@
                                       'y_train.shape',
                                       'X_eval.shape',
                                       'y_eval.shape',
                                       'X_test.shape',
                                       'Task', ]), display_id='output_intput')
 
         try:
-            import seaborn as sns
             import matplotlib.pyplot as plt
-            from sklearn.preprocessing import LabelEncoder
+
+            y_train = y_train.dropna()
             if exp.task == const.TASK_REGRESSION:
+                from scipy.stats import gaussian_kde
+                kde = gaussian_kde(y_train)
+                kde.set_bandwidth(0.01 * kde.factor)
+                x = np.linspace(y_train.min(), y_train.max(), num=100)
+                y = kde(x)
                 # Draw Plot
                 plt.figure(figsize=(8, 4), dpi=80)
-                sns.kdeplot(y_train.dropna(), shade=True, color="g", label="Proba", alpha=.7, bw_adjust=0.01)
+                plt.plot(x, y, 'g-', alpha=0.7)
+                plt.fill_between(x, y, color='g', alpha=0.2)
             else:
-                le = LabelEncoder()
-                y = le.fit_transform(y_train.dropna())
+                tb = get_tool_box(y_train)
+                vs = tb.value_counts(y_train)
+                labels = list(sorted(vs.keys()))
+                values = [vs[k] for k in labels]
                 # Draw Plot
                 plt.figure(figsize=(8, 4), dpi=80)
-                sns.distplot(y, kde=False, color="g", label="y")
-            # Decoration
+                plt.pie(values, labels=labels, autopct='%1.1f%%')
+
             plt.title('Distribution of y', fontsize=22)
-            plt.legend()
             plt.show()
         except:
             pass
 
     def experiment_end(self, exp, elapsed):
         self.running = False
 
@@ -351,26 +364,26 @@
 
             labels = unique_labels(y_test, y_pred)
             confusion_matrix_data = ConfusionMatrixMeta(confusion_matrix(y_test, y_pred, labels=labels), labels)
         elif exp.task in [const.TASK_REGRESSION]:
             from hypernets.tabular.metrics import calc_score
             evaluation_metrics_data = calc_score(y_test, y_pred, y_proba=None, metrics=('mse', 'mae', 'rmse', 'r2'),
                                                  task=const.TASK_REGRESSION, pos_label=None, classes=None, average=None)
-            evaluation_metrics_data['explained_variance'] = sk_metrics.explained_variance_score(y_true=y_test, y_pred=y_pred)
+            evaluation_metrics_data['explained_variance'] = \
+                sk_metrics.explained_variance_score(y_true=y_test, y_pred=y_pred)
 
         exp.evaluation_ = {
-            'prediction_elapsed': (predict_elapsed,  predict_proba_elapsed),
+            'prediction_elapsed': (predict_elapsed, predict_proba_elapsed),
             'evaluation_metrics': evaluation_metrics_data,
             'confusion_matrix': confusion_matrix_data,
             'classification_report': classification_report_data
         }
 
 
 class ResourceUsageMonitor(Thread):
-
     STATUS_READY = 0
     STATUS_RUNNING = 1
     STATUS_STOP = 2
 
     def __init__(self, interval=30):
         # auto exit if all work thread finished
         super(ResourceUsageMonitor, self).__init__(name=self.__class__.__name__, daemon=True)
@@ -439,14 +452,21 @@
 
     def step_end(self, exp, step, output, elapsed):
         pass
 
     def step_break(self, exp, step, error):
         pass
 
+    def __getstate__(self):
+        states = dict(self.__dict__)
+        if '_rum' in states:
+            del states['_rum']
+
+        return states
+
 
 class ActionType:
     ExperimentStart = 'experimentStart'
     ExperimentBreak = 'experimentBreak'
     ExperimentEnd = 'experimentEnd'
     StepStart = 'stepStart'
     StepBreak = 'stepBreak'
```

### Comparing `hypernets-0.2.5.7/hypernets/experiment/_experiment.py` & `hypernets-0.3.0/hypernets/experiment/_experiment.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 """
 import time
 
 from IPython.display import display
 
 from hypernets.dispatchers.cfg import DispatchCfg
-from hypernets.utils import logging, df_utils
+from hypernets.utils import logging
 
 logger = logging.get_logger(__name__)
 
 
 class ExperimentCallback():
     def experiment_start(self, exp):
         pass
@@ -64,14 +64,15 @@
 
         # trained
         self.start_time = None
         self.end_time = None
         self.model_ = None
 
     def get_data_character(self):
+        from hypernets.utils import df_utils
         data_character = df_utils.get_data_character(self.hyper_model, self.X_train, self.y_train, self.X_eval,
                                                      self.y_eval, self.X_test, self.task)
         return data_character
 
     def run(self, **kwargs):
         self.start_time = time.time()
```

### Comparing `hypernets-0.2.5.7/hypernets/experiment/_extractor.py` & `hypernets-0.3.0/hypernets/experiment/_extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import abc
 import copy
 from collections import OrderedDict, namedtuple
 from typing import List, Set, Dict, Tuple, Optional
 
 import numpy as np
 import pandas as pd
+from scipy import stats
 
 from hypernets.model import Estimator
 from hypernets.utils import logging, get_tree_importances
 
 
 logger = logging.get_logger(__name__)
 
@@ -580,23 +581,33 @@
                 "samples": pseudo_label_stat,
                 "selectedLabel": np2py(classes_[0]),
             }
         return result_extension
 
     @staticmethod
     def get_proba_density_estimation(scores, classes, n_partitions=1000):
-        # from sklearn.neighbors import KernelDensity
         probability_density = {}
-        from seaborn._statistics import KDE
+
+        def calc(proba):
+            cut = 3
+            gridsize = 200
+
+            kde = stats.gaussian_kde(proba, bw_method='scott')
+            kde.set_bandwidth(0.01 * kde.factor)
+            bw = np.sqrt(kde.covariance.squeeze())
+            gridmin = max(proba.min() - bw * cut, -np.inf)
+            gridmax = min(proba.max() + bw * cut, +np.inf)
+            support = np.linspace(gridmin, gridmax, gridsize)
+            return kde(support), support
+
         for i, class_ in enumerate(classes):
             selected_proba = np.array(scores[:, i])
-            selected_proba_series = pd.Series(selected_proba).dropna()  # todo use numpy instead to remove pandas
+            proba = selected_proba[~np.isnan(selected_proba)]
             # selected_proba = selected_proba.reshape((selected_proba.shape[0], 1))
-            estimator = KDE(bw_method='scott', bw_adjust=0.01, gridsize=200, cut=3, clip=None, cumulative=False)
-            density, support = estimator(selected_proba_series, weights=None)
+            density, support = calc(proba)
             probability_density[class_] = {
                 'gaussian': {
                     "X": support.tolist(),
                     "probaDensity": density.tolist()
                 }
             }
         return probability_density
```

### Comparing `hypernets-0.2.5.7/hypernets/experiment/_maker.py` & `hypernets-0.3.0/hypernets/experiment/_maker.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 """
 from sklearn.metrics import get_scorer
 
 from hypernets.discriminators import make_discriminator
 from hypernets.experiment import CompeteExperiment
 from hypernets.experiment.cfg import ExperimentCfg as cfg
 from hypernets.model import HyperModel
+from hypernets.model.objectives import create_objective
 from hypernets.searchers import make_searcher, PlaybackSearcher
 from hypernets.tabular import get_tool_box
 from hypernets.tabular.cache import clear as _clear_cache
 from hypernets.tabular.cfg import TabularCfg as tcfg
 from hypernets.utils import const, logging, isnotebook, load_module, DocLens
 
 logger = logging.get_logger(__name__)
@@ -34,29 +35,61 @@
 
 def default_search_callbacks():
     cbs = cfg.hyper_model_callbacks_notebook if isnotebook() else cfg.hyper_model_callbacks_console
     cbs = [load_module(cb)() if isinstance(cb, str) else cb for cb in cbs]
     return cbs
 
 
-def to_search_object(search_space, optimize_direction, searcher, searcher_options):
+def to_objective_object(o, force_minimize=False, **kwargs):
+    from hypernets.core.objective import Objective
+
+    if isinstance(o, str):
+        return create_objective(o, force_minimize=force_minimize, **kwargs)
+    elif isinstance(o, Objective):
+        return o
+    else:
+        raise RuntimeError("objective specific should be instanced by 'Objective' or a string")
+
+
+def to_search_object(search_space, optimize_direction, searcher, searcher_options,
+                     reward_metric=None, scorer=None, objectives=None,  task=None, pos_label=None):
+
     def to_searcher(cls, options):
         assert search_space is not None, '"search_space" should be specified if "searcher" is None or str.'
         assert optimize_direction in {'max', 'min'}
-        if options is None:
-            options = {}
-        options['optimize_direction'] = optimize_direction
-        s = make_searcher(cls, search_space, **options)
+        s = make_searcher(cls, search_space, optimize_direction=optimize_direction, **options)
 
         return s
 
     if searcher is None:
         from hypernets.searchers import EvolutionSearcher
         sch = to_searcher(EvolutionSearcher, searcher_options)
     elif isinstance(searcher, (type, str)):
+        from hypernets.searchers.moo import MOOSearcher
+        from hypernets.searchers import get_searcher_cls
+
+        search_cls = get_searcher_cls(searcher)
+        if issubclass(search_cls, MOOSearcher):
+            from hypernets.model.objectives import PredictionObjective
+            from hypernets.searchers.moead_searcher import MOEADSearcher
+            from hypernets.core import get_random_state
+
+            if objectives is None:
+                objectives = ['nf']
+            objectives_instance = []
+            force_minimize = (search_cls == MOEADSearcher)
+            for o in objectives:
+                objectives_instance.append(to_objective_object(o, force_minimize=force_minimize,
+                                                               task=task, pos_label=pos_label))
+
+            objectives_instance.insert(0, PredictionObjective.create(reward_metric, force_minimize=force_minimize,
+                                                                     task=task, pos_label=pos_label))
+            searcher_options['objectives'] = objectives_instance
+            searcher_options['random_state'] = get_random_state()
+
         sch = to_searcher(searcher, searcher_options)
     else:
         from hypernets.core.searcher import Searcher as SearcherSpec
         if not isinstance(searcher, SearcherSpec):
             logger.warning(f'Unrecognized searcher "{searcher}".')
         sch = searcher
 
@@ -86,14 +119,15 @@
                     searcher_options=None,
                     search_space=None,
                     search_callbacks=None,
                     early_stopping_rounds=10,
                     early_stopping_time_limit=3600,
                     early_stopping_reward=None,
                     reward_metric=None,
+                    objectives=None,
                     optimize_direction=None,
                     hyper_model_options=None,
                     discriminator=None,
                     evaluation_metrics='auto',
                     evaluation_persist_prediction=False,
                     evaluation_persist_prediction_dir=None,
                     report_render=None,
@@ -125,17 +159,18 @@
         If None, inference the type of task automatically
     id : str or None, (default=None)
         The experiment id.
     callbacks: list of ExperimentCallback, optional
         ExperimentCallback list.
     searcher : str, searcher class, search object, optional
         The hypernets Searcher instance to explore search space, default is EvolutionSearcher instance.
-        For str, should be one of 'evolution', 'mcts', 'random'.
-        For class, should be one of EvolutionSearcher, MCTSSearcher, RandomSearcher, or subclass of hypernets Searcher.
-        For other, should be instance of hypernets Searcher.
+        For str, should be one of 'evolution', 'mcts', 'random', 'nsga2', 'moead'.  # TODO rnsga
+        For class, should be one of EvolutionSearcher, MCTSSearcher, RandomSearcher, MOEADSearcher, NSGAIISearrcher
+         or subclass of hypernets Searcher.
+        For other, should be instanced of hypernets Searcher.
     searcher_options: dict, optional, default is None
         The options to create searcher, is used if searcher is str.
     search_space : callable, optional
         Used to initialize searcher instance (if searcher is None, str or class).
     search_callbacks
         Hypernets search callbacks, used to initialize searcher instance (if searcher is None, str or class).
         If log_level >= WARNNING, default is EarlyStoppingCallback only.
@@ -158,31 +193,38 @@
             - mse
             - mae
             - msle
             - precision
             - rmse
             - r2
             - recall
+    objectives : List[Union[Objective, str]] optional, (default to ['nf'] )
+        Used for multi-objectives optimization, "reward_metric" is alway picked as the first objective, specilly for
+        "MOEADSearcher", will force the indicator to be the smaller the better by converting score to a negative number.
+        For str as identifier of objectives, possible values:
+            - elapsed
+            - pred_perf
+            - nf
     optimize_direction : str, optional
         Hypernets search reward metric direction, default is detected from reward_metric.
     discriminator : instance of hypernets.discriminator.BaseDiscriminator, optional
         Discriminator is used to determine whether to continue training
     hyper_model_options: dict, optional
         Options to initlize HyperModel except *reward_metric*, *task*, *callbacks*, *discriminator*.
     evaluation_metrics: str, list, or None (default='auto'),
         If *eval_data* is not None, it used to evaluate model with the metrics.
-        For str should be 'auto', it will selected metrics accord to machine learning task type.
+        For str should be 'auto', it will select metrics accord to machine learning task type.
         For list should be metrics name.
     evaluation_persist_prediction: bool (default=False)
     evaluation_persist_prediction_dir: str or None (default='predction')
         The dir to persist prediction, if exists will be overwritten
     report_render: str, obj, optional, default is None
         The experiment report render.
         For str should be one of 'excel'
-        for obj should be instance ReportRender
+        for obj should be instanced of ReportRender
     report_render_options: dict, optional
         The options to create render, is used if render is str.
     experiment_cls: class, or None, (default=CompeteExperiment)
         The experiment type, CompeteExperiment or it's subclass.
     n_jobs: int, default None
         If not None, update value of option `TabularCfg.joblib_njobs`.
     clear_cache: bool, optional, (default False)
@@ -280,15 +322,24 @@
 
     if isinstance(scorer, str):
         scorer = get_scorer(scorer)
 
     if optimize_direction is None or len(optimize_direction) == 0:
         optimize_direction = 'max' if scorer._sign > 0 else 'min'
 
-    searcher = to_search_object(search_space, optimize_direction, searcher, searcher_options)
+    if searcher_options is None:
+        searcher_options = {}
+
+    searcher = to_search_object(search_space, optimize_direction, searcher, searcher_options,
+                                reward_metric=reward_metric, scorer=scorer, objectives=objectives, task=task,
+                                pos_label=kwargs.get('pos_label'))
+
+    if searcher.kind() == const.SEARCHER_MOO:
+        if 'psi' in [_.name for _ in searcher.objectives]:
+            assert X_test is not None, "psi objective requires test dataset"
 
     if cfg.experiment_auto_down_sample_enabled and not isinstance(searcher, PlaybackSearcher) \
             and 'down_sample_search' not in kwargs.keys():
         train_data_shape = tb.get_shape(X_train)
         if train_data_shape[0] > cfg.experiment_auto_down_sample_rows_threshold:
             kwargs['down_sample_search'] = True
 
@@ -297,15 +348,16 @@
     search_callbacks = append_early_stopping_callbacks(search_callbacks)
 
     if callbacks is None:
         callbacks = default_experiment_callbacks()
 
     if eval_data is not None:
         from hypernets.experiment import MLEvaluateCallback
-        if task in [const.TASK_REGRESSION, const.TASK_BINARY, const.TASK_MULTICLASS]:
+        if task in [const.TASK_REGRESSION, const.TASK_BINARY, const.TASK_MULTICLASS]\
+                and searcher.kind() == const.SEARCHER_SOO:
             if evaluation_persist_prediction is True:
                 persist_dir = evaluation_persist_prediction_dir
             else:
                 persist_dir = None
             callbacks.append(MLEvaluateCallback(evaluation_metrics, persist_dir))
 
     if report_render is not None:
```

### Comparing `hypernets-0.2.5.7/hypernets/experiment/cfg.py` & `hypernets-0.3.0/hypernets/experiment/cfg.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/experiment/compete.py` & `hypernets-0.3.0/hypernets/experiment/compete.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,14 +82,15 @@
     ENSEMBLE = 'ensemble'
     TRAINING = 'training'
     PSEUDO_LABELING = 'pseudo_labeling'
     FEATURE_RESELECTION = 'feature_reselection'
     FINAL_SEARCHING = 'two_stage_searching'
     FINAL_ENSEMBLE = 'final_ensemble'
     FINAL_TRAINING = 'final_train'
+    FINAL_MOO = 'final_moo'
 
 
 class ExperimentStep(BaseEstimator):
     STATUS_NONE = -1
     STATUS_SUCCESS = 0
     STATUS_FAILED = 1
     STATUS_SKIPPED = 2
@@ -147,14 +148,15 @@
         params = super()._get_param_names()
         return filter(lambda x: x != 'experiment', params)
 
     def __getstate__(self):
         state = super().__getstate__()
         # Don't pickle experiment
         if 'experiment' in state.keys():
+            state = state.copy()
             state['experiment'] = None
         return state
 
     def _repr_df_(self):
         init_params = self.get_params()
         fitted_params = self.get_fitted_params()
 
@@ -992,20 +994,30 @@
                                                 until_step_name=self.name)
         if fitted_step is None:
             model = self.search(X_train.copy(), y_train.copy(),
                                 X_test=X_test.copy() if X_test is not None else None,
                                 X_eval=X_eval.copy() if X_eval is not None else None,
                                 y_eval=y_eval.copy() if y_eval is not None else None,
                                 dataset_id=dataset_id, **kwargs)
-            if model.get_best_trial() is None or model.get_best_trial().reward == 0:
+            best_trial = model.get_best_trial()
+
+            if best_trial is None:
                 raise RuntimeError('Not found available trial, change experiment settings and try again pls.')
+            else:
+                if not isinstance(best_trial, list) and best_trial.reward == 0:
+                    raise RuntimeError('Not found available trial, change experiment settings and try again pls.')
+            if isinstance(best_trial, list):
+                best_reward = [t.reward for t in best_trial]
+            else:
+                best_reward = best_trial.reward
+
             self.dataset_id = dataset_id
             self.model = model
             self.history_ = model.history
-            self.best_reward_ = model.get_best_trial().reward
+            self.best_reward_ = best_reward
         else:
             logger.info(f'reuse fitted step: {fitted_step.name}')
             self.status_ = self.STATUS_SKIPPED
             self.from_fitted_step(fitted_step)
 
         logger.info(f'{self.name} best_reward: {self.best_reward_}')
 
@@ -1014,15 +1026,15 @@
     def search(self, X_train, y_train, X_test=None, X_eval=None, y_eval=None, **kwargs):
         if X_eval is not None:
             kwargs['eval_set'] = (X_eval, y_eval)
         model = copy.deepcopy(self.experiment.hyper_model)  # copy from original hyper_model instance
         es = self.find_early_stopping_callback(model.callbacks)
         if es is not None and es.time_limit is not None and es.time_limit > 0:
             es.time_limit = self.estimate_time_limit(es.time_limit)
-        model.search(X_train, y_train, X_eval, y_eval, cv=self.cv, num_folds=self.num_folds, **kwargs)
+        model.search(X_train, y_train, X_eval, y_eval, X_test=X_test, cv=self.cv, num_folds=self.num_folds, **kwargs)
         return model
 
     def from_fitted_step(self, fitted_step):
         self.dataset_id = fitted_step.dataset_id
         self.model = fitted_step.model
         self.history_ = fitted_step.history_
         self.best_reward_ = fitted_step.best_reward_
@@ -1256,15 +1268,15 @@
         super().__init__(experiment, name)
 
         self.scorer = scorer if scorer is not None else get_scorer('neg_log_loss')
         self.ensemble_size = ensemble_size
 
     def select_trials(self, hyper_model):
         """
-        select trails to ensemble from hyper_model (and it's history)
+        select trials to ensemble from hyper_model (and it's history)
         """
         best_trials = hyper_model.get_top_trials(self.ensemble_size)
         return best_trials
 
     def build_estimator(self, hyper_model, X_train, y_train, X_eval=None, y_eval=None, **kwargs):
         trials = self.select_trials(hyper_model)
         estimators = [hyper_model.load_estimator(trial.model_file) for trial in trials]
@@ -1340,14 +1352,29 @@
             estimator = hyper_model.final_train(trial.space_sample, X_all, y_all, **kwargs)
         else:
             estimator = hyper_model.load_estimator(hyper_model.get_best_trial().model_file)
 
         return estimator
 
 
+class MOOFinalStep(EstimatorBuilderStep):
+
+    def __init__(self, experiment, name):
+        super().__init__(experiment, name)
+
+    def build_estimator(self, hyper_model, X_train, y_train, X_test=None, X_eval=None, y_eval=None, **kwargs):
+        # get the estimator that corresponding non-dominated solution
+        estimators = []
+        for t in hyper_model.history.get_best():
+            estimators.append(hyper_model.load_estimator(t.model_file))
+
+        logger.info(f"best trails are: {estimators}")
+        return estimators
+
+
 class PseudoLabelStep(ExperimentStep):
     def __init__(self, experiment, name, estimator_builder_name,
                  strategy=None, proba_threshold=None, proba_quantile=None, sample_number=None,
                  resplit=False):
         super().__init__(experiment, name)
 
         pl = get_tool_box(pd.DataFrame).pseudo_labeling(strategy=strategy)
@@ -1500,14 +1527,18 @@
             logger.info(f'create experiment with {names}, random_state={self.random_state}')
         self.steps = steps
 
         # fitted
         self.hyper_model_ = None
 
     def train(self, hyper_model, X_train, y_train, X_test, X_eval=None, y_eval=None, **kwargs):
+        tb = get_tool_box(X_train, y_train, X_test, X_eval, y_eval)
+        if tb.__name__.lower().find('dask') >= 0:
+            tb.dump_cluster_info()
+
         from_step = self.get_step_index(kwargs.pop('from_step', None), 0)
         to_step = self.get_step_index(kwargs.pop('to_step', None), len(self.steps) - 1)
         assert from_step <= to_step
 
         for i, step in enumerate(self.steps):
             if i > to_step:
                 break
@@ -1599,16 +1630,25 @@
         last_step = steps[-1]
         assert getattr(last_step, 'estimator_', None) is not None
 
         pipeline_steps = [(step.name, step) for step in steps if not step.is_transform_skipped()]
 
         if len(pipeline_steps) > 0:
             tb = get_tool_box(X_train, y_train, X_test, X_eval, y_eval)
-            pipeline_steps += [('estimator', last_step.estimator_)]
-            estimator = tb.transformers['Pipeline'](pipeline_steps)
+            last_estimator = last_step.estimator_
+            if isinstance(last_estimator, list):
+                pipelines = []
+                for item in last_estimator:
+                    pipeline_model = tb.transformers['Pipeline'](pipeline_steps + [('estimator', item)])
+                    pipelines.append(pipeline_model)
+                estimator = pipelines
+            else:
+                pipeline_steps += [('estimator', last_step.estimator_)]
+                estimator = tb.transformers['Pipeline'](pipeline_steps)
+
             if logger.is_info_enabled():
                 names = [step[0] for step in pipeline_steps]
                 logger.info(f'trained experiment pipeline: {names}')
         else:
             estimator = last_step.estimator_
             if logger.is_info_enabled():
                 logger.info(f'trained experiment estimator:\n{estimator}')
@@ -1851,15 +1891,16 @@
             try:
                 tb.collinearity_detector()
             except NotImplementedError:
                 raise NotImplementedError('collinearity_detection is not supported for your data')
 
         if feature_generation:
             if 'FeatureGenerationTransformer' not in tb.transformers.keys():
-                raise NotImplementedError('feature_generation is not supported for your data')
+                raise ValueError('feature_generation is not supported for your data, '
+                                 'or "featuretools" is not installed.')
 
             if data_cleaner_args is None:
                 data_cleaner_args = {}
             cs = tb.column_selector
             reserve_columns = data_cleaner_args.get('reserve_columns')
             reserve_columns = list(reserve_columns) if reserve_columns is not None else []
             if feature_generation_datetime_cols is None:
@@ -1993,32 +2034,39 @@
                                      max_trials=down_sample_search_max_trials,
                                      time_limit=down_sample_search_time_limit))
             else:
                 steps.append(creator(self, StepNames.FINAL_SEARCHING,
                                      cv=cv, num_folds=num_folds))
 
         # final train
-        if ensemble_size is not None and ensemble_size > 1:
-            creator = creators[StepNames.FINAL_ENSEMBLE]
-            last_step = creator(self, StepNames.FINAL_ENSEMBLE, scorer=scorer, ensemble_size=ensemble_size)
+        if hyper_model.searcher.kind() == const.SEARCHER_MOO:
+            creator = creators[StepNames.FINAL_MOO]
+            last_step = creator(self, StepNames.FINAL_MOO)
         else:
-            creator = creators[StepNames.FINAL_TRAINING]
-            last_step = creator(self, StepNames.FINAL_TRAINING, retrain_on_wholedata=retrain_on_wholedata)
+            if ensemble_size is not None and ensemble_size > 1:
+                creator = creators[StepNames.FINAL_ENSEMBLE]
+                last_step = creator(self, StepNames.FINAL_ENSEMBLE, scorer=scorer, ensemble_size=ensemble_size)
+            else:
+                creator = creators[StepNames.FINAL_TRAINING]
+                last_step = creator(self, StepNames.FINAL_TRAINING, retrain_on_wholedata=retrain_on_wholedata)
         steps.append(last_step)
 
         # ignore warnings
         import warnings
         warnings.filterwarnings('ignore')
 
         if log_level is not None:
             _set_log_level(log_level)
 
         self.run_kwargs = kwargs
 
         self.evaluation_ = None
+
+        hyper_model.context.put("exp", self)
+
         super(CompeteExperiment, self).__init__(steps,
                                                 hyper_model, X_train, y_train, X_eval=X_eval, y_eval=y_eval,
                                                 X_test=X_test, eval_size=eval_size, task=task,
                                                 id=id,
                                                 callbacks=callbacks,
                                                 random_state=random_state)
 
@@ -2036,14 +2084,15 @@
             StepNames.ENSEMBLE: EnsembleStep,
             StepNames.TRAINING: FinalTrainStep,
             StepNames.FEATURE_RESELECTION: PermutationImportanceSelectionStep,
             StepNames.PSEUDO_LABELING: PseudoLabelStep,
             StepNames.FINAL_SEARCHING: SpaceSearchWithDownSampleStep if down_sample_search else SpaceSearchStep,
             StepNames.FINAL_ENSEMBLE: EnsembleStep,
             StepNames.FINAL_TRAINING: FinalTrainStep,
+            StepNames.FINAL_MOO: MOOFinalStep,
         }
 
         tb = get_tool_box(X_train, y_train, X_test, X_eval, y_eval)
         if hasattr(tb, 'exist_dask_object') \
                 and tb.exist_dask_object(X_train, y_train, X_test, X_eval, y_eval):
             mapping[StepNames.ENSEMBLE] = DaskEnsembleStep
             mapping[StepNames.FINAL_ENSEMBLE] = DaskEnsembleStep
```

### Comparing `hypernets-0.2.5.7/hypernets/experiment/general.py` & `hypernets-0.3.0/hypernets/experiment/general.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/experiment/job.py` & `hypernets-0.3.0/hypernets/experiment/job.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/experiment/report.py` & `hypernets-0.3.0/hypernets/experiment/report.py`

 * *Files 0% similar despite different names*

```diff
@@ -860,13 +860,19 @@
                 self._write_ensemble(step)
             elif step.type == StepType.PseudoLabeling:
                 self._write_pseudo_labeling(step)
 
         logger.info(f"write report excel to {self.workbook.filename}")
         self.workbook.close()
 
+    def __getstate__(self):
+        states = dict(self.__dict__)
+        if 'workbook' in states:
+            del states['workbook']
+        return states
+
 
 def get_render(name):  # instance factory
     if name == 'excel':
         return ExcelReportRender
     raise ValueError(f"Unknown render '{name}' .")
```

### Comparing `hypernets-0.2.5.7/hypernets/hyperctl/api.py` & `hypernets-0.3.0/hypernets/hyperctl/api.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import os
+import tempfile
 
 from hypernets.hyperctl import consts,utils
 from hypernets.utils import logging as hyn_logging
 
 logger = hyn_logging.get_logger(__name__)
 
+_job_dict = {}
+
 
 def get_job(job_name, api_server_portal):
     url_get_job = f"{api_server_portal}/hyperctl/api/job/{job_name}"
     data = utils.get_request(url_get_job)
     return data
 
 
@@ -19,23 +22,47 @@
     assert job_name
     assert api_server_portal
 
     return job_name, api_server_portal
 
 
 def get_job_params():
+    global _job_dict
+    dev_job_params = _job_dict.get('params')
+    if dev_job_params is not None:
+        return dev_job_params
+
     job_name, api_server_portal = _get_job_name_and_damon_portal()
     return get_job(job_name, api_server_portal)['params']
 
 
 def get_job_data_dir():
+    global _job_dict
+    dev_job_data_dir = _job_dict.get('job_data_dir')
+    if dev_job_data_dir is not None:
+        return dev_job_data_dir
+
     job_working_dir = os.getenv(consts.KEY_ENV_JOB_WORKING_DIR)
     return job_working_dir
 
 
+def inject(params, job_data_dir=None):
+    global _job_dict
+    job_dict = _job_dict
+    job_dict['params'] = params
+    if job_data_dir is None:
+        tempfile.gettempdir()
+        job_dict['job_data_dir'] = tempfile.mkdtemp(prefix='hyperctl-')
+
+
+def reset_dev_params():
+    global _job_dict
+    _job_dict = {}
+
+
 def list_jobs(api_server_portal):
     # if api_server_portal is None:
     #     api_server_portal = os.getenv(consts.KEY_ENV_api_server_portal)
     assert api_server_portal
     url_get_jobs = f"{api_server_portal}/hyperctl/api/job"
     data = utils.get_request(url_get_jobs)
     return data['jobs']
```

### Comparing `hypernets-0.2.5.7/hypernets/hyperctl/appliation.py` & `hypernets-0.3.0/hypernets/hyperctl/appliation.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/hyperctl/batch.py` & `hypernets-0.3.0/hypernets/hyperctl/batch.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/hyperctl/callbacks.py` & `hypernets-0.3.0/hypernets/hyperctl/callbacks.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/hyperctl/cli.py` & `hypernets-0.3.0/hypernets/hyperctl/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     # 1.1. checkout output
     if output_path.exists():
         raise FileExistsError(output)
 
     # load file
     config_dict = load_yaml(yaml_file)
 
-    # 1.3. check values should be array
+    # 1.3. check values should be a list
     assert "params" in config_dict
 
     params = config_dict['params']
     for k, v in params.items():
         if not isinstance(v, list):
             raise ValueError(f"Value of param '{k}' should be list")
```

### Comparing `hypernets-0.2.5.7/hypernets/hyperctl/consts.py` & `hypernets-0.3.0/hypernets/hyperctl/consts.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/hyperctl/executor.py` & `hypernets-0.3.0/hypernets/hyperctl/executor.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/hyperctl/scheduler.py` & `hypernets-0.3.0/hypernets/hyperctl/scheduler.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/hyperctl/server.py` & `hypernets-0.3.0/hypernets/hyperctl/server.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/hyperctl/utils.py` & `hypernets-0.3.0/hypernets/hyperctl/utils.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/model/estimator.py` & `hypernets-0.3.0/hypernets/model/estimator.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,27 +2,37 @@
 """
 
 """
 import copy
 
 import numpy as np
 from sklearn.model_selection import KFold, StratifiedKFold
+from hypernets.utils import const
 
 
 class Estimator():
-    def __init__(self, space_sample, task='binary', discriminator=None):
+    def __init__(self, space_sample, task=const.TASK_BINARY, discriminator=None):
         self.space_sample = space_sample
         self.task = task
         self.discriminator = discriminator
 
         # fitted
         self.model = None
         self.cv_ = None
         self.cv_models_ = None
 
+    @property
+    def _estimator_type(self):
+        if self.task in {const.TASK_BINARY, const.TASK_MULTICLASS, const.TASK_MULTILABEL}:
+            return 'classifier'
+        elif self.task in {const.TASK_REGRESSION, }:
+            return 'regressor'
+        else:
+            return None
+
     def set_discriminator(self, discriminator):
         self.discriminator = discriminator
 
     def summary(self):
         raise NotImplementedError
 
     def fit(self, X, y, **kwargs):
```

### Comparing `hypernets-0.2.5.7/hypernets/model/hyper_model.py` & `hypernets-0.3.0/hypernets/model/hyper_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 """
 
 """
 import time
 import traceback
 from collections import UserDict
 
+from ..core.context import DefaultContext
 from ..core.meta_learner import MetaLearner
-from ..core.trial import Trial, TrialHistory, DiskTrialStore
+from ..core.trial import Trial, TrialHistory, DiskTrialStore, DominateBasedTrialHistory
 from ..discriminators import UnPromisingTrial
 from ..dispatchers import get_dispatcher
 from ..tabular import get_tool_box
 from ..utils import logging, const, to_repr
 
 logger = logging.get_logger(__name__)
 
@@ -26,165 +27,214 @@
         :param reward_metric:
         :param task:
         """
         self.searcher = searcher
         self.dispatcher = dispatcher
         self.callbacks = callbacks if callbacks is not None else []
         self.reward_metric = reward_metric
-        self.history = TrialHistory(searcher.optimize_direction)
+
+        searcher_type = searcher.kind()
+
+        if searcher_type == const.SEARCHER_MOO:
+            objective_names = [_.name for _ in searcher.objectives]
+            directions = [_.direction for _ in searcher.objectives]
+            self.history = DominateBasedTrialHistory(directions=directions, objective_names=objective_names)
+        else:
+            self.history = TrialHistory(searcher.optimize_direction)
+
         self.task = task
         self.discriminator = discriminator
         if self.discriminator:
             self.discriminator.bind_history(self.history)
 
+        self.context = DefaultContext()
+
     def _get_estimator(self, space_sample):
         raise NotImplementedError
 
+    @property
+    def reward_metrics(self):
+        if isinstance(self.reward_metric, list):
+            return self.reward_metric
+        else:
+            return [self.reward_metric]
+
     def load_estimator(self, model_file):
         raise NotImplementedError
 
-    def _run_trial(self, space_sample, trial_no, X, y, X_eval, y_eval, cv=False, num_folds=3, model_file=None,
-                   **fit_kwargs):
-
+    def _run_trial(self, space_sample, trial_no, X, y, X_eval, y_eval, X_test=None, cv=False, num_folds=3,
+                   model_file=None, **fit_kwargs):
         start_time = time.time()
         estimator = self._get_estimator(space_sample)
         if self.discriminator:
             estimator.set_discriminator(self.discriminator)
 
         for callback in self.callbacks:
             try:
                 callback.on_build_estimator(self, space_sample, estimator, trial_no)
             except Exception as e:
                 logger.warn(e)
 
         metrics = fit_kwargs.pop('metrics') if 'metrics' in fit_kwargs else None
         if metrics is not None:
             assert isinstance(metrics, (tuple, list)), 'metrics should be list or tuple'
-            if not any(map(lambda _: _ is self.reward_metric, metrics)):
-                metrics = list(metrics) + [self.reward_metric]
+            metrics = list(set(list(metrics)).union(set(self.reward_metrics)))
         else:
-            metrics = [self.reward_metric]
+            metrics = self.reward_metrics
 
         succeeded = False
         scores = None
         oof = None
         oof_scores = None
+        x_vals = None
+        y_vals = None
+        X_trains = None
+        y_trains = None
         try:
             if cv:
-                scores, oof, oof_scores = estimator.fit_cross_validation(X, y, stratified=True, num_folds=num_folds,
-                                                                         shuffle=False, random_state=9527,
-                                                                         metrics=metrics,
-                                                                         **fit_kwargs)
+                 ret_data = estimator.fit_cross_validation(X, y, stratified=True, num_folds=num_folds, shuffle=False,
+                                                           random_state=9527, metrics=metrics, **fit_kwargs)
+                 scores, oof, oof_scores, X_trains, y_trains, x_vals, y_vals = ret_data
             else:
                 estimator.fit(X, y, **fit_kwargs)
             succeeded = True
         except UnPromisingTrial as e:
             logger.info(f'{e}')
         except Exception as e:
             logger.error(f'run_trail failed! trail_no={trial_no}')
             track = traceback.format_exc()
             logger.error(track)
 
         if succeeded:
-            if scores is None:
-                scores = estimator.evaluate(X_eval, y_eval, metrics=metrics, **fit_kwargs)
-            reward = self._get_reward(scores, self.reward_metric)
 
             if model_file is None or len(model_file) == 0:
                 model_file = '%05d_%s.pkl' % (trial_no, space_sample.space_id)
             estimator.save(model_file)
 
-            elapsed = time.time() - start_time
+            elapsed = time.time() - start_time  # Notes: does not contains evaluation
+            trial = Trial(space_sample, trial_no, reward=None, elapsed=elapsed,
+                          model_file=model_file, succeeded=succeeded)
+            trial.context = self.context
+
+            if self.searcher.kind() != const.SEARCHER_MOO:
+                if scores is None:
+                    scores = estimator.evaluate(X_eval, y_eval, metrics=metrics, **fit_kwargs)
+                reward = self._get_reward(scores, self.reward_metrics)
+            else:
+                if cv:
+                    assert x_vals is not None and y_vals is not None
+                    reward = [fn.evaluate_cv(trial, estimator, X_trains, y_trains,
+                                             x_vals, y_vals, X_test)
+                              for fn in self.searcher.objectives]
+                else:
+                    reward = [fn.evaluate(trial, estimator, X_eval, y_eval, X, y, X_test) for fn in self.searcher.objectives]
 
-            trial = Trial(space_sample, trial_no, reward, elapsed, model_file, succeeded)
+            trial.reward = reward
             trial.iteration_scores = estimator.get_iteration_scores()
             trial.memo['scores'] = scores
+
             if oof is not None and self._is_memory_enough(oof):
                 trial.memo['oof'] = oof
             if oof_scores is not None:
                 trial.memo['oof_scores'] = oof_scores
 
             # improved = self.history.append(trial)
-
             self.searcher.update_result(space_sample, reward)
         else:
             elapsed = time.time() - start_time
-            trial = Trial(space_sample, trial_no, 0, elapsed, succeeded=succeeded)
-
+            if self.searcher.kind() == const.SEARCHER_MOO:
+                nan_scores = [None] * len(self.searcher.objectives)
+            else:
+                nan_scores = 0
+            trial = Trial(space_sample, trial_no, nan_scores, elapsed, succeeded=succeeded)
             if self.history is not None:
                 t = self.history.get_worst()
                 if t is not None:
                     self.searcher.update_result(space_sample, t.reward)
 
         return trial
 
     @staticmethod
     def _is_memory_enough(oof):
         tb = get_tool_box(oof)
         free = tb.memory_free() / tb.memory_total()
         return free > 0.618
 
-    def _get_reward(self, value, key=None):
+    def _get_reward(self, value: dict, keys: list = None):
         def cast_float(value):
             try:
                 fv = float(value)
                 return fv
             except TypeError:
                 return None
 
-        if key is None:
-            key = 'reward'
-        elif callable(key) and hasattr(key, '__name__'):
-            key = key.__name__
-
-        fv = cast_float(value)
-        if fv is not None:
-            reward = fv
-        elif isinstance(value, (dict, UserDict)) and key in value and cast_float(value[key]) is not None:
-            reward = cast_float(value[key])
-        else:
-            raise ValueError(
-                f'[value] should be a numeric or a dict which has a key named "{key}" whose value is a numeric.')
-        return reward
+        if keys is None:
+            keys = ['reward']
+
+        if not isinstance(value, (dict, UserDict)):
+            raise ValueError(f"[value] should be a dict but is {value} ")
+
+        rewards = []
+        for key in keys:
+            if callable(key) and hasattr(key, '__name__'):
+                key_name = key.__name__
+            else:
+                key_name = key
+            if key_name in value:
+                reward = cast_float(value[key_name])
+                if reward is not None:
+                    rewards.append(reward)
+                else:
+                    raise ValueError(
+                        f'[value] should be a numeric or a dict which has a key named "{key}" whose value is a numeric.')
+
+        return rewards
 
     def get_best_trial(self):
         return self.history.get_best()
 
     @property
     def best_reward(self):
         best = self.get_best_trial()
         if best is not None:
-            return best.reward
+            if isinstance(best, list):
+                return [t.reward for t in best]
+            else:
+                return best.reward
         else:
             return None
 
     @property
     def best_trial_no(self):
         best = self.get_best_trial()
         if best is not None:
-            return best.trial_no
+            if isinstance(best, list):
+                return [t.trial_no for t in best]
+            else:
+                return best.trial_no
         else:
             return None
 
     def get_top_trials(self, top_n):
         return self.history.get_top(top_n)
 
     def _before_search(self):
         pass
 
     def _after_search(self, last_trial_no):
         pass
 
-    def search(self, X, y, X_eval, y_eval, cv=False, num_folds=3, max_trials=10, dataset_id=None, trial_store=None,
+    def search(self, X, y, X_eval, y_eval, X_test=None, cv=False, num_folds=3, max_trials=10, dataset_id=None, trial_store=None,
                **fit_kwargs):
         """
         :param X: Pandas or Dask DataFrame, feature data for training
         :param y: Pandas or Dask Series, target values for training
         :param X_eval: (Pandas or Dask DataFrame) or None, feature data for evaluation
         :param y_eval: (Pandas or Dask Series) or None, target values for evaluation
+        :param X_test: (Pandas or Dask Series) or None, target values for evaluation of indicators like PSI
         :param cv: Optional, int(default=False), If set to `true`, use cross-validation instead of evaluation set reward to guide the search process
         :param num_folds: Optional, int(default=3), Number of cross-validated folds, only valid when cv is true
         :param max_trials: Optional, int(default=10), The upper limit of the number of search trials, the search process stops when the number is exceeded
         :param dataset_id:
         :param trial_store:
         :param fit_kwargs: Optional, dict, parameters for fit method of model
         :return:
@@ -210,15 +260,15 @@
                 callback.on_search_start(self, X, y, X_eval, y_eval,
                                          cv, num_folds, max_trials, dataset_id, trial_store,
                                          **fit_kwargs)
             except Exception as e:
                 logger.warn(e)
 
         try:
-            trial_no = dispatcher.dispatch(self, X, y, X_eval, y_eval,
+            trial_no = dispatcher.dispatch(self, X, y, X_eval, y_eval, X_test,
                                            cv, num_folds, max_trials, dataset_id, trial_store,
                                            **fit_kwargs)
 
             for callback in self.callbacks:
                 try:
                     callback.on_search_end(self)
                 except Exception as e:
```

### Comparing `hypernets-0.2.5.7/hypernets/pipeline/base.py` & `hypernets-0.3.0/hypernets/pipeline/base.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/pipeline/transformers.py` & `hypernets-0.3.0/hypernets/pipeline/transformers.py`

 * *Files 1% similar despite different names*

```diff
@@ -371,7 +371,16 @@
             kwargs['datetime_cols'] = datetime_cols
         if max_depth != 1:
             kwargs['max_depth'] = max_depth
         if feature_selection_args is not None:
             kwargs['feature_selection_args'] = feature_selection_args
 
         HyperTransformer.__init__(self, feature_generators.FeatureGenerationTransformer, space, name, **kwargs)
+
+
+class FeatureImportanceSelection(HyperTransformer):
+    def __init__(self, quantile, importances, space=None, name=None,  **kwargs):
+        if kwargs is None:
+            kwargs = {}
+
+        HyperTransformer.__init__(self, sklearn_ex.FeatureImportanceSelection, space, name, quantile=quantile,
+                                  importances=importances, **kwargs)
```

### Comparing `hypernets-0.2.5.7/hypernets/searchers/__init__.py` & `hypernets-0.3.0/hypernets/searchers/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 """
 
 """
 __author__ = 'yangjian'
 
 from .evolution_searcher import EvolutionSearcher
 from .mcts_searcher import MCTSSearcher
+from .moead_searcher import MOEADSearcher
+from .nsga_searcher import NSGAIISearcher, RNSGAIISearcher
 from .random_searcher import RandomSearcher
 from .playback_searcher import PlaybackSearcher
 from .grid_searcher import GridSearcher
 from ..core.searcher import Searcher
 
 searcher_dict = {
     'mcts': MCTSSearcher,
@@ -22,15 +24,21 @@
     'RandomSearcher': RandomSearcher,
     'random': RandomSearcher,
     'grid': GridSearcher,
     'Grid': GridSearcher,
     'GridSearcher': GridSearcher,
     'playback': PlaybackSearcher,
     'PlaybackSearcher': PlaybackSearcher,
-    'Playback': PlaybackSearcher
+    'Playback': PlaybackSearcher,
+    'nsga2': NSGAIISearcher,
+    'rnsga2': RNSGAIISearcher,
+    'NSGAIISearcher': NSGAIISearcher,
+    'RNSGAIISearcher': RNSGAIISearcher,
+    'moead': MOEADSearcher,
+    'MOEADSearcher': MOEADSearcher
 }
 
 
 def get_searcher_cls(identifier):
     if isinstance(identifier, str):
         cls = searcher_dict.get(identifier, None)
         if cls is None:
@@ -42,20 +50,24 @@
             return identifier
         else:
             raise ValueError(f'Wrong searcher type:{identifier}')
     else:
         raise ValueError(f'Illegal identifier:{identifier}')
 
 
-def make_searcher(cls, search_space_fn, optimize_direction='min', **kwargs):
+def make_searcher(cls, search_space_fn, optimize_direction='min', objectives=None, **kwargs):
+    from hypernets.searchers.moo import MOOSearcher
+
     cls = get_searcher_cls(cls)
 
     if cls == EvolutionSearcher:
         default_kwargs = dict(population_size=30, sample_size=10, candidates_size=10,
-                              regularized=True, use_meta_learner=True)
+                              regularized=True, use_meta_learner=True, optimize_direction=optimize_direction)
     elif cls == MCTSSearcher:
-        default_kwargs = dict(max_node_space=10)
+        default_kwargs = dict(max_node_space=10, optimize_direction=optimize_direction)
+    elif issubclass(cls, MOOSearcher):
+        default_kwargs = dict(objectives=objectives)
     else:
         default_kwargs = {}
     kwargs = {**default_kwargs, **kwargs}
-    searcher = cls(search_space_fn, optimize_direction=optimize_direction, **kwargs)
+    searcher = cls(search_space_fn, **kwargs)
     return searcher
```

### Comparing `hypernets-0.2.5.7/hypernets/searchers/evolution_searcher.py` & `hypernets-0.3.0/hypernets/searchers/evolution_searcher.py`

 * *Files 6% similar despite different names*

```diff
@@ -84,45 +84,48 @@
                     hp.assign(new_value)
                 else:
                     hp.assign(parent_params[i].value)
         return offspring_space
 
 
 class EvolutionSearcher(Searcher):
-    """
-    Evolutionary Algorithm
+    """Evolutionary Algorithm
+
+    Parameters
+    ----------
+    space_fn: callable, required
+        A search space function which when called returns a `HyperSpace` instance
+    population_size: int, required
+        Size of population
+    sample_size: int, required
+        The number of parent candidates selected in each cycle of evolution
+    regularized: bool
+        (default=False), Whether to enable regularized
+    candidates_size: int, (default=10)
+        The number of samples for the meta-learner to evaluate candidate paths when roll out
+    optimize_direction: 'min' or 'max', (default='min')
+        Whether the search process is approaching the maximum or minimum reward value.
+    use_meta_learner: bool, (default=True)
+        Whether to enable meta leaner. Meta-learner aims to evaluate the performance of unseen samples based on
+        previously evaluated samples. It provides a practical solution to accurately estimate a search branch with
+        many simulations without involving the actual training.
+    space_sample_validation_fn: callable or None, (default=None)
+        Used to verify the validity of samples from the search space, and can be used to add specific constraint
+        rules to the search space to reduce the size of the space.
 
     References
     ----------
         Real, Esteban, et al. "Regularized evolution for image classifier architecture search." Proceedings of the aaai conference on artificial intelligence. Vol. 33. 2019.
     """
 
     def __init__(self, space_fn, population_size, sample_size, regularized=False,
                  candidates_size=10, optimize_direction=OptimizeDirection.Minimize, use_meta_learner=True,
                  space_sample_validation_fn=None, random_state=None):
         """
-        :param space_fn: callable, required
-            A search space function which when called returns a `HyperSpace` instance
-        :param population_size: int, required
-            Size of population
-        :param sample_size: int, required
-            The number of parent candidates selected in each cycle of evolution
-        :param regularized: bool
-            (default=False), Whether to enable regularized
-        :param candidates_size: int, (default=10)
-            The number of samples for the meta-learner to evaluate candidate paths when roll out
-        :param optimize_direction: 'min' or 'max', (default='min')
-            Whether the search process is approaching the maximum or minimum reward value.
-        :param use_meta_learner: bool, (default=True)
-            Whether to enable meta leaner. Meta-learner aims to evaluate the performance of unseen samples based on
-            previously evaluated samples. It provides a practical solution to accurately estimate a search branch with
-            many simulations without involving the actual training.
-        :param space_sample_validation_fn: callable or None, (default=None)
-            Used to verify the validity of samples from the search space, and can be used to add specific constraint
-            rules to the search space to reduce the size of the space.
+
         """
         Searcher.__init__(self, space_fn=space_fn, optimize_direction=optimize_direction,
                           use_meta_learner=use_meta_learner, space_sample_validation_fn=space_sample_validation_fn)
         self.random_state = random_state if random_state is not None else get_random_state()
         self.population = Population(size=population_size, optimize_direction=optimize_direction,
                                      random_state=self.random_state)
         self.sample_size = sample_size
@@ -133,15 +136,15 @@
     def population_size(self):
         return self.population.size
 
     @property
     def parallelizable(self):
         return True
 
-    def sample(self):
+    def sample(self, space_options=None):
         if self.population.initializing:
             space_sample = self._sample_and_check(self._random_sample)
             return space_sample
         else:
             best = self.population.sample_best(self.sample_size)
             offspring = self._get_offspring(best.space_sample)
             if offspring is not None:
@@ -183,14 +186,16 @@
             try:
                 candidate = self._sample_and_check(lambda: self.population.mutate(space_sample, new_space))
                 return candidate
             except:
                 return None
 
     def update_result(self, space_sample, result):
+        result = result[0]
+
         if not self.population.initializing:
             self.population.eliminate(regularized=self.regularized)
         self.population.append(space_sample, result)
         if self.use_meta_learner and self.meta_learner is not None:
             assert self.meta_learner is not None
             self.meta_learner.new_sample(space_sample)
```

### Comparing `hypernets-0.2.5.7/hypernets/searchers/grid_searcher.py` & `hypernets-0.3.0/hypernets/searchers/grid_searcher.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         self.all_combinations = list(ParameterGrid(self.grid))
         self.position_ = -1
 
     @property
     def parallelizable(self):
         return True
 
-    def sample(self):
+    def sample(self, space_options=None):
         sample = self._sample_and_check(self._get_sample)
         return sample
 
     def _get_sample(self):
         self.position_ += 1
 
         if self.position_ >= len(self.all_combinations):
```

### Comparing `hypernets-0.2.5.7/hypernets/searchers/mcts_core.py` & `hypernets-0.3.0/hypernets/searchers/mcts_core.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/searchers/mcts_searcher.py` & `hypernets-0.3.0/hypernets/searchers/mcts_searcher.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,39 +4,43 @@
 
 """
 from .mcts_core import *
 from ..core.searcher import Searcher, OptimizeDirection
 
 
 class MCTSSearcher(Searcher):
-    """
+    """MCTSSearcher
+
+    Parameters
+    ----------
+    space_fn: Callable
+        A search space function which when called returns a `HyperSpace` object.
+    policy: hypernets.searchers.mcts_core.BasePolicy, (default=None)
+        The policy for *Selection* and *Backpropagation* phases, `UCT` by default.
+    max_node_space: int, (default=10)
+        Maximum space for node expansion
+    candidates_size: int, (default=10)
+        The number of samples for the meta-learner to evaluate candidate paths when roll out
+    optimize_direction: 'min' or 'max', (default='min')
+        Whether the search process is approaching the maximum or minimum reward value
+    use_meta_learner: bool, (default=True)
+        Meta-learner aims to evaluate the performance of unseen samples based on previously evaluated samples. It provides a practical solution to accurately estimate a search branch with many simulations without involving the actual training
+    space_sample_validation_fn: Callable or None, (default=None)
+        Used to verify the validity of samples from the search space, and can be used to add specific constraint rules to the search space to reduce the size of the space
+
     References
     ----------
-        Wang, Linnan, et al. "Alphax: exploring neural architectures with deep neural networks and monte carlo tree search." arXiv preprint arXiv:1903.11059 (2019).
-        Browne, Cameron B., et al. "A survey of monte carlo tree search methods." IEEE Transactions on Computational Intelligence and AI in games 4.1 (2012): 1-43.
+
+    [1] Wang, Linnan, et al. "Alphax: exploring neural architectures with deep neural networks and monte carlo tree search." arXiv preprint arXiv:1903.11059 (2019).
+
+    [2] Browne, Cameron B., et al. "A survey of monte carlo tree search methods." IEEE Transactions on Computational Intelligence and AI in games 4.1 (2012): 1-43.
     """
 
     def __init__(self, space_fn, policy=None, max_node_space=10, candidates_size=10,
                  optimize_direction=OptimizeDirection.Minimize, use_meta_learner=True, space_sample_validation_fn=None):
-        """
-        :param space_fn: Callable
-            A search space function which when called returns a `HyperSpace` object.
-        :param policy: hypernets.searchers.mcts_core.BasePolicy, (default=None)
-            The policy for *Selection* and *Backpropagation* phases, `UCT` by default.
-        :param max_node_space: int, (default=10)
-            Maximum space for node expansion
-        :param candidates_size: int, (default=10)
-            The number of samples for the meta-learner to evaluate candidate paths when roll out
-        :param optimize_direction: 'min' or 'max', (default='min')
-            Whether the search process is approaching the maximum or minimum reward value
-        :param use_meta_learner: bool, (default=True)
-            Meta-learner aims to evaluate the performance of unseen samples based on previously evaluated samples. It provides a practical solution to accurately estimate a search branch with many simulations without involving the actual training
-        :param space_sample_validation_fn: Callable or None, (default=None)
-            Used to verify the validity of samples from the search space, and can be used to add specific constraint rules to the search space to reduce the size of the space
-        """
         if policy is None:
             policy = UCT()
         self.tree = MCTree(space_fn, policy, max_node_space=max_node_space)
         Searcher.__init__(self, space_fn, optimize_direction, use_meta_learner=use_meta_learner,
                           space_sample_validation_fn=space_sample_validation_fn)
         self.nodes_map = {}
         self.candidates_size = candidates_size
@@ -44,15 +48,15 @@
     @property
     def max_node_space(self):
         return self.tree.max_node_space
 
     def parallelizable(self):
         return self.use_meta_learner and self.meta_learner is not None
 
-    def sample(self):
+    def sample(self, space_options=None):
         # print('Sample')
         _, best_node = self.tree.selection_and_expansion()
         # print(f'Sample: {best_node.info()}')
 
         if self.use_meta_learner and self.meta_learner is not None:
             space_sample, candidate_sim_score, candidates_avg_score = self._select_best_candidate(best_node)
             # support for parallelize sampling
@@ -85,14 +89,15 @@
         # print(f'selected candidates scores:{scores}, argmax:{index}')
         return candidates[index], candidate_sim_score, candidates_avg_score
 
     def get_best(self):
         raise NotImplementedError
 
     def update_result(self, space_sample, result):
+        result = result[0]
         best_node = self.nodes_map[space_sample.space_id]
         # print(f'Update result: space:{space_sample.space_id}, result:{result}, node:{best_node.info()}')
         self.tree.back_propagation(best_node, result)
         # print(f'After back propagation: {best_node.info()}')
         # print('\n\n')
         if self.use_meta_learner and self.meta_learner is not None:
             assert self.meta_learner is not None
```

### Comparing `hypernets-0.2.5.7/hypernets/searchers/playback_searcher.py` & `hypernets-0.3.0/hypernets/searchers/playback_searcher.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
         super(PlaybackSearcher, self).__init__(None, use_meta_learner=False, optimize_direction=optimize_direction)
 
     @property
     def parallelizable(self):
         return True
 
-    def sample(self):
+    def sample(self, space_options=None):
         if self.index >= len(self.samples):
             raise EarlyStoppingError('no more samples.')
         sample = self.samples[self.index]
         self.index += 1
         return sample
 
     def update_result(self, space, result):
```

### Comparing `hypernets-0.2.5.7/hypernets/searchers/random_searcher.py` & `hypernets-0.3.0/hypernets/searchers/random_searcher.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     def __init__(self, space_fn, optimize_direction=OptimizeDirection.Minimize, space_sample_validation_fn=None):
         Searcher.__init__(self, space_fn, optimize_direction, space_sample_validation_fn=space_sample_validation_fn)
 
     @property
     def parallelizable(self):
         return True
 
-    def sample(self):
+    def sample(self, space_options=None):
         sample = self._sample_and_check(self._random_sample)
         return sample
 
     def get_best(self):
         raise NotImplementedError
 
     def update_result(self, space, result):
```

### Comparing `hypernets-0.2.5.7/hypernets/tabular/__init__.py` & `hypernets-0.3.0/hypernets/tabular/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 # -*- coding:utf-8 -*-
 """
 
 """
 from ._base import get_tool_box, register_toolbox, register_transformer, tb_transformer
 from .toolbox import ToolBox
 
-register_toolbox(ToolBox)
+register_toolbox(ToolBox, aliases=('default', 'pandas'))
 
 try:
     import dask.dataframe as dd
 
     import dask_ml
     from .dask_ex import DaskToolBox
 
-    register_toolbox(DaskToolBox, 0)
+    register_toolbox(DaskToolBox, pos=0, aliases=('dask',))
     is_dask_installed = True
 except ImportError:
     # import traceback
     # traceback.print_exc()
     is_dask_installed = False
 
 try:
     import cupy
     import cudf
     import cuml
     from .cuml_ex import CumlToolBox
 
-    register_toolbox(CumlToolBox, 0)
+    register_toolbox(CumlToolBox, pos=0, aliases=('cuml', 'rapids'))
     is_cuml_installed = True
 except ImportError:
     # import traceback
     #
     # traceback.print_exc()
     is_cuml_installed = False
```

### Comparing `hypernets-0.2.5.7/hypernets/tabular/_base.py` & `hypernets-0.3.0/hypernets/tabular/_base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # -*- coding:utf-8 -*-
 """
 
 """
-from collections import namedtuple
 import time
+from collections import namedtuple
 
 TbNamedEntity = namedtuple('TbNamedEntity', ['entity', 'name', 'dtypes'])
 
 _tool_boxes = []
 _tool_boxes_update_at = 0
 
 _tb_transformers = []  # list of TbNamedEntity
 _tb_transformers_update_at = 0
 
 _tb_extensions = []  # list of TbNamedEntity
 _tb_extensions_update_at = 0
 
 
-def register_toolbox(tb, pos=None):
+def register_toolbox(tb, pos=None, aliases=None):
     if pos is None:
-        _tool_boxes.append(tb)
+        _tool_boxes.append((tb, aliases))
     else:
-        _tool_boxes.insert(pos, tb)
+        _tool_boxes.insert(pos, (tb, aliases))
 
     global _tool_boxes_update_at
     _tool_boxes_update_at = time.time()
 
 
 def register_transformer(transformer_cls, *, name=None, dtypes=None):
     assert isinstance(transformer_cls, type)
@@ -57,20 +57,27 @@
     _tb_extensions.append(TbNamedEntity(entity=extension, name=name, dtypes=dtypes))
 
     global _tb_extensions_update_at
     _tb_extensions_update_at = time.time()
 
 
 def get_tool_box(*data):
-    for tb in _tool_boxes:
-        if tb.accept(*data):
-            return tb
+    assert len(data) > 0
+    if len(data) == 1 and isinstance(data[0], str):
+        # get toolbox by alias
+        for tb, aliases in _tool_boxes:
+            if aliases is not None and data[0] in aliases:
+                return tb
+    else:
+        for tb, _ in _tool_boxes:
+            if tb.accept(*data):
+                return tb
 
     raise ValueError(f'No toolbox found for your data with types: {[type(x) for x in data]}. '
-                     f'Registered tabular toolboxes are {[t.__name__ for t in _tool_boxes]}.')
+                     f'Registered tabular toolboxes are {[tb.__name__ for tb, _ in _tool_boxes]}.')
 
 
 def get_transformers(dtypes):
     """
     Find available transformers for the specified dtypes
     """
     return _filter_entities(_tb_transformers, dtypes)
```

### Comparing `hypernets-0.2.5.7/hypernets/tabular/cache.py` & `hypernets-0.3.0/hypernets/tabular/cache.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,28 @@
 _STRATEGY_TRANSFORM = 'transform'
 
 _KIND_DEFAULT = 'pickle'
 _KIND_PARQUET = 'parquet'
 _KIND_LIST = 'list'
 _KIND_NONE = 'none'
 
+_is_parquet_ready_flag = None
+
+
+def _is_parquet_ready(tb):
+    global _is_parquet_ready_flag
+    if _is_parquet_ready_flag is None:
+        try:
+            tb.parquet()
+            _is_parquet_ready_flag = True
+        except ImportError as e:
+            logger.warning(f'{e}, so cache strategy "{_STRATEGY_DATA}" is disabled.')
+            _is_parquet_ready_flag = False
+    return _is_parquet_ready_flag
+
 
 class SkipCache(Exception):
     pass
 
 
 class CacheCallback:
     def on_enter(self, fn, *args, **kwargs):
@@ -191,14 +205,17 @@
         if cache_path is not None and not loaded:
             try:
                 for c in callbacks:
                     c.on_store(fn, result, *args, **kwargs)
 
                 # store cache
                 cache_strategy = strategy if strategy is not None else cfg.cache_strategy
+                if cache_strategy == _STRATEGY_DATA and not _is_parquet_ready(tb):
+                    cache_strategy = _STRATEGY_TRANSFORM
+
                 if cache_strategy == _STRATEGY_TRANSFORM and (result is None or transformer is not None):
                     cache_data = None
                     meta = {'strategy': _STRATEGY_TRANSFORM}
                 else:
                     cache_data = result
                     meta = {'strategy': _STRATEGY_DATA}
 
@@ -237,15 +254,15 @@
     meta['version'] = __version__
 
     if data is None:
         meta.update({'kind': _KIND_NONE, 'items': []})
     elif isinstance(data, (list, tuple)):
         items = [f'_{i}' for i in range(len(data))]
         for d, i in zip(data, items):
-            _store_cache(f'{cache_path}{i}', d, meta)
+            _store_cache(toolbox, f'{cache_path}{i}', d, meta)
         meta.update({'kind': _KIND_LIST, 'items': items})
     else:
         pq = toolbox.parquet()
         if isinstance(data, pq.acceptable_types):
             item = f'.parquet'
             pq.store(data, f'{cache_path}{item}', filesystem=fs)
             meta.update({'kind': _KIND_PARQUET, 'items': [item]})
@@ -268,15 +285,15 @@
 
     data_kind = meta['kind']
     items = meta['items']
 
     if data_kind == _KIND_NONE:
         data = None
     elif data_kind == _KIND_LIST:
-        data = [_load_cache(f'{cache_path}{i}')[0] for i in items]
+        data = [_load_cache(toolbox, f'{cache_path}{i}')[0] for i in items]
     elif data_kind == _KIND_DEFAULT:  # pickle
         with fs.open(f'{cache_path}{items[0]}', 'rb') as f:
             data = pickle.load(f)
     elif data_kind == _KIND_PARQUET:
         pq = toolbox.parquet()
         data = pq.load(f'{cache_path}{items[0]}', filesystem=fs)
     else:
```

### Comparing `hypernets-0.2.5.7/hypernets/tabular/cfg.py` & `hypernets-0.3.0/hypernets/tabular/cfg.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tabular/collinearity.py` & `hypernets-0.3.0/hypernets/tabular/collinearity.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tabular/column_selector.py` & `hypernets-0.3.0/hypernets/tabular/column_selector.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,15 +170,15 @@
             return v is None or \
                    (isinstance(v, tuple) and len(v) == 2 and -90.0 <= v[0] <= 90.0 and -180.0 <= v[1] <= 180.0)
         except:
             return False
 
     @staticmethod
     def _reduce_is_latlong(df):
-        fn = np.vectorize(LatLongColumnSelector._is_latlong, otypes=[np.bool], signature='()->()')
+        fn = np.vectorize(LatLongColumnSelector._is_latlong, otypes=[bool], signature='()->()')
         return df.apply(fn).all(axis=0)
 
 
 class MinMaxColumnSelector(object):
     def __init__(self, min=None, max=None):
         self.min = min
         self.max = max
```

### Comparing `hypernets-0.2.5.7/hypernets/tabular/cuml_ex/_data_cleaner.py` & `hypernets-0.3.0/hypernets/tabular/cuml_ex/_data_cleaner.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tabular/cuml_ex/_data_hasher.py` & `hypernets-0.3.0/hypernets/tabular/cuml_ex/_data_hasher.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tabular/cuml_ex/_dataframe_mapper.py` & `hypernets-0.3.0/hypernets/tabular/cuml_ex/_dataframe_mapper.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tabular/cuml_ex/_drift_detection.py` & `hypernets-0.3.0/hypernets/tabular/cuml_ex/_drift_detection.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tabular/cuml_ex/_ensemble.py` & `hypernets-0.3.0/hypernets/tabular/cuml_ex/_ensemble.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tabular/cuml_ex/_estimator.py` & `hypernets-0.3.0/hypernets/tabular/cuml_ex/_estimator.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tabular/cuml_ex/_estimator_detector.py` & `hypernets-0.3.0/hypernets/tabular/cuml_ex/_estimator_detector.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tabular/cuml_ex/_metrics.py` & `hypernets-0.3.0/hypernets/tabular/cuml_ex/_metrics.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tabular/cuml_ex/_model_selection.py` & `hypernets-0.3.0/hypernets/tabular/cuml_ex/_model_selection.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tabular/cuml_ex/_persistence.py` & `hypernets-0.3.0/hypernets/tabular/cuml_ex/_persistence.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tabular/cuml_ex/_pseudo_labeling.py` & `hypernets-0.3.0/hypernets/tabular/cuml_ex/_pseudo_labeling.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tabular/cuml_ex/_toolbox.py` & `hypernets-0.3.0/hypernets/tabular/cuml_ex/_toolbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 import pandas as pd
 from cuml.common.array import CumlArray
 
 from hypernets.utils import const, logging
 from . import _data_cleaner
 from . import _dataframe_mapper, _metrics, _data_hasher, _model_selection, _ensemble, _drift_detection
 from . import _estimator_detector
-from . import _persistence
 from . import _pseudo_labeling
 from . import _transformer  # NOQA,  register customized transformer
 from .. import sklearn_ex as sk_ex
 from ..toolbox import ToolBox, register_transformer, randint
 
 try:
     import xgboost
@@ -154,14 +153,15 @@
                 'json': cudf.read_json,
             }
         df = ToolBox.load_data(data_path, reset_index=reset_index, reader_mapping=reader_mapping, **kwargs)
         return df
 
     @staticmethod
     def parquet():
+        from . import _persistence
         return _persistence.CumlParquetPersistence()
 
     @staticmethod
     def unique(y):
         if isinstance(y, cudf.Series):
             uniques = y.unique().to_pandas().values
             uniques = set(uniques)
```

### Comparing `hypernets-0.2.5.7/hypernets/tabular/cuml_ex/_transformer.py` & `hypernets-0.3.0/hypernets/tabular/cuml_ex/_transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -246,17 +246,23 @@
         return target
 
 
 @tb_transformer(cudf.DataFrame, name='OneHotEncoder')
 class LocalizableOneHotEncoder(OneHotEncoder, Localizable):
     def as_local(self):
         from .. import CumlToolBox
-        target = sk_pre.OneHotEncoder(categories=CumlToolBox.to_local(self.categories)[0],
-                                      drop=self.drop, sparse=self.sparse,
-                                      dtype=self.dtype, handle_unknown=self.handle_unknown)
+        options = dict(categories=CumlToolBox.to_local(self.categories)[0],
+                       drop=self.drop,  # sparse=self.sparse,
+                       dtype=self.dtype, handle_unknown=self.handle_unknown)
+        if 'sparse_output' in inspect.signature(sk_pre.OneHotEncoder.__init__).parameters.keys():
+            # above sklearn 1.2
+            options['sparse_output'] = self.sparse
+        else:
+            options['sparse'] = self.sparse
+        target = sk_pre.OneHotEncoder(**options)
         copy_attrs_as_local(self, target, 'categories_', 'drop_idx_')
 
         try:
             if hasattr(target, '_compute_n_features_outs'):
                 target._infrequent_enabled = False
                 target._n_features_outs = target._compute_n_features_outs()
         except:
```

### Comparing `hypernets-0.2.5.7/hypernets/tabular/dask_ex/__init__.py` & `hypernets-0.3.0/hypernets/tabular/dask_ex/__init__.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tabular/dask_ex/_collinearity.py` & `hypernets-0.3.0/hypernets/tabular/dask_ex/_collinearity.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tabular/dask_ex/_data_cleaner.py` & `hypernets-0.3.0/hypernets/tabular/dask_ex/_data_cleaner.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tabular/dask_ex/_data_hasher.py` & `hypernets-0.3.0/hypernets/tabular/dask_ex/_data_hasher.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tabular/dask_ex/_dataframe_mapper.py` & `hypernets-0.3.0/hypernets/tabular/dask_ex/_dataframe_mapper.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tabular/dask_ex/_drift_detection.py` & `hypernets-0.3.0/hypernets/tabular/dask_ex/_drift_detection.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tabular/dask_ex/_ensemble.py` & `hypernets-0.3.0/hypernets/tabular/dask_ex/_ensemble.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tabular/dask_ex/_metrics.py` & `hypernets-0.3.0/hypernets/tabular/dask_ex/_metrics.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tabular/dask_ex/_model_selection.py` & `hypernets-0.3.0/hypernets/tabular/dask_ex/_model_selection.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tabular/dask_ex/_persistence.py` & `hypernets-0.3.0/hypernets/tabular/dask_ex/_persistence.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tabular/dask_ex/_pseudo_labeling.py` & `hypernets-0.3.0/hypernets/tabular/dask_ex/_pseudo_labeling.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tabular/dask_ex/_toolbox.py` & `hypernets-0.3.0/hypernets/tabular/dask_ex/_toolbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 from hypernets.utils import logging, const, is_os_linux
 from . import _collinearity, _drift_detection, _pseudo_labeling, _model_selection, _ensemble
 from . import _data_cleaner
 from . import _data_hasher
 from . import _dataframe_mapper
 from . import _feature_generators
 from . import _metrics
-from . import _persistence
 from . import _transformers as tfs
 from .. import sklearn_ex as sk_ex
 
 try:
     import lightgbm
 
     lightgbm_installed = True
@@ -84,14 +83,39 @@
 
     @staticmethod
     def dask_worker_count():
         client = DaskToolBox.default_client()
         return len(client.ncores()) if client else 0
 
     @staticmethod
+    def dump_cluster_info(cluster=None, log_level=logging.INFO):
+        if not logger.is_enabled_for(log_level):
+            return
+
+        if cluster is None:
+            client = DaskToolBox.default_client()
+            if client is None:
+                logger.log(log_level, 'Not found dask default client.')
+                return
+            cluster = client.cluster
+
+        msgs = [f'Dask cluster: {cluster}', ]
+        try:
+            msgs.append(f'scheduler: {cluster.scheduler}')
+            msgs.append('workers:')
+            GB = 1024 ** 3
+            for i, wk in cluster.workers.items():
+                mem_limit = wk.memory_limit / GB
+                msgs.append(f'\t[{i}]: {wk}, mem: {mem_limit:.1f}GB')
+        except:
+            pass
+
+        logger.log(log_level, '\n'.join(msgs))
+
+    @staticmethod
     def is_dask_dataframe(X):
         return isinstance(X, dd.DataFrame)
 
     @staticmethod
     def is_dask_series(X):
         return isinstance(X, dd.Series)
 
@@ -207,14 +231,15 @@
             uniques = set(uniques)
         else:
             uniques = ToolBox.unique(y)
         return uniques
 
     @staticmethod
     def parquet():
+        from . import _persistence
         return _persistence.DaskParquetPersistence()
 
     # @staticmethod
     # def unique_array(ar, return_index=False, return_inverse=False, return_counts=False, axis=None):
     #     assert axis is None or axis == 0
     #     return da.unique(ar, return_index=return_index, return_inverse=return_inverse, return_counts=return_counts)
     @staticmethod
@@ -791,13 +816,16 @@
     # CategorizeEncoder=tfs.CategorizeEncoder,
     # MultiKBinsDiscretizer=tfs.MultiKBinsDiscretizer,
     # MultiVarLenFeatureEncoder=tfs.MultiVarLenFeatureEncoder,
     # LocalizedTfidfVectorizer=tfs.LocalizedTfidfVectorizer,
 
     # TfidfEncoder=sk_ex.TfidfEncoder,
     # DatetimeEncoder=sk_ex.DatetimeEncoder,
-    FeatureGenerationTransformer=_feature_generators.DaskFeatureGenerationTransformer,
+    # FeatureGenerationTransformer=_feature_generators.DaskFeatureGenerationTransformer,
     FeatureImportancesSelectionTransformer=sk_ex.FeatureImportancesSelectionTransformer,
 )
 
+if _feature_generators.is_feature_generator_ready:
+    _predefined_transformers['FeatureGenerationTransformer'] = _feature_generators.DaskFeatureGenerationTransformer
+
 for name, tf in _predefined_transformers.items():
     register_transformer(tf, name=name, dtypes=dd.DataFrame)
```

### Comparing `hypernets-0.2.5.7/hypernets/tabular/dask_ex/_transformers.py` & `hypernets-0.3.0/hypernets/tabular/dask_ex/_transformers.py`

 * *Files 1% similar despite different names*

```diff
@@ -256,15 +256,15 @@
         unseen = cat.shape[0]  # len(cat)
         if unseen >= xi >= 1:
             return cat[xi - 1]
         else:
             dtype = dtypes[col]
             if dtype in (np.float32, np.float64, float):
                 return np.nan
-            elif dtype in (np.int32, np.int64, np.int, np.uint32, np.uint64, np.uint):
+            elif dtype in (np.int32, np.int64, np.uint32, np.uint64, np.uint, int):
                 return -1
             else:
                 return None
 
     pdf = pdf.copy()
     for col in categories.keys():
         vf = np.vectorize(decode_column, excluded='col', otypes=[dtypes[col]])
@@ -887,15 +887,15 @@
     def fit_part(part, max_features=None, max_df=None, min_df=None):
         t = skex.LocalizedTfidfVectorizer(use_idf=False, max_features=max_features, max_df=max_df, min_df=min_df)
         t.fit(part)
         return pd.Series(t.vocabulary_)
 
     @staticmethod
     def agg_part(part):
-        return pd.Series(index=part.columns)
+        return pd.Series(index=part.columns, dtype='f8')
 
     @staticmethod
     def transform_part(part, voc):
         t = skex.LocalizedTfidfVectorizer(use_idf=False, vocabulary=voc)
         t.fit(np.array(['']))
         result = t.transform(part).toarray()
```

### Comparing `hypernets-0.2.5.7/hypernets/tabular/data_cleaner.py` & `hypernets-0.3.0/hypernets/tabular/data_cleaner.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tabular/data_hasher.py` & `hypernets-0.3.0/hypernets/tabular/data_hasher.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tabular/dataframe_mapper.py` & `hypernets-0.3.0/hypernets/tabular/dataframe_mapper.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tabular/datasets/Bike_Sharing.csv` & `hypernets-0.3.0/hypernets/tabular/datasets/Bike_Sharing.csv`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tabular/datasets/adult-uci.csv.gz` & `hypernets-0.3.0/hypernets/tabular/datasets/adult-uci.csv.gz`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tabular/datasets/bank-uci.csv.gz` & `hypernets-0.3.0/hypernets/tabular/datasets/bank-uci.csv.gz`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tabular/datasets/blood.csv` & `hypernets-0.3.0/hypernets/tabular/datasets/blood.csv`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tabular/datasets/dsutils.py` & `hypernets-0.3.0/hypernets/tabular/datasets/dsutils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # -*- coding:utf-8 -*-
 import os
 
 basedir = os.path.dirname(__file__)
 
 
 def load_boston():
-    from sklearn import datasets
     import pandas as pd
-    boston_dataset = datasets.load_boston()
-    data = pd.DataFrame(boston_dataset.data)
-    data.columns = boston_dataset.feature_names
-    data.insert(0, 'target', boston_dataset.target)
+    from sklearn import datasets
+    # boston_dataset = datasets.load_boston()
+    # data = pd.DataFrame(boston_dataset.data)
+    # data.columns = boston_dataset.feature_names
+    # data.insert(0, 'target', boston_dataset.target)
+    data = pd.read_csv(f'{basedir}/boston.csv.gz', compression='gzip')
     return data
 
 
 def load_heart_disease_uci():
     import pandas as pd
     data = pd.read_csv(f'{basedir}/heart-disease-uci.csv')
     return data
```

### Comparing `hypernets-0.2.5.7/hypernets/tabular/datasets/glass_uci.csv` & `hypernets-0.3.0/hypernets/tabular/datasets/glass_uci.csv`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tabular/datasets/heart-disease-uci.csv` & `hypernets-0.3.0/hypernets/tabular/datasets/heart-disease-uci.csv`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tabular/datasets/movielens_sample.txt` & `hypernets-0.3.0/hypernets/tabular/datasets/movielens_sample.txt`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tabular/datasets/telescope.csv` & `hypernets-0.3.0/hypernets/tabular/datasets/telescope.csv`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tabular/drift_detection.py` & `hypernets-0.3.0/hypernets/tabular/drift_detection.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tabular/ensemble/base_ensemble.py` & `hypernets-0.3.0/hypernets/tabular/ensemble/base_ensemble.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,21 @@
         self.random_state = random_state
         self.classes_ = None
         for est in estimators:
             if est is not None and self.classes_ is None and hasattr(est, 'classes_'):
                 self.classes_ = est.classes_
                 break
 
+    @property
+    def _estimator_type(self):
+        for est in self.estimators:
+            if est is not None:
+                return est._estimator_type
+        return None
+
     def _estimator_predict(self, estimator, X):
         if self.task == 'regression':
             pred = estimator.predict(X)
         else:
             # if self.classes_ is None and hasattr(estimator, 'classes_'):
             #     self.classes_ = estimator.classes_
             assert self.classes_ is not None
```

### Comparing `hypernets-0.2.5.7/hypernets/tabular/ensemble/stacking.py` & `hypernets-0.3.0/hypernets/tabular/ensemble/stacking.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tabular/ensemble/voting.py` & `hypernets-0.3.0/hypernets/tabular/ensemble/voting.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tabular/estimator_detector.py` & `hypernets-0.3.0/hypernets/tabular/estimator_detector.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tabular/evaluator/_base.py` & `hypernets-0.3.0/hypernets/tabular/evaluator/_base.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tabular/evaluator/auto_sklearn.py` & `hypernets-0.3.0/hypernets/tabular/evaluator/auto_sklearn.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tabular/evaluator/h2o.py` & `hypernets-0.3.0/hypernets/tabular/evaluator/h2o.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tabular/evaluator/hyperdt.py` & `hypernets-0.3.0/hypernets/tabular/evaluator/hyperdt.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tabular/evaluator/hypergbm.py` & `hypernets-0.3.0/hypernets/tabular/evaluator/hypergbm.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tabular/evaluator/tests.py` & `hypernets-0.3.0/hypernets/tabular/evaluator/tests.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tabular/evaluator/tpot.py` & `hypernets-0.3.0/hypernets/tabular/evaluator/tpot.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tabular/feature_generators/_primitives.py` & `hypernets-0.3.0/hypernets/tabular/feature_generators/_primitives.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 # coding: UTF-8
 """
 
 """
 from functools import partial
 
+import featuretools as ft
 import numpy as np
+import pandas as pd
 from featuretools.primitives import Haversine, TransformPrimitive
 from featuretools.utils.gen_utils import Library
 from sklearn.pipeline import make_pipeline
 
 from hypernets.tabular.cfg import TabularCfg as cfg
+from hypernets.utils import Version
 from . import _base
 
 try:
     import geohash
 
     is_geohash_installed = True
 except ImportError:
     is_geohash_installed = False
 
+_TO_DASK_SERIES = Version(ft.__version__) >= Version('1.20')
+
 
 class DaskCompatibleTransformPrimitive(TransformPrimitive):
     compatibility = [Library.PANDAS, Library.DASK]
     return_dtype = 'object'
     commutative = True
 
     def get_function(self):
@@ -44,15 +49,20 @@
         return self.fn_pd(x1, *args)
 
     def fn_pd(self, x1, *args):
         raise NotImplementedError()
 
     def fn_dask_part(self, part):
         arrs = [part.iloc[:, i] for i in range(len(part.columns))]
-        return self.fn_pd(*arrs)
+        result = self.fn_pd(*arrs)
+
+        if _TO_DASK_SERIES and isinstance(result, np.ndarray):
+            result = pd.Series(result)
+
+        return result
 
 
 class CrossCategorical(DaskCompatibleTransformPrimitive):
     name = "cross_categorical"
     input_types = [_base.ColumnSchema(logical_type=_base.Categorical),
                    _base.ColumnSchema(logical_type=_base.Categorical)]
     return_type = _base.ColumnSchema(logical_type=_base.Categorical, semantic_tags={'category'})
@@ -133,13 +143,21 @@
             encoder = make_pipeline(tfs['LocalizedTfidfVectorizer'](max_features=self.tfidf_max_features),
                                     tfs['TruncatedSVD'](n_components=self.number_output_features))
             xt = encoder.fit_transform(x1)
             self.encoder_ = encoder
         else:
             xt = self.encoder_.transform(x1)
 
+        if _TO_DASK_SERIES:
+            from hypernets.tabular import is_dask_installed
+            if is_dask_installed:
+                from hypernets.tabular.dask_ex import DaskToolBox
+                if DaskToolBox.is_dask_array(xt):
+                    xt = DaskToolBox.to_dask_frame_or_series(xt)
+                    xt = DaskToolBox.make_divisions_known(xt)
+
         if hasattr(xt, 'iloc'):
             result = [xt.iloc[:, i] for i in range(xt.shape[1])]
         else:
             result = [xt[:, i] for i in range(xt.shape[1])]
 
         return result
```

### Comparing `hypernets-0.2.5.7/hypernets/tabular/feature_generators/_transformers.py` & `hypernets-0.3.0/hypernets/tabular/feature_generators/_transformers.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tabular/lifelong_learning/_split.py` & `hypernets-0.3.0/hypernets/tabular/lifelong_learning/_split.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tabular/metrics.py` & `hypernets-0.3.0/hypernets/tabular/metrics.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tabular/persistence.py` & `hypernets-0.3.0/hypernets/tabular/persistence.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tabular/pseudo_labeling.py` & `hypernets-0.3.0/hypernets/tabular/pseudo_labeling.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tabular/sklearn_ex.py` & `hypernets-0.3.0/hypernets/tabular/sklearn_ex.py`

 * *Files 6% similar despite different names*

```diff
@@ -189,15 +189,15 @@
         assert len(X.shape) == 2
         assert isinstance(X, pd.DataFrame) or self.columns is None
 
         if isinstance(X, pd.DataFrame):
             if self.columns is None:
                 self.columns = X.columns.tolist()
             for col in self.columns:
-                data = X.loc[:, col]
+                data = X[col]
                 if data.dtype == 'object':
                     data = data.astype('str')
                     # print(f'Column "{col}" has been convert to "str" type.')
                 le = SafeLabelEncoder()
                 le.fit(data)
                 self.encoders[col] = le
         else:
@@ -212,21 +212,21 @@
 
     def transform(self, X):
         assert len(X.shape) == 2
         assert isinstance(X, pd.DataFrame) or self.columns is None
 
         if self.columns is not None:  # dataframe
             for col in self.columns:
-                data = X.loc[:, col]
+                data = X[col]
                 if data.dtype == 'object':
                     data = data.astype('str')
                 data_t = self.encoders[col].transform(data)
                 if self.dtype:
                     data_t = data_t.astype(self.dtype)
-                X.loc[:, col] = data_t
+                X[col] = data_t
         else:
             n_features = X.shape[1]
             assert n_features == len(self.encoders.items())
             for n in range(n_features):
                 X[:, n] = self.encoders[n].transform(X[:, n])
             if self.dtype:
                 X = X.astype(self.dtype)
@@ -237,23 +237,23 @@
         assert len(X.shape) == 2
         assert isinstance(X, pd.DataFrame) or self.columns is None
 
         if isinstance(X, pd.DataFrame):
             if self.columns is None:
                 self.columns = X.columns.tolist()
             for col in self.columns:
-                data = X.loc[:, col]
+                data = X[col]
                 if data.dtype == 'object':
                     data = data.astype('str')
                     # print(f'Column "{col}" has been convert to "str" type.')
                 le = SafeLabelEncoder()
                 data_t = le.fit_transform(data)
                 if self.dtype:
                     data_t = data_t.astype(self.dtype)
-                X.loc[:, col] = data_t
+                X[col] = data_t
                 self.encoders[col] = le
         else:
             n_features = X.shape[1]
             for n in range(n_features):
                 data = X[:, n]
                 le = SafeLabelEncoder()
                 X[:, n] = le.fit_transform(data)
@@ -722,16 +722,16 @@
 
     def fit(self, X, y=None):
         self.new_columns = []
         if self.columns is None:
             self.columns = X.columns.tolist()
         for col in self.columns:
             new_name = col + const.COLUMNNAME_POSTFIX_DISCRETE
-            n_unique = X.loc[:, col].nunique()
-            n_null = X.loc[:, col].isnull().sum()
+            n_unique = X[col].nunique()
+            # n_null = X[col].isnull().sum()
             c_bins = self.bins
             if c_bins is None or c_bins <= 0:
                 c_bins = round(n_unique ** 0.25) + 1
             encoder = KBinsDiscretizer(n_bins=c_bins, encode='ordinal', strategy=self.strategy)
             self.new_columns.append((col, new_name, encoder.n_bins))
             encoder.fit(X[[col]])
             self.encoders[col] = encoder
@@ -1126,15 +1126,18 @@
         assert getattr(Xc, 'dt', None) is not None
         dfs = []
 
         for k, c in self.extract_.items():
             if c is None:
                 c = k
             if isinstance(c, str):
-                t = getattr(Xc.dt, c)
+                if hasattr(Xc.dt, c):
+                    t = getattr(Xc.dt, c)
+                else:
+                    continue
             else:
                 t = c(Xc)
             t.name = f'{Xc.name}_{k}'
             dfs.append(t)
 
         if self.drop_constants and len(Xc) > 1:
             dfs = [t for t in dfs if t.nunique() > 1]
@@ -1572,7 +1575,42 @@
     def fit_transform(self, X, y=None, **kwargs):
         assert y is not None
 
         if str(y.dtype) == 'object':
             le = self.label_encoder_cls()
             y = le.fit_transform(y)
         return super().fit_transform(X, y, **kwargs)
+
+
+@tb_transformer(pd.DataFrame)
+class FeatureImportanceSelection(BaseEstimator):
+
+    def __init__(self, importances, quantile, min_features=3):
+        super(FeatureImportanceSelection, self).__init__()
+        self.quantile = quantile
+        self.importances = importances
+        self.min_features = min_features
+
+        n_features = int(round(len(self.importances) * (1 - self.quantile), 0))
+        if n_features < min_features:
+            n_features = min_features
+        imps = [_[1] for _ in importances]
+        self._important_features = [self.importances[i] for i in np.argsort(-np.array(imps))[: n_features]]
+
+    def feature_usage(self):
+        return len(self.important_features) / len(self.importances)
+
+    def fit(self, X, y=None, **kwargs):
+        return self
+
+    def fit_transform(self, X, y=None, **kwargs):
+        self.fit(X, y, **kwargs)
+        return self.transform(X)
+
+    def transform(self, X):
+        important_feature_names = [_[0] for _ in self.important_features]
+        reversed_features = list(filter(lambda f: f in important_feature_names, X.columns.values))
+        return X[reversed_features]
+
+    @property
+    def important_features(self):
+        return self._important_features
```

### Comparing `hypernets-0.2.5.7/hypernets/tabular/toolbox.py` & `hypernets-0.3.0/hypernets/tabular/toolbox.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 from . import estimator_detector as estimator_detector_
 from . import feature_generators as feature_generators_
 from . import metrics as metrics_
 from . import pseudo_labeling as pseudo_labeling_
 from . import sklearn_ex as sk_ex  # NOQA,  register customized transformer
 from ._base import ToolboxMeta, register_transformer
 from .cfg import TabularCfg as c
-from .persistence import ParquetPersistence
 
 try:
     import lightgbm
 
     lightgbm_installed = True
 except ImportError:
     lightgbm_installed = False
@@ -150,14 +149,15 @@
         if reset_index:
             df.reset_index(drop=True, inplace=True)
 
         return df
 
     @staticmethod
     def parquet():
+        from .persistence import ParquetPersistence
         return ParquetPersistence()
 
     @staticmethod
     def unique(y):
         if hasattr(y, 'unique'):
             uniques = set(y.unique())
         else:
@@ -720,16 +720,19 @@
     # GaussRankScaler=sk_ex.GaussRankScaler,
     # VarLenFeatureEncoder=sk_ex.VarLenFeatureEncoder,
     # MultiVarLenFeatureEncoder=sk_ex.MultiVarLenFeatureEncoder,
     # LocalizedTfidfVectorizer=sk_ex.LocalizedTfidfVectorizer,
     # TfidfEncoder=sk_ex.TfidfEncoder,
     # DatetimeEncoder=sk_ex.DatetimeEncoder,
 
-    FeatureGenerationTransformer=feature_generators_.FeatureGenerationTransformer,
+    # FeatureGenerationTransformer=feature_generators_.FeatureGenerationTransformer,
 )
 
+if feature_generators_.is_feature_generator_ready:
+    _predefined_transformers['FeatureGenerationTransformer'] = feature_generators_.FeatureGenerationTransformer
+
 for name, tf in _predefined_transformers.items():
     register_transformer(tf, name=name, dtypes=pd.DataFrame)
 
 __all__ = [
     ToolBox.__name__,
 ]
```

### Comparing `hypernets-0.2.5.7/hypernets/tests/core/callback_test.py` & `hypernets-0.3.0/hypernets/tests/core/callback_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,43 +7,63 @@
 from hypernets.core.callbacks import EarlyStoppingCallback, EarlyStoppingError
 import pytest
 
 
 class Test_Callback:
     def test_early_stopping(self):
         es = EarlyStoppingCallback(3, 'min')
-        es.on_trial_end(None, None, 1, 0.9, True, 0)
-        es.on_trial_end(None, None, 2, 0.9, True, 0)
-        es.on_trial_end(None, None, 3, 0.9, True, 0)
+        es.on_trial_end(None, None, 1, [0.9], True, 0)
+        es.on_trial_end(None, None, 2, [0.9], True, 0)
+        es.on_trial_end(None, None, 3, [0.9], True, 0)
 
         with pytest.raises(EarlyStoppingError) as ese:
-            es.on_trial_end(None, None, 4, 0.9, True, 0)
+            es.on_trial_end(None, None, 4, [0.9], True, 0)
         assert ese.value.args[0].find('reason: max_no_improvement_trials') > -0
 
         es = EarlyStoppingCallback(3, 'min')
-        es.on_trial_end(None, None, 1, 0.9, True, 0)
-        es.on_trial_end(None, None, 2, 0.8, True, 0)
-        es.on_trial_end(None, None, 3, 0.8, True, 0)
-        es.on_trial_end(None, None, 4, 0.8, True, 0)
+        es.on_trial_end(None, None, 1, [0.9], True, 0)
+        es.on_trial_end(None, None, 2, [0.8], True, 0)
+        es.on_trial_end(None, None, 3, [0.8], True, 0)
+        es.on_trial_end(None, None, 4, [0.8], True, 0)
 
         with pytest.raises(EarlyStoppingError) as ese:
-            es.on_trial_end(None, None, 5, 0.8, True, 0)
+            es.on_trial_end(None, None, 5, [0.8], True, 0)
         assert ese.value.args[0].find('reason: max_no_improvement_trials') > -0
 
         es = EarlyStoppingCallback(3, 'max')
-        es.on_trial_end(None, None, 1, 0.9, True, 0)
-        es.on_trial_end(None, None, 2, 0.9, True, 0)
-        es.on_trial_end(None, None, 3, 0.9, True, 0)
+        es.on_trial_end(None, None, 1, [0.9], True, 0)
+        es.on_trial_end(None, None, 2, [0.9], True, 0)
+        es.on_trial_end(None, None, 3, [0.9], True, 0)
 
         with pytest.raises(EarlyStoppingError) as ese:
-            es.on_trial_end(None, None, 4, 0.9, True, 0)
+            es.on_trial_end(None, None, 4, [0.9], True, 0)
         assert ese.value.args[0].find('reason: max_no_improvement_trials') > -0
 
         es = EarlyStoppingCallback(3, 'max')
-        es.on_trial_end(None, None, 1, 0.9, True, 0)
-        es.on_trial_end(None, None, 2, 0.91, True, 0)
-        es.on_trial_end(None, None, 3, 0.91, True, 0)
-        es.on_trial_end(None, None, 4, 0.91, True, 0)
+        es.on_trial_end(None, None, 1, [0.9], True, 0)
+        es.on_trial_end(None, None, 2, [0.91], True, 0)
+        es.on_trial_end(None, None, 3, [0.91], True, 0)
+        es.on_trial_end(None, None, 4, [0.91], True, 0)
 
         with pytest.raises(EarlyStoppingError) as ese:
-            es.on_trial_end(None, None, 5, 0.91, True, 0)
+            es.on_trial_end(None, None, 5, [0.91], True, 0)
         assert ese.value.args[0].find('reason: max_no_improvement_trials') > -0
+
+#    def test_early_stopping_by_pareto(self):
+#
+#        es = EarlyStoppingCallback(3, 'min')
+#        es.on_trial_end(None, None, 1, [0.9, 0.9], True, 0)
+#        es.on_trial_end(None, None, 2, [0.95, 0.8], True, 0)
+#        es.on_trial_end(None, None, 3, [0.95, 0.7], True, 0)
+#
+#        with pytest.raises(EarlyStoppingError) as ese:
+#            es.on_trial_end(None, None, 4, [0.9, 0.9], True, 0)
+#        assert ese.value.args[0].find('reason: max_no_improvement_trials') > -0
+#
+#        es = EarlyStoppingCallback(3, 'max')
+#        es.on_trial_end(None, None, 1, [0.9, 0.9], True, 0)
+#        es.on_trial_end(None, None, 2, [0.8, 0.95], True, 0)
+#        es.on_trial_end(None, None, 3, [0.9, 0.9], True, 0)
+#
+#        with pytest.raises(EarlyStoppingError) as ese:
+#            es.on_trial_end(None, None, 4, [0.9, 0.9], True, 0)
+#        assert ese.value.args[0].find('reason: max_no_improvement_trials') > -0
```

### Comparing `hypernets-0.2.5.7/hypernets/tests/core/connection_space_test.py` & `hypernets-0.3.0/hypernets/tests/core/connection_space_test.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tests/core/hyper_space_test.py` & `hypernets-0.3.0/hypernets/tests/core/hyper_space_test.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tests/core/mutable_test.py` & `hypernets-0.3.0/hypernets/tests/core/mutable_test.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tests/core/parameter_test.py` & `hypernets-0.3.0/hypernets/tests/core/parameter_test.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tests/discriminators/__init__.py` & `hypernets-0.3.0/hypernets/tests/discriminators/__init__.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tests/discriminators/base_test.py` & `hypernets-0.3.0/hypernets/tests/discriminators/base_test.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tests/discriminators/percentile.py` & `hypernets-0.3.0/hypernets/tests/discriminators/percentile.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tests/dispatchers/process_test.py` & `hypernets-0.3.0/hypernets/tests/dispatchers/process_test.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tests/experiment/experiment_factory.py` & `hypernets-0.3.0/hypernets/tests/experiment/experiment_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from hypernets.experiment import make_experiment
 from hypernets.tabular.datasets import dsutils
 from hypernets.tabular.sklearn_ex import MultiLabelEncoder
 from hypernets.utils import const
 
 
 def _create_experiment(predefined_kwargs, maker=None, need_test=False, user_kwargs=None):
-    df = dsutils.load_boston()
+    df = dsutils.load_boston().head(1000)
     df['Constant'] = [0 for i in range(df.shape[0])]
     df['Id'] = [i for i in range(df.shape[0])]
     target = 'target'
     df_train, df_test = train_test_split(df, test_size=0.2, random_state=1234)
     df_test.pop(target)
     df_train['Drifted'] = np.random.random(df_train.shape[0])
     df_test['Drifted'] = np.random.random(df_test.shape[0]) * 100
```

### Comparing `hypernets-0.2.5.7/hypernets/tests/experiment/extractor_test.py` & `hypernets-0.3.0/hypernets/tests/experiment/extractor_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from hypernets.tests.experiment import experiment_factory
 from hypernets.experiment.compete import DataCleanStep, DriftDetectStep
 from hypernets.experiment import ExperimentExtractor, StepMeta
-import time
+import pytest
+from hypernets.tabular.feature_generators import is_feature_generator_ready
 
 
 def _run_experiment(creator):
     exp = creator()
     estimator = exp.run(max_trials=3)
     experiment_data = ExperimentExtractor(exp).extract()
     assert estimator is not None
@@ -69,14 +70,15 @@
     print(multicollinearity_detect_step)
     unselected_features = multicollinearity_detect_step.extension['unselected_features']
     assert len(unselected_features.keys()) > 0
     assert "INDUS" in unselected_features
     assert unselected_features['INDUS']['reserved'] == 'CRIM'
 
 
+@pytest.mark.skipif(not is_feature_generator_ready, reason='feature_generator is not ready')
 def test_feature_generation_extractor():
     exp_data, estimator = _run_experiment(experiment_factory.create_feature_generation_experiment)
     fg_step = exp_data.steps[2]
 
     output_features = fg_step.extension['outputFeatures']
     assert len(output_features) > 0
```

### Comparing `hypernets-0.2.5.7/hypernets/tests/experiment/general_experiment_test.py` & `hypernets-0.3.0/hypernets/tests/experiment/general_experiment_test.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tests/experiment/job_test.py` & `hypernets-0.3.0/hypernets/tests/experiment/job_test.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,14 +5,22 @@
 
 from hypernets.examples.plain_model import PlainModel, PlainSearchSpace
 from hypernets.experiment import CompeteExperiment
 from hypernets.experiment.job import ExperimentJobCreator, CompeteExperimentJobCreator
 from hypernets.tabular.datasets import dsutils
 from hypernets.utils import const, common as common_util
 
+try:
+    from pandas.io.parquet import get_engine
+
+    get_engine('auto')
+    is_pd_parquet_ready = True
+except:
+    is_pd_parquet_ready = False
+
 
 class BloodDatasetJobEngine(CompeteExperimentJobCreator):
 
     def _create_experiment(self, make_options):
         from hypernets.experiment import make_experiment
         train_data = dsutils.load_blood()
         experiment = make_experiment(PlainModel, train_data, **make_options)
@@ -23,14 +31,15 @@
 
     def test_read_txt_file(self):
         from hypernets.tabular.datasets.dsutils import basedir
         with pytest.raises(ValueError):
             txt_file = f'{basedir}/movielens_sample.txt'
             ExperimentJobCreator._read_file(txt_file)
 
+    @pytest.mark.skipif(not is_pd_parquet_ready, reason='pandas parquet engine is not ready')
     def test_read_supported_file(self):
         from hypernets.tabular.datasets.dsutils import basedir
         csv_file = f'{basedir}/heart-disease-uci.csv'
         df_csv = ExperimentJobCreator._read_file(csv_file)
         assert df_csv.shape[0] > 1
 
         file_path = common_util.get_temp_file_path(prefix="heart-disease-uci", suffix=".parquet")
```

### Comparing `hypernets-0.2.5.7/hypernets/tests/experiment/report_test.py` & `hypernets-0.3.0/hypernets/tests/experiment/report_test.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tests/experiment/run_export_experiment_report.py` & `hypernets-0.3.0/hypernets/tests/experiment/run_export_experiment_report.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tests/hyperctl/batch_factory.py` & `hypernets-0.3.0/hypernets/tests/hyperctl/batch_factory.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tests/hyperctl/test_application.py` & `hypernets-0.3.0/hypernets/tests/hyperctl/test_application.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tests/hyperctl/test_batch.py` & `hypernets-0.3.0/hypernets/tests/hyperctl/test_batch.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tests/hyperctl/test_cli.py` & `hypernets-0.3.0/hypernets/tests/hyperctl/test_cli.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tests/hyperctl/test_scheduler.py` & `hypernets-0.3.0/hypernets/tests/hyperctl/test_scheduler.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,18 +200,18 @@
         app.start()
         batch = app.batch
         assert_batch_finished(batch, _ShellJob.STATUS_SUCCEED)
         assert_local_job_succeed(batch.jobs)
 
 
 @skip_if_windows
-class TestLocaBatch(BaseBatchAppTest):
+class TestLocalBatch(BaseBatchAppTest):
     @classmethod
     def setup_class(cls):
-        super(TestLocaBatch, cls).setup_class()
+        super(TestLocalBatch, cls).setup_class()
         batch = create_local_batch()
         app = BatchApplication(batch, server_port=8082,
                                scheduler_exit_on_finish=True,
                                scheduler_interval=1000)
         cls.app = app
 
     def test_run_batch(self):
```

### Comparing `hypernets-0.2.5.7/hypernets/tests/model/plain_model_test.py` & `hypernets-0.3.0/hypernets/tests/model/plain_model_test.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tests/pipeline/pipeline_test.py` & `hypernets-0.3.0/hypernets/tests/pipeline/pipeline_test.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tests/searchers/evolution_test.py` & `hypernets-0.3.0/hypernets/tests/searchers/evolution_test.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tests/searchers/grid_test.py` & `hypernets-0.3.0/hypernets/tests/searchers/grid_test.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tests/searchers/mcts_test.py` & `hypernets-0.3.0/hypernets/tests/searchers/mcts_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     def test_mcts_searcher(self):
         searcher = MCTSSearcher(self.get_space, max_node_space=10)
 
         for i in range(1000):
             space_sample = searcher.sample()
             assert space_sample.all_assigned == True
             print(space_sample.params_summary())
-            searcher.update_result(space_sample, np.random.uniform(0.1, 0.9))
+            searcher.update_result(space_sample, [np.random.uniform(0.1, 0.9)])
 
         assert searcher.tree.root.visits == 1000
         assert len(searcher.nodes_map.items()) == 1000
 
     def test_mcts_searcher_parallelize(self):
         searcher = MCTSSearcher(self.get_space, max_node_space=10)
         history = TrialHistory(OptimizeDirection.Maximize)
@@ -95,30 +95,30 @@
             space_sample = searcher.sample()
             running_samples.append(space_sample)
         assert searcher.tree.root.visits == 10
         for sample in running_samples:
             reward = np.random.uniform(0.1, 0.9)
             trial = Trial(sample, trial_no, reward, 10)
             history.append(trial)
-            searcher.update_result(sample, reward)
+            searcher.update_result(sample, [reward])
             trial_no += 1
 
         assert searcher.tree.root.visits == 10
         assert len(searcher.nodes_map.items()) == 10
         running_samples = []
         for i in range(10):
             space_sample = searcher.sample()
             running_samples.append(space_sample)
         assert searcher.tree.root.visits == 20
 
         for sample in running_samples:
             reward = np.random.uniform(0.1, 0.9)
             trial = Trial(sample, trial_no, reward, 10)
             history.append(trial)
-            searcher.update_result(sample, reward)
+            searcher.update_result(sample, [reward])
 
         assert searcher.tree.root.visits == 20
 
     def test_set_random_state(self):
         from hypernets.core import set_random_state
         set_random_state(9527)
```

### Comparing `hypernets-0.2.5.7/hypernets/tests/searchers/playback_test.py` & `hypernets-0.3.0/hypernets/tests/searchers/playback_test.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tests/searchers/random_test.py` & `hypernets-0.3.0/hypernets/tests/searchers/random_test.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tests/tabular/cache_test.py` & `hypernets-0.3.0/hypernets/tests/tabular/cache_test.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tests/tabular/column_selector_test.py` & `hypernets-0.3.0/hypernets/tests/tabular/column_selector_test.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tests/tabular/data_cleaner_test.py` & `hypernets-0.3.0/hypernets/tests/tabular/data_cleaner_test.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tests/tabular/drift_detection_test.py` & `hypernets-0.3.0/hypernets/tests/tabular/drift_detection_test.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tests/tabular/ensemble/ensemble_test.py` & `hypernets-0.3.0/hypernets/tests/tabular/ensemble/ensemble_test.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tests/tabular/feature_generator_test.py` & `hypernets-0.3.0/hypernets/tests/tabular/feature_generator_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # -*- coding:utf-8 -*-
 """
 
 """
 import math
 from datetime import datetime
 
-import featuretools as ft
 import numpy as np
 import pandas as pd
 import pytest
 from sklearn.impute import SimpleImputer
 from sklearn.model_selection import train_test_split
 from sklearn.pipeline import Pipeline
 from sklearn.preprocessing import OrdinalEncoder, StandardScaler
 
 from hypernets.tabular.column_selector import column_object_category_bool, column_number_exclude_timedelta
 from hypernets.tabular.dataframe_mapper import DataFrameMapper
 from hypernets.tabular.datasets import dsutils
-from hypernets.tabular.feature_generators import FeatureGenerationTransformer, is_geohash_installed
+from hypernets.tabular.feature_generators import FeatureGenerationTransformer, is_geohash_installed, \
+    is_feature_generator_ready
 from hypernets.tabular.sklearn_ex import FeatureSelectionTransformer
 from hypernets.utils import logging
 
 if_geohash_ready = pytest.mark.skipif(not is_geohash_installed, reason='python-geohash is not installed')
 
 logger = logging.getLogger(__name__)
 
@@ -34,22 +34,24 @@
     preprocessor = DataFrameMapper(features=[(column_object_category_bool, cat_transformer),
                                              (column_number_exclude_timedelta, num_transformer)],
                                    input_df=True,
                                    df_out=True)
     return preprocessor
 
 
+@pytest.mark.skipif(not is_feature_generator_ready, reason='feature_generator is not ready')
 class Test_FeatureGenerator():
     def test_char_add(self):
         x1 = ['1', '2']
         x2 = ['c', 'd']
         x3 = np.char.add(x1, x2)
         assert list(x3) == ['1c', '2d']
 
     def test_ft_primitives(self):
+        import featuretools as ft
         tps = ft.primitives.get_transform_primitives()
         assert tps
 
     def test_pipeline(self):
         df = dsutils.load_bank()
         df.drop(['id'], axis=1, inplace=True)
         X_train, X_test = train_test_split(df.head(100), test_size=0.2, random_state=42)
```

### Comparing `hypernets-0.2.5.7/hypernets/tests/tabular/feature_importance_test.py` & `hypernets-0.3.0/hypernets/tests/tabular/feature_importance_test.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tests/tabular/lifelong_learning/split_test.py` & `hypernets-0.3.0/hypernets/tests/tabular/lifelong_learning/split_test.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tests/tabular/persitence_test.py` & `hypernets-0.3.0/hypernets/tests/tabular/persitence_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 import os
 from os import path
 
 import numpy as np
 import pandas as pd
+import pytest
 
 from hypernets.tabular.datasets import dsutils
-from hypernets.tabular.persistence import ParquetPersistence
 from hypernets.tests import test_output_dir
 from hypernets.utils import fs
 
-p = ParquetPersistence()
+try:
+    from hypernets.tabular.persistence import ParquetPersistence
 
+    p = ParquetPersistence()
+    is_parquet_persitence_ready = True
+except:
+    is_parquet_persitence_ready = False
 
+
+@pytest.mark.skipif(not is_parquet_persitence_ready, reason='ParquetPersistence is not installed')
 class TestPersistence:
     @classmethod
     def setup_class(cls):
         os.makedirs(f'{test_output_dir}/{cls.__name__}')
         fs.mkdirs(f'/{cls.__name__}', exist_ok=True)
 
     @classmethod
```

### Comparing `hypernets-0.2.5.7/hypernets/tests/tabular/psudo_labeling_test.py` & `hypernets-0.3.0/hypernets/tests/tabular/psudo_labeling_test.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tests/tabular/sklearn_transformer_test.py` & `hypernets-0.3.0/hypernets/tests/tabular/sklearn_transformer_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,16 +80,17 @@
              (column_number_exclude_timedelta, PolynomialFeatures(2)),
              ], input_df=True, df_out=True
         )
         x_new = dfm.fit_transform(X, y)
         # assert x_new.columns.to_list() == ['b_c_d_l_0', 'b_c_d_l_1', 'a_a', 'a_b', 'a_missing_value', 'e_False',
         #                                    'e_True', 'f_c', 'f_d', 'f_missing_value', '1', 'b', 'c', 'd', 'l',
         #                                    'b^2', 'b c', 'b d', 'b l', 'c^2', 'c d', 'c l', 'd^2', 'd l', 'l^2']
-        assert x_new.columns.to_list() == ['b_c_d_l_0', 'b_c_d_l_1', 'a_a', 'a_b', 'a_missing_value', 'e_False',
-                                           'e_True', 'f_c', 'f_d', 'f_missing_value']
+        # assert x_new.columns.to_list() == ['b_c_d_l_0', 'b_c_d_l_1', 'a_a', 'a_b', 'a_missing_value', 'e_False',
+        #                                    'e_True', 'f_c', 'f_d', 'f_missing_value']
+        assert {'b_c_d_l_0', 'b_c_d_l_1'}.issubset(set(x_new.columns.to_list()))
 
     def test_no_feature(self):
         df = get_df()[0]
         dfm = DataFrameMapper(
             [([], preprocessing.LabelEncoder())],
             input_df=True,
             df_out=True)
```

### Comparing `hypernets-0.2.5.7/hypernets/tests/tabular/tb_cuml/cache_test.py` & `hypernets-0.3.0/hypernets/tests/tabular/tb_cuml/cache_test.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tests/tabular/tb_cuml/data_split_test.py` & `hypernets-0.3.0/hypernets/tests/tabular/tb_cuml/data_split_test.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tests/tabular/tb_cuml/drift_detection_test.py` & `hypernets-0.3.0/hypernets/tests/tabular/tb_cuml/drift_detection_test.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tests/tabular/tb_cuml/estimator_test.py` & `hypernets-0.3.0/hypernets/tests/tabular/tb_cuml/estimator_test.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tests/tabular/tb_cuml/experiment_test.py` & `hypernets-0.3.0/hypernets/tests/tabular/tb_cuml/experiment_test.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tests/tabular/tb_cuml/toolbox_test.py` & `hypernets-0.3.0/hypernets/tests/tabular/tb_cuml/toolbox_test.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tests/tabular/tb_cuml/transformer_test.py` & `hypernets-0.3.0/hypernets/tests/tabular/tb_cuml/transformer_test.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tests/tabular/tb_dask/__init__.py` & `hypernets-0.3.0/hypernets/tests/tabular/tb_dask/__init__.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tests/tabular/tb_dask/cache_test.py` & `hypernets-0.3.0/hypernets/tests/tabular/tb_dask/cache_test.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tests/tabular/tb_dask/dask_ex_test.py` & `hypernets-0.3.0/hypernets/tests/tabular/tb_dask/dask_ex_test.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tests/tabular/tb_dask/dask_transofromer_test.py` & `hypernets-0.3.0/hypernets/tests/tabular/tb_dask/dask_transofromer_test.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tests/tabular/tb_dask/drift_detection_test.py` & `hypernets-0.3.0/hypernets/tests/tabular/tb_dask/drift_detection_test.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tests/tabular/tb_dask/feature_generator_dask_test.py` & `hypernets-0.3.0/hypernets/tests/tabular/tb_dask/feature_generator_dask_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,27 +7,28 @@
 
 import pandas as pd
 import pytest
 from sklearn.pipeline import Pipeline
 
 from hypernets.tabular import get_tool_box
 from hypernets.tabular.datasets import dsutils
-from hypernets.tabular.feature_generators import is_geohash_installed
+from hypernets.tabular.feature_generators import is_geohash_installed, is_feature_generator_ready
 from hypernets.utils import logging
 from . import if_dask_ready, is_dask_installed, setup_dask
 
 if is_dask_installed:
     import dask.dataframe as dd
 
 if_geohash_ready = pytest.mark.skipif(not is_geohash_installed, reason='python-geohash is not installed')
 
 logger = logging.getLogger(__name__)
 
 
 @if_dask_ready
+@pytest.mark.skipif(not is_feature_generator_ready, reason='feature_generator is not ready')
 class TestFeatureGeneratorWithDask:
     @classmethod
     def setup_class(cls):
         setup_dask(cls)
 
     def test_pipeline(self):
         df = dsutils.load_bank()
```

### Comparing `hypernets-0.2.5.7/hypernets/tests/tabular/tb_dask/persitence_test.py` & `hypernets-0.3.0/hypernets/tests/tabular/tb_dask/persitence_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 import glob
 import os
 
+import pytest
+
 from hypernets.tabular.datasets import dsutils
 from hypernets.tests import test_output_dir
 from hypernets.utils import fs
 from . import if_dask_ready, is_dask_installed, setup_dask
 
+is_parquet_ready = False
 if is_dask_installed:
     import dask.dataframe as dd
     import dask.array as da
     from hypernets.tabular.dask_ex import DaskToolBox
 
-    p = DaskToolBox.parquet()
+    try:
+        p = DaskToolBox.parquet()
+        is_parquet_ready = True
+    except:
+        pass
 
 
+@pytest.mark.skipif(not is_parquet_ready, reason='ParquetPersistence is not installed')
 @if_dask_ready
 class TestDaskPersistence:
     @classmethod
     def setup_class(cls):
         setup_dask(cls)
         os.makedirs(f'{test_output_dir}/{cls.__name__}')
         fs.mkdirs(f'/{cls.__name__}', exist_ok=True)
```

### Comparing `hypernets-0.2.5.7/hypernets/tests/tabular/tb_dask/toolbox_test.py` & `hypernets-0.3.0/hypernets/tests/tabular/tb_dask/toolbox_test.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tests/tabular/toolbox_test.py` & `hypernets-0.3.0/hypernets/tests/tabular/toolbox_test.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tests/tabular/utils_test.py` & `hypernets-0.3.0/hypernets/tests/tabular/utils_test.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tests/trial/trial_history_test.py` & `hypernets-0.3.0/hypernets/tests/trial/trial_history_test.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tests/trial/trial_store_test.py` & `hypernets-0.3.0/hypernets/tests/trial/trial_store_test.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tests/utils/common_test.py` & `hypernets-0.3.0/hypernets/tests/utils/common_test.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tests/utils/df_utils_test.py` & `hypernets-0.3.0/hypernets/tests/utils/df_utils_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from hypernets.utils import df_utils
-from hypernets.tabular.datasets import dsutils
 import numpy as np
 from sklearn.preprocessing import LabelEncoder
 
 from hypernets.experiment import CompeteExperiment, Experiment
 from hypernets.tabular import get_tool_box
 from hypernets.tabular.datasets import dsutils
 from hypernets.tests.model.plain_model_test import create_plain_model
```

### Comparing `hypernets-0.2.5.7/hypernets/tests/utils/estimators_test.py` & `hypernets-0.3.0/hypernets/tests/utils/estimators_test.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tests/utils/ssh_utils_test.py` & `hypernets-0.3.0/hypernets/tests/utils/ssh_utils_test.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tests/utils/tic_toc_test.py` & `hypernets-0.3.0/hypernets/tests/utils/tic_toc_test.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/tests/utils/tuning_test.py` & `hypernets-0.3.0/hypernets/tests/utils/tuning_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,36 +25,36 @@
 
 
 class Test_ParamTuning():
     def test_search_params(self):
         print('start')
         history = search_params(func1, 'grid', max_trials=10, optimize_direction='max')
         best = history.get_best()
-        assert best.reward == 14.370000000000001
+        assert best.reward[0] == 14.370000000000001
         assert best.trial_no == 10
 
     def test_trigger_by_trials(self):
         from hypernets.core import EarlyStoppingCallback
         es = EarlyStoppingCallback(3, 'max',
                                    time_limit=3600,
                                    expected_reward=1)
 
         history = search_params(func_early_stopping, 'grid', max_trials=10, optimize_direction='max', callbacks=[es])
         best = history.get_best()
-        assert best.reward == 0.6
+        assert best.reward[0] == 0.6
         assert best.trial_no == 1
         assert len(history.trials) == 4
         assert es.triggered_reason == EarlyStoppingCallback.REASON_TRIAL_LIMIT
 
     def test_trigger_by_reward(self):
         from hypernets.core import EarlyStoppingCallback
         es = EarlyStoppingCallback(3, 'max',
                                    time_limit=3600,
                                    expected_reward=0.5)
 
         history = search_params(func_early_stopping, 'grid', max_trials=10, optimize_direction='max', callbacks=[es])
         best = history.get_best()
-        assert best.reward == 0.6
+        assert best.reward[0] == 0.6
         assert best.trial_no == 1
         assert len(history.trials) == 1
         assert es.triggered_reason == EarlyStoppingCallback.REASON_EXPECTED_REWARD
```

### Comparing `hypernets-0.2.5.7/hypernets/utils/__init__.py` & `hypernets-0.3.0/hypernets/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/utils/_doc_lens.py` & `hypernets-0.3.0/hypernets/utils/_doc_lens.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/utils/_estimators.py` & `hypernets-0.3.0/hypernets/utils/_estimators.py`

 * *Files identical despite different names*

```diff
@@ -44,15 +44,14 @@
         with fs.open(model_path, 'rb') as f:
             stub = pickle.load(f)
 
     return stub
 
 
 def get_tree_importances(tree_model):
-
     def catch_exception(func):
         def _wrapper(model):
             try:
                 return func(model)
             except Exception as e:
                 return False
 
@@ -75,15 +74,15 @@
 
     @catch_exception
     def is_decision_tree_model(m):
         from sklearn.tree import BaseDecisionTree
         return isinstance(m, BaseDecisionTree)
 
     def is_numpy_num_type(v):
-        for t in [np.int, np.int32, np.int64, np.float, np.float32, np.float64]:
+        for t in [int, float, np.int32, np.int64, np.float32, np.float64]:
             if isinstance(v, t) is True:
                 return True
             else:
                 continue
         return False
 
     def get_imp(n_features):
```

### Comparing `hypernets-0.2.5.7/hypernets/utils/_fsutils.py` & `hypernets-0.3.0/hypernets/utils/_fsutils.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/utils/_perf.py` & `hypernets-0.3.0/hypernets/utils/_perf.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/utils/_tic_tok.py` & `hypernets-0.3.0/hypernets/utils/_tic_tok.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/utils/common.py` & `hypernets-0.3.0/hypernets/utils/common.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets/utils/df_utils.py` & `hypernets-0.3.0/hypernets/utils/df_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-import json
-
 import numpy as np
 import pandas as pd
-from dask import dataframe as dd
 
 from hypernets.tabular import column_selector as col_se
 
 
 def get_data_character(hyper_model, X_train, y_train, X_eval=None, y_eval=None, X_test=None, task=None):
 
 	dtype2usagetype = {'object':'str', 'int64':'int', 'float64':'float', 'datetime64[ns]':'date', 'timedelta64[ns]':'date'}
@@ -66,14 +63,15 @@
 
 		if X_test is None:
 			shape_x_test = []
 		else:
 			shape_x_test = list(X_test.shape)
 
 	else:
+		from dask import dataframe as dd
 		datatype_y = dtype2usagetype[str(y_train.dtype)]
 
 		Missing_y = y_train.isnull().compute().tolist().count(True)
 		Unique_y = len(y_train.unique().compute().tolist())
 
 		if task == 'binary':	
 			Freq_y = y_train.value_counts().compute().tolist()[0]
@@ -251,9 +249,9 @@
 	elif _is_pylist(array_data):
 		return np.array(array_data)
 	elif _is_cudf_series(array_data):
 		return array_data.to_numpy()
 	elif _is_cupy_array(array_data):
 		return np.array(array_data.tolist())
 	else:
-		logger.warning(f"unseen data type {type(array_data)} convert to numpy ndarray")
+		logger.warning(f"unseen data type {type(array_data)} to convert to ndarray")
 		return array_data
```

### Comparing `hypernets-0.2.5.7/hypernets/utils/logging.py` & `hypernets-0.3.0/hypernets/utils/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,14 +137,17 @@
 
     def error(self, msg, *args, **kwargs):
         self.log(ERROR, msg, *args, **kwargs)
 
     def warning(self, msg, *args, **kwargs):
         self.log(WARN, msg, *args, **kwargs)
 
+    def warn(self, msg, *args, **kwargs):
+        self.log(WARN, msg, *args, **kwargs)
+
     def info(self, msg, *args, **kwargs):
         self.log(INFO, msg, *args, **kwargs)
 
     def debug(self, msg, *args, **kwargs):
         self.log(DEBUG, msg, *args, **kwargs)
 
     def log_if(self, level, msg, condition, *args):
@@ -189,14 +192,23 @@
 
     def is_info_enabled(self):
         return self.isEnabledFor(INFO)
 
     def is_warning_enabled(self):
         return self.isEnabledFor(WARN)
 
+    def is_enabled_for(self, level):
+        return self.isEnabledFor(level)
+
+    def isEnabledFor(self, level):
+        if self.disabled:
+            return False
+
+        return level >= self.getEffectiveLevel()
+
 
 def get_logger(name):
     original_logger_class = _logging.getLoggerClass()
     _logging.setLoggerClass(CustomizedLogger)
     logger = _logging.getLogger(name)
     _logging.setLoggerClass(original_logger_class)
```

### Comparing `hypernets-0.2.5.7/hypernets/utils/param_tuning.py` & `hypernets-0.3.0/hypernets/utils/param_tuning.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,31 +99,33 @@
             ps = space_sample.get_assigned_params()
             params = {p.alias.split('.')[-1]: p.value for p in ps}
             func_params = func_kwargs.copy()
             func_params.update(params)
 
             trial_start = time.time()
             result = func(**func_params)
-            assert isinstance(result, (float, dict))
+            assert isinstance(result, (float, dict, list))
 
             if isinstance(result, dict):
                 assert 'reward' in result.keys()
-                last_reward = result['reward']
+                last_reward = [result['reward']]
+            elif isinstance(result, float):
+                last_reward = [result]
             else:
                 last_reward = result
             searcher.update_result(space_sample, last_reward)
             elapsed = time.time() - trial_start
 
             trial = Trial(space_sample, trial_no, last_reward, elapsed)
             if isinstance(result, dict):
                 memo = result.copy()
                 memo.pop('reward')
                 trial.memo.update(memo)
 
-            if last_reward != 0:  # success
+            if last_reward[0] != 0:  # success
                 improved = history.append(trial)
                 for callback in callbacks:
                     callback.on_trial_end(None, space_sample, trial_no, trial.reward, improved, trial.elapsed)
             if logger.is_info_enabled():
                 best = history.get_best()
                 msg = f'Trial {trial_no} done, reward: {trial.reward}, ' \
                       f'best_trial_no:{best.trial_no}, best_reward:{best.reward}\n'
```

### Comparing `hypernets-0.2.5.7/hypernets/utils/ssh_utils.py` & `hypernets-0.3.0/hypernets/utils/ssh_utils.py`

 * *Files identical despite different names*

### Comparing `hypernets-0.2.5.7/hypernets.egg-info/PKG-INFO` & `hypernets-0.3.0/hypernets.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: hypernets
-Version: 0.2.5.7
+Version: 0.3.0
 Summary: An General Automated Machine Learning Framework
-Home-page: 
+Home-page: https://github.com/DataCanvasIO/Hypernets
 Author: DataCanvas Community
 Author-email: yangjian@zetyun.com
 License: Apache License 2.0
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
@@ -17,54 +17,62 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6.*
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: dask
-Provides-Extra: notebook
 Provides-Extra: extra
+Provides-Extra: notebook
 Provides-Extra: board
 Provides-Extra: tests
 Provides-Extra: cuml
 Provides-Extra: zhcn
+Provides-Extra: dask
+Provides-Extra: fg
 Provides-Extra: all
 License-File: LICENSE
 
 <p align="center">
-<img src="docs/source/images/Hypernets.png" width="500" >
+<img src="https://raw.githubusercontent.com/DataCanvasIO/Hypernets/master/docs/source/images/Hypernets.png" width="500" >
 
 
 [![Python Versions](https://img.shields.io/pypi/pyversions/hypernets.svg)](https://pypi.org/project/hypernets)
 [![Downloads](https://pepy.tech/badge/hypernets)](https://pepy.tech/project/hypernets)
 [![PyPI Version](https://img.shields.io/pypi/v/hypernets.svg)](https://pypi.org/project/hypernets)
 
 ## We Are Hiring！
 Dear folks, we are offering challenging opportunities located in Beijing for both professionals and students who are keen on AutoML/NAS. Come be a part of DataCanvas! Please send your CV to yangjian@zetyun.com. (Application deadline: TBD.)  
 
 ## Hypernets: A General Automated Machine Learning Framework
 Hypernets is a general AutoML framework, based on which it can implement automatic optimization tools for various machine learning frameworks and libraries, including deep learning frameworks such as tensorflow, keras, pytorch, and machine learning libraries like sklearn, lightgbm, xgboost, etc.
+It also adopted various state-of-the-art optimization algorithms, including but not limited to evolution algorithm, monte carlo tree search for single objective optimization and multi-objective optimization algorithms such as MOEA/D,NSGA-II,R-NSGA-II.
 We introduced an abstract search space representation, taking into account the requirements of hyperparameter optimization and neural architecture search(NAS), making Hypernets a general framework that can adapt to various automated machine learning needs. As an abstraction computing layer, tabular toolbox, has successfully implemented in various tabular data types: pandas, dask, cudf, etc.  
 
 
 
 ## Overview
 ### Conceptual Model
 <p align="center">
-<img src="docs/source/images/hypernets_conceptual_model.png" width="100%"/>
+<img src="https://raw.githubusercontent.com/DataCanvasIO/Hypernets/master/docs/source/images/hypernets_conceptual_model.png" width="100%"/>
 </p>
 
 ### Illustration of the Search Space 
 <p align="center">
-<img src="docs/source/images/hypernets_search_space.png" width="100%"/>
+<img src="https://raw.githubusercontent.com/DataCanvasIO/Hypernets/master/docs/source/images/hypernets_search_space.png" width="100%"/>
 </p>
 
+## What's NEW !
+
+- **New feature:** [Multi-objectives optimization support](https://hypernets.readthedocs.io/en/latest/searchers.html#multi-objective-optimization)
+- **New feature:** [Performance and model complexity measurement metrics](https://github.com/DataCanvasIO/HyperGBM/blob/main/hypergbm/examples/66.Objectives_example.ipynb)
+- **New feature:** [Distributed computing](https://hypergbm.readthedocs.io/en/latest/example_dask.html) and [GPU acceleration](https://hypergbm.readthedocs.io/en/latest/example_cuml.html) base on computational abstraction layer
+
 
 ## Installation
 
 ### Conda
 
 Install Hypernets with `conda` from the channel *conda-forge*:
 
@@ -99,43 +107,62 @@
 
 * Install all above with one command:
 ```bash
 pip install hypernets[all]
 ```
 
 
-***Verify installation***:
+To ***Verify*** your installation:
 ```bash
 python -m hypernets.examples.smoke_testing
 ```
 
 ## Related Links
 
 * [A Brief Tutorial for Developing AutoML Tools with Hypernets](https://github.com/BochenLv/knn_toy_model/blob/main/Introduction.md)
 
-## Hypernets related projects
-* [Hypernets](https://github.com/DataCanvasIO/Hypernets): A general automated machine learning (AutoML) framework.
-* [HyperGBM](https://github.com/DataCanvasIO/HyperGBM): A full pipeline AutoML tool integrated various GBM models.
-* [HyperDT/DeepTables](https://github.com/DataCanvasIO/DeepTables): An AutoDL tool for tabular data.
-* [HyperTS](https://github.com/DataCanvasIO/HyperTS): A full pipeline AutoML&AutoDL tool for time series datasets.
-* [HyperKeras](https://github.com/DataCanvasIO/HyperKeras): An AutoDL tool for Neural Architecture Search and Hyperparameter Optimization on Tensorflow and Keras.
-* [HyperBoard](https://github.com/DataCanvasIO/HyperBoard): A visualization tool for Hypernets.
-* [Cooka](https://github.com/DataCanvasIO/Cooka): Lightweight interactive AutoML system.
-
-
-![DataCanvas AutoML Toolkit](docs/source/images/DAT_logo.png)
-
 ## Documents
 * [Overview](https://hypernets.readthedocs.io/en/latest/overview.html)
 * [QuickStart](https://hypernets.readthedocs.io/en/latest/quick_start.html)
 * [Search Space](https://hypernets.readthedocs.io/en/latest/search_space.html)
 * [Searcher](https://hypernets.readthedocs.io/en/latest/searchers.html)
 * [HyperModel](https://hypernets.readthedocs.io/en/latest/hypermodels.html)
 * [Experiment](https://hypernets.readthedocs.io/en/latest/experiment.html)
 ## Neural Architecture Search
 * [Define A DNN Search Space](https://hypernets.readthedocs.io/en/latest/nas.html#define-a-dnn-search-space)
 * [Define A CNN Search Space](https://hypernets.readthedocs.io/en/latest/nas.html#define-a-cnn-search-space)
 * [Define An ENAS Micro Search Space](https://hypernets.readthedocs.io/en/latest/nas.html#define-an-enas-micro-search-space)
 
 
+## Hypernets related projects
+* [Hypernets](https://github.com/DataCanvasIO/Hypernets): A general automated machine learning (AutoML) framework.
+* [HyperGBM](https://github.com/DataCanvasIO/HyperGBM): A full pipeline AutoML tool integrated various GBM models.
+* [HyperDT/DeepTables](https://github.com/DataCanvasIO/DeepTables): An AutoDL tool for tabular data.
+* [HyperTS](https://github.com/DataCanvasIO/HyperTS): A full pipeline AutoML&AutoDL tool for time series datasets.
+* [HyperKeras](https://github.com/DataCanvasIO/HyperKeras): An AutoDL tool for Neural Architecture Search and Hyperparameter Optimization on Tensorflow and Keras.
+* [HyperBoard](https://github.com/DataCanvasIO/HyperBoard): A visualization tool for Hypernets.
+* [Cooka](https://github.com/DataCanvasIO/Cooka): Lightweight interactive AutoML system.
+
+
+![DataCanvas AutoML Toolkit](https://raw.githubusercontent.com/DataCanvasIO/Hypernets/master/docs/source/images/DAT_latest.png)
+
+## Citation
+
+If you use Hypernets in your research, please cite us as follows:
+
+   Jian Yang, Xuefeng Li, Haifeng Wu. 
+   **Hypernets: A General Automated Machine Learning Framework.** https://github.com/DataCanvasIO/Hypernets. 2020. Version 0.2.x.
+
+BibTex:
+
+```
+@misc{hypernets,
+  author={Jian Yang, Xuefeng Li, Haifeng Wu},
+  title={{Hypernets}: { A General Automated Machine Learning Framework}},
+  howpublished={https://github.com/DataCanvasIO/Hypernets},
+  note={Version 0.2.x},
+  year={2020}
+}
+```
+
 ## DataCanvas
 Hypernets is an open source project created by [DataCanvas](https://www.datacanvas.com/).
```

### Comparing `hypernets-0.2.5.7/hypernets.egg-info/SOURCES.txt` & `hypernets-0.3.0/hypernets.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,18 +11,21 @@
 hypernets.egg-info/requires.txt
 hypernets.egg-info/top_level.txt
 hypernets/conf/__init__.py
 hypernets/conf/_configuration.py
 hypernets/core/__init__.py
 hypernets/core/callbacks.py
 hypernets/core/config.py
+hypernets/core/context.py
 hypernets/core/dispatcher.py
 hypernets/core/meta_learner.py
 hypernets/core/mutables.py
+hypernets/core/objective.py
 hypernets/core/ops.py
+hypernets/core/pareto.py
 hypernets/core/random_state.py
 hypernets/core/search_space.py
 hypernets/core/searcher.py
 hypernets/core/stateful.py
 hypernets/core/trial.py
 hypernets/discriminators/__init__.py
 hypernets/discriminators/_base.py
@@ -87,22 +90,27 @@
 hypernets/hyperctl/executor.py
 hypernets/hyperctl/scheduler.py
 hypernets/hyperctl/server.py
 hypernets/hyperctl/utils.py
 hypernets/model/__init__.py
 hypernets/model/estimator.py
 hypernets/model/hyper_model.py
+hypernets/model/objectives.py
 hypernets/pipeline/__init__.py
 hypernets/pipeline/base.py
 hypernets/pipeline/transformers.py
 hypernets/searchers/__init__.py
 hypernets/searchers/evolution_searcher.py
+hypernets/searchers/genetic.py
 hypernets/searchers/grid_searcher.py
 hypernets/searchers/mcts_core.py
 hypernets/searchers/mcts_searcher.py
+hypernets/searchers/moead_searcher.py
+hypernets/searchers/moo.py
+hypernets/searchers/nsga_searcher.py
 hypernets/searchers/playback_searcher.py
 hypernets/searchers/random_searcher.py
 hypernets/server/__init__.py
 hypernets/tabular/__init__.py
 hypernets/tabular/_base.py
 hypernets/tabular/cache.py
 hypernets/tabular/cfg.py
@@ -147,14 +155,15 @@
 hypernets/tabular/dask_ex/_toolbox.py
 hypernets/tabular/dask_ex/_transformers.py
 hypernets/tabular/datasets/Bike_Sharing.csv
 hypernets/tabular/datasets/__init__.py
 hypernets/tabular/datasets/adult-uci.csv.gz
 hypernets/tabular/datasets/bank-uci.csv.gz
 hypernets/tabular/datasets/blood.csv
+hypernets/tabular/datasets/boston.csv.gz
 hypernets/tabular/datasets/dsutils.py
 hypernets/tabular/datasets/glass_uci.csv
 hypernets/tabular/datasets/heart-disease-uci.csv
 hypernets/tabular/datasets/movielens_sample.txt
 hypernets/tabular/datasets/telescope.csv
 hypernets/tabular/ensemble/__init__.py
 hypernets/tabular/ensemble/base_ensemble.py
@@ -202,22 +211,27 @@
 hypernets/tests/hyperctl/plain_job_script.py
 hypernets/tests/hyperctl/test_application.py
 hypernets/tests/hyperctl/test_batch.py
 hypernets/tests/hyperctl/test_cli.py
 hypernets/tests/hyperctl/test_scheduler.py
 hypernets/tests/model/__init__.py
 hypernets/tests/model/plain_model_test.py
+hypernets/tests/model/test_objectives.py
 hypernets/tests/pipeline/__init__.py
 hypernets/tests/pipeline/pipeline_test.py
 hypernets/tests/searchers/__init__.py
 hypernets/tests/searchers/evolution_test.py
 hypernets/tests/searchers/grid_test.py
 hypernets/tests/searchers/mcts_test.py
 hypernets/tests/searchers/playback_test.py
 hypernets/tests/searchers/random_test.py
+hypernets/tests/searchers/test_genetic.py
+hypernets/tests/searchers/test_moead_searcher.py
+hypernets/tests/searchers/test_moo.py
+hypernets/tests/searchers/test_nsga2_searcher.py
 hypernets/tests/tabular/__init__.py
 hypernets/tests/tabular/cache_test.py
 hypernets/tests/tabular/column_selector_test.py
 hypernets/tests/tabular/data_cleaner_test.py
 hypernets/tests/tabular/drift_detection_test.py
 hypernets/tests/tabular/feature_generator_test.py
 hypernets/tests/tabular/feature_importance_test.py
```

### Comparing `hypernets-0.2.5.7/setup.py` & `hypernets-0.3.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # -*- coding:utf-8 -*-
 
 from __future__ import absolute_import
 
 from setuptools import find_packages
 from setuptools import setup
 
+home_url = 'https://github.com/DataCanvasIO/Hypernets'
+
 
 def read_requirements(file_path='requirements.txt'):
     import os
 
     if not os.path.exists(file_path):
         return []
 
@@ -35,32 +37,62 @@
 
     if extra and 'all' not in extra.keys():
         extra['all'] = sorted({v for req in extra.values() for v in req})
 
     return extra
 
 
+# def read_description(file_path='README.md',
+#                      image_root=f'{home_url}/raw/main'):
+#     import re
+#     import os
+#
+#     def _encode_image(m):
+#         assert len(m.groups()) == 3
+#
+#         pre, src, post = m.groups()
+#         src = src.rstrip().lstrip()
+#         remote_src = os.path.join(image_root, os.path.relpath(src))
+#         return f'{pre}{remote_src}{post}'
+#
+#     desc = open(file_path, encoding='utf-8').read()
+#
+#     # substitute html image
+#     desc = re.sub(r'(<img\s+src\s*=\s*\")(docs/source/images/[^"]+)(\")', _encode_image, desc)
+#
+#     # substitute markdown image
+#     desc = re.sub(r'(\!\[.*\]\()(docs/source/images/.+)(\))', _encode_image, desc)
+#
+#     return desc
+
+def read_description(file_path='README.md'):
+    with open(file_path, encoding='utf-8') as f:
+        desc = f.read()
+    return desc
+
+
 import hypernets
 
 version = hypernets.__version__
 
-MIN_PYTHON_VERSION = '>=3.6.*'
+MIN_PYTHON_VERSION = '>=3.6'
 
-long_description = open('README.md', encoding='utf-8').read()
+# long_description = open('README.md', encoding='utf-8').read()
+long_description = read_description()
 
 requires = read_requirements()
 extras_require = read_extra_requirements()
 
 setup(
     name='hypernets',
     version=version,
     description='An General Automated Machine Learning Framework',
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url='',
+    url='https://github.com/DataCanvasIO/Hypernets',
     author='DataCanvas Community',
     author_email='yangjian@zetyun.com',
     license='Apache License 2.0',
     install_requires=requires,
     python_requires=MIN_PYTHON_VERSION,
     extras_require=extras_require,
     classifiers=[
```

