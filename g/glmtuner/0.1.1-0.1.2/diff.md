# Comparing `tmp/glmtuner-0.1.1.tar.gz` & `tmp/glmtuner-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glmtuner-0.1.1.tar", last modified: Sat Jul 15 16:54:28 2023, max compression
+gzip compressed data, was "glmtuner-0.1.2.tar", last modified: Mon Jul 17 15:15:02 2023, max compression
```

## Comparing `glmtuner-0.1.1.tar` & `glmtuner-0.1.2.tar`

### file list

```diff
@@ -1,82 +1,85 @@
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 16:54:28.926215 glmtuner-0.1.1/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    11524 2023-07-15 16:54:23.000000 glmtuner-0.1.1/LICENSE
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    18438 2023-07-15 16:54:28.926215 glmtuner-0.1.1/PKG-INFO
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    17854 2023-07-15 16:54:23.000000 glmtuner-0.1.1/README.md
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       87 2023-07-15 16:54:23.000000 glmtuner-0.1.1/pyproject.toml
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       38 2023-07-15 16:54:28.930215 glmtuner-0.1.1/setup.cfg
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2006 2023-07-15 16:54:23.000000 glmtuner-0.1.1/setup.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 16:54:27.802214 glmtuner-0.1.1/src/
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 16:54:27.854214 glmtuner-0.1.1/src/glmtuner/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      250 2023-07-15 16:54:21.000000 glmtuner-0.1.1/src/glmtuner/__init__.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 16:54:27.866213 glmtuner-0.1.1/src/glmtuner/api/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       41 2023-07-15 16:54:18.000000 glmtuner-0.1.1/src/glmtuner/api/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4515 2023-07-15 16:54:18.000000 glmtuner-0.1.1/src/glmtuner/api/app.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2053 2023-07-15 16:54:18.000000 glmtuner-0.1.1/src/glmtuner/api/protocol.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 16:54:27.870214 glmtuner-0.1.1/src/glmtuner/chat/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       49 2023-07-15 16:54:19.000000 glmtuner-0.1.1/src/glmtuner/chat/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2948 2023-07-15 16:54:18.000000 glmtuner-0.1.1/src/glmtuner/chat/stream_chat.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 16:54:27.878214 glmtuner-0.1.1/src/glmtuner/dsets/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      165 2023-07-15 16:54:19.000000 glmtuner-0.1.1/src/glmtuner/dsets/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     6589 2023-07-15 16:54:19.000000 glmtuner-0.1.1/src/glmtuner/dsets/collator.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4249 2023-07-15 16:54:19.000000 glmtuner-0.1.1/src/glmtuner/dsets/loader.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     7475 2023-07-15 16:54:19.000000 glmtuner-0.1.1/src/glmtuner/dsets/preprocess.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 16:54:27.986214 glmtuner-0.1.1/src/glmtuner/extras/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 16:54:19.000000 glmtuner-0.1.1/src/glmtuner/extras/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3000 2023-07-15 16:54:19.000000 glmtuner-0.1.1/src/glmtuner/extras/callbacks.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      312 2023-07-15 16:54:19.000000 glmtuner-0.1.1/src/glmtuner/extras/constants.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      751 2023-07-15 16:54:19.000000 glmtuner-0.1.1/src/glmtuner/extras/logging.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     5062 2023-07-15 16:54:19.000000 glmtuner-0.1.1/src/glmtuner/extras/misc.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1716 2023-07-15 16:54:19.000000 glmtuner-0.1.1/src/glmtuner/extras/ploting.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2172 2023-07-15 16:54:19.000000 glmtuner-0.1.1/src/glmtuner/extras/save_and_load.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 16:54:27.998214 glmtuner-0.1.1/src/glmtuner/hparams/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      302 2023-07-15 16:54:20.000000 glmtuner-0.1.1/src/glmtuner/hparams/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4283 2023-07-15 16:54:20.000000 glmtuner-0.1.1/src/glmtuner/hparams/data_args.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3309 2023-07-15 16:54:20.000000 glmtuner-0.1.1/src/glmtuner/hparams/finetuning_args.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      382 2023-07-15 16:54:20.000000 glmtuner-0.1.1/src/glmtuner/hparams/general_args.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1685 2023-07-15 16:54:20.000000 glmtuner-0.1.1/src/glmtuner/hparams/generating_args.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3310 2023-07-15 16:54:20.000000 glmtuner-0.1.1/src/glmtuner/hparams/model_args.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 16:54:28.002214 glmtuner-0.1.1/src/glmtuner/tuner/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      208 2023-07-15 16:54:21.000000 glmtuner-0.1.1/src/glmtuner/tuner/__init__.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 16:54:28.050214 glmtuner-0.1.1/src/glmtuner/tuner/core/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      136 2023-07-15 16:54:20.000000 glmtuner-0.1.1/src/glmtuner/tuner/core/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4113 2023-07-15 16:54:20.000000 glmtuner-0.1.1/src/glmtuner/tuner/core/adapter.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     8739 2023-07-15 16:54:20.000000 glmtuner-0.1.1/src/glmtuner/tuner/core/loader.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     5669 2023-07-15 16:54:20.000000 glmtuner-0.1.1/src/glmtuner/tuner/core/parser.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4125 2023-07-15 16:54:20.000000 glmtuner-0.1.1/src/glmtuner/tuner/core/trainer.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 16:54:28.058214 glmtuner-0.1.1/src/glmtuner/tuner/ppo/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       49 2023-07-15 16:54:21.000000 glmtuner-0.1.1/src/glmtuner/tuner/ppo/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    11291 2023-07-15 16:54:20.000000 glmtuner-0.1.1/src/glmtuner/tuner/ppo/trainer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1673 2023-07-15 16:54:21.000000 glmtuner-0.1.1/src/glmtuner/tuner/ppo/utils.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3022 2023-07-15 16:54:21.000000 glmtuner-0.1.1/src/glmtuner/tuner/ppo/workflow.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 16:54:28.110214 glmtuner-0.1.1/src/glmtuner/tuner/rm/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       47 2023-07-15 16:54:21.000000 glmtuner-0.1.1/src/glmtuner/tuner/rm/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      725 2023-07-15 16:54:21.000000 glmtuner-0.1.1/src/glmtuner/tuner/rm/collator.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      273 2023-07-15 16:54:21.000000 glmtuner-0.1.1/src/glmtuner/tuner/rm/metric.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1523 2023-07-15 16:54:21.000000 glmtuner-0.1.1/src/glmtuner/tuner/rm/trainer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2888 2023-07-15 16:54:21.000000 glmtuner-0.1.1/src/glmtuner/tuner/rm/workflow.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 16:54:28.294214 glmtuner-0.1.1/src/glmtuner/tuner/sft/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       49 2023-07-15 16:54:21.000000 glmtuner-0.1.1/src/glmtuner/tuner/sft/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2200 2023-07-15 16:54:21.000000 glmtuner-0.1.1/src/glmtuner/tuner/sft/metric.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2657 2023-07-15 16:54:21.000000 glmtuner-0.1.1/src/glmtuner/tuner/sft/trainer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4208 2023-07-15 16:54:21.000000 glmtuner-0.1.1/src/glmtuner/tuner/sft/workflow.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 16:54:28.646215 glmtuner-0.1.1/src/glmtuner/webui/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       48 2023-07-15 16:54:22.000000 glmtuner-0.1.1/src/glmtuner/webui/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2605 2023-07-15 16:54:21.000000 glmtuner-0.1.1/src/glmtuner/webui/chat.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2394 2023-07-15 16:54:21.000000 glmtuner-0.1.1/src/glmtuner/webui/common.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 16:54:28.890215 glmtuner-0.1.1/src/glmtuner/webui/components/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      242 2023-07-15 16:54:22.000000 glmtuner-0.1.1/src/glmtuner/webui/components/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      612 2023-07-15 16:54:22.000000 glmtuner-0.1.1/src/glmtuner/webui/components/data.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1778 2023-07-15 16:54:22.000000 glmtuner-0.1.1/src/glmtuner/webui/components/eval.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2740 2023-07-15 16:54:22.000000 glmtuner-0.1.1/src/glmtuner/webui/components/infer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1311 2023-07-15 16:54:22.000000 glmtuner-0.1.1/src/glmtuner/webui/components/model.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3862 2023-07-15 16:54:22.000000 glmtuner-0.1.1/src/glmtuner/webui/components/sft.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      387 2023-07-15 16:54:22.000000 glmtuner-0.1.1/src/glmtuner/webui/css.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1030 2023-07-15 16:54:22.000000 glmtuner-0.1.1/src/glmtuner/webui/interface.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     6525 2023-07-15 16:54:22.000000 glmtuner-0.1.1/src/glmtuner/webui/runner.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2501 2023-07-15 16:54:22.000000 glmtuner-0.1.1/src/glmtuner/webui/utils.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 16:54:27.862213 glmtuner-0.1.1/src/glmtuner.egg-info/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    18438 2023-07-15 16:54:26.000000 glmtuner-0.1.1/src/glmtuner.egg-info/PKG-INFO
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2038 2023-07-15 16:54:27.000000 glmtuner-0.1.1/src/glmtuner.egg-info/SOURCES.txt
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        1 2023-07-15 16:54:26.000000 glmtuner-0.1.1/src/glmtuner.egg-info/dependency_links.txt
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      227 2023-07-15 16:54:26.000000 glmtuner-0.1.1/src/glmtuner.egg-info/requires.txt
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        9 2023-07-15 16:54:26.000000 glmtuner-0.1.1/src/glmtuner.egg-info/top_level.txt
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-17 15:15:02.498501 glmtuner-0.1.2/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    11524 2023-07-17 15:14:50.000000 glmtuner-0.1.2/LICENSE
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    18380 2023-07-17 15:15:02.494501 glmtuner-0.1.2/PKG-INFO
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    17795 2023-07-17 15:14:51.000000 glmtuner-0.1.2/README.md
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       87 2023-07-17 15:14:50.000000 glmtuner-0.1.2/pyproject.toml
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       38 2023-07-17 15:15:02.498501 glmtuner-0.1.2/setup.cfg
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2006 2023-07-17 15:14:51.000000 glmtuner-0.1.2/setup.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-17 15:15:02.082502 glmtuner-0.1.2/src/
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-17 15:15:02.126501 glmtuner-0.1.2/src/glmtuner/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      250 2023-07-17 15:14:49.000000 glmtuner-0.1.2/src/glmtuner/__init__.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-17 15:15:02.170501 glmtuner-0.1.2/src/glmtuner/api/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       41 2023-07-17 15:14:46.000000 glmtuner-0.1.2/src/glmtuner/api/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4489 2023-07-17 15:14:46.000000 glmtuner-0.1.2/src/glmtuner/api/app.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2053 2023-07-17 15:14:46.000000 glmtuner-0.1.2/src/glmtuner/api/protocol.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-17 15:15:02.174502 glmtuner-0.1.2/src/glmtuner/chat/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       49 2023-07-17 15:14:46.000000 glmtuner-0.1.2/src/glmtuner/chat/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2943 2023-07-17 15:14:46.000000 glmtuner-0.1.2/src/glmtuner/chat/stream_chat.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-17 15:15:02.182501 glmtuner-0.1.2/src/glmtuner/dsets/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      165 2023-07-17 15:14:47.000000 glmtuner-0.1.2/src/glmtuner/dsets/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     6589 2023-07-17 15:14:46.000000 glmtuner-0.1.2/src/glmtuner/dsets/collator.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4249 2023-07-17 15:14:46.000000 glmtuner-0.1.2/src/glmtuner/dsets/loader.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     7475 2023-07-17 15:14:47.000000 glmtuner-0.1.2/src/glmtuner/dsets/preprocess.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-17 15:15:02.194501 glmtuner-0.1.2/src/glmtuner/extras/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2023-07-17 15:14:47.000000 glmtuner-0.1.2/src/glmtuner/extras/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3000 2023-07-17 15:14:47.000000 glmtuner-0.1.2/src/glmtuner/extras/callbacks.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      306 2023-07-17 15:14:47.000000 glmtuner-0.1.2/src/glmtuner/extras/constants.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      751 2023-07-17 15:14:47.000000 glmtuner-0.1.2/src/glmtuner/extras/logging.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     5062 2023-07-17 15:14:47.000000 glmtuner-0.1.2/src/glmtuner/extras/misc.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1788 2023-07-17 15:14:47.000000 glmtuner-0.1.2/src/glmtuner/extras/ploting.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2172 2023-07-17 15:14:47.000000 glmtuner-0.1.2/src/glmtuner/extras/save_and_load.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-17 15:15:02.202501 glmtuner-0.1.2/src/glmtuner/hparams/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      302 2023-07-17 15:14:47.000000 glmtuner-0.1.2/src/glmtuner/hparams/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4283 2023-07-17 15:14:47.000000 glmtuner-0.1.2/src/glmtuner/hparams/data_args.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3309 2023-07-17 15:14:47.000000 glmtuner-0.1.2/src/glmtuner/hparams/finetuning_args.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      382 2023-07-17 15:14:47.000000 glmtuner-0.1.2/src/glmtuner/hparams/general_args.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1685 2023-07-17 15:14:47.000000 glmtuner-0.1.2/src/glmtuner/hparams/generating_args.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3310 2023-07-17 15:14:47.000000 glmtuner-0.1.2/src/glmtuner/hparams/model_args.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-17 15:15:02.206501 glmtuner-0.1.2/src/glmtuner/tuner/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      208 2023-07-17 15:14:49.000000 glmtuner-0.1.2/src/glmtuner/tuner/__init__.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-17 15:15:02.430501 glmtuner-0.1.2/src/glmtuner/tuner/core/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      136 2023-07-17 15:14:48.000000 glmtuner-0.1.2/src/glmtuner/tuner/core/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4113 2023-07-17 15:14:48.000000 glmtuner-0.1.2/src/glmtuner/tuner/core/adapter.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     8545 2023-07-17 15:14:48.000000 glmtuner-0.1.2/src/glmtuner/tuner/core/loader.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     5669 2023-07-17 15:14:48.000000 glmtuner-0.1.2/src/glmtuner/tuner/core/parser.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4125 2023-07-17 15:14:48.000000 glmtuner-0.1.2/src/glmtuner/tuner/core/trainer.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-17 15:15:02.450501 glmtuner-0.1.2/src/glmtuner/tuner/ppo/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       49 2023-07-17 15:14:48.000000 glmtuner-0.1.2/src/glmtuner/tuner/ppo/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    10451 2023-07-17 15:14:48.000000 glmtuner-0.1.2/src/glmtuner/tuner/ppo/trainer.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1673 2023-07-17 15:14:48.000000 glmtuner-0.1.2/src/glmtuner/tuner/ppo/utils.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3066 2023-07-17 15:14:48.000000 glmtuner-0.1.2/src/glmtuner/tuner/ppo/workflow.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-17 15:15:02.458501 glmtuner-0.1.2/src/glmtuner/tuner/rm/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       47 2023-07-17 15:14:49.000000 glmtuner-0.1.2/src/glmtuner/tuner/rm/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      725 2023-07-17 15:14:48.000000 glmtuner-0.1.2/src/glmtuner/tuner/rm/collator.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      273 2023-07-17 15:14:48.000000 glmtuner-0.1.2/src/glmtuner/tuner/rm/metric.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1523 2023-07-17 15:14:48.000000 glmtuner-0.1.2/src/glmtuner/tuner/rm/trainer.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2888 2023-07-17 15:14:48.000000 glmtuner-0.1.2/src/glmtuner/tuner/rm/workflow.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-17 15:15:02.466501 glmtuner-0.1.2/src/glmtuner/tuner/sft/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       49 2023-07-17 15:14:49.000000 glmtuner-0.1.2/src/glmtuner/tuner/sft/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2200 2023-07-17 15:14:49.000000 glmtuner-0.1.2/src/glmtuner/tuner/sft/metric.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2587 2023-07-17 15:14:49.000000 glmtuner-0.1.2/src/glmtuner/tuner/sft/trainer.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4208 2023-07-17 15:14:49.000000 glmtuner-0.1.2/src/glmtuner/tuner/sft/workflow.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-17 15:15:02.478501 glmtuner-0.1.2/src/glmtuner/webui/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       48 2023-07-17 15:14:50.000000 glmtuner-0.1.2/src/glmtuner/webui/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2456 2023-07-17 15:14:49.000000 glmtuner-0.1.2/src/glmtuner/webui/chat.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2564 2023-07-17 15:14:49.000000 glmtuner-0.1.2/src/glmtuner/webui/common.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-17 15:15:02.494501 glmtuner-0.1.2/src/glmtuner/webui/components/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      234 2023-07-17 15:14:50.000000 glmtuner-0.1.2/src/glmtuner/webui/components/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1789 2023-07-17 15:14:49.000000 glmtuner-0.1.2/src/glmtuner/webui/components/chatbot.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      625 2023-07-17 15:14:49.000000 glmtuner-0.1.2/src/glmtuner/webui/components/data.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2191 2023-07-17 15:14:49.000000 glmtuner-0.1.2/src/glmtuner/webui/components/eval.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1353 2023-07-17 15:14:49.000000 glmtuner-0.1.2/src/glmtuner/webui/components/infer.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3694 2023-07-17 15:14:49.000000 glmtuner-0.1.2/src/glmtuner/webui/components/sft.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1493 2023-07-17 15:14:50.000000 glmtuner-0.1.2/src/glmtuner/webui/components/top.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      387 2023-07-17 15:14:49.000000 glmtuner-0.1.2/src/glmtuner/webui/css.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1461 2023-07-17 15:14:50.000000 glmtuner-0.1.2/src/glmtuner/webui/interface.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     8980 2023-07-17 15:14:50.000000 glmtuner-0.1.2/src/glmtuner/webui/locales.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1224 2023-07-17 15:14:50.000000 glmtuner-0.1.2/src/glmtuner/webui/manager.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     6552 2023-07-17 15:14:50.000000 glmtuner-0.1.2/src/glmtuner/webui/runner.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2606 2023-07-17 15:14:50.000000 glmtuner-0.1.2/src/glmtuner/webui/utils.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-17 15:15:02.134502 glmtuner-0.1.2/src/glmtuner.egg-info/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    18380 2023-07-17 15:15:00.000000 glmtuner-0.1.2/src/glmtuner.egg-info/PKG-INFO
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2137 2023-07-17 15:15:01.000000 glmtuner-0.1.2/src/glmtuner.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        1 2023-07-17 15:15:00.000000 glmtuner-0.1.2/src/glmtuner.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      219 2023-07-17 15:15:00.000000 glmtuner-0.1.2/src/glmtuner.egg-info/requires.txt
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        9 2023-07-17 15:15:00.000000 glmtuner-0.1.2/src/glmtuner.egg-info/top_level.txt
```

### Comparing `glmtuner-0.1.1/LICENSE` & `glmtuner-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.1/PKG-INFO` & `glmtuner-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glmtuner
-Version: 0.1.1
+Version: 0.1.2
 Summary: Fine-tuning ChatGLM-6B with PEFT
 Home-page: https://github.com/hiyouga/ChatGLM-Efficient-Tuning
 Author: hiyouga
 Author-email: hiyouga@buaa.edu.cn
 License: Apache 2.0 License
 Keywords: ChatGLM,LLM,ChatGPT,transformer,pytorch,deep learning
 Classifier: Development Status :: 3 - Alpha
@@ -275,15 +275,14 @@
 | LoRA (r=8)       |     4      | FP16 |  20GB  | 8ex/s |
 | LoRA (r=8)       |     4      | INT8 |  10GB  | 8ex/s |
 | LoRA (r=8)       |     4      | INT4 |   8GB  | 8ex/s |
 | P-Tuning (p=16)  |     4      | FP16 |  20GB  | 8ex/s |
 | P-Tuning (p=16)  |     4      | INT8 |  16GB  | 8ex/s |
 | P-Tuning (p=16)  |     4      | INT4 |  12GB  | 8ex/s |
 | Freeze (l=3)     |     4      | FP16 |  24GB  | 8ex/s |
-| Freeze (l=3)     |     4      | INT8 |  12GB  | 8ex/s |
 
 | RM  method       | Batch size | Mode |  GRAM  | Speed |
 | ---------------- | ---------- | ---- | ------ | ----- |
 | LoRA (r=8) + rm  |     4      | FP16 |  22GB  | -     |
 | LoRA (r=8) + rm  |     1      | INT8 |  11GB  | -     |
 
 | RLHF method      | Batch size | Mode |  GRAM  | Speed |
```

### Comparing `glmtuner-0.1.1/README.md` & `glmtuner-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -251,15 +251,14 @@
 | LoRA (r=8)       |     4      | FP16 |  20GB  | 8ex/s |
 | LoRA (r=8)       |     4      | INT8 |  10GB  | 8ex/s |
 | LoRA (r=8)       |     4      | INT4 |   8GB  | 8ex/s |
 | P-Tuning (p=16)  |     4      | FP16 |  20GB  | 8ex/s |
 | P-Tuning (p=16)  |     4      | INT8 |  16GB  | 8ex/s |
 | P-Tuning (p=16)  |     4      | INT4 |  12GB  | 8ex/s |
 | Freeze (l=3)     |     4      | FP16 |  24GB  | 8ex/s |
-| Freeze (l=3)     |     4      | INT8 |  12GB  | 8ex/s |
 
 | RM  method       | Batch size | Mode |  GRAM  | Speed |
 | ---------------- | ---------- | ---- | ------ | ----- |
 | LoRA (r=8) + rm  |     4      | FP16 |  22GB  | -     |
 | LoRA (r=8) + rm  |     1      | INT8 |  11GB  | -     |
 
 | RLHF method      | Batch size | Mode |  GRAM  | Speed |
```

### Comparing `glmtuner-0.1.1/setup.py` & `glmtuner-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.1/src/glmtuner/api/app.py` & `glmtuner-0.1.2/src/glmtuner/api/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 import uvicorn
 from fastapi import FastAPI, HTTPException
 from fastapi.middleware.cors import CORSMiddleware
 from contextlib import asynccontextmanager
 from sse_starlette import EventSourceResponse
 from typing import List, Tuple
 
@@ -87,37 +88,37 @@
     async def predict(query: str, history: List[Tuple[str, str]], request: ChatCompletionRequest):
         choice_data = ChatCompletionResponseStreamChoice(
             index=0,
             delta=DeltaMessage(role="assistant"),
             finish_reason=None
         )
         chunk = ChatCompletionStreamResponse(model=request.model, choices=[choice_data], object="chat.completion.chunk")
-        yield chunk.json(exclude_unset=True, ensure_ascii=False)
+        yield json.dumps(chunk, ensure_ascii=False)
 
         for new_text in chat_model.stream_chat(
             query, history, temperature=request.temperature, top_p=request.top_p, max_new_tokens=request.max_tokens
         ):
             if len(new_text) == 0:
                 continue
 
             choice_data = ChatCompletionResponseStreamChoice(
                 index=0,
                 delta=DeltaMessage(content=new_text),
                 finish_reason=None
             )
             chunk = ChatCompletionStreamResponse(model=request.model, choices=[choice_data], object="chat.completion.chunk")
-            yield chunk.json(exclude_unset=True, ensure_ascii=False)
+            yield json.dumps(chunk, ensure_ascii=False)
 
         choice_data = ChatCompletionResponseStreamChoice(
             index=0,
             delta=DeltaMessage(),
             finish_reason="stop"
         )
         chunk = ChatCompletionStreamResponse(model=request.model, choices=[choice_data], object="chat.completion.chunk")
-        yield chunk.json(exclude_unset=True, ensure_ascii=False)
+        yield json.dumps(chunk, ensure_ascii=False)
         yield "[DONE]"
 
     return app
 
 
 if __name__ == "__main__":
     app = create_app()
```

### Comparing `glmtuner-0.1.1/src/glmtuner/api/protocol.py` & `glmtuner-0.1.2/src/glmtuner/api/protocol.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.1/src/glmtuner/chat/stream_chat.py` & `glmtuner-0.1.2/src/glmtuner/chat/stream_chat.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,35 +32,37 @@
         top_k = input_kwargs.pop("top_k", None)
         repetition_penalty = input_kwargs.pop("repetition_penalty", None)
         max_length = input_kwargs.pop("max_length", None)
         max_new_tokens = input_kwargs.pop("max_new_tokens", None)
 
         gen_kwargs = self.generating_args.to_dict()
         gen_kwargs.update(dict(
-            temperature=temperature if temperature else gen_kwargs["temperature"],
-            top_p=top_p if top_p else gen_kwargs["top_p"],
-            top_k=top_k if top_k else gen_kwargs["top_k"],
-            repetition_penalty=repetition_penalty if repetition_penalty else gen_kwargs["repetition_penalty"]
+            temperature=temperature or gen_kwargs["temperature"],
+            top_p=top_p or gen_kwargs["top_p"],
+            top_k=top_k or gen_kwargs["top_k"],
+            repetition_penalty=repetition_penalty or gen_kwargs["repetition_penalty"]
         ))
 
         if max_length:
             gen_kwargs.pop("max_new_tokens", None)
             gen_kwargs["max_length"] = max_length
 
         if max_new_tokens:
             gen_kwargs.pop("max_length", None)
             gen_kwargs["max_new_tokens"] = max_new_tokens
 
         return gen_kwargs
 
+    @torch.inference_mode()
     def chat(self, query: str, history: Optional[List[Tuple[str, str]]] = None, **input_kwargs) -> str:
         gen_kwargs = self.process_args(**input_kwargs)
         response = self.model.chat(self.tokenizer, query, history, **gen_kwargs)
         return response
 
+    @torch.inference_mode()
     def stream_chat(
         self, query: str, history: Optional[List[Tuple[str, str]]] = None, **input_kwargs
     ) -> Generator[str, None, None]:
         gen_kwargs = self.process_args(**input_kwargs)
         current_length = 0
         for new_response, _ in self.model.stream_chat(self.tokenizer, query, history, **gen_kwargs):
             if len(new_response) == current_length:
```

### Comparing `glmtuner-0.1.1/src/glmtuner/dsets/collator.py` & `glmtuner-0.1.2/src/glmtuner/dsets/collator.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.1/src/glmtuner/dsets/loader.py` & `glmtuner-0.1.2/src/glmtuner/dsets/loader.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.1/src/glmtuner/dsets/preprocess.py` & `glmtuner-0.1.2/src/glmtuner/dsets/preprocess.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.1/src/glmtuner/extras/callbacks.py` & `glmtuner-0.1.2/src/glmtuner/extras/callbacks.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.1/src/glmtuner/extras/logging.py` & `glmtuner-0.1.2/src/glmtuner/extras/logging.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.1/src/glmtuner/extras/misc.py` & `glmtuner-0.1.2/src/glmtuner/extras/misc.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.1/src/glmtuner/extras/ploting.py` & `glmtuner-0.1.2/src/glmtuner/extras/ploting.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import os
+import math
 import json
 import matplotlib.pyplot as plt
 from typing import List, Optional
 from transformers.trainer import TRAINER_STATE_NAME
 
 from glmtuner.extras.logging import get_logger
 
 
 logger = get_logger(__name__)
 
 
-def smooth(scalars: List[float], weight: Optional[float] = 0.9) -> List[float]:
+def smooth(scalars: List[float]) -> List[float]:
     r"""
     EMA implementation according to TensorBoard.
     """
     last = scalars[0]
     smoothed = list()
+    weight = 1.8 * (1 / (1 + math.exp(-0.05 * len(scalars))) - 0.5) # a sigmoid function
     for next_val in scalars:
         smoothed_val = last * weight + (1 - weight) * next_val
         smoothed.append(smoothed_val)
         last = smoothed_val
     return smoothed
```

### Comparing `glmtuner-0.1.1/src/glmtuner/extras/save_and_load.py` & `glmtuner-0.1.2/src/glmtuner/extras/save_and_load.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.1/src/glmtuner/hparams/data_args.py` & `glmtuner-0.1.2/src/glmtuner/hparams/data_args.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.1/src/glmtuner/hparams/finetuning_args.py` & `glmtuner-0.1.2/src/glmtuner/hparams/finetuning_args.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.1/src/glmtuner/hparams/generating_args.py` & `glmtuner-0.1.2/src/glmtuner/hparams/generating_args.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.1/src/glmtuner/hparams/model_args.py` & `glmtuner-0.1.2/src/glmtuner/hparams/model_args.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.1/src/glmtuner/tuner/core/adapter.py` & `glmtuner-0.1.2/src/glmtuner/tuner/core/adapter.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.1/src/glmtuner/tuner/core/loader.py` & `glmtuner-0.1.2/src/glmtuner/tuner/core/loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     AutoModel,
     AutoTokenizer,
     BitsAndBytesConfig
 )
 from transformers.utils import check_min_version
 from transformers.utils.versions import require_version
 from transformers.modeling_utils import PretrainedConfig, PreTrainedModel
-from transformers.tokenization_utils import PreTrainedTokenizer
+from transformers.tokenization_utils import PreTrainedTokenizerBase
 from trl import AutoModelForCausalLMWithValueHead
 
 from glmtuner.extras.logging import get_logger
 from glmtuner.extras.misc import prepare_model_for_training, print_trainable_params
 from glmtuner.extras.save_and_load import load_valuehead_params
 from glmtuner.hparams import ModelArguments, FinetuningArguments
 from glmtuner.tuner.core.adapter import init_adapter
@@ -24,23 +24,23 @@
 logger = get_logger(__name__)
 
 
 check_min_version("4.27.4")
 require_version("datasets>=2.10.0", "To fix: pip install datasets>=2.10.0")
 require_version("accelerate>=0.19.0", "To fix: pip install accelerate>=0.19.0")
 require_version("peft>=0.3.0", "To fix: pip install peft>=0.3.0")
-require_version("trl>=0.4.4", "To fix: pip install trl>=0.4.4")
+require_version("trl>=0.4.7", "To fix: pip install trl>=0.4.7")
 
 
 def load_model_and_tokenizer(
     model_args: ModelArguments,
     finetuning_args: FinetuningArguments,
     is_trainable: Optional[bool] = False,
     stage: Optional[Literal["sft", "rm", "ppo"]] = "sft"
-) -> Tuple[PreTrainedModel, PreTrainedTokenizer]:
+) -> Tuple[PreTrainedModel, PreTrainedTokenizerBase]:
     r"""
     Loads pretrained model and tokenizer.
 
     Support both training and inference.
     """
 
     if (not is_trainable) and model_args.checkpoint_dir is None:
@@ -114,19 +114,19 @@
     else:
         model_to_load = model_args.model_name_or_path
 
     # Load and prepare pretrained models (without valuehead).
     model = AutoModel.from_pretrained(model_to_load, config=config, **config_kwargs)
 
     # Register auto class to save the custom code files.
-    if hasattr(config, "auto_map") and "AutoConfig" in config.auto_map and isinstance(config, PretrainedConfig):
+    if isinstance(config, PretrainedConfig):
         config.__class__.register_for_auto_class()
-    if hasattr(config, "auto_map") and "AutoTokenizer" in config.auto_map and isinstance(tokenizer, PreTrainedTokenizer):
+    if isinstance(tokenizer, PreTrainedTokenizerBase):
         tokenizer.__class__.register_for_auto_class()
-    if hasattr(config, "auto_map") and "AutoModel" in config.auto_map and isinstance(model, PreTrainedModel):
+    if isinstance(model, PreTrainedModel):
         model.__class__.register_for_auto_class()
 
     if tokenizer.eos_token_id == 130005: # ChatGLM-6B
         output_embedding_base_layer = model
         output_embedding_layer_name = "lm_head"
     elif tokenizer.eos_token_id == 2: # ChatGLM2-6B
         assert hasattr(model, "transformer"), "Please update the model files of ChatGLM-6B."
```

### Comparing `glmtuner-0.1.1/src/glmtuner/tuner/core/parser.py` & `glmtuner-0.1.2/src/glmtuner/tuner/core/parser.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.1/src/glmtuner/tuner/core/trainer.py` & `glmtuner-0.1.2/src/glmtuner/tuner/core/trainer.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.1/src/glmtuner/tuner/ppo/trainer.py` & `glmtuner-0.1.2/src/glmtuner/tuner/ppo/trainer.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 logger = get_logger(__name__)
 
 
 class PPOTrainerForChatGLM(PPOTrainer, PeftTrainer):
     r"""
     Inherits PPOTrainer.
     """
-
     def __init__(
         self,
         training_args: Seq2SeqTrainingArguments,
         finetuning_args: FinetuningArguments,
         callbacks: List[LogCallback],
         **kwargs
     ):
@@ -43,136 +42,125 @@
         self.data_collator = self.accelerator.prepare(kwargs["data_collator"]) # override the data collator of PPOTrainer
         self._remove_log()
 
     def ppo_train(self, max_target_length: int) -> None:
         r"""
         Implements training loop for the PPO stage, like _inner_training_loop() in Huggingface's Trainer.
         """
-
-        total_train_batch_size = self.config.batch_size * self.config.gradient_accumulation_steps * self.args.world_size
+        total_train_batch_size = (
+            self.args.per_device_train_batch_size * self.args.gradient_accumulation_steps * self.args.world_size
+        )
         len_dataloader = len(self.dataloader)
-        num_steps_per_epoch = max(len_dataloader // self.config.gradient_accumulation_steps, 1)
         num_examples = len(self.dataset)
         num_train_epochs = self.args.num_train_epochs
-        max_steps = math.ceil(num_train_epochs * num_steps_per_epoch)
+        max_steps = math.ceil(num_train_epochs * len_dataloader)
 
         self.state.max_steps = max_steps
         self.state.num_train_epochs = num_train_epochs
         self.state.is_local_process_zero = self.is_local_process_zero()
         self.state.is_world_process_zero = self.is_world_process_zero()
 
         if self.is_world_process_zero():
             logger.info("***** Running training *****")
             logger.info(f"  Num examples = {num_examples}")
             logger.info(f"  Num Epochs = {num_train_epochs}")
-            logger.info(f"  Instantaneous batch size per device = {self.config.batch_size}")
+            logger.info(f"  Instantaneous batch size per device = {self.args.per_device_train_batch_size}")
             logger.info(f"  Total train batch size (w. parallel, distributed & accumulation) = {total_train_batch_size}")
-            logger.info(f"  Gradient Accumulation steps = {self.config.gradient_accumulation_steps}")
+            logger.info(f"  Gradient Accumulation steps = {self.args.gradient_accumulation_steps}")
             logger.info(f"  Total optimization steps = {max_steps}")
             logger.info(f"  Number of trainable parameters = {sum(p.numel() for p in self.model.parameters() if p.requires_grad)}")
 
         # Keyword arguments for `model.generate`
         gen_kwargs = {
             "top_k": 0.0,
             "top_p": 1.0,
             "do_sample": True,
             "pad_token_id": self.tokenizer.pad_token_id,
             "eos_token_id": self.tokenizer.eos_token_id,
             "logits_processor": get_logits_processor()
         }
-        output_length_sampler = LengthSampler(max_target_length // 2, max_target_length)
+        length_sampler = LengthSampler(max_target_length // 2, max_target_length)
         unwrapped_model: PreTrainedModel = self.accelerator.unwrap_model(self.model)
 
         dataiter = iter(self.dataloader)
         steps_trained = 0
         loss_meter = AverageMeter()
         reward_meter = AverageMeter()
         self.log_callback.on_train_begin(self.args, self.state, self.control)
 
         for step in tqdm(range(max_steps), disable=not self.is_world_process_zero(), leave=False):
+            batch = next(dataiter)
+            steps_trained += 1
 
-            for _ in range(self.config.gradient_accumulation_steps):
-
-                batch = next(dataiter)
-                steps_trained += 1
+            unwrapped_model.gradient_checkpointing_disable()
+            unwrapped_model.config.use_cache = True
 
-                unwrapped_model.gradient_checkpointing_disable()
-                unwrapped_model.config.use_cache = True
-
-                # Get response from ChatGLM
-                query_tensors: torch.Tensor = batch["input_ids"]
-                response_tensors = self.generate(batch, length_sampler=output_length_sampler, return_prompt=False, **gen_kwargs)
-
-                queries: List[torch.Tensor] = []
-                responses: List[torch.Tensor] = []
-                for i in range(len(query_tensors)):
-                    query_length = (query_tensors[i] != self.tokenizer.pad_token_id).nonzero()[0]
-                    response_length = (response_tensors[i] != self.tokenizer.pad_token_id).nonzero()[-1] + 1
-                    queries.append(query_tensors[i, query_length:]) # remove padding from left
-                    if response_length < 2: # make response have at least 2 tokens
-                        responses.append(response_tensors.new_empty(2).fill_(self.tokenizer.eos_token_id))
-                    else:
-                        responses.append(response_tensors[i, :response_length]) # remove padding from right
-
-                # Compute rewards
-                replace_model(unwrapped_model, target="reward")
+            # Get responses
+            query_tensors = batch["input_ids"]
+            response_tensors = self.generate(batch, length_sampler, return_prompt=False, **gen_kwargs)
+
+            queries, responses = [], []
+            for i in range(len(query_tensors)):
+                query_length = (query_tensors[i] != self.tokenizer.pad_token_id).nonzero()[0]
+                response_length = (response_tensors[i] != self.tokenizer.pad_token_id).nonzero()[-1] + 1
+                queries.append(query_tensors[i, query_length:]) # remove padding from left
+                responses.append(response_tensors[i, :response_length]) # remove padding from right
+
+            # Compute rewards
+            replace_model(unwrapped_model, target="reward")
+            with torch.no_grad():
                 _, _, values = self.model(**self.prepare_model_inputs(queries, responses))
-                rewards = [reward for reward in values[-1].to(torch.float32)] # use float32 type
-                replace_model(unwrapped_model, target="default") # make sure the model is default at the end
-
-                # Run PPO step
-                unwrapped_model.gradient_checkpointing_enable()
-                unwrapped_model.config.use_cache = False
+            rewards = [reward for reward in values[-1].to(torch.float32)] # use float32 type
+            replace_model(unwrapped_model, target="default")
 
-                stats = self.step(queries, responses, rewards)
+            # Run PPO step
+            unwrapped_model.gradient_checkpointing_enable()
+            unwrapped_model.config.use_cache = False
+            stats = self.step(queries, responses, rewards)
 
-                loss_meter.update(stats["ppo/loss/total"], n=len(rewards))
-                reward_meter.update(torch.stack(rewards).mean().item(), n=len(rewards))
-
-                if self.control.should_epoch_stop or self.control.should_training_stop:
-                    break
-
-                if steps_trained == len_dataloader:
-                    dataiter = iter(self.dataloader)
-                    steps_trained = 0
+            loss_meter.update(stats["ppo/loss/total"], n=len(rewards))
+            reward_meter.update(torch.stack(rewards).mean().item(), n=len(rewards))
 
             if self.is_world_process_zero() and (step+1) % self.args.logging_steps == 0:
-                logs = {
-                    "loss": round(loss_meter.avg, 4),
-                    "reward": round(reward_meter.avg, 4),
-                    "learning_rate": stats["ppo/learning_rate"],
-                    "epoch": round(step / num_steps_per_epoch, 2)
-                }
+                logs = dict(
+                    loss=round(loss_meter.avg, 4),
+                    reward=round(reward_meter.avg, 4),
+                    learning_rate=stats["ppo/learning_rate"],
+                    epoch=round(step / len_dataloader, 2)
+                )
                 print(logs)
                 logs["step"] = step
                 self.state.log_history.append(logs)
                 self.log_callback.on_log(self.args, self.state, self.control)
                 loss_meter.reset()
                 reward_meter.reset()
 
             if (step+1) % self.args.save_steps == 0: # save checkpoint
                 self.save_model(os.path.join(self.args.output_dir, f"checkpoint-{step+1}"))
 
-            if self.control.should_training_stop:
+            if self.control.should_epoch_stop or self.control.should_training_stop:
                 break
 
+            if steps_trained == len_dataloader:
+                dataiter = iter(self.dataloader)
+                steps_trained = 0
+
     @torch.no_grad()
     def generate(
         self,
         inputs: Dict[str, torch.Tensor],
         length_sampler: Optional[Callable] = None,
         return_prompt: Optional[bool] = True,
         **generation_kwargs
     ) -> torch.Tensor:
         r"""
         Generates model's responses given queries.
 
         Subclass and override to inject custom behavior.
         """
-
         self.model, layer_norm_params = cast_layernorm_dtype(self.model)
 
         if length_sampler is not None:
             generation_kwargs["max_new_tokens"] = length_sampler()
 
         unwrapped_model = self.accelerator.unwrap_model(self.model)
 
@@ -199,15 +187,14 @@
         return_logits: bool = False
     ):
         r"""
         Calculates model outputs in multiple batches.
 
         Subclass and override to inject custom behavior.
         """
-
         bs = len(queries)
         fbs = self.config.mini_batch_size
         all_logprobs = []
         all_logits = []
         all_masks = []
         all_values = []
 
@@ -219,25 +206,22 @@
 
             if self.is_distributed: # re-generate them to adapt padded inputs
                 input_kwargs["attention_mask"] = self.data_collator.get_attention_masks(input_ids, device=self.current_device)
                 input_kwargs["position_ids"] = self.data_collator.get_position_ids(input_ids, device=self.current_device)
 
             logits, _, values = model(**input_kwargs)
             logprobs = logprobs_from_logits(logits[:, :-1, :], input_ids[:, 1:])
-
             values = values.transpose(0, 1)
             masks = torch.zeros_like(input_ids)
 
             for j in range(fbs):
                 start = len(query_batch[j]) - 1
                 start += (input_ids[j] != self.tokenizer.pad_token_id).nonzero()[0].item()
                 end = start + len(response_batch[j])
                 masks[j][start:end] = 1
-                if len(masks[j][start:end]) < 2:
-                    raise ValueError("Responses are too short. Make sure they are at least 4 tokens long.")
 
             if return_logits:
                 all_logits.append(logits)
             else:
                 del logits
             all_values.append(values)
             all_logprobs.append(logprobs)
```

### Comparing `glmtuner-0.1.1/src/glmtuner/tuner/ppo/utils.py` & `glmtuner-0.1.2/src/glmtuner/tuner/ppo/utils.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.1/src/glmtuner/tuner/ppo/workflow.py` & `glmtuner-0.1.2/src/glmtuner/tuner/ppo/workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     dataset = preprocess_dataset(dataset, tokenizer, data_args, training_args, stage="ppo")
     data_collator = DataCollatorForChatGLM(tokenizer, model.pretrained_model)
 
     ppo_config = PPOConfig(
         model_name=model_args.model_name_or_path,
         learning_rate=training_args.learning_rate,
         mini_batch_size=training_args.per_device_train_batch_size,
-        batch_size=training_args.per_device_train_batch_size,
+        batch_size=training_args.per_device_train_batch_size * training_args.gradient_accumulation_steps,
         gradient_accumulation_steps=training_args.gradient_accumulation_steps,
         ppo_epochs=1,
         max_grad_norm=training_args.max_grad_norm
     )
 
     optimizer = AdamW(filter(lambda p: p.requires_grad, model.parameters()), lr=ppo_config.learning_rate)
     total_train_batch_size = \
```

### Comparing `glmtuner-0.1.1/src/glmtuner/tuner/rm/collator.py` & `glmtuner-0.1.2/src/glmtuner/tuner/rm/collator.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.1/src/glmtuner/tuner/rm/trainer.py` & `glmtuner-0.1.2/src/glmtuner/tuner/rm/trainer.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.1/src/glmtuner/tuner/rm/workflow.py` & `glmtuner-0.1.2/src/glmtuner/tuner/rm/workflow.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.1/src/glmtuner/tuner/sft/metric.py` & `glmtuner-0.1.2/src/glmtuner/tuner/sft/metric.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.1/src/glmtuner/tuner/sft/trainer.py` & `glmtuner-0.1.2/src/glmtuner/tuner/sft/trainer.py`

 * *Files 11% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
         output_prediction_file = os.path.join(self.args.output_dir, "generated_predictions.jsonl")
         logger.info(f"Saving prediction results to {output_prediction_file}")
 
         preds = np.where(predict_results.predictions != IGNORE_INDEX, predict_results.predictions, self.tokenizer.pad_token_id)
         labels = np.where(predict_results.label_ids != IGNORE_INDEX, predict_results.label_ids, self.tokenizer.pad_token_id)
 
-        decoded_preds = self.tokenizer.batch_decode(preds, skip_special_tokens=True, clean_up_tokenization_spaces=True)
-        decoded_labels = self.tokenizer.batch_decode(labels, skip_special_tokens=True, clean_up_tokenization_spaces=True)
+        decoded_preds = self.tokenizer.batch_decode(preds, skip_special_tokens=True)
+        decoded_labels = self.tokenizer.batch_decode(labels, skip_special_tokens=True)
 
         with open(output_prediction_file, "w", encoding="utf-8") as writer:
             res: List[str] = []
             for pred, label in zip(decoded_preds, decoded_labels):
                 res.append(json.dumps({"label": label, "predict": pred}, ensure_ascii=False))
             writer.write("\n".join(res))
```

### Comparing `glmtuner-0.1.1/src/glmtuner/tuner/sft/workflow.py` & `glmtuner-0.1.2/src/glmtuner/tuner/sft/workflow.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.1/src/glmtuner/webui/chat.py` & `glmtuner-0.1.2/src/glmtuner/webui/chat.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,64 +1,66 @@
 import os
 from typing import List, Tuple
 
 from glmtuner.chat.stream_chat import ChatModel
-from glmtuner.extras.constants import SUPPORTED_MODELS
 from glmtuner.extras.misc import torch_gc
 from glmtuner.hparams import GeneratingArguments
 from glmtuner.tuner import get_infer_args
-from glmtuner.webui.common import get_save_dir
+from glmtuner.webui.common import get_model_path, get_save_dir
+from glmtuner.webui.locales import ALERTS
 
 
 class WebChatModel(ChatModel):
 
     def __init__(self):
         self.model = None
         self.tokenizer = None
         self.generating_args = GeneratingArguments()
 
-    def load_model(self, model_name: str, model_path: str, checkpoints: list, quantization_bit: str):
+    def load_model(
+        self, lang: str, model_name: str, checkpoints: list,
+        finetuning_type: str, quantization_bit: str
+    ):
         if self.model is not None:
-            yield "You have loaded a model, please unload it first."
+            yield ALERTS["err_exists"][lang]
             return
 
         if not model_name:
-            yield "Please select a model."
+            yield ALERTS["err_no_model"][lang]
             return
 
-        if model_path:
-            if not os.path.isdir(model_path):
-                return None, "Cannot find model directory in local disk.", None, None
-            model_name_or_path = model_path
-        elif model_name in SUPPORTED_MODELS: # TODO: use list in gr.State
-            model_name_or_path = SUPPORTED_MODELS[model_name]["hf_path"]
-        else:
-            return None, "Invalid model.", None, None
+        model_name_or_path = get_model_path(model_name)
+        if not model_name_or_path:
+            yield ALERTS["err_no_path"][lang]
+            return
 
         if checkpoints:
-            checkpoint_dir = ",".join([os.path.join(get_save_dir(model_name), checkpoint) for checkpoint in checkpoints])
+            checkpoint_dir = ",".join(
+                [os.path.join(get_save_dir(model_name), finetuning_type, checkpoint) for checkpoint in checkpoints]
+            )
         else:
             checkpoint_dir = None
 
-        yield "Loading model..."
+        yield ALERTS["info_loading"][lang]
         args = dict(
             model_name_or_path=model_name_or_path,
+            finetuning_type=finetuning_type,
             checkpoint_dir=checkpoint_dir,
             quantization_bit=int(quantization_bit) if quantization_bit else None
         )
         super().__init__(*get_infer_args(args))
 
-        yield "Model loaded, now you can chat with your model."
+        yield ALERTS["info_loaded"][lang]
 
-    def unload_model(self):
-        yield "Unloading model..."
+    def unload_model(self, lang: str):
+        yield ALERTS["info_unloading"][lang]
         self.model = None
         self.tokenizer = None
         torch_gc()
-        yield "Model unloaded, please load a model first."
+        yield ALERTS["info_unloaded"][lang]
 
     def predict(
         self,
         chatbot: List[Tuple[str, str]],
         query: str,
         history: List[Tuple[str, str]],
         max_length: int,
```

### Comparing `glmtuner-0.1.1/src/glmtuner/webui/components/data.py` & `glmtuner-0.1.2/src/glmtuner/webui/components/data.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import gradio as gr
+from gradio.blocks import Block
 from gradio.components import Component
 from typing import Tuple
 
 
-def create_preview_box() -> Tuple[Component, Component, Component]:
+def create_preview_box() -> Tuple[Block, Component, Component, Component]:
     with gr.Box(visible=False, elem_classes="modal-box") as preview_box:
         with gr.Row():
-            preview_count = gr.Number(label="Count", interactive=False)
+            preview_count = gr.Number(interactive=False)
 
         with gr.Row():
-            preview_samples = gr.JSON(label="Sample", interactive=False)
+            preview_samples = gr.JSON(interactive=False)
 
-        close_btn = gr.Button("Close")
+        close_btn = gr.Button()
 
     close_btn.click(lambda: gr.update(visible=False), outputs=[preview_box])
 
-    return preview_box, preview_count, preview_samples
+    return preview_box, preview_count, preview_samples, close_btn
```

### Comparing `glmtuner-0.1.1/src/glmtuner/webui/components/eval.py` & `glmtuner-0.1.2/src/glmtuner/webui/components/eval.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,44 +1,59 @@
+from typing import Dict
 import gradio as gr
 from gradio.components import Component
 
-from glmtuner.webui.common import list_datasets
+from glmtuner.webui.common import list_dataset, DEFAULT_DATA_DIR
 from glmtuner.webui.components.data import create_preview_box
 from glmtuner.webui.runner import Runner
 from glmtuner.webui.utils import can_preview, get_preview
 
 
-def create_eval_tab(model_name: Component, model_path: Component, checkpoints: Component, runner: Runner) -> None:
+def create_eval_tab(top_elems: Dict[str, Component], runner: Runner) -> Dict[str, Component]:
     with gr.Row():
-        dataset = gr.Dropdown(label="Dataset", choices=list_datasets(), multiselect=True, interactive=True, scale=4)
-        preview_btn = gr.Button("Preview", interactive=False, scale=1)
-
-    preview_box, preview_count, preview_samples = create_preview_box()
-
-    dataset.change(can_preview, [dataset], [preview_btn])
-    preview_btn.click(
-        get_preview, [dataset], [preview_count, preview_samples]
-    ).then(
-        lambda: gr.update(visible=True), outputs=[preview_box]
-    )
+        dataset_dir = gr.Textbox(value=DEFAULT_DATA_DIR, interactive=True, scale=2)
+        dataset = gr.Dropdown(multiselect=True, interactive=True, scale=4)
+        preview_btn = gr.Button(interactive=False, scale=1)
+
+    preview_box, preview_count, preview_samples, close_btn = create_preview_box()
+
+    dataset_dir.change(list_dataset, [dataset_dir], [dataset])
+    dataset.change(can_preview, [dataset_dir, dataset], [preview_btn])
+    preview_btn.click(get_preview, [dataset_dir, dataset], [preview_count, preview_samples, preview_box])
 
     with gr.Row():
-        max_samples = gr.Textbox(
-            label="Max samples", value="100000", info="Number of samples for training.", interactive=True
-        )
-        per_device_eval_batch_size = gr.Slider(
-            label="Batch size", value=8, minimum=1, maximum=128, step=1, info="Eval batch size.", interactive=True
-        )
-        quantization_bit = gr.Dropdown([8, 4], label="Quantization bit", info="Quantize model to 4/8-bit mode.")
+        max_samples = gr.Textbox(value="100000", interactive=True)
+        batch_size = gr.Slider(value=8, minimum=1, maximum=128, step=1, interactive=True)
+        quantization_bit = gr.Dropdown([8, 4])
+        predict = gr.Checkbox(value=True)
 
     with gr.Row():
-        start_btn = gr.Button("Start evaluation")
-        stop_btn = gr.Button("Abort")
+        start_btn = gr.Button()
+        stop_btn = gr.Button()
 
-    output = gr.Markdown(value="Ready")
+    output_box = gr.Markdown()
 
     start_btn.click(
         runner.run_eval,
-        [model_name, model_path, checkpoints, dataset, max_samples, per_device_eval_batch_size, quantization_bit],
-        [output]
+        [
+            top_elems["lang"], top_elems["model_name"], top_elems["checkpoints"], top_elems["finetuning_type"],
+            dataset, dataset_dir, max_samples, batch_size, quantization_bit, predict
+        ],
+        [output_box]
     )
     stop_btn.click(runner.set_abort, queue=False)
+
+    return dict(
+        dataset_dir=dataset_dir,
+        dataset=dataset,
+        preview_btn=preview_btn,
+        preview_count=preview_count,
+        preview_samples=preview_samples,
+        close_btn=close_btn,
+        max_samples=max_samples,
+        batch_size=batch_size,
+        quantization_bit=quantization_bit,
+        predict=predict,
+        start_btn=start_btn,
+        stop_btn=stop_btn,
+        output_box=output_box
+    )
```

### Comparing `glmtuner-0.1.1/src/glmtuner/webui/components/sft.py` & `glmtuner-0.1.2/src/glmtuner/webui/components/sft.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,90 +1,93 @@
+from typing import Dict
+from transformers.trainer_utils import SchedulerType
+
 import gradio as gr
 from gradio.components import Component
-from transformers.trainer_utils import SchedulerType
 
-from glmtuner.webui.common import list_datasets
+from glmtuner.webui.common import list_dataset, DEFAULT_DATA_DIR
 from glmtuner.webui.components.data import create_preview_box
 from glmtuner.webui.runner import Runner
-from glmtuner.webui.utils import can_preview, get_preview, get_time, gen_plot
+from glmtuner.webui.utils import can_preview, get_preview, gen_plot
 
 
-def create_sft_tab(model_name: Component, model_path: Component, checkpoints: Component, runner: Runner) -> None:
+def create_sft_tab(top_elems: Dict[str, Component], runner: Runner) -> Dict[str, Component]:
     with gr.Row():
-        finetuning_type = gr.Dropdown(
-            label="Finetuning method", value="lora",
-            choices=["full", "freeze", "p_tuning", "lora"], interactive=True, scale=2
-        )
-        dataset = gr.Dropdown(label="Dataset", choices=list_datasets(), multiselect=True, interactive=True, scale=2)
-        preview_btn = gr.Button("Preview", interactive=False, scale=1)
+        dataset_dir = gr.Textbox(value=DEFAULT_DATA_DIR, interactive=True, scale=1)
+        dataset = gr.Dropdown(multiselect=True, interactive=True, scale=4)
+        preview_btn = gr.Button(interactive=False, scale=1)
 
-    preview_box, preview_count, preview_samples = create_preview_box()
+    preview_box, preview_count, preview_samples, close_btn = create_preview_box()
 
-    dataset.change(can_preview, [dataset], [preview_btn])
-    preview_btn.click(
-        get_preview, [dataset], [preview_count, preview_samples]
-    ).then(
-        lambda: gr.update(visible=True), outputs=[preview_box]
-    )
+    dataset_dir.change(list_dataset, [dataset_dir], [dataset])
+    dataset.change(can_preview, [dataset_dir, dataset], [preview_btn])
+    preview_btn.click(get_preview, [dataset_dir, dataset], [preview_count, preview_samples, preview_box])
 
     with gr.Row():
-        learning_rate = gr.Textbox(
-            label="Learning rate", value="5e-5", info="The initial learning rate for AdamW.", interactive=True
-        )
-        num_train_epochs = gr.Textbox(
-            label="Epochs", value="3.0", info="Total number of training epochs to perform.", interactive=True
-        )
-        max_samples = gr.Textbox(
-            label="Max samples", value="100000", info="Number of samples for training.", interactive=True
-        )
-        quantization_bit = gr.Dropdown([8, 4], label="Quantization bit", info="Quantize model to 4/8-bit mode.")
+        learning_rate = gr.Textbox(value="5e-5", interactive=True)
+        num_train_epochs = gr.Textbox(value="3.0", interactive=True)
+        max_samples = gr.Textbox(value="100000", interactive=True)
+        quantization_bit = gr.Dropdown([8, 4])
 
     with gr.Row():
-        per_device_train_batch_size = gr.Slider(
-            label="Batch size", value=4, minimum=1, maximum=128, step=1,
-            info="Train batch size.", interactive=True
-        )
-        gradient_accumulation_steps = gr.Slider(
-            label="Gradient accumulation", value=4, minimum=1, maximum=32, step=1,
-            info="Accumulation steps.", interactive=True
-        )
+        batch_size = gr.Slider(value=4, minimum=1, maximum=128, step=1, interactive=True)
+        gradient_accumulation_steps = gr.Slider(value=4, minimum=1, maximum=32, step=1, interactive=True)
         lr_scheduler_type = gr.Dropdown(
-            label="LR Scheduler", value="cosine", info="Scheduler type.",
-            choices=[scheduler.value for scheduler in SchedulerType], interactive=True
+            value="cosine", choices=[scheduler.value for scheduler in SchedulerType], interactive=True
         )
-        fp16 = gr.Checkbox(label="fp16", value=True)
+        fp16 = gr.Checkbox(value=True)
 
     with gr.Row():
-        logging_steps = gr.Slider(
-            label="Logging steps", value=5, minimum=5, maximum=1000, step=5,
-            info="Number of update steps between two logs.", interactive=True
-        )
-        save_steps = gr.Slider(
-            label="Save steps", value=100, minimum=10, maximum=2000, step=10,
-            info="Number of updates steps before two checkpoint saves.", interactive=True
-        )
+        logging_steps = gr.Slider(value=5, minimum=5, maximum=1000, step=5, interactive=True)
+        save_steps = gr.Slider(value=100, minimum=10, maximum=2000, step=10, interactive=True)
 
     with gr.Row():
-        start_btn = gr.Button("Start training")
-        stop_btn = gr.Button("Abort")
+        start_btn = gr.Button()
+        stop_btn = gr.Button()
 
     with gr.Row():
         with gr.Column(scale=4):
-            output_dir = gr.Textbox(label="Checkpoint name", value=get_time(), interactive=True)
-            output_info = gr.Markdown(value="Ready")
+            output_dir = gr.Textbox(interactive=True)
+            output_box = gr.Markdown()
 
         with gr.Column(scale=1):
-            loss_viewer = gr.Plot(label="Loss")
+            loss_viewer = gr.Plot()
 
     start_btn.click(
         runner.run_train,
         [
-            model_name, model_path, checkpoints, output_dir, finetuning_type,
-            dataset, learning_rate, num_train_epochs, max_samples,
-            fp16, quantization_bit, per_device_train_batch_size, gradient_accumulation_steps,
-            lr_scheduler_type, logging_steps, save_steps
+            top_elems["lang"], top_elems["model_name"], top_elems["checkpoints"], top_elems["finetuning_type"],
+            dataset, dataset_dir, learning_rate, num_train_epochs, max_samples,
+            fp16, quantization_bit, batch_size, gradient_accumulation_steps,
+            lr_scheduler_type, logging_steps, save_steps, output_dir
         ],
-        output_info
+        [output_box]
     )
     stop_btn.click(runner.set_abort, queue=False)
 
-    output_info.change(gen_plot, [model_name, output_dir], loss_viewer, queue=False)
+    output_box.change(
+        gen_plot, [top_elems["model_name"], top_elems["finetuning_type"], output_dir], loss_viewer, queue=False
+    )
+
+    return dict(
+        dataset_dir=dataset_dir,
+        dataset=dataset,
+        preview_btn=preview_btn,
+        preview_count=preview_count,
+        preview_samples=preview_samples,
+        close_btn=close_btn,
+        learning_rate=learning_rate,
+        num_train_epochs=num_train_epochs,
+        max_samples=max_samples,
+        quantization_bit=quantization_bit,
+        batch_size=batch_size,
+        gradient_accumulation_steps=gradient_accumulation_steps,
+        lr_scheduler_type=lr_scheduler_type,
+        fp16=fp16,
+        logging_steps=logging_steps,
+        save_steps=save_steps,
+        start_btn=start_btn,
+        stop_btn=stop_btn,
+        output_dir=output_dir,
+        output_box=output_box,
+        loss_viewer=loss_viewer
+    )
```

### Comparing `glmtuner-0.1.1/src/glmtuner/webui/runner.py` & `glmtuner-0.1.2/src/glmtuner/webui/runner.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,97 +2,94 @@
 import os
 import threading
 import time
 import transformers
 from typing import Optional, Tuple
 
 from glmtuner.extras.callbacks import LogCallback
-from glmtuner.extras.constants import SUPPORTED_MODELS
 from glmtuner.extras.logging import LoggerHandler
 from glmtuner.extras.misc import torch_gc
 from glmtuner.tuner import get_train_args, run_sft
-from glmtuner.webui.common import get_save_dir, DATA_DIR
+from glmtuner.webui.common import get_model_path, get_save_dir
+from glmtuner.webui.locales import ALERTS
 from glmtuner.webui.utils import format_info, get_eval_results
 
 
 class Runner:
 
     def __init__(self):
         self.aborted = False
         self.running = False
 
     def set_abort(self):
         self.aborted = True
         self.running = False
 
-    def initialize(self, model_name: str, model_path: str, dataset: list) -> Tuple[str, str, LoggerHandler, LogCallback]:
+    def initialize(self, lang: str, model_name: str, dataset: list) -> Tuple[str, str, LoggerHandler, LogCallback]:
         if self.running:
-            return None, "A process is in running, please abort it firstly.", None, None
+            return None, ALERTS["err_conflict"][lang], None, None
 
         if not model_name:
-            return None, "Please select a model.", None, None
+            return None, ALERTS["err_no_model"][lang], None, None
 
-        if model_path:
-            if not os.path.isdir(model_path):
-                return None, "Cannot find model directory in local disk.", None, None
-            model_name_or_path = model_path
-        elif model_name in SUPPORTED_MODELS: # TODO: use list in gr.State
-            model_name_or_path = SUPPORTED_MODELS[model_name]["hf_path"]
-        else:
-            return None, "Invalid model.", None, None
+        model_name_or_path = get_model_path(model_name)
+        if not model_name_or_path:
+            return None, ALERTS["err_no_path"][lang], None, None
 
         if len(dataset) == 0:
-            return None, "Please choose datasets.", None, None
+            return None, ALERTS["err_no_dataset"][lang], None, None
 
         self.aborted = False
         self.running = True
 
         logger_handler = LoggerHandler()
         logger_handler.setLevel(logging.INFO)
         logging.root.addHandler(logger_handler)
         transformers.logging.add_handler(logger_handler)
         trainer_callback = LogCallback(self)
 
         return model_name_or_path, "", logger_handler, trainer_callback
 
-    def finalize(self, finish_info: Optional[str] = None) -> str:
+    def finalize(self, lang: str, finish_info: Optional[str] = None) -> str:
         self.running = False
         torch_gc()
         if self.aborted:
-            return "Ready"
+            return ALERTS["info_aborted"][lang]
         else:
-            return finish_info if finish_info is not None else "Finished"
+            return finish_info if finish_info is not None else ALERTS["info_finished"][lang]
 
     def run_train(
-        self, model_name, model_path, checkpoints, output_dir, finetuning_type,
-        dataset, learning_rate, num_train_epochs, max_samples,
-        fp16, quantization_bit, per_device_train_batch_size, gradient_accumulation_steps,
-        lr_scheduler_type, logging_steps, save_steps
+        self, lang, model_name, checkpoints, finetuning_type,
+        dataset, dataset_dir, learning_rate, num_train_epochs, max_samples,
+        fp16, quantization_bit, batch_size, gradient_accumulation_steps,
+        lr_scheduler_type, logging_steps, save_steps, output_dir
     ):
-        model_name_or_path, error, logger_handler, trainer_callback = self.initialize(model_name, model_path, dataset)
+        model_name_or_path, error, logger_handler, trainer_callback = self.initialize(lang, model_name, dataset)
         if error:
             yield error
             return
 
         if checkpoints:
-            checkpoint_dir = ",".join([os.path.join(get_save_dir(model_name), checkpoint) for checkpoint in checkpoints])
+            checkpoint_dir = ",".join(
+                [os.path.join(get_save_dir(model_name), finetuning_type, checkpoint) for checkpoint in checkpoints]
+            )
         else:
             checkpoint_dir = None
 
         args = dict(
             model_name_or_path=model_name_or_path,
             do_train=True,
             finetuning_type=finetuning_type,
             dataset=",".join(dataset),
-            dataset_dir=DATA_DIR,
+            dataset_dir=dataset_dir,
             max_samples=int(max_samples),
-            output_dir=os.path.join(get_save_dir(model_name), output_dir),
+            output_dir=os.path.join(get_save_dir(model_name), finetuning_type, output_dir),
             checkpoint_dir=checkpoint_dir,
             overwrite_cache=True,
-            per_device_train_batch_size=per_device_train_batch_size,
+            per_device_train_batch_size=batch_size,
             gradient_accumulation_steps=gradient_accumulation_steps,
             lr_scheduler_type=lr_scheduler_type,
             logging_steps=logging_steps,
             save_steps=save_steps,
             learning_rate=float(learning_rate),
             num_train_epochs=float(num_train_epochs),
             fp16=fp16,
@@ -109,49 +106,57 @@
         )
         thread = threading.Thread(target=run_sft, kwargs=run_args)
         thread.start()
 
         while thread.is_alive():
             time.sleep(1)
             if self.aborted:
-                yield "Aborted, wait for terminating..."
+                yield ALERTS["info_aborting"][lang]
             else:
                 yield format_info(logger_handler.log, trainer_callback.tracker)
 
-        yield self.finalize()
+        yield self.finalize(lang)
 
     def run_eval(
-        self, model_name, model_path, checkpoints, dataset, max_samples, per_device_eval_batch_size,
-        quantization_bit
+        self, lang, model_name, checkpoints, finetuning_type,
+        dataset, dataset_dir, max_samples, batch_size, quantization_bit, predict
     ):
-        model_name_or_path, error, logger_handler, trainer_callback = self.initialize(model_name, model_path, dataset)
+        model_name_or_path, error, logger_handler, trainer_callback = self.initialize(lang, model_name, dataset)
         if error:
             yield error
             return
 
         if checkpoints:
-            checkpoint_dir = ",".join([os.path.join(get_save_dir(model_name), checkpoint) for checkpoint in checkpoints])
-            output_dir = os.path.join(get_save_dir(model_name), "eval_" + "_".join(checkpoints))
+            checkpoint_dir = ",".join(
+                [os.path.join(get_save_dir(model_name), finetuning_type, checkpoint) for checkpoint in checkpoints]
+            )
+            output_dir = os.path.join(get_save_dir(model_name), finetuning_type, "eval_" + "_".join(checkpoints))
         else:
             checkpoint_dir = None
-            output_dir = os.path.join(get_save_dir(model_name), "eval_base")
+            output_dir = os.path.join(get_save_dir(model_name), finetuning_type, "eval_base")
 
         args = dict(
             model_name_or_path=model_name_or_path,
             do_eval=True,
+            finetuning_type=finetuning_type,
             dataset=",".join(dataset),
-            dataset_dir=DATA_DIR,
+            dataset_dir=dataset_dir,
             max_samples=int(max_samples),
             output_dir=output_dir,
             checkpoint_dir=checkpoint_dir,
             overwrite_cache=True,
             predict_with_generate=True,
-            per_device_eval_batch_size=per_device_eval_batch_size,
+            per_device_eval_batch_size=batch_size,
             quantization_bit=int(quantization_bit) if quantization_bit else None
         )
+
+        if predict:
+            args.pop("do_eval", None)
+            args["do_predict"] = True
+
         model_args, data_args, training_args, finetuning_args, _ = get_train_args(args)
 
         run_args = dict(
             model_args=model_args,
             data_args=data_args,
             training_args=training_args,
             finetuning_args=finetuning_args,
@@ -159,12 +164,12 @@
         )
         thread = threading.Thread(target=run_sft, kwargs=run_args)
         thread.start()
 
         while thread.is_alive():
             time.sleep(1)
             if self.aborted:
-                yield "Aborted, wait for terminating..."
+                yield ALERTS["info_aborting"][lang]
             else:
                 yield format_info(logger_handler.log, trainer_callback.tracker)
 
-        yield self.finalize(get_eval_results(os.path.join(output_dir, "eval_results.json")))
+        yield self.finalize(lang, get_eval_results(os.path.join(output_dir, "eval_results.json")))
```

### Comparing `glmtuner-0.1.1/src/glmtuner/webui/utils.py` & `glmtuner-0.1.2/src/glmtuner/webui/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,63 +1,62 @@
-import json
 import os
-from datetime import datetime
-from typing import Tuple
-
+import json
 import gradio as gr
 import matplotlib.figure
 import matplotlib.pyplot as plt
+from typing import Tuple
+from datetime import datetime
 
 from glmtuner.extras.ploting import smooth
-from glmtuner.webui.common import get_save_dir, DATA_DIR
+from glmtuner.webui.common import get_save_dir, DATA_CONFIG
 
 
 def format_info(log: str, tracker: dict) -> str:
     info = log
     if "current_steps" in tracker:
-        info += "Running **{:d}/{:d}**: {} < {}".format(
+        info += "Running **{:d}/{:d}**: {} < {}\n".format(
             tracker["current_steps"], tracker["total_steps"], tracker["elapsed_time"], tracker["remaining_time"]
         )
     return info
 
 
 def get_time() -> str:
     return datetime.now().strftime('%Y-%m-%d-%H-%M-%S')
 
 
-def can_preview(dataset: list) -> dict:
-    with open(os.path.join(DATA_DIR, "dataset_info.json"), "r", encoding="utf-8") as f:
+def can_preview(dataset_dir: str, dataset: list) -> dict:
+    with open(os.path.join(dataset_dir, DATA_CONFIG), "r", encoding="utf-8") as f:
         dataset_info = json.load(f)
     if (
         len(dataset) > 0
         and "file_name" in dataset_info[dataset[0]]
-        and os.path.isfile(os.path.join(DATA_DIR, dataset_info[dataset[0]]["file_name"]))
+        and os.path.isfile(os.path.join(dataset_dir, dataset_info[dataset[0]]["file_name"]))
     ):
         return gr.update(interactive=True)
     else:
         return gr.update(interactive=False)
 
 
-def get_preview(dataset: list) -> Tuple[int, list]:
-    with open(os.path.join(DATA_DIR, "dataset_info.json"), "r", encoding="utf-8") as f:
+def get_preview(dataset_dir: str, dataset: list) -> Tuple[int, list, dict]:
+    with open(os.path.join(dataset_dir, DATA_CONFIG), "r", encoding="utf-8") as f:
         dataset_info = json.load(f)
     data_file = dataset_info[dataset[0]]["file_name"]
-    with open(os.path.join(DATA_DIR, data_file), "r", encoding="utf-8") as f:
+    with open(os.path.join(dataset_dir, data_file), "r", encoding="utf-8") as f:
         data = json.load(f)
-    return len(data), data[:2]
+    return len(data), data[:2], gr.update(visible=True)
 
 
 def get_eval_results(path: os.PathLike) -> str:
     with open(path, "r", encoding="utf-8") as f:
         result = json.dumps(json.load(f), indent=4)
     return "```json\n{}\n```\n".format(result)
 
 
-def gen_plot(base_model: str, output_dir: str) -> matplotlib.figure.Figure:
-    log_file = os.path.join(get_save_dir(base_model), output_dir, "trainer_log.jsonl")
+def gen_plot(base_model: str, finetuning_type: str, output_dir: str) -> matplotlib.figure.Figure:
+    log_file = os.path.join(get_save_dir(base_model), finetuning_type, output_dir, "trainer_log.jsonl")
     if not os.path.isfile(log_file):
         return None
 
     plt.close("all")
     fig = plt.figure()
     ax = fig.add_subplot(111)
     steps, losses = [], []
```

### Comparing `glmtuner-0.1.1/src/glmtuner.egg-info/PKG-INFO` & `glmtuner-0.1.2/src/glmtuner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glmtuner
-Version: 0.1.1
+Version: 0.1.2
 Summary: Fine-tuning ChatGLM-6B with PEFT
 Home-page: https://github.com/hiyouga/ChatGLM-Efficient-Tuning
 Author: hiyouga
 Author-email: hiyouga@buaa.edu.cn
 License: Apache 2.0 License
 Keywords: ChatGLM,LLM,ChatGPT,transformer,pytorch,deep learning
 Classifier: Development Status :: 3 - Alpha
@@ -275,15 +275,14 @@
 | LoRA (r=8)       |     4      | FP16 |  20GB  | 8ex/s |
 | LoRA (r=8)       |     4      | INT8 |  10GB  | 8ex/s |
 | LoRA (r=8)       |     4      | INT4 |   8GB  | 8ex/s |
 | P-Tuning (p=16)  |     4      | FP16 |  20GB  | 8ex/s |
 | P-Tuning (p=16)  |     4      | INT8 |  16GB  | 8ex/s |
 | P-Tuning (p=16)  |     4      | INT4 |  12GB  | 8ex/s |
 | Freeze (l=3)     |     4      | FP16 |  24GB  | 8ex/s |
-| Freeze (l=3)     |     4      | INT8 |  12GB  | 8ex/s |
 
 | RM  method       | Batch size | Mode |  GRAM  | Speed |
 | ---------------- | ---------- | ---- | ------ | ----- |
 | LoRA (r=8) + rm  |     4      | FP16 |  22GB  | -     |
 | LoRA (r=8) + rm  |     1      | INT8 |  11GB  | -     |
 
 | RLHF method      | Batch size | Mode |  GRAM  | Speed |
```

### Comparing `glmtuner-0.1.1/src/glmtuner.egg-info/SOURCES.txt` & `glmtuner-0.1.2/src/glmtuner.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,18 @@
 src/glmtuner/tuner/sft/trainer.py
 src/glmtuner/tuner/sft/workflow.py
 src/glmtuner/webui/__init__.py
 src/glmtuner/webui/chat.py
 src/glmtuner/webui/common.py
 src/glmtuner/webui/css.py
 src/glmtuner/webui/interface.py
+src/glmtuner/webui/locales.py
+src/glmtuner/webui/manager.py
 src/glmtuner/webui/runner.py
 src/glmtuner/webui/utils.py
 src/glmtuner/webui/components/__init__.py
+src/glmtuner/webui/components/chatbot.py
 src/glmtuner/webui/components/data.py
 src/glmtuner/webui/components/eval.py
 src/glmtuner/webui/components/infer.py
-src/glmtuner/webui/components/model.py
-src/glmtuner/webui/components/sft.py
+src/glmtuner/webui/components/sft.py
+src/glmtuner/webui/components/top.py
```

