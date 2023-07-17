# Comparing `tmp/ml-starter-0.1.8.tar.gz` & `tmp/ml-starter-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-starter-0.1.8.tar", last modified: Tue Jun 27 05:21:27 2023, max compression
+gzip compressed data, was "ml-starter-0.1.9.tar", last modified: Tue Jun 27 06:45:35 2023, max compression
```

## Comparing `ml-starter-0.1.8.tar` & `ml-starter-0.1.9.tar`

### file list

```diff
@@ -1,171 +1,171 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:27.611322 ml-starter-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-27 05:21:15.000000 ml-starter-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-27 05:21:15.000000 ml-starter-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-27 05:21:27.611322 ml-starter-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-27 05:21:15.000000 ml-starter-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:27.595322 ml-starter-0.1.8/ml/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:27.595322 ml-starter-0.1.8/ml/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/core/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/core/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    25216 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/core/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/core/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:27.595322 ml-starter-0.1.8/ml/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/launchers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/launchers/mp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/launchers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/launchers/torchrun.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:27.595322 ml-starter-0.1.8/ml/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/loggers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/loggers/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)    44768 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/loggers/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/loggers/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)    13618 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:27.595322 ml-starter-0.1.8/ml/lr_schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/lr_schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/lr_schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/lr_schedulers/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/lr_schedulers/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/lr_schedulers/cosine_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/lr_schedulers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/lr_schedulers/linear_no_decay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:27.599322 ml-starter-0.1.8/ml/lr_schedulers/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/lr_schedulers/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/lr_schedulers/scripts/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:27.599322 ml-starter-0.1.8/ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/models/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/models/codebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/models/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/models/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/models/kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)    49884 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/models/lora.py
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/models/norms.py
--rw-r--r--   0 runner    (1001) docker     (123)    16423 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/models/parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:27.599322 ml-starter-0.1.8/ml/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/optimizers/adamw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/optimizers/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/optimizers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/optimizers/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/optimizers/lion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/optimizers/sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/optimizers/shampoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/optimizers/types.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:27.599322 ml-starter-0.1.8/ml/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/scripts/launch.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/scripts/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/scripts/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:27.603322 ml-starter-0.1.8/ml/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18929 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/tasks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:27.603322 ml-starter-0.1.8/ml/tasks/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/tasks/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/tasks/datasets/async_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/tasks/datasets/clippify.py
--rw-r--r--   0 runner    (1001) docker     (123)     7359 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/tasks/datasets/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/tasks/datasets/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/tasks/datasets/multi_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/tasks/datasets/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/tasks/datasets/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/tasks/datasets/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/tasks/datasets/video_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:27.603322 ml-starter-0.1.8/ml/tasks/environments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/tasks/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/tasks/environments/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/tasks/environments/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/tasks/environments/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:27.603322 ml-starter-0.1.8/ml/tasks/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/tasks/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/tasks/losses/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/tasks/losses/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/tasks/losses/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/tasks/losses/reduce.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:27.603322 ml-starter-0.1.8/ml/tasks/rl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/tasks/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18535 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/tasks/rl/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/tasks/rl/replay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:27.603322 ml-starter-0.1.8/ml/tasks/sl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/tasks/sl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/tasks/sl/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:27.607322 ml-starter-0.1.8/ml/trainers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20792 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/trainers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9499 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/trainers/learning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:27.607322 ml-starter-0.1.8/ml/trainers/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/trainers/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/trainers/mixins/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9259 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/trainers/mixins/cpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/trainers/mixins/data_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/trainers/mixins/gpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/trainers/mixins/grad_clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/trainers/mixins/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/trainers/mixins/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/trainers/mixins/monitor_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/trainers/mixins/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/trainers/mixins/step_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/trainers/rl.py
--rw-r--r--   0 runner    (1001) docker     (123)     9864 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/trainers/sl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:27.611322 ml-starter-0.1.8/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/atomic.py
--rw-r--r--   0 runner    (1001) docker     (123)    13214 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:27.611322 ml-starter-0.1.8/ml/utils/device/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/device/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/device/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/device/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/device/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/device/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/large_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/staging.py
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13028 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/torch_distributed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:27.611322 ml-starter-0.1.8/ml/utils/triton/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/triton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/triton/kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/triton/lion.py
--rw-r--r--   0 runner    (1001) docker     (123)    20942 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:27.611322 ml-starter-0.1.8/ml_starter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-27 05:21:27.000000 ml-starter-0.1.8/ml_starter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-06-27 05:21:27.000000 ml-starter-0.1.8/ml_starter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 05:21:27.000000 ml-starter-0.1.8/ml_starter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-27 05:21:27.000000 ml-starter-0.1.8/ml_starter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-27 05:21:27.000000 ml-starter-0.1.8/ml_starter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-27 05:21:15.000000 ml-starter-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-27 05:21:15.000000 ml-starter-0.1.8/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-27 05:21:15.000000 ml-starter-0.1.8/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-27 05:21:15.000000 ml-starter-0.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-27 05:21:27.611322 ml-starter-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-27 05:21:15.000000 ml-starter-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:45:35.608343 ml-starter-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-27 06:45:21.000000 ml-starter-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-27 06:45:21.000000 ml-starter-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-27 06:45:35.608343 ml-starter-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-27 06:45:21.000000 ml-starter-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:45:35.592342 ml-starter-0.1.9/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:45:35.592342 ml-starter-0.1.9/ml/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/core/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/core/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26065 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/core/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:45:35.592342 ml-starter-0.1.9/ml/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/launchers/mp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10157 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/launchers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/launchers/torchrun.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:45:35.592342 ml-starter-0.1.9/ml/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/loggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/loggers/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44768 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/loggers/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/loggers/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13618 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:45:35.596342 ml-starter-0.1.9/ml/lr_schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/lr_schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/lr_schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/lr_schedulers/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/lr_schedulers/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/lr_schedulers/cosine_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/lr_schedulers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/lr_schedulers/linear_no_decay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:45:35.596342 ml-starter-0.1.9/ml/lr_schedulers/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/lr_schedulers/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/lr_schedulers/scripts/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:45:35.596342 ml-starter-0.1.9/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/models/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/models/codebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/models/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/models/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/models/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49884 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/models/lora.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/models/norms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16423 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/models/parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:45:35.596342 ml-starter-0.1.9/ml/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/optimizers/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/optimizers/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/optimizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/optimizers/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/optimizers/lion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/optimizers/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/optimizers/shampoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/optimizers/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:45:35.596342 ml-starter-0.1.9/ml/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/scripts/launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/scripts/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/scripts/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:45:35.600343 ml-starter-0.1.9/ml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18929 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/tasks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:45:35.600343 ml-starter-0.1.9/ml/tasks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/tasks/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/tasks/datasets/async_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/tasks/datasets/clippify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7359 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/tasks/datasets/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/tasks/datasets/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/tasks/datasets/multi_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/tasks/datasets/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/tasks/datasets/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/tasks/datasets/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/tasks/datasets/video_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:45:35.600343 ml-starter-0.1.9/ml/tasks/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/tasks/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/tasks/environments/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/tasks/environments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/tasks/environments/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:45:35.600343 ml-starter-0.1.9/ml/tasks/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/tasks/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/tasks/losses/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/tasks/losses/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/tasks/losses/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/tasks/losses/reduce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:45:35.600343 ml-starter-0.1.9/ml/tasks/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/tasks/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18535 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/tasks/rl/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/tasks/rl/replay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:45:35.600343 ml-starter-0.1.9/ml/tasks/sl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/tasks/sl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/tasks/sl/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:45:35.600343 ml-starter-0.1.9/ml/trainers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20792 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/trainers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9499 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/trainers/learning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:45:35.604343 ml-starter-0.1.9/ml/trainers/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/trainers/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/trainers/mixins/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9259 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/trainers/mixins/cpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/trainers/mixins/data_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/trainers/mixins/gpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/trainers/mixins/grad_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/trainers/mixins/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/trainers/mixins/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/trainers/mixins/monitor_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/trainers/mixins/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/trainers/mixins/step_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/trainers/rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9864 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/trainers/sl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:45:35.608343 ml-starter-0.1.9/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/utils/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/utils/atomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13214 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/utils/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/utils/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/utils/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:45:35.608343 ml-starter-0.1.9/ml/utils/device/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/utils/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/utils/device/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/utils/device/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/utils/device/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/utils/device/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/utils/device/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/utils/large_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/utils/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/utils/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/utils/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/utils/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/utils/staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13028 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/utils/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/utils/torch_distributed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:45:35.608343 ml-starter-0.1.9/ml/utils/triton/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/utils/triton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/utils/triton/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/utils/triton/lion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20942 2023-06-27 06:45:21.000000 ml-starter-0.1.9/ml/utils/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:45:35.608343 ml-starter-0.1.9/ml_starter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-27 06:45:35.000000 ml-starter-0.1.9/ml_starter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-06-27 06:45:35.000000 ml-starter-0.1.9/ml_starter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 06:45:35.000000 ml-starter-0.1.9/ml_starter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-27 06:45:35.000000 ml-starter-0.1.9/ml_starter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-27 06:45:35.000000 ml-starter-0.1.9/ml_starter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-27 06:45:21.000000 ml-starter-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-27 06:45:21.000000 ml-starter-0.1.9/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-27 06:45:21.000000 ml-starter-0.1.9/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-27 06:45:21.000000 ml-starter-0.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-27 06:45:35.608343 ml-starter-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-27 06:45:21.000000 ml-starter-0.1.9/setup.py
```

### Comparing `ml-starter-0.1.8/LICENSE` & `ml-starter-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/PKG-INFO` & `ml-starter-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.1.8
+Version: 0.1.9
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.1.8/README.md` & `ml-starter-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/api.py` & `ml-starter-0.1.9/ml/api.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/core/common_types.py` & `ml-starter-0.1.9/ml/core/common_types.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/core/config.py` & `ml-starter-0.1.9/ml/core/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/core/env.py` & `ml-starter-0.1.9/ml/core/env.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/core/registry.py` & `ml-starter-0.1.9/ml/core/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,27 @@
 project_dirs = _ProjectDirs()
 
 # Some aliases for the project directory accessors.
 add_project_dir = project_dirs.add
 project_dir_paths = project_dirs.paths
 
 
+def _iter_directory(subfiles: list[Path], *curdirs: Path) -> Iterator[Path]:
+    for curdir in curdirs:
+        for subpath in curdir.iterdir():
+            if subpath.stem.startswith("__"):
+                continue
+            if subpath.is_file() and subpath.suffix == ".py":
+                subfile = subpath.resolve()
+                subfiles.append(subfile)
+                yield subfile
+            elif subpath.is_dir():
+                yield from _iter_directory(subfiles, subpath)
+
+
 def get_name(key: str, config: BaseContainer) -> str:
     if not isinstance(config, DictConfig):
         raise ValueError(f"Expected {key} config to be a dictionary, got {type(config)}")
     if NAME_KEY not in config:
         raise ValueError(f"Malformed {key} config; missing expected key {NAME_KEY}")
     name = config[NAME_KEY]
     if not isinstance(name, str):
@@ -110,15 +123,15 @@
         names.append(name)
     return names
 
 
 class register_base(ABC, Generic[Entry, Config]):  # noqa: N801
     """Defines the base registry type."""
 
-    REGISTRY: dict[str, tuple[type[Entry], type[Config]]] = {}
+    REGISTRY: dict[str, tuple[type[Entry], type[Config] | Config]] = {}
     REGISTRY_LOCATIONS: dict[str, Path] = {}
 
     @classmethod
     @abstractmethod
     def search_directory(cls) -> Path:
         """Returns the directory to search for entries."""
 
@@ -201,44 +214,49 @@
             if name in cls.REGISTRY:
                 return
 
         # This gets populated the first time we walk the directories, so that
         # the second time we can just iterate through it again.
         subfiles: list[Path] = []
 
-        def iter_directory(*curdirs: Path) -> Iterator[Path]:
-            for curdir in curdirs:
-                for subpath in curdir.iterdir():
-                    if subpath.stem.startswith("__"):
-                        continue
-                    if subpath.is_file() and subpath.suffix == ".py":
-                        subfile = subpath.resolve()
-                        subfiles.append(subfile)
-                        yield subfile
-                    elif subpath.is_dir():
-                        yield from iter_directory(subpath)
-
         # Next sweep over the search directory and check for prefix matches.
         search_dir = cls.search_directory()
         search_dirs = [base_dir / search_dir for base_dir in project_dirs.paths]
         search_dirs = [search_dir for search_dir in search_dirs if search_dir.is_dir()]
-        for path in iter_directory(*search_dirs):
+        for path in _iter_directory(subfiles, *search_dirs):
             if path.stem.lower().startswith(lower_name) or lower_name.startswith(path.stem.lower()):
                 cls.manual_import(path)
                 if name in cls.REGISTRY:
                     return
 
         # Finally, try loading files from the requested import path until
         # we've imported the name that we're looking for.
         for path in subfiles:
             cls.manual_import(path)
             if name in cls.REGISTRY:
                 return
 
     @classmethod
+    def populate_full_regisry(cls) -> None:
+        """Populates the complete registry, removing invalid cached values."""
+        cls.REGISTRY.clear()
+        cls.REGISTRY_LOCATIONS.clear()
+
+        # This gets populated the first time we walk the directories, so that
+        # the second time we can just iterate through it again.
+        subfiles: list[Path] = []
+
+        # Sweep over the search directory and import everything.
+        search_dir = cls.search_directory()
+        search_dirs = [base_dir / search_dir for base_dir in project_dirs.paths]
+        search_dirs = [search_dir for search_dir in search_dirs if search_dir.is_dir()]
+        for path in _iter_directory(subfiles, *search_dirs):
+            cls.manual_import(path)
+
+    @classmethod
     @functools.lru_cache(None)
     def lookup(cls, name: str) -> tuple[type[Entry], type[Config]]:
         # Just loads the entry, if it already exists.
         if name in cls.REGISTRY:
             return cls.REGISTRY[name]
 
         # If not found, populates the registry. If still not found, then
@@ -341,15 +359,15 @@
         # Adds the registry entry and the entry's location to their respective
         # dictionaries. We overwrite any outdated cache entries.
         self.REGISTRY[self.name] = cast(tuple[type[Entry], type[Config]], (entry, self.config))
         self.REGISTRY_LOCATIONS[self.name] = registry_location
 
         # Adds all default configurations as well.
         for key, default_cfg in self.config.get_defaults().items():
-            self.REGISTRY[key] = cast(tuple[type[Entry], type[Config]], (entry, default_cfg))
+            self.REGISTRY[key] = (cast(type[Entry], entry), default_cfg)
             self.REGISTRY_LOCATIONS[key] = registry_location
 
         return entry
 
 
 class multi_register_base(register_base[Entry, Config], Generic[Entry, Config]):  # noqa: N801
     """Defines a registry which produces multiple objects."""
@@ -438,103 +456,103 @@
                 reg_cfgs[i] = reg_cfg
             raw_config[cls.config_key()] = reg_cfgs
 
 
 class register_model(register_base["BaseModel", "BaseModelConfig"]):  # noqa: N801
     """Defines a registry for holding modules."""
 
-    REGISTRY: dict[str, tuple[type["BaseModel"], type["BaseModelConfig"]]] = {}
+    REGISTRY: dict[str, tuple[type["BaseModel"], "type[BaseModelConfig] | BaseModelConfig"]] = {}
     REGISTRY_LOCATIONS: dict[str, Path] = {}
 
     @classmethod
     def search_directory(cls) -> Path:
         return Path("models")
 
     @classmethod
     def config_key(cls) -> str:
         return "model"
 
 
 class register_task(register_base["BaseTask", "BaseTaskConfig"]):  # noqa: N801
     """Defines a registry for holding tasks."""
 
-    REGISTRY: dict[str, tuple[type["BaseTask"], type["BaseTaskConfig"]]] = {}
+    REGISTRY: dict[str, tuple[type["BaseTask"], "type[BaseTaskConfig] | BaseTaskConfig"]] = {}
     REGISTRY_LOCATIONS: dict[str, Path] = {}
 
     @classmethod
     def search_directory(cls) -> Path:
         return Path("tasks")
 
     @classmethod
     def config_key(cls) -> str:
         return "task"
 
 
 class register_trainer(register_base["BaseTrainer", "BaseTrainerConfig"]):  # noqa: N801
     """Defines a registry for holding trainers."""
 
-    REGISTRY: dict[str, tuple[type["BaseTrainer"], type["BaseTrainerConfig"]]] = {}
+    REGISTRY: dict[str, tuple[type["BaseTrainer"], "type[BaseTrainerConfig] | BaseTrainerConfig"]] = {}
     REGISTRY_LOCATIONS: dict[str, Path] = {}
 
     @classmethod
     def search_directory(cls) -> Path:
         return Path("trainers")
 
     @classmethod
     def config_key(cls) -> str:
         return "trainer"
 
 
 class register_optimizer(register_base["BaseOptimizer", "BaseOptimizerConfig"]):  # noqa: N801
     """Defines a registry for holding optimizers."""
 
-    REGISTRY: dict[str, tuple[type["BaseOptimizer"], type["BaseOptimizerConfig"]]] = {}
+    REGISTRY: dict[str, tuple[type["BaseOptimizer"], "type[BaseOptimizerConfig] | BaseOptimizerConfig"]] = {}
     REGISTRY_LOCATIONS: dict[str, Path] = {}
 
     @classmethod
     def search_directory(cls) -> Path:
         return Path("optimizers")
 
     @classmethod
     def config_key(cls) -> str:
         return "optimizer"
 
 
 class register_lr_scheduler(register_base["BaseLRScheduler", "BaseLRSchedulerConfig"]):  # noqa: N801
     """Defines a registry for holding learning rate schedulers."""
 
-    REGISTRY: dict[str, tuple[type["BaseLRScheduler"], type["BaseLRSchedulerConfig"]]] = {}
+    REGISTRY: dict[str, tuple[type["BaseLRScheduler"], "type[BaseLRSchedulerConfig] | BaseLRSchedulerConfig"]] = {}
     REGISTRY_LOCATIONS: dict[str, Path] = {}
 
     @classmethod
     def search_directory(cls) -> Path:
         return Path("lr_schedulers")
 
     @classmethod
     def config_key(cls) -> str:
         return "lr_scheduler"
 
 
 class register_logger(multi_register_base["BaseLogger", "BaseLoggerConfig"]):  # noqa: N801
     """Defines a registry for holding loggers."""
 
-    REGISTRY: dict[str, tuple[type["BaseLogger"], type["BaseLoggerConfig"]]] = {}
+    REGISTRY: dict[str, tuple[type["BaseLogger"], "type[BaseLoggerConfig] | BaseLoggerConfig"]] = {}
     REGISTRY_LOCATIONS: dict[str, Path] = {}
 
     @classmethod
     def search_directory(cls) -> Path:
         return Path("loggers")
 
     @classmethod
     def config_key(cls) -> str:
         return "logger"
 
 
 class register_launcher(register_base["BaseLauncher", "BaseLauncherConfig"]):  # noqa: N801
-    REGISTRY: dict[str, tuple[type["BaseLauncher"], type["BaseLauncherConfig"]]] = {}
+    REGISTRY: dict[str, tuple[type["BaseLauncher"], "type[BaseLauncherConfig] | BaseLauncherConfig"]] = {}
     REGISTRY_LOCATIONS: dict[str, Path] = {}
 
     @classmethod
     def search_directory(cls) -> Path:
         return Path("launchers")
 
     @classmethod
```

### Comparing `ml-starter-0.1.8/ml/core/state.py` & `ml-starter-0.1.9/ml/core/state.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/launchers/base.py` & `ml-starter-0.1.9/ml/launchers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/launchers/mp.py` & `ml-starter-0.1.9/ml/launchers/mp.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/launchers/slurm.py` & `ml-starter-0.1.9/ml/launchers/slurm.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,16 @@
 from ml.utils.staging import stage_environment
 from ml.utils.torch_distributed import init_process_group_from_backend
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 T = TypeVar("T", bound="SlurmLauncher")
 
+OmegaConf.register_new_resolver("ml.get_random_slurm_port", get_random_port, replace=True)
+
 SBATCH_TEMPLATE: str = """
 #!/bin/bash
 #SBATCH --job-name={job_name}
 #SBATCH --partition={partition}
 #SBATCH --requeue
 #SBATCH --signal=USR1@90
 #SBATCH --time={time_limit}
@@ -139,15 +141,15 @@
     time_limit: str = conf_field(II("oc.env:SLURM_TIME_LIMIT,3-00:00:00"), help="Time limit string")
     num_nodes: int = conf_field(MISSING, help="Total number of nodes to use")
     gpus_per_node: int = conf_field(II("oc.env:SLURM_GPUS_PER_NODE,8"), help="Number of GPUs per node")
     cpus_per_gpu: int = conf_field(II("oc.env:SLURM_CPUS_PER_GPU,1"), help="Number of CPUs per task")
     gpu_type: str | None = conf_field(None, help="Specific GPU type to pass to gres")
     num_jobs: int = conf_field(1, help="Number of redundant jobs to launch")
     comment: str | None = conf_field(None, help="An optional comment to add to the experiment")
-    master_port: int = conf_field(get_random_port, help="The master port to use")
+    master_port: int = conf_field(II("ml.get_random_slurm_port:1337"), help="The master port to use")
 
 
 def ignore_signal(signum: int, _: FrameType | None) -> None:
     sig = signal.Signals(signum)
     logger.info("Ignoring signal %s", sig.name)
```

### Comparing `ml-starter-0.1.8/ml/launchers/torchrun.py` & `ml-starter-0.1.9/ml/launchers/torchrun.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/loggers/base.py` & `ml-starter-0.1.9/ml/loggers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/loggers/meter.py` & `ml-starter-0.1.9/ml/loggers/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/loggers/multi.py` & `ml-starter-0.1.9/ml/loggers/multi.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/loggers/stdout.py` & `ml-starter-0.1.9/ml/loggers/stdout.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/loggers/tensorboard.py` & `ml-starter-0.1.9/ml/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/lr_schedulers/base.py` & `ml-starter-0.1.9/ml/lr_schedulers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/lr_schedulers/constant.py` & `ml-starter-0.1.9/ml/lr_schedulers/constant.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/lr_schedulers/cosine.py` & `ml-starter-0.1.9/ml/lr_schedulers/cosine.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/lr_schedulers/cosine_decay.py` & `ml-starter-0.1.9/ml/lr_schedulers/cosine_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/lr_schedulers/linear.py` & `ml-starter-0.1.9/ml/lr_schedulers/linear.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/lr_schedulers/linear_no_decay.py` & `ml-starter-0.1.9/ml/lr_schedulers/linear_no_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/lr_schedulers/scripts/plot.py` & `ml-starter-0.1.9/ml/lr_schedulers/scripts/plot.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/models/activations.py` & `ml-starter-0.1.9/ml/models/activations.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/models/base.py` & `ml-starter-0.1.9/ml/models/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/models/codebook.py` & `ml-starter-0.1.9/ml/models/codebook.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/models/embeddings.py` & `ml-starter-0.1.9/ml/models/embeddings.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/models/init.py` & `ml-starter-0.1.9/ml/models/init.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/models/kmeans.py` & `ml-starter-0.1.9/ml/models/kmeans.py`

 * *Files 24% similar despite different names*

```diff
@@ -49,15 +49,16 @@
 
         n_clusters, n_features = centers.shape
         self.n_clusters = n_clusters
         self.n_features = n_features
         self.register_buffer("centers", torch.empty(n_clusters, n_features))
         self.register_buffer("centers_norm", torch.empty(n_clusters))
         self.load_centers(centers)
-        self.kmeans_fn = kmeans_fn(use_triton_if_available)
+        self.kmeans_fn = kmeans_fn(False)
+        self.kmeans_fn_cuda = kmeans_fn(use_triton_if_available)
 
     def load_centers(self, centers: Tensor | np.ndarray) -> None:
         if isinstance(centers, np.ndarray):
             centers = torch.from_numpy(centers)
         assert centers.shape == self.centers.shape, f"Expected shape {self.centers.shape}, got {centers.shape}"
         self.centers.copy_(centers.to(self.centers))
         self.centers_norm.copy_((self.centers**2).sum(-1))
@@ -71,8 +72,9 @@
 
         Args:
             x: The input tensor, with shape ``(*, n_features)``
 
         Returns:
             The cluster IDs, with shape ``(*)``
         """
-        return self.kmeans_fn(x, self.centers, self.centers_norm)
+        kmeans_fn = self.kmeans_fn_cuda if x.is_cuda else self.kmeans_fn
+        return kmeans_fn(x, self.centers, self.centers_norm)
```

### Comparing `ml-starter-0.1.8/ml/models/lora.py` & `ml-starter-0.1.9/ml/models/lora.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/models/norms.py` & `ml-starter-0.1.9/ml/models/norms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/models/parallel.py` & `ml-starter-0.1.9/ml/models/parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/optimizers/adam.py` & `ml-starter-0.1.9/ml/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/optimizers/adamw.py` & `ml-starter-0.1.9/ml/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/optimizers/adan.py` & `ml-starter-0.1.9/ml/optimizers/adan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/optimizers/base.py` & `ml-starter-0.1.9/ml/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/optimizers/common.py` & `ml-starter-0.1.9/ml/optimizers/common.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/optimizers/lion.py` & `ml-starter-0.1.9/ml/optimizers/lion.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Wrapper around the Lion optimizer.
 
 This optimizer was proposed in `Symbolic Discovery of Optimization Algorithms
 <https://arxiv.org/abs/2302.06675>`_.
 
-Lion stands for "Evolved Sign Momentum". It is more memory-efficient than
-Adam since it only keeps track of momentum.
+Lion stands for "Evolved Sign Momentum" (yes, actually). It is more
+memory-efficient than Adam since it only keeps track of momentum.
 
 In the original paper, the authors suggest using a larger batch size and a
 smaller learning rate compared to Adam.
 
 This optimizer shines for tasks like contrasitve learning and diffusion which
 optimize proxy objectives rather than doing something like cross-entropy
 classification, although in the paper the authors show that it performs
```

### Comparing `ml-starter-0.1.8/ml/optimizers/sgd.py` & `ml-starter-0.1.9/ml/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/optimizers/shampoo.py` & `ml-starter-0.1.9/ml/optimizers/shampoo.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/scripts/cli.py` & `ml-starter-0.1.9/ml/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/scripts/stage.py` & `ml-starter-0.1.9/ml/scripts/stage.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/scripts/train.py` & `ml-starter-0.1.9/ml/scripts/train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/tasks/base.py` & `ml-starter-0.1.9/ml/tasks/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/tasks/datasets/async_iterable.py` & `ml-starter-0.1.9/ml/tasks/datasets/async_iterable.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/tasks/datasets/clippify.py` & `ml-starter-0.1.9/ml/tasks/datasets/clippify.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/tasks/datasets/collate.py` & `ml-starter-0.1.9/ml/tasks/datasets/collate.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/tasks/datasets/error_handling.py` & `ml-starter-0.1.9/ml/tasks/datasets/error_handling.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/tasks/datasets/multi_iter.py` & `ml-starter-0.1.9/ml/tasks/datasets/multi_iter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/tasks/datasets/samplers.py` & `ml-starter-0.1.9/ml/tasks/datasets/samplers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/tasks/datasets/streaming.py` & `ml-starter-0.1.9/ml/tasks/datasets/streaming.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/tasks/datasets/transforms.py` & `ml-starter-0.1.9/ml/tasks/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/tasks/datasets/video_file.py` & `ml-starter-0.1.9/ml/tasks/datasets/video_file.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/tasks/environments/base.py` & `ml-starter-0.1.9/ml/tasks/environments/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/tasks/environments/utils.py` & `ml-starter-0.1.9/ml/tasks/environments/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/tasks/environments/worker.py` & `ml-starter-0.1.9/ml/tasks/environments/worker.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/tasks/losses/audio.py` & `ml-starter-0.1.9/ml/tasks/losses/audio.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/tasks/losses/image.py` & `ml-starter-0.1.9/ml/tasks/losses/image.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,24 +17,22 @@
     possible values for the image. This value is the actually the negative
     SSIM, so that minimizing it maximizes the SSIM score.
 
     Parameters:
         kernel_size: Size of the Gaussian kernel.
         stride: Stride of the Gaussian kernel.
         channels: Number of channels in the image.
-        mode: Mode of the SSIM function (see below).
+        mode: Mode of the SSIM function, either ``avg`` or ``std``. The
+            ``avg`` mode uses unweighted ``(K, K)`` regions, while the ``std``
+            mode uses Gaussian weighted ``(K, K)`` regions, which allows for
+            larger regions without worrying about blurring.
         sigma: Standard deviation of the Gaussian kernel.
         dynamic_range: Difference between the maximum and minimum possible
             values for the image.
 
-    Modes:
-        avg: Use unweighted ``(K, K)`` regions
-        std: Use Gaussian weighted ``(K, K)`` regions (can use larger regions
-            without worrying about blurring)
-
     Inputs:
         x: float tensor with shape ``(B, C, H, W)``
         y: float tensor with shape ``(B, C, H, W)``
 
     Outputs:
         float tensor with shape ``(B, C, H - K + 1, W - K + 1)``
     """
```

### Comparing `ml-starter-0.1.8/ml/tasks/losses/loss.py` & `ml-starter-0.1.9/ml/tasks/losses/loss.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/tasks/losses/reduce.py` & `ml-starter-0.1.9/ml/tasks/losses/reduce.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/tasks/rl/base.py` & `ml-starter-0.1.9/ml/tasks/rl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/tasks/rl/replay.py` & `ml-starter-0.1.9/ml/tasks/rl/replay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/tasks/sl/base.py` & `ml-starter-0.1.9/ml/tasks/sl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/trainers/base.py` & `ml-starter-0.1.9/ml/trainers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/trainers/learning.py` & `ml-starter-0.1.9/ml/trainers/learning.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/trainers/mixins/compile.py` & `ml-starter-0.1.9/ml/trainers/mixins/compile.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/trainers/mixins/cpu_stats.py` & `ml-starter-0.1.9/ml/trainers/mixins/cpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/trainers/mixins/data_parallel.py` & `ml-starter-0.1.9/ml/trainers/mixins/data_parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/trainers/mixins/gpu_stats.py` & `ml-starter-0.1.9/ml/trainers/mixins/gpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/trainers/mixins/grad_clipping.py` & `ml-starter-0.1.9/ml/trainers/mixins/grad_clipping.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/trainers/mixins/heartbeat.py` & `ml-starter-0.1.9/ml/trainers/mixins/heartbeat.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/trainers/mixins/mixed_precision.py` & `ml-starter-0.1.9/ml/trainers/mixins/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/trainers/mixins/monitor_process.py` & `ml-starter-0.1.9/ml/trainers/mixins/monitor_process.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/trainers/mixins/profiler.py` & `ml-starter-0.1.9/ml/trainers/mixins/profiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/trainers/mixins/step_wrapper.py` & `ml-starter-0.1.9/ml/trainers/mixins/step_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/trainers/rl.py` & `ml-starter-0.1.9/ml/trainers/rl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/trainers/sl.py` & `ml-starter-0.1.9/ml/trainers/sl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/utils/argparse.py` & `ml-starter-0.1.9/ml/utils/argparse.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/utils/atomic.py` & `ml-starter-0.1.9/ml/utils/atomic.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/utils/audio.py` & `ml-starter-0.1.9/ml/utils/audio.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/utils/augmentation.py` & `ml-starter-0.1.9/ml/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/utils/caching.py` & `ml-starter-0.1.9/ml/utils/caching.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/utils/checkpoint.py` & `ml-starter-0.1.9/ml/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/utils/cli.py` & `ml-starter-0.1.9/ml/utils/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/utils/colors.py` & `ml-starter-0.1.9/ml/utils/colors.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/utils/data.py` & `ml-starter-0.1.9/ml/utils/data.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/utils/datetime.py` & `ml-starter-0.1.9/ml/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/utils/device/auto.py` & `ml-starter-0.1.9/ml/utils/device/auto.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,47 +8,46 @@
 
     export DISABLE_METAL=1
     export DISABLE_GPU=1
 """
 
 import functools
 import logging
-from typing import Type
 
 from ml.utils.device.base import BaseDevice
 from ml.utils.device.cpu import CPUDevice
 from ml.utils.device.gpu import GPUDevice
 from ml.utils.device.metal import MetalDevice
 from ml.utils.logging import DEBUGALL
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 # These devices are ordered by priority, so an earlier device in the list
 # is preferred to a later device in the list.
-ALL_DEVICES: list[Type[BaseDevice]] = [
+ALL_DEVICES: list[type[BaseDevice]] = [
     MetalDevice,
     GPUDevice,
     CPUDevice,
 ]
 
 
 class AutoDevice:
     """Mixin to automatically detect the device type to use."""
 
     @classmethod
     @functools.lru_cache(None)
-    def detect_device(cls) -> Type[BaseDevice]:
+    def detect_device(cls) -> type[BaseDevice]:
         for device_type in ALL_DEVICES:
             if device_type.has_device():
                 logger.log(DEBUGALL, "Device: [%s]", device_type.get_device())
                 return device_type
         raise RuntimeError("Could not automatically detect the device to use")
 
     @classmethod
-    def get_device_from_key(cls, key: str) -> Type[BaseDevice]:
+    def get_device_from_key(cls, key: str) -> type[BaseDevice]:
         if key == "auto":
             return AutoDevice.detect_device()
         if key == "cpu":
             return CPUDevice
         if key == "metal":
             return MetalDevice
         if key == "gpu":
```

### Comparing `ml-starter-0.1.8/ml/utils/device/base.py` & `ml-starter-0.1.9/ml/utils/device/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/utils/device/cpu.py` & `ml-starter-0.1.9/ml/utils/device/cpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/utils/device/gpu.py` & `ml-starter-0.1.9/ml/utils/device/gpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/utils/device/metal.py` & `ml-starter-0.1.9/ml/utils/device/metal.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/utils/distributed.py` & `ml-starter-0.1.9/ml/utils/distributed.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,16 +142,19 @@
 
     if init_method != _INIT_METHOD:
         os.environ["INIT_METHOD"] = _INIT_METHOD = init_method
     else:
         raise ValueError(f"Init method {init_method} is already set")
 
 
-def get_random_port() -> int:
-    return (hash(time.time()) + random.randint(0, 100000)) % (65_535 - 10_000) + 10_000
+def get_random_port(default: int = 1337) -> int:
+    try:
+        return (hash(time.time()) + random.randint(0, 100000)) % (65_535 - 10_000) + 10_000
+    except Exception:
+        return default
 
 
 def set_dist(
     rank: int,
     local_rank: int,
     world_size: int,
     local_world_size: int,
```

### Comparing `ml-starter-0.1.8/ml/utils/image.py` & `ml-starter-0.1.9/ml/utils/image.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/utils/io.py` & `ml-starter-0.1.9/ml/utils/io.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/utils/large_models.py` & `ml-starter-0.1.9/ml/utils/large_models.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/utils/logging.py` & `ml-starter-0.1.9/ml/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/utils/meter.py` & `ml-starter-0.1.9/ml/utils/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/utils/parallel.py` & `ml-starter-0.1.9/ml/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/utils/staging.py` & `ml-starter-0.1.9/ml/utils/staging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/utils/testing.py` & `ml-starter-0.1.9/ml/utils/testing.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/utils/timer.py` & `ml-starter-0.1.9/ml/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/utils/tokens.py` & `ml-starter-0.1.9/ml/utils/tokens.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/utils/torch_distributed.py` & `ml-starter-0.1.9/ml/utils/torch_distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/utils/triton/kmeans.py` & `ml-starter-0.1.9/ml/utils/triton/kmeans.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/utils/triton/lion.py` & `ml-starter-0.1.9/ml/utils/triton/lion.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml/utils/video.py` & `ml-starter-0.1.9/ml/utils/video.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/ml_starter.egg-info/PKG-INFO` & `ml-starter-0.1.9/ml_starter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.1.8
+Version: 0.1.9
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.1.8/ml_starter.egg-info/SOURCES.txt` & `ml-starter-0.1.9/ml_starter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/pyproject.toml` & `ml-starter-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.8/setup.py` & `ml-starter-0.1.9/setup.py`

 * *Files identical despite different names*

