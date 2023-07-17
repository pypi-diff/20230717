# Comparing `tmp/deprl-0.1.7.tar.gz` & `tmp/deprl-0.1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deprl-0.1.7.tar", max compression
+gzip compressed data, was "deprl-0.1.7.1.tar", max compression
```

## Comparing `deprl-0.1.7.tar` & `deprl-0.1.7.1.tar`

### file list

```diff
@@ -1,104 +1,104 @@
--rw-r--r--   0        0        0     1083 2023-06-24 08:15:25.085768 deprl-0.1.7/LICENSE
--rw-r--r--   0        0        0     8744 2023-07-17 20:54:31.856231 deprl-0.1.7/README.md
--rw-r--r--   0        0        0      563 2023-07-17 19:00:57.722034 deprl-0.1.7/deprl/__init__.py
--rw-r--r--   0        0        0     6481 2023-07-17 19:01:02.334145 deprl-0.1.7/deprl/custom_agents.py
--rw-r--r--   0        0        0     8956 2023-06-24 10:36:54.750864 deprl-0.1.7/deprl/custom_distributed.py
--rw-r--r--   0        0        0     3639 2023-04-27 12:08:50.580729 deprl-0.1.7/deprl/custom_mpo_torch.py
--rw-r--r--   0        0        0     3541 2023-07-17 19:00:57.722034 deprl-0.1.7/deprl/custom_test_environment.py
--rw-r--r--   0        0        0     1244 2023-04-27 12:08:50.580729 deprl-0.1.7/deprl/custom_torso.py
--rw-r--r--   0        0        0     5910 2023-07-17 19:48:36.494493 deprl-0.1.7/deprl/custom_trainer.py
--rw-r--r--   0        0        0     7373 2023-04-09 21:53:51.364949 deprl-0.1.7/deprl/dep_controller.py
--rw-r--r--   0        0        0      132 2023-06-24 12:25:57.343025 deprl-0.1.7/deprl/env_wrappers/__init__.py
--rw-r--r--   0        0        0     6471 2023-07-17 19:00:57.730034 deprl-0.1.7/deprl/env_wrappers/wrappers.py
--rw-r--r--   0        0        0     2175 2023-07-17 19:00:57.730034 deprl-0.1.7/deprl/log.py
--rw-r--r--   0        0        0     7722 2023-06-24 09:16:24.447868 deprl-0.1.7/deprl/main.py
--rw-r--r--   0        0        0      704 2023-06-24 12:25:57.351026 deprl-0.1.7/deprl/param_files/default_agents.json
--rw-r--r--   0        0        0     9156 2023-07-17 19:01:02.334145 deprl-0.1.7/deprl/play.py
--rw-r--r--   0        0        0    11578 2023-06-04 08:48:50.159176 deprl-0.1.7/deprl/play_plot.py
--rw-r--r--   0        0        0       80 2023-05-14 15:41:46.780895 deprl-0.1.7/deprl/plot.py
--rw-r--r--   0        0        0     9570 2023-06-05 17:53:13.795777 deprl-0.1.7/deprl/record_data_myoleg.py
--rw-r--r--   0        0        0     9458 2023-06-04 21:20:27.262283 deprl-0.1.7/deprl/record_video_myoleg.py
--rw-r--r--   0        0        0     8951 2023-07-12 16:45:11.388605 deprl-0.1.7/deprl/save_actor.py
--rw-r--r--   0        0        0     8754 2023-06-03 11:57:19.300487 deprl-0.1.7/deprl/time_play_baoding.py
--rw-r--r--   0        0        0      230 2023-07-17 19:00:57.734034 deprl-0.1.7/deprl/utils/__init__.py
--rw-r--r--   0        0        0     3053 2023-06-24 12:24:30.438761 deprl-0.1.7/deprl/utils/analysis_utils.py
--rw-r--r--   0        0        0     9582 2023-06-01 15:04:44.000000 deprl-0.1.7/deprl/utils/resources/exp_gait.zml
--rw-r--r--   0        0        0     6056 2023-07-17 19:27:01.013893 deprl-0.1.7/deprl/utils/utils.py
--rw-r--r--   0        0        0    16024 2023-06-04 09:09:44.415824 deprl-0.1.7/deprl/utils/utils_scone_gait_sto.py
--rw-r--r--   0        0        0       39 2023-04-27 12:08:50.580729 deprl-0.1.7/deprl/vendor/__init__.py
--rwxr-xr-x   0        0        0       80 2023-04-27 12:08:50.580729 deprl-0.1.7/deprl/vendor/tonic/.gitignore
--rw-r--r--   0        0        0     1110 2023-04-27 12:08:50.580729 deprl-0.1.7/deprl/vendor/tonic/LICENSE
--rw-r--r--   0        0        0      207 2023-04-27 12:08:50.580729 deprl-0.1.7/deprl/vendor/tonic/__init__.py
--rw-r--r--   0        0        0      178 2023-04-27 12:08:50.580729 deprl-0.1.7/deprl/vendor/tonic/agents/__init__.py
--rw-r--r--   0        0        0     1255 2023-07-17 19:01:02.334145 deprl-0.1.7/deprl/vendor/tonic/agents/agent.py
--rw-r--r--   0        0        0     3954 2023-04-27 12:08:50.580729 deprl-0.1.7/deprl/vendor/tonic/agents/basic.py
--rw-r--r--   0        0        0      293 2023-04-27 12:08:50.580729 deprl-0.1.7/deprl/vendor/tonic/environments/__init__.py
--rw-r--r--   0        0        0     5731 2023-07-17 19:48:36.094486 deprl-0.1.7/deprl/vendor/tonic/environments/builders.py
--rw-r--r--   0        0        0     6612 2023-04-27 12:08:50.580729 deprl-0.1.7/deprl/vendor/tonic/environments/distributed.py
--rw-r--r--   0        0        0     1914 2023-04-27 12:08:50.580729 deprl-0.1.7/deprl/vendor/tonic/environments/wrappers.py
--rw-r--r--   0        0        0      175 2023-04-27 12:08:50.584729 deprl-0.1.7/deprl/vendor/tonic/explorations/__init__.py
--rw-r--r--   0        0        0     2939 2023-04-27 12:08:50.584729 deprl-0.1.7/deprl/vendor/tonic/explorations/noisy.py
--rw-r--r--   0        0        0     8754 2023-04-27 12:08:50.584729 deprl-0.1.7/deprl/vendor/tonic/play.py
--rw-r--r--   0        0        0    18151 2023-05-14 15:41:47.404899 deprl-0.1.7/deprl/vendor/tonic/plot.py
--rw-r--r--   0        0        0      167 2023-04-27 12:08:50.584729 deprl-0.1.7/deprl/vendor/tonic/replays/__init__.py
--rw-r--r--   0        0        0     3636 2023-04-27 12:08:50.584729 deprl-0.1.7/deprl/vendor/tonic/replays/buffers.py
--rw-r--r--   0        0        0     2815 2023-04-27 12:08:50.584729 deprl-0.1.7/deprl/vendor/tonic/replays/segments.py
--rw-r--r--   0        0        0      821 2023-04-27 12:08:50.584729 deprl-0.1.7/deprl/vendor/tonic/replays/utils.py
--rw-r--r--   0        0        0      103 2023-04-27 12:08:50.584729 deprl-0.1.7/deprl/vendor/tonic/tensorflow/__init__.py
--rw-r--r--   0        0        0      303 2023-04-27 12:08:50.584729 deprl-0.1.7/deprl/vendor/tonic/tensorflow/agents/__init__.py
--rw-r--r--   0        0        0     4630 2023-04-27 12:08:50.584729 deprl-0.1.7/deprl/vendor/tonic/tensorflow/agents/a2c.py
--rw-r--r--   0        0        0      519 2023-04-27 12:08:50.584729 deprl-0.1.7/deprl/vendor/tonic/tensorflow/agents/agent.py
--rw-r--r--   0        0        0     1456 2023-04-27 12:08:50.584729 deprl-0.1.7/deprl/vendor/tonic/tensorflow/agents/d4pg.py
--rw-r--r--   0        0        0     4327 2023-04-27 12:08:50.584729 deprl-0.1.7/deprl/vendor/tonic/tensorflow/agents/ddpg.py
--rw-r--r--   0        0        0     4089 2023-04-27 12:08:50.584729 deprl-0.1.7/deprl/vendor/tonic/tensorflow/agents/mpo.py
--rw-r--r--   0        0        0     2452 2023-04-27 12:08:50.584729 deprl-0.1.7/deprl/vendor/tonic/tensorflow/agents/ppo.py
--rw-r--r--   0        0        0     1868 2023-04-27 12:08:50.584729 deprl-0.1.7/deprl/vendor/tonic/tensorflow/agents/sac.py
--rw-r--r--   0        0        0     2181 2023-04-27 12:08:50.584729 deprl-0.1.7/deprl/vendor/tonic/tensorflow/agents/td3.py
--rw-r--r--   0        0        0     1448 2023-04-27 12:08:50.584729 deprl-0.1.7/deprl/vendor/tonic/tensorflow/agents/td4.py
--rw-r--r--   0        0        0     3754 2023-04-27 12:08:50.584729 deprl-0.1.7/deprl/vendor/tonic/tensorflow/agents/trpo.py
--rw-r--r--   0        0        0      819 2023-04-27 12:08:50.584729 deprl-0.1.7/deprl/vendor/tonic/tensorflow/models/__init__.py
--rw-r--r--   0        0        0     6247 2023-04-27 12:08:50.584729 deprl-0.1.7/deprl/vendor/tonic/tensorflow/models/actor_critics.py
--rw-r--r--   0        0        0     4849 2023-04-27 12:08:50.584729 deprl-0.1.7/deprl/vendor/tonic/tensorflow/models/actors.py
--rw-r--r--   0        0        0     3046 2023-04-27 12:08:50.584729 deprl-0.1.7/deprl/vendor/tonic/tensorflow/models/critics.py
--rw-r--r--   0        0        0      734 2023-04-27 12:08:50.584729 deprl-0.1.7/deprl/vendor/tonic/tensorflow/models/encoders.py
--rw-r--r--   0        0        0      627 2023-04-27 12:08:50.584729 deprl-0.1.7/deprl/vendor/tonic/tensorflow/models/utils.py
--rw-r--r--   0        0        0       88 2023-04-27 12:08:50.584729 deprl-0.1.7/deprl/vendor/tonic/tensorflow/normalizers/__init__.py
--rw-r--r--   0        0        0     2442 2023-04-27 12:08:50.584729 deprl-0.1.7/deprl/vendor/tonic/tensorflow/normalizers/mean_stds.py
--rw-r--r--   0        0        0     1339 2023-04-27 12:08:50.584729 deprl-0.1.7/deprl/vendor/tonic/tensorflow/normalizers/returns.py
--rw-r--r--   0        0        0     1260 2023-04-27 12:08:50.588729 deprl-0.1.7/deprl/vendor/tonic/tensorflow/updaters/__init__.py
--rw-r--r--   0        0        0    19301 2023-04-27 12:08:50.588729 deprl-0.1.7/deprl/vendor/tonic/tensorflow/updaters/actors.py
--rw-r--r--   0        0        0    13820 2023-04-27 12:08:50.588729 deprl-0.1.7/deprl/vendor/tonic/tensorflow/updaters/critics.py
--rw-r--r--   0        0        0     4232 2023-04-27 12:08:50.588729 deprl-0.1.7/deprl/vendor/tonic/tensorflow/updaters/optimizers.py
--rw-r--r--   0        0        0      193 2023-04-27 12:08:50.588729 deprl-0.1.7/deprl/vendor/tonic/tensorflow/updaters/utils.py
--rw-r--r--   0        0        0      103 2023-04-27 12:08:50.588729 deprl-0.1.7/deprl/vendor/tonic/torch/__init__.py
--rw-r--r--   0        0        0      277 2023-04-27 12:08:50.588729 deprl-0.1.7/deprl/vendor/tonic/torch/agents/__init__.py
--rw-r--r--   0        0        0     5287 2023-04-27 12:08:50.588729 deprl-0.1.7/deprl/vendor/tonic/torch/agents/a2c.py
--rw-r--r--   0        0        0     1441 2023-05-14 15:41:46.528893 deprl-0.1.7/deprl/vendor/tonic/torch/agents/agent.py
--rw-r--r--   0        0        0     1522 2023-04-27 12:08:50.588729 deprl-0.1.7/deprl/vendor/tonic/torch/agents/d4pg.py
--rw-r--r--   0        0        0     4551 2023-04-27 12:08:50.588729 deprl-0.1.7/deprl/vendor/tonic/torch/agents/ddpg.py
--rw-r--r--   0        0        0     4446 2023-04-27 12:08:50.588729 deprl-0.1.7/deprl/vendor/tonic/torch/agents/mpo.py
--rw-r--r--   0        0        0     2608 2023-04-27 12:08:50.588729 deprl-0.1.7/deprl/vendor/tonic/torch/agents/ppo.py
--rw-r--r--   0        0        0     2102 2023-04-27 12:08:50.588729 deprl-0.1.7/deprl/vendor/tonic/torch/agents/sac.py
--rw-r--r--   0        0        0     2315 2023-04-27 12:08:50.588729 deprl-0.1.7/deprl/vendor/tonic/torch/agents/td3.py
--rw-r--r--   0        0        0     4077 2023-04-27 12:08:50.588729 deprl-0.1.7/deprl/vendor/tonic/torch/agents/trpo.py
--rw-r--r--   0        0        0      817 2023-04-27 12:08:50.588729 deprl-0.1.7/deprl/vendor/tonic/torch/models/__init__.py
--rw-r--r--   0        0        0     5824 2023-04-27 12:08:50.588729 deprl-0.1.7/deprl/vendor/tonic/torch/models/actor_critics.py
--rw-r--r--   0        0        0     4874 2023-04-27 12:08:50.588729 deprl-0.1.7/deprl/vendor/tonic/torch/models/actors.py
--rw-r--r--   0        0        0     3177 2023-04-27 12:08:50.588729 deprl-0.1.7/deprl/vendor/tonic/torch/models/critics.py
--rw-r--r--   0        0        0     1084 2023-04-27 12:08:50.588729 deprl-0.1.7/deprl/vendor/tonic/torch/models/encoders.py
--rw-r--r--   0        0        0      791 2023-04-27 12:08:50.588729 deprl-0.1.7/deprl/vendor/tonic/torch/models/utils.py
--rw-r--r--   0        0        0       88 2023-04-27 12:08:50.588729 deprl-0.1.7/deprl/vendor/tonic/torch/normalizers/__init__.py
--rw-r--r--   0        0        0     2615 2023-04-27 12:08:50.588729 deprl-0.1.7/deprl/vendor/tonic/torch/normalizers/mean_stds.py
--rw-r--r--   0        0        0     1429 2023-04-27 12:08:50.588729 deprl-0.1.7/deprl/vendor/tonic/torch/normalizers/returns.py
--rw-r--r--   0        0        0     1156 2023-04-27 12:08:50.588729 deprl-0.1.7/deprl/vendor/tonic/torch/updaters/__init__.py
--rw-r--r--   0        0        0    20504 2023-04-27 12:08:50.588729 deprl-0.1.7/deprl/vendor/tonic/torch/updaters/actors.py
--rw-r--r--   0        0        0    11054 2023-04-27 12:08:50.588729 deprl-0.1.7/deprl/vendor/tonic/torch/updaters/critics.py
--rw-r--r--   0        0        0     4317 2023-04-27 12:08:50.588729 deprl-0.1.7/deprl/vendor/tonic/torch/updaters/optimizers.py
--rw-r--r--   0        0        0      156 2023-04-27 12:08:50.588729 deprl-0.1.7/deprl/vendor/tonic/torch/updaters/utils.py
--rw-r--r--   0        0        0     5722 2023-04-27 12:08:50.588729 deprl-0.1.7/deprl/vendor/tonic/train.py
--rw-r--r--   0        0        0      213 2023-04-27 12:08:50.588729 deprl-0.1.7/deprl/vendor/tonic/utils/__init__.py
--rw-r--r--   0        0        0      822 2023-04-27 12:08:50.588729 deprl-0.1.7/deprl/vendor/tonic/utils/csv_utils.py
--rw-r--r--   0        0        0     8867 2023-04-27 12:08:50.588729 deprl-0.1.7/deprl/vendor/tonic/utils/logger.py
--rw-r--r--   0        0        0     5477 2023-04-27 12:08:50.588729 deprl-0.1.7/deprl/vendor/tonic/utils/trainer.py
--rw-r--r--   0        0        0     1227 2023-07-17 21:01:36.202885 deprl-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     9650 1970-01-01 00:00:00.000000 deprl-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-06-24 08:15:25.085768 deprl-0.1.7.1/LICENSE
+-rw-r--r--   0        0        0     8744 2023-07-17 20:54:31.856231 deprl-0.1.7.1/README.md
+-rw-r--r--   0        0        0      563 2023-07-17 19:00:57.722034 deprl-0.1.7.1/deprl/__init__.py
+-rw-r--r--   0        0        0     6481 2023-07-17 19:01:02.334145 deprl-0.1.7.1/deprl/custom_agents.py
+-rw-r--r--   0        0        0     8956 2023-06-24 10:36:54.750864 deprl-0.1.7.1/deprl/custom_distributed.py
+-rw-r--r--   0        0        0     3639 2023-04-27 12:08:50.580729 deprl-0.1.7.1/deprl/custom_mpo_torch.py
+-rw-r--r--   0        0        0     3541 2023-07-17 19:00:57.722034 deprl-0.1.7.1/deprl/custom_test_environment.py
+-rw-r--r--   0        0        0     1244 2023-04-27 12:08:50.580729 deprl-0.1.7.1/deprl/custom_torso.py
+-rw-r--r--   0        0        0     5910 2023-07-17 19:48:36.494493 deprl-0.1.7.1/deprl/custom_trainer.py
+-rw-r--r--   0        0        0     7373 2023-04-09 21:53:51.364949 deprl-0.1.7.1/deprl/dep_controller.py
+-rw-r--r--   0        0        0      132 2023-06-24 12:25:57.343025 deprl-0.1.7.1/deprl/env_wrappers/__init__.py
+-rw-r--r--   0        0        0     6471 2023-07-17 19:00:57.730034 deprl-0.1.7.1/deprl/env_wrappers/wrappers.py
+-rw-r--r--   0        0        0     2175 2023-07-17 19:00:57.730034 deprl-0.1.7.1/deprl/log.py
+-rw-r--r--   0        0        0     7722 2023-06-24 09:16:24.447868 deprl-0.1.7.1/deprl/main.py
+-rw-r--r--   0        0        0      704 2023-06-24 12:25:57.351026 deprl-0.1.7.1/deprl/param_files/default_agents.json
+-rw-r--r--   0        0        0     9156 2023-07-17 19:01:02.334145 deprl-0.1.7.1/deprl/play.py
+-rw-r--r--   0        0        0    11578 2023-06-04 08:48:50.159176 deprl-0.1.7.1/deprl/play_plot.py
+-rw-r--r--   0        0        0       80 2023-05-14 15:41:46.780895 deprl-0.1.7.1/deprl/plot.py
+-rw-r--r--   0        0        0     9570 2023-06-05 17:53:13.795777 deprl-0.1.7.1/deprl/record_data_myoleg.py
+-rw-r--r--   0        0        0     9458 2023-06-04 21:20:27.262283 deprl-0.1.7.1/deprl/record_video_myoleg.py
+-rw-r--r--   0        0        0     8951 2023-07-12 16:45:11.388605 deprl-0.1.7.1/deprl/save_actor.py
+-rw-r--r--   0        0        0     8754 2023-06-03 11:57:19.300487 deprl-0.1.7.1/deprl/time_play_baoding.py
+-rw-r--r--   0        0        0      230 2023-07-17 19:00:57.734034 deprl-0.1.7.1/deprl/utils/__init__.py
+-rw-r--r--   0        0        0     3053 2023-06-24 12:24:30.438761 deprl-0.1.7.1/deprl/utils/analysis_utils.py
+-rw-r--r--   0        0        0     9582 2023-06-01 15:04:44.000000 deprl-0.1.7.1/deprl/utils/resources/exp_gait.zml
+-rw-r--r--   0        0        0     6188 2023-07-17 21:32:46.311048 deprl-0.1.7.1/deprl/utils/utils.py
+-rw-r--r--   0        0        0    16024 2023-06-04 09:09:44.415824 deprl-0.1.7.1/deprl/utils/utils_scone_gait_sto.py
+-rw-r--r--   0        0        0       39 2023-04-27 12:08:50.580729 deprl-0.1.7.1/deprl/vendor/__init__.py
+-rwxr-xr-x   0        0        0       80 2023-04-27 12:08:50.580729 deprl-0.1.7.1/deprl/vendor/tonic/.gitignore
+-rw-r--r--   0        0        0     1110 2023-04-27 12:08:50.580729 deprl-0.1.7.1/deprl/vendor/tonic/LICENSE
+-rw-r--r--   0        0        0      207 2023-04-27 12:08:50.580729 deprl-0.1.7.1/deprl/vendor/tonic/__init__.py
+-rw-r--r--   0        0        0      178 2023-04-27 12:08:50.580729 deprl-0.1.7.1/deprl/vendor/tonic/agents/__init__.py
+-rw-r--r--   0        0        0     1255 2023-07-17 19:01:02.334145 deprl-0.1.7.1/deprl/vendor/tonic/agents/agent.py
+-rw-r--r--   0        0        0     3954 2023-04-27 12:08:50.580729 deprl-0.1.7.1/deprl/vendor/tonic/agents/basic.py
+-rw-r--r--   0        0        0      293 2023-04-27 12:08:50.580729 deprl-0.1.7.1/deprl/vendor/tonic/environments/__init__.py
+-rw-r--r--   0        0        0     5731 2023-07-17 19:48:36.094486 deprl-0.1.7.1/deprl/vendor/tonic/environments/builders.py
+-rw-r--r--   0        0        0     6612 2023-04-27 12:08:50.580729 deprl-0.1.7.1/deprl/vendor/tonic/environments/distributed.py
+-rw-r--r--   0        0        0     1914 2023-04-27 12:08:50.580729 deprl-0.1.7.1/deprl/vendor/tonic/environments/wrappers.py
+-rw-r--r--   0        0        0      175 2023-04-27 12:08:50.584729 deprl-0.1.7.1/deprl/vendor/tonic/explorations/__init__.py
+-rw-r--r--   0        0        0     2939 2023-04-27 12:08:50.584729 deprl-0.1.7.1/deprl/vendor/tonic/explorations/noisy.py
+-rw-r--r--   0        0        0     8754 2023-04-27 12:08:50.584729 deprl-0.1.7.1/deprl/vendor/tonic/play.py
+-rw-r--r--   0        0        0    18151 2023-05-14 15:41:47.404899 deprl-0.1.7.1/deprl/vendor/tonic/plot.py
+-rw-r--r--   0        0        0      167 2023-04-27 12:08:50.584729 deprl-0.1.7.1/deprl/vendor/tonic/replays/__init__.py
+-rw-r--r--   0        0        0     3636 2023-04-27 12:08:50.584729 deprl-0.1.7.1/deprl/vendor/tonic/replays/buffers.py
+-rw-r--r--   0        0        0     2815 2023-04-27 12:08:50.584729 deprl-0.1.7.1/deprl/vendor/tonic/replays/segments.py
+-rw-r--r--   0        0        0      821 2023-04-27 12:08:50.584729 deprl-0.1.7.1/deprl/vendor/tonic/replays/utils.py
+-rw-r--r--   0        0        0      103 2023-04-27 12:08:50.584729 deprl-0.1.7.1/deprl/vendor/tonic/tensorflow/__init__.py
+-rw-r--r--   0        0        0      303 2023-04-27 12:08:50.584729 deprl-0.1.7.1/deprl/vendor/tonic/tensorflow/agents/__init__.py
+-rw-r--r--   0        0        0     4630 2023-04-27 12:08:50.584729 deprl-0.1.7.1/deprl/vendor/tonic/tensorflow/agents/a2c.py
+-rw-r--r--   0        0        0      519 2023-04-27 12:08:50.584729 deprl-0.1.7.1/deprl/vendor/tonic/tensorflow/agents/agent.py
+-rw-r--r--   0        0        0     1456 2023-04-27 12:08:50.584729 deprl-0.1.7.1/deprl/vendor/tonic/tensorflow/agents/d4pg.py
+-rw-r--r--   0        0        0     4327 2023-04-27 12:08:50.584729 deprl-0.1.7.1/deprl/vendor/tonic/tensorflow/agents/ddpg.py
+-rw-r--r--   0        0        0     4089 2023-04-27 12:08:50.584729 deprl-0.1.7.1/deprl/vendor/tonic/tensorflow/agents/mpo.py
+-rw-r--r--   0        0        0     2452 2023-04-27 12:08:50.584729 deprl-0.1.7.1/deprl/vendor/tonic/tensorflow/agents/ppo.py
+-rw-r--r--   0        0        0     1868 2023-04-27 12:08:50.584729 deprl-0.1.7.1/deprl/vendor/tonic/tensorflow/agents/sac.py
+-rw-r--r--   0        0        0     2181 2023-04-27 12:08:50.584729 deprl-0.1.7.1/deprl/vendor/tonic/tensorflow/agents/td3.py
+-rw-r--r--   0        0        0     1448 2023-04-27 12:08:50.584729 deprl-0.1.7.1/deprl/vendor/tonic/tensorflow/agents/td4.py
+-rw-r--r--   0        0        0     3754 2023-04-27 12:08:50.584729 deprl-0.1.7.1/deprl/vendor/tonic/tensorflow/agents/trpo.py
+-rw-r--r--   0        0        0      819 2023-04-27 12:08:50.584729 deprl-0.1.7.1/deprl/vendor/tonic/tensorflow/models/__init__.py
+-rw-r--r--   0        0        0     6247 2023-04-27 12:08:50.584729 deprl-0.1.7.1/deprl/vendor/tonic/tensorflow/models/actor_critics.py
+-rw-r--r--   0        0        0     4849 2023-04-27 12:08:50.584729 deprl-0.1.7.1/deprl/vendor/tonic/tensorflow/models/actors.py
+-rw-r--r--   0        0        0     3046 2023-04-27 12:08:50.584729 deprl-0.1.7.1/deprl/vendor/tonic/tensorflow/models/critics.py
+-rw-r--r--   0        0        0      734 2023-04-27 12:08:50.584729 deprl-0.1.7.1/deprl/vendor/tonic/tensorflow/models/encoders.py
+-rw-r--r--   0        0        0      627 2023-04-27 12:08:50.584729 deprl-0.1.7.1/deprl/vendor/tonic/tensorflow/models/utils.py
+-rw-r--r--   0        0        0       88 2023-04-27 12:08:50.584729 deprl-0.1.7.1/deprl/vendor/tonic/tensorflow/normalizers/__init__.py
+-rw-r--r--   0        0        0     2442 2023-04-27 12:08:50.584729 deprl-0.1.7.1/deprl/vendor/tonic/tensorflow/normalizers/mean_stds.py
+-rw-r--r--   0        0        0     1339 2023-04-27 12:08:50.584729 deprl-0.1.7.1/deprl/vendor/tonic/tensorflow/normalizers/returns.py
+-rw-r--r--   0        0        0     1260 2023-04-27 12:08:50.588729 deprl-0.1.7.1/deprl/vendor/tonic/tensorflow/updaters/__init__.py
+-rw-r--r--   0        0        0    19301 2023-04-27 12:08:50.588729 deprl-0.1.7.1/deprl/vendor/tonic/tensorflow/updaters/actors.py
+-rw-r--r--   0        0        0    13820 2023-04-27 12:08:50.588729 deprl-0.1.7.1/deprl/vendor/tonic/tensorflow/updaters/critics.py
+-rw-r--r--   0        0        0     4232 2023-04-27 12:08:50.588729 deprl-0.1.7.1/deprl/vendor/tonic/tensorflow/updaters/optimizers.py
+-rw-r--r--   0        0        0      193 2023-04-27 12:08:50.588729 deprl-0.1.7.1/deprl/vendor/tonic/tensorflow/updaters/utils.py
+-rw-r--r--   0        0        0      103 2023-04-27 12:08:50.588729 deprl-0.1.7.1/deprl/vendor/tonic/torch/__init__.py
+-rw-r--r--   0        0        0      277 2023-04-27 12:08:50.588729 deprl-0.1.7.1/deprl/vendor/tonic/torch/agents/__init__.py
+-rw-r--r--   0        0        0     5287 2023-04-27 12:08:50.588729 deprl-0.1.7.1/deprl/vendor/tonic/torch/agents/a2c.py
+-rw-r--r--   0        0        0     1441 2023-05-14 15:41:46.528893 deprl-0.1.7.1/deprl/vendor/tonic/torch/agents/agent.py
+-rw-r--r--   0        0        0     1522 2023-04-27 12:08:50.588729 deprl-0.1.7.1/deprl/vendor/tonic/torch/agents/d4pg.py
+-rw-r--r--   0        0        0     4551 2023-04-27 12:08:50.588729 deprl-0.1.7.1/deprl/vendor/tonic/torch/agents/ddpg.py
+-rw-r--r--   0        0        0     4446 2023-04-27 12:08:50.588729 deprl-0.1.7.1/deprl/vendor/tonic/torch/agents/mpo.py
+-rw-r--r--   0        0        0     2608 2023-04-27 12:08:50.588729 deprl-0.1.7.1/deprl/vendor/tonic/torch/agents/ppo.py
+-rw-r--r--   0        0        0     2102 2023-04-27 12:08:50.588729 deprl-0.1.7.1/deprl/vendor/tonic/torch/agents/sac.py
+-rw-r--r--   0        0        0     2315 2023-04-27 12:08:50.588729 deprl-0.1.7.1/deprl/vendor/tonic/torch/agents/td3.py
+-rw-r--r--   0        0        0     4077 2023-04-27 12:08:50.588729 deprl-0.1.7.1/deprl/vendor/tonic/torch/agents/trpo.py
+-rw-r--r--   0        0        0      817 2023-04-27 12:08:50.588729 deprl-0.1.7.1/deprl/vendor/tonic/torch/models/__init__.py
+-rw-r--r--   0        0        0     5824 2023-04-27 12:08:50.588729 deprl-0.1.7.1/deprl/vendor/tonic/torch/models/actor_critics.py
+-rw-r--r--   0        0        0     4874 2023-04-27 12:08:50.588729 deprl-0.1.7.1/deprl/vendor/tonic/torch/models/actors.py
+-rw-r--r--   0        0        0     3177 2023-04-27 12:08:50.588729 deprl-0.1.7.1/deprl/vendor/tonic/torch/models/critics.py
+-rw-r--r--   0        0        0     1084 2023-04-27 12:08:50.588729 deprl-0.1.7.1/deprl/vendor/tonic/torch/models/encoders.py
+-rw-r--r--   0        0        0      791 2023-04-27 12:08:50.588729 deprl-0.1.7.1/deprl/vendor/tonic/torch/models/utils.py
+-rw-r--r--   0        0        0       88 2023-04-27 12:08:50.588729 deprl-0.1.7.1/deprl/vendor/tonic/torch/normalizers/__init__.py
+-rw-r--r--   0        0        0     2615 2023-04-27 12:08:50.588729 deprl-0.1.7.1/deprl/vendor/tonic/torch/normalizers/mean_stds.py
+-rw-r--r--   0        0        0     1429 2023-04-27 12:08:50.588729 deprl-0.1.7.1/deprl/vendor/tonic/torch/normalizers/returns.py
+-rw-r--r--   0        0        0     1156 2023-04-27 12:08:50.588729 deprl-0.1.7.1/deprl/vendor/tonic/torch/updaters/__init__.py
+-rw-r--r--   0        0        0    20504 2023-04-27 12:08:50.588729 deprl-0.1.7.1/deprl/vendor/tonic/torch/updaters/actors.py
+-rw-r--r--   0        0        0    11054 2023-04-27 12:08:50.588729 deprl-0.1.7.1/deprl/vendor/tonic/torch/updaters/critics.py
+-rw-r--r--   0        0        0     4317 2023-04-27 12:08:50.588729 deprl-0.1.7.1/deprl/vendor/tonic/torch/updaters/optimizers.py
+-rw-r--r--   0        0        0      156 2023-04-27 12:08:50.588729 deprl-0.1.7.1/deprl/vendor/tonic/torch/updaters/utils.py
+-rw-r--r--   0        0        0     5722 2023-04-27 12:08:50.588729 deprl-0.1.7.1/deprl/vendor/tonic/train.py
+-rw-r--r--   0        0        0      213 2023-04-27 12:08:50.588729 deprl-0.1.7.1/deprl/vendor/tonic/utils/__init__.py
+-rw-r--r--   0        0        0      822 2023-04-27 12:08:50.588729 deprl-0.1.7.1/deprl/vendor/tonic/utils/csv_utils.py
+-rw-r--r--   0        0        0     8867 2023-04-27 12:08:50.588729 deprl-0.1.7.1/deprl/vendor/tonic/utils/logger.py
+-rw-r--r--   0        0        0     5477 2023-04-27 12:08:50.588729 deprl-0.1.7.1/deprl/vendor/tonic/utils/trainer.py
+-rw-r--r--   0        0        0     1214 2023-07-17 21:38:16.002031 deprl-0.1.7.1/pyproject.toml
+-rw-r--r--   0        0        0     9614 1970-01-01 00:00:00.000000 deprl-0.1.7.1/PKG-INFO
```

### Comparing `deprl-0.1.7/LICENSE` & `deprl-0.1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/README.md` & `deprl-0.1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/__init__.py` & `deprl-0.1.7.1/deprl/__init__.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/custom_agents.py` & `deprl-0.1.7.1/deprl/custom_agents.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/custom_distributed.py` & `deprl-0.1.7.1/deprl/custom_distributed.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/custom_mpo_torch.py` & `deprl-0.1.7.1/deprl/custom_mpo_torch.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/custom_test_environment.py` & `deprl-0.1.7.1/deprl/custom_test_environment.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/custom_torso.py` & `deprl-0.1.7.1/deprl/custom_torso.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/custom_trainer.py` & `deprl-0.1.7.1/deprl/custom_trainer.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/dep_controller.py` & `deprl-0.1.7.1/deprl/dep_controller.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/env_wrappers/wrappers.py` & `deprl-0.1.7.1/deprl/env_wrappers/wrappers.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/log.py` & `deprl-0.1.7.1/deprl/log.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/main.py` & `deprl-0.1.7.1/deprl/main.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/param_files/default_agents.json` & `deprl-0.1.7.1/deprl/param_files/default_agents.json`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/play.py` & `deprl-0.1.7.1/deprl/play.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/play_plot.py` & `deprl-0.1.7.1/deprl/play_plot.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/record_data_myoleg.py` & `deprl-0.1.7.1/deprl/record_data_myoleg.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/record_video_myoleg.py` & `deprl-0.1.7.1/deprl/record_video_myoleg.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/save_actor.py` & `deprl-0.1.7.1/deprl/save_actor.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/time_play_baoding.py` & `deprl-0.1.7.1/deprl/time_play_baoding.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/utils/analysis_utils.py` & `deprl-0.1.7.1/deprl/utils/analysis_utils.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/utils/resources/exp_gait.zml` & `deprl-0.1.7.1/deprl/utils/resources/exp_gait.zml`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/utils/utils.py` & `deprl-0.1.7.1/deprl/utils/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,21 +51,27 @@
     # Load the weights of the agent form a checkpoint.
     agent.load(checkpoint_path)
     agent.noisy = noisy
     return agent
 
 
 def load_baseline(environment):
-    if "myoLegWalk" in str(environment):
+    identifier = (
+        environment.env_name
+        if hasattr(environment, "env_name")
+        else str(environment)
+    )
+    print(identifier)
+    if "myoLegWalk" in identifier:
         logger.log("Load LegWalk Baseline")
         return load_baseline_myolegwalk(environment)
-    if "myoChallengeChaseTagP1" in str(environment):
+    if "myoChallengeChaseTagP1" in identifier:
         logger.log("Load ChaseTagP1 Baseline")
         return load_baseline_myochasetagp1(environment, noisy=True)
-    if "myoChallengeRelocateP1" in str(environment):
+    if "myoChallengeRelocateP1" in identifier:
         logger.log("Load RelocateP1 Baseline")
         return load_baseline_myorelocatep1(environment)
 
 
 def load_baseline_myolegwalk(environment, noisy=False):
     modelurl = (
         "https://drive.google.com/uc?id=1UkiUozk-PM8JbQCZNoy2Jr2t1StLcAzx"
```

### Comparing `deprl-0.1.7/deprl/utils/utils_scone_gait_sto.py` & `deprl-0.1.7.1/deprl/utils/utils_scone_gait_sto.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/LICENSE` & `deprl-0.1.7.1/deprl/vendor/tonic/LICENSE`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/agents/agent.py` & `deprl-0.1.7.1/deprl/vendor/tonic/agents/agent.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/agents/basic.py` & `deprl-0.1.7.1/deprl/vendor/tonic/agents/basic.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/environments/builders.py` & `deprl-0.1.7.1/deprl/vendor/tonic/environments/builders.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/environments/distributed.py` & `deprl-0.1.7.1/deprl/vendor/tonic/environments/distributed.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/environments/wrappers.py` & `deprl-0.1.7.1/deprl/vendor/tonic/environments/wrappers.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/explorations/noisy.py` & `deprl-0.1.7.1/deprl/vendor/tonic/explorations/noisy.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/play.py` & `deprl-0.1.7.1/deprl/vendor/tonic/play.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/plot.py` & `deprl-0.1.7.1/deprl/vendor/tonic/plot.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/replays/buffers.py` & `deprl-0.1.7.1/deprl/vendor/tonic/replays/buffers.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/replays/segments.py` & `deprl-0.1.7.1/deprl/vendor/tonic/replays/segments.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/replays/utils.py` & `deprl-0.1.7.1/deprl/vendor/tonic/replays/utils.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/tensorflow/agents/a2c.py` & `deprl-0.1.7.1/deprl/vendor/tonic/tensorflow/agents/a2c.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/tensorflow/agents/agent.py` & `deprl-0.1.7.1/deprl/vendor/tonic/tensorflow/agents/agent.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/tensorflow/agents/d4pg.py` & `deprl-0.1.7.1/deprl/vendor/tonic/tensorflow/agents/d4pg.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/tensorflow/agents/ddpg.py` & `deprl-0.1.7.1/deprl/vendor/tonic/tensorflow/agents/ddpg.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/tensorflow/agents/mpo.py` & `deprl-0.1.7.1/deprl/vendor/tonic/tensorflow/agents/mpo.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/tensorflow/agents/ppo.py` & `deprl-0.1.7.1/deprl/vendor/tonic/tensorflow/agents/ppo.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/tensorflow/agents/sac.py` & `deprl-0.1.7.1/deprl/vendor/tonic/tensorflow/agents/sac.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/tensorflow/agents/td3.py` & `deprl-0.1.7.1/deprl/vendor/tonic/tensorflow/agents/td3.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/tensorflow/agents/td4.py` & `deprl-0.1.7.1/deprl/vendor/tonic/tensorflow/agents/td4.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/tensorflow/agents/trpo.py` & `deprl-0.1.7.1/deprl/vendor/tonic/tensorflow/agents/trpo.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/tensorflow/models/__init__.py` & `deprl-0.1.7.1/deprl/vendor/tonic/tensorflow/models/__init__.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/tensorflow/models/actor_critics.py` & `deprl-0.1.7.1/deprl/vendor/tonic/tensorflow/models/actor_critics.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/tensorflow/models/actors.py` & `deprl-0.1.7.1/deprl/vendor/tonic/tensorflow/models/actors.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/tensorflow/models/critics.py` & `deprl-0.1.7.1/deprl/vendor/tonic/tensorflow/models/critics.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/tensorflow/models/encoders.py` & `deprl-0.1.7.1/deprl/vendor/tonic/tensorflow/models/encoders.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/tensorflow/models/utils.py` & `deprl-0.1.7.1/deprl/vendor/tonic/tensorflow/models/utils.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/tensorflow/normalizers/mean_stds.py` & `deprl-0.1.7.1/deprl/vendor/tonic/tensorflow/normalizers/mean_stds.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/tensorflow/normalizers/returns.py` & `deprl-0.1.7.1/deprl/vendor/tonic/tensorflow/normalizers/returns.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/tensorflow/updaters/__init__.py` & `deprl-0.1.7.1/deprl/vendor/tonic/tensorflow/updaters/__init__.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/tensorflow/updaters/actors.py` & `deprl-0.1.7.1/deprl/vendor/tonic/tensorflow/updaters/actors.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/tensorflow/updaters/critics.py` & `deprl-0.1.7.1/deprl/vendor/tonic/tensorflow/updaters/critics.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/tensorflow/updaters/optimizers.py` & `deprl-0.1.7.1/deprl/vendor/tonic/tensorflow/updaters/optimizers.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/torch/agents/a2c.py` & `deprl-0.1.7.1/deprl/vendor/tonic/torch/agents/a2c.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/torch/agents/agent.py` & `deprl-0.1.7.1/deprl/vendor/tonic/torch/agents/agent.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/torch/agents/d4pg.py` & `deprl-0.1.7.1/deprl/vendor/tonic/torch/agents/d4pg.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/torch/agents/ddpg.py` & `deprl-0.1.7.1/deprl/vendor/tonic/torch/agents/ddpg.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/torch/agents/mpo.py` & `deprl-0.1.7.1/deprl/vendor/tonic/torch/agents/mpo.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/torch/agents/ppo.py` & `deprl-0.1.7.1/deprl/vendor/tonic/torch/agents/ppo.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/torch/agents/sac.py` & `deprl-0.1.7.1/deprl/vendor/tonic/torch/agents/sac.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/torch/agents/td3.py` & `deprl-0.1.7.1/deprl/vendor/tonic/torch/agents/td3.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/torch/agents/trpo.py` & `deprl-0.1.7.1/deprl/vendor/tonic/torch/agents/trpo.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/torch/models/__init__.py` & `deprl-0.1.7.1/deprl/vendor/tonic/torch/models/__init__.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/torch/models/actor_critics.py` & `deprl-0.1.7.1/deprl/vendor/tonic/torch/models/actor_critics.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/torch/models/actors.py` & `deprl-0.1.7.1/deprl/vendor/tonic/torch/models/actors.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/torch/models/critics.py` & `deprl-0.1.7.1/deprl/vendor/tonic/torch/models/critics.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/torch/models/encoders.py` & `deprl-0.1.7.1/deprl/vendor/tonic/torch/models/encoders.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/torch/models/utils.py` & `deprl-0.1.7.1/deprl/vendor/tonic/torch/models/utils.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/torch/normalizers/mean_stds.py` & `deprl-0.1.7.1/deprl/vendor/tonic/torch/normalizers/mean_stds.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/torch/normalizers/returns.py` & `deprl-0.1.7.1/deprl/vendor/tonic/torch/normalizers/returns.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/torch/updaters/__init__.py` & `deprl-0.1.7.1/deprl/vendor/tonic/torch/updaters/__init__.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/torch/updaters/actors.py` & `deprl-0.1.7.1/deprl/vendor/tonic/torch/updaters/actors.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/torch/updaters/critics.py` & `deprl-0.1.7.1/deprl/vendor/tonic/torch/updaters/critics.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/torch/updaters/optimizers.py` & `deprl-0.1.7.1/deprl/vendor/tonic/torch/updaters/optimizers.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/train.py` & `deprl-0.1.7.1/deprl/vendor/tonic/train.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/utils/csv_utils.py` & `deprl-0.1.7.1/deprl/vendor/tonic/utils/csv_utils.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/utils/logger.py` & `deprl-0.1.7.1/deprl/vendor/tonic/utils/logger.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/deprl/vendor/tonic/utils/trainer.py` & `deprl-0.1.7.1/deprl/vendor/tonic/utils/trainer.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.7/pyproject.toml` & `deprl-0.1.7.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deprl"
-version = "0.1.7"
+version = "0.1.7.001"
 description = "DEP-RL, a method for robust control of musculoskeletal systems."
 authors = ["Pierre Schumacher <pierre.schumacher@tuebingen.mpg.de>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
@@ -13,15 +13,14 @@
 termcolor = "^2.2.0"
 jaxlib = "^0.4.7"
 jax = "^0.4.8"
 pandas = "^2.0.1"
 gdown = "^4.7.1"
 gym = "0.13.0"
 pytest = "^7.4.0"
-torch = "^2.0.1"
 
 [tool.poetry.group.dev.dependencies]
 pudb = "*"
 pre-commit = "*"
 wandb = "^0.13.11"
 ostrichrl = {git = "https://github.com/P-Schumacher/ostrichrl.git", branch="fix/setuptools"}
 warmup = {git = "https://github.com/P-Schumacher/warmup.git"}
```

### Comparing `deprl-0.1.7/PKG-INFO` & `deprl-0.1.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deprl
-Version: 0.1.7
+Version: 0.1.7.1
 Summary: DEP-RL, a method for robust control of musculoskeletal systems.
 License: MIT
 Author: Pierre Schumacher
 Author-email: pierre.schumacher@tuebingen.mpg.de
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -16,15 +16,14 @@
 Requires-Dist: jax (>=0.4.8,<0.5.0)
 Requires-Dist: jaxlib (>=0.4.7,<0.5.0)
 Requires-Dist: numpy (>=1.22.4,<2.0.0)
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: pytest (>=7.4.0,<8.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: termcolor (>=2.2.0,<3.0.0)
-Requires-Dist: torch (>=2.0.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # DEP-RL: Embodied Exploration for Reinforcement Learning in Overactuated and Musculoskeletal Systems
  [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
  [![PyPI](https://img.shields.io/pypi/v/deprl)](https://pypi.org/project/deprl/)
  [![Downloads](https://pepy.tech/badge/deprl)](https://pepy.tech/project/deprl)
```

